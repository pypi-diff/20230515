# Comparing `tmp/aepp-0.2.8.tar.gz` & `tmp/aepp-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aepp-0.2.8.tar", last modified: Sun Mar 12 19:34:49 2023, max compression
+gzip compressed data, was "aepp-0.2.9.tar", last modified: Tue Apr  4 09:30:10 2023, max compression
```

## Comparing `aepp-0.2.8.tar` & `aepp-0.2.9.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-03-12 19:34:49.083621 aepp-0.2.8/
--rw-rw-rw-   0        0        0    10337 2021-10-20 19:48:57.000000 aepp-0.2.8/LICENSE
--rw-rw-rw-   0        0        0       16 2021-10-20 19:48:57.000000 aepp-0.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0     3852 2023-03-12 19:34:49.082624 aepp-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     3189 2023-01-11 08:15:57.000000 aepp-0.2.8/README.md
-drwxrwxrwx   0        0        0        0 2023-03-12 19:34:49.040737 aepp-0.2.8/aepp/
--rw-rw-rw-   0        0        0     4601 2022-11-04 20:05:49.000000 aepp-0.2.8/aepp/__init__.py
--rw-rw-rw-   0        0        0       21 2023-03-12 19:07:29.000000 aepp-0.2.8/aepp/__version__.py
--rw-rw-rw-   0        0        0     4272 2023-02-04 09:19:40.000000 aepp-0.2.8/aepp/accesscontrol.py
--rw-rw-rw-   0        0        0    32652 2023-03-12 19:31:31.000000 aepp-0.2.8/aepp/catalog.py
--rw-rw-rw-   0        0        0     1766 2023-03-12 19:07:29.000000 aepp-0.2.8/aepp/config.py
--rw-rw-rw-   0        0        0    12808 2023-03-12 19:07:29.000000 aepp-0.2.8/aepp/configs.py
--rw-rw-rw-   0        0        0    23066 2023-03-12 19:07:29.000000 aepp-0.2.8/aepp/connector.py
--rw-rw-rw-   0        0        0    37405 2023-02-04 09:20:35.000000 aepp-0.2.8/aepp/customerprofile.py
--rw-rw-rw-   0        0        0    13212 2023-02-04 09:22:21.000000 aepp-0.2.8/aepp/dataaccess.py
--rw-rw-rw-   0        0        0    26369 2023-02-04 09:24:20.000000 aepp-0.2.8/aepp/dataprep.py
--rw-rw-rw-   0        0        0     7742 2023-03-12 19:07:12.000000 aepp-0.2.8/aepp/datasets.py
--rw-rw-rw-   0        0        0    23348 2023-02-04 09:31:59.000000 aepp-0.2.8/aepp/destination.py
--rw-rw-rw-   0        0        0    68559 2023-02-23 08:41:11.000000 aepp-0.2.8/aepp/flowservice.py
--rw-rw-rw-   0        0        0    18994 2023-02-04 09:30:09.000000 aepp-0.2.8/aepp/identity.py
--rw-rw-rw-   0        0        0    20359 2023-03-12 19:25:32.000000 aepp-0.2.8/aepp/ingestion.py
--rw-rw-rw-   0        0        0     8905 2023-02-04 09:35:43.000000 aepp-0.2.8/aepp/observability.py
--rw-rw-rw-   0        0        0    15229 2023-02-04 09:37:12.000000 aepp-0.2.8/aepp/policy.py
--rw-rw-rw-   0        0        0     7746 2023-02-04 09:39:18.000000 aepp-0.2.8/aepp/privacyservice.py
--rw-rw-rw-   0        0        0    51377 2023-02-09 17:51:38.000000 aepp-0.2.8/aepp/queryservice.py
--rw-rw-rw-   0        0        0     7186 2023-03-12 19:07:29.000000 aepp-0.2.8/aepp/sandboxes.py
--rw-rw-rw-   0        0        0   143778 2023-03-12 19:07:12.000000 aepp-0.2.8/aepp/schema.py
--rw-rw-rw-   0        0        0    37429 2023-02-04 09:44:52.000000 aepp-0.2.8/aepp/segmentation.py
--rw-rw-rw-   0        0        0     7145 2023-02-04 09:46:19.000000 aepp-0.2.8/aepp/sensei.py
-drwxrwxrwx   0        0        0        0 2023-03-12 19:34:49.057692 aepp-0.2.8/aepp.egg-info/
--rw-rw-rw-   0        0        0     3852 2023-03-12 19:34:48.000000 aepp-0.2.8/aepp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      738 2023-03-12 19:34:48.000000 aepp-0.2.8/aepp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-12 19:34:48.000000 aepp-0.2.8/aepp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-03-12 19:34:48.000000 aepp-0.2.8/aepp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-03-12 19:34:48.000000 aepp-0.2.8/aepp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-12 19:34:49.084619 aepp-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1584 2022-11-15 13:03:17.000000 aepp-0.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-12 19:34:49.079633 aepp-0.2.8/tests/
--rw-rw-rw-   0        0        0        0 2023-03-12 19:07:12.000000 aepp-0.2.8/tests/__init__.py
--rw-rw-rw-   0        0        0     1623 2023-03-12 19:07:12.000000 aepp-0.2.8/tests/catalog_test.py
--rw-rw-rw-   0        0        0      615 2023-03-12 19:07:12.000000 aepp-0.2.8/tests/dataaccess_test.py
--rw-rw-rw-   0        0        0      470 2023-03-12 19:07:12.000000 aepp-0.2.8/tests/datasets_test.py
--rw-rw-rw-   0        0        0     3585 2023-03-12 19:07:12.000000 aepp-0.2.8/tests/flowservice_test.py
--rw-rw-rw-   0        0        0     2151 2023-03-12 19:07:12.000000 aepp-0.2.8/tests/schema_test.py
+drwxrwxrwx   0        0        0        0 2023-04-04 09:30:10.865281 aepp-0.2.9/
+-rw-rw-rw-   0        0        0    10337 2021-10-20 19:48:57.000000 aepp-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0       16 2021-10-20 19:48:57.000000 aepp-0.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     3916 2023-04-04 09:30:10.864284 aepp-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3253 2023-04-04 08:33:58.000000 aepp-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-04 09:30:10.822395 aepp-0.2.9/aepp/
+-rw-rw-rw-   0        0        0     4601 2022-11-04 20:05:49.000000 aepp-0.2.9/aepp/__init__.py
+-rw-rw-rw-   0        0        0       21 2023-04-04 08:48:21.000000 aepp-0.2.9/aepp/__version__.py
+-rw-rw-rw-   0        0        0     4272 2023-02-04 09:19:40.000000 aepp-0.2.9/aepp/accesscontrol.py
+-rw-rw-rw-   0        0        0    33405 2023-04-04 08:52:22.000000 aepp-0.2.9/aepp/catalog.py
+-rw-rw-rw-   0        0        0     1836 2023-04-04 08:33:58.000000 aepp-0.2.9/aepp/config.py
+-rw-rw-rw-   0        0        0    12808 2023-03-12 19:07:29.000000 aepp-0.2.9/aepp/configs.py
+-rw-rw-rw-   0        0        0    23296 2023-04-04 08:43:31.000000 aepp-0.2.9/aepp/connector.py
+-rw-rw-rw-   0        0        0    37405 2023-02-04 09:20:35.000000 aepp-0.2.9/aepp/customerprofile.py
+-rw-rw-rw-   0        0        0    13212 2023-02-04 09:22:21.000000 aepp-0.2.9/aepp/dataaccess.py
+-rw-rw-rw-   0        0        0    26369 2023-02-04 09:24:20.000000 aepp-0.2.9/aepp/dataprep.py
+-rw-rw-rw-   0        0        0     7742 2023-03-12 19:07:12.000000 aepp-0.2.9/aepp/datasets.py
+-rw-rw-rw-   0        0        0    23348 2023-02-04 09:31:59.000000 aepp-0.2.9/aepp/destination.py
+-rw-rw-rw-   0        0        0     4251 2023-04-04 08:33:58.000000 aepp-0.2.9/aepp/destinationinstanceservice.py
+-rw-rw-rw-   0        0        0    71154 2023-04-04 08:47:18.000000 aepp-0.2.9/aepp/flowservice.py
+-rw-rw-rw-   0        0        0    18994 2023-02-04 09:30:09.000000 aepp-0.2.9/aepp/identity.py
+-rw-rw-rw-   0        0        0    20359 2023-03-12 19:25:32.000000 aepp-0.2.9/aepp/ingestion.py
+-rw-rw-rw-   0        0        0     8905 2023-02-04 09:35:43.000000 aepp-0.2.9/aepp/observability.py
+-rw-rw-rw-   0        0        0    15229 2023-02-04 09:37:12.000000 aepp-0.2.9/aepp/policy.py
+-rw-rw-rw-   0        0        0     7746 2023-02-04 09:39:18.000000 aepp-0.2.9/aepp/privacyservice.py
+-rw-rw-rw-   0        0        0    51377 2023-02-09 17:51:38.000000 aepp-0.2.9/aepp/queryservice.py
+-rw-rw-rw-   0        0        0     7186 2023-03-12 19:07:29.000000 aepp-0.2.9/aepp/sandboxes.py
+-rw-rw-rw-   0        0        0   144959 2023-04-04 09:26:16.000000 aepp-0.2.9/aepp/schema.py
+-rw-rw-rw-   0        0        0    37429 2023-02-04 09:44:52.000000 aepp-0.2.9/aepp/segmentation.py
+-rw-rw-rw-   0        0        0     7145 2023-02-04 09:46:19.000000 aepp-0.2.9/aepp/sensei.py
+drwxrwxrwx   0        0        0        0 2023-04-04 09:30:10.838353 aepp-0.2.9/aepp.egg-info/
+-rw-rw-rw-   0        0        0     3916 2023-04-04 09:30:10.000000 aepp-0.2.9/aepp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      814 2023-04-04 09:30:10.000000 aepp-0.2.9/aepp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-04 09:30:10.000000 aepp-0.2.9/aepp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-04-04 09:30:10.000000 aepp-0.2.9/aepp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-04 09:30:10.000000 aepp-0.2.9/aepp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-04 09:30:10.866278 aepp-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1584 2022-11-15 13:03:17.000000 aepp-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-04 09:30:10.860294 aepp-0.2.9/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-12 19:07:12.000000 aepp-0.2.9/tests/__init__.py
+-rw-rw-rw-   0        0        0     1623 2023-03-12 19:07:12.000000 aepp-0.2.9/tests/catalog_test.py
+-rw-rw-rw-   0        0        0      615 2023-03-12 19:07:12.000000 aepp-0.2.9/tests/dataaccess_test.py
+-rw-rw-rw-   0        0        0      470 2023-03-12 19:07:12.000000 aepp-0.2.9/tests/datasets_test.py
+-rw-rw-rw-   0        0        0     1482 2023-04-04 08:33:58.000000 aepp-0.2.9/tests/destinationinstanceservice_test.py
+-rw-rw-rw-   0        0        0     3585 2023-03-12 19:07:12.000000 aepp-0.2.9/tests/flowservice_test.py
+-rw-rw-rw-   0        0        0     2151 2023-03-12 19:07:12.000000 aepp-0.2.9/tests/schema_test.py
```

### Comparing `aepp-0.2.8/LICENSE` & `aepp-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aepp-0.2.8/PKG-INFO` & `aepp-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aepp
-Version: 0.2.8
+Version: 0.2.9
 Summary: Package to manage AEP API endpoint and some helper functions
 Home-page: https://github.com/pitchmuc/aep
 Author: Julien Piccini
 Author-email: piccini.julien@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -69,14 +69,15 @@
 * [segmentation](./docs/segmentation.md)
 * [dataprep](./docs/dataprep.md)
 * [flowservice](./docs/flowservice.md)
 * [policy](./docs/policy.md)
 * [datasets](./docs/datasets.md)
 * [ingestion](./docs/ingestion.md)
 * [destination Authoring](./docs/destination.md)
+* [destination Instance](./docs/destinationinstanceservice.md)
 * [observability](./docs/observability.md)
 * accesscontrol
 * sensei
 * [privacyservice](./docs/privacyservice.md) (see 2nd note below)
 
 Last but not least, the core methods are described here: [main](./docs/main.md)
```

### Comparing `aepp-0.2.8/README.md` & `aepp-0.2.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 * [segmentation](./docs/segmentation.md)
 * [dataprep](./docs/dataprep.md)
 * [flowservice](./docs/flowservice.md)
 * [policy](./docs/policy.md)
 * [datasets](./docs/datasets.md)
 * [ingestion](./docs/ingestion.md)
 * [destination Authoring](./docs/destination.md)
+* [destination Instance](./docs/destinationinstanceservice.md)
 * [observability](./docs/observability.md)
 * accesscontrol
 * sensei
 * [privacyservice](./docs/privacyservice.md) (see 2nd note below)
 
 Last but not least, the core methods are described here: [main](./docs/main.md)
```

### Comparing `aepp-0.2.8/aepp/__init__.py` & `aepp-0.2.9/aepp/__init__.py`

 * *Files identical despite different names*

### Comparing `aepp-0.2.8/aepp/accesscontrol.py` & `aepp-0.2.9/aepp/accesscontrol.py`

 * *Files identical despite different names*

### Comparing `aepp-0.2.8/aepp/catalog.py` & `aepp-0.2.9/aepp/catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -415,14 +415,30 @@
             raise Exception("Expected a datasetId argument")
         if self.loggingEnabled:
             self.logger.debug(f"Starting getDataset for : {datasetId}")
         path = f"/dataSets/{datasetId}"
         res = self.connector.getData(self.endpoint+path, headers=self.header)
         return res
 
+    def getDataSetObservableSchema(self, datasetId: str = None):
+        """
+        Return a single dataset observable schema.
+        Which means that the fields that has been used in that dataset.
+        Arguments:
+            datasetId : REQUIRED : Id of the dataset for which the observable schema should be retrieved.
+        """
+        if datasetId is None:
+            raise Exception("Expected a datasetId argument")
+        if self.loggingEnabled:
+            self.logger.debug(f"Starting getDataset for : {datasetId}")
+        path = f"/dataSets/{datasetId}"
+        params = {"properties" : "observableSchema"}
+        res = self.connector.getData(self.endpoint+path,params=params, headers=self.header)
+        return res
+
     def deleteDataSet(self, datasetId: str = None):
         """
         Delete a dataset by its id.
         Arguments:
             datasetId : REQUIRED : Id of the dataset to be deleted.
         """
         if datasetId is None:
```

### Comparing `aepp-0.2.8/aepp/config.py` & `aepp-0.2.9/aepp/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,13 +43,14 @@
     "dataaccess": "/data/foundation/export",
     "mapping": "/data/foundation/conversion",
     "policy": "/data/foundation/dulepolicy",
     "dataset": "/data/foundation/dataset",
     "ingestion": "/data/foundation/import",
     "observability": "/data/infrastructure/observability/insights",
     "destinationAuthoring": "/data/core/activation/authoring",
+    "destinationInstance" : "/data/core/activation/disflowprovider",
     "streaming": {
         "inlet": "",
         "collection": "https://dcs.adobedc.net"
     },
     "audit": "/data/foundation"
 }
```

### Comparing `aepp-0.2.8/aepp/configs.py` & `aepp-0.2.9/aepp/configs.py`

 * *Files identical despite different names*

### Comparing `aepp-0.2.8/aepp/connector.py` & `aepp-0.2.9/aepp/connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -335,14 +335,18 @@
                         self.logger.error(
                             f"GET method failed: {res.status_code}, {res['errorMessage']}"
                         )
                     print(f"status code : {res.status_code}")
                     print(f"error message : {res['errorMessage']}")
         except:
             pass
+        ## returning some errors in the console
+        if type(res_json) == dict:
+            if 'status' in res_json.keys() and 'report' in res_json.keys():
+                self.logger.warning(json.dumps(res_json,indent=2))
         return res_json
 
     def headData(
         self, endpoint: str, params: dict = None, headers: dict = None, *args, **kwargs
     ):
         """
         Abstraction for the head method.
```

### Comparing `aepp-0.2.8/aepp/customerprofile.py` & `aepp-0.2.9/aepp/customerprofile.py`

 * *Files identical despite different names*

### Comparing `aepp-0.2.8/aepp/dataaccess.py` & `aepp-0.2.9/aepp/dataaccess.py`

 * *Files identical despite different names*

### Comparing `aepp-0.2.8/aepp/dataprep.py` & `aepp-0.2.9/aepp/dataprep.py`

 * *Files identical despite different names*

### Comparing `aepp-0.2.8/aepp/datasets.py` & `aepp-0.2.9/aepp/datasets.py`

 * *Files identical despite different names*

### Comparing `aepp-0.2.8/aepp/destination.py` & `aepp-0.2.9/aepp/destination.py`

 * *Files identical despite different names*

### Comparing `aepp-0.2.8/aepp/flowservice.py` & `aepp-0.2.9/aepp/flowservice.py`

 * *Files 2% similar despite different names*

```diff
@@ -748,15 +748,15 @@
         path = "/runs"
         params = {"limit": limit, "count": kwargs.get("count", False)}
         if prop is not None:
             params["property"] = prop
         if kwargs.get("continuationToken", False):
             params["continuationToken"] = kwargs.get("continuationToken")
         res: dict = self.connector.getData(self.endpoint + path, params=params)
-        items: list = res["items"]
+        items: list = res.get("items",[])
         nextPage = res["_links"].get("next", {}).get("href", "")
         while nextPage != "" and len(items) < float(n_results):
             token: str = res["_links"]["next"].get("href", "")
             continuationToken: str = token.split("=")[1]
             params["continuationToken"] = continuationToken
             res = self.connector.getData(self.endpoint + path, params=params)
             items += res.get('items')
@@ -1238,36 +1238,101 @@
                 }
 
             }
         ]
         res = self.updateFlow(flowId=flowId, operation=op)
         return res
     
-    def getLandingZoneContainer(self)->dict:
+    def getLandingZoneContainer(
+        self,
+        dlz_type: str = "user_drop_zone"
+    ) -> dict:
         """
-        Returns a dictionary of the your available Data Landing Zone containers.
+        Returns a dictionary of the available Data Landing Zone container information.
+        Arguments:
+            dlz_type : OPTIONAL : The type of DLZ container - default to "user_drop_zone" but can be "dlz_destination"
         """
         if self.loggingEnabled:
             self.logger.debug(f"Starting getLandingZoneContainer")
         path = f"/data/foundation/connectors/landingzone"
-        params = {"type":"user_drop_zone"}
-        res = self.connector.getData(self.endpoint_gloal + path,params=params)
+        params = {"type": dlz_type}
+        res = self.connector.getData(self.endpoint_gloal + path, params=params)
         return res
+
+    def getLandingZoneContainerName(
+        self,
+        dlz_type: str = "user_drop_zone"
+    ) -> str:
+        """
+        Returns the name of the DLZ container corresponding to this type.
+        Arguments:
+            dlz_type : OPTIONAL : The type of DLZ container - default to "user_drop_zone" but can be "dlz_destination"
+        """
+        return self.getLandingZoneContainer(dlz_type=dlz_type)["containerName"]
+
+    def getLandingZoneContainerTTL(
+        self,
+        dlz_type: str = "user_drop_zone"
+    ) -> int:
+        """
+        Returns the TTL in days of the DLZ container corresponding to this type.
+        Arguments:
+            dlz_type : OPTIONAL : The type of DLZ container - default to "user_drop_zone" but can be "dlz_destination"
+        """
+        return int(self.getLandingZoneContainer(dlz_type=dlz_type)["containerTTL"])
     
-    def getLandingZoneCredential(self)->dict:
+    def getLandingZoneCredential(
+        self,
+        dlz_type: str = "user_drop_zone"
+    ) -> dict:
         """
         Returns a dictionary with the credential to be used in order to create a new zone
+        Arguments:
+            dlz_type : OPTIONAL : The type of DLZ container - default to "user_drop_zone" but can be "dlz_destination"
         """
         if self.loggingEnabled:
             self.logger.debug(f"Starting getLandingZoneCredential")
         path = f"/data/foundation/connectors/landingzone/credentials"
-        params = {"type":"user_drop_zone"}
+        params = {"type": dlz_type}
         res = self.connector.getData(self.endpoint_gloal + path,params=params)
         return res
 
+    def getLandingZoneSASUri(
+        self,
+        dlz_type: str = "user_drop_zone"
+    ) -> str:
+        """
+        Returns the SAS URI of the DLZ container corresponding to this type.
+        Arguments:
+            dlz_type : OPTIONAL : The type of DLZ container - default to "user_drop_zone" but can be "dlz_destination"
+        """
+        return self.getLandingZoneCredential(dlz_type=dlz_type)["SASUri"]
+
+    def getLandingZoneSASToken(
+        self,
+        dlz_type: str = "user_drop_zone"
+    ) -> str:
+        """
+        Returns the SAS token of the DLZ container corresponding to this type.
+        Arguments:
+            dlz_type : OPTIONAL : The type of DLZ container - default to "user_drop_zone" but can be "dlz_destination"
+        """
+        return self.getLandingZoneCredential(dlz_type=dlz_type)["SASToken"]
+
+    def getLandingZoneStorageAccountName(
+        self,
+        dlz_type: str = "user_drop_zone"
+    ) -> str:
+        """
+        Returns the storage account name of the DLZ container corresponding to this type.
+        Arguments:
+            dlz_type : OPTIONAL : The type of DLZ container - default to "user_drop_zone" but can be "dlz_destination"
+        """
+        return self.getLandingZoneCredential(dlz_type=dlz_type)["storageAccountName"]
+
     def exploreLandingZone(self,fileType:str='delimited')->list:
         """
         Return the structure of your landing zones
         Arguments:
             fileType : OPTIONAL : The type of the file to see.
         """
         path ="/connectionSpecs/26f526f2-58f4-4712-961d-e41bf1ccc0e8/explore"
```

### Comparing `aepp-0.2.8/aepp/identity.py` & `aepp-0.2.9/aepp/identity.py`

 * *Files identical despite different names*

### Comparing `aepp-0.2.8/aepp/ingestion.py` & `aepp-0.2.9/aepp/ingestion.py`

 * *Files identical despite different names*

### Comparing `aepp-0.2.8/aepp/observability.py` & `aepp-0.2.9/aepp/observability.py`

 * *Files identical despite different names*

### Comparing `aepp-0.2.8/aepp/policy.py` & `aepp-0.2.9/aepp/policy.py`

 * *Files identical despite different names*

### Comparing `aepp-0.2.8/aepp/privacyservice.py` & `aepp-0.2.9/aepp/privacyservice.py`

 * *Files identical despite different names*

### Comparing `aepp-0.2.8/aepp/queryservice.py` & `aepp-0.2.9/aepp/queryservice.py`

 * *Files identical despite different names*

### Comparing `aepp-0.2.8/aepp/sandboxes.py` & `aepp-0.2.9/aepp/sandboxes.py`

 * *Files identical despite different names*

### Comparing `aepp-0.2.8/aepp/schema.py` & `aepp-0.2.9/aepp/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -256,15 +256,17 @@
         privateHeader["Accept"] = f"application/vnd.adobe.{format}+json"
         res = self.connector.getData(
             self.endpoint + path, params=params, headers=privateHeader, verbose=verbose
         )
         if kwargs.get("debug", False):
             if "results" not in res.keys():
                 print(res)
-        data = res["results"]
+        data = res.get("results",[])
+        if len(data) == 0:
+            return res
         page = res.get("_page",{})
         nextPage = page.get('next',None)
         while nextPage is not None:
             params['start'] = nextPage
             res = self.connector.getData(
             self.endpoint + path, params=params, headers=privateHeader, verbose=verbose
             )
@@ -2272,27 +2274,31 @@
                 else:
                     if typed:
                         dictionary[key] = mydict[key].get('type','object')
                     else:
                         dictionary[key] = ""
         return dictionary 
 
-    def __transformationDF__(self,mydict:dict=None,dictionary:dict=None,path:str=None,queryPath:bool=False)->dict:
+    def __transformationDF__(self,mydict:dict=None,dictionary:dict=None,path:str=None,queryPath:bool=False,description:bool=False,xdmType:bool=False)->dict:
         """
         Transform the current XDM schema to a dictionary.
         Arguments:
             mydict : the fieldgroup
             dictionary : the dictionary that gather the paths
             path : path that is currently being developed
             queryPath: boolean to tell if we want to add the query path
+            description : boolean to tell if you want to retrieve the description
+            xdmType : boolean to know if you want to retrieve the xdm Type
         """
         if dictionary is None:
             dictionary = {'path':[],'type':[]}
             if queryPath:
-                 dictionary['querypath'] = []
+                dictionary['querypath'] = []
+            if description:
+                dictionary['description'] = []
         else:
             dictionary = dictionary
         for key in mydict:
             if type(mydict[key]) == dict:
                 if mydict[key].get('type') == 'object':
                     if path is None:
                         if key != "property" and key != "customFields":
@@ -2302,44 +2308,53 @@
                     else:
                         tmp_path = f"{path}.{key}"
                     if tmp_path is not None:
                         dictionary["path"].append(tmp_path)
                         dictionary["type"].append(f"{mydict[key].get('type')}")
                         if queryPath:
                             dictionary["querypath"].append(self.__cleanPath__(tmp_path))
+                        if description:
+                            dictionary["description"].append(f"{mydict[key].get('description','')}")
                     properties = mydict[key].get('properties',None)
                     if properties is not None:
-                        self.__transformationDF__(properties,dictionary,tmp_path,queryPath)
+                        self.__transformationDF__(properties,dictionary,tmp_path,queryPath,description)
                 elif mydict[key].get('type') == 'array':
                     levelProperties = mydict[key]['items'].get('properties',None)
                     if levelProperties is not None:
                         if path is None:
                             tmp_path = key
                         else :
                             tmp_path = f"{path}.{key}[]{{}}"
                         dictionary["path"].append(tmp_path)
                         dictionary["type"].append(f"[{mydict[key]['items'].get('type')}]")
                         if queryPath and tmp_path is not None:
                             dictionary["querypath"].append(self.__cleanPath__(tmp_path))
-                        self.__transformationDF__(levelProperties,dictionary,tmp_path,queryPath)
+                        if description and tmp_path is not None:
+                            dictionary["description"].append(mydict[key]['items'].get('description',''))
+                        self.__transformationDF__(levelProperties,dictionary,tmp_path,queryPath,description)
                     else:
                         finalpath = f"{path}.{key}"
                         dictionary["path"].append(finalpath)
                         dictionary["type"].append(f"[{mydict[key]['items'].get('type')}]")
                         if queryPath and finalpath is not None:
                             dictionary["querypath"].append(self.__cleanPath__(finalpath))
+                        if description and finalpath is not None:
+                            dictionary["description"].append(mydict[key]['items'].get('description',''))
                 else:
                     if path is not None:
                         finalpath = f"{path}.{key}"
                     else:
                         finalpath = f"{key}"
                     dictionary["path"].append(finalpath)
                     dictionary["type"].append(mydict[key].get('type','object'))
                     if queryPath and finalpath is not None:
                         dictionary["querypath"].append(self.__cleanPath__(finalpath))
+                    if description and finalpath is not None:
+                        dictionary["description"].append(mydict[key].get('description',''))
+
         return dictionary
     
     def __setField__(self,completePathList:list=None,fieldGroup:dict=None,newField:str=None,obj:dict=None)->dict:
         """
         Create a field with the attribute provided
         Arguments:
             completePathList : list of path to use for creation of the field.
@@ -2679,24 +2694,25 @@
         definition = self.fieldGroup.get('definitions',self.fieldGroup.get('properties',{}))
         data = self.__transformationDict__(definition,typed)
         if save:
             filename = self.fieldGroup.get('title',f'unknown_fieldGroup_{str(int(time.time()))}')
             aepp.saveFile(module='schema',file=data,filename=f"{filename}.json",type_file='json')
         return data
 
-    def to_dataframe(self,save:bool=False,queryPath:bool=False)->pd.DataFrame:
+    def to_dataframe(self,save:bool=False,queryPath:bool=False,description:bool=False)->pd.DataFrame:
         """
         Generate a dataframe with the row representing each possible path.
         Arguments:
             save : OPTIONAL : If you wish to save it with the title used by the field group.
                 save as csv with the title used. Not title, used "unknown_fieldGroup_" + timestamp.
             queryPath : OPTIONAL : If you want to have the query path to be used.
+            description : OPTIONAL : If you want to have the description used
         """
         definition = self.fieldGroup.get('definitions',self.fieldGroup.get('properties',{}))
-        data = self.__transformationDF__(definition,queryPath=queryPath)
+        data = self.__transformationDF__(definition,queryPath=queryPath,description=description)
         df = pd.DataFrame(data)
         if save:
             title = self.fieldGroup.get('title',f'unknown_fieldGroup_{str(int(time.time()))}')
             df.to_csv(f"{title}.csv",index=False)
         return df
     
     def to_xdm(self)->dict:
@@ -2967,25 +2983,25 @@
         Arguments:
             name : REQUIRED : a string to be used for the title of the FieldGroup
         """
         self.schema['title'] = name
         self.title = name
         return None
 
-    def to_dataframe(self,save:bool=False,queryPath: bool = False)->pd.DataFrame:
+    def to_dataframe(self,save:bool=False,queryPath: bool = False,description:bool = False)->pd.DataFrame:
         """
         Extract the information from the Field Group to DataFrame. You need to have instanciated the Field Group manager.
         Arguments:
             save : OPTIONAL : If you wish to save it with the title used by the field group.
                 save as csv with the title used. Not title, used "unknown_schema_" + timestamp.
             queryPath : OPTIONAL : If you want to have the query path to be used.
         """
         df = pd.DataFrame({'path':[],'type':[],'fieldGroup':[]})
         for fgmanager in self.fieldGroupsManagers:
-            tmp_df = fgmanager.to_dataframe(queryPath=queryPath)
+            tmp_df = fgmanager.to_dataframe(queryPath=queryPath,description=description)
             tmp_df['fieldGroup'] = fgmanager.title
             df = df.append(tmp_df,ignore_index=True)
         if save:
             title = self.schema.get('title',f'unknown_schema_{str(int(time.time()))}.csv')
             df.to_csv(f"{title}.csv",index=False)
         df = df[~df.duplicated('path')].reset_index(drop=True)
         return df
```

### Comparing `aepp-0.2.8/aepp/segmentation.py` & `aepp-0.2.9/aepp/segmentation.py`

 * *Files identical despite different names*

### Comparing `aepp-0.2.8/aepp/sensei.py` & `aepp-0.2.9/aepp/sensei.py`

 * *Files identical despite different names*

### Comparing `aepp-0.2.8/aepp.egg-info/PKG-INFO` & `aepp-0.2.9/aepp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aepp
-Version: 0.2.8
+Version: 0.2.9
 Summary: Package to manage AEP API endpoint and some helper functions
 Home-page: https://github.com/pitchmuc/aep
 Author: Julien Piccini
 Author-email: piccini.julien@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -69,14 +69,15 @@
 * [segmentation](./docs/segmentation.md)
 * [dataprep](./docs/dataprep.md)
 * [flowservice](./docs/flowservice.md)
 * [policy](./docs/policy.md)
 * [datasets](./docs/datasets.md)
 * [ingestion](./docs/ingestion.md)
 * [destination Authoring](./docs/destination.md)
+* [destination Instance](./docs/destinationinstanceservice.md)
 * [observability](./docs/observability.md)
 * accesscontrol
 * sensei
 * [privacyservice](./docs/privacyservice.md) (see 2nd note below)
 
 Last but not least, the core methods are described here: [main](./docs/main.md)
```

### Comparing `aepp-0.2.8/aepp.egg-info/SOURCES.txt` & `aepp-0.2.9/aepp.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 aepp/configs.py
 aepp/connector.py
 aepp/customerprofile.py
 aepp/dataaccess.py
 aepp/dataprep.py
 aepp/datasets.py
 aepp/destination.py
+aepp/destinationinstanceservice.py
 aepp/flowservice.py
 aepp/identity.py
 aepp/ingestion.py
 aepp/observability.py
 aepp/policy.py
 aepp/privacyservice.py
 aepp/queryservice.py
@@ -30,9 +31,10 @@
 aepp.egg-info/dependency_links.txt
 aepp.egg-info/requires.txt
 aepp.egg-info/top_level.txt
 tests/__init__.py
 tests/catalog_test.py
 tests/dataaccess_test.py
 tests/datasets_test.py
+tests/destinationinstanceservice_test.py
 tests/flowservice_test.py
 tests/schema_test.py
```

### Comparing `aepp-0.2.8/setup.py` & `aepp-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `aepp-0.2.8/tests/catalog_test.py` & `aepp-0.2.9/tests/catalog_test.py`

 * *Files identical despite different names*

### Comparing `aepp-0.2.8/tests/dataaccess_test.py` & `aepp-0.2.9/tests/dataaccess_test.py`

 * *Files identical despite different names*

### Comparing `aepp-0.2.8/tests/flowservice_test.py` & `aepp-0.2.9/tests/flowservice_test.py`

 * *Files identical despite different names*

### Comparing `aepp-0.2.8/tests/schema_test.py` & `aepp-0.2.9/tests/schema_test.py`

 * *Files identical despite different names*

