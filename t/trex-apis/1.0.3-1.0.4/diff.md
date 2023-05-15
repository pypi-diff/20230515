# Comparing `tmp/trex-apis-1.0.3.tar.gz` & `tmp/trex-apis-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trex-apis-1.0.3.tar", last modified: Mon May 15 02:08:24 2023, max compression
+gzip compressed data, was "trex-apis-1.0.4.tar", last modified: Mon May 15 06:06:52 2023, max compression
```

## Comparing `trex-apis-1.0.3.tar` & `trex-apis-1.0.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 02:08:24.915940 trex-apis-1.0.3/
--rw-r--r--   0 jacklok    (501) staff       (20)      447 2023-05-15 02:08:24.916204 trex-apis-1.0.3/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)       25 2021-06-30 02:28:26.000000 trex-apis-1.0.3/README.md
--rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-05-15 02:08:24.917218 trex-apis-1.0.3/setup.cfg
--rw-r--r--   0 jacklok    (501) staff       (20)      713 2023-05-15 02:07:30.000000 trex-apis-1.0.3/setup.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 02:08:24.889255 trex-apis-1.0.3/trex_apis.egg-info/
--rw-r--r--   0 jacklok    (501) staff       (20)      447 2023-05-15 02:08:24.000000 trex-apis-1.0.3/trex_apis.egg-info/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)     1328 2023-05-15 02:08:24.000000 trex-apis-1.0.3/trex_apis.egg-info/SOURCES.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-05-15 02:08:24.000000 trex-apis-1.0.3/trex_apis.egg-info/dependency_links.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       23 2023-05-15 02:08:24.000000 trex-apis-1.0.3/trex_apis.egg-info/requires.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        8 2023-05-15 02:08:24.000000 trex-apis-1.0.3/trex_apis.egg-info/top_level.txt
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 02:08:24.889793 trex-apis-1.0.3/trexapi/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:30:07.000000 trex-apis-1.0.3/trexapi/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      837 2023-04-19 06:13:09.000000 trex-apis-1.0.3/trexapi/conf.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 02:08:24.905620 trex-apis-1.0.3/trexapi/controllers/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:45:28.000000 trex-apis-1.0.3/trexapi/controllers/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)    11544 2023-04-24 08:15:59.000000 trex-apis-1.0.3/trexapi/controllers/api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2259 2022-11-14 14:26:16.000000 trex-apis-1.0.3/trexapi/controllers/app_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    35947 2023-05-05 09:27:49.000000 trex-apis-1.0.3/trexapi/controllers/customer_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     6945 2023-04-13 05:36:42.000000 trex-apis-1.0.3/trexapi/controllers/customer_membership_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4750 2023-01-30 07:03:11.000000 trex-apis-1.0.3/trexapi/controllers/customer_reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    13204 2023-05-15 02:06:38.000000 trex-apis-1.0.3/trexapi/controllers/loyalty_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1214 2023-05-07 13:49:51.000000 trex-apis-1.0.3/trexapi/controllers/lucky_draw_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    11170 2023-05-05 09:32:39.000000 trex-apis-1.0.3/trexapi/controllers/outlet_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1430 2022-09-26 04:18:01.000000 trex-apis-1.0.3/trexapi/controllers/payment_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    22728 2023-01-13 04:39:15.000000 trex-apis-1.0.3/trexapi/controllers/pos_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    27329 2023-04-18 07:01:48.000000 trex-apis-1.0.3/trexapi/controllers/reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7315 2023-04-20 09:46:08.000000 trex-apis-1.0.3/trexapi/controllers/sales_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)      998 2023-04-18 06:08:18.000000 trex-apis-1.0.3/trexapi/controllers/transaction_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    43378 2023-05-12 14:04:03.000000 trex-apis-1.0.3/trexapi/controllers/user_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2980 2023-01-30 02:56:35.000000 trex-apis-1.0.3/trexapi/controllers/user_reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    15185 2023-04-07 15:27:24.000000 trex-apis-1.0.3/trexapi/controllers/voucher_api_routes.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 02:08:24.906656 trex-apis-1.0.3/trexapi/decorators/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-01 08:42:13.000000 trex-apis-1.0.3/trexapi/decorators/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4734 2023-05-05 09:06:37.000000 trex-apis-1.0.3/trexapi/decorators/api_decorators.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 02:08:24.910101 trex-apis-1.0.3/trexapi/forms/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-12 06:42:53.000000 trex-apis-1.0.3/trexapi/forms/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7419 2023-02-08 10:14:32.000000 trex-apis-1.0.3/trexapi/forms/customer_api_forms.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7285 2023-04-18 02:42:03.000000 trex-apis-1.0.3/trexapi/forms/reward_api_forms.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1547 2023-04-18 02:41:54.000000 trex-apis-1.0.3/trexapi/forms/sales_api_forms.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2505 2023-05-09 02:01:04.000000 trex-apis-1.0.3/trexapi/forms/user_api_forms.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 02:08:24.911393 trex-apis-1.0.3/trexapi/libs/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-05 10:17:19.000000 trex-apis-1.0.3/trexapi/libs/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1143 2021-07-05 10:57:23.000000 trex-apis-1.0.3/trexapi/libs/flask_auth_wrapper.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 02:08:24.913672 trex-apis-1.0.3/trexapi/utils/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-08 10:01:06.000000 trex-apis-1.0.3/trexapi/utils/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1347 2022-12-20 01:23:01.000000 trex-apis-1.0.3/trexapi/utils/api_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)    76256 2023-04-24 10:05:07.000000 trex-apis-1.0.3/trexapi/utils/reward_transaction_helper.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 06:06:52.119286 trex-apis-1.0.4/
+-rw-r--r--   0 jacklok    (501) staff       (20)      447 2023-05-15 06:06:52.119410 trex-apis-1.0.4/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)       25 2021-06-30 02:28:26.000000 trex-apis-1.0.4/README.md
+-rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-05-15 06:06:52.119850 trex-apis-1.0.4/setup.cfg
+-rw-r--r--   0 jacklok    (501) staff       (20)      713 2023-05-15 06:06:46.000000 trex-apis-1.0.4/setup.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 06:06:52.096436 trex-apis-1.0.4/trex_apis.egg-info/
+-rw-r--r--   0 jacklok    (501) staff       (20)      447 2023-05-15 06:06:51.000000 trex-apis-1.0.4/trex_apis.egg-info/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)     1328 2023-05-15 06:06:51.000000 trex-apis-1.0.4/trex_apis.egg-info/SOURCES.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-05-15 06:06:51.000000 trex-apis-1.0.4/trex_apis.egg-info/dependency_links.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       23 2023-05-15 06:06:51.000000 trex-apis-1.0.4/trex_apis.egg-info/requires.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        8 2023-05-15 06:06:51.000000 trex-apis-1.0.4/trex_apis.egg-info/top_level.txt
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 06:06:52.096992 trex-apis-1.0.4/trexapi/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:30:07.000000 trex-apis-1.0.4/trexapi/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      837 2023-04-19 06:13:09.000000 trex-apis-1.0.4/trexapi/conf.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 06:06:52.111374 trex-apis-1.0.4/trexapi/controllers/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:45:28.000000 trex-apis-1.0.4/trexapi/controllers/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    14569 2023-05-15 02:45:00.000000 trex-apis-1.0.4/trexapi/controllers/api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2259 2022-11-14 14:26:16.000000 trex-apis-1.0.4/trexapi/controllers/app_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    35947 2023-05-05 09:27:49.000000 trex-apis-1.0.4/trexapi/controllers/customer_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     6945 2023-04-13 05:36:42.000000 trex-apis-1.0.4/trexapi/controllers/customer_membership_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4750 2023-01-30 07:03:11.000000 trex-apis-1.0.4/trexapi/controllers/customer_reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    13204 2023-05-15 02:06:38.000000 trex-apis-1.0.4/trexapi/controllers/loyalty_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1214 2023-05-07 13:49:51.000000 trex-apis-1.0.4/trexapi/controllers/lucky_draw_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    11170 2023-05-05 09:32:39.000000 trex-apis-1.0.4/trexapi/controllers/outlet_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1430 2022-09-26 04:18:01.000000 trex-apis-1.0.4/trexapi/controllers/payment_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    22728 2023-01-13 04:39:15.000000 trex-apis-1.0.4/trexapi/controllers/pos_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    27329 2023-04-18 07:01:48.000000 trex-apis-1.0.4/trexapi/controllers/reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7315 2023-04-20 09:46:08.000000 trex-apis-1.0.4/trexapi/controllers/sales_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      998 2023-04-18 06:08:18.000000 trex-apis-1.0.4/trexapi/controllers/transaction_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    43378 2023-05-12 14:04:03.000000 trex-apis-1.0.4/trexapi/controllers/user_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2980 2023-01-30 02:56:35.000000 trex-apis-1.0.4/trexapi/controllers/user_reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    15185 2023-04-07 15:27:24.000000 trex-apis-1.0.4/trexapi/controllers/voucher_api_routes.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 06:06:52.112479 trex-apis-1.0.4/trexapi/decorators/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-01 08:42:13.000000 trex-apis-1.0.4/trexapi/decorators/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4734 2023-05-05 09:06:37.000000 trex-apis-1.0.4/trexapi/decorators/api_decorators.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 06:06:52.115279 trex-apis-1.0.4/trexapi/forms/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-12 06:42:53.000000 trex-apis-1.0.4/trexapi/forms/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7419 2023-02-08 10:14:32.000000 trex-apis-1.0.4/trexapi/forms/customer_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7285 2023-04-18 02:42:03.000000 trex-apis-1.0.4/trexapi/forms/reward_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1547 2023-04-18 02:41:54.000000 trex-apis-1.0.4/trexapi/forms/sales_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2505 2023-05-09 02:01:04.000000 trex-apis-1.0.4/trexapi/forms/user_api_forms.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 06:06:52.116165 trex-apis-1.0.4/trexapi/libs/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-05 10:17:19.000000 trex-apis-1.0.4/trexapi/libs/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1143 2021-07-05 10:57:23.000000 trex-apis-1.0.4/trexapi/libs/flask_auth_wrapper.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 06:06:52.117740 trex-apis-1.0.4/trexapi/utils/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-08 10:01:06.000000 trex-apis-1.0.4/trexapi/utils/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1347 2022-12-20 01:23:01.000000 trex-apis-1.0.4/trexapi/utils/api_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    76256 2023-04-24 10:05:07.000000 trex-apis-1.0.4/trexapi/utils/reward_transaction_helper.py
```

### Comparing `trex-apis-1.0.3/setup.py` & `trex-apis-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
      name='trex-apis',  
-     version='1.0.3',
+     version='1.0.4',
      author="Jack Lok",
      author_email="sglok77@gmail.com",
      description="TRex APIs package",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://bitbucket.org/lokjac/trex-apis",
      packages=setuptools.find_packages(),
```

### Comparing `trex-apis-1.0.3/trex_apis.egg-info/SOURCES.txt` & `trex-apis-1.0.4/trex_apis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.3/trexapi/conf.py` & `trex-apis-1.0.4/trexapi/conf.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.3/trexapi/controllers/api_routes.py` & `trex-apis-1.0.4/trexapi/controllers/api_routes.py`

 * *Files 16% similar despite different names*

```diff
@@ -131,14 +131,75 @@
         
         return output_json
     
 class APIResource(APIBaseResource):
     
     def get(self):
         return conf.VERSION    
+
+class AccountActivatedAPIResource(APIBaseResource):  
+    
+    @auth.login_required
+    def post(self):
+        username    = auth.current_user()
+        
+        acct_id     = request.headers.get('x-acct-id')
+        api_key     = request.headers.get('x-api-key')
+        outlet_key  = request.headers.get('x-outlet-key')
+        
+        logger.debug('acct_id=%s', acct_id)    
+        logger.debug('api_key=%s', api_key)
+        logger.debug('outlet_key=%s', outlet_key)
+        
+        is_valid            = False
+        is_authorized       = False
+        output_json = {}
+        
+        if is_not_empty(acct_id) and is_not_empty(api_key):
+            db_client = create_db_client(caller_info="AccountActivatedAPIResource.post")
+            with db_client.context():
+                merchant_acct = MerchantAcct.fetch(acct_id)
+            
+                if merchant_acct:
+                    if api_key == merchant_acct.api_key:
+                        merchant_user               = MerchantUser.get_by_username(username)
+                        
+                        is_authorized = self.is_outlet_authorized(merchant_user, outlet_key)
+                        if is_authorized:
+                            (expiry_datetime, token)    = self.generate_token(acct_id, username)
+                            logger.debug('outlet is_authorized=%s', is_authorized)
+                            logger.debug('expiry_datetime=%s', expiry_datetime)
+                            
+                            output_json =  {
+                                            'auth_token'        : token,
+                                            'expires_in'        : int(api_conf.API_TOKEN_EXPIRY_LENGTH_IN_MINUTE) * 60,
+                                            #'expiry_datetime'   : expiry_datetime.strftime('%d-%m-%Y %h:%M:$S'),
+                                            'granted_outlet'    : merchant_user.granted_outlet_details_list,
+                                            'username'          : merchant_user.username,
+                                            'name'              : merchant_user.name,
+                                            'is_admin'          : merchant_user.is_admin,
+                                            'granted_access'    : merchant_user.permission.get('granted_access'),
+                                            'gravatar_url'      : merchant_user.gravatar_url,
+                                            }
+                
+                            logger.debug('output_json=%s', output_json)
+                            
+                            is_valid = True
+                    
+            if is_valid:
+                return output_json
+            
+            elif is_authorized==False:
+                abort(400, msg=["User is not authorized due to outlet is not granted"])
+                    
+        abort(400, msg=["Failed to authenticate"])
+        
+    
+    def is_outlet_authorized(self, merchant_user, outlet_key):
+        return True 
     
 class AuthenticateAPIResource(APIBaseResource):  
     
     @auth.login_required
     def post(self):
         username    = auth.current_user()
         
@@ -198,15 +259,15 @@
                     
         abort(400, msg=["Failed to authenticate"])
         
     
     def is_outlet_authorized(self, merchant_user, outlet_key):
         return True    
 
-class ProgramDeviceAuthenticate(AuthenticateAPIResource):
+class ProgramDeviceAuthenticate(AccountActivatedAPIResource):
     def is_outlet_authorized(self, merchant_user, outlet_key):
         if merchant_user.is_admin:
             return True
         else:
             data_in_json        = request.get_json()
             activation_code     = data_in_json.get('activation_code')
             device_setting      = LoyaltyDeviceSetting.get_by_activation_code(activation_code)
@@ -226,15 +287,15 @@
                 else:
                     logger.debug('login outlet is not granted outlet')    
             else:
                 logger.debug('login outlet is not same as device setting assigned outlet')
                         
         return False
             
-class POSDeviceAuthenticate(AuthenticateAPIResource):
+class POSDeviceAuthenticate(AccountActivatedAPIResource):
     def is_outlet_authorized(self, merchant_user, outlet_key):
         if merchant_user.is_admin:
             return True
         else:
             data_in_json        = request.get_json()
             activation_code     = data_in_json.get('activation_code')
             device_setting      = POSSetting.get_by_activation_code(activation_code)
```

### Comparing `trex-apis-1.0.3/trexapi/controllers/app_api_routes.py` & `trex-apis-1.0.4/trexapi/controllers/app_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.3/trexapi/controllers/customer_api_routes.py` & `trex-apis-1.0.4/trexapi/controllers/customer_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.3/trexapi/controllers/customer_membership_api_routes.py` & `trex-apis-1.0.4/trexapi/controllers/customer_membership_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.3/trexapi/controllers/customer_reward_api_routes.py` & `trex-apis-1.0.4/trexapi/controllers/customer_reward_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.3/trexapi/controllers/loyalty_api_routes.py` & `trex-apis-1.0.4/trexapi/controllers/loyalty_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.3/trexapi/controllers/lucky_draw_api_routes.py` & `trex-apis-1.0.4/trexapi/controllers/lucky_draw_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.3/trexapi/controllers/outlet_api_routes.py` & `trex-apis-1.0.4/trexapi/controllers/outlet_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.3/trexapi/controllers/payment_api_routes.py` & `trex-apis-1.0.4/trexapi/controllers/payment_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.3/trexapi/controllers/pos_api_routes.py` & `trex-apis-1.0.4/trexapi/controllers/pos_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.3/trexapi/controllers/reward_api_routes.py` & `trex-apis-1.0.4/trexapi/controllers/reward_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.3/trexapi/controllers/sales_api_routes.py` & `trex-apis-1.0.4/trexapi/controllers/sales_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.3/trexapi/controllers/transaction_api_routes.py` & `trex-apis-1.0.4/trexapi/controllers/transaction_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.3/trexapi/controllers/user_api_routes.py` & `trex-apis-1.0.4/trexapi/controllers/user_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.3/trexapi/controllers/user_reward_api_routes.py` & `trex-apis-1.0.4/trexapi/controllers/user_reward_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.3/trexapi/controllers/voucher_api_routes.py` & `trex-apis-1.0.4/trexapi/controllers/voucher_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.3/trexapi/decorators/api_decorators.py` & `trex-apis-1.0.4/trexapi/decorators/api_decorators.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.3/trexapi/forms/customer_api_forms.py` & `trex-apis-1.0.4/trexapi/forms/customer_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.3/trexapi/forms/reward_api_forms.py` & `trex-apis-1.0.4/trexapi/forms/reward_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.3/trexapi/forms/sales_api_forms.py` & `trex-apis-1.0.4/trexapi/forms/sales_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.3/trexapi/forms/user_api_forms.py` & `trex-apis-1.0.4/trexapi/forms/user_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.3/trexapi/libs/flask_auth_wrapper.py` & `trex-apis-1.0.4/trexapi/libs/flask_auth_wrapper.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.3/trexapi/utils/api_helpers.py` & `trex-apis-1.0.4/trexapi/utils/api_helpers.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.3/trexapi/utils/reward_transaction_helper.py` & `trex-apis-1.0.4/trexapi/utils/reward_transaction_helper.py`

 * *Files identical despite different names*

