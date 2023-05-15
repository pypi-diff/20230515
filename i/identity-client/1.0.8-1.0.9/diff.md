# Comparing `tmp/identity_client-1.0.8.tar.gz` & `tmp/identity_client-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/identity_client-1.0.8.tar", last modified: Wed May  6 14:21:52 2020, max compression
+gzip compressed data, was "dist/identity_client-1.0.9.tar", last modified: Fri May  8 08:22:12 2020, max compression
```

## Comparing `identity_client-1.0.8.tar` & `identity_client-1.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-05-06 14:21:52.000000 identity_client-1.0.8/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1080 2020-05-06 14:21:52.000000 identity_client-1.0.8/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       54 2020-05-06 14:21:29.000000 identity_client-1.0.8/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-05-06 14:21:52.000000 identity_client-1.0.8/identity_client/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2020-05-06 14:21:29.000000 identity_client-1.0.8/identity_client/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3188 2020-05-06 14:21:29.000000 identity_client-1.0.8/identity_client/identity_session_auth.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4267 2020-05-06 14:21:29.000000 identity_client-1.0.8/identity_client/views.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-05-06 14:21:52.000000 identity_client-1.0.8/identity_client.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1080 2020-05-06 14:21:52.000000 identity_client-1.0.8/identity_client.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      306 2020-05-06 14:21:52.000000 identity_client-1.0.8/identity_client.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2020-05-06 14:21:52.000000 identity_client-1.0.8/identity_client.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       57 2020-05-06 14:21:52.000000 identity_client-1.0.8/identity_client.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       16 2020-05-06 14:21:52.000000 identity_client-1.0.8/identity_client.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2020-05-06 14:21:52.000000 identity_client-1.0.8/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1424 2020-05-06 14:21:52.000000 identity_client-1.0.8/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-05-08 08:22:12.000000 identity_client-1.0.9/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1080 2020-05-08 08:22:12.000000 identity_client-1.0.9/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       54 2020-05-08 08:21:58.000000 identity_client-1.0.9/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-05-08 08:22:12.000000 identity_client-1.0.9/identity_client/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2020-05-08 08:21:58.000000 identity_client-1.0.9/identity_client/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3264 2020-05-08 08:21:58.000000 identity_client-1.0.9/identity_client/identity_session_auth.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4333 2020-05-08 08:21:58.000000 identity_client-1.0.9/identity_client/views.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-05-08 08:22:12.000000 identity_client-1.0.9/identity_client.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1080 2020-05-08 08:22:12.000000 identity_client-1.0.9/identity_client.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      306 2020-05-08 08:22:12.000000 identity_client-1.0.9/identity_client.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2020-05-08 08:22:12.000000 identity_client-1.0.9/identity_client.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       57 2020-05-08 08:22:12.000000 identity_client-1.0.9/identity_client.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       16 2020-05-08 08:22:12.000000 identity_client-1.0.9/identity_client.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2020-05-08 08:22:12.000000 identity_client-1.0.9/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1424 2020-05-08 08:22:12.000000 identity_client-1.0.9/setup.py
```

### Comparing `identity_client-1.0.8/PKG-INFO` & `identity_client-1.0.9/identity_client.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: identity_client
-Version: 1.0.8
+Name: identity-client
+Version: 1.0.9
 Summary: A middleware and a set of handlers to handle Code Grant authentication with Cognito
 Home-page: UNKNOWN
 Author: STITCH
 Author-email: panovitch@gmail.com
 License: MIT
 Description: # identity-client
         Client lib for the identity service
```

### Comparing `identity_client-1.0.8/identity_client/identity_session_auth.py` & `identity_client-1.0.9/identity_client/identity_session_auth.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from urllib.parse import urljoin
 from rest_framework import authentication
 from django.contrib.auth.models import User
 from django.conf import settings
 from rest_framework import exceptions
 import requests
 
 
@@ -30,17 +31,18 @@
     """
 
     def authenticate(self, request):
         shared_cookie = request.COOKIES.get("sso_shared_session")
         if not shared_cookie:
             # auth not attempted
             return None
+
+        validate_url = urljoin(settings.IDENTITY_HOST, "internal/sessions/validate/")
         user_info_reply = requests.post(
-            f"{settings.IDENTITY_HOST}/auth/validate_sso_session/",
-            json={"sso_session_cookie": shared_cookie},
+            validate_url, json={"sso_session_cookie": shared_cookie},
         )
 
         try:
             user_info_reply.raise_for_status()
         except requests.exceptions.HTTPError as e:
             message = (
                 "User info request failed",
@@ -62,18 +64,17 @@
     """
 
     def authenticate(self, request):
         api_key = request.META.get("HTTP_X_USER_API_KEY")
         if not api_key:
             # auth not attempted
             return None
-        user_info_reply = requests.post(
-            f"{settings.IDENTITY_HOST}/internal/api_keys/validate/",
-            json={"api_key": api_key},
-        )
+
+        validate_url = urljoin(settings.IDENTITY_HOST, "internal/api_keys/validate/")
+        user_info_reply = requests.post(validate_url, json={"api_key": api_key},)
 
         try:
             user_info_reply.raise_for_status()
         except requests.exceptions.HTTPError as e:
             message = (
                 "User info request failed",
                 e.response.status_code,
```

### Comparing `identity_client-1.0.8/identity_client/views.py` & `identity_client-1.0.9/identity_client/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from django.urls import path, include
 from django.contrib.auth.models import User
-from rest_framework.decorators import api_view, permission_classes, authentication_classes
+from rest_framework.decorators import (
+    api_view,
+    permission_classes,
+    authentication_classes,
+)
 from rest_framework.permissions import AllowAny
 from rest_framework.response import Response
 from django.utils.timezone import now
 from django.contrib.sessions.models import Session
-
+from urllib.parse import urljoin
 import requests
 from django.conf import settings
 from django.http import HttpResponseRedirect, HttpResponse, HttpResponseBadRequest
 
 
 def include_auth_urls():
     return include([path(r"login/", login), path(r"logout/", logout)])
@@ -28,16 +32,17 @@
     auth_redirect_url = auth_redirect_url.replace("http", "https")
     auth_code: str = request.query_params.get("code", "")
     app_redirect_url: str = request.query_params.get("state", "")
 
     client_id = settings.IDENTITY_CLIENT_ID
     client_secret = settings.IDENTITY_CLIENT_SECRET
 
+    token_url = urljoin(settings.IDENTITY_HOST, "/o/token/")
     reply = requests.post(
-        f"{settings.IDENTITY_HOST}/o/token/",
+        token_url,
         data={
             "grant_type": "authorization_code",
             "code": auth_code,
             "redirect_uri": auth_redirect_url,
         },
         auth=(client_id, client_secret),
     )
@@ -49,16 +54,17 @@
             e.response.status_code,
             e.response.content,
             auth_redirect_url,
         )
         return HttpResponse(f"Unauthorized: {message}", status=401)
 
     tokens = reply.json()
+    introspect_url = urljoin(settings.IDENTITY_HOST, "/o/introspect/")
     introspect_response = requests.post(
-        f"{settings.IDENTITY_HOST}/o/introspect/",
+        introspect_url,
         data={"token": tokens["access_token"],},
         headers={"Authorization": "Bearer " + tokens["access_token"]},
     )
     try:
         reply.raise_for_status()
     except requests.exceptions.HTTPError as e:
         message = (
@@ -77,19 +83,18 @@
     return HttpResponseRedirect(redirect_to=app_redirect_url)
 
 
 @api_view(["GET"])
 @permission_classes([AllowAny])
 @authentication_classes([])
 def logout(request):
-    app_redirect_url: str = request.query_params.get("state", "")
     request.session.flush()
-    response = HttpResponseRedirect(redirect_to=app_redirect_url)
-    sso_domain = getattr(settings, "IDENTITY_SSO_DOMAIN", None)
-    response.delete_cookie("sso_shared_session", domain=sso_domain)
+    state: str = request.query_params.get("state", "")
+    redirect_url = urljoin(settings.IDENTITY_HOST, "auth/logout/")
+    response = HttpResponseRedirect(redirect_to=f"{redirect_url}?state={state}")
     return response
 
 
 @api_view(["POST"])
 @permission_classes([AllowAny])
 @authentication_classes([])
 def flush_session_view(request):
```

### Comparing `identity_client-1.0.8/identity_client.egg-info/PKG-INFO` & `identity_client-1.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: identity-client
-Version: 1.0.8
+Name: identity_client
+Version: 1.0.9
 Summary: A middleware and a set of handlers to handle Code Grant authentication with Cognito
 Home-page: UNKNOWN
 Author: STITCH
 Author-email: panovitch@gmail.com
 License: MIT
 Description: # identity-client
         Client lib for the identity service
```

### Comparing `identity_client-1.0.8/setup.py` & `identity_client-1.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 def readall(path):
     with open(path, encoding="utf-8") as fp:
         return fp.read()
 
 
 setup(
     name="identity_client",
-    version="1.0.8",
+    version="1.0.9",
     description="A middleware and a set of handlers to handle "
     "Code Grant authentication with Cognito",
     long_description=readall("README.md"),
     long_description_content_type="text/markdown",
     author="STITCH",
     author_email="panovitch@gmail.com",
     license="MIT",
```

