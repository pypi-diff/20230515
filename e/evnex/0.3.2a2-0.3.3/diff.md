# Comparing `tmp/evnex-0.3.2a2.tar.gz` & `tmp/evnex-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evnex-0.3.2a2.tar", max compression
+gzip compressed data, was "evnex-0.3.3.tar", max compression
```

## Comparing `evnex-0.3.2a2.tar` & `evnex-0.3.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2022-11-24 09:52:54.275678 evnex-0.3.2a2/LICENSE
--rw-r--r--   0        0        0     1673 2022-11-24 09:52:54.275678 evnex-0.3.2a2/README.md
--rw-r--r--   0        0        0       23 2022-11-24 09:52:54.275678 evnex-0.3.2a2/evnex/__init__.py
--rw-r--r--   0        0        0    17825 2022-11-24 09:52:54.275678 evnex-0.3.2a2/evnex/api.py
--rw-r--r--   0        0        0       51 2022-11-24 09:52:54.275678 evnex-0.3.2a2/evnex/errors.py
--rw-r--r--   0        0        0        0 2022-11-24 09:52:54.275678 evnex-0.3.2a2/evnex/schema/__init__.py
--rw-r--r--   0        0        0     3589 2022-11-24 09:52:54.275678 evnex-0.3.2a2/evnex/schema/charge_points.py
--rw-r--r--   0        0        0      117 2022-11-24 09:52:54.275678 evnex-0.3.2a2/evnex/schema/commands.py
--rw-r--r--   0        0        0       95 2022-11-24 09:52:54.275678 evnex-0.3.2a2/evnex/schema/cost.py
--rw-r--r--   0        0        0      650 2022-11-24 09:52:54.275678 evnex-0.3.2a2/evnex/schema/org.py
--rw-r--r--   0        0        0      439 2022-11-24 09:52:54.275678 evnex-0.3.2a2/evnex/schema/user.py
--rw-r--r--   0        0        0        0 2022-11-24 09:52:54.275678 evnex-0.3.2a2/evnex/schema/v3/__init__.py
--rw-r--r--   0        0        0     1472 2022-11-24 09:52:54.275678 evnex-0.3.2a2/evnex/schema/v3/charge_points.py
--rw-r--r--   0        0        0      156 2022-11-24 09:52:54.275678 evnex-0.3.2a2/evnex/schema/v3/commands.py
--rw-r--r--   0        0        0      273 2022-11-24 09:52:54.275678 evnex-0.3.2a2/evnex/schema/v3/cost.py
--rw-r--r--   0        0        0      608 2022-11-24 09:52:54.275678 evnex-0.3.2a2/evnex/schema/v3/generic.py
--rw-r--r--   0        0        0      338 2022-11-24 09:52:54.275678 evnex-0.3.2a2/evnex/schema/v3/relationships.py
--rw-r--r--   0        0        0      702 2022-11-24 09:52:54.275678 evnex-0.3.2a2/pyproject.toml
--rw-r--r--   0        0        0     2523 1970-01-01 00:00:00.000000 evnex-0.3.2a2/setup.py
--rw-r--r--   0        0        0     2474 1970-01-01 00:00:00.000000 evnex-0.3.2a2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-11-27 20:54:46.626771 evnex-0.3.3/LICENSE
+-rw-r--r--   0        0        0     1673 2022-11-27 20:54:46.626771 evnex-0.3.3/README.md
+-rw-r--r--   0        0        0       23 2022-11-27 20:54:46.626771 evnex-0.3.3/evnex/__init__.py
+-rw-r--r--   0        0        0    18049 2022-11-27 20:54:46.626771 evnex-0.3.3/evnex/api.py
+-rw-r--r--   0        0        0       51 2022-11-27 20:54:46.626771 evnex-0.3.3/evnex/errors.py
+-rw-r--r--   0        0        0        0 2022-11-27 20:54:46.626771 evnex-0.3.3/evnex/schema/__init__.py
+-rw-r--r--   0        0        0     3589 2022-11-27 20:54:46.626771 evnex-0.3.3/evnex/schema/charge_points.py
+-rw-r--r--   0        0        0      117 2022-11-27 20:54:46.626771 evnex-0.3.3/evnex/schema/commands.py
+-rw-r--r--   0        0        0       95 2022-11-27 20:54:46.626771 evnex-0.3.3/evnex/schema/cost.py
+-rw-r--r--   0        0        0      650 2022-11-27 20:54:46.626771 evnex-0.3.3/evnex/schema/org.py
+-rw-r--r--   0        0        0      439 2022-11-27 20:54:46.626771 evnex-0.3.3/evnex/schema/user.py
+-rw-r--r--   0        0        0        0 2022-11-27 20:54:46.626771 evnex-0.3.3/evnex/schema/v3/__init__.py
+-rw-r--r--   0        0        0     1472 2022-11-27 20:54:46.626771 evnex-0.3.3/evnex/schema/v3/charge_points.py
+-rw-r--r--   0        0        0      156 2022-11-27 20:54:46.626771 evnex-0.3.3/evnex/schema/v3/commands.py
+-rw-r--r--   0        0        0      273 2022-11-27 20:54:46.626771 evnex-0.3.3/evnex/schema/v3/cost.py
+-rw-r--r--   0        0        0      608 2022-11-27 20:54:46.626771 evnex-0.3.3/evnex/schema/v3/generic.py
+-rw-r--r--   0        0        0      338 2022-11-27 20:54:46.626771 evnex-0.3.3/evnex/schema/v3/relationships.py
+-rw-r--r--   0        0        0      700 2022-11-27 20:54:46.626771 evnex-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2521 1970-01-01 00:00:00.000000 evnex-0.3.3/setup.py
+-rw-r--r--   0        0        0     2472 1970-01-01 00:00:00.000000 evnex-0.3.3/PKG-INFO
```

### Comparing `evnex-0.3.2a2/LICENSE` & `evnex-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `evnex-0.3.2a2/README.md` & `evnex-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `evnex-0.3.2a2/evnex/api.py` & `evnex-0.3.3/evnex/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,14 +144,17 @@
         if response.status_code == 401:
             logger.debug("Access Token likely expired, re-authenticate then retry")
             raise NotAuthorizedException()
         if not response.is_success:
             logger.warning(
                 f"Unsuccessful request\n{response.status_code}\n{response.text}"
             )
+        logger.debug(
+            f"Raw EVNEX API response.\n{response.status_code}\n{response.text}"
+        )
 
         response.raise_for_status()
 
         try:
             return response.json()
         except:
             logger.debug(
@@ -221,14 +224,17 @@
         self, charge_point_id: str
     ) -> EvnexV3APIResponse[EvnexChargePointDetailV3]:
 
         r = await self.httpx_client.get(
             f"https://client-api.evnex.io/v3/charge-points/{charge_point_id}",
             headers=self._common_headers,
         )
+        logger.debug(
+            f"Raw get charge point detail response.\n{r.status_code}\n{r.text}"
+        )
         json_data = await self._check_api_response(r)
         return EvnexV3APIResponse[EvnexChargePointDetailV3](**json_data)
 
     @retry(
         wait=wait_random_exponential(multiplier=1, max=60),
         retry=retry_if_not_exception_type((ValidationError, NotAuthorizedException)),
     )
```

### Comparing `evnex-0.3.2a2/evnex/schema/charge_points.py` & `evnex-0.3.3/evnex/schema/charge_points.py`

 * *Files identical despite different names*

### Comparing `evnex-0.3.2a2/evnex/schema/org.py` & `evnex-0.3.3/evnex/schema/org.py`

 * *Files identical despite different names*

### Comparing `evnex-0.3.2a2/evnex/schema/v3/charge_points.py` & `evnex-0.3.3/evnex/schema/v3/charge_points.py`

 * *Files identical despite different names*

### Comparing `evnex-0.3.2a2/evnex/schema/v3/generic.py` & `evnex-0.3.3/evnex/schema/v3/generic.py`

 * *Files identical despite different names*

### Comparing `evnex-0.3.2a2/pyproject.toml` & `evnex-0.3.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "evnex"
-version = "0.3.2a2"
+version = "0.3.3"
 description = "A Python wrapper for the EVNEX Cloud API"
 authors = ["Brian Thorne <brian@hardbyte.nz>"]
 readme = "README.md"
 repository = "https://github.com/hardbyte/python-evnex"
 license = "Apache-2.0"
 
 [tool.poetry.urls]
```

### Comparing `evnex-0.3.2a2/setup.py` & `evnex-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['httpx>=0.23,<0.24',
  'pycognito>=2022.11,<2023.0',
  'pydantic>=1.10,<2.0',
  'tenacity>=8.1,<9.0']
 
 setup_kwargs = {
     'name': 'evnex',
-    'version': '0.3.2a2',
+    'version': '0.3.3',
     'description': 'A Python wrapper for the EVNEX Cloud API',
     'long_description': '# python-evnex\n\nPython client for the Evnex API.\n\nAuthor not affiliated with Evnex.\n\n## Features \n\n- Talks to your Evnex charger via Cloud API\n- Automatic retries with exponential backoff\n- Automatic re-authentication\n- Optionally pass in a `httpx` client\n- Optionally pass in tokens to resume existing session\n\n## Installation\n\n```\npip install evnex\n```\n\n\n## Usage\n\n```python\nimport asyncio\nfrom pydantic import BaseSettings, SecretStr\nfrom evnex.api import Evnex\n\n\nclass EvnexAuthDetails(BaseSettings):\n    EVNEX_CLIENT_USERNAME: str\n    EVNEX_CLIENT_PASSWORD: SecretStr\n\n\nasync def main():\n    creds = EvnexAuthDetails()\n    evnex = Evnex(username=creds.EVNEX_CLIENT_USERNAME,\n                  password=creds.EVNEX_CLIENT_PASSWORD.get_secret_value())\n\n    user_data = await evnex.get_user_detail()\n\n    for org in user_data.organisations:\n        print("Getting 7 day insight for", org.name, "User:", user_data.name)\n        insights = await evnex.get_org_insight(days=7, org_id=org.id)\n\n        for segment in insights:\n            print(segment)\n\n\nif __name__ == \'__main__\':\n    asyncio.run(main())\n```\n\n## Examples\n\n`python-evnex` is intended as a library, but a few example scripts are provided in the `examples` folder.\n\nProviding authentication for the examples is via environment variables, e.g. on nix systems:\n\n```\nexport EVNEX_CLIENT_USERNAME=you@example.com\nexport EVNEX_CLIENT_PASSWORD=<your password>\n\npython -m examples.get_charge_point_detail\n```\n\n## Developer Notes\n\n### Making a new release\n\nWhat ends up on PyPi is what really matters. \n\nUpdate the version in `pyproject.toml`, build and publish with poetry:\n\n```shell\npoetry build\npoetry publish\n```\n',
     'author': 'Brian Thorne',
     'author_email': 'brian@hardbyte.nz',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/hardbyte/python-evnex',
```

### Comparing `evnex-0.3.2a2/PKG-INFO` & `evnex-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evnex
-Version: 0.3.2a2
+Version: 0.3.3
 Summary: A Python wrapper for the EVNEX Cloud API
 Home-page: https://github.com/hardbyte/python-evnex
 License: Apache-2.0
 Author: Brian Thorne
 Author-email: brian@hardbyte.nz
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

