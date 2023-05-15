# Comparing `tmp/trex-apis-1.0.2.tar.gz` & `tmp/trex-apis-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trex-apis-1.0.2.tar", last modified: Mon May  8 02:59:42 2023, max compression
+gzip compressed data, was "trex-apis-1.0.3.tar", last modified: Mon May 15 02:08:24 2023, max compression
```

## Comparing `trex-apis-1.0.2.tar` & `trex-apis-1.0.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-08 02:59:42.400350 trex-apis-1.0.2/
--rw-r--r--   0 jacklok    (501) staff       (20)      447 2023-05-08 02:59:42.400508 trex-apis-1.0.2/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)       25 2021-06-30 02:28:26.000000 trex-apis-1.0.2/README.md
--rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-05-08 02:59:42.401034 trex-apis-1.0.2/setup.cfg
--rw-r--r--   0 jacklok    (501) staff       (20)      713 2023-05-08 02:59:25.000000 trex-apis-1.0.2/setup.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-08 02:59:42.371375 trex-apis-1.0.2/trex_apis.egg-info/
--rw-r--r--   0 jacklok    (501) staff       (20)      447 2023-05-08 02:59:42.000000 trex-apis-1.0.2/trex_apis.egg-info/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)     1328 2023-05-08 02:59:42.000000 trex-apis-1.0.2/trex_apis.egg-info/SOURCES.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-05-08 02:59:42.000000 trex-apis-1.0.2/trex_apis.egg-info/dependency_links.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       23 2023-05-08 02:59:42.000000 trex-apis-1.0.2/trex_apis.egg-info/requires.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        8 2023-05-08 02:59:42.000000 trex-apis-1.0.2/trex_apis.egg-info/top_level.txt
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-08 02:59:42.371975 trex-apis-1.0.2/trexapi/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:30:07.000000 trex-apis-1.0.2/trexapi/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      837 2023-04-19 06:13:09.000000 trex-apis-1.0.2/trexapi/conf.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-08 02:59:42.390752 trex-apis-1.0.2/trexapi/controllers/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:45:28.000000 trex-apis-1.0.2/trexapi/controllers/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)    11544 2023-04-24 08:15:59.000000 trex-apis-1.0.2/trexapi/controllers/api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2259 2022-11-14 14:26:16.000000 trex-apis-1.0.2/trexapi/controllers/app_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    35947 2023-05-05 09:27:49.000000 trex-apis-1.0.2/trexapi/controllers/customer_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     6945 2023-04-13 05:36:42.000000 trex-apis-1.0.2/trexapi/controllers/customer_membership_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4750 2023-01-30 07:03:11.000000 trex-apis-1.0.2/trexapi/controllers/customer_reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    12965 2023-03-24 05:50:51.000000 trex-apis-1.0.2/trexapi/controllers/loyalty_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1214 2023-05-07 13:49:51.000000 trex-apis-1.0.2/trexapi/controllers/lucky_draw_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    11170 2023-05-05 09:32:39.000000 trex-apis-1.0.2/trexapi/controllers/outlet_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1430 2022-09-26 04:18:01.000000 trex-apis-1.0.2/trexapi/controllers/payment_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    22728 2023-01-13 04:39:15.000000 trex-apis-1.0.2/trexapi/controllers/pos_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    27329 2023-04-18 07:01:48.000000 trex-apis-1.0.2/trexapi/controllers/reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7315 2023-04-20 09:46:08.000000 trex-apis-1.0.2/trexapi/controllers/sales_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)      998 2023-04-18 06:08:18.000000 trex-apis-1.0.2/trexapi/controllers/transaction_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    36081 2023-04-03 08:51:30.000000 trex-apis-1.0.2/trexapi/controllers/user_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2980 2023-01-30 02:56:35.000000 trex-apis-1.0.2/trexapi/controllers/user_reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    15185 2023-04-07 15:27:24.000000 trex-apis-1.0.2/trexapi/controllers/voucher_api_routes.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-08 02:59:42.392060 trex-apis-1.0.2/trexapi/decorators/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-01 08:42:13.000000 trex-apis-1.0.2/trexapi/decorators/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4734 2023-05-05 09:06:37.000000 trex-apis-1.0.2/trexapi/decorators/api_decorators.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-08 02:59:42.395362 trex-apis-1.0.2/trexapi/forms/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-12 06:42:53.000000 trex-apis-1.0.2/trexapi/forms/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7419 2023-02-08 10:14:32.000000 trex-apis-1.0.2/trexapi/forms/customer_api_forms.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7285 2023-04-18 02:42:03.000000 trex-apis-1.0.2/trexapi/forms/reward_api_forms.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1547 2023-04-18 02:41:54.000000 trex-apis-1.0.2/trexapi/forms/sales_api_forms.py
--rw-r--r--   0 jacklok    (501) staff       (20)     3344 2023-01-18 01:16:56.000000 trex-apis-1.0.2/trexapi/forms/user_api_forms.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-08 02:59:42.396583 trex-apis-1.0.2/trexapi/libs/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-05 10:17:19.000000 trex-apis-1.0.2/trexapi/libs/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1143 2021-07-05 10:57:23.000000 trex-apis-1.0.2/trexapi/libs/flask_auth_wrapper.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-08 02:59:42.398606 trex-apis-1.0.2/trexapi/utils/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-08 10:01:06.000000 trex-apis-1.0.2/trexapi/utils/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1347 2022-12-20 01:23:01.000000 trex-apis-1.0.2/trexapi/utils/api_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)    76256 2023-04-24 10:05:07.000000 trex-apis-1.0.2/trexapi/utils/reward_transaction_helper.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 02:08:24.915940 trex-apis-1.0.3/
+-rw-r--r--   0 jacklok    (501) staff       (20)      447 2023-05-15 02:08:24.916204 trex-apis-1.0.3/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)       25 2021-06-30 02:28:26.000000 trex-apis-1.0.3/README.md
+-rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-05-15 02:08:24.917218 trex-apis-1.0.3/setup.cfg
+-rw-r--r--   0 jacklok    (501) staff       (20)      713 2023-05-15 02:07:30.000000 trex-apis-1.0.3/setup.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 02:08:24.889255 trex-apis-1.0.3/trex_apis.egg-info/
+-rw-r--r--   0 jacklok    (501) staff       (20)      447 2023-05-15 02:08:24.000000 trex-apis-1.0.3/trex_apis.egg-info/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)     1328 2023-05-15 02:08:24.000000 trex-apis-1.0.3/trex_apis.egg-info/SOURCES.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-05-15 02:08:24.000000 trex-apis-1.0.3/trex_apis.egg-info/dependency_links.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       23 2023-05-15 02:08:24.000000 trex-apis-1.0.3/trex_apis.egg-info/requires.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        8 2023-05-15 02:08:24.000000 trex-apis-1.0.3/trex_apis.egg-info/top_level.txt
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 02:08:24.889793 trex-apis-1.0.3/trexapi/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:30:07.000000 trex-apis-1.0.3/trexapi/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      837 2023-04-19 06:13:09.000000 trex-apis-1.0.3/trexapi/conf.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 02:08:24.905620 trex-apis-1.0.3/trexapi/controllers/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:45:28.000000 trex-apis-1.0.3/trexapi/controllers/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    11544 2023-04-24 08:15:59.000000 trex-apis-1.0.3/trexapi/controllers/api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2259 2022-11-14 14:26:16.000000 trex-apis-1.0.3/trexapi/controllers/app_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    35947 2023-05-05 09:27:49.000000 trex-apis-1.0.3/trexapi/controllers/customer_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     6945 2023-04-13 05:36:42.000000 trex-apis-1.0.3/trexapi/controllers/customer_membership_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4750 2023-01-30 07:03:11.000000 trex-apis-1.0.3/trexapi/controllers/customer_reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    13204 2023-05-15 02:06:38.000000 trex-apis-1.0.3/trexapi/controllers/loyalty_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1214 2023-05-07 13:49:51.000000 trex-apis-1.0.3/trexapi/controllers/lucky_draw_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    11170 2023-05-05 09:32:39.000000 trex-apis-1.0.3/trexapi/controllers/outlet_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1430 2022-09-26 04:18:01.000000 trex-apis-1.0.3/trexapi/controllers/payment_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    22728 2023-01-13 04:39:15.000000 trex-apis-1.0.3/trexapi/controllers/pos_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    27329 2023-04-18 07:01:48.000000 trex-apis-1.0.3/trexapi/controllers/reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7315 2023-04-20 09:46:08.000000 trex-apis-1.0.3/trexapi/controllers/sales_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      998 2023-04-18 06:08:18.000000 trex-apis-1.0.3/trexapi/controllers/transaction_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    43378 2023-05-12 14:04:03.000000 trex-apis-1.0.3/trexapi/controllers/user_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2980 2023-01-30 02:56:35.000000 trex-apis-1.0.3/trexapi/controllers/user_reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    15185 2023-04-07 15:27:24.000000 trex-apis-1.0.3/trexapi/controllers/voucher_api_routes.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 02:08:24.906656 trex-apis-1.0.3/trexapi/decorators/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-01 08:42:13.000000 trex-apis-1.0.3/trexapi/decorators/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4734 2023-05-05 09:06:37.000000 trex-apis-1.0.3/trexapi/decorators/api_decorators.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 02:08:24.910101 trex-apis-1.0.3/trexapi/forms/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-12 06:42:53.000000 trex-apis-1.0.3/trexapi/forms/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7419 2023-02-08 10:14:32.000000 trex-apis-1.0.3/trexapi/forms/customer_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7285 2023-04-18 02:42:03.000000 trex-apis-1.0.3/trexapi/forms/reward_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1547 2023-04-18 02:41:54.000000 trex-apis-1.0.3/trexapi/forms/sales_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2505 2023-05-09 02:01:04.000000 trex-apis-1.0.3/trexapi/forms/user_api_forms.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 02:08:24.911393 trex-apis-1.0.3/trexapi/libs/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-05 10:17:19.000000 trex-apis-1.0.3/trexapi/libs/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1143 2021-07-05 10:57:23.000000 trex-apis-1.0.3/trexapi/libs/flask_auth_wrapper.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-05-15 02:08:24.913672 trex-apis-1.0.3/trexapi/utils/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-08 10:01:06.000000 trex-apis-1.0.3/trexapi/utils/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1347 2022-12-20 01:23:01.000000 trex-apis-1.0.3/trexapi/utils/api_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    76256 2023-04-24 10:05:07.000000 trex-apis-1.0.3/trexapi/utils/reward_transaction_helper.py
```

### Comparing `trex-apis-1.0.2/setup.py` & `trex-apis-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
      name='trex-apis',  
-     version='1.0.2',
+     version='1.0.3',
      author="Jack Lok",
      author_email="sglok77@gmail.com",
      description="TRex APIs package",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://bitbucket.org/lokjac/trex-apis",
      packages=setuptools.find_packages(),
```

### Comparing `trex-apis-1.0.2/trex_apis.egg-info/SOURCES.txt` & `trex-apis-1.0.3/trex_apis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.2/trexapi/conf.py` & `trex-apis-1.0.3/trexapi/conf.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.2/trexapi/controllers/api_routes.py` & `trex-apis-1.0.3/trexapi/controllers/api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.2/trexapi/controllers/app_api_routes.py` & `trex-apis-1.0.3/trexapi/controllers/app_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.2/trexapi/controllers/customer_api_routes.py` & `trex-apis-1.0.3/trexapi/controllers/customer_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.2/trexapi/controllers/customer_membership_api_routes.py` & `trex-apis-1.0.3/trexapi/controllers/customer_membership_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.2/trexapi/controllers/customer_reward_api_routes.py` & `trex-apis-1.0.3/trexapi/controllers/customer_reward_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.2/trexapi/controllers/loyalty_api_routes.py` & `trex-apis-1.0.3/trexapi/controllers/loyalty_api_routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,17 @@
         if device_setting:
             logger.info('Found device setting');
             if device_setting.activated==False:
             #if True:
                 logger.info('device activation code is valid');
                 device_setting_details = None
                 with db_client.context():
-                    device_setting.activate(device_id)
+                    if device_setting.is_test_setting==False:
+                        device_setting.activate(device_id)
+                    
                     device_setting_details                              = merchant_helpers.construct_setting_by_outlet(device_setting.assigned_outlet_entity, device_setting=device_setting) 
                     
                     device_setting_details['logo_image_url']            = url_for('system_bp.merchant_logo_image_url', merchant_act_key=device_setting_details.get('account_id'))
                 
                 return create_rest_message(status_code=StatusCode.OK,
                                                **device_setting_details
                                                )
@@ -134,26 +136,29 @@
             logger.info('Device activation code is valid');
             
             is_valid = False
             device_setting_details = None
             
             with db_client.context():
                 device_setting = LoyaltyDeviceSetting.get_by_activation_code(activation_code)
-                if device_setting.activated:
-                    if device_setting.device_id == device_id:
+                if device_setting.is_test_setting==False:
+                    if device_setting.activated:
+                        if device_setting.device_id == device_id:
+                            is_valid = True
+                        
+                    else:
                         is_valid = True
-                    
+                        device_setting.activate(device_id)
                 else:
                     is_valid = True
-                    device_setting.activate(device_id)
-            
+                
                 if is_valid:    
                     device_setting_details                                 = merchant_helpers.construct_setting_by_outlet(device_setting.assigned_outlet_entity, device_setting=device_setting)
                     #pos_setting_details['logo_image_url']               = url_for('system_bp.merchant_logo_image_url', merchant_act_key=pos_setting_details.get('account_id'))
-            
+                
             if is_valid:
                 
                 logger.debug('device_setting_details=%s', device_setting_details);
                 
                 return create_rest_message(status_code=StatusCode.OK,
                                            **device_setting_details
                                            )
```

### Comparing `trex-apis-1.0.2/trexapi/controllers/lucky_draw_api_routes.py` & `trex-apis-1.0.3/trexapi/controllers/lucky_draw_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.2/trexapi/controllers/outlet_api_routes.py` & `trex-apis-1.0.3/trexapi/controllers/outlet_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.2/trexapi/controllers/payment_api_routes.py` & `trex-apis-1.0.3/trexapi/controllers/payment_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.2/trexapi/controllers/pos_api_routes.py` & `trex-apis-1.0.3/trexapi/controllers/pos_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.2/trexapi/controllers/reward_api_routes.py` & `trex-apis-1.0.3/trexapi/controllers/reward_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.2/trexapi/controllers/sales_api_routes.py` & `trex-apis-1.0.3/trexapi/controllers/sales_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.2/trexapi/controllers/transaction_api_routes.py` & `trex-apis-1.0.3/trexapi/controllers/transaction_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.2/trexapi/controllers/user_api_routes.py` & `trex-apis-1.0.3/trexapi/controllers/user_api_routes.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from trexmodel.utils.model.model_util import create_db_client
 from datetime import datetime
 from trexlib.utils.string_util import is_not_empty
 from trexmodel.models.datastore.user_models import User
 from trexadmin.libs.http import create_rest_message
 from trexadmin.libs.http import StatusCode
 from werkzeug.datastructures import ImmutableMultiDict
-from trexapi.forms.user_api_forms import UserRegistrationForm
+from trexapi.forms.user_api_forms import UserRegistrationForm, UserUpdateForm
 from trexapi.conf import APPLICATION_NAME, APPLICATION_BASE_URL
 from trexmail.email_helper import trigger_send_email
 from trexmodel.models.datastore.merchant_models import MerchantAcct, Outlet
 from trexmodel.models.datastore.customer_models import Customer
 from trexmodel.models.datastore.reward_models import CustomerEntitledVoucher,\
     CustomerPointReward, CustomerEntitledTierRewardSummary
 from trexapi.utils.api_helpers import generate_user_auth_token
@@ -121,14 +121,78 @@
             return create_rest_message(error_message, status_code=StatusCode.BAD_REQUEST)
             
     except:
         logger.error('user_register: Fail to register user due to %s', get_tracelog())
         
         return create_rest_message(status_code=StatusCode.BAD_REQUEST)
 
+@user_api_bp.route('/update', methods=['POST'])
+def user_update():
+    logger.debug('user_update: ---user_register---')
+    
+    try:
+        user_data_in_json   = request.get_json()
+        logger.debug('user_update: user_data_in_json=%s', user_data_in_json)
+        
+        update_user_form  = UserUpdateForm(ImmutableMultiDict(user_data_in_json))
+        if update_user_form.validate():
+            logger.debug('update_user_form:  update input is valid')
+            db_client = create_db_client(caller_info="user_update")
+            
+            with db_client.context():
+                reference_code  = update_user_form.reference_code.data
+                name            = update_user_form.name.data
+                mobile_phone    = update_user_form.mobile_phone.data
+                birth_date      = update_user_form.birth_date.data
+                gender          = update_user_form.gender.data
+                
+                birth_date      = datetime.strptime(birth_date, '%d-%m-%Y')
+                
+                logger.debug('reference_code=%s', reference_code)
+                logger.debug('name=%s', name)
+                logger.debug('mobile_phone=%s', mobile_phone)
+                logger.debug('birth_date=%s', birth_date)
+                logger.debug('gender=%s', gender)
+                
+                user_acct = User.get_by_reference_code(reference_code)
+                if user_acct:
+                    original_mobile_phone   = user_acct.mobile_phone
+                    user_acct.name          = name
+                    user_acct.mobile_phone  = mobile_phone
+                    user_acct.birth_date    = birth_date
+                    user_acct.gender        = gender
+                    
+                    if is_not_empty(mobile_phone):
+                        if original_mobile_phone!=mobile_phone:
+                            checking_mobile_phone_user_acct = User.get_by_mobile_phone(mobile_phone)
+                            if checking_mobile_phone_user_acct is None:
+                                User.update(user_acct)
+                            else:
+                                return create_rest_message('Mobile Phone have been taken', status_code=StatusCode.BAD_REQUEST)
+                        else:
+                            User.update(user_acct)
+                                
+                    
+                else:
+                    return create_rest_message('User account is not found', status_code=StatusCode.BAD_REQUEST)
+                
+                                
+            return create_rest_message(status_code=StatusCode.OK)
+            
+        else:
+            logger.warn('user_register: user registration input is invalid')
+            error_message = update_user_form.create_rest_return_error_message()
+            
+            return create_rest_message(error_message, status_code=StatusCode.BAD_REQUEST)
+            
+    except:
+        logger.error('user_register: Fail to update user due to %s', get_tracelog())
+        
+        return create_rest_message(status_code=StatusCode.BAD_REQUEST)
+    
 
 @user_api_bp.route('/auth', methods=['POST'])
 def auth_user():
     
     user_data_in_json   = request.get_json()
     email               = user_data_in_json.get('email')
     password            = user_data_in_json.get('password')
@@ -239,15 +303,15 @@
             return create_rest_message(status_code=StatusCode.BAD_REQUEST)
             
     else:
         logger.warn('verify_mobile_phone_account: user verify input is invalid')
         return create_rest_message(status_code=StatusCode.BAD_REQUEST)        
 
 @user_api_bp.route('/register-as-customer', methods=['POST'])
-@user_auth_token_required
+#@user_auth_token_required
 def register_user_as_customer():
     user_data_in_json           = request.get_json()
     reference_code              = user_data_in_json.get('reference_code')
     merchant_reference_code     = user_data_in_json.get('merchant_reference_code')
     outlet_key                  = user_data_in_json.get('outlet_key')
     
     logger.debug('register_user_as_customer: user_data_in_json=%s', user_data_in_json)
@@ -282,21 +346,21 @@
                             
                             email           = existing_user_acct.email
                             mobile_phone    = existing_user_acct.mobile_phone
                             
                             logger.debug('email=%s', email)
                             logger.debug('mobile_phone=%s', mobile_phone)
                             
-                            checking_customer = Customer.get_by_email(email) 
+                            checking_customer = Customer.get_by_email(email, merchant_acct=merchant_acct) 
                             
                             if checking_customer:
                                 is_email_used = True
                             else:
                                 if is_not_empty(mobile_phone):
-                                    checking_customer = Customer.get_by_mobile_phone(mobile_phone)
+                                    checking_customer = Customer.get_by_mobile_phone(mobile_phone, merchant_acct=merchant_acct)
                                     if checking_customer:
                                         is_mobile_phone_used = True
                             
                             logger.debug('is_email_used=%s', is_email_used)
                             logger.debug('is_mobile_phone_used=%s', is_mobile_phone_used)
                             
                             if is_email_used == False and is_mobile_phone_used == False:
@@ -498,14 +562,15 @@
             'prepaid_summary'   : customer.prepaid_summary,
             'voucher_summary'   : customer.entitled_voucher_summary,
             }
     
     return jsonify(result)
     
 @user_api_bp.route('/<reference_code>', methods=['GET'])
+@user_auth_token_required
 def read_user_acct(reference_code):
     
     if is_not_empty(reference_code):
         db_client = create_db_client(caller_info="read_user_acct")
         user_acct = None
         with db_client.context():
             user_acct = User.get_by_reference_code(reference_code)
@@ -538,14 +603,99 @@
         else:
             logger.debug('user account is not found')
             return create_rest_message(status_code=StatusCode.BAD_REQUEST)
             
     else:
         logger.warn('verify_user: user verify input is invalid')
         return create_rest_message(status_code=StatusCode.BAD_REQUEST)    
+
+@user_api_bp.route('/<reference_code>/joined-brands-list', methods=['GET'])
+#@user_auth_token_required
+def list_joined_brands(reference_code):
+    limit           = request.args.get('limit')
+    start_cursor    = request.args.get('start_cursor')
+    
+    logger.debug('limit=%s', limit)
+    logger.debug('start_cursor=%s', start_cursor)
+    
+    if is_not_empty(reference_code):
+        db_client = create_db_client(caller_info="list_joined_brands")
+        brands_list     = []
+        user_acct       = None
+        result_data     = {}
+        
+        if is_not_empty(limit):
+            limit = int(limit)
+        
+        with db_client.context():
+            user_acct = User.get_by_reference_code(reference_code)
+        
+        if user_acct:
+            logger.debug('verify_user: found user account by reference_code=%s', reference_code)
+            
+            
+            
+            with db_client.context():
+                (customer_accts_list, next_cursor) = Customer.list_paginated_by_user_account(user_acct, start_cursor=start_cursor, limit=limit)
+                
+                for customer_acct in customer_accts_list:
+                    merchant_acct = customer_acct.registered_merchant_acct
+                    brands_list.append({
+                                        'key'       : merchant_acct.key_in_str,
+                                        'name'      : merchant_acct.brand_name,
+                                        'logo_url'  : merchant_acct.logo_public_url,
+                                        
+                                        })
+                    '''
+                    brands_list.append({
+                                        'key'       : merchant_acct.key_in_str,
+                                        'name'      : merchant_acct.brand_name,
+                                        'logo_url'  : merchant_acct.logo_public_url,
+                                        
+                                        })
+                    brands_list.append({
+                                        'key'       : merchant_acct.key_in_str,
+                                        'name'      : merchant_acct.brand_name,
+                                        'logo_url'  : merchant_acct.logo_public_url,
+                                        
+                                        })
+                    brands_list.append({
+                                        'key'       : merchant_acct.key_in_str,
+                                        'name'      : merchant_acct.brand_name,
+                                        'logo_url'  : merchant_acct.logo_public_url,
+                                        
+                                        })
+                    brands_list.append({
+                                        'key'       : merchant_acct.key_in_str,
+                                        'name'      : merchant_acct.brand_name,
+                                        'logo_url'  : merchant_acct.logo_public_url,
+                                        
+                                        })
+                    brands_list.append({
+                                        'key'       : merchant_acct.key_in_str,
+                                        'name'      : merchant_acct.brand_name,
+                                        'logo_url'  : merchant_acct.logo_public_url,
+                                        
+                                        })
+                     '''                    
+                result_data= {
+                                'result'        : brands_list,
+                                'count'         : len(brands_list),
+                                }
+                  
+                if is_not_empty(next_cursor):
+                    result_data['next_cursor'] = next_cursor  
+        
+        
+        
+        return create_rest_message(status_code=StatusCode.OK,
+                                   **result_data, 
+                                   )
+    else:
+        return create_rest_message(status_code=StatusCode.BAD_REQUEST)   
     
 @user_api_bp.route('/reset-email-vc', methods=['PUT'])
 def reset_email_verification_code():
     email = request.args.get('email') or request.form.get('email') or request.json.get('email')
     
     logger.debug('reset_email_verification_code: going to reset email verification code by email=%s', email)
```

### Comparing `trex-apis-1.0.2/trexapi/controllers/user_reward_api_routes.py` & `trex-apis-1.0.3/trexapi/controllers/user_reward_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.2/trexapi/controllers/voucher_api_routes.py` & `trex-apis-1.0.3/trexapi/controllers/voucher_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.2/trexapi/decorators/api_decorators.py` & `trex-apis-1.0.3/trexapi/decorators/api_decorators.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.2/trexapi/forms/customer_api_forms.py` & `trex-apis-1.0.3/trexapi/forms/customer_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.2/trexapi/forms/reward_api_forms.py` & `trex-apis-1.0.3/trexapi/forms/reward_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.2/trexapi/forms/sales_api_forms.py` & `trex-apis-1.0.3/trexapi/forms/sales_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.2/trexapi/forms/user_api_forms.py` & `trex-apis-1.0.3/trexapi/forms/user_api_forms.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 from wtforms import StringField, PasswordField, validators, DateField
 from trexadmin.forms.base_forms import ValidationBaseForm
 from trexadmin.libs.wtforms import validators as custom_validator
 from flask_babel import gettext
 from datetime import date
 
-class UserRegistrationForm(ValidationBaseForm):
+class UserMinForm(ValidationBaseForm):
     name                = StringField(gettext('Name'), validators=[
                                         validators.InputRequired(gettext('Name is required')),
                                         validators.Length(min=3, max=300, message='Name length must be within 3 and 300 characters'),
                                         
                                         ]
                                         )
-    email               = StringField('Email Address', validators=[
-                                        validators.Email(gettext("Please enter valid email address.")),
-                                        validators.InputRequired(gettext('Email is required')),
-                                        ]
-                                        )
     mobile_phone        = StringField('Mobile Phone', validators=[
                                         #validators.InputRequired(gettext('Mobile Phone is required')),
                                         ]
                                         )
     
     gender              = StringField('Gender', validators=[
                                         validators.InputRequired(gettext('Gender is required')),
@@ -27,35 +22,29 @@
                                         )
     
     birth_date          = StringField('Mobile Phone', validators=[
                                         validators.InputRequired(gettext('Birth date is required')),
                                         ]
                                         )
     
-    password            = StringField(gettext('Password'), validators=[
-                                        validators.InputRequired(gettext('Password is required')),
-                                        
-                                        ]
-                                        )
     
-class UserDetailsForm(UserRegistrationForm):
     
-    gender              = StringField(gettext('Gender'), [
-                                        validators.Optional(),
-                                        validators.Length(min=1, max=1, message=gettext('Gender value is either m or f')),
-                                        
+class UserRegistrationForm(UserMinForm):
+    email               = StringField('Email Address', validators=[
+                                        validators.Email(gettext("Please enter valid email address.")),
+                                        validators.InputRequired(gettext('Email is required')),
                                         ]
                                         )
     
-    birth_date          = DateField('Date of Birth', format='%d/%m/%Y', validators=[
-                                            validators.Optional(),
-                                        ])
-    
-    mobile_phone        = StringField('Mobile Phone', validators=[
-                                        custom_validator.RequiredIfOtherFieldEmpty(
-                                                        ['email'],
-                                                        message=gettext("Either email or mobile phone is required"),
-                                                        
-                                                        ),
+    password            = StringField(gettext('Password'), validators=[
+                                        validators.InputRequired(gettext('Password is required')),
                                         
                                         ]
-                                        )    
+                                        )  
+    
+class UserUpdateForm(UserMinForm):
+    reference_code      = StringField('User Reference Code', validators=[
+                                        validators.InputRequired(gettext('User Reference Code is required')),
+                                        ]
+                                        )      
+    
+
```

### Comparing `trex-apis-1.0.2/trexapi/libs/flask_auth_wrapper.py` & `trex-apis-1.0.3/trexapi/libs/flask_auth_wrapper.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.2/trexapi/utils/api_helpers.py` & `trex-apis-1.0.3/trexapi/utils/api_helpers.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.2/trexapi/utils/reward_transaction_helper.py` & `trex-apis-1.0.3/trexapi/utils/reward_transaction_helper.py`

 * *Files identical despite different names*

