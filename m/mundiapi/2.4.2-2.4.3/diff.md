# Comparing `tmp/mundiapi-2.4.2.tar.gz` & `tmp/mundiapi-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mundiapi-2.4.2.tar", last modified: Fri Mar 31 21:07:12 2023, max compression
+gzip compressed data, was "dist/mundiapi-2.4.3.tar", last modified: Mon May 15 20:38:28 2023, max compression
```

## Comparing `mundiapi-2.4.2.tar` & `mundiapi-2.4.3.tar`

### file list

```diff
@@ -1,446 +1,446 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 21:07:12.000000 mundiapi-2.4.2/
--rw-r--r--   0 root         (0) root         (0)     1213 2023-03-31 21:07:08.000000 mundiapi-2.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       36 2023-03-31 21:07:08.000000 mundiapi-2.4.2/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 21:07:12.000000 mundiapi-2.4.2/mundiapi/
--rw-r--r--   0 root         (0) root         (0)     2243 2023-03-31 21:07:09.000000 mundiapi-2.4.2/mundiapi/mundiapi_client.py
--rw-r--r--   0 root         (0) root         (0)    13738 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/api_helper.py
--rw-r--r--   0 root         (0) root         (0)      163 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 21:07:12.000000 mundiapi-2.4.2/mundiapi/exceptions/
--rw-r--r--   0 root         (0) root         (0)       58 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      900 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/exceptions/api_exception.py
--rw-r--r--   0 root         (0) root         (0)     1360 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/exceptions/error_exception.py
--rw-r--r--   0 root         (0) root         (0)      898 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 21:07:12.000000 mundiapi-2.4.2/mundiapi/models/
--rw-r--r--   0 root         (0) root         (0)     1586 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/charges_due_date_request.py
--rw-r--r--   0 root         (0) root         (0)     1374 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/device_1.py
--rw-r--r--   0 root         (0) root         (0)     2195 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/price_bracket.py
--rw-r--r--   0 root         (0) root         (0)     3228 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/recipients_transfers_response.py
--rw-r--r--   0 root         (0) root         (0)     2743 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/pricing_scheme_4.py
--rw-r--r--   0 root         (0) root         (0)     7715 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/charges_metadata_response.py
--rw-r--r--   0 root         (0) root         (0)     7713 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/charges_due_date_response.py
--rw-r--r--   0 root         (0) root         (0)     1781 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_anticipation_limits_response.py
--rw-r--r--   0 root         (0) root         (0)     1620 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_bank_transfer_payment_request.py
--rw-r--r--   0 root         (0) root         (0)     2693 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_voucher_payment_request.py
--rw-r--r--   0 root         (0) root         (0)     1633 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_cancel_subscription_request.py
--rw-r--r--   0 root         (0) root         (0)     4401 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/subscriptions_items_usages_usage_id_response.py
--rw-r--r--   0 root         (0) root         (0)     8529 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/invoice.py
--rw-r--r--   0 root         (0) root         (0)     1627 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_location_request.py
--rw-r--r--   0 root         (0) root         (0)     1465 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/customers_access_tokens_request.py
--rw-r--r--   0 root         (0) root         (0)     3943 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/bank_account_1.py
--rw-r--r--   0 root         (0) root         (0)     1432 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/customers_metadata_request.py
--rw-r--r--   0 root         (0) root         (0)     1757 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/subscriptions_billing_date_request.py
--rw-r--r--   0 root         (0) root         (0)     1834 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/split.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/recipients_default_bank_account_request.py
--rw-r--r--   0 root         (0) root         (0)     1988 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/list_withdrawals.py
--rw-r--r--   0 root         (0) root         (0)     1865 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_payment_authentication_request.py
--rw-r--r--   0 root         (0) root         (0)     1683 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/fine.py
--rw-r--r--   0 root         (0) root         (0)     1598 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/pix_additional_information.py
--rw-r--r--   0 root         (0) root         (0)     1637 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/recipients_transfers_request.py
--rw-r--r--   0 root         (0) root         (0)     2002 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/list_customers_response.py
--rw-r--r--   0 root         (0) root         (0)     3466 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/submerchant.py
--rw-r--r--   0 root         (0) root         (0)     1397 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/update_invoice_status_request.py
--rw-r--r--   0 root         (0) root         (0)     3789 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_charge_request.py
--rw-r--r--   0 root         (0) root         (0)     1943 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/usages.py
--rw-r--r--   0 root         (0) root         (0)     1437 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_checkout_bank_transfer_payment_response.py
--rw-r--r--   0 root         (0) root         (0)     5259 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/customer.py
--rw-r--r--   0 root         (0) root         (0)     1670 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/tokens_request.py
--rw-r--r--   0 root         (0) root         (0)     2568 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_card_payment_contactless_request.py
--rw-r--r--   0 root         (0) root         (0)     2059 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/charges_transactions_response.py
--rw-r--r--   0 root         (0) root         (0)     2843 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/charges_request.py
--rw-r--r--   0 root         (0) root         (0)     2553 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/tokens_response.py
--rw-r--r--   0 root         (0) root         (0)     6757 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_checkout_payment_request.py
--rw-r--r--   0 root         (0) root         (0)     2237 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_price_bracket_response.py
--rw-r--r--   0 root         (0) root         (0)     2879 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/threed_secure_1.py
--rw-r--r--   0 root         (0) root         (0)     6990 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/orders_closed_response.py
--rw-r--r--   0 root         (0) root         (0)     1376 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/device.py
--rw-r--r--   0 root         (0) root         (0)     1362 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/bank_transfer.py
--rw-r--r--   0 root         (0) root         (0)     3993 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_recipient_request.py
--rw-r--r--   0 root         (0) root         (0)     2051 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/customers_access_tokens_response_1.py
--rw-r--r--   0 root         (0) root         (0)     1409 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_charges_summary_response.py
--rw-r--r--   0 root         (0) root         (0)     2938 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_checkout_credit_card_payment_request.py
--rw-r--r--   0 root         (0) root         (0)     3980 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_bank_account_request.py
--rw-r--r--   0 root         (0) root         (0)     1643 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/update_current_cycle_end_date_request.py
--rw-r--r--   0 root         (0) root         (0)     5656 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/customers_addresses_response_1.py
--rw-r--r--   0 root         (0) root         (0)     1576 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/bank_transfer_2.py
--rw-r--r--   0 root         (0) root         (0)     2034 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/options_2.py
--rw-r--r--   0 root         (0) root         (0)     5618 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/billingaddress_3.py
--rw-r--r--   0 root         (0) root         (0)     1580 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_period_request.py
--rw-r--r--   0 root         (0) root         (0)     1405 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_device_request.py
--rw-r--r--   0 root         (0) root         (0)     4408 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/subscriptions_discounts_response.py
--rw-r--r--   0 root         (0) root         (0)     6098 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/credit_card_1.py
--rw-r--r--   0 root         (0) root         (0)     2042 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/list_subscriptions_response.py
--rw-r--r--   0 root         (0) root         (0)     2437 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_antifraud_response.py
--rw-r--r--   0 root         (0) root         (0)     1951 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/debit_card_2.py
--rw-r--r--   0 root         (0) root         (0)     2013 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_checkout_debit_card_payment_response.py
--rw-r--r--   0 root         (0) root         (0)     2969 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/subscriptions_items_request.py
--rw-r--r--   0 root         (0) root         (0)     1917 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/update_subscription_split_request.py
--rw-r--r--   0 root         (0) root         (0)     3556 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_checkout_payment_settings_response.py
--rw-r--r--   0 root         (0) root         (0)     1520 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/update_subscription_due_days_request.py
--rw-r--r--   0 root         (0) root         (0)     1527 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/options_1.py
--rw-r--r--   0 root         (0) root         (0)     1991 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/customers_cards_response_1.py
--rw-r--r--   0 root         (0) root         (0)     1435 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/recipients_metadata_request.py
--rw-r--r--   0 root         (0) root         (0)     6121 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/customers_cards_renew_response.py
--rw-r--r--   0 root         (0) root         (0)     8616 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/subscriptions_partial_invoice_response.py
--rw-r--r--   0 root         (0) root         (0)     1794 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_transaction_report_file_response.py
--rw-r--r--   0 root         (0) root         (0)     1898 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_subscription_split_response.py
--rw-r--r--   0 root         (0) root         (0)     4328 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_usage_response.py
--rw-r--r--   0 root         (0) root         (0)     7220 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/plans_response_1.py
--rw-r--r--   0 root         (0) root         (0)     5560 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_bank_account_response.py
--rw-r--r--   0 root         (0) root         (0)     2663 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/plans_items_request_1.py
--rw-r--r--   0 root         (0) root         (0)     1722 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/recipients_anticipation_limits_response.py
--rw-r--r--   0 root         (0) root         (0)     6890 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/recipient.py
--rw-r--r--   0 root         (0) root         (0)     1420 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/plans_metadata_request.py
--rw-r--r--   0 root         (0) root         (0)     5222 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_card_request.py
--rw-r--r--   0 root         (0) root         (0)    11218 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/subscriptions_request_1.py
--rw-r--r--   0 root         (0) root         (0)     2458 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/subscriptions_increments_request.py
--rw-r--r--   0 root         (0) root         (0)     5296 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_customer_response.py
--rw-r--r--   0 root         (0) root         (0)     2394 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/update_recipient_request.py
--rw-r--r--   0 root         (0) root         (0)     4452 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_plan_item_response.py
--rw-r--r--   0 root         (0) root         (0)     2000 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/list_anticipation_response.py
--rw-r--r--   0 root         (0) root         (0)     4094 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/cycle.py
--rw-r--r--   0 root         (0) root         (0)     2079 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/list_charge_transactions_response.py
--rw-r--r--   0 root         (0) root         (0)     1417 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/update_current_cycle_status_request.py
--rw-r--r--   0 root         (0) root         (0)     3306 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_invoice_item_response.py
--rw-r--r--   0 root         (0) root         (0)     1982 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/list_order_response.py
--rw-r--r--   0 root         (0) root         (0)     3677 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_customer_request.py
--rw-r--r--   0 root         (0) root         (0)     1419 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_device_response.py
--rw-r--r--   0 root         (0) root         (0)     4132 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_period_response.py
--rw-r--r--   0 root         (0) root         (0)     4420 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/subscriptions_increments_response.py
--rw-r--r--   0 root         (0) root         (0)     2179 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_pix_bank_account_response.py
--rw-r--r--   0 root         (0) root         (0)     5287 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/customers_response.py
--rw-r--r--   0 root         (0) root         (0)     1591 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/location.py
--rw-r--r--   0 root         (0) root         (0)     2005 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/list_discounts_response.py
--rw-r--r--   0 root         (0) root         (0)     4097 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/period.py
--rw-r--r--   0 root         (0) root         (0)    12195 2023-03-31 21:07:09.000000 mundiapi-2.4.2/mundiapi/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2439 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_order_item_response.py
--rw-r--r--   0 root         (0) root         (0)     8601 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/subscriptions_cycles_pay_response.py
--rw-r--r--   0 root         (0) root         (0)     6974 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/orders_response_1.py
--rw-r--r--   0 root         (0) root         (0)     2391 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/update_automatic_anticipation_settings_request.py
--rw-r--r--   0 root         (0) root         (0)     3111 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/update_card_request.py
--rw-r--r--   0 root         (0) root         (0)     6943 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/order.py
--rw-r--r--   0 root         (0) root         (0)     2059 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/subscriptions_items_response_3.py
--rw-r--r--   0 root         (0) root         (0)     1570 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_card_options_request.py
--rw-r--r--   0 root         (0) root         (0)     2116 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_transfer.py
--rw-r--r--   0 root         (0) root         (0)     2109 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/recipients_anticipations_request.py
--rw-r--r--   0 root         (0) root         (0)     1772 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_emv_data_tlv_decrypt_request.py
--rw-r--r--   0 root         (0) root         (0)     1904 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/gateway_response.py
--rw-r--r--   0 root         (0) root         (0)     2333 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/update_charge_card_request.py
--rw-r--r--   0 root         (0) root         (0)     1656 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_checkout_card_installment_options_response.py
--rw-r--r--   0 root         (0) root         (0)     6978 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_order_response.py
--rw-r--r--   0 root         (0) root         (0)     3645 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/customers_request.py
--rw-r--r--   0 root         (0) root         (0)     1752 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/update_subscription_card_request.py
--rw-r--r--   0 root         (0) root         (0)     4258 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/private_label.py
--rw-r--r--   0 root         (0) root         (0)     1448 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/subscriptions_cycles_pay_request.py
--rw-r--r--   0 root         (0) root         (0)     1444 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/subscriptions_metadata_request.py
--rw-r--r--   0 root         (0) root         (0)     1970 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/list_plans_response.py
--rw-r--r--   0 root         (0) root         (0)     4333 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_private_label_payment_request.py
--rw-r--r--   0 root         (0) root         (0)     3437 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_billing_address_response.py
--rw-r--r--   0 root         (0) root         (0)     1445 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_clear_sale_request.py
--rw-r--r--   0 root         (0) root         (0)     3656 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/update_customer_request.py
--rw-r--r--   0 root         (0) root         (0)     4138 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/recipients_anticipations_response.py
--rw-r--r--   0 root         (0) root         (0)     1808 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/authentication_2.py
--rw-r--r--   0 root         (0) root         (0)     8582 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/invoices_metadata_response.py
--rw-r--r--   0 root         (0) root         (0)     1427 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/clear_sale_request.py
--rw-r--r--   0 root         (0) root         (0)     2246 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/orders_items_request.py
--rw-r--r--   0 root         (0) root         (0)     6105 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/customers_cards_response.py
--rw-r--r--   0 root         (0) root         (0)     3185 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_transfer_response.py
--rw-r--r--   0 root         (0) root         (0)     1652 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_transfer_target_response.py
--rw-r--r--   0 root         (0) root         (0)     4162 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/subscriptions_cycles_response.py
--rw-r--r--   0 root         (0) root         (0)     2591 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_access_token_response.py
--rw-r--r--   0 root         (0) root         (0)     1997 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/list_invoices_response.py
--rw-r--r--   0 root         (0) root         (0)     2069 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/customers_addresses_request_1.py
--rw-r--r--   0 root         (0) root         (0)     2629 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_emv_decrypt_request.py
--rw-r--r--   0 root         (0) root         (0)     2385 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/recipients_request_1.py
--rw-r--r--   0 root         (0) root         (0)     6975 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/recipients_default_bank_account_response.py
--rw-r--r--   0 root         (0) root         (0)     2862 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/credit_card_2.py
--rw-r--r--   0 root         (0) root         (0)     6707 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/checkout.py
--rw-r--r--   0 root         (0) root         (0)     1614 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/subscriptions_gateway_affiliation_id_request.py
--rw-r--r--   0 root         (0) root         (0)     2744 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_split_response.py
--rw-r--r--   0 root         (0) root         (0)     5551 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/default_bank_account.py
--rw-r--r--   0 root         (0) root         (0)     1995 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_phones_request.py
--rw-r--r--   0 root         (0) root         (0)     2981 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_usages_details_response.py
--rw-r--r--   0 root         (0) root         (0)     7222 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_plan_response.py
--rw-r--r--   0 root         (0) root         (0)     2550 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_google_pay_request.py
--rw-r--r--   0 root         (0) root         (0)     2985 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/update_subscription_item_request.py
--rw-r--r--   0 root         (0) root         (0)     2027 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/subscriptions_response_3.py
--rw-r--r--   0 root         (0) root         (0)     4641 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/update_charge_payment_method_request.py
--rw-r--r--   0 root         (0) root         (0)     1660 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_token_request.py
--rw-r--r--   0 root         (0) root         (0)     2857 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_pricing_scheme_response.py
--rw-r--r--   0 root         (0) root         (0)     2146 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_pix_payer_response.py
--rw-r--r--   0 root         (0) root         (0)     2328 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_gateway_recipient_response.py
--rw-r--r--   0 root         (0) root         (0)     3640 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/customer_8.py
--rw-r--r--   0 root         (0) root         (0)     1711 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_interest_response.py
--rw-r--r--   0 root         (0) root         (0)     1948 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/list_transfers.py
--rw-r--r--   0 root         (0) root         (0)     4612 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/charges_payment_method_request.py
--rw-r--r--   0 root         (0) root         (0)     6273 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_order_request.py
--rw-r--r--   0 root         (0) root         (0)     2012 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/setup.py
--rw-r--r--   0 root         (0) root         (0)    92051 2023-03-31 21:07:09.000000 mundiapi-2.4.2/mundiapi/models/get_transaction_response.py
--rw-r--r--   0 root         (0) root         (0)     2774 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/recipients_balance_response.py
--rw-r--r--   0 root         (0) root         (0)     2434 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/orders_items_response_1.py
--rw-r--r--   0 root         (0) root         (0)     2872 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_cancel_charge_request.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_location_response.py
--rw-r--r--   0 root         (0) root         (0)     3124 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_card_token_response.py
--rw-r--r--   0 root         (0) root         (0)     4805 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_boleto_payment_request.py
--rw-r--r--   0 root         (0) root         (0)     2034 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_checkout_debit_card_payment_request.py
--rw-r--r--   0 root         (0) root         (0)     6996 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/orders_metadata_response.py
--rw-r--r--   0 root         (0) root         (0)     2263 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/subscriptions_payment_method_request.py
--rw-r--r--   0 root         (0) root         (0)     3734 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_debit_card_payment_request.py
--rw-r--r--   0 root         (0) root         (0)     2497 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/charges_capture_request.py
--rw-r--r--   0 root         (0) root         (0)     1395 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_gateway_error_response.py
--rw-r--r--   0 root         (0) root         (0)     2004 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/list_recipient_response.py
--rw-r--r--   0 root         (0) root         (0)    11229 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_subscription_request.py
--rw-r--r--   0 root         (0) root         (0)     2111 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_transfer_settings_request.py
--rw-r--r--   0 root         (0) root         (0)     1967 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/orders_response.py
--rw-r--r--   0 root         (0) root         (0)     3785 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/shipping.py
--rw-r--r--   0 root         (0) root         (0)     2046 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/update_address_request.py
--rw-r--r--   0 root         (0) root         (0)     4032 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/shipping_3.py
--rw-r--r--   0 root         (0) root         (0)     1989 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/list_transfer_response.py
--rw-r--r--   0 root         (0) root         (0)     1653 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_withdraw_request.py
--rw-r--r--   0 root         (0) root         (0)     2724 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_balance_response.py
--rw-r--r--   0 root         (0) root         (0)     4378 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/subscriptions_items_usages_response.py
--rw-r--r--   0 root         (0) root         (0)     1429 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/invoices_metadata_request.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/update_transfer_settings_request.py
--rw-r--r--   0 root         (0) root         (0)     2015 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/recipients_transfers_response_1.py
--rw-r--r--   0 root         (0) root         (0)     2000 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/list_usages_details_response.py
--rw-r--r--   0 root         (0) root         (0)     2134 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/header.py
--rw-r--r--   0 root         (0) root         (0)     2814 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/pricing_scheme.py
--rw-r--r--   0 root         (0) root         (0)     1882 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_checkout_boleto_payment_response.py
--rw-r--r--   0 root         (0) root         (0)     7690 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/charges_response.py
--rw-r--r--   0 root         (0) root         (0)     2123 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/update_order_item_request.py
--rw-r--r--   0 root         (0) root         (0)     2690 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/plans_items_request.py
--rw-r--r--   0 root         (0) root         (0)     3753 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/subscriptions_items_request_1.py
--rw-r--r--   0 root         (0) root         (0)     1695 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/interest.py
--rw-r--r--   0 root         (0) root         (0)     2918 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_three_d_secure_request.py
--rw-r--r--   0 root         (0) root         (0)     1989 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/recipients_response.py
--rw-r--r--   0 root         (0) root         (0)     6468 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_plan_request.py
--rw-r--r--   0 root         (0) root         (0)     1620 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/update_subscription_affiliation_id_request.py
--rw-r--r--   0 root         (0) root         (0)     3779 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/charges_request_1.py
--rw-r--r--   0 root         (0) root         (0)    10486 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_checkout_payment_response.py
--rw-r--r--   0 root         (0) root         (0)     2256 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_order_item_request.py
--rw-r--r--   0 root         (0) root         (0)     1419 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/update_metadata_request.py
--rw-r--r--   0 root         (0) root         (0)     1933 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/setup_1.py
--rw-r--r--   0 root         (0) root         (0)     2013 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/list_increments_response.py
--rw-r--r--   0 root         (0) root         (0)     2168 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_price_bracket_request.py
--rw-r--r--   0 root         (0) root         (0)     5631 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_address_response.py
--rw-r--r--   0 root         (0) root         (0)     1828 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_cancel_charge_split_rules_request.py
--rw-r--r--   0 root         (0) root         (0)     4090 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_anticipation_response.py
--rw-r--r--   0 root         (0) root         (0)     2393 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/cancel_split_request.py
--rw-r--r--   0 root         (0) root         (0)     5096 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/update_plan_request.py
--rw-r--r--   0 root         (0) root         (0)     1679 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_anticipation_limit_response.py
--rw-r--r--   0 root         (0) root         (0)     1788 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/update_subscription_billing_date_request.py
--rw-r--r--   0 root         (0) root         (0)     1652 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_withdraw_target_response.py
--rw-r--r--   0 root         (0) root         (0)     2076 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_split_options_request.py
--rw-r--r--   0 root         (0) root         (0)     1402 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/update_order_status_request.py
--rw-r--r--   0 root         (0) root         (0)     2434 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_increment_request.py
--rw-r--r--   0 root         (0) root         (0)    10537 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_subscription_response.py
--rw-r--r--   0 root         (0) root         (0)     1529 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/header_1.py
--rw-r--r--   0 root         (0) root         (0)     1455 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_access_token_request.py
--rw-r--r--   0 root         (0) root         (0)     2534 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_token_response.py
--rw-r--r--   0 root         (0) root         (0)     2033 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/list_transactions_response.py
--rw-r--r--   0 root         (0) root         (0)     5252 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_transfer.py
--rw-r--r--   0 root         (0) root         (0)     1935 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_gateway_response_response.py
--rw-r--r--   0 root         (0) root         (0)     2698 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/update_plan_item_request.py
--rw-r--r--   0 root         (0) root         (0)     2683 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_checkout_credit_card_payment_response.py
--rw-r--r--   0 root         (0) root         (0)     2119 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/list_transactions_files_response.py
--rw-r--r--   0 root         (0) root         (0)     1987 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/invoices_response_2.py
--rw-r--r--   0 root         (0) root         (0)     2001 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/list_addresses_response.py
--rw-r--r--   0 root         (0) root         (0)     2042 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_checkout_boleto_payment_request.py
--rw-r--r--   0 root         (0) root         (0)     2607 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/customers_access_tokens_response.py
--rw-r--r--   0 root         (0) root         (0)     2068 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_setup_response.py
--rw-r--r--   0 root         (0) root         (0)     3662 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_address_request.py
--rw-r--r--   0 root         (0) root         (0)     3482 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_sub_merchant_request.py
--rw-r--r--   0 root         (0) root         (0)     2782 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_pricing_scheme_request.py
--rw-r--r--   0 root         (0) root         (0)     7712 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/charges_capture_response.py
--rw-r--r--   0 root         (0) root         (0)     1696 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/update_subscription_start_at_request.py
--rw-r--r--   0 root         (0) root         (0)     1652 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_transfer_source_response.py
--rw-r--r--   0 root         (0) root         (0)     1423 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/orders_metadata_request.py
--rw-r--r--   0 root         (0) root         (0)     3770 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_subscription_item_request.py
--rw-r--r--   0 root         (0) root         (0)     1617 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_transfer_request.py
--rw-r--r--   0 root         (0) root         (0)     2293 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/update_subscription_payment_method_request.py
--rw-r--r--   0 root         (0) root         (0)     2668 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_plan_item_request.py
--rw-r--r--   0 root         (0) root         (0)     2571 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/pix.py
--rw-r--r--   0 root         (0) root         (0)     3829 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_shipping_response.py
--rw-r--r--   0 root         (0) root         (0)     7706 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/charges_retry_response.py
--rw-r--r--   0 root         (0) root         (0)     1553 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/bank_transfer_1.py
--rw-r--r--   0 root         (0) root         (0)     7731 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/charges_payment_method_response.py
--rw-r--r--   0 root         (0) root         (0)     5092 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/plans_request_1.py
--rw-r--r--   0 root         (0) root         (0)     1586 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_google_pay_header_request.py
--rw-r--r--   0 root         (0) root         (0)     3626 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/address_1.py
--rw-r--r--   0 root         (0) root         (0)     1504 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/subscriptions_minimum_price_request.py
--rw-r--r--   0 root         (0) root         (0)     8557 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/invoices_response.py
--rw-r--r--   0 root         (0) root         (0)     2061 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_setup_request.py
--rw-r--r--   0 root         (0) root         (0)     5261 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/customers_cards_request.py
--rw-r--r--   0 root         (0) root         (0)     2013 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_usage_report_response.py
--rw-r--r--   0 root         (0) root         (0)     1620 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/max.py
--rw-r--r--   0 root         (0) root         (0)     1426 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/charges_metadata_request.py
--rw-r--r--   0 root         (0) root         (0)     8576 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/invoices_status_response.py
--rw-r--r--   0 root         (0) root         (0)     1970 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/list_cards_response.py
--rw-r--r--   0 root         (0) root         (0)     4390 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_increment_response.py
--rw-r--r--   0 root         (0) root         (0)     2397 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_emv_data_decrypt_request.py
--rw-r--r--   0 root         (0) root         (0)     3097 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/update_seller_request.py
--rw-r--r--   0 root         (0) root         (0)     6089 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_card_response.py
--rw-r--r--   0 root         (0) root         (0)     2743 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/pricing_scheme_3.py
--rw-r--r--   0 root         (0) root         (0)     2500 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/apple_pay.py
--rw-r--r--   0 root         (0) root         (0)     1804 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/authentication.py
--rw-r--r--   0 root         (0) root         (0)     1989 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_phones_response.py
--rw-r--r--   0 root         (0) root         (0)     6943 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/recipients_metadata_response.py
--rw-r--r--   0 root         (0) root         (0)     3665 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/customers_request_1.py
--rw-r--r--   0 root         (0) root         (0)     2324 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/threed_secure.py
--rw-r--r--   0 root         (0) root         (0)     2094 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_anticipation_request.py
--rw-r--r--   0 root         (0) root         (0)     6921 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/recipients_response_1.py
--rw-r--r--   0 root         (0) root         (0)     2102 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_split_options_response.py
--rw-r--r--   0 root         (0) root         (0)     2037 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/list_access_tokens_response.py
--rw-r--r--   0 root         (0) root         (0)     2095 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_transfer_settings_response.py
--rw-r--r--   0 root         (0) root         (0)     6461 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/plans_request.py
--rw-r--r--   0 root         (0) root         (0)     5530 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/bank_account.py
--rw-r--r--   0 root         (0) root         (0)     8566 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_invoice_response.py
--rw-r--r--   0 root         (0) root         (0)     1636 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/subscriptions_periods_latest_end_at_request.py
--rw-r--r--   0 root         (0) root         (0)     7008 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/recipients_automatic_anticipation_settings_response.py
--rw-r--r--   0 root         (0) root         (0)     2029 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/subscriptions_cycles_response_2.py
--rw-r--r--   0 root         (0) root         (0)     1916 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/update_recipient_bank_account_request.py
--rw-r--r--   0 root         (0) root         (0)     2007 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/list_usages_response.py
--rw-r--r--   0 root         (0) root         (0)     2420 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_card_payment_contactless_poi_request.py
--rw-r--r--   0 root         (0) root         (0)     3709 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_seller_response.py
--rw-r--r--   0 root         (0) root         (0)     2417 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_discount_request.py
--rw-r--r--   0 root         (0) root         (0)     2724 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_usage_request.py
--rw-r--r--   0 root         (0) root         (0)     2539 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_apple_pay_request.py
--rw-r--r--   0 root         (0) root         (0)     6907 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_recipient_response.py
--rw-r--r--   0 root         (0) root         (0)     2136 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_split_request.py
--rw-r--r--   0 root         (0) root         (0)     1905 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_phone_response.py
--rw-r--r--   0 root         (0) root         (0)     2059 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_transaction_report_file_request.py
--rw-r--r--   0 root         (0) root         (0)     1979 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/charges_response_2.py
--rw-r--r--   0 root         (0) root         (0)     1700 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_fine_request.py
--rw-r--r--   0 root         (0) root         (0)     1695 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_fine_response.py
--rw-r--r--   0 root         (0) root         (0)     6049 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/card.py
--rw-r--r--   0 root         (0) root         (0)     2027 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/subscriptions_items_usages_response_1.py
--rw-r--r--   0 root         (0) root         (0)     6948 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_payment_request.py
--rw-r--r--   0 root         (0) root         (0)     7734 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/charges_confirm_payment_response.py
--rw-r--r--   0 root         (0) root         (0)     3098 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/card_9.py
--rw-r--r--   0 root         (0) root         (0)     3135 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/customers_cards_request_1.py
--rw-r--r--   0 root         (0) root         (0)     1418 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_invoice_request.py
--rw-r--r--   0 root         (0) root         (0)     5270 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_withdraw_response.py
--rw-r--r--   0 root         (0) root         (0)     2399 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_automatic_anticipation_settings_request.py
--rw-r--r--   0 root         (0) root         (0)     1960 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/plans_response.py
--rw-r--r--   0 root         (0) root         (0)     3981 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/recipients_request.py
--rw-r--r--   0 root         (0) root         (0)     6987 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/orders_items_response.py
--rw-r--r--   0 root         (0) root         (0)     2705 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/card_11.py
--rw-r--r--   0 root         (0) root         (0)     7242 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/plans_metadata_response.py
--rw-r--r--   0 root         (0) root         (0)     6931 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/recipients_code_response.py
--rw-r--r--   0 root         (0) root         (0)     1602 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/update_charge_due_date_request.py
--rw-r--r--   0 root         (0) root         (0)     1404 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_emv_data_dukpt_decrypt_request.py
--rw-r--r--   0 root         (0) root         (0)     7697 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_charge_response.py
--rw-r--r--   0 root         (0) root         (0)     1642 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_checkout_card_installment_option_request.py
--rw-r--r--   0 root         (0) root         (0)     2494 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/contactless.py
--rw-r--r--   0 root         (0) root         (0)     2784 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_sellers_request.py
--rw-r--r--   0 root         (0) root         (0)     2125 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/orders_items_request_1.py
--rw-r--r--   0 root         (0) root         (0)     1988 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/list_charges_response.py
--rw-r--r--   0 root         (0) root         (0)     1994 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/customers_response_3.py
--rw-r--r--   0 root         (0) root         (0)     3665 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/debit_card_1.py
--rw-r--r--   0 root         (0) root         (0)     1855 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_payment_authentication_response.py
--rw-r--r--   0 root         (0) root         (0)     7662 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/charge.py
--rw-r--r--   0 root         (0) root         (0)     1716 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_interest_request.py
--rw-r--r--   0 root         (0) root         (0)     1724 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/subscriptions_card_request.py
--rw-r--r--   0 root         (0) root         (0)     2010 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/list_cycles_response.py
--rw-r--r--   0 root         (0) root         (0)     5211 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/card_1.py
--rw-r--r--   0 root         (0) root         (0)     1640 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_checkout_bank_transfer_request.py
--rw-r--r--   0 root         (0) root         (0)     6931 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/payment.py
--rw-r--r--   0 root         (0) root         (0)     2442 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/subscriptions_discounts_request.py
--rw-r--r--   0 root         (0) root         (0)     1741 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/paging.py
--rw-r--r--   0 root         (0) root         (0)     4446 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/plans_items_response.py
--rw-r--r--   0 root         (0) root         (0)     2047 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/recipients_anticipations_response_1.py
--rw-r--r--   0 root         (0) root         (0)     2190 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_apple_pay_header_request.py
--rw-r--r--   0 root         (0) root         (0)     4731 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/boleto_1.py
--rw-r--r--   0 root         (0) root         (0)     3964 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/default_bank_account_1.py
--rw-r--r--   0 root         (0) root         (0)     2624 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/voucher.py
--rw-r--r--   0 root         (0) root         (0)     2476 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/token.py
--rw-r--r--   0 root         (0) root         (0)     2198 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/update_price_bracket_request.py
--rw-r--r--   0 root         (0) root         (0)     5733 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_subscription_item_response.py
--rw-r--r--   0 root         (0) root         (0)     1832 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_antifraud_request.py
--rw-r--r--   0 root         (0) root         (0)     5312 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/customers_metadata_response.py
--rw-r--r--   0 root         (0) root         (0)     7703 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/charges_card_response.py
--rw-r--r--   0 root         (0) root         (0)     2861 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_seller_request.py
--rw-r--r--   0 root         (0) root         (0)     2782 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/update_pricing_scheme_request.py
--rw-r--r--   0 root         (0) root         (0)     1789 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/paging_response.py
--rw-r--r--   0 root         (0) root         (0)     4115 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/current_cycle.py
--rw-r--r--   0 root         (0) root         (0)     3393 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/billing_address.py
--rw-r--r--   0 root         (0) root         (0)     2074 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/list_subscription_items_response.py
--rw-r--r--   0 root         (0) root         (0)     1903 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_subscription_split_request.py
--rw-r--r--   0 root         (0) root         (0)     1911 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_phone_request.py
--rw-r--r--   0 root         (0) root         (0)     6968 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/recipients_transfer_settings_response.py
--rw-r--r--   0 root         (0) root         (0)     1620 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/min.py
--rw-r--r--   0 root         (0) root         (0)     3679 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/customers_addresses_request.py
--rw-r--r--   0 root         (0) root         (0)     7189 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/plan.py
--rw-r--r--   0 root         (0) root         (0)     1727 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_cash_payment_request.py
--rw-r--r--   0 root         (0) root         (0)     2506 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_capture_charge_request.py
--rw-r--r--   0 root         (0) root         (0)     2641 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_pix_payment_request.py
--rw-r--r--   0 root         (0) root         (0)     1526 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/update_subscription_minimum_price_request.py
--rw-r--r--   0 root         (0) root         (0)     2510 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/google_pay.py
--rw-r--r--   0 root         (0) root         (0)     1828 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_confirm_payment_request.py
--rw-r--r--   0 root         (0) root         (0)     1599 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/subscriptions_request.py
--rw-r--r--   0 root         (0) root         (0)     6168 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_credit_card_payment_request.py
--rw-r--r--   0 root         (0) root         (0)     5594 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/address.py
--rw-r--r--   0 root         (0) root         (0)     2369 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_automatic_anticipation_response.py
--rw-r--r--   0 root         (0) root         (0)     2001 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/list_seller_response.py
--rw-r--r--   0 root         (0) root         (0)     2015 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/customers_addresses_response.py
--rw-r--r--   0 root         (0) root         (0)     6264 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/orders_request.py
--rw-r--r--   0 root         (0) root         (0)     2734 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_card_token_request.py
--rw-r--r--   0 root         (0) root         (0)     2359 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_three_d_secure_response.py
--rw-r--r--   0 root         (0) root         (0)     1663 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/subscriptions_start_at_request.py
--rw-r--r--   0 root         (0) root         (0)     3647 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/billing_address_1.py
--rw-r--r--   0 root         (0) root         (0)     2324 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/charges_card_request.py
--rw-r--r--   0 root         (0) root         (0)     4047 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_shipping_request.py
--rw-r--r--   0 root         (0) root         (0)     2322 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/create_card_payment_token_request.py
--rw-r--r--   0 root         (0) root         (0)     4377 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_discount_response.py
--rw-r--r--   0 root         (0) root         (0)     1652 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/models/get_withdraw_source_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 21:07:12.000000 mundiapi-2.4.2/mundiapi/controllers/
--rw-r--r--   0 root         (0) root         (0)    36631 2023-03-31 21:07:09.000000 mundiapi-2.4.2/mundiapi/controllers/charges_controller.py
--rw-r--r--   0 root         (0) root         (0)    56276 2023-03-31 21:07:09.000000 mundiapi-2.4.2/mundiapi/controllers/customers_controller.py
--rw-r--r--   0 root         (0) root         (0)     5995 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/controllers/tokens_controller.py
--rw-r--r--   0 root         (0) root         (0)     7100 2023-03-31 21:07:09.000000 mundiapi-2.4.2/mundiapi/controllers/transfers_controller.py
--rw-r--r--   0 root         (0) root         (0)      321 2023-03-31 21:07:09.000000 mundiapi-2.4.2/mundiapi/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)   103373 2023-03-31 21:07:09.000000 mundiapi-2.4.2/mundiapi/controllers/subscriptions_controller.py
--rw-r--r--   0 root         (0) root         (0)    56785 2023-03-31 21:07:09.000000 mundiapi-2.4.2/mundiapi/controllers/recipients_controller.py
--rw-r--r--   0 root         (0) root         (0)     2914 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/controllers/transactions_controller.py
--rw-r--r--   0 root         (0) root         (0)    20610 2023-03-31 21:07:09.000000 mundiapi-2.4.2/mundiapi/controllers/invoices_controller.py
--rw-r--r--   0 root         (0) root         (0)    26680 2023-03-31 21:07:09.000000 mundiapi-2.4.2/mundiapi/controllers/plans_controller.py
--rw-r--r--   0 root         (0) root         (0)    26874 2023-03-31 21:07:09.000000 mundiapi-2.4.2/mundiapi/controllers/orders_controller.py
--rw-r--r--   0 root         (0) root         (0)     3299 2023-03-31 21:07:09.000000 mundiapi-2.4.2/mundiapi/controllers/base_controller.py
--rw-r--r--   0 root         (0) root         (0)    11840 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/controllers/sellers_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 21:07:12.000000 mundiapi-2.4.2/mundiapi/http/
--rw-r--r--   0 root         (0) root         (0)     3533 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/http/requests_client.py
--rw-r--r--   0 root         (0) root         (0)      920 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/http/http_method_enum.py
--rw-r--r--   0 root         (0) root         (0)      181 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/http/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 21:07:12.000000 mundiapi-2.4.2/mundiapi/http/auth/
--rw-r--r--   0 root         (0) root         (0)       31 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/http/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      835 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/http/auth/basic_auth.py
--rw-r--r--   0 root         (0) root         (0)     2820 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/http/http_request.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/http/http_context.py
--rw-r--r--   0 root         (0) root         (0)     7088 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/http/http_client.py
--rw-r--r--   0 root         (0) root         (0)     1115 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/http/http_call_back.py
--rw-r--r--   0 root         (0) root         (0)     1088 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/http/http_response.py
--rw-r--r--   0 root         (0) root         (0)      509 2023-03-31 21:07:08.000000 mundiapi-2.4.2/mundiapi/decorators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 21:07:12.000000 mundiapi-2.4.2/tests/
--rw-r--r--   0 root         (0) root         (0)      669 2023-03-31 21:07:08.000000 mundiapi-2.4.2/tests/http_response_catcher.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-31 21:07:08.000000 mundiapi-2.4.2/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5119 2023-03-31 21:07:08.000000 mundiapi-2.4.2/tests/test_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 21:07:12.000000 mundiapi-2.4.2/tests/controllers/
--rw-r--r--   0 root         (0) root         (0)     1309 2023-03-31 21:07:08.000000 mundiapi-2.4.2/tests/controllers/test_plans_controller.py
--rw-r--r--   0 root         (0) root         (0)     1171 2023-03-31 21:07:08.000000 mundiapi-2.4.2/tests/controllers/test_recipients_controller.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-31 21:07:08.000000 mundiapi-2.4.2/tests/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      963 2023-03-31 21:07:08.000000 mundiapi-2.4.2/tests/controllers/controller_test_base.py
--rw-r--r--   0 root         (0) root         (0)     1574 2023-03-31 21:07:08.000000 mundiapi-2.4.2/tests/controllers/test_subscriptions_controller.py
--rw-r--r--   0 root         (0) root         (0)     1055 2023-03-31 21:07:08.000000 mundiapi-2.4.2/tests/controllers/test_transfers_controller.py
--rw-r--r--   0 root         (0) root         (0)     1501 2023-03-31 21:07:08.000000 mundiapi-2.4.2/tests/controllers/test_invoices_controller.py
--rw-r--r--   0 root         (0) root         (0)     1254 2023-03-31 21:07:08.000000 mundiapi-2.4.2/tests/controllers/test_customers_controller.py
--rw-r--r--   0 root         (0) root         (0)     1313 2023-03-31 21:07:08.000000 mundiapi-2.4.2/tests/controllers/test_orders_controller.py
--rw-r--r--   0 root         (0) root         (0)     1402 2023-03-31 21:07:08.000000 mundiapi-2.4.2/tests/controllers/test_charges_controller.py
--rw-r--r--   0 root         (0) root         (0)      241 2023-03-31 21:07:12.000000 mundiapi-2.4.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      869 2023-03-31 21:07:12.000000 mundiapi-2.4.2/setup.py
--rw-r--r--   0 root         (0) root         (0)       59 2023-03-31 21:07:12.000000 mundiapi-2.4.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 21:07:12.000000 mundiapi-2.4.2/mundiapi.egg-info/
--rw-r--r--   0 root         (0) root         (0)      241 2023-03-31 21:07:12.000000 mundiapi-2.4.2/mundiapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    18414 2023-03-31 21:07:12.000000 mundiapi-2.4.2/mundiapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 21:07:12.000000 mundiapi-2.4.2/mundiapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-03-31 21:07:12.000000 mundiapi-2.4.2/mundiapi.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      102 2023-03-31 21:07:12.000000 mundiapi-2.4.2/mundiapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)   152359 2023-03-31 21:07:09.000000 mundiapi-2.4.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 20:38:28.000000 mundiapi-2.4.3/
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-05-15 20:38:23.000000 mundiapi-2.4.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       36 2023-05-15 20:38:23.000000 mundiapi-2.4.3/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 20:38:28.000000 mundiapi-2.4.3/mundiapi/
+-rw-r--r--   0 root         (0) root         (0)     2243 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/mundiapi_client.py
+-rw-r--r--   0 root         (0) root         (0)    13738 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/api_helper.py
+-rw-r--r--   0 root         (0) root         (0)      163 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 20:38:28.000000 mundiapi-2.4.3/mundiapi/exceptions/
+-rw-r--r--   0 root         (0) root         (0)       58 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      900 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/exceptions/api_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1360 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/exceptions/error_exception.py
+-rw-r--r--   0 root         (0) root         (0)      898 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 20:38:28.000000 mundiapi-2.4.3/mundiapi/models/
+-rw-r--r--   0 root         (0) root         (0)     1586 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/charges_due_date_request.py
+-rw-r--r--   0 root         (0) root         (0)     1374 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/device_1.py
+-rw-r--r--   0 root         (0) root         (0)     2195 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/price_bracket.py
+-rw-r--r--   0 root         (0) root         (0)     3228 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/recipients_transfers_response.py
+-rw-r--r--   0 root         (0) root         (0)     2743 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/pricing_scheme_4.py
+-rw-r--r--   0 root         (0) root         (0)     7715 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/charges_metadata_response.py
+-rw-r--r--   0 root         (0) root         (0)     7713 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/charges_due_date_response.py
+-rw-r--r--   0 root         (0) root         (0)     1781 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_anticipation_limits_response.py
+-rw-r--r--   0 root         (0) root         (0)     1620 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_bank_transfer_payment_request.py
+-rw-r--r--   0 root         (0) root         (0)     3056 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_voucher_payment_request.py
+-rw-r--r--   0 root         (0) root         (0)     1633 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_cancel_subscription_request.py
+-rw-r--r--   0 root         (0) root         (0)     4401 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/subscriptions_items_usages_usage_id_response.py
+-rw-r--r--   0 root         (0) root         (0)     8529 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/invoice.py
+-rw-r--r--   0 root         (0) root         (0)     1627 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_location_request.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/customers_access_tokens_request.py
+-rw-r--r--   0 root         (0) root         (0)     3943 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/bank_account_1.py
+-rw-r--r--   0 root         (0) root         (0)     1432 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/customers_metadata_request.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/subscriptions_billing_date_request.py
+-rw-r--r--   0 root         (0) root         (0)     1834 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/split.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/recipients_default_bank_account_request.py
+-rw-r--r--   0 root         (0) root         (0)     1988 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/list_withdrawals.py
+-rw-r--r--   0 root         (0) root         (0)     1865 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_payment_authentication_request.py
+-rw-r--r--   0 root         (0) root         (0)     1683 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/fine.py
+-rw-r--r--   0 root         (0) root         (0)     1598 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/pix_additional_information.py
+-rw-r--r--   0 root         (0) root         (0)     1637 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/recipients_transfers_request.py
+-rw-r--r--   0 root         (0) root         (0)     2002 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/list_customers_response.py
+-rw-r--r--   0 root         (0) root         (0)     3466 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/submerchant.py
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/update_invoice_status_request.py
+-rw-r--r--   0 root         (0) root         (0)     3789 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_charge_request.py
+-rw-r--r--   0 root         (0) root         (0)     1943 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/usages.py
+-rw-r--r--   0 root         (0) root         (0)     1437 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_checkout_bank_transfer_payment_response.py
+-rw-r--r--   0 root         (0) root         (0)     5259 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/customer.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/tokens_request.py
+-rw-r--r--   0 root         (0) root         (0)     2568 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_card_payment_contactless_request.py
+-rw-r--r--   0 root         (0) root         (0)     2059 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/charges_transactions_response.py
+-rw-r--r--   0 root         (0) root         (0)     2843 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/charges_request.py
+-rw-r--r--   0 root         (0) root         (0)     2553 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/tokens_response.py
+-rw-r--r--   0 root         (0) root         (0)     6757 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_checkout_payment_request.py
+-rw-r--r--   0 root         (0) root         (0)     2237 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_price_bracket_response.py
+-rw-r--r--   0 root         (0) root         (0)     2879 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/threed_secure_1.py
+-rw-r--r--   0 root         (0) root         (0)     6990 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/orders_closed_response.py
+-rw-r--r--   0 root         (0) root         (0)     1376 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/device.py
+-rw-r--r--   0 root         (0) root         (0)     1362 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/bank_transfer.py
+-rw-r--r--   0 root         (0) root         (0)     3993 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_recipient_request.py
+-rw-r--r--   0 root         (0) root         (0)     2051 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/customers_access_tokens_response_1.py
+-rw-r--r--   0 root         (0) root         (0)     1409 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_charges_summary_response.py
+-rw-r--r--   0 root         (0) root         (0)     2938 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_checkout_credit_card_payment_request.py
+-rw-r--r--   0 root         (0) root         (0)     3980 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_bank_account_request.py
+-rw-r--r--   0 root         (0) root         (0)     1643 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/update_current_cycle_end_date_request.py
+-rw-r--r--   0 root         (0) root         (0)     5656 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/customers_addresses_response_1.py
+-rw-r--r--   0 root         (0) root         (0)     1576 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/bank_transfer_2.py
+-rw-r--r--   0 root         (0) root         (0)     2034 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/options_2.py
+-rw-r--r--   0 root         (0) root         (0)     5618 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/billingaddress_3.py
+-rw-r--r--   0 root         (0) root         (0)     1580 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_period_request.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_device_request.py
+-rw-r--r--   0 root         (0) root         (0)     4408 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/subscriptions_discounts_response.py
+-rw-r--r--   0 root         (0) root         (0)     6098 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/credit_card_1.py
+-rw-r--r--   0 root         (0) root         (0)     2042 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/list_subscriptions_response.py
+-rw-r--r--   0 root         (0) root         (0)     2437 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_antifraud_response.py
+-rw-r--r--   0 root         (0) root         (0)     1951 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/debit_card_2.py
+-rw-r--r--   0 root         (0) root         (0)     2013 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_checkout_debit_card_payment_response.py
+-rw-r--r--   0 root         (0) root         (0)     2969 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/subscriptions_items_request.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/update_subscription_split_request.py
+-rw-r--r--   0 root         (0) root         (0)     3556 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_checkout_payment_settings_response.py
+-rw-r--r--   0 root         (0) root         (0)     1520 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/update_subscription_due_days_request.py
+-rw-r--r--   0 root         (0) root         (0)     1527 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/options_1.py
+-rw-r--r--   0 root         (0) root         (0)     1991 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/customers_cards_response_1.py
+-rw-r--r--   0 root         (0) root         (0)     1435 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/recipients_metadata_request.py
+-rw-r--r--   0 root         (0) root         (0)     6121 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/customers_cards_renew_response.py
+-rw-r--r--   0 root         (0) root         (0)     8616 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/subscriptions_partial_invoice_response.py
+-rw-r--r--   0 root         (0) root         (0)     1794 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_transaction_report_file_response.py
+-rw-r--r--   0 root         (0) root         (0)     1898 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_subscription_split_response.py
+-rw-r--r--   0 root         (0) root         (0)     4328 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_usage_response.py
+-rw-r--r--   0 root         (0) root         (0)     7220 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/plans_response_1.py
+-rw-r--r--   0 root         (0) root         (0)     5560 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_bank_account_response.py
+-rw-r--r--   0 root         (0) root         (0)     2663 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/plans_items_request_1.py
+-rw-r--r--   0 root         (0) root         (0)     1722 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/recipients_anticipation_limits_response.py
+-rw-r--r--   0 root         (0) root         (0)     6890 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/recipient.py
+-rw-r--r--   0 root         (0) root         (0)     1420 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/plans_metadata_request.py
+-rw-r--r--   0 root         (0) root         (0)     5222 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_card_request.py
+-rw-r--r--   0 root         (0) root         (0)    11218 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/subscriptions_request_1.py
+-rw-r--r--   0 root         (0) root         (0)     2458 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/subscriptions_increments_request.py
+-rw-r--r--   0 root         (0) root         (0)     5296 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_customer_response.py
+-rw-r--r--   0 root         (0) root         (0)     2394 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/update_recipient_request.py
+-rw-r--r--   0 root         (0) root         (0)     4452 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_plan_item_response.py
+-rw-r--r--   0 root         (0) root         (0)     2000 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/list_anticipation_response.py
+-rw-r--r--   0 root         (0) root         (0)     4094 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/cycle.py
+-rw-r--r--   0 root         (0) root         (0)     2079 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/list_charge_transactions_response.py
+-rw-r--r--   0 root         (0) root         (0)     1417 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/update_current_cycle_status_request.py
+-rw-r--r--   0 root         (0) root         (0)     3306 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_invoice_item_response.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/list_order_response.py
+-rw-r--r--   0 root         (0) root         (0)     3677 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_customer_request.py
+-rw-r--r--   0 root         (0) root         (0)     1419 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_device_response.py
+-rw-r--r--   0 root         (0) root         (0)     4132 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_period_response.py
+-rw-r--r--   0 root         (0) root         (0)     4420 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/subscriptions_increments_response.py
+-rw-r--r--   0 root         (0) root         (0)     2179 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_pix_bank_account_response.py
+-rw-r--r--   0 root         (0) root         (0)     5287 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/customers_response.py
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/location.py
+-rw-r--r--   0 root         (0) root         (0)     2005 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/list_discounts_response.py
+-rw-r--r--   0 root         (0) root         (0)     4097 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/period.py
+-rw-r--r--   0 root         (0) root         (0)    12195 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2439 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_order_item_response.py
+-rw-r--r--   0 root         (0) root         (0)     8601 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/subscriptions_cycles_pay_response.py
+-rw-r--r--   0 root         (0) root         (0)     6974 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/orders_response_1.py
+-rw-r--r--   0 root         (0) root         (0)     2391 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/update_automatic_anticipation_settings_request.py
+-rw-r--r--   0 root         (0) root         (0)     3111 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/update_card_request.py
+-rw-r--r--   0 root         (0) root         (0)     6943 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/order.py
+-rw-r--r--   0 root         (0) root         (0)     2059 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/subscriptions_items_response_3.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_card_options_request.py
+-rw-r--r--   0 root         (0) root         (0)     2116 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_transfer.py
+-rw-r--r--   0 root         (0) root         (0)     2109 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/recipients_anticipations_request.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_emv_data_tlv_decrypt_request.py
+-rw-r--r--   0 root         (0) root         (0)     1904 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/gateway_response.py
+-rw-r--r--   0 root         (0) root         (0)     2333 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/update_charge_card_request.py
+-rw-r--r--   0 root         (0) root         (0)     1656 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_checkout_card_installment_options_response.py
+-rw-r--r--   0 root         (0) root         (0)     6978 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_order_response.py
+-rw-r--r--   0 root         (0) root         (0)     3645 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/customers_request.py
+-rw-r--r--   0 root         (0) root         (0)     1752 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/update_subscription_card_request.py
+-rw-r--r--   0 root         (0) root         (0)     4258 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/private_label.py
+-rw-r--r--   0 root         (0) root         (0)     1448 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/subscriptions_cycles_pay_request.py
+-rw-r--r--   0 root         (0) root         (0)     1444 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/subscriptions_metadata_request.py
+-rw-r--r--   0 root         (0) root         (0)     1970 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/list_plans_response.py
+-rw-r--r--   0 root         (0) root         (0)     4333 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_private_label_payment_request.py
+-rw-r--r--   0 root         (0) root         (0)     3437 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_billing_address_response.py
+-rw-r--r--   0 root         (0) root         (0)     1445 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_clear_sale_request.py
+-rw-r--r--   0 root         (0) root         (0)     3656 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/update_customer_request.py
+-rw-r--r--   0 root         (0) root         (0)     4138 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/recipients_anticipations_response.py
+-rw-r--r--   0 root         (0) root         (0)     1808 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/authentication_2.py
+-rw-r--r--   0 root         (0) root         (0)     8582 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/invoices_metadata_response.py
+-rw-r--r--   0 root         (0) root         (0)     1427 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/clear_sale_request.py
+-rw-r--r--   0 root         (0) root         (0)     2246 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/orders_items_request.py
+-rw-r--r--   0 root         (0) root         (0)     6105 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/customers_cards_response.py
+-rw-r--r--   0 root         (0) root         (0)     3185 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_transfer_response.py
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_transfer_target_response.py
+-rw-r--r--   0 root         (0) root         (0)     4162 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/subscriptions_cycles_response.py
+-rw-r--r--   0 root         (0) root         (0)     2591 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_access_token_response.py
+-rw-r--r--   0 root         (0) root         (0)     1997 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/list_invoices_response.py
+-rw-r--r--   0 root         (0) root         (0)     2069 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/customers_addresses_request_1.py
+-rw-r--r--   0 root         (0) root         (0)     2629 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_emv_decrypt_request.py
+-rw-r--r--   0 root         (0) root         (0)     2385 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/recipients_request_1.py
+-rw-r--r--   0 root         (0) root         (0)     6975 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/recipients_default_bank_account_response.py
+-rw-r--r--   0 root         (0) root         (0)     2862 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/credit_card_2.py
+-rw-r--r--   0 root         (0) root         (0)     6707 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/checkout.py
+-rw-r--r--   0 root         (0) root         (0)     1614 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/subscriptions_gateway_affiliation_id_request.py
+-rw-r--r--   0 root         (0) root         (0)     2744 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_split_response.py
+-rw-r--r--   0 root         (0) root         (0)     5551 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/default_bank_account.py
+-rw-r--r--   0 root         (0) root         (0)     1995 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_phones_request.py
+-rw-r--r--   0 root         (0) root         (0)     2981 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_usages_details_response.py
+-rw-r--r--   0 root         (0) root         (0)     7222 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_plan_response.py
+-rw-r--r--   0 root         (0) root         (0)     2550 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_google_pay_request.py
+-rw-r--r--   0 root         (0) root         (0)     2985 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/update_subscription_item_request.py
+-rw-r--r--   0 root         (0) root         (0)     2027 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/subscriptions_response_3.py
+-rw-r--r--   0 root         (0) root         (0)     4641 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/update_charge_payment_method_request.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_token_request.py
+-rw-r--r--   0 root         (0) root         (0)     2857 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_pricing_scheme_response.py
+-rw-r--r--   0 root         (0) root         (0)     2146 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_pix_payer_response.py
+-rw-r--r--   0 root         (0) root         (0)     2328 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_gateway_recipient_response.py
+-rw-r--r--   0 root         (0) root         (0)     3640 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/customer_8.py
+-rw-r--r--   0 root         (0) root         (0)     1711 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_interest_response.py
+-rw-r--r--   0 root         (0) root         (0)     1948 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/list_transfers.py
+-rw-r--r--   0 root         (0) root         (0)     4612 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/charges_payment_method_request.py
+-rw-r--r--   0 root         (0) root         (0)     6273 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_order_request.py
+-rw-r--r--   0 root         (0) root         (0)     2012 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/setup.py
+-rw-r--r--   0 root         (0) root         (0)    92051 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_transaction_response.py
+-rw-r--r--   0 root         (0) root         (0)     2774 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/recipients_balance_response.py
+-rw-r--r--   0 root         (0) root         (0)     2434 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/orders_items_response_1.py
+-rw-r--r--   0 root         (0) root         (0)     2872 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_cancel_charge_request.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_location_response.py
+-rw-r--r--   0 root         (0) root         (0)     3124 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_card_token_response.py
+-rw-r--r--   0 root         (0) root         (0)     4805 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_boleto_payment_request.py
+-rw-r--r--   0 root         (0) root         (0)     2034 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_checkout_debit_card_payment_request.py
+-rw-r--r--   0 root         (0) root         (0)     6996 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/orders_metadata_response.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/subscriptions_payment_method_request.py
+-rw-r--r--   0 root         (0) root         (0)     3734 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_debit_card_payment_request.py
+-rw-r--r--   0 root         (0) root         (0)     2497 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/charges_capture_request.py
+-rw-r--r--   0 root         (0) root         (0)     1395 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_gateway_error_response.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/list_recipient_response.py
+-rw-r--r--   0 root         (0) root         (0)    11229 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_subscription_request.py
+-rw-r--r--   0 root         (0) root         (0)     2111 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_transfer_settings_request.py
+-rw-r--r--   0 root         (0) root         (0)     1967 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/orders_response.py
+-rw-r--r--   0 root         (0) root         (0)     3785 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/shipping.py
+-rw-r--r--   0 root         (0) root         (0)     2046 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/update_address_request.py
+-rw-r--r--   0 root         (0) root         (0)     4032 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/shipping_3.py
+-rw-r--r--   0 root         (0) root         (0)     1989 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/list_transfer_response.py
+-rw-r--r--   0 root         (0) root         (0)     1653 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_withdraw_request.py
+-rw-r--r--   0 root         (0) root         (0)     2724 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_balance_response.py
+-rw-r--r--   0 root         (0) root         (0)     4378 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/subscriptions_items_usages_response.py
+-rw-r--r--   0 root         (0) root         (0)     1429 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/invoices_metadata_request.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/update_transfer_settings_request.py
+-rw-r--r--   0 root         (0) root         (0)     2015 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/recipients_transfers_response_1.py
+-rw-r--r--   0 root         (0) root         (0)     2000 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/list_usages_details_response.py
+-rw-r--r--   0 root         (0) root         (0)     2134 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/header.py
+-rw-r--r--   0 root         (0) root         (0)     2814 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/pricing_scheme.py
+-rw-r--r--   0 root         (0) root         (0)     1882 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_checkout_boleto_payment_response.py
+-rw-r--r--   0 root         (0) root         (0)     7690 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/charges_response.py
+-rw-r--r--   0 root         (0) root         (0)     2123 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/update_order_item_request.py
+-rw-r--r--   0 root         (0) root         (0)     2690 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/plans_items_request.py
+-rw-r--r--   0 root         (0) root         (0)     3753 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/subscriptions_items_request_1.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/interest.py
+-rw-r--r--   0 root         (0) root         (0)     2918 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_three_d_secure_request.py
+-rw-r--r--   0 root         (0) root         (0)     1989 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/recipients_response.py
+-rw-r--r--   0 root         (0) root         (0)     6468 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_plan_request.py
+-rw-r--r--   0 root         (0) root         (0)     1620 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/update_subscription_affiliation_id_request.py
+-rw-r--r--   0 root         (0) root         (0)     3779 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/charges_request_1.py
+-rw-r--r--   0 root         (0) root         (0)    10486 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_checkout_payment_response.py
+-rw-r--r--   0 root         (0) root         (0)     2256 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_order_item_request.py
+-rw-r--r--   0 root         (0) root         (0)     1419 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/update_metadata_request.py
+-rw-r--r--   0 root         (0) root         (0)     1933 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/setup_1.py
+-rw-r--r--   0 root         (0) root         (0)     2013 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/list_increments_response.py
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_price_bracket_request.py
+-rw-r--r--   0 root         (0) root         (0)     5631 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_address_response.py
+-rw-r--r--   0 root         (0) root         (0)     1828 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_cancel_charge_split_rules_request.py
+-rw-r--r--   0 root         (0) root         (0)     4090 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_anticipation_response.py
+-rw-r--r--   0 root         (0) root         (0)     2393 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/cancel_split_request.py
+-rw-r--r--   0 root         (0) root         (0)     5096 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/update_plan_request.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_anticipation_limit_response.py
+-rw-r--r--   0 root         (0) root         (0)     1788 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/update_subscription_billing_date_request.py
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_withdraw_target_response.py
+-rw-r--r--   0 root         (0) root         (0)     2076 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_split_options_request.py
+-rw-r--r--   0 root         (0) root         (0)     1402 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/update_order_status_request.py
+-rw-r--r--   0 root         (0) root         (0)     2434 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_increment_request.py
+-rw-r--r--   0 root         (0) root         (0)    10537 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_subscription_response.py
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/header_1.py
+-rw-r--r--   0 root         (0) root         (0)     1455 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_access_token_request.py
+-rw-r--r--   0 root         (0) root         (0)     2534 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_token_response.py
+-rw-r--r--   0 root         (0) root         (0)     2033 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/list_transactions_response.py
+-rw-r--r--   0 root         (0) root         (0)     5252 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_transfer.py
+-rw-r--r--   0 root         (0) root         (0)     1935 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_gateway_response_response.py
+-rw-r--r--   0 root         (0) root         (0)     2698 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/update_plan_item_request.py
+-rw-r--r--   0 root         (0) root         (0)     2683 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_checkout_credit_card_payment_response.py
+-rw-r--r--   0 root         (0) root         (0)     2119 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/list_transactions_files_response.py
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/invoices_response_2.py
+-rw-r--r--   0 root         (0) root         (0)     2001 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/list_addresses_response.py
+-rw-r--r--   0 root         (0) root         (0)     2042 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_checkout_boleto_payment_request.py
+-rw-r--r--   0 root         (0) root         (0)     2607 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/customers_access_tokens_response.py
+-rw-r--r--   0 root         (0) root         (0)     2068 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_setup_response.py
+-rw-r--r--   0 root         (0) root         (0)     3662 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_address_request.py
+-rw-r--r--   0 root         (0) root         (0)     3482 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_sub_merchant_request.py
+-rw-r--r--   0 root         (0) root         (0)     2782 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_pricing_scheme_request.py
+-rw-r--r--   0 root         (0) root         (0)     7712 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/charges_capture_response.py
+-rw-r--r--   0 root         (0) root         (0)     1696 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/update_subscription_start_at_request.py
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_transfer_source_response.py
+-rw-r--r--   0 root         (0) root         (0)     1423 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/orders_metadata_request.py
+-rw-r--r--   0 root         (0) root         (0)     3770 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_subscription_item_request.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_transfer_request.py
+-rw-r--r--   0 root         (0) root         (0)     2293 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/update_subscription_payment_method_request.py
+-rw-r--r--   0 root         (0) root         (0)     2668 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_plan_item_request.py
+-rw-r--r--   0 root         (0) root         (0)     2571 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/pix.py
+-rw-r--r--   0 root         (0) root         (0)     3829 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_shipping_response.py
+-rw-r--r--   0 root         (0) root         (0)     7706 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/charges_retry_response.py
+-rw-r--r--   0 root         (0) root         (0)     1553 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/bank_transfer_1.py
+-rw-r--r--   0 root         (0) root         (0)     7731 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/charges_payment_method_response.py
+-rw-r--r--   0 root         (0) root         (0)     5092 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/plans_request_1.py
+-rw-r--r--   0 root         (0) root         (0)     1586 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_google_pay_header_request.py
+-rw-r--r--   0 root         (0) root         (0)     3626 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/address_1.py
+-rw-r--r--   0 root         (0) root         (0)     1504 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/subscriptions_minimum_price_request.py
+-rw-r--r--   0 root         (0) root         (0)     8557 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/invoices_response.py
+-rw-r--r--   0 root         (0) root         (0)     2061 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_setup_request.py
+-rw-r--r--   0 root         (0) root         (0)     5261 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/customers_cards_request.py
+-rw-r--r--   0 root         (0) root         (0)     2013 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_usage_report_response.py
+-rw-r--r--   0 root         (0) root         (0)     1620 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/max.py
+-rw-r--r--   0 root         (0) root         (0)     1426 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/charges_metadata_request.py
+-rw-r--r--   0 root         (0) root         (0)     8576 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/invoices_status_response.py
+-rw-r--r--   0 root         (0) root         (0)     1970 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/list_cards_response.py
+-rw-r--r--   0 root         (0) root         (0)     4390 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_increment_response.py
+-rw-r--r--   0 root         (0) root         (0)     2397 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_emv_data_decrypt_request.py
+-rw-r--r--   0 root         (0) root         (0)     3097 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/update_seller_request.py
+-rw-r--r--   0 root         (0) root         (0)     6089 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_card_response.py
+-rw-r--r--   0 root         (0) root         (0)     2743 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/pricing_scheme_3.py
+-rw-r--r--   0 root         (0) root         (0)     2500 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/apple_pay.py
+-rw-r--r--   0 root         (0) root         (0)     1804 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/authentication.py
+-rw-r--r--   0 root         (0) root         (0)     1989 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_phones_response.py
+-rw-r--r--   0 root         (0) root         (0)     6943 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/recipients_metadata_response.py
+-rw-r--r--   0 root         (0) root         (0)     3665 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/customers_request_1.py
+-rw-r--r--   0 root         (0) root         (0)     2324 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/threed_secure.py
+-rw-r--r--   0 root         (0) root         (0)     2094 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_anticipation_request.py
+-rw-r--r--   0 root         (0) root         (0)     6921 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/recipients_response_1.py
+-rw-r--r--   0 root         (0) root         (0)     2102 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_split_options_response.py
+-rw-r--r--   0 root         (0) root         (0)     2037 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/list_access_tokens_response.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_transfer_settings_response.py
+-rw-r--r--   0 root         (0) root         (0)     6461 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/plans_request.py
+-rw-r--r--   0 root         (0) root         (0)     5530 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/bank_account.py
+-rw-r--r--   0 root         (0) root         (0)     8566 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_invoice_response.py
+-rw-r--r--   0 root         (0) root         (0)     1636 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/subscriptions_periods_latest_end_at_request.py
+-rw-r--r--   0 root         (0) root         (0)     7008 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/recipients_automatic_anticipation_settings_response.py
+-rw-r--r--   0 root         (0) root         (0)     2029 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/subscriptions_cycles_response_2.py
+-rw-r--r--   0 root         (0) root         (0)     1916 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/update_recipient_bank_account_request.py
+-rw-r--r--   0 root         (0) root         (0)     2007 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/list_usages_response.py
+-rw-r--r--   0 root         (0) root         (0)     2420 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_card_payment_contactless_poi_request.py
+-rw-r--r--   0 root         (0) root         (0)     3709 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_seller_response.py
+-rw-r--r--   0 root         (0) root         (0)     2417 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_discount_request.py
+-rw-r--r--   0 root         (0) root         (0)     2724 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_usage_request.py
+-rw-r--r--   0 root         (0) root         (0)     2539 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_apple_pay_request.py
+-rw-r--r--   0 root         (0) root         (0)     6907 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_recipient_response.py
+-rw-r--r--   0 root         (0) root         (0)     2136 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_split_request.py
+-rw-r--r--   0 root         (0) root         (0)     1905 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_phone_response.py
+-rw-r--r--   0 root         (0) root         (0)     2059 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_transaction_report_file_request.py
+-rw-r--r--   0 root         (0) root         (0)     1979 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/charges_response_2.py
+-rw-r--r--   0 root         (0) root         (0)     1700 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_fine_request.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_fine_response.py
+-rw-r--r--   0 root         (0) root         (0)     6049 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/card.py
+-rw-r--r--   0 root         (0) root         (0)     2027 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/subscriptions_items_usages_response_1.py
+-rw-r--r--   0 root         (0) root         (0)     6948 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_payment_request.py
+-rw-r--r--   0 root         (0) root         (0)     7734 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/charges_confirm_payment_response.py
+-rw-r--r--   0 root         (0) root         (0)     3098 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/card_9.py
+-rw-r--r--   0 root         (0) root         (0)     3135 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/customers_cards_request_1.py
+-rw-r--r--   0 root         (0) root         (0)     1418 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_invoice_request.py
+-rw-r--r--   0 root         (0) root         (0)     5270 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_withdraw_response.py
+-rw-r--r--   0 root         (0) root         (0)     2399 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_automatic_anticipation_settings_request.py
+-rw-r--r--   0 root         (0) root         (0)     1960 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/plans_response.py
+-rw-r--r--   0 root         (0) root         (0)     3981 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/recipients_request.py
+-rw-r--r--   0 root         (0) root         (0)     6987 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/orders_items_response.py
+-rw-r--r--   0 root         (0) root         (0)     2705 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/card_11.py
+-rw-r--r--   0 root         (0) root         (0)     7242 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/plans_metadata_response.py
+-rw-r--r--   0 root         (0) root         (0)     6931 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/recipients_code_response.py
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/update_charge_due_date_request.py
+-rw-r--r--   0 root         (0) root         (0)     1404 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_emv_data_dukpt_decrypt_request.py
+-rw-r--r--   0 root         (0) root         (0)     7697 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_charge_response.py
+-rw-r--r--   0 root         (0) root         (0)     1642 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_checkout_card_installment_option_request.py
+-rw-r--r--   0 root         (0) root         (0)     2494 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/contactless.py
+-rw-r--r--   0 root         (0) root         (0)     2784 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_sellers_request.py
+-rw-r--r--   0 root         (0) root         (0)     2125 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/orders_items_request_1.py
+-rw-r--r--   0 root         (0) root         (0)     1988 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/list_charges_response.py
+-rw-r--r--   0 root         (0) root         (0)     1994 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/customers_response_3.py
+-rw-r--r--   0 root         (0) root         (0)     3665 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/debit_card_1.py
+-rw-r--r--   0 root         (0) root         (0)     1855 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_payment_authentication_response.py
+-rw-r--r--   0 root         (0) root         (0)     7662 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/charge.py
+-rw-r--r--   0 root         (0) root         (0)     1716 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_interest_request.py
+-rw-r--r--   0 root         (0) root         (0)     1724 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/subscriptions_card_request.py
+-rw-r--r--   0 root         (0) root         (0)     2010 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/list_cycles_response.py
+-rw-r--r--   0 root         (0) root         (0)     5211 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/card_1.py
+-rw-r--r--   0 root         (0) root         (0)     1640 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_checkout_bank_transfer_request.py
+-rw-r--r--   0 root         (0) root         (0)     6931 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/payment.py
+-rw-r--r--   0 root         (0) root         (0)     2442 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/subscriptions_discounts_request.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/paging.py
+-rw-r--r--   0 root         (0) root         (0)     4446 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/plans_items_response.py
+-rw-r--r--   0 root         (0) root         (0)     2047 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/recipients_anticipations_response_1.py
+-rw-r--r--   0 root         (0) root         (0)     2190 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_apple_pay_header_request.py
+-rw-r--r--   0 root         (0) root         (0)     4731 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/boleto_1.py
+-rw-r--r--   0 root         (0) root         (0)     3964 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/default_bank_account_1.py
+-rw-r--r--   0 root         (0) root         (0)     2624 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/voucher.py
+-rw-r--r--   0 root         (0) root         (0)     2476 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/token.py
+-rw-r--r--   0 root         (0) root         (0)     2198 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/update_price_bracket_request.py
+-rw-r--r--   0 root         (0) root         (0)     5733 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_subscription_item_response.py
+-rw-r--r--   0 root         (0) root         (0)     1832 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_antifraud_request.py
+-rw-r--r--   0 root         (0) root         (0)     5312 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/customers_metadata_response.py
+-rw-r--r--   0 root         (0) root         (0)     7703 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/charges_card_response.py
+-rw-r--r--   0 root         (0) root         (0)     2861 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_seller_request.py
+-rw-r--r--   0 root         (0) root         (0)     2782 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/update_pricing_scheme_request.py
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/paging_response.py
+-rw-r--r--   0 root         (0) root         (0)     4115 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/current_cycle.py
+-rw-r--r--   0 root         (0) root         (0)     3393 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/billing_address.py
+-rw-r--r--   0 root         (0) root         (0)     2074 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/list_subscription_items_response.py
+-rw-r--r--   0 root         (0) root         (0)     1903 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_subscription_split_request.py
+-rw-r--r--   0 root         (0) root         (0)     1911 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_phone_request.py
+-rw-r--r--   0 root         (0) root         (0)     6968 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/recipients_transfer_settings_response.py
+-rw-r--r--   0 root         (0) root         (0)     1620 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/min.py
+-rw-r--r--   0 root         (0) root         (0)     3679 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/customers_addresses_request.py
+-rw-r--r--   0 root         (0) root         (0)     7189 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/plan.py
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_cash_payment_request.py
+-rw-r--r--   0 root         (0) root         (0)     2506 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_capture_charge_request.py
+-rw-r--r--   0 root         (0) root         (0)     2641 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_pix_payment_request.py
+-rw-r--r--   0 root         (0) root         (0)     1526 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/update_subscription_minimum_price_request.py
+-rw-r--r--   0 root         (0) root         (0)     2510 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/google_pay.py
+-rw-r--r--   0 root         (0) root         (0)     1828 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_confirm_payment_request.py
+-rw-r--r--   0 root         (0) root         (0)     1599 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/subscriptions_request.py
+-rw-r--r--   0 root         (0) root         (0)     6168 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_credit_card_payment_request.py
+-rw-r--r--   0 root         (0) root         (0)     5594 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/address.py
+-rw-r--r--   0 root         (0) root         (0)     2369 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_automatic_anticipation_response.py
+-rw-r--r--   0 root         (0) root         (0)     2001 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/list_seller_response.py
+-rw-r--r--   0 root         (0) root         (0)     2015 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/customers_addresses_response.py
+-rw-r--r--   0 root         (0) root         (0)     6264 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/orders_request.py
+-rw-r--r--   0 root         (0) root         (0)     2734 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_card_token_request.py
+-rw-r--r--   0 root         (0) root         (0)     2359 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_three_d_secure_response.py
+-rw-r--r--   0 root         (0) root         (0)     1663 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/subscriptions_start_at_request.py
+-rw-r--r--   0 root         (0) root         (0)     3647 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/billing_address_1.py
+-rw-r--r--   0 root         (0) root         (0)     2324 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/charges_card_request.py
+-rw-r--r--   0 root         (0) root         (0)     4047 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_shipping_request.py
+-rw-r--r--   0 root         (0) root         (0)     2322 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/create_card_payment_token_request.py
+-rw-r--r--   0 root         (0) root         (0)     4377 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_discount_response.py
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/models/get_withdraw_source_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 20:38:28.000000 mundiapi-2.4.3/mundiapi/controllers/
+-rw-r--r--   0 root         (0) root         (0)    36631 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/controllers/charges_controller.py
+-rw-r--r--   0 root         (0) root         (0)    56276 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/controllers/customers_controller.py
+-rw-r--r--   0 root         (0) root         (0)     5995 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/controllers/tokens_controller.py
+-rw-r--r--   0 root         (0) root         (0)     7100 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/controllers/transfers_controller.py
+-rw-r--r--   0 root         (0) root         (0)      321 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   103373 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/controllers/subscriptions_controller.py
+-rw-r--r--   0 root         (0) root         (0)    56785 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/controllers/recipients_controller.py
+-rw-r--r--   0 root         (0) root         (0)     2914 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/controllers/transactions_controller.py
+-rw-r--r--   0 root         (0) root         (0)    20610 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/controllers/invoices_controller.py
+-rw-r--r--   0 root         (0) root         (0)    26680 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/controllers/plans_controller.py
+-rw-r--r--   0 root         (0) root         (0)    26874 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/controllers/orders_controller.py
+-rw-r--r--   0 root         (0) root         (0)     3299 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/controllers/base_controller.py
+-rw-r--r--   0 root         (0) root         (0)    11840 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/controllers/sellers_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 20:38:28.000000 mundiapi-2.4.3/mundiapi/http/
+-rw-r--r--   0 root         (0) root         (0)     3533 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/http/requests_client.py
+-rw-r--r--   0 root         (0) root         (0)      920 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/http/http_method_enum.py
+-rw-r--r--   0 root         (0) root         (0)      181 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/http/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 20:38:28.000000 mundiapi-2.4.3/mundiapi/http/auth/
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/http/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      835 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/http/auth/basic_auth.py
+-rw-r--r--   0 root         (0) root         (0)     2820 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/http/http_request.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/http/http_context.py
+-rw-r--r--   0 root         (0) root         (0)     7088 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/http/http_client.py
+-rw-r--r--   0 root         (0) root         (0)     1115 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/http/http_call_back.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/http/http_response.py
+-rw-r--r--   0 root         (0) root         (0)      509 2023-05-15 20:38:23.000000 mundiapi-2.4.3/mundiapi/decorators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 20:38:28.000000 mundiapi-2.4.3/tests/
+-rw-r--r--   0 root         (0) root         (0)      669 2023-05-15 20:38:23.000000 mundiapi-2.4.3/tests/http_response_catcher.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 20:38:23.000000 mundiapi-2.4.3/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5119 2023-05-15 20:38:23.000000 mundiapi-2.4.3/tests/test_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 20:38:28.000000 mundiapi-2.4.3/tests/controllers/
+-rw-r--r--   0 root         (0) root         (0)     1309 2023-05-15 20:38:23.000000 mundiapi-2.4.3/tests/controllers/test_plans_controller.py
+-rw-r--r--   0 root         (0) root         (0)     1171 2023-05-15 20:38:23.000000 mundiapi-2.4.3/tests/controllers/test_recipients_controller.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 20:38:23.000000 mundiapi-2.4.3/tests/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      963 2023-05-15 20:38:23.000000 mundiapi-2.4.3/tests/controllers/controller_test_base.py
+-rw-r--r--   0 root         (0) root         (0)     1574 2023-05-15 20:38:23.000000 mundiapi-2.4.3/tests/controllers/test_subscriptions_controller.py
+-rw-r--r--   0 root         (0) root         (0)     1055 2023-05-15 20:38:23.000000 mundiapi-2.4.3/tests/controllers/test_transfers_controller.py
+-rw-r--r--   0 root         (0) root         (0)     1501 2023-05-15 20:38:23.000000 mundiapi-2.4.3/tests/controllers/test_invoices_controller.py
+-rw-r--r--   0 root         (0) root         (0)     1254 2023-05-15 20:38:23.000000 mundiapi-2.4.3/tests/controllers/test_customers_controller.py
+-rw-r--r--   0 root         (0) root         (0)     1313 2023-05-15 20:38:23.000000 mundiapi-2.4.3/tests/controllers/test_orders_controller.py
+-rw-r--r--   0 root         (0) root         (0)     1402 2023-05-15 20:38:23.000000 mundiapi-2.4.3/tests/controllers/test_charges_controller.py
+-rw-r--r--   0 root         (0) root         (0)      241 2023-05-15 20:38:28.000000 mundiapi-2.4.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      869 2023-05-15 20:38:27.000000 mundiapi-2.4.3/setup.py
+-rw-r--r--   0 root         (0) root         (0)       59 2023-05-15 20:38:28.000000 mundiapi-2.4.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 20:38:28.000000 mundiapi-2.4.3/mundiapi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      241 2023-05-15 20:38:28.000000 mundiapi-2.4.3/mundiapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    18414 2023-05-15 20:38:28.000000 mundiapi-2.4.3/mundiapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 20:38:28.000000 mundiapi-2.4.3/mundiapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-15 20:38:28.000000 mundiapi-2.4.3/mundiapi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-05-15 20:38:28.000000 mundiapi-2.4.3/mundiapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)   152365 2023-05-15 20:38:23.000000 mundiapi-2.4.3/README.md
```

### Comparing `mundiapi-2.4.2/LICENSE` & `mundiapi-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/mundiapi_client.py` & `mundiapi-2.4.3/mundiapi/mundiapi_client.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/api_helper.py` & `mundiapi-2.4.3/mundiapi/api_helper.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/exceptions/api_exception.py` & `mundiapi-2.4.3/mundiapi/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/exceptions/error_exception.py` & `mundiapi-2.4.3/mundiapi/exceptions/error_exception.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/configuration.py` & `mundiapi-2.4.3/mundiapi/configuration.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/charges_due_date_request.py` & `mundiapi-2.4.3/mundiapi/models/charges_due_date_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/device_1.py` & `mundiapi-2.4.3/mundiapi/models/device_1.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/price_bracket.py` & `mundiapi-2.4.3/mundiapi/models/price_bracket.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/recipients_transfers_response.py` & `mundiapi-2.4.3/mundiapi/models/recipients_transfers_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/pricing_scheme_4.py` & `mundiapi-2.4.3/mundiapi/models/pricing_scheme_4.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/charges_metadata_response.py` & `mundiapi-2.4.3/mundiapi/models/charges_metadata_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/charges_due_date_response.py` & `mundiapi-2.4.3/mundiapi/models/charges_due_date_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_anticipation_limits_response.py` & `mundiapi-2.4.3/mundiapi/models/get_anticipation_limits_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_bank_transfer_payment_request.py` & `mundiapi-2.4.3/mundiapi/models/create_bank_transfer_payment_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_voucher_payment_request.py` & `mundiapi-2.4.3/mundiapi/models/voucher.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,19 @@
     mundiapi
 
     This file was automatically generated by APIMATIC v2.0 ( https://apimatic.io ).
 """
 
 import mundiapi.models.card_1
 
-class CreateVoucherPaymentRequest(object):
+class Voucher(object):
 
-    """Implementation of the 'CreateVoucherPaymentRequest' model.
+    """Implementation of the 'Voucher' model.
 
-    The settings for creating a voucher payment
+    TODO: type model description here.
 
     Attributes:
         statement_descriptor (string): The text that will be shown on the
             voucher's statement
         card_id (string): Card id
         card_token (string): Card token
         card (Card1): TODO: type description here.
@@ -36,15 +36,15 @@
 
     def __init__(self,
                  statement_descriptor=None,
                  card_id=None,
                  card_token=None,
                  card=None,
                  recurrency_cycle=None):
-        """Constructor for the CreateVoucherPaymentRequest class"""
+        """Constructor for the Voucher class"""
 
         # Initialize members of the class
         self.statement_descriptor = statement_descriptor
         self.card_id = card_id
         self.card_token = card_token
         self.card = card
         self.recurrency_cycle = recurrency_cycle
```

### Comparing `mundiapi-2.4.2/mundiapi/models/create_cancel_subscription_request.py` & `mundiapi-2.4.3/mundiapi/models/create_cancel_subscription_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/subscriptions_items_usages_usage_id_response.py` & `mundiapi-2.4.3/mundiapi/models/subscriptions_items_usages_usage_id_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/invoice.py` & `mundiapi-2.4.3/mundiapi/models/invoice.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_location_request.py` & `mundiapi-2.4.3/mundiapi/models/create_location_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/customers_access_tokens_request.py` & `mundiapi-2.4.3/mundiapi/models/customers_access_tokens_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/bank_account_1.py` & `mundiapi-2.4.3/mundiapi/models/bank_account_1.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/customers_metadata_request.py` & `mundiapi-2.4.3/mundiapi/models/customers_metadata_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/subscriptions_billing_date_request.py` & `mundiapi-2.4.3/mundiapi/models/subscriptions_billing_date_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/split.py` & `mundiapi-2.4.3/mundiapi/models/split.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/recipients_default_bank_account_request.py` & `mundiapi-2.4.3/mundiapi/models/recipients_default_bank_account_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/list_withdrawals.py` & `mundiapi-2.4.3/mundiapi/models/list_withdrawals.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_payment_authentication_request.py` & `mundiapi-2.4.3/mundiapi/models/create_payment_authentication_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/fine.py` & `mundiapi-2.4.3/mundiapi/models/fine.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/pix_additional_information.py` & `mundiapi-2.4.3/mundiapi/models/pix_additional_information.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/recipients_transfers_request.py` & `mundiapi-2.4.3/mundiapi/models/recipients_transfers_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/list_customers_response.py` & `mundiapi-2.4.3/mundiapi/models/list_customers_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/submerchant.py` & `mundiapi-2.4.3/mundiapi/models/submerchant.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/update_invoice_status_request.py` & `mundiapi-2.4.3/mundiapi/models/update_invoice_status_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_charge_request.py` & `mundiapi-2.4.3/mundiapi/models/create_charge_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/usages.py` & `mundiapi-2.4.3/mundiapi/models/usages.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_checkout_bank_transfer_payment_response.py` & `mundiapi-2.4.3/mundiapi/models/get_checkout_bank_transfer_payment_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/customer.py` & `mundiapi-2.4.3/mundiapi/models/customer.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/tokens_request.py` & `mundiapi-2.4.3/mundiapi/models/tokens_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_card_payment_contactless_request.py` & `mundiapi-2.4.3/mundiapi/models/create_card_payment_contactless_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/charges_transactions_response.py` & `mundiapi-2.4.3/mundiapi/models/charges_transactions_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/charges_request.py` & `mundiapi-2.4.3/mundiapi/models/charges_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/tokens_response.py` & `mundiapi-2.4.3/mundiapi/models/tokens_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_checkout_payment_request.py` & `mundiapi-2.4.3/mundiapi/models/create_checkout_payment_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_price_bracket_response.py` & `mundiapi-2.4.3/mundiapi/models/get_price_bracket_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/threed_secure_1.py` & `mundiapi-2.4.3/mundiapi/models/threed_secure_1.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/orders_closed_response.py` & `mundiapi-2.4.3/mundiapi/models/orders_closed_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/device.py` & `mundiapi-2.4.3/mundiapi/models/device.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/bank_transfer.py` & `mundiapi-2.4.3/mundiapi/models/bank_transfer.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_recipient_request.py` & `mundiapi-2.4.3/mundiapi/models/create_recipient_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/customers_access_tokens_response_1.py` & `mundiapi-2.4.3/mundiapi/models/customers_access_tokens_response_1.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_charges_summary_response.py` & `mundiapi-2.4.3/mundiapi/models/get_charges_summary_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_checkout_credit_card_payment_request.py` & `mundiapi-2.4.3/mundiapi/models/create_checkout_credit_card_payment_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_bank_account_request.py` & `mundiapi-2.4.3/mundiapi/models/create_bank_account_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/update_current_cycle_end_date_request.py` & `mundiapi-2.4.3/mundiapi/models/update_current_cycle_end_date_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/customers_addresses_response_1.py` & `mundiapi-2.4.3/mundiapi/models/customers_addresses_response_1.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/bank_transfer_2.py` & `mundiapi-2.4.3/mundiapi/models/bank_transfer_2.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/options_2.py` & `mundiapi-2.4.3/mundiapi/models/options_2.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/billingaddress_3.py` & `mundiapi-2.4.3/mundiapi/models/billingaddress_3.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_period_request.py` & `mundiapi-2.4.3/mundiapi/models/create_period_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_device_request.py` & `mundiapi-2.4.3/mundiapi/models/create_device_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/subscriptions_discounts_response.py` & `mundiapi-2.4.3/mundiapi/models/subscriptions_discounts_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/credit_card_1.py` & `mundiapi-2.4.3/mundiapi/models/credit_card_1.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/list_subscriptions_response.py` & `mundiapi-2.4.3/mundiapi/models/list_subscriptions_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_antifraud_response.py` & `mundiapi-2.4.3/mundiapi/models/get_antifraud_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/debit_card_2.py` & `mundiapi-2.4.3/mundiapi/models/debit_card_2.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_checkout_debit_card_payment_response.py` & `mundiapi-2.4.3/mundiapi/models/get_checkout_debit_card_payment_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/subscriptions_items_request.py` & `mundiapi-2.4.3/mundiapi/models/subscriptions_items_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/update_subscription_split_request.py` & `mundiapi-2.4.3/mundiapi/models/update_subscription_split_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_checkout_payment_settings_response.py` & `mundiapi-2.4.3/mundiapi/models/get_checkout_payment_settings_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/update_subscription_due_days_request.py` & `mundiapi-2.4.3/mundiapi/models/update_subscription_due_days_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/options_1.py` & `mundiapi-2.4.3/mundiapi/models/options_1.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/customers_cards_response_1.py` & `mundiapi-2.4.3/mundiapi/models/customers_cards_response_1.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/recipients_metadata_request.py` & `mundiapi-2.4.3/mundiapi/models/recipients_metadata_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/customers_cards_renew_response.py` & `mundiapi-2.4.3/mundiapi/models/customers_cards_renew_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/subscriptions_partial_invoice_response.py` & `mundiapi-2.4.3/mundiapi/models/subscriptions_partial_invoice_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_transaction_report_file_response.py` & `mundiapi-2.4.3/mundiapi/models/get_transaction_report_file_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_subscription_split_response.py` & `mundiapi-2.4.3/mundiapi/models/get_subscription_split_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_usage_response.py` & `mundiapi-2.4.3/mundiapi/models/get_usage_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/plans_response_1.py` & `mundiapi-2.4.3/mundiapi/models/plans_response_1.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_bank_account_response.py` & `mundiapi-2.4.3/mundiapi/models/get_bank_account_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/plans_items_request_1.py` & `mundiapi-2.4.3/mundiapi/models/plans_items_request_1.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/recipients_anticipation_limits_response.py` & `mundiapi-2.4.3/mundiapi/models/recipients_anticipation_limits_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/recipient.py` & `mundiapi-2.4.3/mundiapi/models/recipient.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/plans_metadata_request.py` & `mundiapi-2.4.3/mundiapi/models/plans_metadata_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_card_request.py` & `mundiapi-2.4.3/mundiapi/models/create_card_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/subscriptions_request_1.py` & `mundiapi-2.4.3/mundiapi/models/subscriptions_request_1.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/subscriptions_increments_request.py` & `mundiapi-2.4.3/mundiapi/models/subscriptions_increments_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_customer_response.py` & `mundiapi-2.4.3/mundiapi/models/get_customer_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/update_recipient_request.py` & `mundiapi-2.4.3/mundiapi/models/update_recipient_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_plan_item_response.py` & `mundiapi-2.4.3/mundiapi/models/get_plan_item_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/list_anticipation_response.py` & `mundiapi-2.4.3/mundiapi/models/list_anticipation_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/cycle.py` & `mundiapi-2.4.3/mundiapi/models/cycle.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/list_charge_transactions_response.py` & `mundiapi-2.4.3/mundiapi/models/list_charge_transactions_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/update_current_cycle_status_request.py` & `mundiapi-2.4.3/mundiapi/models/update_current_cycle_status_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_invoice_item_response.py` & `mundiapi-2.4.3/mundiapi/models/get_invoice_item_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/list_order_response.py` & `mundiapi-2.4.3/mundiapi/models/list_order_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_customer_request.py` & `mundiapi-2.4.3/mundiapi/models/create_customer_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_device_response.py` & `mundiapi-2.4.3/mundiapi/models/get_device_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_period_response.py` & `mundiapi-2.4.3/mundiapi/models/get_period_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/subscriptions_increments_response.py` & `mundiapi-2.4.3/mundiapi/models/subscriptions_increments_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_pix_bank_account_response.py` & `mundiapi-2.4.3/mundiapi/models/get_pix_bank_account_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/customers_response.py` & `mundiapi-2.4.3/mundiapi/models/customers_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/location.py` & `mundiapi-2.4.3/mundiapi/models/location.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/list_discounts_response.py` & `mundiapi-2.4.3/mundiapi/models/list_discounts_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/period.py` & `mundiapi-2.4.3/mundiapi/models/period.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/__init__.py` & `mundiapi-2.4.3/mundiapi/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_order_item_response.py` & `mundiapi-2.4.3/mundiapi/models/get_order_item_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/subscriptions_cycles_pay_response.py` & `mundiapi-2.4.3/mundiapi/models/subscriptions_cycles_pay_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/orders_response_1.py` & `mundiapi-2.4.3/mundiapi/models/orders_response_1.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/update_automatic_anticipation_settings_request.py` & `mundiapi-2.4.3/mundiapi/models/update_automatic_anticipation_settings_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/update_card_request.py` & `mundiapi-2.4.3/mundiapi/models/update_card_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/order.py` & `mundiapi-2.4.3/mundiapi/models/order.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/subscriptions_items_response_3.py` & `mundiapi-2.4.3/mundiapi/models/subscriptions_items_response_3.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_card_options_request.py` & `mundiapi-2.4.3/mundiapi/models/create_card_options_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_transfer.py` & `mundiapi-2.4.3/mundiapi/models/create_transfer.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/recipients_anticipations_request.py` & `mundiapi-2.4.3/mundiapi/models/recipients_anticipations_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_emv_data_tlv_decrypt_request.py` & `mundiapi-2.4.3/mundiapi/models/create_emv_data_tlv_decrypt_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/gateway_response.py` & `mundiapi-2.4.3/mundiapi/models/gateway_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/update_charge_card_request.py` & `mundiapi-2.4.3/mundiapi/models/update_charge_card_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_checkout_card_installment_options_response.py` & `mundiapi-2.4.3/mundiapi/models/get_checkout_card_installment_options_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_order_response.py` & `mundiapi-2.4.3/mundiapi/models/get_order_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/customers_request.py` & `mundiapi-2.4.3/mundiapi/models/customers_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/update_subscription_card_request.py` & `mundiapi-2.4.3/mundiapi/models/update_subscription_card_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/private_label.py` & `mundiapi-2.4.3/mundiapi/models/private_label.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/subscriptions_cycles_pay_request.py` & `mundiapi-2.4.3/mundiapi/models/subscriptions_cycles_pay_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/subscriptions_metadata_request.py` & `mundiapi-2.4.3/mundiapi/models/subscriptions_metadata_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/list_plans_response.py` & `mundiapi-2.4.3/mundiapi/models/list_plans_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_private_label_payment_request.py` & `mundiapi-2.4.3/mundiapi/models/create_private_label_payment_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_billing_address_response.py` & `mundiapi-2.4.3/mundiapi/models/get_billing_address_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_clear_sale_request.py` & `mundiapi-2.4.3/mundiapi/models/create_clear_sale_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/update_customer_request.py` & `mundiapi-2.4.3/mundiapi/models/update_customer_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/recipients_anticipations_response.py` & `mundiapi-2.4.3/mundiapi/models/recipients_anticipations_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/authentication_2.py` & `mundiapi-2.4.3/mundiapi/models/authentication_2.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/invoices_metadata_response.py` & `mundiapi-2.4.3/mundiapi/models/invoices_metadata_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/clear_sale_request.py` & `mundiapi-2.4.3/mundiapi/models/clear_sale_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/orders_items_request.py` & `mundiapi-2.4.3/mundiapi/models/orders_items_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/customers_cards_response.py` & `mundiapi-2.4.3/mundiapi/models/customers_cards_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_transfer_response.py` & `mundiapi-2.4.3/mundiapi/models/get_transfer_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_transfer_target_response.py` & `mundiapi-2.4.3/mundiapi/models/get_transfer_target_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/subscriptions_cycles_response.py` & `mundiapi-2.4.3/mundiapi/models/subscriptions_cycles_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_access_token_response.py` & `mundiapi-2.4.3/mundiapi/models/get_access_token_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/list_invoices_response.py` & `mundiapi-2.4.3/mundiapi/models/list_invoices_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/customers_addresses_request_1.py` & `mundiapi-2.4.3/mundiapi/models/customers_addresses_request_1.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_emv_decrypt_request.py` & `mundiapi-2.4.3/mundiapi/models/create_emv_decrypt_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/recipients_request_1.py` & `mundiapi-2.4.3/mundiapi/models/recipients_request_1.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/recipients_default_bank_account_response.py` & `mundiapi-2.4.3/mundiapi/models/recipients_default_bank_account_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/credit_card_2.py` & `mundiapi-2.4.3/mundiapi/models/credit_card_2.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/checkout.py` & `mundiapi-2.4.3/mundiapi/models/checkout.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/subscriptions_gateway_affiliation_id_request.py` & `mundiapi-2.4.3/mundiapi/models/subscriptions_gateway_affiliation_id_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_split_response.py` & `mundiapi-2.4.3/mundiapi/models/get_split_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/default_bank_account.py` & `mundiapi-2.4.3/mundiapi/models/default_bank_account.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_phones_request.py` & `mundiapi-2.4.3/mundiapi/models/create_phones_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_usages_details_response.py` & `mundiapi-2.4.3/mundiapi/models/get_usages_details_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_plan_response.py` & `mundiapi-2.4.3/mundiapi/models/get_plan_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_google_pay_request.py` & `mundiapi-2.4.3/mundiapi/models/create_google_pay_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/update_subscription_item_request.py` & `mundiapi-2.4.3/mundiapi/models/update_subscription_item_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/subscriptions_response_3.py` & `mundiapi-2.4.3/mundiapi/models/subscriptions_response_3.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/update_charge_payment_method_request.py` & `mundiapi-2.4.3/mundiapi/models/update_charge_payment_method_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_token_request.py` & `mundiapi-2.4.3/mundiapi/models/create_token_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_pricing_scheme_response.py` & `mundiapi-2.4.3/mundiapi/models/get_pricing_scheme_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_pix_payer_response.py` & `mundiapi-2.4.3/mundiapi/models/get_pix_payer_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_gateway_recipient_response.py` & `mundiapi-2.4.3/mundiapi/models/get_gateway_recipient_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/customer_8.py` & `mundiapi-2.4.3/mundiapi/models/customer_8.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_interest_response.py` & `mundiapi-2.4.3/mundiapi/models/get_interest_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/list_transfers.py` & `mundiapi-2.4.3/mundiapi/models/list_transfers.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/charges_payment_method_request.py` & `mundiapi-2.4.3/mundiapi/models/charges_payment_method_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_order_request.py` & `mundiapi-2.4.3/mundiapi/models/create_order_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/setup.py` & `mundiapi-2.4.3/mundiapi/models/setup.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_transaction_response.py` & `mundiapi-2.4.3/mundiapi/models/get_transaction_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/recipients_balance_response.py` & `mundiapi-2.4.3/mundiapi/models/recipients_balance_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/orders_items_response_1.py` & `mundiapi-2.4.3/mundiapi/models/orders_items_response_1.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_cancel_charge_request.py` & `mundiapi-2.4.3/mundiapi/models/create_cancel_charge_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_location_response.py` & `mundiapi-2.4.3/mundiapi/models/get_location_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_card_token_response.py` & `mundiapi-2.4.3/mundiapi/models/get_card_token_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_boleto_payment_request.py` & `mundiapi-2.4.3/mundiapi/models/create_boleto_payment_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_checkout_debit_card_payment_request.py` & `mundiapi-2.4.3/mundiapi/models/create_checkout_debit_card_payment_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/orders_metadata_response.py` & `mundiapi-2.4.3/mundiapi/models/orders_metadata_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/subscriptions_payment_method_request.py` & `mundiapi-2.4.3/mundiapi/models/subscriptions_payment_method_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_debit_card_payment_request.py` & `mundiapi-2.4.3/mundiapi/models/create_debit_card_payment_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/charges_capture_request.py` & `mundiapi-2.4.3/mundiapi/models/charges_capture_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_gateway_error_response.py` & `mundiapi-2.4.3/mundiapi/models/get_gateway_error_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/list_recipient_response.py` & `mundiapi-2.4.3/mundiapi/models/list_recipient_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_subscription_request.py` & `mundiapi-2.4.3/mundiapi/models/create_subscription_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_transfer_settings_request.py` & `mundiapi-2.4.3/mundiapi/models/create_transfer_settings_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/orders_response.py` & `mundiapi-2.4.3/mundiapi/models/orders_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/shipping.py` & `mundiapi-2.4.3/mundiapi/models/shipping.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/update_address_request.py` & `mundiapi-2.4.3/mundiapi/models/update_address_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/shipping_3.py` & `mundiapi-2.4.3/mundiapi/models/shipping_3.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/list_transfer_response.py` & `mundiapi-2.4.3/mundiapi/models/list_transfer_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_withdraw_request.py` & `mundiapi-2.4.3/mundiapi/models/create_withdraw_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_balance_response.py` & `mundiapi-2.4.3/mundiapi/models/get_balance_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/subscriptions_items_usages_response.py` & `mundiapi-2.4.3/mundiapi/models/subscriptions_items_usages_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/invoices_metadata_request.py` & `mundiapi-2.4.3/mundiapi/models/invoices_metadata_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/update_transfer_settings_request.py` & `mundiapi-2.4.3/mundiapi/models/update_transfer_settings_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/recipients_transfers_response_1.py` & `mundiapi-2.4.3/mundiapi/models/recipients_transfers_response_1.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/list_usages_details_response.py` & `mundiapi-2.4.3/mundiapi/models/list_usages_details_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/header.py` & `mundiapi-2.4.3/mundiapi/models/header.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/pricing_scheme.py` & `mundiapi-2.4.3/mundiapi/models/pricing_scheme.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_checkout_boleto_payment_response.py` & `mundiapi-2.4.3/mundiapi/models/get_checkout_boleto_payment_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/charges_response.py` & `mundiapi-2.4.3/mundiapi/models/charges_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/update_order_item_request.py` & `mundiapi-2.4.3/mundiapi/models/update_order_item_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/plans_items_request.py` & `mundiapi-2.4.3/mundiapi/models/plans_items_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/subscriptions_items_request_1.py` & `mundiapi-2.4.3/mundiapi/models/subscriptions_items_request_1.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/interest.py` & `mundiapi-2.4.3/mundiapi/models/interest.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_three_d_secure_request.py` & `mundiapi-2.4.3/mundiapi/models/create_three_d_secure_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/recipients_response.py` & `mundiapi-2.4.3/mundiapi/models/recipients_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_plan_request.py` & `mundiapi-2.4.3/mundiapi/models/create_plan_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/update_subscription_affiliation_id_request.py` & `mundiapi-2.4.3/mundiapi/models/update_subscription_affiliation_id_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/charges_request_1.py` & `mundiapi-2.4.3/mundiapi/models/charges_request_1.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_checkout_payment_response.py` & `mundiapi-2.4.3/mundiapi/models/get_checkout_payment_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_order_item_request.py` & `mundiapi-2.4.3/mundiapi/models/create_order_item_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/update_metadata_request.py` & `mundiapi-2.4.3/mundiapi/models/update_metadata_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/setup_1.py` & `mundiapi-2.4.3/mundiapi/models/setup_1.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/list_increments_response.py` & `mundiapi-2.4.3/mundiapi/models/list_increments_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_price_bracket_request.py` & `mundiapi-2.4.3/mundiapi/models/create_price_bracket_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_address_response.py` & `mundiapi-2.4.3/mundiapi/models/get_address_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_cancel_charge_split_rules_request.py` & `mundiapi-2.4.3/mundiapi/models/create_cancel_charge_split_rules_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_anticipation_response.py` & `mundiapi-2.4.3/mundiapi/models/get_anticipation_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/cancel_split_request.py` & `mundiapi-2.4.3/mundiapi/models/cancel_split_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/update_plan_request.py` & `mundiapi-2.4.3/mundiapi/models/update_plan_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_anticipation_limit_response.py` & `mundiapi-2.4.3/mundiapi/models/get_anticipation_limit_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/update_subscription_billing_date_request.py` & `mundiapi-2.4.3/mundiapi/models/update_subscription_billing_date_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_withdraw_target_response.py` & `mundiapi-2.4.3/mundiapi/models/get_withdraw_target_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_split_options_request.py` & `mundiapi-2.4.3/mundiapi/models/create_split_options_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/update_order_status_request.py` & `mundiapi-2.4.3/mundiapi/models/update_order_status_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_increment_request.py` & `mundiapi-2.4.3/mundiapi/models/create_increment_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_subscription_response.py` & `mundiapi-2.4.3/mundiapi/models/get_subscription_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/header_1.py` & `mundiapi-2.4.3/mundiapi/models/header_1.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_access_token_request.py` & `mundiapi-2.4.3/mundiapi/models/create_access_token_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_token_response.py` & `mundiapi-2.4.3/mundiapi/models/get_token_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/list_transactions_response.py` & `mundiapi-2.4.3/mundiapi/models/list_transactions_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_transfer.py` & `mundiapi-2.4.3/mundiapi/models/get_transfer.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_gateway_response_response.py` & `mundiapi-2.4.3/mundiapi/models/get_gateway_response_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/update_plan_item_request.py` & `mundiapi-2.4.3/mundiapi/models/update_plan_item_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_checkout_credit_card_payment_response.py` & `mundiapi-2.4.3/mundiapi/models/get_checkout_credit_card_payment_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/list_transactions_files_response.py` & `mundiapi-2.4.3/mundiapi/models/list_transactions_files_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/invoices_response_2.py` & `mundiapi-2.4.3/mundiapi/models/invoices_response_2.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/list_addresses_response.py` & `mundiapi-2.4.3/mundiapi/models/list_addresses_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_checkout_boleto_payment_request.py` & `mundiapi-2.4.3/mundiapi/models/create_checkout_boleto_payment_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/customers_access_tokens_response.py` & `mundiapi-2.4.3/mundiapi/models/customers_access_tokens_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_setup_response.py` & `mundiapi-2.4.3/mundiapi/models/get_setup_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_address_request.py` & `mundiapi-2.4.3/mundiapi/models/create_address_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_sub_merchant_request.py` & `mundiapi-2.4.3/mundiapi/models/create_sub_merchant_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_pricing_scheme_request.py` & `mundiapi-2.4.3/mundiapi/models/create_pricing_scheme_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/charges_capture_response.py` & `mundiapi-2.4.3/mundiapi/models/charges_capture_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/update_subscription_start_at_request.py` & `mundiapi-2.4.3/mundiapi/models/update_subscription_start_at_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_transfer_source_response.py` & `mundiapi-2.4.3/mundiapi/models/get_transfer_source_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/orders_metadata_request.py` & `mundiapi-2.4.3/mundiapi/models/orders_metadata_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_subscription_item_request.py` & `mundiapi-2.4.3/mundiapi/models/create_subscription_item_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_transfer_request.py` & `mundiapi-2.4.3/mundiapi/models/create_transfer_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/update_subscription_payment_method_request.py` & `mundiapi-2.4.3/mundiapi/models/update_subscription_payment_method_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_plan_item_request.py` & `mundiapi-2.4.3/mundiapi/models/create_plan_item_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/pix.py` & `mundiapi-2.4.3/mundiapi/models/pix.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_shipping_response.py` & `mundiapi-2.4.3/mundiapi/models/get_shipping_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/charges_retry_response.py` & `mundiapi-2.4.3/mundiapi/models/charges_retry_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/bank_transfer_1.py` & `mundiapi-2.4.3/mundiapi/models/bank_transfer_1.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/charges_payment_method_response.py` & `mundiapi-2.4.3/mundiapi/models/charges_payment_method_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/plans_request_1.py` & `mundiapi-2.4.3/mundiapi/models/plans_request_1.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_google_pay_header_request.py` & `mundiapi-2.4.3/mundiapi/models/create_google_pay_header_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/address_1.py` & `mundiapi-2.4.3/mundiapi/models/address_1.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/subscriptions_minimum_price_request.py` & `mundiapi-2.4.3/mundiapi/models/subscriptions_minimum_price_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/invoices_response.py` & `mundiapi-2.4.3/mundiapi/models/invoices_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_setup_request.py` & `mundiapi-2.4.3/mundiapi/models/create_setup_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/customers_cards_request.py` & `mundiapi-2.4.3/mundiapi/models/customers_cards_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_usage_report_response.py` & `mundiapi-2.4.3/mundiapi/models/get_usage_report_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/max.py` & `mundiapi-2.4.3/mundiapi/models/max.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/charges_metadata_request.py` & `mundiapi-2.4.3/mundiapi/models/charges_metadata_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/invoices_status_response.py` & `mundiapi-2.4.3/mundiapi/models/invoices_status_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/list_cards_response.py` & `mundiapi-2.4.3/mundiapi/models/list_cards_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_increment_response.py` & `mundiapi-2.4.3/mundiapi/models/get_increment_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_emv_data_decrypt_request.py` & `mundiapi-2.4.3/mundiapi/models/create_emv_data_decrypt_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/update_seller_request.py` & `mundiapi-2.4.3/mundiapi/models/update_seller_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_card_response.py` & `mundiapi-2.4.3/mundiapi/models/get_card_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/pricing_scheme_3.py` & `mundiapi-2.4.3/mundiapi/models/pricing_scheme_3.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/apple_pay.py` & `mundiapi-2.4.3/mundiapi/models/apple_pay.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/authentication.py` & `mundiapi-2.4.3/mundiapi/models/authentication.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_phones_response.py` & `mundiapi-2.4.3/mundiapi/models/get_phones_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/recipients_metadata_response.py` & `mundiapi-2.4.3/mundiapi/models/recipients_metadata_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/customers_request_1.py` & `mundiapi-2.4.3/mundiapi/models/customers_request_1.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/threed_secure.py` & `mundiapi-2.4.3/mundiapi/models/threed_secure.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_anticipation_request.py` & `mundiapi-2.4.3/mundiapi/models/create_anticipation_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/recipients_response_1.py` & `mundiapi-2.4.3/mundiapi/models/recipients_response_1.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_split_options_response.py` & `mundiapi-2.4.3/mundiapi/models/get_split_options_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/list_access_tokens_response.py` & `mundiapi-2.4.3/mundiapi/models/list_access_tokens_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_transfer_settings_response.py` & `mundiapi-2.4.3/mundiapi/models/get_transfer_settings_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/plans_request.py` & `mundiapi-2.4.3/mundiapi/models/plans_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/bank_account.py` & `mundiapi-2.4.3/mundiapi/models/bank_account.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_invoice_response.py` & `mundiapi-2.4.3/mundiapi/models/get_invoice_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/subscriptions_periods_latest_end_at_request.py` & `mundiapi-2.4.3/mundiapi/models/subscriptions_periods_latest_end_at_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/recipients_automatic_anticipation_settings_response.py` & `mundiapi-2.4.3/mundiapi/models/recipients_automatic_anticipation_settings_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/subscriptions_cycles_response_2.py` & `mundiapi-2.4.3/mundiapi/models/subscriptions_cycles_response_2.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/update_recipient_bank_account_request.py` & `mundiapi-2.4.3/mundiapi/models/update_recipient_bank_account_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/list_usages_response.py` & `mundiapi-2.4.3/mundiapi/models/list_usages_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_card_payment_contactless_poi_request.py` & `mundiapi-2.4.3/mundiapi/models/create_card_payment_contactless_poi_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_seller_response.py` & `mundiapi-2.4.3/mundiapi/models/get_seller_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_discount_request.py` & `mundiapi-2.4.3/mundiapi/models/create_discount_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_usage_request.py` & `mundiapi-2.4.3/mundiapi/models/create_usage_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_apple_pay_request.py` & `mundiapi-2.4.3/mundiapi/models/create_apple_pay_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_recipient_response.py` & `mundiapi-2.4.3/mundiapi/models/get_recipient_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_split_request.py` & `mundiapi-2.4.3/mundiapi/models/create_split_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_phone_response.py` & `mundiapi-2.4.3/mundiapi/models/get_phone_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_transaction_report_file_request.py` & `mundiapi-2.4.3/mundiapi/models/create_transaction_report_file_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/charges_response_2.py` & `mundiapi-2.4.3/mundiapi/models/charges_response_2.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_fine_request.py` & `mundiapi-2.4.3/mundiapi/models/create_fine_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_fine_response.py` & `mundiapi-2.4.3/mundiapi/models/get_fine_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/card.py` & `mundiapi-2.4.3/mundiapi/models/card.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/subscriptions_items_usages_response_1.py` & `mundiapi-2.4.3/mundiapi/models/subscriptions_items_usages_response_1.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_payment_request.py` & `mundiapi-2.4.3/mundiapi/models/create_payment_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/charges_confirm_payment_response.py` & `mundiapi-2.4.3/mundiapi/models/charges_confirm_payment_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/card_9.py` & `mundiapi-2.4.3/mundiapi/models/card_9.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/customers_cards_request_1.py` & `mundiapi-2.4.3/mundiapi/models/customers_cards_request_1.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_invoice_request.py` & `mundiapi-2.4.3/mundiapi/models/create_invoice_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_withdraw_response.py` & `mundiapi-2.4.3/mundiapi/models/get_withdraw_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_automatic_anticipation_settings_request.py` & `mundiapi-2.4.3/mundiapi/models/create_automatic_anticipation_settings_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/plans_response.py` & `mundiapi-2.4.3/mundiapi/models/plans_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/recipients_request.py` & `mundiapi-2.4.3/mundiapi/models/recipients_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/orders_items_response.py` & `mundiapi-2.4.3/mundiapi/models/orders_items_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/card_11.py` & `mundiapi-2.4.3/mundiapi/models/card_11.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/plans_metadata_response.py` & `mundiapi-2.4.3/mundiapi/models/plans_metadata_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/recipients_code_response.py` & `mundiapi-2.4.3/mundiapi/models/recipients_code_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/update_charge_due_date_request.py` & `mundiapi-2.4.3/mundiapi/models/update_charge_due_date_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_emv_data_dukpt_decrypt_request.py` & `mundiapi-2.4.3/mundiapi/models/create_emv_data_dukpt_decrypt_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_charge_response.py` & `mundiapi-2.4.3/mundiapi/models/get_charge_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_checkout_card_installment_option_request.py` & `mundiapi-2.4.3/mundiapi/models/create_checkout_card_installment_option_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/contactless.py` & `mundiapi-2.4.3/mundiapi/models/contactless.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_sellers_request.py` & `mundiapi-2.4.3/mundiapi/models/get_sellers_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/orders_items_request_1.py` & `mundiapi-2.4.3/mundiapi/models/orders_items_request_1.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/list_charges_response.py` & `mundiapi-2.4.3/mundiapi/models/list_charges_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/customers_response_3.py` & `mundiapi-2.4.3/mundiapi/models/customers_response_3.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/debit_card_1.py` & `mundiapi-2.4.3/mundiapi/models/debit_card_1.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_payment_authentication_response.py` & `mundiapi-2.4.3/mundiapi/models/get_payment_authentication_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/charge.py` & `mundiapi-2.4.3/mundiapi/models/charge.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_interest_request.py` & `mundiapi-2.4.3/mundiapi/models/create_interest_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/subscriptions_card_request.py` & `mundiapi-2.4.3/mundiapi/models/subscriptions_card_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/list_cycles_response.py` & `mundiapi-2.4.3/mundiapi/models/list_cycles_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/card_1.py` & `mundiapi-2.4.3/mundiapi/models/card_1.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_checkout_bank_transfer_request.py` & `mundiapi-2.4.3/mundiapi/models/create_checkout_bank_transfer_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/payment.py` & `mundiapi-2.4.3/mundiapi/models/payment.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/subscriptions_discounts_request.py` & `mundiapi-2.4.3/mundiapi/models/subscriptions_discounts_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/paging.py` & `mundiapi-2.4.3/mundiapi/models/paging.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/plans_items_response.py` & `mundiapi-2.4.3/mundiapi/models/plans_items_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/recipients_anticipations_response_1.py` & `mundiapi-2.4.3/mundiapi/models/recipients_anticipations_response_1.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_apple_pay_header_request.py` & `mundiapi-2.4.3/mundiapi/models/create_apple_pay_header_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/boleto_1.py` & `mundiapi-2.4.3/mundiapi/models/boleto_1.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/default_bank_account_1.py` & `mundiapi-2.4.3/mundiapi/models/default_bank_account_1.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/voucher.py` & `mundiapi-2.4.3/mundiapi/models/billing_address.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,56 +2,73 @@
 
 """
     mundiapi
 
     This file was automatically generated by APIMATIC v2.0 ( https://apimatic.io ).
 """
 
-import mundiapi.models.card_1
 
-class Voucher(object):
+class BillingAddress(object):
 
-    """Implementation of the 'Voucher' model.
+    """Implementation of the 'BillingAddress' model.
 
     TODO: type model description here.
 
     Attributes:
-        statement_descriptor (string): The text that will be shown on the
-            voucher's statement
-        card_id (string): Card id
-        card_token (string): Card token
-        card (Card1): TODO: type description here.
-        recurrency_cycle (string): Defines whether the card has been used one
-            or more times.
+        street (string): TODO: type description here.
+        number (string): TODO: type description here.
+        zip_code (string): TODO: type description here.
+        neighborhood (string): TODO: type description here.
+        city (string): TODO: type description here.
+        state (string): TODO: type description here.
+        country (string): TODO: type description here.
+        complement (string): TODO: type description here.
+        line_1 (string): Line 1 for address
+        line_2 (string): Line 2 for address
 
     """
 
     # Create a mapping from Model property names to API property names
     _names = {
-        "statement_descriptor":'statement_descriptor',
-        "card_id":'card_id',
-        "card_token":'card_token',
-        "card":'Card',
-        "recurrency_cycle":'recurrency_cycle'
+        "street":'street',
+        "number":'number',
+        "zip_code":'zip_code',
+        "neighborhood":'neighborhood',
+        "city":'city',
+        "state":'state',
+        "country":'country',
+        "complement":'complement',
+        "line_1":'line_1',
+        "line_2":'line_2'
     }
 
     def __init__(self,
-                 statement_descriptor=None,
-                 card_id=None,
-                 card_token=None,
-                 card=None,
-                 recurrency_cycle=None):
-        """Constructor for the Voucher class"""
+                 street=None,
+                 number=None,
+                 zip_code=None,
+                 neighborhood=None,
+                 city=None,
+                 state=None,
+                 country=None,
+                 complement=None,
+                 line_1=None,
+                 line_2=None):
+        """Constructor for the BillingAddress class"""
 
         # Initialize members of the class
-        self.statement_descriptor = statement_descriptor
-        self.card_id = card_id
-        self.card_token = card_token
-        self.card = card
-        self.recurrency_cycle = recurrency_cycle
+        self.street = street
+        self.number = number
+        self.zip_code = zip_code
+        self.neighborhood = neighborhood
+        self.city = city
+        self.state = state
+        self.country = country
+        self.complement = complement
+        self.line_1 = line_1
+        self.line_2 = line_2
 
 
     @classmethod
     def from_dictionary(cls,
                         dictionary):
         """Creates an instance of this model from a dictionary
 
@@ -64,21 +81,31 @@
             object: An instance of this structure class.
 
         """
         if dictionary is None:
             return None
 
         # Extract variables from the dictionary
-        statement_descriptor = dictionary.get('statement_descriptor')
-        card_id = dictionary.get('card_id')
-        card_token = dictionary.get('card_token')
-        card = mundiapi.models.card_1.Card1.from_dictionary(dictionary.get('Card')) if dictionary.get('Card') else None
-        recurrency_cycle = dictionary.get('recurrency_cycle')
+        street = dictionary.get('street')
+        number = dictionary.get('number')
+        zip_code = dictionary.get('zip_code')
+        neighborhood = dictionary.get('neighborhood')
+        city = dictionary.get('city')
+        state = dictionary.get('state')
+        country = dictionary.get('country')
+        complement = dictionary.get('complement')
+        line_1 = dictionary.get('line_1')
+        line_2 = dictionary.get('line_2')
 
         # Return an object of this model
-        return cls(statement_descriptor,
-                   card_id,
-                   card_token,
-                   card,
-                   recurrency_cycle)
+        return cls(street,
+                   number,
+                   zip_code,
+                   neighborhood,
+                   city,
+                   state,
+                   country,
+                   complement,
+                   line_1,
+                   line_2)
```

### Comparing `mundiapi-2.4.2/mundiapi/models/token.py` & `mundiapi-2.4.3/mundiapi/models/token.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/update_price_bracket_request.py` & `mundiapi-2.4.3/mundiapi/models/update_price_bracket_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_subscription_item_response.py` & `mundiapi-2.4.3/mundiapi/models/get_subscription_item_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_antifraud_request.py` & `mundiapi-2.4.3/mundiapi/models/create_antifraud_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/customers_metadata_response.py` & `mundiapi-2.4.3/mundiapi/models/customers_metadata_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/charges_card_response.py` & `mundiapi-2.4.3/mundiapi/models/charges_card_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_seller_request.py` & `mundiapi-2.4.3/mundiapi/models/create_seller_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/update_pricing_scheme_request.py` & `mundiapi-2.4.3/mundiapi/models/update_pricing_scheme_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/paging_response.py` & `mundiapi-2.4.3/mundiapi/models/paging_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/current_cycle.py` & `mundiapi-2.4.3/mundiapi/models/current_cycle.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/billing_address.py` & `mundiapi-2.4.3/mundiapi/models/billing_address_1.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,29 +3,32 @@
 """
     mundiapi
 
     This file was automatically generated by APIMATIC v2.0 ( https://apimatic.io ).
 """
 
 
-class BillingAddress(object):
+class BillingAddress1(object):
 
-    """Implementation of the 'BillingAddress' model.
+    """Implementation of the 'BillingAddress1' model.
 
     TODO: type model description here.
 
     Attributes:
-        street (string): TODO: type description here.
-        number (string): TODO: type description here.
-        zip_code (string): TODO: type description here.
-        neighborhood (string): TODO: type description here.
-        city (string): TODO: type description here.
-        state (string): TODO: type description here.
-        country (string): TODO: type description here.
-        complement (string): TODO: type description here.
+        street (string): Street
+        number (string): Number
+        zip_code (string): The zip code containing only numbers. No special
+            characters or spaces.
+        neighborhood (string): Neighborhood
+        city (string): City
+        state (string): State
+        country (string): Country. Must be entered using ISO 3166-1 alpha-2
+            format. See https://pt.wikipedia.org/wiki/ISO_3166-1_alfa-2
+        complement (string): Complement
+        metadata (dict<object, string>): Metadata
         line_1 (string): Line 1 for address
         line_2 (string): Line 2 for address
 
     """
 
     # Create a mapping from Model property names to API property names
     _names = {
@@ -33,40 +36,43 @@
         "number":'number',
         "zip_code":'zip_code',
         "neighborhood":'neighborhood',
         "city":'city',
         "state":'state',
         "country":'country',
         "complement":'complement',
+        "metadata":'metadata',
         "line_1":'line_1',
         "line_2":'line_2'
     }
 
     def __init__(self,
                  street=None,
                  number=None,
                  zip_code=None,
                  neighborhood=None,
                  city=None,
                  state=None,
                  country=None,
                  complement=None,
+                 metadata=None,
                  line_1=None,
                  line_2=None):
-        """Constructor for the BillingAddress class"""
+        """Constructor for the BillingAddress1 class"""
 
         # Initialize members of the class
         self.street = street
         self.number = number
         self.zip_code = zip_code
         self.neighborhood = neighborhood
         self.city = city
         self.state = state
         self.country = country
         self.complement = complement
+        self.metadata = metadata
         self.line_1 = line_1
         self.line_2 = line_2
 
 
     @classmethod
     def from_dictionary(cls,
                         dictionary):
@@ -89,23 +95,25 @@
         number = dictionary.get('number')
         zip_code = dictionary.get('zip_code')
         neighborhood = dictionary.get('neighborhood')
         city = dictionary.get('city')
         state = dictionary.get('state')
         country = dictionary.get('country')
         complement = dictionary.get('complement')
+        metadata = dictionary.get('metadata')
         line_1 = dictionary.get('line_1')
         line_2 = dictionary.get('line_2')
 
         # Return an object of this model
         return cls(street,
                    number,
                    zip_code,
                    neighborhood,
                    city,
                    state,
                    country,
                    complement,
+                   metadata,
                    line_1,
                    line_2)
```

### Comparing `mundiapi-2.4.2/mundiapi/models/list_subscription_items_response.py` & `mundiapi-2.4.3/mundiapi/models/list_subscription_items_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_subscription_split_request.py` & `mundiapi-2.4.3/mundiapi/models/create_subscription_split_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_phone_request.py` & `mundiapi-2.4.3/mundiapi/models/create_phone_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/recipients_transfer_settings_response.py` & `mundiapi-2.4.3/mundiapi/models/recipients_transfer_settings_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/min.py` & `mundiapi-2.4.3/mundiapi/models/min.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/customers_addresses_request.py` & `mundiapi-2.4.3/mundiapi/models/customers_addresses_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/plan.py` & `mundiapi-2.4.3/mundiapi/models/plan.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_cash_payment_request.py` & `mundiapi-2.4.3/mundiapi/models/create_cash_payment_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_capture_charge_request.py` & `mundiapi-2.4.3/mundiapi/models/create_capture_charge_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_pix_payment_request.py` & `mundiapi-2.4.3/mundiapi/models/create_pix_payment_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/update_subscription_minimum_price_request.py` & `mundiapi-2.4.3/mundiapi/models/update_subscription_minimum_price_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/google_pay.py` & `mundiapi-2.4.3/mundiapi/models/google_pay.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_confirm_payment_request.py` & `mundiapi-2.4.3/mundiapi/models/create_confirm_payment_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/subscriptions_request.py` & `mundiapi-2.4.3/mundiapi/models/subscriptions_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_credit_card_payment_request.py` & `mundiapi-2.4.3/mundiapi/models/create_credit_card_payment_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/address.py` & `mundiapi-2.4.3/mundiapi/models/address.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_automatic_anticipation_response.py` & `mundiapi-2.4.3/mundiapi/models/get_automatic_anticipation_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/list_seller_response.py` & `mundiapi-2.4.3/mundiapi/models/list_seller_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/customers_addresses_response.py` & `mundiapi-2.4.3/mundiapi/models/customers_addresses_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/orders_request.py` & `mundiapi-2.4.3/mundiapi/models/orders_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_card_token_request.py` & `mundiapi-2.4.3/mundiapi/models/create_card_token_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_three_d_secure_response.py` & `mundiapi-2.4.3/mundiapi/models/get_three_d_secure_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/subscriptions_start_at_request.py` & `mundiapi-2.4.3/mundiapi/models/subscriptions_start_at_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/charges_card_request.py` & `mundiapi-2.4.3/mundiapi/models/charges_card_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_shipping_request.py` & `mundiapi-2.4.3/mundiapi/models/create_shipping_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/create_card_payment_token_request.py` & `mundiapi-2.4.3/mundiapi/models/create_card_payment_token_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_discount_response.py` & `mundiapi-2.4.3/mundiapi/models/get_discount_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/models/get_withdraw_source_response.py` & `mundiapi-2.4.3/mundiapi/models/get_withdraw_source_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/controllers/charges_controller.py` & `mundiapi-2.4.3/mundiapi/controllers/charges_controller.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/controllers/customers_controller.py` & `mundiapi-2.4.3/mundiapi/controllers/customers_controller.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/controllers/tokens_controller.py` & `mundiapi-2.4.3/mundiapi/controllers/tokens_controller.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/controllers/transfers_controller.py` & `mundiapi-2.4.3/mundiapi/controllers/transfers_controller.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/controllers/subscriptions_controller.py` & `mundiapi-2.4.3/mundiapi/controllers/subscriptions_controller.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/controllers/recipients_controller.py` & `mundiapi-2.4.3/mundiapi/controllers/recipients_controller.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/controllers/transactions_controller.py` & `mundiapi-2.4.3/mundiapi/controllers/transactions_controller.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/controllers/invoices_controller.py` & `mundiapi-2.4.3/mundiapi/controllers/invoices_controller.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/controllers/plans_controller.py` & `mundiapi-2.4.3/mundiapi/controllers/plans_controller.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/controllers/orders_controller.py` & `mundiapi-2.4.3/mundiapi/controllers/orders_controller.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/controllers/base_controller.py` & `mundiapi-2.4.3/mundiapi/controllers/base_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     """
 
     http_client = RequestsClient()
 
     http_call_back = None
 
     global_headers = {
-        'user-agent': 'MundiSDK - Python 2.4.2'
+        'user-agent': 'MundiSDK - Python 2.4.3'
     }
 
     def __init__(self, client=None, call_back=None):
         if client != None:
             self.http_client = client
         if call_back != None:
             self.http_call_back = call_back
```

### Comparing `mundiapi-2.4.2/mundiapi/controllers/sellers_controller.py` & `mundiapi-2.4.3/mundiapi/controllers/sellers_controller.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/http/requests_client.py` & `mundiapi-2.4.3/mundiapi/http/requests_client.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/http/http_method_enum.py` & `mundiapi-2.4.3/mundiapi/http/http_method_enum.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/http/auth/basic_auth.py` & `mundiapi-2.4.3/mundiapi/http/auth/basic_auth.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/http/http_request.py` & `mundiapi-2.4.3/mundiapi/http/http_request.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/http/http_context.py` & `mundiapi-2.4.3/mundiapi/http/http_context.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/http/http_client.py` & `mundiapi-2.4.3/mundiapi/http/http_client.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/http/http_call_back.py` & `mundiapi-2.4.3/mundiapi/http/http_call_back.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/mundiapi/http/http_response.py` & `mundiapi-2.4.3/mundiapi/http/http_response.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/tests/http_response_catcher.py` & `mundiapi-2.4.3/tests/http_response_catcher.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/tests/test_helper.py` & `mundiapi-2.4.3/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/tests/controllers/test_plans_controller.py` & `mundiapi-2.4.3/tests/controllers/test_plans_controller.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/tests/controllers/test_recipients_controller.py` & `mundiapi-2.4.3/tests/controllers/test_recipients_controller.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/tests/controllers/controller_test_base.py` & `mundiapi-2.4.3/tests/controllers/controller_test_base.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/tests/controllers/test_subscriptions_controller.py` & `mundiapi-2.4.3/tests/controllers/test_subscriptions_controller.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/tests/controllers/test_transfers_controller.py` & `mundiapi-2.4.3/tests/controllers/test_transfers_controller.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/tests/controllers/test_invoices_controller.py` & `mundiapi-2.4.3/tests/controllers/test_invoices_controller.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/tests/controllers/test_customers_controller.py` & `mundiapi-2.4.3/tests/controllers/test_customers_controller.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/tests/controllers/test_orders_controller.py` & `mundiapi-2.4.3/tests/controllers/test_orders_controller.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/tests/controllers/test_charges_controller.py` & `mundiapi-2.4.3/tests/controllers/test_charges_controller.py`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/setup.py` & `mundiapi-2.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         long_description = fh.read()
 else:
     with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
 
 setup(
     name='mundiapi',
-    version='2.4.2',
+    version='2.4.3',
     description='Mundipagg API',
      
     long_description_content_type="text/markdown",
      author='Mundipagg',
     author_email='suporte@mundipagg.com',
     url='https://github.com/mundipagg/MundiAPI-PYTHON',
     packages=find_packages(),
```

### Comparing `mundiapi-2.4.2/mundiapi.egg-info/SOURCES.txt` & `mundiapi-2.4.3/mundiapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mundiapi-2.4.2/README.md` & `mundiapi-2.4.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -386,16 +386,16 @@
 
 
 #### Example Usage
 
 ```python
 subscription_id = 'subscription_id'
 item_id = 'item_id'
-page = 86
-size = 86
+page = 134
+size = 134
 code = 'code'
 group = 'group'
 used_since = datetime.now()
 used_until = datetime.now()
 
 result = subscriptions_controller.get_usages(subscription_id, item_id, page, size, code, group, used_since, used_until)
 
@@ -824,16 +824,16 @@
 | createdUntil |  ``` Optional ```  | Filter for subscriptions creation date end range |
 
 
 
 #### Example Usage
 
 ```python
-page = 86
-size = 86
+page = 134
+size = 134
 code = 'code'
 billing_type = 'billing_type'
 customer_id = 'customer_id'
 plan_id = 'plan_id'
 card_id = 'card_id'
 status = 'status'
 next_billing_since = datetime.now()
@@ -887,16 +887,16 @@
 
 
 #### Example Usage
 
 ```python
 subscription_id = 'subscription_id'
 cycle_id = 'cycle_id'
-size = 86
-page = 86
+size = 134
+page = 134
 item_id = 'item_id'
 group = 'group'
 
 result = subscriptions_controller.get_usages_details(subscription_id, cycle_id, size, page, item_id, group)
 
 ```
 
@@ -978,16 +978,16 @@
 
 
 
 #### Example Usage
 
 ```python
 subscription_id = 'subscription_id'
-page = 86
-size = 86
+page = 134
+size = 134
 
 result = subscriptions_controller.get_increments(subscription_id, page, size)
 
 ```
 
 #### Errors
 
@@ -1303,16 +1303,16 @@
 
 
 
 #### Example Usage
 
 ```python
 subscription_id = 'subscription_id'
-page = 86
-size = 86
+page = 134
+size = 134
 name = 'name'
 code = 'code'
 status = 'status'
 description = 'description'
 created_since = 'created_since'
 created_until = 'created_until'
 
@@ -1493,16 +1493,16 @@
 
 
 
 #### Example Usage
 
 ```python
 subscription_id = 'subscription_id'
-page = 177
-size = 177
+page = 134
+size = 134
 
 result = subscriptions_controller.get_discounts(subscription_id, page, size)
 
 ```
 
 #### Errors
 
@@ -2184,16 +2184,16 @@
 | customerId |  ``` Optional ```  | Filter for order's customer id |
 
 
 
 #### Example Usage
 
 ```python
-page = 177
-size = 177
+page = 92
+size = 92
 code = 'code'
 status = 'status'
 created_since = datetime.now()
 created_until = datetime.now()
 customer_id = 'customer_id'
 
 result = orders_controller.get_orders(page, size, code, status, created_since, created_until, customer_id)
@@ -2389,16 +2389,16 @@
 | createdUntil |  ``` Optional ```  | Filter for plan's creation date end range |
 
 
 
 #### Example Usage
 
 ```python
-page = 177
-size = 177
+page = 92
+size = 92
 name = 'name'
 status = 'status'
 billing_type = 'billing_type'
 created_since = datetime.now()
 created_until = datetime.now()
 
 result = plans_controller.get_plans(page, size, name, status, billing_type, created_since, created_until)
@@ -3087,16 +3087,16 @@
 | customerDocument |  ``` Optional ```  | Fillter for invoice's document |
 
 
 
 #### Example Usage
 
 ```python
-page = 14
-size = 14
+page = 92
+size = 92
 code = 'code'
 customer_id = 'customer_id'
 subscription_id = 'subscription_id'
 created_since = datetime.now()
 created_until = datetime.now()
 status = 'status'
 due_since = datetime.now()
@@ -3329,16 +3329,16 @@
 
 
 
 #### Example Usage
 
 ```python
 customer_id = 'customer_id'
-page = 14
-size = 14
+page = 184
+size = 184
 
 result = customers_controller.get_cards(customer_id, page, size)
 
 ```
 
 #### Errors
 
@@ -3553,16 +3553,16 @@
 
 
 
 #### Example Usage
 
 ```python
 customer_id = 'customer_id'
-page = 14
-size = 14
+page = 184
+size = 184
 
 result = customers_controller.get_access_tokens(customer_id, page, size)
 
 ```
 
 #### Errors
 
@@ -3792,16 +3792,16 @@
 
 
 
 #### Example Usage
 
 ```python
 customer_id = 'customer_id'
-page = 14
-size = 14
+page = 184
+size = 184
 
 result = customers_controller.get_addresses(customer_id, page, size)
 
 ```
 
 #### Errors
 
@@ -4180,16 +4180,16 @@
 | createdUntil |  ``` Optional ```  | Filter for the end of the range for charge's creation |
 
 
 
 #### Example Usage
 
 ```python
-page = 14
-size = 14
+page = 184
+size = 184
 code = 'code'
 status = 'status'
 payment_method = 'payment_method'
 customer_id = 'customer_id'
 order_id = 'order_id'
 created_since = datetime.now()
 created_until = datetime.now()
@@ -4411,16 +4411,16 @@
 
 
 
 #### Example Usage
 
 ```python
 charge_id = 'charge_id'
-page = 227
-size = 227
+page = 184
+size = 184
 
 result = charges_controller.get_charge_transactions(charge_id, page, size)
 
 ```
 
 #### Errors
 
@@ -4880,16 +4880,16 @@
 
 
 
 #### Example Usage
 
 ```python
 recipient_id = 'recipient_id'
-page = 227
-size = 227
+page = 20
+size = 20
 status = 'status'
 created_since = datetime.now()
 created_until = datetime.now()
 
 result = recipients_controller.get_withdrawals(recipient_id, page, size, status, created_since, created_until)
 
 ```
@@ -5325,16 +5325,16 @@
 
 
 
 #### Example Usage
 
 ```python
 recipient_id = 'recipient_id'
-page = 227
-size = 227
+page = 20
+size = 20
 status = 'status'
 created_since = datetime.now()
 created_until = datetime.now()
 
 result = recipients_controller.get_transfers(recipient_id, page, size, status, created_since, created_until)
 
 ```
@@ -5371,16 +5371,16 @@
 | size |  ``` Optional ```  | Page size |
 
 
 
 #### Example Usage
 
 ```python
-page = 227
-size = 227
+page = 20
+size = 20
 
 result = recipients_controller.get_recipients(page, size)
 
 ```
 
 #### Errors
 
@@ -5429,16 +5429,16 @@
 
 
 
 #### Example Usage
 
 ```python
 recipient_id = 'recipient_id'
-page = 227
-size = 227
+page = 20
+size = 20
 status = 'status'
 timeframe = 'timeframe'
 payment_date_since = datetime.now()
 payment_date_until = datetime.now()
 created_since = datetime.now()
 created_until = datetime.now()
```

