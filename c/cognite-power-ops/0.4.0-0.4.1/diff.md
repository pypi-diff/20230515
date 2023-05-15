# Comparing `tmp/cognite_power_ops-0.4.0.tar.gz` & `tmp/cognite_power_ops-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_power_ops-0.4.0.tar", max compression
+gzip compressed data, was "cognite_power_ops-0.4.1.tar", max compression
```

## Comparing `cognite_power_ops-0.4.0.tar` & `cognite_power_ops-0.4.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0    10758 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/LICENSE
--rw-r--r--   0        0        0      250 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/README.md
--rw-r--r--   0        0        0       76 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/cognite/powerops/__init__.py
--rw-r--r--   0        0        0    10260 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/cognite/powerops/bootstrap.py
--rw-r--r--   0        0        0       65 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/cognite/powerops/client/__init__.py
--rw-r--r--   0        0        0     6203 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/cognite/powerops/client/asset_apis.py
--rw-r--r--   0        0        0      601 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/cognite/powerops/client/config_client.py
--rw-r--r--   0        0        0        0 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/cognite/powerops/client/dm/__init__.py
--rw-r--r--   0        0        0     1891 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/cognite/powerops/client/dm/client.py
--rw-r--r--   0        0        0      895 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/cognite/powerops/client/dm/schema.graphql
--rw-r--r--   0        0        0     2037 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/cognite/powerops/client/dm/schema.py
--rw-r--r--   0        0        0     1875 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/cognite/powerops/client/dm_apis.py
--rw-r--r--   0        0        0     2275 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/cognite/powerops/client/powerops_client.py
--rw-r--r--   0        0        0     3074 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/cognite/powerops/client/shop_api.py
--rw-r--r--   0        0        0    26552 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/cognite/powerops/config.py
--rw-r--r--   0        0        0        0 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/cognite/powerops/data_classes/__init__.py
--rw-r--r--   0        0        0     1221 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/cognite/powerops/data_classes/asset_lists.py
--rw-r--r--   0        0        0     3057 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/cognite/powerops/data_classes/benchmarking_config.py
--rw-r--r--   0        0        0     2984 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/cognite/powerops/data_classes/bid_matrix_generator_config.py
--rw-r--r--   0        0        0    13238 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/data_classes/cdf_resource_collection.py
--rw-r--r--   0        0        0     2513 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/data_classes/common.py
--rw-r--r--   0        0        0      129 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/data_classes/config_model.py
--rw-r--r--   0        0        0     3630 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/data_classes/core.py
--rw-r--r--   0        0        0      128 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/data_classes/generators.py
--rw-r--r--   0        0        0     1482 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/data_classes/market_config.py
--rw-r--r--   0        0        0    16796 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/data_classes/plant.py
--rw-r--r--   0        0        0       99 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/data_classes/price_area.py
--rw-r--r--   0        0        0     5114 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/data_classes/reserve_scenario.py
--rw-r--r--   0        0        0      180 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/data_classes/reservoirs.py
--rw-r--r--   0        0        0     1609 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/data_classes/rkom_bid_combination_config.py
--rw-r--r--   0        0        0      994 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/data_classes/rkom_market_config.py
--rw-r--r--   0        0        0      163 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/data_classes/shared.py
--rw-r--r--   0        0        0     2113 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/data_classes/shop_file_config.py
--rw-r--r--   0        0        0     2815 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/data_classes/shop_output_definition.py
--rw-r--r--   0        0        0     9189 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/data_classes/time_series_mapping.py
--rw-r--r--   0        0        0     1144 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/data_classes/transformation.py
--rw-r--r--   0        0        0     1042 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/logger.py
--rw-r--r--   0        0        0     2070 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/main.py
--rw-r--r--   0        0        0        0 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/utils/__init__.py
--rw-r--r--   0        0        0     1936 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/utils/asset_types.py
--rw-r--r--   0        0        0     1424 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/utils/cdf_auth.py
--rw-r--r--   0        0        0     2724 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/utils/cdf_utils.py
--rw-r--r--   0        0        0      744 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/utils/common.py
--rw-r--r--   0        0        0      324 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/utils/constants.py
--rw-r--r--   0        0        0     3271 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/utils/files.py
--rw-r--r--   0        0        0     4979 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/utils/labels.py
--rw-r--r--   0        0        0     1766 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/utils/mapping/mapping.py
--rw-r--r--   0        0        0     2609 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/utils/mapping/static_mapping.py
--rw-r--r--   0        0        0     3165 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/utils/powerops_asset_hierarchy.py
--rw-r--r--   0        0        0      718 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/utils/powerops_status_events.py
--rw-r--r--   0        0        0     4495 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/utils/relationship_types.py
--rw-r--r--   0        0        0    11602 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/utils/resource_generation.py
--rw-r--r--   0        0        0     1495 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/utils/serializer.py
--rw-r--r--   0        0        0       22 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/version.py
--rw-r--r--   0        0        0     1423 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1346 1970-01-01 00:00:00.000000 cognite_power_ops-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    10758 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/LICENSE
+-rw-r--r--   0        0        0      250 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/README.md
+-rw-r--r--   0        0        0       76 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/__init__.py
+-rw-r--r--   0        0        0    10260 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/bootstrap.py
+-rw-r--r--   0        0        0       65 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/client/__init__.py
+-rw-r--r--   0        0        0     6203 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/client/asset_apis.py
+-rw-r--r--   0        0        0      601 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/client/config_client.py
+-rw-r--r--   0        0        0        0 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/client/dm/__init__.py
+-rw-r--r--   0        0        0     1750 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/client/dm/client.py
+-rw-r--r--   0        0        0      895 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/client/dm/schema.graphql
+-rw-r--r--   0        0        0     2037 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/client/dm/schema.py
+-rw-r--r--   0        0        0     1883 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/client/dm_apis.py
+-rw-r--r--   0        0        0     2294 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/client/powerops_client.py
+-rw-r--r--   0        0        0     2990 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/client/shop_api.py
+-rw-r--r--   0        0        0    26552 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/config.py
+-rw-r--r--   0        0        0        0 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/data_classes/__init__.py
+-rw-r--r--   0        0        0     1221 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/data_classes/asset_lists.py
+-rw-r--r--   0        0        0     3057 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/data_classes/benchmarking_config.py
+-rw-r--r--   0        0        0     2984 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/data_classes/bid_matrix_generator_config.py
+-rw-r--r--   0        0        0    13238 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/data_classes/cdf_resource_collection.py
+-rw-r--r--   0        0        0     2513 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/data_classes/common.py
+-rw-r--r--   0        0        0      129 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/data_classes/config_model.py
+-rw-r--r--   0        0        0     3630 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/data_classes/core.py
+-rw-r--r--   0        0        0      128 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/data_classes/generators.py
+-rw-r--r--   0        0        0     1482 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/data_classes/market_config.py
+-rw-r--r--   0        0        0    16796 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/data_classes/plant.py
+-rw-r--r--   0        0        0       99 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/data_classes/price_area.py
+-rw-r--r--   0        0        0     5114 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/data_classes/reserve_scenario.py
+-rw-r--r--   0        0        0      180 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/data_classes/reservoirs.py
+-rw-r--r--   0        0        0     1609 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/data_classes/rkom_bid_combination_config.py
+-rw-r--r--   0        0        0      994 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/data_classes/rkom_market_config.py
+-rw-r--r--   0        0        0      163 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/data_classes/shared.py
+-rw-r--r--   0        0        0     2113 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/data_classes/shop_file_config.py
+-rw-r--r--   0        0        0     2815 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/data_classes/shop_output_definition.py
+-rw-r--r--   0        0        0     9189 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/data_classes/time_series_mapping.py
+-rw-r--r--   0        0        0     1144 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/data_classes/transformation.py
+-rw-r--r--   0        0        0     1042 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/logger.py
+-rw-r--r--   0        0        0     2070 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/main.py
+-rw-r--r--   0        0        0        0 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/utils/__init__.py
+-rw-r--r--   0        0        0     1936 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/utils/asset_types.py
+-rw-r--r--   0        0        0     1424 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/utils/cdf_auth.py
+-rw-r--r--   0        0        0     2724 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/utils/cdf_utils.py
+-rw-r--r--   0        0        0      744 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/utils/common.py
+-rw-r--r--   0        0        0      324 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/utils/constants.py
+-rw-r--r--   0        0        0     3271 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/utils/files.py
+-rw-r--r--   0        0        0     4979 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/utils/labels.py
+-rw-r--r--   0        0        0     1766 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/utils/mapping/mapping.py
+-rw-r--r--   0        0        0     2609 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/utils/mapping/static_mapping.py
+-rw-r--r--   0        0        0     3165 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/utils/powerops_asset_hierarchy.py
+-rw-r--r--   0        0        0      718 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/utils/powerops_status_events.py
+-rw-r--r--   0        0        0     4495 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/utils/relationship_types.py
+-rw-r--r--   0        0        0    11602 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/utils/resource_generation.py
+-rw-r--r--   0        0        0     1495 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/utils/serializer.py
+-rw-r--r--   0        0        0       22 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/cognite/powerops/version.py
+-rw-r--r--   0        0        0     1434 2023-05-15 08:39:28.798681 cognite_power_ops-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1346 1970-01-01 00:00:00.000000 cognite_power_ops-0.4.1/PKG-INFO
```

### Comparing `cognite_power_ops-0.4.0/LICENSE` & `cognite_power_ops-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/bootstrap.py` & `cognite_power_ops-0.4.1/cognite/powerops/bootstrap.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/client/asset_apis.py` & `cognite_power_ops-0.4.1/cognite/powerops/client/asset_apis.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/client/config_client.py` & `cognite_power_ops-0.4.1/cognite/powerops/client/config_client.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/client/dm/client.py` & `cognite_power_ops-0.4.1/cognite/powerops/client/dm/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 from __future__ import annotations
 
 from typing import Optional
 
 from cachelib import BaseCache, SimpleCache
 from cognite.client import ClientConfig
-from cognite.dm_clients.cdf.get_client import get_client_config
 from cognite.dm_clients.config import settings
 from cognite.dm_clients.domain_modeling import DomainClient, DomainModelAPI
 
 from .schema import (
     Case,
     CommandsConfig,
     FileRef,
@@ -39,19 +38,18 @@
 
 
 def get_power_ops_dm_client(
     cache: Optional[BaseCache] = None,
     space_id: Optional[str] = None,
     data_model: Optional[str] = None,
     schema_version: Optional[int] = None,
-    config: Optional[ClientConfig] = None,
+    config: ClientConfig = None,
 ) -> PowerOpsDmClient:
     """Quick way of instantiating a PowerOpsDmClient with sensible defaults for development."""
     cache = cache if cache is not None else SimpleCache()
-    config = config if config is not None else get_client_config()
     space_external_id = space_id or settings.dm_clients.space
     data_model = data_model or settings.dm_clients.datamodel
     schema_version = schema_version or settings.dm_clients.schema_version
     return PowerOpsDmClient(
         power_ops_dm_schema,
         DomainModelAPI,
         cache,
```

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/client/dm/schema.graphql` & `cognite_power_ops-0.4.1/cognite/powerops/client/dm/schema.graphql`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/client/dm/schema.py` & `cognite_power_ops-0.4.1/cognite/powerops/client/dm/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/client/dm_apis.py` & `cognite_power_ops-0.4.1/cognite/powerops/client/dm_apis.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from typing import Generic, TypeVar
 
-from dm_clients.domain_modeling import DomainModel, DomainModelAPI
+from cognite.dm_clients.domain_modeling import DomainModel, DomainModelAPI
 
 from cognite.powerops.client.dm.client import PowerOpsDmClient
 from cognite.powerops.client.dm.schema import Case, CommandsConfig, Mapping, Scenario, Transformation
 
 DomainModelT = TypeVar("DomainModelT", bound=DomainModel)
```

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/client/powerops_client.py` & `cognite_power_ops-0.4.1/cognite/powerops/client/powerops_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
         self.bechmarkings = BenchmarkingConfigurationsAPI(client, read_dataset, write_dataset)
         self.markets = MarketConfigurationsAPI(client, read_dataset, write_dataset)
         self.rkom_bid_combinations = RKOMBidCombinationConfiguration(client, read_dataset, write_dataset)
 
 
 class PowerOpsClient:
     def __init__(self, read_dataset: str, write_dataset: str, config: Optional[ClientConfig] = None):
-        self.dm = get_power_ops_dm_client()
-        self.core = self.dm._client
+        self.dm = get_power_ops_dm_client(config=config)
+        self.core = CogniteClient(config)
 
         self.configurations = ConfigurationClient()
 
         self.shop = ShopAPI(po_client=self)
 
         self.configurations = ConfigurationsClient(read_dataset, write_dataset, self.core)
         self.generators = GeneratorsAPI(self.core, read_dataset, write_dataset)
```

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/client/shop_api.py` & `cognite_power_ops-0.4.1/cognite/powerops/client/shop_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import random
 import time
 from typing import Optional
 
 from cognite.client.data_classes import FileMetadata
 
-from cognite.powerops.client.powerops_client import PowerOpsClient
-
 
 class ShopRunLog:
     def __init__(self, shop_run_logs: "ShopRunLogs") -> None:
         self._shop_run_logs = shop_run_logs
 
     def file(self) -> FileMetadata:
         return FileMetadata(external_id="log-123", name="shop_123.log")
@@ -115,11 +113,11 @@
         raise NotImplementedError
 
     def retrieve(self, run_id):
         return ShopRun(run_id=run_id)
 
 
 class ShopAPI:
-    def __init__(self, po_client: PowerOpsClient):
+    def __init__(self, po_client):
         self._po_client = po_client
         self.models = ShopModelsAPI(shop_api=self)
         self.runs = ShopRunsApi(shop_api=self)
```

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/config.py` & `cognite_power_ops-0.4.1/cognite/powerops/config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/data_classes/asset_lists.py` & `cognite_power_ops-0.4.1/cognite/powerops/data_classes/asset_lists.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/data_classes/benchmarking_config.py` & `cognite_power_ops-0.4.1/cognite/powerops/data_classes/benchmarking_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/data_classes/bid_matrix_generator_config.py` & `cognite_power_ops-0.4.1/cognite/powerops/data_classes/bid_matrix_generator_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/data_classes/cdf_resource_collection.py` & `cognite_power_ops-0.4.1/cognite/powerops/data_classes/cdf_resource_collection.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/data_classes/common.py` & `cognite_power_ops-0.4.1/cognite/powerops/data_classes/common.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/data_classes/core.py` & `cognite_power_ops-0.4.1/cognite/powerops/data_classes/core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/data_classes/market_config.py` & `cognite_power_ops-0.4.1/cognite/powerops/data_classes/market_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/data_classes/plant.py` & `cognite_power_ops-0.4.1/cognite/powerops/data_classes/plant.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/data_classes/reserve_scenario.py` & `cognite_power_ops-0.4.1/cognite/powerops/data_classes/reserve_scenario.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/data_classes/rkom_bid_combination_config.py` & `cognite_power_ops-0.4.1/cognite/powerops/data_classes/rkom_bid_combination_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/data_classes/rkom_market_config.py` & `cognite_power_ops-0.4.1/cognite/powerops/data_classes/rkom_market_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/data_classes/shop_file_config.py` & `cognite_power_ops-0.4.1/cognite/powerops/data_classes/shop_file_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/data_classes/shop_output_definition.py` & `cognite_power_ops-0.4.1/cognite/powerops/data_classes/shop_output_definition.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/data_classes/time_series_mapping.py` & `cognite_power_ops-0.4.1/cognite/powerops/data_classes/time_series_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/data_classes/transformation.py` & `cognite_power_ops-0.4.1/cognite/powerops/data_classes/transformation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/logger.py` & `cognite_power_ops-0.4.1/cognite/powerops/logger.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/main.py` & `cognite_power_ops-0.4.1/cognite/powerops/main.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/utils/asset_types.py` & `cognite_power_ops-0.4.1/cognite/powerops/utils/asset_types.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/utils/cdf_auth.py` & `cognite_power_ops-0.4.1/cognite/powerops/utils/cdf_auth.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/utils/cdf_utils.py` & `cognite_power_ops-0.4.1/cognite/powerops/utils/cdf_utils.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/utils/common.py` & `cognite_power_ops-0.4.1/cognite/powerops/utils/common.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/utils/files.py` & `cognite_power_ops-0.4.1/cognite/powerops/utils/files.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/utils/labels.py` & `cognite_power_ops-0.4.1/cognite/powerops/utils/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/utils/mapping/mapping.py` & `cognite_power_ops-0.4.1/cognite/powerops/utils/mapping/mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/utils/mapping/static_mapping.py` & `cognite_power_ops-0.4.1/cognite/powerops/utils/mapping/static_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/utils/powerops_asset_hierarchy.py` & `cognite_power_ops-0.4.1/cognite/powerops/utils/powerops_asset_hierarchy.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/utils/powerops_status_events.py` & `cognite_power_ops-0.4.1/cognite/powerops/utils/powerops_status_events.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/utils/relationship_types.py` & `cognite_power_ops-0.4.1/cognite/powerops/utils/relationship_types.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/utils/resource_generation.py` & `cognite_power_ops-0.4.1/cognite/powerops/utils/resource_generation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/cognite/powerops/utils/serializer.py` & `cognite_power_ops-0.4.1/cognite/powerops/utils/serializer.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.0/pyproject.toml` & `cognite_power_ops-0.4.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-power-ops"
-version = "0.4.0"
+version = "0.4.1"
 description = "SDK for power markets operations on Cognite Data Fusion"
 readme = "README.md"
 authors = ["Cognite <support@cognite.com>"]
 license = "Apache 2.0"
 packages = [{include = "cognite", from = "."}]
 
 [tool.black]
@@ -49,11 +49,12 @@
 pytest = "^7.3.1"
 pytest-regressions = "^2.4.2"
 pre-commit = "^3.2.2"
 twine = "^4.0.2"
 pytest-cov = "^4.0.0"
 profilehooks = "^1.12.0"
 pytest-mock = "^3.10.0"
+toml = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cognite_power_ops-0.4.0/PKG-INFO` & `cognite_power_ops-0.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-power-ops
-Version: 0.4.0
+Version: 0.4.1
 Summary: SDK for power markets operations on Cognite Data Fusion
 License: Apache 2.0
 Author: Cognite
 Author-email: support@cognite.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

