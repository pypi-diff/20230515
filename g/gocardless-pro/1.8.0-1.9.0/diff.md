# Comparing `tmp/gocardless_pro-1.8.0.tar.gz` & `tmp/gocardless_pro-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gocardless_pro-1.8.0.tar", last modified: Fri Jul 13 09:57:13 2018, max compression
+gzip compressed data, was "dist/gocardless_pro-1.9.0.tar", last modified: Thu Oct  4 09:45:42 2018, max compression
```

## Comparing `gocardless_pro-1.8.0.tar` & `gocardless_pro-1.9.0.tar`

### file list

```diff
@@ -1,75 +1,79 @@
-drwxr-xr-x   0 cristiangreco   (501) staff       (20)        0 2018-07-13 09:57:13.000000 gocardless_pro-1.8.0/
-drwxr-xr-x   0 cristiangreco   (501) staff       (20)        0 2018-07-13 09:57:13.000000 gocardless_pro-1.8.0/gocardless_pro/
--rw-r--r--   0 cristiangreco   (501) staff       (20)      103 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/__init__.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     4283 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/api_client.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)      561 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/api_response.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     3661 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/client.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     3030 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/errors.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)      465 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/list_response.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)      874 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/paginator.py
-drwxr-xr-x   0 cristiangreco   (501) staff       (20)        0 2018-07-13 09:57:13.000000 gocardless_pro-1.8.0/gocardless_pro/resources/
--rw-r--r--   0 cristiangreco   (501) staff       (20)      733 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/resources/__init__.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)      786 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/resources/bank_details_lookup.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     2776 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/resources/creditor.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     1756 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/resources/creditor_bank_account.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     2107 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/resources/customer.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     1756 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/resources/customer_bank_account.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     3062 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/resources/event.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     1939 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/resources/mandate.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)      817 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/resources/mandate_import.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     1417 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/resources/mandate_import_entry.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)      626 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/resources/mandate_pdf.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     2053 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/resources/payment.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     1773 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/resources/payout.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     1094 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/resources/payout_item.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     1958 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/resources/redirect_flow.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     1444 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/resources/refund.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     2340 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/resources/subscription.py
-drwxr-xr-x   0 cristiangreco   (501) staff       (20)        0 2018-07-13 09:57:13.000000 gocardless_pro-1.8.0/gocardless_pro/services/
--rw-r--r--   0 cristiangreco   (501) staff       (20)      991 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/services/__init__.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     1874 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/services/bank_details_lookups_service.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     2602 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/services/base_service.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     3875 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/services/creditor_bank_accounts_service.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     3387 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/services/creditors_service.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     5101 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/services/customer_bank_accounts_service.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     3394 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/services/customers_service.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     1751 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/services/events_service.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     2362 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/services/mandate_import_entries_service.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     4213 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/services/mandate_imports_service.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     2932 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/services/mandate_pdfs_service.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     5767 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/services/mandates_service.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     6024 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/services/payments_service.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     1158 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/services/payout_items_service.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     1903 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/services/payouts_service.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     3477 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/services/redirect_flows_service.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     4027 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/services/refunds_service.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     5506 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/gocardless_pro/services/subscriptions_service.py
-drwxr-xr-x   0 cristiangreco   (501) staff       (20)        0 2018-07-13 09:57:13.000000 gocardless_pro-1.8.0/gocardless_pro.egg-info/
--rw-r--r--   0 cristiangreco   (501) staff       (20)        1 2018-07-13 09:57:13.000000 gocardless_pro-1.8.0/gocardless_pro.egg-info/dependency_links.txt
--rw-r--r--   0 cristiangreco   (501) staff       (20)    12368 2018-07-13 09:57:13.000000 gocardless_pro-1.8.0/gocardless_pro.egg-info/PKG-INFO
--rw-r--r--   0 cristiangreco   (501) staff       (20)       18 2018-07-13 09:57:13.000000 gocardless_pro-1.8.0/gocardless_pro.egg-info/requires.txt
--rw-r--r--   0 cristiangreco   (501) staff       (20)     2813 2018-07-13 09:57:13.000000 gocardless_pro-1.8.0/gocardless_pro.egg-info/SOURCES.txt
--rw-r--r--   0 cristiangreco   (501) staff       (20)       21 2018-07-13 09:57:13.000000 gocardless_pro-1.8.0/gocardless_pro.egg-info/top_level.txt
--rw-r--r--   0 cristiangreco   (501) staff       (20)    12368 2018-07-13 09:57:13.000000 gocardless_pro-1.8.0/PKG-INFO
--rw-r--r--   0 cristiangreco   (501) staff       (20)     9116 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/README.rst
--rw-r--r--   0 cristiangreco   (501) staff       (20)       59 2018-07-13 09:57:13.000000 gocardless_pro-1.8.0/setup.cfg
--rw-r--r--   0 cristiangreco   (501) staff       (20)      637 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/setup.py
-drwxr-xr-x   0 cristiangreco   (501) staff       (20)        0 2018-07-13 09:57:13.000000 gocardless_pro-1.8.0/tests/
-drwxr-xr-x   0 cristiangreco   (501) staff       (20)        0 2018-07-13 09:57:13.000000 gocardless_pro-1.8.0/tests/integration/
--rw-r--r--   0 cristiangreco   (501) staff       (20)        0 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/tests/integration/__init__.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     2258 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/tests/integration/bank_details_lookups_integration_test.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)    11967 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/tests/integration/creditor_bank_accounts_integration_test.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)    14636 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/tests/integration/creditors_integration_test.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)    14254 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/tests/integration/customer_bank_accounts_integration_test.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)    13659 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/tests/integration/customers_integration_test.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     6875 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/tests/integration/events_integration_test.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     5924 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/tests/integration/mandate_import_entries_integration_test.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     7500 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/tests/integration/mandate_imports_integration_test.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     2055 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/tests/integration/mandate_pdfs_integration_test.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)    15937 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/tests/integration/mandates_integration_test.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)    16297 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/tests/integration/payments_integration_test.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     3536 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/tests/integration/payout_items_integration_test.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     6344 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/tests/integration/payouts_integration_test.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)     8210 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/tests/integration/redirect_flows_integration_test.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)    10510 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/tests/integration/refunds_integration_test.py
--rw-r--r--   0 cristiangreco   (501) staff       (20)    15779 2018-07-13 09:36:24.000000 gocardless_pro-1.8.0/tests/integration/subscriptions_integration_test.py
+drwxr-xr-x   0 jamesturley   (501) staff       (20)        0 2018-10-04 09:45:42.000000 gocardless_pro-1.9.0/
+-rw-r--r--   0 jamesturley   (501) staff       (20)    12615 2018-10-04 09:45:42.000000 gocardless_pro-1.9.0/PKG-INFO
+drwxr-xr-x   0 jamesturley   (501) staff       (20)        0 2018-10-04 09:45:42.000000 gocardless_pro-1.9.0/tests/
+drwxr-xr-x   0 jamesturley   (501) staff       (20)        0 2018-10-04 09:45:42.000000 gocardless_pro-1.9.0/tests/integration/
+-rw-r--r--   0 jamesturley   (501) staff       (20)     2258 2017-12-04 15:26:35.000000 gocardless_pro-1.9.0/tests/integration/bank_details_lookups_integration_test.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)    15937 2017-12-04 15:26:35.000000 gocardless_pro-1.9.0/tests/integration/mandates_integration_test.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)    15014 2018-09-28 09:33:36.000000 gocardless_pro-1.9.0/tests/integration/creditors_integration_test.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)    13974 2018-09-28 09:33:36.000000 gocardless_pro-1.9.0/tests/integration/customers_integration_test.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)    11967 2017-12-04 15:26:35.000000 gocardless_pro-1.9.0/tests/integration/creditor_bank_accounts_integration_test.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)        0 2017-12-04 15:26:35.000000 gocardless_pro-1.9.0/tests/integration/__init__.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     2055 2017-12-04 15:26:35.000000 gocardless_pro-1.9.0/tests/integration/mandate_pdfs_integration_test.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     7500 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/tests/integration/mandate_imports_integration_test.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     8210 2017-12-04 15:26:35.000000 gocardless_pro-1.9.0/tests/integration/redirect_flows_integration_test.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)    10510 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/tests/integration/refunds_integration_test.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     6344 2017-12-04 15:26:35.000000 gocardless_pro-1.9.0/tests/integration/payouts_integration_test.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     3536 2017-12-04 15:26:35.000000 gocardless_pro-1.9.0/tests/integration/payout_items_integration_test.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)    16297 2017-12-04 15:26:35.000000 gocardless_pro-1.9.0/tests/integration/payments_integration_test.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     5924 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/tests/integration/mandate_import_entries_integration_test.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)    14254 2017-12-04 15:26:35.000000 gocardless_pro-1.9.0/tests/integration/customer_bank_accounts_integration_test.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     2472 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/tests/integration/customer_notifications_integration_test.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)    15779 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/tests/integration/subscriptions_integration_test.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     7098 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/tests/integration/events_integration_test.py
+drwxr-xr-x   0 jamesturley   (501) staff       (20)        0 2018-10-04 09:45:42.000000 gocardless_pro-1.9.0/gocardless_pro/
+-rw-r--r--   0 jamesturley   (501) staff       (20)      465 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/list_response.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     3793 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/client.py
+drwxr-xr-x   0 jamesturley   (501) staff       (20)        0 2018-10-04 09:45:42.000000 gocardless_pro-1.9.0/gocardless_pro/resources/
+-rw-r--r--   0 jamesturley   (501) staff       (20)     3183 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/resources/event.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)      786 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/resources/bank_details_lookup.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     2340 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/resources/subscription.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     1773 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/resources/payout.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     1958 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/resources/redirect_flow.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)      790 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/resources/__init__.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)      817 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/resources/mandate_import.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     2914 2018-09-28 09:33:36.000000 gocardless_pro-1.9.0/gocardless_pro/resources/creditor.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     1939 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/resources/mandate.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)      626 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/resources/mandate_pdf.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     2208 2018-09-28 09:33:36.000000 gocardless_pro-1.9.0/gocardless_pro/resources/customer.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     1417 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/resources/mandate_import_entry.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     1094 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/resources/payout_item.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     2053 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/resources/payment.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     1756 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/resources/customer_bank_account.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     1444 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/resources/refund.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     1756 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/resources/creditor_bank_account.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     1857 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/resources/customer_notification.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)      103 2018-10-04 09:40:58.000000 gocardless_pro-1.9.0/gocardless_pro/__init__.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)      561 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/api_response.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)      874 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/paginator.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     3092 2018-10-01 07:51:55.000000 gocardless_pro-1.9.0/gocardless_pro/errors.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     1372 2018-10-04 09:35:30.000000 gocardless_pro-1.9.0/gocardless_pro/webhooks.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     4283 2018-10-04 09:40:59.000000 gocardless_pro-1.9.0/gocardless_pro/api_client.py
+drwxr-xr-x   0 jamesturley   (501) staff       (20)        0 2018-10-04 09:45:42.000000 gocardless_pro-1.9.0/gocardless_pro/services/
+-rw-r--r--   0 jamesturley   (501) staff       (20)     4551 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/services/mandate_imports_service.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     3387 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/services/creditors_service.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     2932 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/services/mandate_pdfs_service.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     1903 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/services/payouts_service.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     5767 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/services/mandates_service.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     1874 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/services/bank_details_lookups_service.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     1064 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/services/__init__.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     2602 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/services/base_service.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     5506 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/services/subscriptions_service.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     5101 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/services/customer_bank_accounts_service.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     1751 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/services/events_service.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     3394 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/services/customers_service.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     3477 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/services/redirect_flows_service.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     1158 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/services/payout_items_service.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     2362 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/services/mandate_import_entries_service.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     6024 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/services/payments_service.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     3875 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/services/creditor_bank_accounts_service.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     1592 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/services/customer_notifications_service.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)     4027 2018-09-24 10:01:29.000000 gocardless_pro-1.9.0/gocardless_pro/services/refunds_service.py
+-rw-r--r--   0 jamesturley   (501) staff       (20)      637 2018-10-04 09:40:59.000000 gocardless_pro-1.9.0/setup.py
+drwxr-xr-x   0 jamesturley   (501) staff       (20)        0 2018-10-04 09:45:42.000000 gocardless_pro-1.9.0/gocardless_pro.egg-info/
+-rw-r--r--   0 jamesturley   (501) staff       (20)    12615 2018-10-04 09:45:42.000000 gocardless_pro-1.9.0/gocardless_pro.egg-info/PKG-INFO
+-rw-r--r--   0 jamesturley   (501) staff       (20)     3009 2018-10-04 09:45:42.000000 gocardless_pro-1.9.0/gocardless_pro.egg-info/SOURCES.txt
+-rw-r--r--   0 jamesturley   (501) staff       (20)       18 2018-10-04 09:45:42.000000 gocardless_pro-1.9.0/gocardless_pro.egg-info/requires.txt
+-rw-r--r--   0 jamesturley   (501) staff       (20)       21 2018-10-04 09:45:42.000000 gocardless_pro-1.9.0/gocardless_pro.egg-info/top_level.txt
+-rw-r--r--   0 jamesturley   (501) staff       (20)        1 2018-10-04 09:45:42.000000 gocardless_pro-1.9.0/gocardless_pro.egg-info/dependency_links.txt
+-rw-r--r--   0 jamesturley   (501) staff       (20)       38 2018-10-04 09:45:42.000000 gocardless_pro-1.9.0/setup.cfg
+-rw-r--r--   0 jamesturley   (501) staff       (20)     9299 2018-10-04 09:35:30.000000 gocardless_pro-1.9.0/README.rst
```

### Comparing `gocardless_pro-1.8.0/gocardless_pro/api_client.py` & `gocardless_pro-1.9.0/gocardless_pro/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,22 +116,22 @@
 
     def _default_headers(self):
         return {
             'Accept': 'application/json',
             'Authorization': 'Bearer {0}'.format(self.access_token),
             'Content-Type': 'application/json',
             'GoCardless-Client-Library': 'gocardless-pro-python',
-            'GoCardless-Client-Version': '1.8.0',
+            'GoCardless-Client-Version': '1.9.0',
             'User-Agent': self._user_agent(),
             'GoCardless-Version': '2015-07-06',
         }
 
     def _user_agent(self):
         python_version = '.'.join(platform.python_version_tuple()[0:2])
         vm_version = '{}.{}.{}-{}{}'.format(*sys.version_info)
         return ' '.join([
-            'gocardless-pro-python/1.8.0',
+            'gocardless-pro-python/1.9.0',
             'python/{0}'.format(python_version),
             '{0}/{1}'.format(platform.python_implementation(), vm_version),
             '{0}/{1}'.format(platform.system(), platform.release()),
             'requests/{0}'.format(requests.__version__),
         ])
```

### Comparing `gocardless_pro-1.8.0/gocardless_pro/api_response.py` & `gocardless_pro-1.9.0/gocardless_pro/api_response.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/gocardless_pro/client.py` & `gocardless_pro-1.9.0/gocardless_pro/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,18 @@
         return services.CustomersService(self._api_client, 3, 0.5)
 
     @property
     def customer_bank_accounts(self):
         return services.CustomerBankAccountsService(self._api_client, 3, 0.5)
 
     @property
+    def customer_notifications(self):
+        return services.CustomerNotificationsService(self._api_client, 3, 0.5)
+
+    @property
     def events(self):
         return services.EventsService(self._api_client, 3, 0.5)
 
     @property
     def mandates(self):
         return services.MandatesService(self._api_client, 3, 0.5)
```

### Comparing `gocardless_pro-1.8.0/gocardless_pro/errors.py` & `gocardless_pro-1.9.0/gocardless_pro/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,7 +99,13 @@
 
 
 class MalformedResponseError(GoCardlessProError):
 
     def __init__(self, message, response):
         super(MalformedResponseError, self).__init__(message)
         self.response = response
+
+
+class InvalidSignatureError(GoCardlessProError):
+    pass
+
+
```

### Comparing `gocardless_pro-1.8.0/gocardless_pro/paginator.py` & `gocardless_pro-1.9.0/gocardless_pro/paginator.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/gocardless_pro/resources/bank_details_lookup.py` & `gocardless_pro-1.9.0/gocardless_pro/resources/bank_details_lookup.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/gocardless_pro/resources/creditor.py` & `gocardless_pro-1.9.0/gocardless_pro/resources/creditor.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,14 +128,18 @@
             return self.attributes.get('default_eur_payout_account')
     
         @property
         def default_gbp_payout_account(self):
             return self.attributes.get('default_gbp_payout_account')
     
         @property
+        def default_nzd_payout_account(self):
+            return self.attributes.get('default_nzd_payout_account')
+    
+        @property
         def default_sek_payout_account(self):
             return self.attributes.get('default_sek_payout_account')
```

### Comparing `gocardless_pro-1.8.0/gocardless_pro/resources/creditor_bank_account.py` & `gocardless_pro-1.9.0/gocardless_pro/resources/creditor_bank_account.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/gocardless_pro/resources/customer.py` & `gocardless_pro-1.9.0/gocardless_pro/resources/customer.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,19 @@
 
     @property
     def metadata(self):
         return self.attributes.get('metadata')
   
 
     @property
+    def phone_number(self):
+        return self.attributes.get('phone_number')
+  
+
+    @property
     def postal_code(self):
         return self.attributes.get('postal_code')
   
 
     @property
     def region(self):
         return self.attributes.get('region')
@@ -104,14 +109,16 @@
 
   
 
   
 
   
 
+  
+
```

### Comparing `gocardless_pro-1.8.0/gocardless_pro/resources/customer_bank_account.py` & `gocardless_pro-1.9.0/gocardless_pro/resources/customer_bank_account.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/gocardless_pro/resources/event.py` & `gocardless_pro-1.9.0/gocardless_pro/resources/event.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,19 @@
 
     @property
     def created_at(self):
         return self.attributes.get('created_at')
   
 
     @property
+    def customer_notifications(self):
+        return self.attributes.get('customer_notifications')
+  
+
+    @property
     def details(self):
         return self.Details(self.attributes.get('details'))
   
 
     @property
     def id(self):
         return self.attributes.get('id')
@@ -53,14 +58,16 @@
 
 
   
 
   
 
   
+
+  
     class Details(object):
         """Wrapper for the response's 'details' attribute."""
 
         def __init__(self, attributes):
             self.attributes = attributes
     
         @property
```

### Comparing `gocardless_pro-1.8.0/gocardless_pro/resources/mandate.py` & `gocardless_pro-1.9.0/gocardless_pro/resources/mandate.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/gocardless_pro/resources/mandate_import.py` & `gocardless_pro-1.9.0/gocardless_pro/resources/mandate_import.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/gocardless_pro/resources/mandate_import_entry.py` & `gocardless_pro-1.9.0/gocardless_pro/resources/mandate_import_entry.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/gocardless_pro/resources/mandate_pdf.py` & `gocardless_pro-1.9.0/gocardless_pro/resources/mandate_pdf.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/gocardless_pro/resources/payment.py` & `gocardless_pro-1.9.0/gocardless_pro/resources/payment.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/gocardless_pro/resources/payout.py` & `gocardless_pro-1.9.0/gocardless_pro/resources/payout.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/gocardless_pro/resources/payout_item.py` & `gocardless_pro-1.9.0/gocardless_pro/resources/payout_item.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/gocardless_pro/resources/redirect_flow.py` & `gocardless_pro-1.9.0/gocardless_pro/resources/redirect_flow.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/gocardless_pro/resources/refund.py` & `gocardless_pro-1.9.0/gocardless_pro/resources/refund.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/gocardless_pro/resources/subscription.py` & `gocardless_pro-1.9.0/gocardless_pro/resources/subscription.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/gocardless_pro/services/__init__.py` & `gocardless_pro-1.9.0/gocardless_pro/services/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 #
 
 from .bank_details_lookups_service import BankDetailsLookupsService
 from .creditors_service import CreditorsService
 from .creditor_bank_accounts_service import CreditorBankAccountsService
 from .customers_service import CustomersService
 from .customer_bank_accounts_service import CustomerBankAccountsService
+from .customer_notifications_service import CustomerNotificationsService
 from .events_service import EventsService
 from .mandates_service import MandatesService
 from .mandate_imports_service import MandateImportsService
 from .mandate_import_entries_service import MandateImportEntriesService
 from .mandate_pdfs_service import MandatePdfsService
 from .payments_service import PaymentsService
 from .payouts_service import PayoutsService
```

### Comparing `gocardless_pro-1.8.0/gocardless_pro/services/bank_details_lookups_service.py` & `gocardless_pro-1.9.0/gocardless_pro/services/bank_details_lookups_service.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/gocardless_pro/services/base_service.py` & `gocardless_pro-1.9.0/gocardless_pro/services/base_service.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/gocardless_pro/services/creditor_bank_accounts_service.py` & `gocardless_pro-1.9.0/gocardless_pro/services/creditor_bank_accounts_service.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/gocardless_pro/services/creditors_service.py` & `gocardless_pro-1.9.0/gocardless_pro/services/creditors_service.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/gocardless_pro/services/customer_bank_accounts_service.py` & `gocardless_pro-1.9.0/gocardless_pro/services/customer_bank_accounts_service.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/gocardless_pro/services/customers_service.py` & `gocardless_pro-1.9.0/gocardless_pro/services/customers_service.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/gocardless_pro/services/events_service.py` & `gocardless_pro-1.9.0/gocardless_pro/services/events_service.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/gocardless_pro/services/mandate_import_entries_service.py` & `gocardless_pro-1.9.0/gocardless_pro/services/mandate_import_entries_service.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/gocardless_pro/services/mandate_imports_service.py` & `gocardless_pro-1.9.0/gocardless_pro/services/mandate_imports_service.py`

 * *Files 19% similar despite different names*

```diff
@@ -75,14 +75,22 @@
         """Submit a mandate import.
 
         Submits the mandate import, which allows it to be processed by a member
         of the
         GoCardless team. Once the import has been submitted, it can no longer
         have entries
         added to it.
+        
+        In our sandbox environment, to aid development, we automatically
+        process mandate
+        imports approximately 10 seconds after they are submitted. This will
+        allow you to
+        test both the "submitted" response and wait for the webhook to confirm
+        the
+        processing has begun.
 
         Args:
               identity (string): Unique identifier, beginning with "IM".
               params (dict, optional): Request body.
 
         Returns:
               ListResponse of MandateImport instances
@@ -103,16 +111,16 @@
         """Cancel a mandate import.
 
         Cancels the mandate import, which aborts the import process and stops
         the mandates
         being set up in GoCardless. Once the import has been cancelled, it can
         no longer have
         entries added to it. Mandate imports which have already been submitted
-        cannot be
-        cancelled.
+        or processed
+        cannot be cancelled.
 
         Args:
               identity (string): Unique identifier, beginning with "IM".
               params (dict, optional): Request body.
 
         Returns:
               ListResponse of MandateImport instances
```

### Comparing `gocardless_pro-1.8.0/gocardless_pro/services/mandate_pdfs_service.py` & `gocardless_pro-1.9.0/gocardless_pro/services/mandate_pdfs_service.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/gocardless_pro/services/mandates_service.py` & `gocardless_pro-1.9.0/gocardless_pro/services/mandates_service.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/gocardless_pro/services/payments_service.py` & `gocardless_pro-1.9.0/gocardless_pro/services/payments_service.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/gocardless_pro/services/payout_items_service.py` & `gocardless_pro-1.9.0/gocardless_pro/services/payout_items_service.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/gocardless_pro/services/payouts_service.py` & `gocardless_pro-1.9.0/gocardless_pro/services/payouts_service.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/gocardless_pro/services/redirect_flows_service.py` & `gocardless_pro-1.9.0/gocardless_pro/services/redirect_flows_service.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/gocardless_pro/services/refunds_service.py` & `gocardless_pro-1.9.0/gocardless_pro/services/refunds_service.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/gocardless_pro/services/subscriptions_service.py` & `gocardless_pro-1.9.0/gocardless_pro/services/subscriptions_service.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/gocardless_pro.egg-info/PKG-INFO` & `gocardless_pro-1.9.0/gocardless_pro.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: gocardless-pro
-Version: 1.8.0
+Version: 1.9.0
 Summary: A client library for the GoCardless Pro API.
 Home-page: https://github.com/gocardless/gocardless-pro-python
 Author: GoCardless
 Author-email: engineering@gocardless.com
 License: MIT
 Description: .. |circle-badge| image:: https://circleci.com/gh/gocardless/gocardless-pro-python.svg?style=shield&circle-token=:circle-token
             :target: https://circleci.com/gh/gocardless/gocardless-pro-python
@@ -14,15 +14,15 @@
         GoCardless Pro Python client library
         ============================================
         
         A Python client for interacting with the GoCardless Pro API.
         
         |circle-badge| |pypi-badge|
         
-        Tested against Python 2.7, 3.3, 3.4, 3.5, and 3.6.
+        Tested against Python 2.7, 3.3, 3.4, 3.5, 3.6 and 3.7.
         
         - `"Getting Started" guide <https://developer.gocardless.com/getting-started/api/introduction/?lang=python>`_ with copy and paste Python code samples
         - `API reference`_
         
         ------------
         
         Install from PyPI:
@@ -163,14 +163,22 @@
         
             # Update a customer bank account
             client.customer_bank_accounts.update('BA123', params={...})
         
             # Disable a customer bank account
             client.customer_bank_accounts.disable('BA123', params={...})
         
+        Customer notifications
+        ''''''''''''''''''''''''''''''''''''''''''
+        
+        .. code:: python
+        
+            # Handle a notification
+            client.customer_notifications.handle('PCN123', params={...})
+        
         Events
         ''''''''''''''''''''''''''''''''''''''''''
         
         .. code:: python
         
             # List events
             client.events.list(params={...})
```

### Comparing `gocardless_pro-1.8.0/gocardless_pro.egg-info/SOURCES.txt` & `gocardless_pro-1.9.0/gocardless_pro.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 gocardless_pro/__init__.py
 gocardless_pro/api_client.py
 gocardless_pro/api_response.py
 gocardless_pro/client.py
 gocardless_pro/errors.py
 gocardless_pro/list_response.py
 gocardless_pro/paginator.py
+gocardless_pro/webhooks.py
 gocardless_pro.egg-info/PKG-INFO
 gocardless_pro.egg-info/SOURCES.txt
 gocardless_pro.egg-info/dependency_links.txt
 gocardless_pro.egg-info/requires.txt
 gocardless_pro.egg-info/top_level.txt
 gocardless_pro/resources/__init__.py
 gocardless_pro/resources/bank_details_lookup.py
 gocardless_pro/resources/creditor.py
 gocardless_pro/resources/creditor_bank_account.py
 gocardless_pro/resources/customer.py
 gocardless_pro/resources/customer_bank_account.py
+gocardless_pro/resources/customer_notification.py
 gocardless_pro/resources/event.py
 gocardless_pro/resources/mandate.py
 gocardless_pro/resources/mandate_import.py
 gocardless_pro/resources/mandate_import_entry.py
 gocardless_pro/resources/mandate_pdf.py
 gocardless_pro/resources/payment.py
 gocardless_pro/resources/payout.py
@@ -31,14 +33,15 @@
 gocardless_pro/resources/subscription.py
 gocardless_pro/services/__init__.py
 gocardless_pro/services/bank_details_lookups_service.py
 gocardless_pro/services/base_service.py
 gocardless_pro/services/creditor_bank_accounts_service.py
 gocardless_pro/services/creditors_service.py
 gocardless_pro/services/customer_bank_accounts_service.py
+gocardless_pro/services/customer_notifications_service.py
 gocardless_pro/services/customers_service.py
 gocardless_pro/services/events_service.py
 gocardless_pro/services/mandate_import_entries_service.py
 gocardless_pro/services/mandate_imports_service.py
 gocardless_pro/services/mandate_pdfs_service.py
 gocardless_pro/services/mandates_service.py
 gocardless_pro/services/payments_service.py
@@ -48,14 +51,15 @@
 gocardless_pro/services/refunds_service.py
 gocardless_pro/services/subscriptions_service.py
 tests/integration/__init__.py
 tests/integration/bank_details_lookups_integration_test.py
 tests/integration/creditor_bank_accounts_integration_test.py
 tests/integration/creditors_integration_test.py
 tests/integration/customer_bank_accounts_integration_test.py
+tests/integration/customer_notifications_integration_test.py
 tests/integration/customers_integration_test.py
 tests/integration/events_integration_test.py
 tests/integration/mandate_import_entries_integration_test.py
 tests/integration/mandate_imports_integration_test.py
 tests/integration/mandate_pdfs_integration_test.py
 tests/integration/mandates_integration_test.py
 tests/integration/payments_integration_test.py
```

### Comparing `gocardless_pro-1.8.0/PKG-INFO` & `gocardless_pro-1.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: gocardless_pro
-Version: 1.8.0
+Version: 1.9.0
 Summary: A client library for the GoCardless Pro API.
 Home-page: https://github.com/gocardless/gocardless-pro-python
 Author: GoCardless
 Author-email: engineering@gocardless.com
 License: MIT
 Description: .. |circle-badge| image:: https://circleci.com/gh/gocardless/gocardless-pro-python.svg?style=shield&circle-token=:circle-token
             :target: https://circleci.com/gh/gocardless/gocardless-pro-python
@@ -14,15 +14,15 @@
         GoCardless Pro Python client library
         ============================================
         
         A Python client for interacting with the GoCardless Pro API.
         
         |circle-badge| |pypi-badge|
         
-        Tested against Python 2.7, 3.3, 3.4, 3.5, and 3.6.
+        Tested against Python 2.7, 3.3, 3.4, 3.5, 3.6 and 3.7.
         
         - `"Getting Started" guide <https://developer.gocardless.com/getting-started/api/introduction/?lang=python>`_ with copy and paste Python code samples
         - `API reference`_
         
         ------------
         
         Install from PyPI:
@@ -163,14 +163,22 @@
         
             # Update a customer bank account
             client.customer_bank_accounts.update('BA123', params={...})
         
             # Disable a customer bank account
             client.customer_bank_accounts.disable('BA123', params={...})
         
+        Customer notifications
+        ''''''''''''''''''''''''''''''''''''''''''
+        
+        .. code:: python
+        
+            # Handle a notification
+            client.customer_notifications.handle('PCN123', params={...})
+        
         Events
         ''''''''''''''''''''''''''''''''''''''''''
         
         .. code:: python
         
             # List events
             client.events.list(params={...})
```

### Comparing `gocardless_pro-1.8.0/README.rst` & `gocardless_pro-1.9.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 GoCardless Pro Python client library
 ============================================
 
 A Python client for interacting with the GoCardless Pro API.
 
 |circle-badge| |pypi-badge|
 
-Tested against Python 2.7, 3.3, 3.4, 3.5, and 3.6.
+Tested against Python 2.7, 3.3, 3.4, 3.5, 3.6 and 3.7.
 
 - `"Getting Started" guide <https://developer.gocardless.com/getting-started/api/introduction/?lang=python>`_ with copy and paste Python code samples
 - `API reference`_
 
 ------------
 
 Install from PyPI:
@@ -155,14 +155,22 @@
 
     # Update a customer bank account
     client.customer_bank_accounts.update('BA123', params={...})
 
     # Disable a customer bank account
     client.customer_bank_accounts.disable('BA123', params={...})
 
+Customer notifications
+''''''''''''''''''''''''''''''''''''''''''
+
+.. code:: python
+
+    # Handle a notification
+    client.customer_notifications.handle('PCN123', params={...})
+
 Events
 ''''''''''''''''''''''''''''''''''''''''''
 
 .. code:: python
 
     # List events
     client.events.list(params={...})
```

### Comparing `gocardless_pro-1.8.0/setup.py` & `gocardless_pro-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with codecs.open('README.rst', 'r', 'utf-8') as file:
     long_description = file.read()
 
 setup(
     name = 'gocardless_pro',
-    version = '1.8.0',
+    version = '1.9.0',
     packages = find_packages(exclude=['tests']),
     install_requires = ['requests>=2.6', 'six'],
     author = 'GoCardless',
     author_email = 'engineering@gocardless.com',
     description = 'A client library for the GoCardless Pro API.',
     long_description = long_description,
     license = 'MIT',
```

### Comparing `gocardless_pro-1.8.0/tests/integration/bank_details_lookups_integration_test.py` & `gocardless_pro-1.9.0/tests/integration/bank_details_lookups_integration_test.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/tests/integration/creditor_bank_accounts_integration_test.py` & `gocardless_pro-1.9.0/tests/integration/creditor_bank_accounts_integration_test.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/tests/integration/creditors_integration_test.py` & `gocardless_pro-1.9.0/tests/integration/creditors_integration_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,16 @@
                  body.get('links')['default_aud_payout_account'])
     assert_equal(response.links.default_dkk_payout_account,
                  body.get('links')['default_dkk_payout_account'])
     assert_equal(response.links.default_eur_payout_account,
                  body.get('links')['default_eur_payout_account'])
     assert_equal(response.links.default_gbp_payout_account,
                  body.get('links')['default_gbp_payout_account'])
+    assert_equal(response.links.default_nzd_payout_account,
+                 body.get('links')['default_nzd_payout_account'])
     assert_equal(response.links.default_sek_payout_account,
                  body.get('links')['default_sek_payout_account'])
 
 @responses.activate
 def test_creditors_create_new_idempotency_key_for_each_call():
     fixture = helpers.load_fixture('creditors')['create']
     helpers.stub_response(fixture)
@@ -220,14 +222,16 @@
                  body.get('links')['default_aud_payout_account'])
     assert_equal(response.links.default_dkk_payout_account,
                  body.get('links')['default_dkk_payout_account'])
     assert_equal(response.links.default_eur_payout_account,
                  body.get('links')['default_eur_payout_account'])
     assert_equal(response.links.default_gbp_payout_account,
                  body.get('links')['default_gbp_payout_account'])
+    assert_equal(response.links.default_nzd_payout_account,
+                 body.get('links')['default_nzd_payout_account'])
     assert_equal(response.links.default_sek_payout_account,
                  body.get('links')['default_sek_payout_account'])
 
 @responses.activate
 def test_timeout_creditors_get_retries():
     fixture = helpers.load_fixture('creditors')['get']
     with helpers.stub_timeout_then_response(fixture) as rsps:
@@ -278,14 +282,16 @@
                  body.get('links')['default_aud_payout_account'])
     assert_equal(response.links.default_dkk_payout_account,
                  body.get('links')['default_dkk_payout_account'])
     assert_equal(response.links.default_eur_payout_account,
                  body.get('links')['default_eur_payout_account'])
     assert_equal(response.links.default_gbp_payout_account,
                  body.get('links')['default_gbp_payout_account'])
+    assert_equal(response.links.default_nzd_payout_account,
+                 body.get('links')['default_nzd_payout_account'])
     assert_equal(response.links.default_sek_payout_account,
                  body.get('links')['default_sek_payout_account'])
 
 @responses.activate
 def test_timeout_creditors_update_retries():
     fixture = helpers.load_fixture('creditors')['update']
     with helpers.stub_timeout_then_response(fixture) as rsps:
```

### Comparing `gocardless_pro-1.8.0/tests/integration/customer_bank_accounts_integration_test.py` & `gocardless_pro-1.9.0/tests/integration/customer_bank_accounts_integration_test.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/tests/integration/customers_integration_test.py` & `gocardless_pro-1.9.0/tests/integration/customers_integration_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     assert_equal(response.danish_identity_number, body.get('danish_identity_number'))
     assert_equal(response.email, body.get('email'))
     assert_equal(response.family_name, body.get('family_name'))
     assert_equal(response.given_name, body.get('given_name'))
     assert_equal(response.id, body.get('id'))
     assert_equal(response.language, body.get('language'))
     assert_equal(response.metadata, body.get('metadata'))
+    assert_equal(response.phone_number, body.get('phone_number'))
     assert_equal(response.postal_code, body.get('postal_code'))
     assert_equal(response.region, body.get('region'))
     assert_equal(response.swedish_identity_number, body.get('swedish_identity_number'))
 
 @responses.activate
 def test_customers_create_new_idempotency_key_for_each_call():
     fixture = helpers.load_fixture('customers')['create']
@@ -129,14 +130,16 @@
                  [b.get('given_name') for b in body])
     assert_equal([r.id for r in response.records],
                  [b.get('id') for b in body])
     assert_equal([r.language for r in response.records],
                  [b.get('language') for b in body])
     assert_equal([r.metadata for r in response.records],
                  [b.get('metadata') for b in body])
+    assert_equal([r.phone_number for r in response.records],
+                 [b.get('phone_number') for b in body])
     assert_equal([r.postal_code for r in response.records],
                  [b.get('postal_code') for b in body])
     assert_equal([r.region for r in response.records],
                  [b.get('region') for b in body])
     assert_equal([r.swedish_identity_number for r in response.records],
                  [b.get('swedish_identity_number') for b in body])
 
@@ -211,14 +214,15 @@
     assert_equal(response.danish_identity_number, body.get('danish_identity_number'))
     assert_equal(response.email, body.get('email'))
     assert_equal(response.family_name, body.get('family_name'))
     assert_equal(response.given_name, body.get('given_name'))
     assert_equal(response.id, body.get('id'))
     assert_equal(response.language, body.get('language'))
     assert_equal(response.metadata, body.get('metadata'))
+    assert_equal(response.phone_number, body.get('phone_number'))
     assert_equal(response.postal_code, body.get('postal_code'))
     assert_equal(response.region, body.get('region'))
     assert_equal(response.swedish_identity_number, body.get('swedish_identity_number'))
 
 @responses.activate
 def test_timeout_customers_get_retries():
     fixture = helpers.load_fixture('customers')['get']
@@ -262,14 +266,15 @@
     assert_equal(response.danish_identity_number, body.get('danish_identity_number'))
     assert_equal(response.email, body.get('email'))
     assert_equal(response.family_name, body.get('family_name'))
     assert_equal(response.given_name, body.get('given_name'))
     assert_equal(response.id, body.get('id'))
     assert_equal(response.language, body.get('language'))
     assert_equal(response.metadata, body.get('metadata'))
+    assert_equal(response.phone_number, body.get('phone_number'))
     assert_equal(response.postal_code, body.get('postal_code'))
     assert_equal(response.region, body.get('region'))
     assert_equal(response.swedish_identity_number, body.get('swedish_identity_number'))
 
 @responses.activate
 def test_timeout_customers_update_retries():
     fixture = helpers.load_fixture('customers')['update']
```

### Comparing `gocardless_pro-1.8.0/tests/integration/events_integration_test.py` & `gocardless_pro-1.9.0/tests/integration/events_integration_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,16 @@
     assert_equal(response.before, fixture['body']['meta']['cursors']['before'])
     assert_equal(response.after, fixture['body']['meta']['cursors']['after'])
     assert_is_none(responses.calls[-1].request.headers.get('Idempotency-Key'))
     assert_equal([r.action for r in response.records],
                  [b.get('action') for b in body])
     assert_equal([r.created_at for r in response.records],
                  [b.get('created_at') for b in body])
+    assert_equal([r.customer_notifications for r in response.records],
+                 [b.get('customer_notifications') for b in body])
     assert_equal([r.id for r in response.records],
                  [b.get('id') for b in body])
     assert_equal([r.metadata for r in response.records],
                  [b.get('metadata') for b in body])
     assert_equal([r.resource_type for r in response.records],
                  [b.get('resource_type') for b in body])
 
@@ -106,14 +108,15 @@
     response = helpers.client.events.get(*fixture['url_params'])
     body = fixture['body']['events']
 
     assert_is_instance(response, resources.Event)
     assert_is_none(responses.calls[-1].request.headers.get('Idempotency-Key'))
     assert_equal(response.action, body.get('action'))
     assert_equal(response.created_at, body.get('created_at'))
+    assert_equal(response.customer_notifications, body.get('customer_notifications'))
     assert_equal(response.id, body.get('id'))
     assert_equal(response.metadata, body.get('metadata'))
     assert_equal(response.resource_type, body.get('resource_type'))
     assert_equal(response.details.cause,
                  body.get('details')['cause'])
     assert_equal(response.details.description,
                  body.get('details')['description'])
```

### Comparing `gocardless_pro-1.8.0/tests/integration/mandate_import_entries_integration_test.py` & `gocardless_pro-1.9.0/tests/integration/mandate_import_entries_integration_test.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/tests/integration/mandate_imports_integration_test.py` & `gocardless_pro-1.9.0/tests/integration/mandate_imports_integration_test.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/tests/integration/mandate_pdfs_integration_test.py` & `gocardless_pro-1.9.0/tests/integration/mandate_pdfs_integration_test.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/tests/integration/mandates_integration_test.py` & `gocardless_pro-1.9.0/tests/integration/mandates_integration_test.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/tests/integration/payments_integration_test.py` & `gocardless_pro-1.9.0/tests/integration/payments_integration_test.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/tests/integration/payout_items_integration_test.py` & `gocardless_pro-1.9.0/tests/integration/payout_items_integration_test.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/tests/integration/payouts_integration_test.py` & `gocardless_pro-1.9.0/tests/integration/payouts_integration_test.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/tests/integration/redirect_flows_integration_test.py` & `gocardless_pro-1.9.0/tests/integration/redirect_flows_integration_test.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/tests/integration/refunds_integration_test.py` & `gocardless_pro-1.9.0/tests/integration/refunds_integration_test.py`

 * *Files identical despite different names*

### Comparing `gocardless_pro-1.8.0/tests/integration/subscriptions_integration_test.py` & `gocardless_pro-1.9.0/tests/integration/subscriptions_integration_test.py`

 * *Files identical despite different names*

