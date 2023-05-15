# Comparing `tmp/thrivve_core-0.2.3.tar.gz` & `tmp/thrivve_core-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/platformLibraries/platformLibraries/thrivve_core/dist/.tmp-2jsphyog/thrivve_core-0.2.3.tar", last modified: Thu May 11 10:52:39 2023, max compression
+gzip compressed data, was "/home/runner/work/platformLibraries/platformLibraries/thrivve_core/dist/.tmp-9z1w5ycc/thrivve_core-0.2.4.tar", last modified: Mon May 15 15:51:15 2023, max compression
```

## Comparing `thrivve_core-0.2.3.tar` & `thrivve_core-0.2.4.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:52:39.000000 thrivve_core-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (122)      746 2023-05-11 10:52:39.000000 thrivve_core-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-11 10:52:39.000000 thrivve_core-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1327 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:52:39.000000 thrivve_core-0.2.3/thrivve_core/
--rw-r--r--   0 runner    (1001) docker     (122)      881 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:52:39.000000 thrivve_core-0.2.3/thrivve_core/app_decorators/
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/app_decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      979 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/app_decorators/app_entry.py
--rw-r--r--   0 runner    (1001) docker     (122)     2110 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/app_decorators/handle_auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     2327 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/app_decorators/handle_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      786 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/app_decorators/handle_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     4319 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/app_decorators/serializer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:52:39.000000 thrivve_core-0.2.3/thrivve_core/helpers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      855 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/acl_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:52:39.000000 thrivve_core-0.2.3/thrivve_core/helpers/amazon/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/amazon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      579 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py
--rw-r--r--   0 runner    (1001) docker     (122)     1353 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/amazon/get_file_url.py
--rw-r--r--   0 runner    (1001) docker     (122)      318 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/amazon/get_plain_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/amazon/get_s3_client.py
--rw-r--r--   0 runner    (1001) docker     (122)      564 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/amazon/upload_file.py
--rw-r--r--   0 runner    (1001) docker     (122)      833 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/atomic_transactions.py
--rw-r--r--   0 runner    (1001) docker     (122)      921 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/atomic_transactions_v2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2687 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:52:39.000000 thrivve_core-0.2.3/thrivve_core/helpers/database/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      677 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/database/base_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     3983 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/database/log_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2244 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3692 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/fetch_relational_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     4723 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2183 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/format_exception.py
--rw-r--r--   0 runner    (1001) docker     (122)      385 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/get_callback.py
--rw-r--r--   0 runner    (1001) docker     (122)      223 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/get_country_code.py
--rw-r--r--   0 runner    (1001) docker     (122)      622 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/get_embedded_function.py
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/get_obj_value.py
--rw-r--r--   0 runner    (1001) docker     (122)      323 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/get_prefix.py
--rw-r--r--   0 runner    (1001) docker     (122)     2723 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/kafka_listener.py
--rw-r--r--   0 runner    (1001) docker     (122)     3023 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/kafka_producer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:52:39.000000 thrivve_core-0.2.3/thrivve_core/helpers/kafka_producers/
--rw-r--r--   0 runner    (1001) docker     (122)      302 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/kafka_producers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      365 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/kafka_producers/log_model_changes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2061 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/kafka_producers/notification_center.py
--rw-r--r--   0 runner    (1001) docker     (122)      276 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/kafka_producers/send_sms.py
--rw-r--r--   0 runner    (1001) docker     (122)      315 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/kafka_producers/send_topic.py
--rw-r--r--   0 runner    (1001) docker     (122)     2007 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/log_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    12403 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/micro_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/numbers.py
--rw-r--r--   0 runner    (1001) docker     (122)     4270 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/search_function.py
--rw-r--r--   0 runner    (1001) docker     (122)      644 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/service_config.py
--rw-r--r--   0 runner    (1001) docker     (122)      825 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/sql.py
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/system_roles.py
--rw-r--r--   0 runner    (1001) docker     (122)     6823 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/time.py
--rw-r--r--   0 runner    (1001) docker     (122)      393 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/topics.py
--rw-r--r--   0 runner    (1001) docker     (122)      841 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/validate_mobile_number.py
--rw-r--r--   0 runner    (1001) docker     (122)      995 2023-05-11 10:52:26.000000 thrivve_core-0.2.3/thrivve_core/helpers/validate_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 10:52:39.000000 thrivve_core-0.2.3/thrivve_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      746 2023-05-11 10:52:39.000000 thrivve_core-0.2.3/thrivve_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2246 2023-05-11 10:52:39.000000 thrivve_core-0.2.3/thrivve_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 10:52:39.000000 thrivve_core-0.2.3/thrivve_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-05-11 10:52:39.000000 thrivve_core-0.2.3/thrivve_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-11 10:52:39.000000 thrivve_core-0.2.3/thrivve_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:51:15.000000 thrivve_core-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (122)      746 2023-05-15 15:51:15.000000 thrivve_core-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-15 15:51:15.000000 thrivve_core-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1327 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:51:15.000000 thrivve_core-0.2.4/thrivve_core/
+-rw-r--r--   0 runner    (1001) docker     (122)      881 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:51:15.000000 thrivve_core-0.2.4/thrivve_core/app_decorators/
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/app_decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      979 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/app_decorators/app_entry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2110 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/app_decorators/handle_auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2327 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/app_decorators/handle_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      786 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/app_decorators/handle_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4611 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/app_decorators/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:51:15.000000 thrivve_core-0.2.4/thrivve_core/helpers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      855 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/acl_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:51:15.000000 thrivve_core-0.2.4/thrivve_core/helpers/amazon/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/amazon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      579 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1353 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/amazon/get_file_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      318 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/amazon/get_plain_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/amazon/get_s3_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      564 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/amazon/upload_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)      833 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/atomic_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      921 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/atomic_transactions_v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2687 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:51:15.000000 thrivve_core-0.2.4/thrivve_core/helpers/database/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      677 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/database/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3983 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/database/log_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2244 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3692 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/fetch_relational_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4723 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2183 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/format_exception.py
+-rw-r--r--   0 runner    (1001) docker     (122)      385 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/get_callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/get_country_code.py
+-rw-r--r--   0 runner    (1001) docker     (122)      622 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/get_embedded_function.py
+-rw-r--r--   0 runner    (1001) docker     (122)      424 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/get_obj_value.py
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/get_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2723 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/kafka_listener.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3023 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/kafka_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:51:15.000000 thrivve_core-0.2.4/thrivve_core/helpers/kafka_producers/
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/kafka_producers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      365 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/kafka_producers/log_model_changes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2061 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/kafka_producers/notification_center.py
+-rw-r--r--   0 runner    (1001) docker     (122)      276 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/kafka_producers/send_sms.py
+-rw-r--r--   0 runner    (1001) docker     (122)      315 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/kafka_producers/send_topic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2007 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12131 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/micro_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)      129 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4270 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/search_function.py
+-rw-r--r--   0 runner    (1001) docker     (122)      644 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/service_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      825 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/sql.py
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/system_roles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6823 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)      393 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/topics.py
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/validate_mobile_number.py
+-rw-r--r--   0 runner    (1001) docker     (122)      995 2023-05-15 15:51:06.000000 thrivve_core-0.2.4/thrivve_core/helpers/validate_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:51:15.000000 thrivve_core-0.2.4/thrivve_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      746 2023-05-15 15:51:15.000000 thrivve_core-0.2.4/thrivve_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2246 2023-05-15 15:51:15.000000 thrivve_core-0.2.4/thrivve_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-15 15:51:15.000000 thrivve_core-0.2.4/thrivve_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-05-15 15:51:15.000000 thrivve_core-0.2.4/thrivve_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-15 15:51:15.000000 thrivve_core-0.2.4/thrivve_core.egg-info/top_level.txt
```

### Comparing `thrivve_core-0.2.3/PKG-INFO` & `thrivve_core-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thrivve_core
-Version: 0.2.3
+Version: 0.2.4
 Summary: thrivveCore package
 Home-page: https://www.wedeliverapp.com/
 Author: Eyad Farra
 Author-email: info@wedeliverapp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `thrivve_core-0.2.3/setup.py` & `thrivve_core-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "Programming Language :: Python :: 3.4",
     "Programming Language :: Python :: 3.5",
     "Programming Language :: Python :: 3.6",
 ]
 
 setup(
     name="thrivve_core",
-    version="0.2.3",
+    version="0.2.4",
     description="thrivveCore package",
     long_description="""# Markdown supported!\n\n* thrivve\n* List of features\n""",
     long_description_content_type="text/markdown",
     url="https://www.wedeliverapp.com/",
     author="Eyad Farra",
     author_email="info@wedeliverapp.com",
     license="MIT",
```

### Comparing `thrivve_core-0.2.3/thrivve_core/__init__.py` & `thrivve_core-0.2.4/thrivve_core/__init__.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.3/thrivve_core/app_decorators/app_entry.py` & `thrivve_core-0.2.4/thrivve_core/app_decorators/app_entry.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.3/thrivve_core/app_decorators/handle_auth.py` & `thrivve_core-0.2.4/thrivve_core/app_decorators/handle_auth.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.3/thrivve_core/app_decorators/handle_exceptions.py` & `thrivve_core-0.2.4/thrivve_core/app_decorators/handle_exceptions.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.3/thrivve_core/app_decorators/handle_response.py` & `thrivve_core-0.2.4/thrivve_core/app_decorators/handle_response.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.3/thrivve_core/app_decorators/serializer.py` & `thrivve_core-0.2.4/thrivve_core/app_decorators/serializer.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,26 @@
         if isinstance(data, list) and len(data):
             data = obj[0]
         object_mapper(data)
     except UnmappedInstanceError:
         return False
     return True
 
+def is_result_row(obj):
+    try:
+        data = obj
+        if isinstance(data, list) and len(data):
+            data = obj[0]
+
+        if hasattr(data, '__row_data__'):
+            return True
+    except UnmappedInstanceError:
+        return False
+    return False
+
 
 def serializer(schema=None, many=False):
     def factory(func):
         @wraps(func)
         def decorator(*args, **kwargs):
 
             is_function_with_validated_data = False
@@ -99,15 +111,15 @@
                         items=items,
                         total=result.total,
                         next_num=result.next_num,
                         prev_num=result.prev_num,
                         page=result.page,
                         per_page=result.per_page
                     )
-                elif is_mapped(result):  # is model instance
+                elif is_mapped(result) or is_result_row(result):  # is model instance
                     output = schema(many=isinstance(result, list)).dump(result)
                 else:
                     output = result
             except ValidationError as e:
                 raise AppValidationError(e.messages)
 
             return output
```

### Comparing `thrivve_core-0.2.3/thrivve_core/base.py` & `thrivve_core-0.2.4/thrivve_core/base.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.3/thrivve_core/helpers/acl_enum.py` & `thrivve_core-0.2.4/thrivve_core/helpers/acl_enum.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.3/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py` & `thrivve_core-0.2.4/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.3/thrivve_core/helpers/amazon/get_file_url.py` & `thrivve_core-0.2.4/thrivve_core/helpers/amazon/get_file_url.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.3/thrivve_core/helpers/amazon/get_s3_client.py` & `thrivve_core-0.2.4/thrivve_core/helpers/amazon/get_s3_client.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.3/thrivve_core/helpers/amazon/upload_file.py` & `thrivve_core-0.2.4/thrivve_core/helpers/amazon/upload_file.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.3/thrivve_core/helpers/atomic_transactions.py` & `thrivve_core-0.2.4/thrivve_core/helpers/atomic_transactions.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.3/thrivve_core/helpers/atomic_transactions_v2.py` & `thrivve_core-0.2.4/thrivve_core/helpers/atomic_transactions_v2.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.3/thrivve_core/helpers/auth.py` & `thrivve_core-0.2.4/thrivve_core/helpers/auth.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.3/thrivve_core/helpers/config.py` & `thrivve_core-0.2.4/thrivve_core/helpers/config.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.3/thrivve_core/helpers/database/base_model.py` & `thrivve_core-0.2.4/thrivve_core/helpers/database/base_model.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.3/thrivve_core/helpers/database/log_model.py` & `thrivve_core-0.2.4/thrivve_core/helpers/database/log_model.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.3/thrivve_core/helpers/enums.py` & `thrivve_core-0.2.4/thrivve_core/helpers/enums.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.3/thrivve_core/helpers/exceptions.py` & `thrivve_core-0.2.4/thrivve_core/helpers/exceptions.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.3/thrivve_core/helpers/fetch_relational_data.py` & `thrivve_core-0.2.4/thrivve_core/helpers/fetch_relational_data.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.3/thrivve_core/helpers/filters.py` & `thrivve_core-0.2.4/thrivve_core/helpers/filters.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.3/thrivve_core/helpers/format_exception.py` & `thrivve_core-0.2.4/thrivve_core/helpers/format_exception.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.3/thrivve_core/helpers/get_embedded_function.py` & `thrivve_core-0.2.4/thrivve_core/helpers/get_embedded_function.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.3/thrivve_core/helpers/kafka_listener.py` & `thrivve_core-0.2.4/thrivve_core/helpers/kafka_listener.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.3/thrivve_core/helpers/kafka_producer.py` & `thrivve_core-0.2.4/thrivve_core/helpers/kafka_producer.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.3/thrivve_core/helpers/kafka_producers/notification_center.py` & `thrivve_core-0.2.4/thrivve_core/helpers/kafka_producers/notification_center.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.3/thrivve_core/helpers/log_config.py` & `thrivve_core-0.2.4/thrivve_core/helpers/log_config.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.3/thrivve_core/helpers/micro_fetcher.py` & `thrivve_core-0.2.4/thrivve_core/helpers/micro_fetcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import flask_sqlalchemy
 
 from thrivve_core import ThrivveCore
 from thrivve_core.helpers.exceptions import AppMicroFetcherError, AppFetchServiceDataError
 import requests
 import json
 
-from thrivve_core.helpers.get_obj_value import get_obj_value
+from thrivve_core.helpers.get_obj_value import get_obj_value, set_obj_value
 
 from thrivve_core.helpers.service_config import ServiceConfig
 
 from thrivve_core.helpers.enums import QueryTypes
 
 
 class MicroFetcher(object):
@@ -298,26 +298,21 @@
                     data = self.base_data.items
                 else:
                     data = self.base_data
 
                 if isinstance(data, list):
                     for row in data:
                         for rd in result:
-                            if get_obj_value(row, self.lookup_key) == rd.get(self.column_name):
-                                try:
-                                    setattr(row, self.output_key, rd)
-                                except AttributeError:
-                                    row[self.output_key] = rd
+                            if get_obj_value(row, self.lookup_key) == str(rd.get(self.column_name)):
+                                set_obj_value(row, self.output_key, rd)
                 else:
                     for rd in result:
                         if get_obj_value(data, self.lookup_key) == rd.get(self.column_name):
-                            try:
-                                setattr(data, self.output_key, rd)
-                            except AttributeError:
-                                data[self.output_key] = rd
+                            set_obj_value(data, self.output_key, rd)
+
 
                 if isinstance(self.base_data, flask_sqlalchemy.Pagination):
                     self.base_data.items = data
                 else:
                     self.base_data = data
 
             return self.base_data
```

### Comparing `thrivve_core-0.2.3/thrivve_core/helpers/search_function.py` & `thrivve_core-0.2.4/thrivve_core/helpers/search_function.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.3/thrivve_core/helpers/service_config.py` & `thrivve_core-0.2.4/thrivve_core/helpers/service_config.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.3/thrivve_core/helpers/sql.py` & `thrivve_core-0.2.4/thrivve_core/helpers/sql.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.3/thrivve_core/helpers/time.py` & `thrivve_core-0.2.4/thrivve_core/helpers/time.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.3/thrivve_core/helpers/validate_mobile_number.py` & `thrivve_core-0.2.4/thrivve_core/helpers/validate_mobile_number.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.3/thrivve_core/helpers/validate_parameters.py` & `thrivve_core-0.2.4/thrivve_core/helpers/validate_parameters.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.2.3/thrivve_core.egg-info/PKG-INFO` & `thrivve_core-0.2.4/thrivve_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thrivve-core
-Version: 0.2.3
+Version: 0.2.4
 Summary: thrivveCore package
 Home-page: https://www.wedeliverapp.com/
 Author: Eyad Farra
 Author-email: info@wedeliverapp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `thrivve_core-0.2.3/thrivve_core.egg-info/SOURCES.txt` & `thrivve_core-0.2.4/thrivve_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

