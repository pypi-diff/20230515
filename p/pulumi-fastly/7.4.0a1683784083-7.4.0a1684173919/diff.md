# Comparing `tmp/pulumi_fastly-7.4.0a1683784083.tar.gz` & `tmp/pulumi_fastly-7.4.0a1684173919.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_fastly-7.4.0a1683784083.tar", last modified: Thu May 11 05:54:01 2023, max compression
+gzip compressed data, was "pulumi_fastly-7.4.0a1684173919.tar", last modified: Mon May 15 18:09:47 2023, max compression
```

## Comparing `pulumi_fastly-7.4.0a1683784083.tar` & `pulumi_fastly-7.4.0a1684173919.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:54:01.842075 pulumi_fastly-7.4.0a1683784083/
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-11 05:54:01.842075 pulumi_fastly-7.4.0a1683784083/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:54:01.842075 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   505955 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:54:01.842075 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/get_datacenters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/get_dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/get_fastly_ip_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/get_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/get_tls_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/get_tls_activation_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/get_tls_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/get_tls_certificate_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/get_tls_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/get_tls_configuration_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/get_tls_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/get_tls_platform_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/get_tls_platform_certificate_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/get_tls_private_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/get_tls_private_key_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/get_tls_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/get_tls_subscription_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/get_waf_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)   450473 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13944 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/service_acl_entries.py
--rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/service_authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)    93253 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/service_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    14001 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/service_dictionary_items.py
--rw-r--r--   0 runner    (1001) docker     (123)    14198 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/service_dynamic_snippet_content.py
--rw-r--r--   0 runner    (1001) docker     (123)   124679 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/service_vcl.py
--rw-r--r--   0 runner    (1001) docker     (123)    81770 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/service_waf_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/tls_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)    23023 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/tls_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    26052 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/tls_platform_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/tls_private_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    32406 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/tls_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/tls_subscription_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11556 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:54:01.842075 pulumi_fastly-7.4.0a1683784083/pulumi_fastly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/pulumi_fastly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 05:54:01.842075 pulumi_fastly-7.4.0a1683784083/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-11 05:54:01.000000 pulumi_fastly-7.4.0a1683784083/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:09:47.780386 pulumi_fastly-7.4.0a1684173919/
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-15 18:09:47.780386 pulumi_fastly-7.4.0a1684173919/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:09:47.776385 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   506107 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:09:47.780386 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/get_datacenters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/get_dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/get_fastly_ip_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/get_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/get_tls_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/get_tls_activation_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/get_tls_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/get_tls_certificate_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/get_tls_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/get_tls_configuration_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/get_tls_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/get_tls_platform_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/get_tls_platform_certificate_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/get_tls_private_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/get_tls_private_key_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/get_tls_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/get_tls_subscription_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/get_waf_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)   450605 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13944 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/service_acl_entries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/service_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93253 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/service_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14001 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/service_dictionary_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14198 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/service_dynamic_snippet_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124679 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/service_vcl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81770 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/service_waf_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/tls_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23023 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/tls_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26052 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/tls_platform_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/tls_private_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34762 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/tls_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/tls_subscription_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11556 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:09:47.780386 pulumi_fastly-7.4.0a1684173919/pulumi_fastly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/pulumi_fastly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 18:09:47.780386 pulumi_fastly-7.4.0a1684173919/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-15 18:09:47.000000 pulumi_fastly-7.4.0a1684173919/setup.py
```

### Comparing `pulumi_fastly-7.4.0a1683784083/PKG-INFO` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi_fastly
-Version: 7.4.0a1683784083
+Name: pulumi-fastly
+Version: 7.4.0a1684173919
 Summary: A Pulumi package for creating and managing fastly cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-fastly
 Keywords: pulumi fastly
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_fastly-7.4.0a1683784083/README.md` & `pulumi_fastly-7.4.0a1684173919/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/__init__.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/_inputs.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/_inputs.py`

 * *Files identical despite different names*

```diff
@@ -1814,53 +1814,54 @@
 
 
 @pulumi.input_type
 class ServiceComputeLoggingGcArgs:
     def __init__(__self__, *,
                  bucket_name: pulumi.Input[str],
                  name: pulumi.Input[str],
-                 project_id: pulumi.Input[str],
                  account_name: Optional[pulumi.Input[str]] = None,
                  compression_codec: Optional[pulumi.Input[str]] = None,
                  gzip_level: Optional[pulumi.Input[int]] = None,
                  message_type: Optional[pulumi.Input[str]] = None,
                  path: Optional[pulumi.Input[str]] = None,
                  period: Optional[pulumi.Input[int]] = None,
+                 project_id: Optional[pulumi.Input[str]] = None,
                  secret_key: Optional[pulumi.Input[str]] = None,
                  timestamp_format: Optional[pulumi.Input[str]] = None,
                  user: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] bucket_name: The name of the bucket in which to store the logs
         :param pulumi.Input[str] name: A unique name to identify this GCS endpoint. It is important to note that changing this attribute will delete and recreate the resource
-        :param pulumi.Input[str] project_id: The ID of your Google Cloud Platform project
         :param pulumi.Input[str] account_name: The google account name used to obtain temporary credentials (default none). You may optionally provide this via an environment variable, `FASTLY_GCS_ACCOUNT_NAME`.
         :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
         :param pulumi.Input[int] gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param pulumi.Input[str] message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param pulumi.Input[str] path: Path to store the files. Must end with a trailing slash. If this field is left empty, the files will be saved in the bucket's root path
         :param pulumi.Input[int] period: How frequently the logs should be transferred, in seconds (Default 3600)
+        :param pulumi.Input[str] project_id: The ID of your Google Cloud Platform project
         :param pulumi.Input[str] secret_key: The secret key associated with the target gcs bucket on your account. You may optionally provide this secret via an environment variable, `FASTLY_GCS_SECRET_KEY`. A typical format for the key is PEM format, containing actual newline characters where required
         :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         :param pulumi.Input[str] user: Your Google Cloud Platform service account email address. The `client_email` field in your service account authentication JSON. You may optionally provide this via an environment variable, `FASTLY_GCS_EMAIL`.
         """
         pulumi.set(__self__, "bucket_name", bucket_name)
         pulumi.set(__self__, "name", name)
-        pulumi.set(__self__, "project_id", project_id)
         if account_name is not None:
             pulumi.set(__self__, "account_name", account_name)
         if compression_codec is not None:
             pulumi.set(__self__, "compression_codec", compression_codec)
         if gzip_level is not None:
             pulumi.set(__self__, "gzip_level", gzip_level)
         if message_type is not None:
             pulumi.set(__self__, "message_type", message_type)
         if path is not None:
             pulumi.set(__self__, "path", path)
         if period is not None:
             pulumi.set(__self__, "period", period)
+        if project_id is not None:
+            pulumi.set(__self__, "project_id", project_id)
         if secret_key is not None:
             pulumi.set(__self__, "secret_key", secret_key)
         if timestamp_format is not None:
             pulumi.set(__self__, "timestamp_format", timestamp_format)
         if user is not None:
             pulumi.set(__self__, "user", user)
 
@@ -1885,26 +1886,14 @@
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter(name="projectId")
-    def project_id(self) -> pulumi.Input[str]:
-        """
-        The ID of your Google Cloud Platform project
-        """
-        return pulumi.get(self, "project_id")
-
-    @project_id.setter
-    def project_id(self, value: pulumi.Input[str]):
-        pulumi.set(self, "project_id", value)
-
-    @property
     @pulumi.getter(name="accountName")
     def account_name(self) -> Optional[pulumi.Input[str]]:
         """
         The google account name used to obtain temporary credentials (default none). You may optionally provide this via an environment variable, `FASTLY_GCS_ACCOUNT_NAME`.
         """
         return pulumi.get(self, "account_name")
 
@@ -1969,14 +1958,26 @@
         return pulumi.get(self, "period")
 
     @period.setter
     def period(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "period", value)
 
     @property
+    @pulumi.getter(name="projectId")
+    def project_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        The ID of your Google Cloud Platform project
+        """
+        return pulumi.get(self, "project_id")
+
+    @project_id.setter
+    def project_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "project_id", value)
+
+    @property
     @pulumi.getter(name="secretKey")
     def secret_key(self) -> Optional[pulumi.Input[str]]:
         """
         The secret key associated with the target gcs bucket on your account. You may optionally provide this secret via an environment variable, `FASTLY_GCS_SECRET_KEY`. A typical format for the key is PEM format, containing actual newline characters where required
         """
         return pulumi.get(self, "secret_key")
 
@@ -7224,49 +7225,48 @@
 
 
 @pulumi.input_type
 class ServiceVclLoggingGcArgs:
     def __init__(__self__, *,
                  bucket_name: pulumi.Input[str],
                  name: pulumi.Input[str],
-                 project_id: pulumi.Input[str],
                  account_name: Optional[pulumi.Input[str]] = None,
                  compression_codec: Optional[pulumi.Input[str]] = None,
                  format: Optional[pulumi.Input[str]] = None,
                  format_version: Optional[pulumi.Input[int]] = None,
                  gzip_level: Optional[pulumi.Input[int]] = None,
                  message_type: Optional[pulumi.Input[str]] = None,
                  path: Optional[pulumi.Input[str]] = None,
                  period: Optional[pulumi.Input[int]] = None,
                  placement: Optional[pulumi.Input[str]] = None,
+                 project_id: Optional[pulumi.Input[str]] = None,
                  response_condition: Optional[pulumi.Input[str]] = None,
                  secret_key: Optional[pulumi.Input[str]] = None,
                  timestamp_format: Optional[pulumi.Input[str]] = None,
                  user: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] bucket_name: The name of the bucket in which to store the logs
         :param pulumi.Input[str] name: A unique name to identify this GCS endpoint. It is important to note that changing this attribute will delete and recreate the resource
-        :param pulumi.Input[str] project_id: The ID of your Google Cloud Platform project
         :param pulumi.Input[str] account_name: The google account name used to obtain temporary credentials (default none). You may optionally provide this via an environment variable, `FASTLY_GCS_ACCOUNT_NAME`.
         :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
         :param pulumi.Input[str] format: Apache-style string or VCL variables to use for log formatting
         :param pulumi.Input[int] format_version: The version of the custom logging format used for the configured endpoint. Can be either 1 or 2. (Default: 2)
         :param pulumi.Input[int] gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param pulumi.Input[str] message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param pulumi.Input[str] path: Path to store the files. Must end with a trailing slash. If this field is left empty, the files will be saved in the bucket's root path
         :param pulumi.Input[int] period: How frequently the logs should be transferred, in seconds (Default 3600)
         :param pulumi.Input[str] placement: Where in the generated VCL the logging call should be placed.
+        :param pulumi.Input[str] project_id: The ID of your Google Cloud Platform project
         :param pulumi.Input[str] response_condition: Name of a condition to apply this logging.
         :param pulumi.Input[str] secret_key: The secret key associated with the target gcs bucket on your account. You may optionally provide this secret via an environment variable, `FASTLY_GCS_SECRET_KEY`. A typical format for the key is PEM format, containing actual newline characters where required
         :param pulumi.Input[str] timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         :param pulumi.Input[str] user: Your Google Cloud Platform service account email address. The `client_email` field in your service account authentication JSON. You may optionally provide this via an environment variable, `FASTLY_GCS_EMAIL`.
         """
         pulumi.set(__self__, "bucket_name", bucket_name)
         pulumi.set(__self__, "name", name)
-        pulumi.set(__self__, "project_id", project_id)
         if account_name is not None:
             pulumi.set(__self__, "account_name", account_name)
         if compression_codec is not None:
             pulumi.set(__self__, "compression_codec", compression_codec)
         if format is not None:
             pulumi.set(__self__, "format", format)
         if format_version is not None:
@@ -7277,14 +7277,16 @@
             pulumi.set(__self__, "message_type", message_type)
         if path is not None:
             pulumi.set(__self__, "path", path)
         if period is not None:
             pulumi.set(__self__, "period", period)
         if placement is not None:
             pulumi.set(__self__, "placement", placement)
+        if project_id is not None:
+            pulumi.set(__self__, "project_id", project_id)
         if response_condition is not None:
             pulumi.set(__self__, "response_condition", response_condition)
         if secret_key is not None:
             pulumi.set(__self__, "secret_key", secret_key)
         if timestamp_format is not None:
             pulumi.set(__self__, "timestamp_format", timestamp_format)
         if user is not None:
@@ -7311,26 +7313,14 @@
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter(name="projectId")
-    def project_id(self) -> pulumi.Input[str]:
-        """
-        The ID of your Google Cloud Platform project
-        """
-        return pulumi.get(self, "project_id")
-
-    @project_id.setter
-    def project_id(self, value: pulumi.Input[str]):
-        pulumi.set(self, "project_id", value)
-
-    @property
     @pulumi.getter(name="accountName")
     def account_name(self) -> Optional[pulumi.Input[str]]:
         """
         The google account name used to obtain temporary credentials (default none). You may optionally provide this via an environment variable, `FASTLY_GCS_ACCOUNT_NAME`.
         """
         return pulumi.get(self, "account_name")
 
@@ -7431,14 +7421,26 @@
         return pulumi.get(self, "placement")
 
     @placement.setter
     def placement(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "placement", value)
 
     @property
+    @pulumi.getter(name="projectId")
+    def project_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        The ID of your Google Cloud Platform project
+        """
+        return pulumi.get(self, "project_id")
+
+    @project_id.setter
+    def project_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "project_id", value)
+
+    @property
     @pulumi.getter(name="responseCondition")
     def response_condition(self) -> Optional[pulumi.Input[str]]:
         """
         Name of a condition to apply this logging.
         """
         return pulumi.get(self, "response_condition")
```

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/_utilities.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/config/vars.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/get_datacenters.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/get_datacenters.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/get_dictionaries.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/get_dictionaries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/get_fastly_ip_ranges.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/get_fastly_ip_ranges.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/get_services.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/get_services.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/get_tls_activation.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/get_tls_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/get_tls_activation_ids.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/get_tls_activation_ids.py`

 * *Files 17% similar despite different names*

```diff
@@ -69,14 +69,25 @@
 
 
 def get_tls_activation_ids(certificate_id: Optional[str] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetTlsActivationIdsResult:
     """
     Use this data source to get the list of TLS Activation identifiers in Fastly.
 
+    ## Example Usage
+
+    ```python
+    import pulumi
+    import pulumi_fastly as fastly
+
+    example_tls_activation_ids = fastly.get_tls_activation_ids(certificate_id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
+    example_tls_activation = [fastly.get_tls_activation(id=__value) for __key, __value in example_tls_activation_ids.ids]
+    pulumi.export("activationDomains", [a.domain for a in example_tls_activation])
+    ```
+
 
     :param str certificate_id: ID of TLS certificate used to filter activations
     """
     __args__ = dict()
     __args__['certificateId'] = certificate_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('fastly:index/getTlsActivationIds:getTlsActivationIds', __args__, opts=opts, typ=GetTlsActivationIdsResult).value
@@ -89,11 +100,22 @@
 
 @_utilities.lift_output_func(get_tls_activation_ids)
 def get_tls_activation_ids_output(certificate_id: Optional[pulumi.Input[Optional[str]]] = None,
                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTlsActivationIdsResult]:
     """
     Use this data source to get the list of TLS Activation identifiers in Fastly.
 
+    ## Example Usage
+
+    ```python
+    import pulumi
+    import pulumi_fastly as fastly
+
+    example_tls_activation_ids = fastly.get_tls_activation_ids(certificate_id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
+    example_tls_activation = [fastly.get_tls_activation(id=__value) for __key, __value in example_tls_activation_ids.ids]
+    pulumi.export("activationDomains", [a.domain for a in example_tls_activation])
+    ```
+
 
     :param str certificate_id: ID of TLS certificate used to filter activations
     """
     ...
```

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/get_tls_certificate.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/get_tls_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/get_tls_certificate_ids.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/get_tls_certificate_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/get_tls_configuration.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/get_tls_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/get_tls_configuration_ids.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/get_tls_configuration_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/get_tls_domain.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/get_tls_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/get_tls_platform_certificate.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/get_tls_platform_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/get_tls_platform_certificate_ids.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/get_tls_platform_certificate_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/get_tls_private_key.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/get_tls_private_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/get_tls_private_key_ids.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/get_tls_private_key_ids.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_fastly as fastly
 
     demo = fastly.get_tls_private_key_ids()
-    example = fastly.get_tls_private_key(id=fastly_tls_private_key_ids["demo"]["ids"])
+    example = fastly.get_tls_private_key(id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
     ```
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('fastly:index/getTlsPrivateKeyIds:getTlsPrivateKeyIds', __args__, opts=opts, typ=GetTlsPrivateKeyIdsResult).value
 
     return AwaitableGetTlsPrivateKeyIdsResult(
```

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/get_tls_subscription.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/get_tls_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/get_tls_subscription_ids.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/get_tls_subscription_ids.py`

 * *Files 14% similar despite different names*

```diff
@@ -54,14 +54,25 @@
             id=self.id,
             ids=self.ids)
 
 
 def get_tls_subscription_ids(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetTlsSubscriptionIdsResult:
     """
     Use this data source to get the list of IDs of TLS Subscriptions in Fastly.
+
+    ## Example Usage
+
+    ```python
+    import pulumi
+    import pulumi_fastly as fastly
+
+    example_tls_subscription_ids = fastly.get_tls_subscription_ids()
+    example_tls_subscription = [fastly.get_tls_subscription(id=__value) for __key, __value in example_tls_subscription_ids.ids]
+    pulumi.export("subscriptionDomains", [a.certificate_authority for a in example_tls_subscription])
+    ```
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('fastly:index/getTlsSubscriptionIds:getTlsSubscriptionIds', __args__, opts=opts, typ=GetTlsSubscriptionIdsResult).value
 
     return AwaitableGetTlsSubscriptionIdsResult(
         id=__ret__.id,
```

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/get_waf_rules.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/get_waf_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/outputs.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1636,24 +1636,24 @@
 @pulumi.output_type
 class ServiceComputeLoggingGc(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "bucketName":
             suggest = "bucket_name"
-        elif key == "projectId":
-            suggest = "project_id"
         elif key == "accountName":
             suggest = "account_name"
         elif key == "compressionCodec":
             suggest = "compression_codec"
         elif key == "gzipLevel":
             suggest = "gzip_level"
         elif key == "messageType":
             suggest = "message_type"
+        elif key == "projectId":
+            suggest = "project_id"
         elif key == "secretKey":
             suggest = "secret_key"
         elif key == "timestampFormat":
             suggest = "timestamp_format"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in ServiceComputeLoggingGc. Access the value via the '{suggest}' property getter instead.")
@@ -1665,53 +1665,54 @@
     def get(self, key: str, default = None) -> Any:
         ServiceComputeLoggingGc.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  bucket_name: str,
                  name: str,
-                 project_id: str,
                  account_name: Optional[str] = None,
                  compression_codec: Optional[str] = None,
                  gzip_level: Optional[int] = None,
                  message_type: Optional[str] = None,
                  path: Optional[str] = None,
                  period: Optional[int] = None,
+                 project_id: Optional[str] = None,
                  secret_key: Optional[str] = None,
                  timestamp_format: Optional[str] = None,
                  user: Optional[str] = None):
         """
         :param str bucket_name: The name of the bucket in which to store the logs
         :param str name: A unique name to identify this GCS endpoint. It is important to note that changing this attribute will delete and recreate the resource
-        :param str project_id: The ID of your Google Cloud Platform project
         :param str account_name: The google account name used to obtain temporary credentials (default none). You may optionally provide this via an environment variable, `FASTLY_GCS_ACCOUNT_NAME`.
         :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
         :param int gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param str message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param str path: Path to store the files. Must end with a trailing slash. If this field is left empty, the files will be saved in the bucket's root path
         :param int period: How frequently the logs should be transferred, in seconds (Default 3600)
+        :param str project_id: The ID of your Google Cloud Platform project
         :param str secret_key: The secret key associated with the target gcs bucket on your account. You may optionally provide this secret via an environment variable, `FASTLY_GCS_SECRET_KEY`. A typical format for the key is PEM format, containing actual newline characters where required
         :param str timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         :param str user: Your Google Cloud Platform service account email address. The `client_email` field in your service account authentication JSON. You may optionally provide this via an environment variable, `FASTLY_GCS_EMAIL`.
         """
         pulumi.set(__self__, "bucket_name", bucket_name)
         pulumi.set(__self__, "name", name)
-        pulumi.set(__self__, "project_id", project_id)
         if account_name is not None:
             pulumi.set(__self__, "account_name", account_name)
         if compression_codec is not None:
             pulumi.set(__self__, "compression_codec", compression_codec)
         if gzip_level is not None:
             pulumi.set(__self__, "gzip_level", gzip_level)
         if message_type is not None:
             pulumi.set(__self__, "message_type", message_type)
         if path is not None:
             pulumi.set(__self__, "path", path)
         if period is not None:
             pulumi.set(__self__, "period", period)
+        if project_id is not None:
+            pulumi.set(__self__, "project_id", project_id)
         if secret_key is not None:
             pulumi.set(__self__, "secret_key", secret_key)
         if timestamp_format is not None:
             pulumi.set(__self__, "timestamp_format", timestamp_format)
         if user is not None:
             pulumi.set(__self__, "user", user)
 
@@ -1728,22 +1729,14 @@
     def name(self) -> str:
         """
         A unique name to identify this GCS endpoint. It is important to note that changing this attribute will delete and recreate the resource
         """
         return pulumi.get(self, "name")
 
     @property
-    @pulumi.getter(name="projectId")
-    def project_id(self) -> str:
-        """
-        The ID of your Google Cloud Platform project
-        """
-        return pulumi.get(self, "project_id")
-
-    @property
     @pulumi.getter(name="accountName")
     def account_name(self) -> Optional[str]:
         """
         The google account name used to obtain temporary credentials (default none). You may optionally provide this via an environment variable, `FASTLY_GCS_ACCOUNT_NAME`.
         """
         return pulumi.get(self, "account_name")
 
@@ -1784,14 +1777,22 @@
     def period(self) -> Optional[int]:
         """
         How frequently the logs should be transferred, in seconds (Default 3600)
         """
         return pulumi.get(self, "period")
 
     @property
+    @pulumi.getter(name="projectId")
+    def project_id(self) -> Optional[str]:
+        """
+        The ID of your Google Cloud Platform project
+        """
+        return pulumi.get(self, "project_id")
+
+    @property
     @pulumi.getter(name="secretKey")
     def secret_key(self) -> Optional[str]:
         """
         The secret key associated with the target gcs bucket on your account. You may optionally provide this secret via an environment variable, `FASTLY_GCS_SECRET_KEY`. A typical format for the key is PEM format, containing actual newline characters where required
         """
         return pulumi.get(self, "secret_key")
 
@@ -6474,26 +6475,26 @@
 @pulumi.output_type
 class ServiceVclLoggingGc(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "bucketName":
             suggest = "bucket_name"
-        elif key == "projectId":
-            suggest = "project_id"
         elif key == "accountName":
             suggest = "account_name"
         elif key == "compressionCodec":
             suggest = "compression_codec"
         elif key == "formatVersion":
             suggest = "format_version"
         elif key == "gzipLevel":
             suggest = "gzip_level"
         elif key == "messageType":
             suggest = "message_type"
+        elif key == "projectId":
+            suggest = "project_id"
         elif key == "responseCondition":
             suggest = "response_condition"
         elif key == "secretKey":
             suggest = "secret_key"
         elif key == "timestampFormat":
             suggest = "timestamp_format"
 
@@ -6507,49 +6508,48 @@
     def get(self, key: str, default = None) -> Any:
         ServiceVclLoggingGc.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  bucket_name: str,
                  name: str,
-                 project_id: str,
                  account_name: Optional[str] = None,
                  compression_codec: Optional[str] = None,
                  format: Optional[str] = None,
                  format_version: Optional[int] = None,
                  gzip_level: Optional[int] = None,
                  message_type: Optional[str] = None,
                  path: Optional[str] = None,
                  period: Optional[int] = None,
                  placement: Optional[str] = None,
+                 project_id: Optional[str] = None,
                  response_condition: Optional[str] = None,
                  secret_key: Optional[str] = None,
                  timestamp_format: Optional[str] = None,
                  user: Optional[str] = None):
         """
         :param str bucket_name: The name of the bucket in which to store the logs
         :param str name: A unique name to identify this GCS endpoint. It is important to note that changing this attribute will delete and recreate the resource
-        :param str project_id: The ID of your Google Cloud Platform project
         :param str account_name: The google account name used to obtain temporary credentials (default none). You may optionally provide this via an environment variable, `FASTLY_GCS_ACCOUNT_NAME`.
         :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
         :param str format: Apache-style string or VCL variables to use for log formatting
         :param int format_version: The version of the custom logging format used for the configured endpoint. Can be either 1 or 2. (Default: 2)
         :param int gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param str message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param str path: Path to store the files. Must end with a trailing slash. If this field is left empty, the files will be saved in the bucket's root path
         :param int period: How frequently the logs should be transferred, in seconds (Default 3600)
         :param str placement: Where in the generated VCL the logging call should be placed.
+        :param str project_id: The ID of your Google Cloud Platform project
         :param str response_condition: Name of a condition to apply this logging.
         :param str secret_key: The secret key associated with the target gcs bucket on your account. You may optionally provide this secret via an environment variable, `FASTLY_GCS_SECRET_KEY`. A typical format for the key is PEM format, containing actual newline characters where required
         :param str timestamp_format: The `strftime` specified timestamp formatting (default `%Y-%m-%dT%H:%M:%S.000`)
         :param str user: Your Google Cloud Platform service account email address. The `client_email` field in your service account authentication JSON. You may optionally provide this via an environment variable, `FASTLY_GCS_EMAIL`.
         """
         pulumi.set(__self__, "bucket_name", bucket_name)
         pulumi.set(__self__, "name", name)
-        pulumi.set(__self__, "project_id", project_id)
         if account_name is not None:
             pulumi.set(__self__, "account_name", account_name)
         if compression_codec is not None:
             pulumi.set(__self__, "compression_codec", compression_codec)
         if format is not None:
             pulumi.set(__self__, "format", format)
         if format_version is not None:
@@ -6560,14 +6560,16 @@
             pulumi.set(__self__, "message_type", message_type)
         if path is not None:
             pulumi.set(__self__, "path", path)
         if period is not None:
             pulumi.set(__self__, "period", period)
         if placement is not None:
             pulumi.set(__self__, "placement", placement)
+        if project_id is not None:
+            pulumi.set(__self__, "project_id", project_id)
         if response_condition is not None:
             pulumi.set(__self__, "response_condition", response_condition)
         if secret_key is not None:
             pulumi.set(__self__, "secret_key", secret_key)
         if timestamp_format is not None:
             pulumi.set(__self__, "timestamp_format", timestamp_format)
         if user is not None:
@@ -6586,22 +6588,14 @@
     def name(self) -> str:
         """
         A unique name to identify this GCS endpoint. It is important to note that changing this attribute will delete and recreate the resource
         """
         return pulumi.get(self, "name")
 
     @property
-    @pulumi.getter(name="projectId")
-    def project_id(self) -> str:
-        """
-        The ID of your Google Cloud Platform project
-        """
-        return pulumi.get(self, "project_id")
-
-    @property
     @pulumi.getter(name="accountName")
     def account_name(self) -> Optional[str]:
         """
         The google account name used to obtain temporary credentials (default none). You may optionally provide this via an environment variable, `FASTLY_GCS_ACCOUNT_NAME`.
         """
         return pulumi.get(self, "account_name")
 
@@ -6666,14 +6660,22 @@
     def placement(self) -> Optional[str]:
         """
         Where in the generated VCL the logging call should be placed.
         """
         return pulumi.get(self, "placement")
 
     @property
+    @pulumi.getter(name="projectId")
+    def project_id(self) -> Optional[str]:
+        """
+        The ID of your Google Cloud Platform project
+        """
+        return pulumi.get(self, "project_id")
+
+    @property
     @pulumi.getter(name="responseCondition")
     def response_condition(self) -> Optional[str]:
         """
         Name of a condition to apply this logging.
         """
         return pulumi.get(self, "response_condition")
```

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/provider.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/service_acl_entries.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/service_acl_entries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/service_authorization.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/service_authorization.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/service_compute.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/service_compute.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/service_dictionary_items.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/service_dictionary_items.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/service_dynamic_snippet_content.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/service_dynamic_snippet_content.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/service_vcl.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/service_vcl.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/service_waf_configuration.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/service_waf_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/tls_activation.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/tls_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/tls_certificate.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/tls_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/tls_platform_certificate.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/tls_platform_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/tls_private_key.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/tls_private_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/tls_subscription.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/tls_subscription.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,16 @@
         """
         The set of arguments for constructing a TlsSubscription resource.
         :param pulumi.Input[str] certificate_authority: The entity that issues and certifies the TLS certificates for your subscription. Valid values are `lets-encrypt` or `globalsign`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] domains: List of domains on which to enable TLS.
         :param pulumi.Input[str] common_name: The common name associated with the subscription generated by Fastly TLS. If you do not pass a common name on create, we will default to the first TLS domain included. If provided, the domain chosen as the common name must be included in TLS domains.
         :param pulumi.Input[str] configuration_id: The ID of the set of TLS configuration options that apply to the enabled domains on this subscription.
         :param pulumi.Input[bool] force_destroy: Always delete subscription, even when active domains are present. Defaults to false.
+               
+               !> **Warning:** by default, the Fastly API protects you from disabling production traffic by preventing updating or deleting subscriptions with active domains. The use of `force_update` and `force_destroy` will override these protections. Take extra care using these options if you are handling production traffic.
         :param pulumi.Input[bool] force_update: Always update subscription, even when active domains are present. Defaults to false.
         """
         pulumi.set(__self__, "certificate_authority", certificate_authority)
         pulumi.set(__self__, "domains", domains)
         if common_name is not None:
             pulumi.set(__self__, "common_name", common_name)
         if configuration_id is not None:
@@ -91,14 +93,16 @@
         pulumi.set(self, "configuration_id", value)
 
     @property
     @pulumi.getter(name="forceDestroy")
     def force_destroy(self) -> Optional[pulumi.Input[bool]]:
         """
         Always delete subscription, even when active domains are present. Defaults to false.
+
+        !> **Warning:** by default, the Fastly API protects you from disabling production traffic by preventing updating or deleting subscriptions with active domains. The use of `force_update` and `force_destroy` will override these protections. Take extra care using these options if you are handling production traffic.
         """
         return pulumi.get(self, "force_destroy")
 
     @force_destroy.setter
     def force_destroy(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "force_destroy", value)
 
@@ -136,14 +140,16 @@
         :param pulumi.Input[str] certificate_authority: The entity that issues and certifies the TLS certificates for your subscription. Valid values are `lets-encrypt` or `globalsign`.
         :param pulumi.Input[str] certificate_id: The certificate ID associated with the subscription.
         :param pulumi.Input[str] common_name: The common name associated with the subscription generated by Fastly TLS. If you do not pass a common name on create, we will default to the first TLS domain included. If provided, the domain chosen as the common name must be included in TLS domains.
         :param pulumi.Input[str] configuration_id: The ID of the set of TLS configuration options that apply to the enabled domains on this subscription.
         :param pulumi.Input[str] created_at: Timestamp (GMT) when the subscription was created.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] domains: List of domains on which to enable TLS.
         :param pulumi.Input[bool] force_destroy: Always delete subscription, even when active domains are present. Defaults to false.
+               
+               !> **Warning:** by default, the Fastly API protects you from disabling production traffic by preventing updating or deleting subscriptions with active domains. The use of `force_update` and `force_destroy` will override these protections. Take extra care using these options if you are handling production traffic.
         :param pulumi.Input[bool] force_update: Always update subscription, even when active domains are present. Defaults to false.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] managed_dns_challenge: The details required to configure DNS to respond to ACME DNS challenge in order to verify domain ownership.
         :param pulumi.Input[Sequence[pulumi.Input['TlsSubscriptionManagedDnsChallengeArgs']]] managed_dns_challenges: A list of options for configuring DNS to respond to ACME DNS challenge in order to verify domain ownership.
         :param pulumi.Input[Sequence[pulumi.Input['TlsSubscriptionManagedHttpChallengeArgs']]] managed_http_challenges: A list of options for configuring DNS to respond to ACME HTTP challenge in order to verify domain ownership. Best accessed through a `for` expression to filter the relevant record.
         :param pulumi.Input[str] state: The current state of the subscription. The list of possible states are: `pending`, `processing`, `issued`, and `renewing`.
         :param pulumi.Input[str] updated_at: Timestamp (GMT) when the subscription was updated.
         """
@@ -250,14 +256,16 @@
         pulumi.set(self, "domains", value)
 
     @property
     @pulumi.getter(name="forceDestroy")
     def force_destroy(self) -> Optional[pulumi.Input[bool]]:
         """
         Always delete subscription, even when active domains are present. Defaults to false.
+
+        !> **Warning:** by default, the Fastly API protects you from disabling production traffic by preventing updating or deleting subscriptions with active domains. The use of `force_update` and `force_destroy` will override these protections. Take extra care using these options if you are handling production traffic.
         """
         return pulumi.get(self, "force_destroy")
 
     @force_destroy.setter
     def force_destroy(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "force_destroy", value)
 
@@ -368,14 +376,16 @@
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] certificate_authority: The entity that issues and certifies the TLS certificates for your subscription. Valid values are `lets-encrypt` or `globalsign`.
         :param pulumi.Input[str] common_name: The common name associated with the subscription generated by Fastly TLS. If you do not pass a common name on create, we will default to the first TLS domain included. If provided, the domain chosen as the common name must be included in TLS domains.
         :param pulumi.Input[str] configuration_id: The ID of the set of TLS configuration options that apply to the enabled domains on this subscription.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] domains: List of domains on which to enable TLS.
         :param pulumi.Input[bool] force_destroy: Always delete subscription, even when active domains are present. Defaults to false.
+               
+               !> **Warning:** by default, the Fastly API protects you from disabling production traffic by preventing updating or deleting subscriptions with active domains. The use of `force_update` and `force_destroy` will override these protections. Take extra care using these options if you are handling production traffic.
         :param pulumi.Input[bool] force_update: Always update subscription, even when active domains are present. Defaults to false.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: TlsSubscriptionArgs,
@@ -479,14 +489,16 @@
         :param pulumi.Input[str] certificate_authority: The entity that issues and certifies the TLS certificates for your subscription. Valid values are `lets-encrypt` or `globalsign`.
         :param pulumi.Input[str] certificate_id: The certificate ID associated with the subscription.
         :param pulumi.Input[str] common_name: The common name associated with the subscription generated by Fastly TLS. If you do not pass a common name on create, we will default to the first TLS domain included. If provided, the domain chosen as the common name must be included in TLS domains.
         :param pulumi.Input[str] configuration_id: The ID of the set of TLS configuration options that apply to the enabled domains on this subscription.
         :param pulumi.Input[str] created_at: Timestamp (GMT) when the subscription was created.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] domains: List of domains on which to enable TLS.
         :param pulumi.Input[bool] force_destroy: Always delete subscription, even when active domains are present. Defaults to false.
+               
+               !> **Warning:** by default, the Fastly API protects you from disabling production traffic by preventing updating or deleting subscriptions with active domains. The use of `force_update` and `force_destroy` will override these protections. Take extra care using these options if you are handling production traffic.
         :param pulumi.Input[bool] force_update: Always update subscription, even when active domains are present. Defaults to false.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] managed_dns_challenge: The details required to configure DNS to respond to ACME DNS challenge in order to verify domain ownership.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['TlsSubscriptionManagedDnsChallengeArgs']]]] managed_dns_challenges: A list of options for configuring DNS to respond to ACME DNS challenge in order to verify domain ownership.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['TlsSubscriptionManagedHttpChallengeArgs']]]] managed_http_challenges: A list of options for configuring DNS to respond to ACME HTTP challenge in order to verify domain ownership. Best accessed through a `for` expression to filter the relevant record.
         :param pulumi.Input[str] state: The current state of the subscription. The list of possible states are: `pending`, `processing`, `issued`, and `renewing`.
         :param pulumi.Input[str] updated_at: Timestamp (GMT) when the subscription was updated.
         """
@@ -558,14 +570,16 @@
         return pulumi.get(self, "domains")
 
     @property
     @pulumi.getter(name="forceDestroy")
     def force_destroy(self) -> pulumi.Output[Optional[bool]]:
         """
         Always delete subscription, even when active domains are present. Defaults to false.
+
+        !> **Warning:** by default, the Fastly API protects you from disabling production traffic by preventing updating or deleting subscriptions with active domains. The use of `force_update` and `force_destroy` will override these protections. Take extra care using these options if you are handling production traffic.
         """
         return pulumi.get(self, "force_destroy")
 
     @property
     @pulumi.getter(name="forceUpdate")
     def force_update(self) -> pulumi.Output[Optional[bool]]:
         """
```

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/tls_subscription_validation.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/tls_subscription_validation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly/user.py` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly.egg-info/PKG-INFO` & `pulumi_fastly-7.4.0a1684173919/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi-fastly
-Version: 7.4.0a1683784083
+Name: pulumi_fastly
+Version: 7.4.0a1684173919
 Summary: A Pulumi package for creating and managing fastly cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-fastly
 Keywords: pulumi fastly
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_fastly-7.4.0a1683784083/pulumi_fastly.egg-info/SOURCES.txt` & `pulumi_fastly-7.4.0a1684173919/pulumi_fastly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-7.4.0a1683784083/setup.py` & `pulumi_fastly-7.4.0a1684173919/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "7.4.0a1683784083"
-PLUGIN_VERSION = "7.4.0-alpha.1683784083+38587be1"
+VERSION = "7.4.0a1684173919"
+PLUGIN_VERSION = "7.4.0-alpha.1684173919+41e6433e"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'fastly', PLUGIN_VERSION])
         except OSError as error:
```

