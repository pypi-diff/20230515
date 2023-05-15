# Comparing `tmp/api-client-lnx-edge-0.3.0.tar.gz` & `tmp/api-client-lnx-edge-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/ntulli/Leadnomics/edge-api-client/dist/tmpwkbnk74r/api-client-lnx-edge-0.3.0.tar", last modified: Wed Nov  9 18:49:17 2022, max compression
+gzip compressed data, was "/Users/ntulli/Leadnomics/edge-api-client/dist/.tmp-2s374mv6/api-client-lnx-edge-0.3.1.tar", last modified: Mon May 15 18:13:19 2023, max compression
```

## Comparing `api-client-lnx-edge-0.3.0.tar` & `api-client-lnx-edge-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2022-11-09 18:49:17.000000 api-client-lnx-edge-0.3.0/
--rw-r--r--   0 ntulli     (502) staff       (20)     1104 2022-11-09 18:49:17.000000 api-client-lnx-edge-0.3.0/PKG-INFO
--rw-r--r--   0 ntulli     (502) staff       (20)      738 2022-11-08 16:55:35.000000 api-client-lnx-edge-0.3.0/README.md
--rw-r--r--   0 ntulli     (502) staff       (20)      100 2021-08-23 17:29:30.000000 api-client-lnx-edge-0.3.0/pyproject.toml
--rw-r--r--   0 ntulli     (502) staff       (20)       38 2022-11-09 18:49:17.000000 api-client-lnx-edge-0.3.0/setup.cfg
--rw-r--r--   0 ntulli     (502) staff       (20)      767 2022-11-09 18:48:47.000000 api-client-lnx-edge-0.3.0/setup.py
-drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2022-11-09 18:49:17.000000 api-client-lnx-edge-0.3.0/src/
-drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2022-11-09 18:49:17.000000 api-client-lnx-edge-0.3.0/src/api_client_lnx_edge.egg-info/
--rw-r--r--   0 ntulli     (502) staff       (20)     1104 2022-11-09 18:49:17.000000 api-client-lnx-edge-0.3.0/src/api_client_lnx_edge.egg-info/PKG-INFO
--rw-r--r--   0 ntulli     (502) staff       (20)      477 2022-11-09 18:49:17.000000 api-client-lnx-edge-0.3.0/src/api_client_lnx_edge.egg-info/SOURCES.txt
--rw-r--r--   0 ntulli     (502) staff       (20)        1 2022-11-09 18:49:17.000000 api-client-lnx-edge-0.3.0/src/api_client_lnx_edge.egg-info/dependency_links.txt
--rw-r--r--   0 ntulli     (502) staff       (20)       50 2022-11-09 18:49:17.000000 api-client-lnx-edge-0.3.0/src/api_client_lnx_edge.egg-info/requires.txt
--rw-r--r--   0 ntulli     (502) staff       (20)       16 2022-11-09 18:49:17.000000 api-client-lnx-edge-0.3.0/src/api_client_lnx_edge.egg-info/top_level.txt
-drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2022-11-09 18:49:17.000000 api-client-lnx-edge-0.3.0/src/edge_api_client/
--rw-r--r--   0 ntulli     (502) staff       (20)       26 2022-10-11 15:31:34.000000 api-client-lnx-edge-0.3.0/src/edge_api_client/__init__.py
--rw-r--r--   0 ntulli     (502) staff       (20)     1135 2022-10-22 18:30:37.000000 api-client-lnx-edge-0.3.0/src/edge_api_client/base.py
--rw-r--r--   0 ntulli     (502) staff       (20)    18467 2022-11-08 16:57:56.000000 api-client-lnx-edge-0.3.0/src/edge_api_client/edge.py
-drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2022-11-09 18:49:17.000000 api-client-lnx-edge-0.3.0/src/edge_api_client/utilities/
--rw-r--r--   0 ntulli     (502) staff       (20)       90 2022-10-11 15:47:27.000000 api-client-lnx-edge-0.3.0/src/edge_api_client/utilities/__init__.py
--rw-r--r--   0 ntulli     (502) staff       (20)     2532 2022-10-11 15:47:27.000000 api-client-lnx-edge-0.3.0/src/edge_api_client/utilities/funcs.py
--rw-r--r--   0 ntulli     (502) staff       (20)     2446 2022-11-09 18:30:15.000000 api-client-lnx-edge-0.3.0/src/edge_api_client/utilities/schemas.py
+drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2023-05-15 18:13:19.000000 api-client-lnx-edge-0.3.1/
+-rw-r--r--   0 ntulli     (502) staff       (20)     1104 2023-05-15 18:13:19.000000 api-client-lnx-edge-0.3.1/PKG-INFO
+-rw-r--r--   0 ntulli     (502) staff       (20)      738 2023-05-15 16:41:00.000000 api-client-lnx-edge-0.3.1/README.md
+-rw-r--r--   0 ntulli     (502) staff       (20)      100 2021-08-23 17:29:30.000000 api-client-lnx-edge-0.3.1/pyproject.toml
+-rw-r--r--   0 ntulli     (502) staff       (20)       38 2023-05-15 18:13:19.000000 api-client-lnx-edge-0.3.1/setup.cfg
+-rw-r--r--   0 ntulli     (502) staff       (20)      767 2023-05-15 18:04:36.000000 api-client-lnx-edge-0.3.1/setup.py
+drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2023-05-15 18:13:19.000000 api-client-lnx-edge-0.3.1/src/
+drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2023-05-15 18:13:19.000000 api-client-lnx-edge-0.3.1/src/api_client_lnx_edge.egg-info/
+-rw-r--r--   0 ntulli     (502) staff       (20)     1104 2023-05-15 18:13:19.000000 api-client-lnx-edge-0.3.1/src/api_client_lnx_edge.egg-info/PKG-INFO
+-rw-r--r--   0 ntulli     (502) staff       (20)      496 2023-05-15 18:13:19.000000 api-client-lnx-edge-0.3.1/src/api_client_lnx_edge.egg-info/SOURCES.txt
+-rw-r--r--   0 ntulli     (502) staff       (20)        1 2023-05-15 18:13:19.000000 api-client-lnx-edge-0.3.1/src/api_client_lnx_edge.egg-info/dependency_links.txt
+-rw-r--r--   0 ntulli     (502) staff       (20)       50 2023-05-15 18:13:19.000000 api-client-lnx-edge-0.3.1/src/api_client_lnx_edge.egg-info/requires.txt
+-rw-r--r--   0 ntulli     (502) staff       (20)       16 2023-05-15 18:13:19.000000 api-client-lnx-edge-0.3.1/src/api_client_lnx_edge.egg-info/top_level.txt
+drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2023-05-15 18:13:19.000000 api-client-lnx-edge-0.3.1/src/edge_api_client/
+-rw-r--r--   0 ntulli     (502) staff       (20)       26 2022-10-11 15:31:34.000000 api-client-lnx-edge-0.3.1/src/edge_api_client/__init__.py
+-rw-r--r--   0 ntulli     (502) staff       (20)     1135 2022-10-22 18:30:37.000000 api-client-lnx-edge-0.3.1/src/edge_api_client/base.py
+-rw-r--r--   0 ntulli     (502) staff       (20)    18902 2023-05-15 18:01:45.000000 api-client-lnx-edge-0.3.1/src/edge_api_client/edge.py
+drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2023-05-15 18:13:19.000000 api-client-lnx-edge-0.3.1/src/edge_api_client/utilities/
+-rw-r--r--   0 ntulli     (502) staff       (20)       90 2023-05-15 16:41:00.000000 api-client-lnx-edge-0.3.1/src/edge_api_client/utilities/__init__.py
+-rw-r--r--   0 ntulli     (502) staff       (20)     2532 2023-05-15 16:41:00.000000 api-client-lnx-edge-0.3.1/src/edge_api_client/utilities/funcs.py
+-rw-r--r--   0 ntulli     (502) staff       (20)     2446 2022-11-09 18:30:15.000000 api-client-lnx-edge-0.3.1/src/edge_api_client/utilities/schemas.py
+drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2023-05-15 18:13:19.000000 api-client-lnx-edge-0.3.1/tests/
+-rw-r--r--   0 ntulli     (502) staff       (20)      322 2021-08-23 19:03:52.000000 api-client-lnx-edge-0.3.1/tests/test_auth.py
```

### Comparing `api-client-lnx-edge-0.3.0/PKG-INFO` & `api-client-lnx-edge-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-client-lnx-edge
-Version: 0.3.0
+Version: 0.3.1
 Summary: Client for the LNX Edge API
 Home-page: https://github.com/Lnmix/edge_api_client
 Author: Nick Tulli
 Author-email: ntulli@leadnomics.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `api-client-lnx-edge-0.3.0/README.md` & `api-client-lnx-edge-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `api-client-lnx-edge-0.3.0/setup.py` & `api-client-lnx-edge-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='api-client-lnx-edge',
-    version='0.3.0',
+    version='0.3.1',
     description='Client for the LNX Edge API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Lnmix/edge_api_client',
     author='Nick Tulli',
     author_email='ntulli@leadnomics.com',
     package_dir={'': 'src'},
```

### Comparing `api-client-lnx-edge-0.3.0/src/api_client_lnx_edge.egg-info/PKG-INFO` & `api-client-lnx-edge-0.3.1/src/api_client_lnx_edge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-client-lnx-edge
-Version: 0.3.0
+Version: 0.3.1
 Summary: Client for the LNX Edge API
 Home-page: https://github.com/Lnmix/edge_api_client
 Author: Nick Tulli
 Author-email: ntulli@leadnomics.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `api-client-lnx-edge-0.3.0/src/edge_api_client/base.py` & `api-client-lnx-edge-0.3.1/src/edge_api_client/base.py`

 * *Files identical despite different names*

### Comparing `api-client-lnx-edge-0.3.0/src/edge_api_client/edge.py` & `api-client-lnx-edge-0.3.1/src/edge_api_client/edge.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import requests
-from typing import List
+from typing import List, Tuple
 from datetime import datetime, date
 
 from .base import BaseAPIClient
 from .utilities import get_dayparting, format_adjustment_date, build_filters, build_daterange
 from .utilities.schemas import CreateOfferSchema
 
 
@@ -204,16 +204,16 @@
         schema = CreateOfferSchema()
         json_data = schema.load({k: v for k, v in body.items() if v is not None})
 
         return self._post('api/offers', json=schema.dump(json_data))
 
     def _get_report(self,
                     dimensions: list,
-                    start_date: (datetime, date, str),
-                    end_date: (datetime, date, str),
+                    start_date: Tuple[datetime, date, str],
+                    end_date: Tuple[datetime, date, str],
                     timezone: str = 'America/New_York',
                     metrics: list = None,
                     filters: list = None,
                     rows_per_page: int = 10000,
                     row_offset: int = 0,
                     **kwargs) -> requests.Response:
         """ Get a report with arguments. """
@@ -232,43 +232,43 @@
         #  filters like `affiliate_id=XXXX` with ease.
         report_config.update((k, kwargs[k]) for k in report_config.keys() & kwargs.keys())
 
         resp = self._post('api/reports', json=report_config)
 
         return resp
 
-    def get_advertiser_report(self, start_date: (datetime, date, str), end_date: (datetime, date, str), **kwargs) -> requests.Response:
+    def get_advertiser_report(self, start_date: Tuple[datetime, date, str], end_date: Tuple[datetime, date, str], **kwargs) -> requests.Response:
         """ Get default advertiser report.
 
         :param start_date: YYYY-MM-DD date
         :param end_date: YYYY-MM-DD date
         :return: response
         """
         return self._get_report(
             dimensions=['advertiserId', 'advertiserName'],
             start_date=start_date,
             end_date=end_date,
             **kwargs
         )
 
-    def get_affiliate_report(self, start_date: (datetime, date, str), end_date: (datetime, date, str), **kwargs) -> requests.Response:
+    def get_affiliate_report(self, start_date: Tuple[datetime, date, str], end_date: Tuple[datetime, date, str], **kwargs) -> requests.Response:
         """ Get default affiliate report.
 
         :param start_date: YYYY-MM-DD date
         :param end_date: YYYY-MM-DD date
         :return: response
         """
         return self._get_report(
             dimensions=['affiliateId', 'affiliateCompany'],
             start_date=start_date,
             end_date=end_date,
             **kwargs
         )
 
-    def get_click_report(self, start_date: (datetime, date, str), end_date: (datetime, date, str), **kwargs) -> requests.Response:
+    def get_click_report(self, start_date: Tuple[datetime, date, str], end_date: Tuple[datetime, date, str], **kwargs) -> requests.Response:
         """ Get default click report.
 
         :param start_date: YYYY-MM-DD date
         :param end_date: YYYY-MM-DD date
         :return: response
         """
         return self._get_report(
@@ -276,57 +276,57 @@
                         's1', 's2', 's3', 's4', 's5', 'ipaddress', 'go_disposition'],
             metrics=['conversions', 'paidConversions', 'lnxProfit', 'lnxRevenue', 'lnxCost'],
             start_date=start_date,
             end_date=end_date,
             **kwargs
         )
 
-    def get_daily_report(self, start_date: (datetime, date, str), end_date: (datetime, date, str), **kwargs) -> requests.Response:
+    def get_daily_report(self, start_date: Tuple[datetime, date, str], end_date: Tuple[datetime, date, str], **kwargs) -> requests.Response:
         """ Get default daily report.
 
         :param start_date: YYYY-MM-DD date
         :param end_date: YYYY-MM-DD date
         :return: response
         """
         return self._get_report(
             dimensions=['timestampDay'],
             start_date=start_date,
             end_date=end_date,
             **kwargs
         )
 
-    def get_hourly_report(self, start_date: (datetime, date, str), end_date: (datetime, date, str), **kwargs) -> requests.Response:
+    def get_hourly_report(self, start_date: Tuple[datetime, date, str], end_date: Tuple[datetime, date, str], **kwargs) -> requests.Response:
         """ Get default hourly report.
 
         :param start_date: YYYY-MM-DD date
         :param end_date: YYYY-MM-DD date
         :return: response
         """
         return self._get_report(
             dimensions=['timestampDay', 'hourOfDay'],
             start_date=start_date,
             end_date=end_date,
             **kwargs
         )
 
-    def get_offer_report(self, start_date: (datetime, date, str), end_date: (datetime, date, str), **kwargs) -> requests.Response:
+    def get_offer_report(self, start_date: Tuple[datetime, date, str], end_date: Tuple[datetime, date, str], **kwargs) -> requests.Response:
         """ Get default offer report.
 
         :param start_date: YYYY-MM-DD date
         :param end_date: YYYY-MM-DD date
         :return: response
         """
         return self._get_report(
             dimensions=['offerId', 'offerName'],
             start_date=start_date,
             end_date=end_date,
             **kwargs
         )
 
-    def get_paid_conversion_report(self, start_date: (datetime, date, str), end_date: (datetime, date, str), **kwargs) -> requests.Response:
+    def get_paid_conversion_report(self, start_date: Tuple[datetime, date, str], end_date: Tuple[datetime, date, str], **kwargs) -> requests.Response:
         """ Get default paid conversion report.
 
         :param start_date: YYYY-MM-DD date
         :param end_date: YYYY-MM-DD date
         :return: response
         """
         return self._get_report(
@@ -335,29 +335,29 @@
             metrics=['lnxProfit', 'lnxRevenue', 'lnxCost'],
             filters=[{'type': 'gt', 'value': 0, 'column': 'paidConversions'}],
             start_date=start_date,
             end_date=end_date,
             **kwargs
         )
 
-    def get_product_report(self, start_date: (datetime, date, str), end_date: (datetime, date, str), **kwargs) -> requests.Response:
+    def get_product_report(self, start_date: Tuple[datetime, date, str], end_date: Tuple[datetime, date, str], **kwargs) -> requests.Response:
         """ Get default product report.
 
         :param start_date: YYYY-MM-DD date
         :param end_date: YYYY-MM-DD date
         :return: response
         """
         return self._get_report(
             dimensions=['productId', 'productName'],
             start_date=start_date,
             end_date=end_date,
             **kwargs
         )
 
-    def get_sessions_report(self, start_date: (datetime, date, str), end_date: (datetime, date, str), **kwargs) -> requests.Response:
+    def get_sessions_report(self, start_date: Tuple[datetime, date, str], end_date: Tuple[datetime, date, str], **kwargs) -> requests.Response:
         """ Get default sessions report.
 
         :param start_date: YYYY-MM-DD date
         :param end_date: YYYY-MM-DD date
         :return: response
         """
         return self._get_report(
@@ -365,29 +365,29 @@
                         's1', 's2', 's3', 's4', 's5', 'ipaddress', 'go_disposition'],
             metrics=['clicks', 'conversions', 'paidConversions', 'lnxProfit', 'lnxRevenue', 'lnxCost'],
             start_date=start_date,
             end_date=end_date,
             **kwargs
         )
 
-    def get_suboffer_report(self, start_date: (datetime, date, str), end_date: (datetime, date, str), **kwargs) -> requests.Response:
+    def get_suboffer_report(self, start_date: Tuple[datetime, date, str], end_date: Tuple[datetime, date, str], **kwargs) -> requests.Response:
         """ Get default suboffer report.
 
         :param start_date: YYYY-MM-DD date
         :param end_date: YYYY-MM-DD date
         :return: response
         """
         return self._get_report(
             dimensions=['subOfferId', 'subOfferName'],
             start_date=start_date,
             end_date=end_date,
             **kwargs
         )
 
-    def get_total_conversion_report(self, start_date: (datetime, date, str), end_date: (datetime, date, str), **kwargs) -> requests.Response:
+    def get_total_conversion_report(self, start_date: Tuple[datetime, date, str], end_date: Tuple[datetime, date, str], **kwargs) -> requests.Response:
         """ Get default total conversion report.
 
         :param start_date: YYYY-MM-DD date
         :param end_date: YYYY-MM-DD date
         :return: response
         """
         return self._get_report(
@@ -425,9 +425,17 @@
 
         resp = self._post('api/adjust-stats', json=data)
 
         return resp
 
         # TODO: get ALL entities. Including verticals, domains, etc.
 
+    def get_offer_approvals(self, offer_id, **kwargs) -> requests.Response:
+        """ Given an offer ID, return all approved affiliates.
+
+        :param offer_id: an Edge offer ID
+        :return: response object
+        """
+        return self._get('api/offers/{}/affiliates'.format(offer_id), **kwargs)
+
     def __repr__(self):
         return f'EdgeAPI(staging={self.staging})'
```

### Comparing `api-client-lnx-edge-0.3.0/src/edge_api_client/utilities/funcs.py` & `api-client-lnx-edge-0.3.1/src/edge_api_client/utilities/funcs.py`

 * *Files identical despite different names*

### Comparing `api-client-lnx-edge-0.3.0/src/edge_api_client/utilities/schemas.py` & `api-client-lnx-edge-0.3.1/src/edge_api_client/utilities/schemas.py`

 * *Files identical despite different names*

