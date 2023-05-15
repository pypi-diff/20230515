# Comparing `tmp/descope-1.5.0.tar.gz` & `tmp/descope-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "descope-1.5.0.tar", max compression
+gzip compressed data, was "descope-1.5.1.tar", max compression
```

## Comparing `descope-1.5.0.tar` & `descope-1.5.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1064 2023-05-07 10:57:55.656598 descope-1.5.0/LICENSE
--rw-r--r--   0        0        0    29105 2023-05-07 10:57:55.656598 descope-1.5.0/README.md
--rw-r--r--   0        0        0      531 2023-05-07 10:57:55.660598 descope-1.5.0/descope/__init__.py
--rw-r--r--   0        0        0      211 2023-05-07 10:57:55.660598 descope-1.5.0/descope/_auth_base.py
--rw-r--r--   0        0        0    20959 2023-05-07 10:57:55.660598 descope-1.5.0/descope/auth.py
--rw-r--r--   0        0        0        0 2023-05-07 10:57:55.660598 descope-1.5.0/descope/authmethod/__init__.py
--rw-r--r--   0        0        0     5319 2023-05-07 10:57:55.660598 descope-1.5.0/descope/authmethod/enchantedlink.py
--rw-r--r--   0        0        0     6200 2023-05-07 10:57:55.660598 descope-1.5.0/descope/authmethod/magiclink.py
--rw-r--r--   0        0        0     1528 2023-05-07 10:57:55.660598 descope-1.5.0/descope/authmethod/oauth.py
--rw-r--r--   0        0        0    11067 2023-05-07 10:57:55.660598 descope-1.5.0/descope/authmethod/otp.py
--rw-r--r--   0        0        0     8146 2023-05-07 10:57:55.660598 descope-1.5.0/descope/authmethod/password.py
--rw-r--r--   0        0        0     1481 2023-05-07 10:57:55.660598 descope-1.5.0/descope/authmethod/saml.py
--rw-r--r--   0        0        0     5128 2023-05-07 10:57:55.660598 descope-1.5.0/descope/authmethod/totp.py
--rw-r--r--   0        0        0     6705 2023-05-07 10:57:55.660598 descope-1.5.0/descope/authmethod/webauthn.py
--rw-r--r--   0        0        0     4296 2023-05-07 10:57:55.660598 descope-1.5.0/descope/common.py
--rw-r--r--   0        0        0    11310 2023-05-07 10:57:55.660598 descope-1.5.0/descope/descope_client.py
--rw-r--r--   0        0        0     1420 2023-05-07 10:57:55.660598 descope-1.5.0/descope/exceptions.py
--rw-r--r--   0        0        0     5798 2023-05-07 10:57:55.660598 descope-1.5.0/descope/management/access_key.py
--rw-r--r--   0        0        0     3811 2023-05-07 10:57:55.660598 descope-1.5.0/descope/management/common.py
--rw-r--r--   0        0        0     3394 2023-05-07 10:57:55.660598 descope-1.5.0/descope/management/flow.py
--rw-r--r--   0        0        0     3971 2023-05-07 10:57:55.660598 descope-1.5.0/descope/management/group.py
--rw-r--r--   0        0        0      959 2023-05-07 10:57:55.660598 descope-1.5.0/descope/management/jwt.py
--rw-r--r--   0        0        0     2531 2023-05-07 10:57:55.660598 descope-1.5.0/descope/management/permission.py
--rw-r--r--   0        0        0     3094 2023-05-07 10:57:55.660598 descope-1.5.0/descope/management/role.py
--rw-r--r--   0        0        0     5895 2023-05-07 10:57:55.660598 descope-1.5.0/descope/management/sso_settings.py
--rw-r--r--   0        0        0     3685 2023-05-07 10:57:55.660598 descope-1.5.0/descope/management/tenant.py
--rw-r--r--   0        0        0    27563 2023-05-07 10:57:55.660598 descope-1.5.0/descope/management/user.py
--rw-r--r--   0        0        0     1556 2023-05-07 10:57:55.660598 descope-1.5.0/descope/mgmt.py
--rw-r--r--   0        0        0     1152 2023-05-07 10:58:19.424900 descope-1.5.0/pyproject.toml
--rw-r--r--   0        0        0    30198 1970-01-01 00:00:00.000000 descope-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-15 15:16:00.107712 descope-1.5.1/LICENSE
+-rw-r--r--   0        0        0    31005 2023-05-15 15:16:00.107712 descope-1.5.1/README.md
+-rw-r--r--   0        0        0      531 2023-05-15 15:16:00.107712 descope-1.5.1/descope/__init__.py
+-rw-r--r--   0        0        0      211 2023-05-15 15:16:00.107712 descope-1.5.1/descope/_auth_base.py
+-rw-r--r--   0        0        0    21437 2023-05-15 15:16:00.107712 descope-1.5.1/descope/auth.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:16:00.107712 descope-1.5.1/descope/authmethod/__init__.py
+-rw-r--r--   0        0        0     5319 2023-05-15 15:16:00.107712 descope-1.5.1/descope/authmethod/enchantedlink.py
+-rw-r--r--   0        0        0     6200 2023-05-15 15:16:00.107712 descope-1.5.1/descope/authmethod/magiclink.py
+-rw-r--r--   0        0        0     1528 2023-05-15 15:16:00.107712 descope-1.5.1/descope/authmethod/oauth.py
+-rw-r--r--   0        0        0    11067 2023-05-15 15:16:00.107712 descope-1.5.1/descope/authmethod/otp.py
+-rw-r--r--   0        0        0     8146 2023-05-15 15:16:00.107712 descope-1.5.1/descope/authmethod/password.py
+-rw-r--r--   0        0        0     1481 2023-05-15 15:16:00.107712 descope-1.5.1/descope/authmethod/saml.py
+-rw-r--r--   0        0        0     5128 2023-05-15 15:16:00.107712 descope-1.5.1/descope/authmethod/totp.py
+-rw-r--r--   0        0        0     6705 2023-05-15 15:16:00.107712 descope-1.5.1/descope/authmethod/webauthn.py
+-rw-r--r--   0        0        0     4296 2023-05-15 15:16:00.107712 descope-1.5.1/descope/common.py
+-rw-r--r--   0        0        0    11583 2023-05-15 15:16:00.107712 descope-1.5.1/descope/descope_client.py
+-rw-r--r--   0        0        0     1420 2023-05-15 15:16:00.107712 descope-1.5.1/descope/exceptions.py
+-rw-r--r--   0        0        0     5798 2023-05-15 15:16:00.107712 descope-1.5.1/descope/management/access_key.py
+-rw-r--r--   0        0        0     3933 2023-05-15 15:16:00.107712 descope-1.5.1/descope/management/common.py
+-rw-r--r--   0        0        0     3394 2023-05-15 15:16:00.107712 descope-1.5.1/descope/management/flow.py
+-rw-r--r--   0        0        0     3971 2023-05-15 15:16:00.107712 descope-1.5.1/descope/management/group.py
+-rw-r--r--   0        0        0      959 2023-05-15 15:16:00.107712 descope-1.5.1/descope/management/jwt.py
+-rw-r--r--   0        0        0     2531 2023-05-15 15:16:00.107712 descope-1.5.1/descope/management/permission.py
+-rw-r--r--   0        0        0     3094 2023-05-15 15:16:00.107712 descope-1.5.1/descope/management/role.py
+-rw-r--r--   0        0        0     5895 2023-05-15 15:16:00.107712 descope-1.5.1/descope/management/sso_settings.py
+-rw-r--r--   0        0        0     3685 2023-05-15 15:16:00.107712 descope-1.5.1/descope/management/tenant.py
+-rw-r--r--   0        0        0    29070 2023-05-15 15:16:00.107712 descope-1.5.1/descope/management/user.py
+-rw-r--r--   0        0        0     1556 2023-05-15 15:16:00.107712 descope-1.5.1/descope/mgmt.py
+-rw-r--r--   0        0        0     1220 2023-05-15 15:16:27.592050 descope-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0    32073 1970-01-01 00:00:00.000000 descope-1.5.1/PKG-INFO
```

### Comparing `descope-1.5.0/LICENSE` & `descope-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `descope-1.5.0/README.md` & `descope-1.5.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -26,17 +26,48 @@
 # Initialized after setting the DESCOPE_PROJECT_ID env var
 descope_client = DescopeClient()
 
 # ** Or directly **
 descope_client = DescopeClient(project_id="<Project ID>")
 ```
 
-## Usage
+## Authentication Functions
 
-Here are some examples how to manage and authenticate users:
+These sections show how to use the SDK to perform various authentication/authorization functions:
+
+1. [OTP Authentication](#otp-authentication)
+2. [Magic Link](#magic-link)
+3. [Enchanted Link](#enchanted-link)
+4. [OAuth](#oauth)
+5. [SSO/SAML](#ssosaml)
+6. [TOTP Authentication](#totp-authentication)
+7. [Passwords](#passwords)
+8. [Session Validation](#session-validation)
+9. [Roles & Permission Validation](#roles--permission-validation)
+10. [Logging Out](#logging-out)
+
+## API Managment Function
+
+These sections show how to use the SDK to perform permission and user management functions. You will need to create an instance of `DescopeClient` by following the [Setup](#setup-1) guide, before you can use any of these functions:
+
+1. [Manage Tenants](#manage-tenants)
+2. [Manage Users](#manage-users)
+3. [Manage Access Keys](#manage-access-keys)
+4. [Manage SSO Setting](#manage-sso-setting)
+5. [Manage Permissions](#manage-permissions)
+6. [Manage Roles](#manage-roles)
+7. [Query SSO Groups](#query-sso-groups)
+8. [Manage Flows](#manage-flows)
+9. [Manage JWTs](#manage-jwts)
+
+If you wish to run any of our code samples and play with them, check out our [Code Examples](#code-examples) section.
+
+If you're performing end-to-end testing, check out the [Utils for your end to end (e2e) tests and integration tests](#utils-for-your-end-to-end-e2e-tests-and-integration-tests) section. You will need to use the `DescopeClient` object created under [Setup](#setup-1) guide.
+
+For rate limiting information, please confer to the [API Rate Limits](#api-rate-limits) section.
 
 ### OTP Authentication
 
 Send a user a one-time password (OTP) using your preferred delivery method (_email / SMS_). An email address or phone number must be provided accordingly.
 
 The user can either `sign up`, `sign in` or `sign up or in`
 
@@ -441,15 +472,15 @@
 tenants = tenants_resp["tenants"]
     for tenant in tenants:
         # Do something
 ```
 
 ### Manage Users
 
-You can create, update, delete or load users, as well as search according to filters:
+You can create, update, delete or load users, as well as setting new password, expire password and search according to filters:
 
 ```Python
 # A user must have a login ID, other fields are optional.
 # Roles should be set directly if no tenants exist, otherwise set
 # on a per-tenant basis.
 descope_client.mgmt.user.create(
     login_id="desmond@descope.com",
@@ -509,14 +540,28 @@
 # results can be paginated using the limit and page parameters
 users_resp = descope_client.mgmt.user.search_all(tenant_ids=["my-tenant-id"])
 users = users_resp["users"]
     for user in users:
         # Do something
 ```
 
+#### Set or Expire User Password
+
+You can set or expire a user's password.
+Note: When setting a password, it will automatically be set as expired.
+The user will not be able log-in using an expired password, and will be required replace it on next login.
+
+```Python
+// Set a user's password
+descope_client.mgmt.user.setPassword('<login-id>', '<some-password>');
+
+// Or alternatively, expire a user password
+descope_client.mgmt.user.expirePassword('<login-id>');
+```
+
 ### Manage Access Keys
 
 You can create, update, delete or load access keys, as well as search according to filters:
 
 ```Python
 # An access key must have a name and expiration, other fields are optional.
 # Roles should be set directly if no tenants exist, otherwise set
@@ -773,17 +818,17 @@
 link = resp["link"]
 pending_ref = resp["pendingRef"]
 
 # Note 1: The generate code/link functions, work only for test users, will not work for regular users.
 # Note 2: In case of testing sign-in / sign-up operations with test users, need to make sure to generate the code prior calling the sign-in / sign-up operations.
 ```
 
-## API Rate limits
+## API Rate Limits
 
-Handle API rate limits by comparing the exception to the APIRateLimitExceeded exception, which includes the RateLimitParameters map with the key "Retry-After." This key indicates how many seconds until the next valid API call can take place. More information on Descope's rate limit is covered here: [Descope rate limit reference page](https://docs.descope.com/rate-limit)
+Handle API rate limits by comparing the exception to the APIRateLimitExceeded exception, which includes the RateLimitParameters map with the key "Retry-After." This key indicates how many seconds until the next valid API call can take place.
 
 ```python
 try:
     descope_client.magiclink.sign_up_or_in(
         method=DeliveryMethod.EMAIL,
         login_id="desmond@descope.com",
         uri="http://myapp.com/verify-magic-link",
```

### Comparing `descope-1.5.0/descope/__init__.py` & `descope-1.5.1/descope/__init__.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.0/descope/auth.py` & `descope-1.5.1/descope/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 import json
 import os
 import platform
 import re
 from threading import Lock
 from typing import Tuple
 
@@ -398,33 +399,40 @@
             ).get("permissions", [])
             jwt_response["roles"] = jwt_response.get(REFRESH_SESSION_TOKEN_NAME).get(
                 "roles", []
             )
             jwt_response["tenants"] = jwt_response.get(REFRESH_SESSION_TOKEN_NAME).get(
                 "tenants", {}
             )
+        else:
+            jwt_response["permissions"] = jwt_response.get("permissions", [])
+            jwt_response["roles"] = jwt_response.get("roles", [])
+            jwt_response["tenants"] = jwt_response.get("tenants", {})
 
         # Save the projectID also in the dict top level
-        issuer = jwt_response.get(SESSION_TOKEN_NAME, {}).get(
-            "iss", None
-        ) or jwt_response.get(REFRESH_SESSION_TOKEN_NAME, {}).get("iss", "")
+        issuer = (
+            jwt_response.get(SESSION_TOKEN_NAME, {}).get("iss", None)
+            or jwt_response.get(REFRESH_SESSION_TOKEN_NAME, {}).get("iss", None)
+            or jwt_response.get("iss", "")
+        )
         jwt_response["projectId"] = issuer.rsplit("/")[
             -1
         ]  # support both url issuer and project ID issuer
 
+        sub = (
+            jwt_response.get(SESSION_TOKEN_NAME, {}).get("sub", None)
+            or jwt_response.get(REFRESH_SESSION_TOKEN_NAME, {}).get("sub", None)
+            or jwt_response.get("sub", "")
+        )
         if user_jwt:
             # Save the userID also in the dict top level
-            jwt_response["userId"] = jwt_response.get(SESSION_TOKEN_NAME, {}).get(
-                "sub", None
-            ) or jwt_response.get(REFRESH_SESSION_TOKEN_NAME, {}).get("sub", None)
+            jwt_response["userId"] = sub
         else:
             # Save the AccessKeyID also in the dict top level
-            jwt_response["keyId"] = jwt_response.get(SESSION_TOKEN_NAME, {}).get(
-                "sub", None
-            )
+            jwt_response["keyId"] = sub
 
         return jwt_response
 
     def _generate_auth_info(
         self, response_body: dict, refresh_token: str, user_jwt: bool
     ) -> dict:
         jwt_response = {}
@@ -539,14 +547,17 @@
                 400,
                 ERROR_TYPE_INVALID_TOKEN,
                 "Session token is required for validation",
             )
 
         try:
             res = self._validate_token(session_token)
+            res[SESSION_TOKEN_NAME] = copy.deepcopy(
+                res
+            )  # Duplicate for saving backward compatibility but keep the same structure as the refresh operation response
             return self.adjust_properties(res, True)
         except RateLimitException as e:
             raise e
         except Exception as e:
             raise AuthException(
                 401, ERROR_TYPE_INVALID_TOKEN, f"Invalid session token: {e}"
             )
```

### Comparing `descope-1.5.0/descope/authmethod/enchantedlink.py` & `descope-1.5.1/descope/authmethod/enchantedlink.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.0/descope/authmethod/magiclink.py` & `descope-1.5.1/descope/authmethod/magiclink.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.0/descope/authmethod/oauth.py` & `descope-1.5.1/descope/authmethod/oauth.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.0/descope/authmethod/otp.py` & `descope-1.5.1/descope/authmethod/otp.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.0/descope/authmethod/password.py` & `descope-1.5.1/descope/authmethod/password.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.0/descope/authmethod/saml.py` & `descope-1.5.1/descope/authmethod/saml.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.0/descope/authmethod/totp.py` & `descope-1.5.1/descope/authmethod/totp.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.0/descope/authmethod/webauthn.py` & `descope-1.5.1/descope/authmethod/webauthn.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.0/descope/common.py` & `descope-1.5.1/descope/common.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.0/descope/descope_client.py` & `descope-1.5.1/descope/descope_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -171,15 +171,18 @@
                 return False
         return True
 
     def validate_session(self, session_token: str) -> dict:
         """
         Validate a session token. Call this function for every incoming request to your
         private endpoints. Alternatively, use validate_and_refresh_session in order to
-        automatically refresh expired sessions.
+        automatically refresh expired sessions. If you need to use these specific claims
+        [amr, drn, exp, iss, rexp, sub, jwt] in the top level of the response dict, please use
+        them from the sessionToken key instead, as these claims will soon be deprecated from the top level
+        of the response dict.
 
         Args:
         session_token (str): The session token to be validated
 
         Return value (dict):
         Return dict includes the session token and all JWT claims
```

### Comparing `descope-1.5.0/descope/exceptions.py` & `descope-1.5.1/descope/exceptions.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.0/descope/management/access_key.py` & `descope-1.5.1/descope/management/access_key.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.0/descope/management/common.py` & `descope-1.5.1/descope/management/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     user_update_email_path = "/v1/mgmt/user/update/email"
     user_update_phone_path = "/v1/mgmt/user/update/phone"
     user_update_name_path = "/v1/mgmt/user/update/name"
     user_update_picture_path = "/v1/mgmt/user/update/picture"
     user_update_custom_attribute_path = "/v1/mgmt/user/update/customAttribute"
     user_add_role_path = "/v1/mgmt/user/update/role/add"
     user_remove_role_path = "/v1/mgmt/user/update/role/remove"
+    user_set_password_path = "/v1/mgmt/user/password/set"
+    user_expire_password_path = "/v1/mgmt/user/password/expire"
     user_add_tenant_path = "/v1/mgmt/user/update/tenant/add"
     user_remove_tenant_path = "/v1/mgmt/user/update/tenant/remove"
     user_generate_otp_for_test_path = "/v1/mgmt/tests/generate/otp"
     user_generate_magic_link_for_test_path = "/v1/mgmt/tests/generate/magiclink"
     user_generate_enchanted_link_for_test_path = "/v1/mgmt/tests/generate/enchantedlink"
 
     # access key
```

### Comparing `descope-1.5.0/descope/management/flow.py` & `descope-1.5.1/descope/management/flow.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.0/descope/management/group.py` & `descope-1.5.1/descope/management/group.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.0/descope/management/jwt.py` & `descope-1.5.1/descope/management/jwt.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.0/descope/management/permission.py` & `descope-1.5.1/descope/management/permission.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.0/descope/management/role.py` & `descope-1.5.1/descope/management/role.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.0/descope/management/sso_settings.py` & `descope-1.5.1/descope/management/sso_settings.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.0/descope/management/tenant.py` & `descope-1.5.1/descope/management/tenant.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.0/descope/management/user.py` & `descope-1.5.1/descope/management/user.py`

 * *Files 8% similar despite different names*

```diff
@@ -715,14 +715,61 @@
         response = self._auth.do_post(
             MgmtV1.user_remove_role_path,
             {"loginId": login_id, "tenantId": tenant_id, "roleNames": role_names},
             pswd=self._auth.management_key,
         )
         return response.json()
 
+    def set_password(
+        self,
+        login_id: str,
+        password: str,
+    ) -> None:
+        """
+            Set the password for the given login ID.
+            Note: The password will automatically be set as expired.
+            The user will not be able to log-in with this password, and will be required to replace it on next login.
+            See also: expire_password
+
+        Args:
+        login_id (str): The login ID of the user to set the password to.
+        password (str): The new password to set to the user.
+
+        Raise:
+        AuthException: raised if the operation fails
+        """
+        self._auth.do_post(
+            MgmtV1.user_set_password_path,
+            {"loginId": login_id, "password": password},
+            pswd=self._auth.management_key,
+        )
+        return
+
+    def expire_password(
+        self,
+        login_id: str,
+    ) -> None:
+        """
+            Expires the password for the given login ID.
+            Note: user sign-in with an expired password, the user will get an error with code.
+            Use the `password.send_reset` or `password.replace` methods to reset/replace the password.
+
+        Args:
+        login_id (str): The login ID of the user expire the password to.
+
+        Raise:
+        AuthException: raised if the operation fails
+        """
+        self._auth.do_post(
+            MgmtV1.user_expire_password_path,
+            {"loginId": login_id},
+            pswd=self._auth.management_key,
+        )
+        return
+
     def generate_otp_for_test_user(
         self,
         method: DeliveryMethod,
         login_id: str,
     ) -> dict:
         """
         Generate OTP for the given login ID of a test user.
```

### Comparing `descope-1.5.0/descope/mgmt.py` & `descope-1.5.1/descope/mgmt.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.0/pyproject.toml` & `descope-1.5.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "descope"
-version = "1.5.0"
+version = "1.5.1"
 description = "Descope Python SDK"
 authors = ["Descope <info@descope.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://descope.com/"
 repository = "https://github.com/descope/python-sdk"
 documentation = "https://docs.descope.com"
@@ -21,28 +21,27 @@
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/descope/python-sdk/issues"
 
 
 [tool.poetry.dependencies]
 python = "^3.7"
-requests = "2.28.2"
-PyJWT = "==2.6.0"
-cryptography = "==40.0.2"
-email-validator = "==1.3.1"
+requests = "2.30.0" # First support for python 3.10
+PyJWT = {version = "2.7.0", extras = ["crypto"]} # Latest secrutiy update
+email-validator = "==2.0.0.post2"
 
 [tool.poetry.group.dev.dependencies]
 mock = "5.0.2"
 pre-commit = "2.21.0"
 Flask = "2.2.5"
 flake8 = "5.0.4"
 flake8-bugbear = "22.12.6"
 pytest-cov = "4.0.0"
 pytest = "7.3.1"
 black = "23.3.0"
-liccheck = "0.8.3"
+liccheck = "0.9.0"
 isort = "5.11.4"
 pep8-naming = "0.13.3"
 
 [build-system]
 requires = ["poetry-core>=1.1.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `descope-1.5.0/PKG-INFO` & `descope-1.5.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: descope
-Version: 1.5.0
+Version: 1.5.1
 Summary: Descope Python SDK
 Home-page: https://descope.com/
 License: MIT
 Author: Descope
 Author-email: info@descope.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -13,18 +13,17 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: PyJWT (==2.6.0)
-Requires-Dist: cryptography (==40.0.2)
-Requires-Dist: email-validator (==1.3.1)
-Requires-Dist: requests (==2.28.2)
+Requires-Dist: PyJWT[crypto] (==2.7.0)
+Requires-Dist: email-validator (==2.0.0.post2)
+Requires-Dist: requests (==2.30.0)
 Project-URL: Bug Tracker, https://github.com/descope/python-sdk/issues
 Project-URL: Documentation, https://docs.descope.com
 Project-URL: Repository, https://github.com/descope/python-sdk
 Description-Content-Type: text/markdown
 
 # Descope SDK for Python
 
@@ -54,17 +53,48 @@
 # Initialized after setting the DESCOPE_PROJECT_ID env var
 descope_client = DescopeClient()
 
 # ** Or directly **
 descope_client = DescopeClient(project_id="<Project ID>")
 ```
 
-## Usage
+## Authentication Functions
 
-Here are some examples how to manage and authenticate users:
+These sections show how to use the SDK to perform various authentication/authorization functions:
+
+1. [OTP Authentication](#otp-authentication)
+2. [Magic Link](#magic-link)
+3. [Enchanted Link](#enchanted-link)
+4. [OAuth](#oauth)
+5. [SSO/SAML](#ssosaml)
+6. [TOTP Authentication](#totp-authentication)
+7. [Passwords](#passwords)
+8. [Session Validation](#session-validation)
+9. [Roles & Permission Validation](#roles--permission-validation)
+10. [Logging Out](#logging-out)
+
+## API Managment Function
+
+These sections show how to use the SDK to perform permission and user management functions. You will need to create an instance of `DescopeClient` by following the [Setup](#setup-1) guide, before you can use any of these functions:
+
+1. [Manage Tenants](#manage-tenants)
+2. [Manage Users](#manage-users)
+3. [Manage Access Keys](#manage-access-keys)
+4. [Manage SSO Setting](#manage-sso-setting)
+5. [Manage Permissions](#manage-permissions)
+6. [Manage Roles](#manage-roles)
+7. [Query SSO Groups](#query-sso-groups)
+8. [Manage Flows](#manage-flows)
+9. [Manage JWTs](#manage-jwts)
+
+If you wish to run any of our code samples and play with them, check out our [Code Examples](#code-examples) section.
+
+If you're performing end-to-end testing, check out the [Utils for your end to end (e2e) tests and integration tests](#utils-for-your-end-to-end-e2e-tests-and-integration-tests) section. You will need to use the `DescopeClient` object created under [Setup](#setup-1) guide.
+
+For rate limiting information, please confer to the [API Rate Limits](#api-rate-limits) section.
 
 ### OTP Authentication
 
 Send a user a one-time password (OTP) using your preferred delivery method (_email / SMS_). An email address or phone number must be provided accordingly.
 
 The user can either `sign up`, `sign in` or `sign up or in`
 
@@ -469,15 +499,15 @@
 tenants = tenants_resp["tenants"]
     for tenant in tenants:
         # Do something
 ```
 
 ### Manage Users
 
-You can create, update, delete or load users, as well as search according to filters:
+You can create, update, delete or load users, as well as setting new password, expire password and search according to filters:
 
 ```Python
 # A user must have a login ID, other fields are optional.
 # Roles should be set directly if no tenants exist, otherwise set
 # on a per-tenant basis.
 descope_client.mgmt.user.create(
     login_id="desmond@descope.com",
@@ -537,14 +567,28 @@
 # results can be paginated using the limit and page parameters
 users_resp = descope_client.mgmt.user.search_all(tenant_ids=["my-tenant-id"])
 users = users_resp["users"]
     for user in users:
         # Do something
 ```
 
+#### Set or Expire User Password
+
+You can set or expire a user's password.
+Note: When setting a password, it will automatically be set as expired.
+The user will not be able log-in using an expired password, and will be required replace it on next login.
+
+```Python
+// Set a user's password
+descope_client.mgmt.user.setPassword('<login-id>', '<some-password>');
+
+// Or alternatively, expire a user password
+descope_client.mgmt.user.expirePassword('<login-id>');
+```
+
 ### Manage Access Keys
 
 You can create, update, delete or load access keys, as well as search according to filters:
 
 ```Python
 # An access key must have a name and expiration, other fields are optional.
 # Roles should be set directly if no tenants exist, otherwise set
@@ -801,17 +845,17 @@
 link = resp["link"]
 pending_ref = resp["pendingRef"]
 
 # Note 1: The generate code/link functions, work only for test users, will not work for regular users.
 # Note 2: In case of testing sign-in / sign-up operations with test users, need to make sure to generate the code prior calling the sign-in / sign-up operations.
 ```
 
-## API Rate limits
+## API Rate Limits
 
-Handle API rate limits by comparing the exception to the APIRateLimitExceeded exception, which includes the RateLimitParameters map with the key "Retry-After." This key indicates how many seconds until the next valid API call can take place. More information on Descope's rate limit is covered here: [Descope rate limit reference page](https://docs.descope.com/rate-limit)
+Handle API rate limits by comparing the exception to the APIRateLimitExceeded exception, which includes the RateLimitParameters map with the key "Retry-After." This key indicates how many seconds until the next valid API call can take place.
 
 ```python
 try:
     descope_client.magiclink.sign_up_or_in(
         method=DeliveryMethod.EMAIL,
         login_id="desmond@descope.com",
         uri="http://myapp.com/verify-magic-link",
```

