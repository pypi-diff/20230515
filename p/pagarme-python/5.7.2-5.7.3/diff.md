# Comparing `tmp/pagarme-python-5.7.2.tar.gz` & `tmp/pagarme-python-5.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pagarme-python-5.7.2.tar", last modified: Mon Apr  3 17:33:23 2023, max compression
+gzip compressed data, was "dist/pagarme-python-5.7.3.tar", last modified: Mon May 15 20:13:48 2023, max compression
```

## Comparing `pagarme-python-5.7.2.tar` & `pagarme-python-5.7.3.tar`

### file list

```diff
@@ -1,272 +1,272 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 17:33:23.000000 pagarme-python-5.7.2/
--rw-r--r--   0 root         (0) root         (0)     1213 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       36 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 17:33:23.000000 pagarme-python-5.7.2/tests/
--rw-r--r--   0 root         (0) root         (0)      681 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/tests/http_response_catcher.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5125 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/tests/test_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 17:33:23.000000 pagarme-python-5.7.2/tests/controllers/
--rw-r--r--   0 root         (0) root         (0)     1321 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/tests/controllers/test_plans_controller.py
--rw-r--r--   0 root         (0) root         (0)     1718 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/tests/controllers/test_recipients_controller.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/tests/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      999 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/tests/controllers/controller_test_base.py
--rw-r--r--   0 root         (0) root         (0)     1586 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/tests/controllers/test_subscriptions_controller.py
--rw-r--r--   0 root         (0) root         (0)     1067 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/tests/controllers/test_transfers_controller.py
--rw-r--r--   0 root         (0) root         (0)     1513 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/tests/controllers/test_invoices_controller.py
--rw-r--r--   0 root         (0) root         (0)     1266 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/tests/controllers/test_customers_controller.py
--rw-r--r--   0 root         (0) root         (0)     1325 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/tests/controllers/test_orders_controller.py
--rw-r--r--   0 root         (0) root         (0)     1414 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/tests/controllers/test_charges_controller.py
--rw-r--r--   0 root         (0) root         (0)      244 2023-04-03 17:33:23.000000 pagarme-python-5.7.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      872 2023-04-03 17:33:21.000000 pagarme-python-5.7.2/setup.py
--rw-r--r--   0 root         (0) root         (0)       59 2023-04-03 17:33:23.000000 pagarme-python-5.7.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 17:33:23.000000 pagarme-python-5.7.2/pagarme_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)      244 2023-04-03 17:33:23.000000 pagarme-python-5.7.2/pagarme_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12967 2023-04-03 17:33:23.000000 pagarme-python-5.7.2/pagarme_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-03 17:33:23.000000 pagarme-python-5.7.2/pagarme_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-03 17:33:23.000000 pagarme-python-5.7.2/pagarme_python.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      102 2023-04-03 17:33:23.000000 pagarme-python-5.7.2/pagarme_python.egg-info/requires.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 17:33:23.000000 pagarme-python-5.7.2/pagarmecoreapi/
--rw-r--r--   0 root         (0) root         (0)    13744 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/api_helper.py
--rw-r--r--   0 root         (0) root         (0)     2327 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/pagarmecoreapi_client.py
--rw-r--r--   0 root         (0) root         (0)      169 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 17:33:23.000000 pagarme-python-5.7.2/pagarmecoreapi/exceptions/
--rw-r--r--   0 root         (0) root         (0)       58 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      906 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/exceptions/api_exception.py
--rw-r--r--   0 root         (0) root         (0)     1384 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/exceptions/error_exception.py
--rw-r--r--   0 root         (0) root         (0)      905 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 17:33:23.000000 pagarme-python-5.7.2/pagarmecoreapi/models/
--rw-r--r--   0 root         (0) root         (0)     1941 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_anticipation_limits_response.py
--rw-r--r--   0 root         (0) root         (0)     1626 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_bank_transfer_payment_request.py
--rw-r--r--   0 root         (0) root         (0)     2742 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_voucher_payment_request.py
--rw-r--r--   0 root         (0) root         (0)     1639 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_cancel_subscription_request.py
--rw-r--r--   0 root         (0) root         (0)     1633 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_location_request.py
--rw-r--r--   0 root         (0) root         (0)     2095 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/list_withdrawals.py
--rw-r--r--   0 root         (0) root         (0)     1957 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_payment_authentication_request.py
--rw-r--r--   0 root         (0) root         (0)     1604 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/pix_additional_information.py
--rw-r--r--   0 root         (0) root         (0)     2109 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/list_customers_response.py
--rw-r--r--   0 root         (0) root         (0)     1403 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/update_invoice_status_request.py
--rw-r--r--   0 root         (0) root         (0)     3934 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_charge_request.py
--rw-r--r--   0 root         (0) root         (0)     1443 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_checkout_bank_transfer_payment_response.py
--rw-r--r--   0 root         (0) root         (0)     2748 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_card_payment_contactless_request.py
--rw-r--r--   0 root         (0) root         (0)     7653 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_checkout_payment_request.py
--rw-r--r--   0 root         (0) root         (0)     2243 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_price_bracket_response.py
--rw-r--r--   0 root         (0) root         (0)     4074 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_recipient_request.py
--rw-r--r--   0 root         (0) root         (0)     1415 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_charges_summary_response.py
--rw-r--r--   0 root         (0) root         (0)     3067 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_checkout_credit_card_payment_request.py
--rw-r--r--   0 root         (0) root         (0)     3986 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_bank_account_request.py
--rw-r--r--   0 root         (0) root         (0)     1655 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/update_current_cycle_end_date_request.py
--rw-r--r--   0 root         (0) root         (0)     1592 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_period_request.py
--rw-r--r--   0 root         (0) root         (0)     1411 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_device_request.py
--rw-r--r--   0 root         (0) root         (0)     2149 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/list_subscriptions_response.py
--rw-r--r--   0 root         (0) root         (0)     2443 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_antifraud_response.py
--rw-r--r--   0 root         (0) root         (0)     2125 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_checkout_debit_card_payment_response.py
--rw-r--r--   0 root         (0) root         (0)     2619 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_checkout_pix_payment_request.py
--rw-r--r--   0 root         (0) root         (0)     1935 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/update_subscription_split_request.py
--rw-r--r--   0 root         (0) root         (0)     3645 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_checkout_payment_settings_response.py
--rw-r--r--   0 root         (0) root         (0)     1526 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/update_subscription_due_days_request.py
--rw-r--r--   0 root         (0) root         (0)     1806 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_transaction_report_file_response.py
--rw-r--r--   0 root         (0) root         (0)     1921 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_subscription_split_response.py
--rw-r--r--   0 root         (0) root         (0)     4352 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_usage_response.py
--rw-r--r--   0 root         (0) root         (0)     5625 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_bank_account_response.py
--rw-r--r--   0 root         (0) root         (0)     5360 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_card_request.py
--rw-r--r--   0 root         (0) root         (0)     5390 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_customer_response.py
--rw-r--r--   0 root         (0) root         (0)     2400 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/update_recipient_request.py
--rw-r--r--   0 root         (0) root         (0)     4619 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_plan_item_response.py
--rw-r--r--   0 root         (0) root         (0)     2107 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/list_anticipation_response.py
--rw-r--r--   0 root         (0) root         (0)     2186 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/list_charge_transactions_response.py
--rw-r--r--   0 root         (0) root         (0)     1423 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/update_current_cycle_status_request.py
--rw-r--r--   0 root         (0) root         (0)     3489 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_invoice_item_response.py
--rw-r--r--   0 root         (0) root         (0)     2089 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/list_order_response.py
--rw-r--r--   0 root         (0) root         (0)     3763 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_customer_request.py
--rw-r--r--   0 root         (0) root         (0)     1425 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_device_response.py
--rw-r--r--   0 root         (0) root         (0)     4156 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_period_response.py
--rw-r--r--   0 root         (0) root         (0)     2185 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_pix_bank_account_response.py
--rw-r--r--   0 root         (0) root         (0)     2112 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/list_discounts_response.py
--rw-r--r--   0 root         (0) root         (0)     7165 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2445 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_order_item_response.py
--rw-r--r--   0 root         (0) root         (0)     2397 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/update_automatic_anticipation_settings_request.py
--rw-r--r--   0 root         (0) root         (0)     3168 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/update_card_request.py
--rw-r--r--   0 root         (0) root         (0)     1576 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_card_options_request.py
--rw-r--r--   0 root         (0) root         (0)     2116 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_transfer.py
--rw-r--r--   0 root         (0) root         (0)     1778 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_emv_data_tlv_decrypt_request.py
--rw-r--r--   0 root         (0) root         (0)     2382 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/update_charge_card_request.py
--rw-r--r--   0 root         (0) root         (0)     1662 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_checkout_card_installment_options_response.py
--rw-r--r--   0 root         (0) root         (0)     7387 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_order_response.py
--rw-r--r--   0 root         (0) root         (0)     1801 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/update_subscription_card_request.py
--rw-r--r--   0 root         (0) root         (0)     2077 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/list_plans_response.py
--rw-r--r--   0 root         (0) root         (0)     4382 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_private_label_payment_request.py
--rw-r--r--   0 root         (0) root         (0)     3443 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_billing_address_response.py
--rw-r--r--   0 root         (0) root         (0)     1451 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_clear_sale_request.py
--rw-r--r--   0 root         (0) root         (0)     3742 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/update_customer_request.py
--rw-r--r--   0 root         (0) root         (0)     3257 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_transfer_response.py
--rw-r--r--   0 root         (0) root         (0)     1658 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_transfer_target_response.py
--rw-r--r--   0 root         (0) root         (0)     2686 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_access_token_response.py
--rw-r--r--   0 root         (0) root         (0)     2104 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/list_invoices_response.py
--rw-r--r--   0 root         (0) root         (0)     2659 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_emv_decrypt_request.py
--rw-r--r--   0 root         (0) root         (0)     2812 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_split_response.py
--rw-r--r--   0 root         (0) root         (0)     2033 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_phones_request.py
--rw-r--r--   0 root         (0) root         (0)     3113 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_usages_details_response.py
--rw-r--r--   0 root         (0) root         (0)     7246 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_plan_response.py
--rw-r--r--   0 root         (0) root         (0)     2658 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_google_pay_request.py
--rw-r--r--   0 root         (0) root         (0)     3075 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/update_subscription_item_request.py
--rw-r--r--   0 root         (0) root         (0)     5413 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/update_charge_payment_method_request.py
--rw-r--r--   0 root         (0) root         (0)     1733 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_token_request.py
--rw-r--r--   0 root         (0) root         (0)     2875 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_pricing_scheme_response.py
--rw-r--r--   0 root         (0) root         (0)     2363 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_pix_payer_response.py
--rw-r--r--   0 root         (0) root         (0)     2334 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_gateway_recipient_response.py
--rw-r--r--   0 root         (0) root         (0)     1717 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_interest_response.py
--rw-r--r--   0 root         (0) root         (0)     2055 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/list_transfers.py
--rw-r--r--   0 root         (0) root         (0)     6618 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_order_request.py
--rw-r--r--   0 root         (0) root         (0)    94351 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_transaction_response.py
--rw-r--r--   0 root         (0) root         (0)     2902 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_cancel_charge_request.py
--rw-r--r--   0 root         (0) root         (0)     1650 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_location_response.py
--rw-r--r--   0 root         (0) root         (0)     3130 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_card_token_response.py
--rw-r--r--   0 root         (0) root         (0)     5304 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_boleto_payment_request.py
--rw-r--r--   0 root         (0) root         (0)     2151 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_checkout_debit_card_payment_request.py
--rw-r--r--   0 root         (0) root         (0)     4055 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_debit_card_payment_request.py
--rw-r--r--   0 root         (0) root         (0)     1401 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_gateway_error_response.py
--rw-r--r--   0 root         (0) root         (0)     2111 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/list_recipient_response.py
--rw-r--r--   0 root         (0) root         (0)    11778 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_subscription_request.py
--rw-r--r--   0 root         (0) root         (0)     2117 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_transfer_settings_request.py
--rw-r--r--   0 root         (0) root         (0)     2052 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/update_address_request.py
--rw-r--r--   0 root         (0) root         (0)     2096 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/list_transfer_response.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_withdraw_request.py
--rw-r--r--   0 root         (0) root         (0)     2780 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_balance_response.py
--rw-r--r--   0 root         (0) root         (0)     2112 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/update_transfer_settings_request.py
--rw-r--r--   0 root         (0) root         (0)     2049 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/list_usages_details_response.py
--rw-r--r--   0 root         (0) root         (0)     1894 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_checkout_boleto_payment_response.py
--rw-r--r--   0 root         (0) root         (0)     2129 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/update_order_item_request.py
--rw-r--r--   0 root         (0) root         (0)     2924 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_three_d_secure_request.py
--rw-r--r--   0 root         (0) root         (0)     6570 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_plan_request.py
--rw-r--r--   0 root         (0) root         (0)     1626 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/update_subscription_affiliation_id_request.py
--rw-r--r--   0 root         (0) root         (0)    11310 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_checkout_payment_response.py
--rw-r--r--   0 root         (0) root         (0)     2384 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_checkout_pix_payment_response.py
--rw-r--r--   0 root         (0) root         (0)     2262 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_order_item_request.py
--rw-r--r--   0 root         (0) root         (0)     1425 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/update_metadata_request.py
--rw-r--r--   0 root         (0) root         (0)     2120 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/list_increments_response.py
--rw-r--r--   0 root         (0) root         (0)     2174 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_price_bracket_request.py
--rw-r--r--   0 root         (0) root         (0)     5726 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_address_response.py
--rw-r--r--   0 root         (0) root         (0)     1834 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_cancel_charge_split_rules_request.py
--rw-r--r--   0 root         (0) root         (0)     4152 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_anticipation_response.py
--rw-r--r--   0 root         (0) root         (0)     2480 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/cancel_split_request.py
--rw-r--r--   0 root         (0) root         (0)     5102 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/update_plan_request.py
--rw-r--r--   0 root         (0) root         (0)     1685 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_anticipation_limit_response.py
--rw-r--r--   0 root         (0) root         (0)     1800 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/update_subscription_billing_date_request.py
--rw-r--r--   0 root         (0) root         (0)     1658 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_withdraw_target_response.py
--rw-r--r--   0 root         (0) root         (0)     2082 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_split_options_request.py
--rw-r--r--   0 root         (0) root         (0)     1408 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/update_order_status_request.py
--rw-r--r--   0 root         (0) root         (0)     2440 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_increment_request.py
--rw-r--r--   0 root         (0) root         (0)    11008 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_subscription_response.py
--rw-r--r--   0 root         (0) root         (0)     1461 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_access_token_request.py
--rw-r--r--   0 root         (0) root         (0)     2609 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_token_response.py
--rw-r--r--   0 root         (0) root         (0)     2140 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/list_transactions_response.py
--rw-r--r--   0 root         (0) root         (0)     5288 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_transfer.py
--rw-r--r--   0 root         (0) root         (0)     1953 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_gateway_response_response.py
--rw-r--r--   0 root         (0) root         (0)     2788 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/update_plan_item_request.py
--rw-r--r--   0 root         (0) root         (0)     2807 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_checkout_credit_card_payment_response.py
--rw-r--r--   0 root         (0) root         (0)     2226 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/list_transactions_files_response.py
--rw-r--r--   0 root         (0) root         (0)     2108 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/list_addresses_response.py
--rw-r--r--   0 root         (0) root         (0)     2054 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_checkout_boleto_payment_request.py
--rw-r--r--   0 root         (0) root         (0)     2074 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_setup_response.py
--rw-r--r--   0 root         (0) root         (0)     3668 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_address_request.py
--rw-r--r--   0 root         (0) root         (0)     3576 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_sub_merchant_request.py
--rw-r--r--   0 root         (0) root         (0)     2800 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_pricing_scheme_request.py
--rw-r--r--   0 root         (0) root         (0)     1708 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/update_subscription_start_at_request.py
--rw-r--r--   0 root         (0) root         (0)     1658 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_transfer_source_response.py
--rw-r--r--   0 root         (0) root         (0)     3872 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_subscription_item_request.py
--rw-r--r--   0 root         (0) root         (0)     1623 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_transfer_request.py
--rw-r--r--   0 root         (0) root         (0)     2342 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/update_subscription_payment_method_request.py
--rw-r--r--   0 root         (0) root         (0)     2758 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_plan_item_request.py
--rw-r--r--   0 root         (0) root         (0)     3911 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_shipping_response.py
--rw-r--r--   0 root         (0) root         (0)     1592 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_google_pay_header_request.py
--rw-r--r--   0 root         (0) root         (0)     2119 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_setup_request.py
--rw-r--r--   0 root         (0) root         (0)     2019 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_usage_report_response.py
--rw-r--r--   0 root         (0) root         (0)     2077 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/list_cards_response.py
--rw-r--r--   0 root         (0) root         (0)     4426 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_increment_response.py
--rw-r--r--   0 root         (0) root         (0)     2427 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_emv_data_decrypt_request.py
--rw-r--r--   0 root         (0) root         (0)     3115 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/update_seller_request.py
--rw-r--r--   0 root         (0) root         (0)     6274 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_card_response.py
--rw-r--r--   0 root         (0) root         (0)     2013 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_phones_response.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_anticipation_request.py
--rw-r--r--   0 root         (0) root         (0)     2108 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_split_options_response.py
--rw-r--r--   0 root         (0) root         (0)     2144 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/list_access_tokens_response.py
--rw-r--r--   0 root         (0) root         (0)     2101 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_transfer_settings_response.py
--rw-r--r--   0 root         (0) root         (0)     9005 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_invoice_response.py
--rw-r--r--   0 root         (0) root         (0)     2004 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/update_recipient_bank_account_request.py
--rw-r--r--   0 root         (0) root         (0)     2114 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/list_usages_response.py
--rw-r--r--   0 root         (0) root         (0)     2426 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_card_payment_contactless_poi_request.py
--rw-r--r--   0 root         (0) root         (0)     3727 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_seller_response.py
--rw-r--r--   0 root         (0) root         (0)     2423 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_discount_request.py
--rw-r--r--   0 root         (0) root         (0)     2736 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_usage_request.py
--rw-r--r--   0 root         (0) root         (0)     2648 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_apple_pay_request.py
--rw-r--r--   0 root         (0) root         (0)     6930 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_recipient_response.py
--rw-r--r--   0 root         (0) root         (0)     2504 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_split_request.py
--rw-r--r--   0 root         (0) root         (0)     1911 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_phone_response.py
--rw-r--r--   0 root         (0) root         (0)     2071 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_transaction_report_file_request.py
--rw-r--r--   0 root         (0) root         (0)     1706 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_fine_request.py
--rw-r--r--   0 root         (0) root         (0)     1701 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_fine_response.py
--rw-r--r--   0 root         (0) root         (0)     8022 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_payment_request.py
--rw-r--r--   0 root         (0) root         (0)     1424 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_invoice_request.py
--rw-r--r--   0 root         (0) root         (0)     5306 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_withdraw_response.py
--rw-r--r--   0 root         (0) root         (0)     2405 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_automatic_anticipation_settings_request.py
--rw-r--r--   0 root         (0) root         (0)     1614 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/update_charge_due_date_request.py
--rw-r--r--   0 root         (0) root         (0)     1410 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_emv_data_dukpt_decrypt_request.py
--rw-r--r--   0 root         (0) root         (0)     7964 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_charge_response.py
--rw-r--r--   0 root         (0) root         (0)     1648 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_checkout_card_installment_option_request.py
--rw-r--r--   0 root         (0) root         (0)     2790 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_sellers_request.py
--rw-r--r--   0 root         (0) root         (0)     2095 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/list_charges_response.py
--rw-r--r--   0 root         (0) root         (0)     1944 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_payment_authentication_response.py
--rw-r--r--   0 root         (0) root         (0)     1722 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_interest_request.py
--rw-r--r--   0 root         (0) root         (0)     2117 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/list_cycles_response.py
--rw-r--r--   0 root         (0) root         (0)     1646 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_checkout_bank_transfer_request.py
--rw-r--r--   0 root         (0) root         (0)     2196 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_apple_pay_header_request.py
--rw-r--r--   0 root         (0) root         (0)     2204 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/update_price_bracket_request.py
--rw-r--r--   0 root         (0) root         (0)     5870 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_subscription_item_response.py
--rw-r--r--   0 root         (0) root         (0)     1850 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_antifraud_request.py
--rw-r--r--   0 root         (0) root         (0)     2879 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_seller_request.py
--rw-r--r--   0 root         (0) root         (0)     2800 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/update_pricing_scheme_request.py
--rw-r--r--   0 root         (0) root         (0)     1795 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/paging_response.py
--rw-r--r--   0 root         (0) root         (0)     2181 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/list_subscription_items_response.py
--rw-r--r--   0 root         (0) root         (0)     1935 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_subscription_split_request.py
--rw-r--r--   0 root         (0) root         (0)     1917 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_phone_request.py
--rw-r--r--   0 root         (0) root         (0)     1733 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_cash_payment_request.py
--rw-r--r--   0 root         (0) root         (0)     2524 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_capture_charge_request.py
--rw-r--r--   0 root         (0) root         (0)     2665 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_pix_payment_request.py
--rw-r--r--   0 root         (0) root         (0)     1532 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/update_subscription_minimum_price_request.py
--rw-r--r--   0 root         (0) root         (0)     1834 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_confirm_payment_request.py
--rw-r--r--   0 root         (0) root         (0)     6465 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_credit_card_payment_request.py
--rw-r--r--   0 root         (0) root         (0)     2375 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_automatic_anticipation_response.py
--rw-r--r--   0 root         (0) root         (0)     2031 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/list_seller_response.py
--rw-r--r--   0 root         (0) root         (0)     2740 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_card_token_request.py
--rw-r--r--   0 root         (0) root         (0)     2365 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_three_d_secure_response.py
--rw-r--r--   0 root         (0) root         (0)     4127 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/create_shipping_request.py
--rw-r--r--   0 root         (0) root         (0)     4413 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_discount_response.py
--rw-r--r--   0 root         (0) root         (0)     1658 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/models/get_withdraw_source_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 17:33:23.000000 pagarme-python-5.7.2/pagarmecoreapi/controllers/
--rw-r--r--   0 root         (0) root         (0)    36176 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/controllers/charges_controller.py
--rw-r--r--   0 root         (0) root         (0)    55854 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/controllers/customers_controller.py
--rw-r--r--   0 root         (0) root         (0)     6055 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/controllers/tokens_controller.py
--rw-r--r--   0 root         (0) root         (0)     7154 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/controllers/transfers_controller.py
--rw-r--r--   0 root         (0) root         (0)      321 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    99671 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/controllers/subscriptions_controller.py
--rw-r--r--   0 root         (0) root         (0)    58037 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/controllers/recipients_controller.py
--rw-r--r--   0 root         (0) root         (0)     2962 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/controllers/transactions_controller.py
--rw-r--r--   0 root         (0) root         (0)    20247 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/controllers/invoices_controller.py
--rw-r--r--   0 root         (0) root         (0)    26708 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/controllers/plans_controller.py
--rw-r--r--   0 root         (0) root         (0)    26679 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/controllers/orders_controller.py
--rw-r--r--   0 root         (0) root         (0)     3335 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/controllers/base_controller.py
--rw-r--r--   0 root         (0) root         (0)    11888 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/controllers/sellers_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 17:33:23.000000 pagarme-python-5.7.2/pagarmecoreapi/http/
--rw-r--r--   0 root         (0) root         (0)     3557 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/http/requests_client.py
--rw-r--r--   0 root         (0) root         (0)      926 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/http/http_method_enum.py
--rw-r--r--   0 root         (0) root         (0)      181 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/http/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 17:33:23.000000 pagarme-python-5.7.2/pagarmecoreapi/http/auth/
--rw-r--r--   0 root         (0) root         (0)       31 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/http/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      847 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/http/auth/basic_auth.py
--rw-r--r--   0 root         (0) root         (0)     2832 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/http/http_request.py
--rw-r--r--   0 root         (0) root         (0)      967 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/http/http_context.py
--rw-r--r--   0 root         (0) root         (0)     7106 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/http/http_client.py
--rw-r--r--   0 root         (0) root         (0)     1121 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/http/http_call_back.py
--rw-r--r--   0 root         (0) root         (0)     1094 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/http/http_response.py
--rw-r--r--   0 root         (0) root         (0)      515 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/pagarmecoreapi/decorators.py
--rw-r--r--   0 root         (0) root         (0)   151640 2023-04-03 17:33:15.000000 pagarme-python-5.7.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 20:13:48.000000 pagarme-python-5.7.3/
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       36 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 20:13:48.000000 pagarme-python-5.7.3/tests/
+-rw-r--r--   0 root         (0) root         (0)      681 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/tests/http_response_catcher.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5125 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/tests/test_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 20:13:48.000000 pagarme-python-5.7.3/tests/controllers/
+-rw-r--r--   0 root         (0) root         (0)     1321 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/tests/controllers/test_plans_controller.py
+-rw-r--r--   0 root         (0) root         (0)     1718 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/tests/controllers/test_recipients_controller.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/tests/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      999 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/tests/controllers/controller_test_base.py
+-rw-r--r--   0 root         (0) root         (0)     1586 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/tests/controllers/test_subscriptions_controller.py
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/tests/controllers/test_transfers_controller.py
+-rw-r--r--   0 root         (0) root         (0)     1513 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/tests/controllers/test_invoices_controller.py
+-rw-r--r--   0 root         (0) root         (0)     1266 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/tests/controllers/test_customers_controller.py
+-rw-r--r--   0 root         (0) root         (0)     1325 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/tests/controllers/test_orders_controller.py
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/tests/controllers/test_charges_controller.py
+-rw-r--r--   0 root         (0) root         (0)      244 2023-05-15 20:13:48.000000 pagarme-python-5.7.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      872 2023-05-15 20:13:47.000000 pagarme-python-5.7.3/setup.py
+-rw-r--r--   0 root         (0) root         (0)       59 2023-05-15 20:13:48.000000 pagarme-python-5.7.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 20:13:48.000000 pagarme-python-5.7.3/pagarme_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      244 2023-05-15 20:13:48.000000 pagarme-python-5.7.3/pagarme_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12967 2023-05-15 20:13:48.000000 pagarme-python-5.7.3/pagarme_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 20:13:48.000000 pagarme-python-5.7.3/pagarme_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-15 20:13:48.000000 pagarme-python-5.7.3/pagarme_python.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-05-15 20:13:48.000000 pagarme-python-5.7.3/pagarme_python.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 20:13:48.000000 pagarme-python-5.7.3/pagarmecoreapi/
+-rw-r--r--   0 root         (0) root         (0)    13744 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/api_helper.py
+-rw-r--r--   0 root         (0) root         (0)     2327 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/pagarmecoreapi_client.py
+-rw-r--r--   0 root         (0) root         (0)      169 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 20:13:48.000000 pagarme-python-5.7.3/pagarmecoreapi/exceptions/
+-rw-r--r--   0 root         (0) root         (0)       58 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      906 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/exceptions/api_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1384 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/exceptions/error_exception.py
+-rw-r--r--   0 root         (0) root         (0)      905 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 20:13:48.000000 pagarme-python-5.7.3/pagarmecoreapi/models/
+-rw-r--r--   0 root         (0) root         (0)     1941 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_anticipation_limits_response.py
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_bank_transfer_payment_request.py
+-rw-r--r--   0 root         (0) root         (0)     3105 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_voucher_payment_request.py
+-rw-r--r--   0 root         (0) root         (0)     1639 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_cancel_subscription_request.py
+-rw-r--r--   0 root         (0) root         (0)     1633 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_location_request.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/list_withdrawals.py
+-rw-r--r--   0 root         (0) root         (0)     1957 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_payment_authentication_request.py
+-rw-r--r--   0 root         (0) root         (0)     1604 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/pix_additional_information.py
+-rw-r--r--   0 root         (0) root         (0)     2109 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/list_customers_response.py
+-rw-r--r--   0 root         (0) root         (0)     1403 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/update_invoice_status_request.py
+-rw-r--r--   0 root         (0) root         (0)     3934 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_charge_request.py
+-rw-r--r--   0 root         (0) root         (0)     1443 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_checkout_bank_transfer_payment_response.py
+-rw-r--r--   0 root         (0) root         (0)     2748 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_card_payment_contactless_request.py
+-rw-r--r--   0 root         (0) root         (0)     7653 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_checkout_payment_request.py
+-rw-r--r--   0 root         (0) root         (0)     2243 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_price_bracket_response.py
+-rw-r--r--   0 root         (0) root         (0)     4074 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_recipient_request.py
+-rw-r--r--   0 root         (0) root         (0)     1415 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_charges_summary_response.py
+-rw-r--r--   0 root         (0) root         (0)     3067 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_checkout_credit_card_payment_request.py
+-rw-r--r--   0 root         (0) root         (0)     3986 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_bank_account_request.py
+-rw-r--r--   0 root         (0) root         (0)     1655 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/update_current_cycle_end_date_request.py
+-rw-r--r--   0 root         (0) root         (0)     1592 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_period_request.py
+-rw-r--r--   0 root         (0) root         (0)     1411 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_device_request.py
+-rw-r--r--   0 root         (0) root         (0)     2149 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/list_subscriptions_response.py
+-rw-r--r--   0 root         (0) root         (0)     2443 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_antifraud_response.py
+-rw-r--r--   0 root         (0) root         (0)     2125 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_checkout_debit_card_payment_response.py
+-rw-r--r--   0 root         (0) root         (0)     2619 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_checkout_pix_payment_request.py
+-rw-r--r--   0 root         (0) root         (0)     1935 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/update_subscription_split_request.py
+-rw-r--r--   0 root         (0) root         (0)     3645 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_checkout_payment_settings_response.py
+-rw-r--r--   0 root         (0) root         (0)     1526 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/update_subscription_due_days_request.py
+-rw-r--r--   0 root         (0) root         (0)     1806 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_transaction_report_file_response.py
+-rw-r--r--   0 root         (0) root         (0)     1921 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_subscription_split_response.py
+-rw-r--r--   0 root         (0) root         (0)     4352 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_usage_response.py
+-rw-r--r--   0 root         (0) root         (0)     5625 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_bank_account_response.py
+-rw-r--r--   0 root         (0) root         (0)     5360 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_card_request.py
+-rw-r--r--   0 root         (0) root         (0)     5390 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_customer_response.py
+-rw-r--r--   0 root         (0) root         (0)     2400 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/update_recipient_request.py
+-rw-r--r--   0 root         (0) root         (0)     4619 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_plan_item_response.py
+-rw-r--r--   0 root         (0) root         (0)     2107 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/list_anticipation_response.py
+-rw-r--r--   0 root         (0) root         (0)     2186 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/list_charge_transactions_response.py
+-rw-r--r--   0 root         (0) root         (0)     1423 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/update_current_cycle_status_request.py
+-rw-r--r--   0 root         (0) root         (0)     3489 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_invoice_item_response.py
+-rw-r--r--   0 root         (0) root         (0)     2089 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/list_order_response.py
+-rw-r--r--   0 root         (0) root         (0)     3763 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_customer_request.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_device_response.py
+-rw-r--r--   0 root         (0) root         (0)     4156 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_period_response.py
+-rw-r--r--   0 root         (0) root         (0)     2185 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_pix_bank_account_response.py
+-rw-r--r--   0 root         (0) root         (0)     2112 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/list_discounts_response.py
+-rw-r--r--   0 root         (0) root         (0)     7165 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2445 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_order_item_response.py
+-rw-r--r--   0 root         (0) root         (0)     2397 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/update_automatic_anticipation_settings_request.py
+-rw-r--r--   0 root         (0) root         (0)     3168 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/update_card_request.py
+-rw-r--r--   0 root         (0) root         (0)     1576 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_card_options_request.py
+-rw-r--r--   0 root         (0) root         (0)     2116 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_transfer.py
+-rw-r--r--   0 root         (0) root         (0)     1778 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_emv_data_tlv_decrypt_request.py
+-rw-r--r--   0 root         (0) root         (0)     2382 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/update_charge_card_request.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_checkout_card_installment_options_response.py
+-rw-r--r--   0 root         (0) root         (0)     7387 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_order_response.py
+-rw-r--r--   0 root         (0) root         (0)     1801 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/update_subscription_card_request.py
+-rw-r--r--   0 root         (0) root         (0)     2077 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/list_plans_response.py
+-rw-r--r--   0 root         (0) root         (0)     4382 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_private_label_payment_request.py
+-rw-r--r--   0 root         (0) root         (0)     3443 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_billing_address_response.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_clear_sale_request.py
+-rw-r--r--   0 root         (0) root         (0)     3742 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/update_customer_request.py
+-rw-r--r--   0 root         (0) root         (0)     3257 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_transfer_response.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_transfer_target_response.py
+-rw-r--r--   0 root         (0) root         (0)     2686 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_access_token_response.py
+-rw-r--r--   0 root         (0) root         (0)     2104 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/list_invoices_response.py
+-rw-r--r--   0 root         (0) root         (0)     2659 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_emv_decrypt_request.py
+-rw-r--r--   0 root         (0) root         (0)     2812 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_split_response.py
+-rw-r--r--   0 root         (0) root         (0)     2033 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_phones_request.py
+-rw-r--r--   0 root         (0) root         (0)     3113 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_usages_details_response.py
+-rw-r--r--   0 root         (0) root         (0)     7246 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_plan_response.py
+-rw-r--r--   0 root         (0) root         (0)     2658 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_google_pay_request.py
+-rw-r--r--   0 root         (0) root         (0)     3075 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/update_subscription_item_request.py
+-rw-r--r--   0 root         (0) root         (0)     5413 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/update_charge_payment_method_request.py
+-rw-r--r--   0 root         (0) root         (0)     1733 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_token_request.py
+-rw-r--r--   0 root         (0) root         (0)     2875 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_pricing_scheme_response.py
+-rw-r--r--   0 root         (0) root         (0)     2363 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_pix_payer_response.py
+-rw-r--r--   0 root         (0) root         (0)     2334 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_gateway_recipient_response.py
+-rw-r--r--   0 root         (0) root         (0)     1717 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_interest_response.py
+-rw-r--r--   0 root         (0) root         (0)     2055 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/list_transfers.py
+-rw-r--r--   0 root         (0) root         (0)     6618 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_order_request.py
+-rw-r--r--   0 root         (0) root         (0)    94351 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_transaction_response.py
+-rw-r--r--   0 root         (0) root         (0)     2902 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_cancel_charge_request.py
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_location_response.py
+-rw-r--r--   0 root         (0) root         (0)     3130 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_card_token_response.py
+-rw-r--r--   0 root         (0) root         (0)     5304 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_boleto_payment_request.py
+-rw-r--r--   0 root         (0) root         (0)     2151 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_checkout_debit_card_payment_request.py
+-rw-r--r--   0 root         (0) root         (0)     4055 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_debit_card_payment_request.py
+-rw-r--r--   0 root         (0) root         (0)     1401 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_gateway_error_response.py
+-rw-r--r--   0 root         (0) root         (0)     2111 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/list_recipient_response.py
+-rw-r--r--   0 root         (0) root         (0)    11778 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_subscription_request.py
+-rw-r--r--   0 root         (0) root         (0)     2117 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_transfer_settings_request.py
+-rw-r--r--   0 root         (0) root         (0)     2052 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/update_address_request.py
+-rw-r--r--   0 root         (0) root         (0)     2096 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/list_transfer_response.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_withdraw_request.py
+-rw-r--r--   0 root         (0) root         (0)     2780 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_balance_response.py
+-rw-r--r--   0 root         (0) root         (0)     2112 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/update_transfer_settings_request.py
+-rw-r--r--   0 root         (0) root         (0)     2049 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/list_usages_details_response.py
+-rw-r--r--   0 root         (0) root         (0)     1894 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_checkout_boleto_payment_response.py
+-rw-r--r--   0 root         (0) root         (0)     2129 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/update_order_item_request.py
+-rw-r--r--   0 root         (0) root         (0)     2924 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_three_d_secure_request.py
+-rw-r--r--   0 root         (0) root         (0)     6570 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_plan_request.py
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/update_subscription_affiliation_id_request.py
+-rw-r--r--   0 root         (0) root         (0)    11310 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_checkout_payment_response.py
+-rw-r--r--   0 root         (0) root         (0)     2384 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_checkout_pix_payment_response.py
+-rw-r--r--   0 root         (0) root         (0)     2262 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_order_item_request.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/update_metadata_request.py
+-rw-r--r--   0 root         (0) root         (0)     2120 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/list_increments_response.py
+-rw-r--r--   0 root         (0) root         (0)     2174 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_price_bracket_request.py
+-rw-r--r--   0 root         (0) root         (0)     5726 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_address_response.py
+-rw-r--r--   0 root         (0) root         (0)     1834 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_cancel_charge_split_rules_request.py
+-rw-r--r--   0 root         (0) root         (0)     4152 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_anticipation_response.py
+-rw-r--r--   0 root         (0) root         (0)     2480 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/cancel_split_request.py
+-rw-r--r--   0 root         (0) root         (0)     5102 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/update_plan_request.py
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_anticipation_limit_response.py
+-rw-r--r--   0 root         (0) root         (0)     1800 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/update_subscription_billing_date_request.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_withdraw_target_response.py
+-rw-r--r--   0 root         (0) root         (0)     2082 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_split_options_request.py
+-rw-r--r--   0 root         (0) root         (0)     1408 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/update_order_status_request.py
+-rw-r--r--   0 root         (0) root         (0)     2440 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_increment_request.py
+-rw-r--r--   0 root         (0) root         (0)    11008 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_subscription_response.py
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_access_token_request.py
+-rw-r--r--   0 root         (0) root         (0)     2609 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_token_response.py
+-rw-r--r--   0 root         (0) root         (0)     2140 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/list_transactions_response.py
+-rw-r--r--   0 root         (0) root         (0)     5288 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_transfer.py
+-rw-r--r--   0 root         (0) root         (0)     1953 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_gateway_response_response.py
+-rw-r--r--   0 root         (0) root         (0)     2788 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/update_plan_item_request.py
+-rw-r--r--   0 root         (0) root         (0)     2807 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_checkout_credit_card_payment_response.py
+-rw-r--r--   0 root         (0) root         (0)     2226 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/list_transactions_files_response.py
+-rw-r--r--   0 root         (0) root         (0)     2108 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/list_addresses_response.py
+-rw-r--r--   0 root         (0) root         (0)     2054 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_checkout_boleto_payment_request.py
+-rw-r--r--   0 root         (0) root         (0)     2074 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_setup_response.py
+-rw-r--r--   0 root         (0) root         (0)     3668 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_address_request.py
+-rw-r--r--   0 root         (0) root         (0)     3576 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_sub_merchant_request.py
+-rw-r--r--   0 root         (0) root         (0)     2800 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_pricing_scheme_request.py
+-rw-r--r--   0 root         (0) root         (0)     1708 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/update_subscription_start_at_request.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_transfer_source_response.py
+-rw-r--r--   0 root         (0) root         (0)     3872 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_subscription_item_request.py
+-rw-r--r--   0 root         (0) root         (0)     1623 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_transfer_request.py
+-rw-r--r--   0 root         (0) root         (0)     2342 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/update_subscription_payment_method_request.py
+-rw-r--r--   0 root         (0) root         (0)     2758 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_plan_item_request.py
+-rw-r--r--   0 root         (0) root         (0)     3911 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_shipping_response.py
+-rw-r--r--   0 root         (0) root         (0)     1592 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_google_pay_header_request.py
+-rw-r--r--   0 root         (0) root         (0)     2119 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_setup_request.py
+-rw-r--r--   0 root         (0) root         (0)     2019 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_usage_report_response.py
+-rw-r--r--   0 root         (0) root         (0)     2077 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/list_cards_response.py
+-rw-r--r--   0 root         (0) root         (0)     4426 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_increment_response.py
+-rw-r--r--   0 root         (0) root         (0)     2427 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_emv_data_decrypt_request.py
+-rw-r--r--   0 root         (0) root         (0)     3115 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/update_seller_request.py
+-rw-r--r--   0 root         (0) root         (0)     6274 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_card_response.py
+-rw-r--r--   0 root         (0) root         (0)     2013 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_phones_response.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_anticipation_request.py
+-rw-r--r--   0 root         (0) root         (0)     2108 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_split_options_response.py
+-rw-r--r--   0 root         (0) root         (0)     2144 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/list_access_tokens_response.py
+-rw-r--r--   0 root         (0) root         (0)     2101 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_transfer_settings_response.py
+-rw-r--r--   0 root         (0) root         (0)     9005 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_invoice_response.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/update_recipient_bank_account_request.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/list_usages_response.py
+-rw-r--r--   0 root         (0) root         (0)     2426 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_card_payment_contactless_poi_request.py
+-rw-r--r--   0 root         (0) root         (0)     3727 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_seller_response.py
+-rw-r--r--   0 root         (0) root         (0)     2423 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_discount_request.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_usage_request.py
+-rw-r--r--   0 root         (0) root         (0)     2648 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_apple_pay_request.py
+-rw-r--r--   0 root         (0) root         (0)     6930 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_recipient_response.py
+-rw-r--r--   0 root         (0) root         (0)     2504 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_split_request.py
+-rw-r--r--   0 root         (0) root         (0)     1911 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_phone_response.py
+-rw-r--r--   0 root         (0) root         (0)     2071 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_transaction_report_file_request.py
+-rw-r--r--   0 root         (0) root         (0)     1706 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_fine_request.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_fine_response.py
+-rw-r--r--   0 root         (0) root         (0)     8022 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_payment_request.py
+-rw-r--r--   0 root         (0) root         (0)     1424 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_invoice_request.py
+-rw-r--r--   0 root         (0) root         (0)     5306 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_withdraw_response.py
+-rw-r--r--   0 root         (0) root         (0)     2405 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_automatic_anticipation_settings_request.py
+-rw-r--r--   0 root         (0) root         (0)     1614 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/update_charge_due_date_request.py
+-rw-r--r--   0 root         (0) root         (0)     1410 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_emv_data_dukpt_decrypt_request.py
+-rw-r--r--   0 root         (0) root         (0)     7964 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_charge_response.py
+-rw-r--r--   0 root         (0) root         (0)     1648 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_checkout_card_installment_option_request.py
+-rw-r--r--   0 root         (0) root         (0)     2790 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_sellers_request.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/list_charges_response.py
+-rw-r--r--   0 root         (0) root         (0)     1944 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_payment_authentication_response.py
+-rw-r--r--   0 root         (0) root         (0)     1722 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_interest_request.py
+-rw-r--r--   0 root         (0) root         (0)     2117 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/list_cycles_response.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_checkout_bank_transfer_request.py
+-rw-r--r--   0 root         (0) root         (0)     2196 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_apple_pay_header_request.py
+-rw-r--r--   0 root         (0) root         (0)     2204 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/update_price_bracket_request.py
+-rw-r--r--   0 root         (0) root         (0)     5870 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_subscription_item_response.py
+-rw-r--r--   0 root         (0) root         (0)     1850 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_antifraud_request.py
+-rw-r--r--   0 root         (0) root         (0)     2879 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_seller_request.py
+-rw-r--r--   0 root         (0) root         (0)     2800 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/update_pricing_scheme_request.py
+-rw-r--r--   0 root         (0) root         (0)     1795 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/paging_response.py
+-rw-r--r--   0 root         (0) root         (0)     2181 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/list_subscription_items_response.py
+-rw-r--r--   0 root         (0) root         (0)     1935 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_subscription_split_request.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_phone_request.py
+-rw-r--r--   0 root         (0) root         (0)     1733 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_cash_payment_request.py
+-rw-r--r--   0 root         (0) root         (0)     2524 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_capture_charge_request.py
+-rw-r--r--   0 root         (0) root         (0)     2665 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_pix_payment_request.py
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/update_subscription_minimum_price_request.py
+-rw-r--r--   0 root         (0) root         (0)     1834 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_confirm_payment_request.py
+-rw-r--r--   0 root         (0) root         (0)     6465 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_credit_card_payment_request.py
+-rw-r--r--   0 root         (0) root         (0)     2375 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_automatic_anticipation_response.py
+-rw-r--r--   0 root         (0) root         (0)     2031 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/list_seller_response.py
+-rw-r--r--   0 root         (0) root         (0)     2740 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_card_token_request.py
+-rw-r--r--   0 root         (0) root         (0)     2365 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_three_d_secure_response.py
+-rw-r--r--   0 root         (0) root         (0)     4127 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/create_shipping_request.py
+-rw-r--r--   0 root         (0) root         (0)     4413 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_discount_response.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/models/get_withdraw_source_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 20:13:48.000000 pagarme-python-5.7.3/pagarmecoreapi/controllers/
+-rw-r--r--   0 root         (0) root         (0)    36176 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/controllers/charges_controller.py
+-rw-r--r--   0 root         (0) root         (0)    55854 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/controllers/customers_controller.py
+-rw-r--r--   0 root         (0) root         (0)     6055 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/controllers/tokens_controller.py
+-rw-r--r--   0 root         (0) root         (0)     7154 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/controllers/transfers_controller.py
+-rw-r--r--   0 root         (0) root         (0)      321 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    99671 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/controllers/subscriptions_controller.py
+-rw-r--r--   0 root         (0) root         (0)    58037 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/controllers/recipients_controller.py
+-rw-r--r--   0 root         (0) root         (0)     2962 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/controllers/transactions_controller.py
+-rw-r--r--   0 root         (0) root         (0)    20247 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/controllers/invoices_controller.py
+-rw-r--r--   0 root         (0) root         (0)    26708 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/controllers/plans_controller.py
+-rw-r--r--   0 root         (0) root         (0)    26679 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/controllers/orders_controller.py
+-rw-r--r--   0 root         (0) root         (0)     3335 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/controllers/base_controller.py
+-rw-r--r--   0 root         (0) root         (0)    11888 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/controllers/sellers_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 20:13:48.000000 pagarme-python-5.7.3/pagarmecoreapi/http/
+-rw-r--r--   0 root         (0) root         (0)     3557 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/http/requests_client.py
+-rw-r--r--   0 root         (0) root         (0)      926 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/http/http_method_enum.py
+-rw-r--r--   0 root         (0) root         (0)      181 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/http/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 20:13:48.000000 pagarme-python-5.7.3/pagarmecoreapi/http/auth/
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/http/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      847 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/http/auth/basic_auth.py
+-rw-r--r--   0 root         (0) root         (0)     2832 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/http/http_request.py
+-rw-r--r--   0 root         (0) root         (0)      967 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/http/http_context.py
+-rw-r--r--   0 root         (0) root         (0)     7106 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/http/http_client.py
+-rw-r--r--   0 root         (0) root         (0)     1121 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/http/http_call_back.py
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/http/http_response.py
+-rw-r--r--   0 root         (0) root         (0)      515 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/pagarmecoreapi/decorators.py
+-rw-r--r--   0 root         (0) root         (0)   151618 2023-05-15 20:13:43.000000 pagarme-python-5.7.3/README.md
```

### Comparing `pagarme-python-5.7.2/LICENSE` & `pagarme-python-5.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/tests/http_response_catcher.py` & `pagarme-python-5.7.3/tests/http_response_catcher.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/tests/test_helper.py` & `pagarme-python-5.7.3/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/tests/controllers/test_plans_controller.py` & `pagarme-python-5.7.3/tests/controllers/test_plans_controller.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/tests/controllers/test_recipients_controller.py` & `pagarme-python-5.7.3/tests/controllers/test_recipients_controller.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/tests/controllers/controller_test_base.py` & `pagarme-python-5.7.3/tests/controllers/controller_test_base.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/tests/controllers/test_subscriptions_controller.py` & `pagarme-python-5.7.3/tests/controllers/test_subscriptions_controller.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/tests/controllers/test_transfers_controller.py` & `pagarme-python-5.7.3/tests/controllers/test_transfers_controller.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/tests/controllers/test_invoices_controller.py` & `pagarme-python-5.7.3/tests/controllers/test_invoices_controller.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/tests/controllers/test_customers_controller.py` & `pagarme-python-5.7.3/tests/controllers/test_customers_controller.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/tests/controllers/test_orders_controller.py` & `pagarme-python-5.7.3/tests/controllers/test_orders_controller.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/tests/controllers/test_charges_controller.py` & `pagarme-python-5.7.3/tests/controllers/test_charges_controller.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/setup.py` & `pagarme-python-5.7.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         long_description = fh.read()
 else:
     with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
 
 setup(
     name='pagarme-python',
-    version='5.7.2',
+    version='5.7.3',
     description='Pagarme API',
      
     long_description_content_type="text/markdown",
      author='Pagarme',
     author_email='support@pagar.me',
     url='https://github.com/pagarme/pagarme-core-api-python',
     packages=find_packages(),
```

### Comparing `pagarme-python-5.7.2/pagarme_python.egg-info/SOURCES.txt` & `pagarme-python-5.7.3/pagarme_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/api_helper.py` & `pagarme-python-5.7.3/pagarmecoreapi/api_helper.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/pagarmecoreapi_client.py` & `pagarme-python-5.7.3/pagarmecoreapi/pagarmecoreapi_client.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/exceptions/api_exception.py` & `pagarme-python-5.7.3/pagarmecoreapi/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/exceptions/error_exception.py` & `pagarme-python-5.7.3/pagarmecoreapi/exceptions/error_exception.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/configuration.py` & `pagarme-python-5.7.3/pagarmecoreapi/configuration.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_anticipation_limits_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_anticipation_limits_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_bank_transfer_payment_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_bank_transfer_payment_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_voucher_payment_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_voucher_payment_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,40 +18,44 @@
         statement_descriptor (string): The text that will be shown on the
             voucher's statement
         card_id (string): Card id
         card_token (string): Card token
         card (CreateCardRequest): Card data
         recurrency_cycle (string): Defines whether the card has been used one
             or more times.
+        merchant_category_code (long|int): Customer business segment code
 
     """
 
     # Create a mapping from Model property names to API property names
     _names = {
         "statement_descriptor":'statement_descriptor',
         "card_id":'card_id',
         "card_token":'card_token',
         "card":'Card',
-        "recurrency_cycle":'recurrency_cycle'
+        "recurrency_cycle":'recurrency_cycle',
+        "merchant_category_code":'merchant_category_code'
     }
 
     def __init__(self,
                  statement_descriptor=None,
                  card_id=None,
                  card_token=None,
                  card=None,
-                 recurrency_cycle=None):
+                 recurrency_cycle=None,
+                 merchant_category_code=None):
         """Constructor for the CreateVoucherPaymentRequest class"""
 
         # Initialize members of the class
         self.statement_descriptor = statement_descriptor
         self.card_id = card_id
         self.card_token = card_token
         self.card = card
         self.recurrency_cycle = recurrency_cycle
+        self.merchant_category_code = merchant_category_code
 
 
     @classmethod
     def from_dictionary(cls,
                         dictionary):
         """Creates an instance of this model from a dictionary
 
@@ -69,16 +73,18 @@
 
         # Extract variables from the dictionary
         statement_descriptor = dictionary.get('statement_descriptor')
         card_id = dictionary.get('card_id')
         card_token = dictionary.get('card_token')
         card = pagarmecoreapi.models.create_card_request.CreateCardRequest.from_dictionary(dictionary.get('Card')) if dictionary.get('Card') else None
         recurrency_cycle = dictionary.get('recurrency_cycle')
+        merchant_category_code = dictionary.get('merchant_category_code')
 
         # Return an object of this model
         return cls(statement_descriptor,
                    card_id,
                    card_token,
                    card,
-                   recurrency_cycle)
+                   recurrency_cycle,
+                   merchant_category_code)
```

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_cancel_subscription_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_cancel_subscription_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_location_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_location_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/list_withdrawals.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/list_withdrawals.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_payment_authentication_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_payment_authentication_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/pix_additional_information.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/pix_additional_information.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/list_customers_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/list_customers_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/update_invoice_status_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/update_invoice_status_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_charge_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_charge_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_checkout_bank_transfer_payment_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_checkout_bank_transfer_payment_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_card_payment_contactless_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_card_payment_contactless_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_checkout_payment_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_checkout_payment_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_price_bracket_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_price_bracket_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_recipient_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_recipient_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_charges_summary_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_charges_summary_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_checkout_credit_card_payment_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_checkout_credit_card_payment_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_bank_account_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_bank_account_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/update_current_cycle_end_date_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/update_current_cycle_end_date_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_period_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_period_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_device_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_device_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/list_subscriptions_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/list_subscriptions_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_antifraud_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_antifraud_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_checkout_debit_card_payment_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_checkout_debit_card_payment_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_checkout_pix_payment_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_checkout_pix_payment_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/update_subscription_split_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/update_subscription_split_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_checkout_payment_settings_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_checkout_payment_settings_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/update_subscription_due_days_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/update_subscription_due_days_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_transaction_report_file_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_transaction_report_file_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_subscription_split_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_subscription_split_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_usage_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_usage_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_bank_account_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_bank_account_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_card_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_card_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_customer_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_customer_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/update_recipient_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/update_recipient_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_plan_item_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_plan_item_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/list_anticipation_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/list_anticipation_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/list_charge_transactions_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/list_charge_transactions_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/update_current_cycle_status_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/update_current_cycle_status_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_invoice_item_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_invoice_item_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/list_order_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/list_order_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_customer_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_customer_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_device_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_device_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_period_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_period_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_pix_bank_account_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_pix_bank_account_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/list_discounts_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/list_discounts_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/__init__.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_order_item_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_order_item_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/update_automatic_anticipation_settings_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/update_automatic_anticipation_settings_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/update_card_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/update_card_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_card_options_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_card_options_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_transfer.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_transfer.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_emv_data_tlv_decrypt_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_emv_data_tlv_decrypt_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/update_charge_card_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/update_charge_card_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_checkout_card_installment_options_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_checkout_card_installment_options_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_order_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_order_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/update_subscription_card_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/update_subscription_card_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/list_plans_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/list_plans_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_private_label_payment_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_private_label_payment_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_billing_address_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_billing_address_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_clear_sale_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_clear_sale_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/update_customer_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/update_customer_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_transfer_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_transfer_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_transfer_target_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_transfer_target_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_access_token_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_access_token_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/list_invoices_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/list_invoices_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_emv_decrypt_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_emv_decrypt_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_split_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_split_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_phones_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_phones_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_usages_details_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_usages_details_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_plan_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_plan_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_google_pay_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_google_pay_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/update_subscription_item_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/update_subscription_item_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/update_charge_payment_method_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/update_charge_payment_method_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_token_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_token_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_pricing_scheme_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_pricing_scheme_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_pix_payer_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_pix_payer_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_gateway_recipient_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_gateway_recipient_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_interest_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_interest_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/list_transfers.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/list_transfers.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_order_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_order_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_transaction_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_transaction_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_cancel_charge_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_cancel_charge_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_location_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_location_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_card_token_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_card_token_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_boleto_payment_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_boleto_payment_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_checkout_debit_card_payment_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_checkout_debit_card_payment_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_debit_card_payment_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_debit_card_payment_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_gateway_error_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_gateway_error_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/list_recipient_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/list_recipient_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_subscription_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_subscription_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_transfer_settings_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_transfer_settings_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/update_address_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/update_address_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/list_transfer_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/list_transfer_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_withdraw_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_withdraw_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_balance_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_balance_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/update_transfer_settings_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/update_transfer_settings_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/list_usages_details_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/list_usages_details_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_checkout_boleto_payment_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_checkout_boleto_payment_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/update_order_item_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/update_order_item_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_three_d_secure_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_three_d_secure_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_plan_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_plan_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/update_subscription_affiliation_id_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/update_subscription_affiliation_id_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_checkout_payment_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_checkout_payment_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_checkout_pix_payment_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_checkout_pix_payment_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_order_item_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_order_item_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/update_metadata_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/update_metadata_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/list_increments_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/list_increments_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_price_bracket_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_price_bracket_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_address_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_address_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_cancel_charge_split_rules_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_cancel_charge_split_rules_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_anticipation_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_anticipation_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/cancel_split_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/cancel_split_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/update_plan_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/update_plan_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_anticipation_limit_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_anticipation_limit_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/update_subscription_billing_date_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/update_subscription_billing_date_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_withdraw_target_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_withdraw_target_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_split_options_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_split_options_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/update_order_status_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/update_order_status_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_increment_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_increment_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_subscription_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_subscription_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_access_token_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_access_token_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_token_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_token_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/list_transactions_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/list_transactions_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_transfer.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_transfer.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_gateway_response_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_gateway_response_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/update_plan_item_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/update_plan_item_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_checkout_credit_card_payment_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_checkout_credit_card_payment_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/list_transactions_files_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/list_transactions_files_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/list_addresses_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/list_addresses_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_checkout_boleto_payment_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_checkout_boleto_payment_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_setup_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_setup_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_address_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_address_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_sub_merchant_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_sub_merchant_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_pricing_scheme_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_pricing_scheme_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/update_subscription_start_at_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/update_subscription_start_at_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_transfer_source_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_transfer_source_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_subscription_item_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_subscription_item_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_transfer_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_transfer_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/update_subscription_payment_method_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/update_subscription_payment_method_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_plan_item_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_plan_item_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_shipping_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_shipping_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_google_pay_header_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_google_pay_header_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_setup_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_setup_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_usage_report_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_usage_report_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/list_cards_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/list_cards_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_increment_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_increment_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_emv_data_decrypt_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_emv_data_decrypt_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/update_seller_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/update_seller_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_card_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_card_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_phones_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_phones_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_anticipation_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_anticipation_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_split_options_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_split_options_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/list_access_tokens_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/list_access_tokens_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_transfer_settings_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_transfer_settings_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_invoice_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_invoice_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/update_recipient_bank_account_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/update_recipient_bank_account_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/list_usages_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/list_usages_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_card_payment_contactless_poi_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_card_payment_contactless_poi_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_seller_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_seller_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_discount_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_discount_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_usage_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_usage_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_apple_pay_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_apple_pay_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_recipient_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_recipient_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_split_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_split_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_phone_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_phone_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_transaction_report_file_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_transaction_report_file_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_fine_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_fine_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_fine_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_fine_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_payment_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_payment_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_invoice_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_invoice_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_withdraw_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_withdraw_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_automatic_anticipation_settings_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_automatic_anticipation_settings_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/update_charge_due_date_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/update_charge_due_date_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_emv_data_dukpt_decrypt_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_emv_data_dukpt_decrypt_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_charge_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_charge_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_checkout_card_installment_option_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_checkout_card_installment_option_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_sellers_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_sellers_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/list_charges_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/list_charges_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_payment_authentication_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_payment_authentication_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_interest_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_interest_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/list_cycles_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/list_cycles_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_checkout_bank_transfer_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_checkout_bank_transfer_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_apple_pay_header_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_apple_pay_header_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/update_price_bracket_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/update_price_bracket_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_subscription_item_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_subscription_item_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_antifraud_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_antifraud_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_seller_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_seller_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/update_pricing_scheme_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/update_pricing_scheme_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/paging_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/paging_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/list_subscription_items_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/list_subscription_items_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_subscription_split_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_subscription_split_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_phone_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_phone_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_cash_payment_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_cash_payment_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_capture_charge_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_capture_charge_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_pix_payment_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_pix_payment_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/update_subscription_minimum_price_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/update_subscription_minimum_price_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_confirm_payment_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_confirm_payment_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_credit_card_payment_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_credit_card_payment_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_automatic_anticipation_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_automatic_anticipation_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/list_seller_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/list_seller_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_card_token_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_card_token_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_three_d_secure_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_three_d_secure_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/create_shipping_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/create_shipping_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_discount_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_discount_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/models/get_withdraw_source_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/models/get_withdraw_source_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/controllers/charges_controller.py` & `pagarme-python-5.7.3/pagarmecoreapi/controllers/charges_controller.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/controllers/customers_controller.py` & `pagarme-python-5.7.3/pagarmecoreapi/controllers/customers_controller.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/controllers/tokens_controller.py` & `pagarme-python-5.7.3/pagarmecoreapi/controllers/tokens_controller.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/controllers/transfers_controller.py` & `pagarme-python-5.7.3/pagarmecoreapi/controllers/transfers_controller.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/controllers/subscriptions_controller.py` & `pagarme-python-5.7.3/pagarmecoreapi/controllers/subscriptions_controller.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/controllers/recipients_controller.py` & `pagarme-python-5.7.3/pagarmecoreapi/controllers/recipients_controller.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/controllers/transactions_controller.py` & `pagarme-python-5.7.3/pagarmecoreapi/controllers/transactions_controller.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/controllers/invoices_controller.py` & `pagarme-python-5.7.3/pagarmecoreapi/controllers/invoices_controller.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/controllers/plans_controller.py` & `pagarme-python-5.7.3/pagarmecoreapi/controllers/plans_controller.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/controllers/orders_controller.py` & `pagarme-python-5.7.3/pagarmecoreapi/controllers/orders_controller.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/controllers/base_controller.py` & `pagarme-python-5.7.3/pagarmecoreapi/controllers/base_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     """
 
     http_client = RequestsClient()
 
     http_call_back = None
 
     global_headers = {
-        'user-agent': 'PagarmeCoreApi - Python 5.7.2'
+        'user-agent': 'PagarmeCoreApi - Python 5.7.3'
     }
 
     def __init__(self, client=None, call_back=None):
         if client != None:
             self.http_client = client
         if call_back != None:
             self.http_call_back = call_back
```

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/controllers/sellers_controller.py` & `pagarme-python-5.7.3/pagarmecoreapi/controllers/sellers_controller.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/http/requests_client.py` & `pagarme-python-5.7.3/pagarmecoreapi/http/requests_client.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/http/http_method_enum.py` & `pagarme-python-5.7.3/pagarmecoreapi/http/http_method_enum.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/http/auth/basic_auth.py` & `pagarme-python-5.7.3/pagarmecoreapi/http/auth/basic_auth.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/http/http_request.py` & `pagarme-python-5.7.3/pagarmecoreapi/http/http_request.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/http/http_context.py` & `pagarme-python-5.7.3/pagarmecoreapi/http/http_context.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/http/http_client.py` & `pagarme-python-5.7.3/pagarmecoreapi/http/http_client.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/http/http_call_back.py` & `pagarme-python-5.7.3/pagarmecoreapi/http/http_call_back.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/http/http_response.py` & `pagarme-python-5.7.3/pagarmecoreapi/http/http_response.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/pagarmecoreapi/decorators.py` & `pagarme-python-5.7.3/pagarmecoreapi/decorators.py`

 * *Files identical despite different names*

### Comparing `pagarme-python-5.7.2/README.md` & `pagarme-python-5.7.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -424,16 +424,16 @@
 
 
 
 #### Example Usage
 
 ```python
 subscription_id = 'subscription_id'
-page = 130
-size = 130
+page = 11
+size = 11
 
 result = subscriptions_controller.get_increments(subscription_id, page, size)
 
 ```
 
 #### Errors
 
@@ -663,16 +663,16 @@
 
 
 
 #### Example Usage
 
 ```python
 subscription_id = 'subscription_id'
-page = 130
-size = 130
+page = 11
+size = 11
 name = 'name'
 code = 'code'
 status = 'status'
 description = 'description'
 created_since = 'created_since'
 created_until = 'created_until'
 
@@ -1048,16 +1048,16 @@
 
 
 #### Example Usage
 
 ```python
 subscription_id = 'subscription_id'
 item_id = 'item_id'
-page = 222
-size = 222
+page = 11
+size = 11
 code = 'code'
 group = 'group'
 used_since = datetime.now()
 used_until = datetime.now()
 
 result = subscriptions_controller.get_usages(subscription_id, item_id, page, size, code, group, used_since, used_until)
 
@@ -1282,16 +1282,16 @@
 
 
 
 #### Example Usage
 
 ```python
 subscription_id = 'subscription_id'
-page = 222
-size = 222
+page = 11
+size = 11
 
 result = subscriptions_controller.get_discounts(subscription_id, page, size)
 
 ```
 
 #### Errors
 
@@ -1434,16 +1434,16 @@
 | createdUntil |  ``` Optional ```  | Filter for subscriptions creation date end range |
 
 
 
 #### Example Usage
 
 ```python
-page = 222
-size = 222
+page = 61
+size = 61
 code = 'code'
 billing_type = 'billing_type'
 customer_id = 'customer_id'
 plan_id = 'plan_id'
 card_id = 'card_id'
 status = 'status'
 next_billing_since = datetime.now()
@@ -1816,16 +1816,16 @@
 | customerId |  ``` Optional ```  | Filter for order's customer id |
 
 
 
 #### Example Usage
 
 ```python
-page = 222
-size = 222
+page = 61
+size = 61
 code = 'code'
 status = 'status'
 created_since = datetime.now()
 created_until = datetime.now()
 customer_id = 'customer_id'
 
 result = orders_controller.get_orders(page, size, code, status, created_since, created_until, customer_id)
@@ -2506,16 +2506,16 @@
 | createdUntil |  ``` Optional ```  | Filter for plan's creation date end range |
 
 
 
 #### Example Usage
 
 ```python
-page = 222
-size = 222
+page = 61
+size = 61
 name = 'name'
 status = 'status'
 billing_type = 'billing_type'
 created_since = datetime.now()
 created_until = datetime.now()
 
 result = plans_controller.get_plans(page, size, name, status, billing_type, created_since, created_until)
@@ -2946,16 +2946,16 @@
 | customerDocument |  ``` Optional ```  | TODO: Add a parameter description |
 
 
 
 #### Example Usage
 
 ```python
-page = 222
-size = 222
+page = 61
+size = 61
 code = 'code'
 customer_id = 'customer_id'
 subscription_id = 'subscription_id'
 created_since = datetime.now()
 created_until = datetime.now()
 status = 'status'
 due_since = datetime.now()
@@ -3237,16 +3237,16 @@
 
 
 
 #### Example Usage
 
 ```python
 customer_id = 'customer_id'
-page = 180
-size = 180
+page = 20
+size = 20
 
 result = customers_controller.get_access_tokens(customer_id, page, size)
 
 ```
 
 #### Errors
 
@@ -3697,16 +3697,16 @@
 
 
 
 #### Example Usage
 
 ```python
 customer_id = 'customer_id'
-page = 180
-size = 180
+page = 20
+size = 20
 
 result = customers_controller.get_cards(customer_id, page, size)
 
 ```
 
 #### Errors
 
@@ -3921,16 +3921,16 @@
 
 
 
 #### Example Usage
 
 ```python
 customer_id = 'customer_id'
-page = 180
-size = 180
+page = 20
+size = 20
 
 result = customers_controller.get_addresses(customer_id, page, size)
 
 ```
 
 #### Errors
 
@@ -4114,16 +4114,16 @@
 
 
 
 #### Example Usage
 
 ```python
 charge_id = 'charge_id'
-page = 180
-size = 180
+page = 20
+size = 20
 
 result = charges_controller.get_charge_transactions(charge_id, page, size)
 
 ```
 
 #### Errors
 
@@ -4171,16 +4171,16 @@
 | createdUntil |  ``` Optional ```  | Filter for the end of the range for charge's creation |
 
 
 
 #### Example Usage
 
 ```python
-page = 180
-size = 180
+page = 20
+size = 20
 code = 'code'
 status = 'status'
 payment_method = 'payment_method'
 customer_id = 'customer_id'
 order_id = 'order_id'
 created_since = datetime.now()
 created_until = datetime.now()
@@ -4957,16 +4957,16 @@
 
 
 
 #### Example Usage
 
 ```python
 recipient_id = 'recipient_id'
-page = 180
-size = 180
+page = 20
+size = 20
 status = 'status'
 timeframe = 'timeframe'
 payment_date_since = datetime.now()
 payment_date_until = datetime.now()
 created_since = datetime.now()
 created_until = datetime.now()
 
@@ -5316,16 +5316,16 @@
 | size |  ``` Optional ```  | Page size |
 
 
 
 #### Example Usage
 
 ```python
-page = 16
-size = 16
+page = 111
+size = 111
 
 result = recipients_controller.get_recipients(page, size)
 
 ```
 
 #### Errors
 
@@ -5411,16 +5411,16 @@
 
 
 
 #### Example Usage
 
 ```python
 recipient_id = 'recipient_id'
-page = 16
-size = 16
+page = 111
+size = 111
 status = 'status'
 created_since = datetime.now()
 created_until = datetime.now()
 
 result = recipients_controller.get_transfers(recipient_id, page, size, status, created_since, created_until)
 
 ```
@@ -5466,16 +5466,16 @@
 
 
 
 #### Example Usage
 
 ```python
 recipient_id = 'recipient_id'
-page = 16
-size = 16
+page = 111
+size = 111
 status = 'status'
 created_since = datetime.now()
 created_until = datetime.now()
 
 result = recipients_controller.get_withdrawals(recipient_id, page, size, status, created_since, created_until)
 
 ```
```

