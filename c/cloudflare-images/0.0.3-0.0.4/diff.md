# Comparing `tmp/cloudflare_images-0.0.3.tar.gz` & `tmp/cloudflare_images-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudflare_images-0.0.3.tar", max compression
+gzip compressed data, was "cloudflare_images-0.0.4.tar", max compression
```

## Comparing `cloudflare_images-0.0.3.tar` & `cloudflare_images-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1491 2023-04-23 21:35:59.824537 cloudflare_images-0.0.3/LICENSE
--rw-r--r--   0        0        0      265 2023-04-23 22:17:07.618439 cloudflare_images-0.0.3/README.md
--rw-r--r--   0        0        0      112 2023-05-01 02:28:42.966649 cloudflare_images-0.0.3/cloudflare_images/__init__.py
--rw-r--r--   0        0        0     7737 2023-04-23 22:59:59.288543 cloudflare_images-0.0.3/cloudflare_images/api.py
--rw-r--r--   0        0        0     3827 2023-04-26 17:23:10.020196 cloudflare_images-0.0.3/cloudflare_images/django.py
--rw-r--r--   0        0        0     1581 2023-05-01 02:28:00.153503 cloudflare_images-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1189 1970-01-01 00:00:00.000000 cloudflare_images-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-04-23 21:35:59.824537 cloudflare_images-0.0.4/LICENSE
+-rw-r--r--   0        0        0      265 2023-04-23 22:17:07.618439 cloudflare_images-0.0.4/README.md
+-rw-r--r--   0        0        0      112 2023-05-15 15:37:50.513888 cloudflare_images-0.0.4/cloudflare_images/__init__.py
+-rw-r--r--   0        0        0     8629 2023-05-15 15:59:04.074001 cloudflare_images-0.0.4/cloudflare_images/api.py
+-rw-r--r--   0        0        0     3827 2023-04-26 17:23:10.020196 cloudflare_images-0.0.4/cloudflare_images/django.py
+-rw-r--r--   0        0        0     1545 2023-05-15 15:37:54.685151 cloudflare_images-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1152 1970-01-01 00:00:00.000000 cloudflare_images-0.0.4/PKG-INFO
```

### Comparing `cloudflare_images-0.0.3/LICENSE` & `cloudflare_images-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudflare_images-0.0.3/cloudflare_images/api.py` & `cloudflare_images-0.0.4/cloudflare_images/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from typing import Final
 
 import httpx
-from pydantic import BaseSettings, Field
+from pydantic import Field
+from start_cloudflare import CF
 
-CF_API_URL: Final = "https://api.cloudflare.com"
 CF_DELIVER: Final = "https://imagedelivery.net"
 
 
-class CloudflareImagesAPIv1(BaseSettings):
+class CloudflareImagesAPIv1(CF):
     """
     Need to setup a Cloudflare Images account to use. See Cloudflare Images [docs](https://developers.cloudflare.com/images/cloudflare-images/).
     With required variables secured:
 
     Field in .env | Cloudflare API Credential | Where credential found
     :--|:--:|:--
-    `CF_IMG_ACCT` | Account ID |  `https://dash.cloudflare.com/<acct_id>/images/images`
+    `CF_ACCT_ID` | Account ID |  `https://dash.cloudflare.com/<acct_id>/images/images`
     `CF_IMG_HASH` | Account Hash | `https://dash.cloudflare.com/<acct_id>/images/images`
     `CF_IMG_TOKEN` | API Secret | Generate / save via `https://dash.cloudflare.com/<acct_id>/profile/api-tokens`
 
     Add secrets to .env file and use as follows:
 
     Examples:
     ```py title="Example Usage" linenums="1" hl_lines="4 14 23"
     >>> from pathlib import Path
     >>> import os
     >>> import io
     >>> cf = CloudflareImagesAPIv1() # will error out since missing key values
     Traceback (most recent call last):
     pydantic.error_wrappers.ValidationError: 3 validation errors for CloudflareImagesAPIv1
-    acct_id
+    account_id
       field required (type=value_error.missing)
     cf_img_hash
       field required (type=value_error.missing)
     api_token
       field required (type=value_error.missing)
     >>> os.environ['CF_ACCT_ID'] = "ABC"
     >>> cf = CloudflareImagesAPIv1() # will error out since still missing other values
@@ -41,15 +41,15 @@
     cf_img_hash
       field required (type=value_error.missing)
     api_token
       field required (type=value_error.missing)
     >>> # we'll add all the values needed
     >>> os.environ['CF_IMG_HASH'], os.environ['CF_IMG_TOKEN'] = "DEF", "XYZ"
     >>> cf = CloudflareImagesAPIv1() # no longer errors out
-    >>> cf.headers
+    >>> CF.set_bearer_auth(cf.api_token)
     {'Authorization': 'Bearer XYZ'}
     >>> cf.base_api
     'https://api.cloudflare.com/client/v4/accounts/ABC/images/v1'
     >>> cf.base_delivery
     'https://imagedelivery.net/DEF'
     >>> cf.url('hi-bob', 'w=400,sharpen=3')
     'https://imagedelivery.net/DEF/hi-bob/w=400,sharpen=3'
@@ -59,19 +59,19 @@
     >>> img = io.BytesIO(p.read_bytes())
     >>> type(img)
     <class '_io.BytesIO'>
     >>> # Can now use img in `cf.post('sample_id', img)`
     ```
     """  # noqa: E501
 
-    acct_id: str = Field(
+    account_id: str = Field(
         default=...,
         repr=False,
         title="Cloudflare Account ID",
-        description="Used in other Cloudflare services like R2, etc.",
+        description="Overrides the base setting by making this mandatory.",
         env="CF_ACCT_ID",
     )
     cf_img_hash: str = Field(
         default=...,
         repr=False,
         title="Cloudflare Image Hash",
         description="Assigned when you create a Cloudflare Images account",
@@ -102,28 +102,35 @@
     )
 
     class Config:
         env_file = ".env"
         env_file_encoding = "utf-8"
 
     @property
-    def headers(self) -> dict:
-        return {"Authorization": f"Bearer {self.api_token}"}
-
-    @property
     def client(self):
         return httpx.Client(timeout=self.timeout)
 
     @property
-    def base_api(self):
-        """Construct URL based on Cloudflare API [format](https://developers.cloudflare.com/images/cloudflare-images/api-request/)"""  # noqa: E501
-        client = f"client/{self.client_api_ver}"
-        account = f"accounts/{self.acct_id}"
-        images = f"images/{self.images_api_ver}"
-        return "/".join([CF_API_URL, client, account, images])
+    def base_api(self) -> str:
+        """Construct URL based on Cloudflare API [format](https://developers.cloudflare.com/images/cloudflare-images/api-request/)
+
+        Examples:
+            >>> import os
+            >>> os.environ['CF_ACCT_ID'] = "ABC"
+            >>> os.environ['CF_IMG_HASH'], os.environ['CF_IMG_TOKEN'] = "DEF", "XYZ"
+            >>> cf = CloudflareImagesAPIv1()
+            >>> cf.base_api
+            'https://api.cloudflare.com/client/v4/accounts/ABC/images/v1'
+
+        Returns:
+            str: URL endpoint to make requests with the Cloudflare-supplied credentials.
+        """
+        return self.add_account_endpoint(
+            f"/{self.account_id}/images/{self.images_api_ver}"
+        )
 
     @property
     def base_delivery(self):
         """The images are served with the following format:
 
         `https://imagedelivery.net/<ACCOUNT_HASH>/<IMAGE_ID>/<VARIANT_NAME>`
 
@@ -132,17 +139,31 @@
         `https://imagedelivery.net/<ACCOUNT_HASH>`
 
         See Cloudflare [docs](https://developers.cloudflare.com/images/cloudflare-images/serve-images/).
 
         """  # noqa: E501
         return "/".join([CF_DELIVER, self.cf_img_hash])
 
-    def url(self, img_id: str, variant: str = "public"):
+    def url(self, img_id: str, variant: str = "public") -> str:
         """Generates url based on the Cloudflare hash of the account. The `variant` is based on
         how these are customized on Cloudflare Images. See also flexible variant [docs](https://developers.cloudflare.com/images/cloudflare-images/transform/flexible-variants/)
+        Examples:
+            >>> import os
+            >>> os.environ['CF_ACCT_ID'] = "ABC"
+            >>> os.environ['CF_IMG_HASH'], os.environ['CF_IMG_TOKEN'] = "DEF", "XYZ"
+            >>> cf = CloudflareImagesAPIv1()
+            >>> cf.url('sample-img', 'avatar')
+            'https://imagedelivery.net/DEF/sample-img/avatar'
+
+        Args:
+            img_id (str): The uploaded ID
+            variant (str, optional): The variant created in the Cloudflare Images dashboard. Defaults to "public".
+
+        Returns:
+            str: URL to display the request `img_id` with `variant`.
         """  # noqa: E501
         return "/".join([self.base_delivery, img_id, variant])
 
     def get(self, img_id: str, *args, **kwargs) -> httpx.Response:
         """Issue httpx GET request to the image found in storage. Assuming request like
         `CFImage().get('target-img-id')`, returns a response with metadata:
 
@@ -166,33 +187,33 @@
                 "errors": [],
                 "messages": []
             }'
             ```
         """
         return self.client.get(
             url=f"{self.base_api}/{img_id}",
-            headers=self.headers,
+            headers=CF.set_bearer_auth(self.api_token),
             *args,
             **kwargs,
         )
 
     def delete(self, img_id: str, *args, **kwargs) -> httpx.Response:
         """Issue httpx [DELETE](https://developers.cloudflare.com/images/cloudflare-images/transform/delete-images/) request to the image."""  # noqa: E501
         return self.client.delete(
             url=f"{self.base_api}/{img_id}",
-            headers=self.headers,
+            headers=CF.set_bearer_auth(self.api_token),
             *args,
             **kwargs,
         )
 
     def post(self, img_id: str, img: bytes, *args, **kwargs) -> httpx.Response:
         """Issue httpx [POST](https://developers.cloudflare.com/images/cloudflare-images/upload-images/upload-via-url/) request to upload image."""  # noqa: E501
         return self.client.post(
             url=self.base_api,
-            headers=self.headers,
+            headers=CF.set_bearer_auth(self.api_token),
             data={"id": img_id},
             files={"file": (img_id, img)},
             *args,
             **kwargs,
         )
 
     def upsert(self, img_id: str, img: bytes) -> httpx.Response:
```

### Comparing `cloudflare_images-0.0.3/cloudflare_images/django.py` & `cloudflare_images-0.0.4/cloudflare_images/django.py`

 * *Files identical despite different names*

### Comparing `cloudflare_images-0.0.3/pyproject.toml` & `cloudflare_images-0.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cloudflare-images"
 description = "Wrapper around Cloudflare Images API, usable custom Django storage class."
-version = "0.0.3"
+version = "0.0.4"
 authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 homepage = "https://mv3.dev"
 repository = "https://github.com/justmars/cloudflare-images"
 documentation = "https://mv3.dev/cloudflare-images"
 classifiers = [
@@ -14,36 +14,33 @@
   "Typing :: Typed",
   "Development Status :: 4 - Beta",
   "Framework :: Pytest",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-python-dotenv = "^0.21"
 httpx = "^0.24.0"
-pydantic = "^1.10.7"
 django = "^4.2"
+start-cloudflare = "^0.0.1"
 
 [tool.poetry.group.dev.dependencies] # latest as of Jan. 2023
 rich = "^13.3"
-black = "^23.3.0"
 pytest = "^7.2"
 pytest-datadir = "^1.4.1"
 pytest-cov = "^2.12.1"
 pre-commit = "^2.21"
 mkdocs = "^1.4.2"
 mkdocstrings = { extras = ["python"], version = "^0.20.0" }
 mkdocs-material = "^9.1"
-ipykernel = "^6.22.0"
 
 [tool.pytest.ini_options]
 minversion = "7.2"
 addopts = "-ra -q --doctest-modules --cov"
 filterwarnings = ["ignore::DeprecationWarning"]
-testpaths = ["tests"]
+testpaths = ["tests", "cloudflare_images"]
 
 [tool.ruff]
 ignore = ["F401", "F403"]
 fixable = ["F", "E", "W", "I001"]
 select = ["F", "E", "W", "I001"]
 
 [tool.black]
```

### Comparing `cloudflare_images-0.0.3/PKG-INFO` & `cloudflare_images-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudflare-images
-Version: 0.0.3
+Version: 0.0.4
 Summary: Wrapper around Cloudflare Images API, usable custom Django storage class.
 Home-page: https://mv3.dev
 License: BSD-3-Clause
 Author: Marcelino G. Veloso III
 Author-email: mars@veloso.one
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -12,16 +12,15 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Dist: django (>=4.2,<5.0)
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
-Requires-Dist: pydantic (>=1.10.7,<2.0.0)
-Requires-Dist: python-dotenv (>=0.21,<0.22)
+Requires-Dist: start-cloudflare (>=0.0.1,<0.0.2)
 Project-URL: Documentation, https://mv3.dev/cloudflare-images
 Project-URL: Repository, https://github.com/justmars/cloudflare-images
 Description-Content-Type: text/markdown
 
 # cloudflare-images
 
 ![Github CI](https://github.com/justmars/cloudflare-images/actions/workflows/main.yml/badge.svg)
```

