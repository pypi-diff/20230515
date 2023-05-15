# Comparing `tmp/oic-1.5.0.tar.gz` & `tmp/oic-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oic-1.5.0.tar", last modified: Wed Dec 14 13:46:18 2022, max compression
+gzip compressed data, was "oic-1.6.0.tar", last modified: Mon May 15 07:01:49 2023, max compression
```

## Comparing `oic-1.5.0.tar` & `oic-1.6.0.tar`

### file list

```diff
@@ -1,90 +1,129 @@
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2022-12-14 13:46:18.698082 oic-1.5.0/
--rw-r--r--   0 tomas     (1000) tomas     (1000)      563 2021-02-12 13:09:56.000000 oic-1.5.0/LICENSE.txt
--rw-r--r--   0 tomas     (1000) tomas     (1000)       25 2021-02-12 13:09:56.000000 oic-1.5.0/MANIFEST.in
--rw-r--r--   0 tomas     (1000) tomas     (1000)     5417 2022-12-14 13:46:18.698082 oic-1.5.0/PKG-INFO
--rw-r--r--   0 tomas     (1000) tomas     (1000)     4502 2022-03-08 09:59:02.000000 oic-1.5.0/README.rst
--rw-r--r--   0 tomas     (1000) tomas     (1000)      281 2022-12-14 13:46:18.698082 oic-1.5.0/setup.cfg
--rwxr-xr-x   0 tomas     (1000) tomas     (1000)     3249 2022-11-17 17:11:12.000000 oic-1.5.0/setup.py
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2022-12-14 13:46:18.674082 oic-1.5.0/src/
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2022-12-14 13:46:18.678082 oic-1.5.0/src/oic/
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1450 2022-12-14 13:44:53.000000 oic-1.5.0/src/oic/__init__.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1492 2021-02-12 13:09:56.000000 oic-1.5.0/src/oic/exception.py
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2022-12-14 13:46:18.682082 oic-1.5.0/src/oic/extension/
--rw-r--r--   0 tomas     (1000) tomas     (1000)       22 2021-02-12 13:09:56.000000 oic-1.5.0/src/oic/extension/__init__.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    13271 2022-08-03 13:05:54.000000 oic-1.5.0/src/oic/extension/client.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     3803 2022-03-08 09:59:02.000000 oic-1.5.0/src/oic/extension/device_flow.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     2232 2021-02-12 13:09:56.000000 oic-1.5.0/src/oic/extension/heart.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     8286 2021-02-12 13:09:56.000000 oic-1.5.0/src/oic/extension/message.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     4191 2022-03-08 09:59:02.000000 oic-1.5.0/src/oic/extension/pop.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     2817 2021-02-12 13:09:56.000000 oic-1.5.0/src/oic/extension/popjwt.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     5495 2022-03-08 09:59:02.000000 oic-1.5.0/src/oic/extension/proof_of_possesion.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    29600 2022-03-08 09:59:02.000000 oic-1.5.0/src/oic/extension/provider.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     5033 2021-02-12 13:09:56.000000 oic-1.5.0/src/oic/extension/signed_http_req.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)      256 2021-02-12 13:09:56.000000 oic-1.5.0/src/oic/extension/single.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     2430 2021-02-12 13:09:56.000000 oic-1.5.0/src/oic/extension/sts.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     5217 2022-03-08 09:59:02.000000 oic-1.5.0/src/oic/extension/token.py
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2022-12-14 13:46:18.686082 oic-1.5.0/src/oic/oauth2/
--rw-r--r--   0 tomas     (1000) tomas     (1000)    41469 2022-11-17 17:11:12.000000 oic-1.5.0/src/oic/oauth2/__init__.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     5968 2022-12-12 07:43:41.000000 oic-1.5.0/src/oic/oauth2/base.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    11396 2022-03-08 09:59:06.000000 oic-1.5.0/src/oic/oauth2/consumer.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1111 2021-02-12 13:09:56.000000 oic-1.5.0/src/oic/oauth2/exception.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     4766 2022-03-08 09:59:02.000000 oic-1.5.0/src/oic/oauth2/grant.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    39289 2022-03-08 09:59:02.000000 oic-1.5.0/src/oic/oauth2/message.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    38987 2022-11-17 17:11:12.000000 oic-1.5.0/src/oic/oauth2/provider.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     7168 2022-08-03 13:05:54.000000 oic-1.5.0/src/oic/oauth2/util.py
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2022-12-14 13:46:18.690082 oic-1.5.0/src/oic/oic/
--rw-r--r--   0 tomas     (1000) tomas     (1000)    65764 2022-11-17 17:11:12.000000 oic-1.5.0/src/oic/oic/__init__.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     7823 2022-03-08 09:59:02.000000 oic-1.5.0/src/oic/oic/claims_provider.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    18280 2022-08-03 13:05:54.000000 oic-1.5.0/src/oic/oic/consumer.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    40833 2022-11-17 17:11:12.000000 oic-1.5.0/src/oic/oic/message.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    83874 2022-11-17 17:11:12.000000 oic-1.5.0/src/oic/oic/provider.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)        0 2021-02-12 13:09:56.000000 oic-1.5.0/src/oic/py.typed
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2022-12-14 13:46:18.694082 oic-1.5.0/src/oic/utils/
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1054 2021-02-12 13:09:56.000000 oic-1.5.0/src/oic/utils/__init__.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     5780 2022-03-08 09:59:02.000000 oic-1.5.0/src/oic/utils/aes.py
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2022-12-14 13:46:18.698082 oic-1.5.0/src/oic/utils/authn/
--rw-r--r--   0 tomas     (1000) tomas     (1000)       23 2021-02-12 13:09:56.000000 oic-1.5.0/src/oic/utils/authn/__init__.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     7127 2022-03-08 09:59:02.000000 oic-1.5.0/src/oic/utils/authn/authn_context.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    18164 2022-03-08 09:59:02.000000 oic-1.5.0/src/oic/utils/authn/client.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1635 2021-02-12 13:09:56.000000 oic-1.5.0/src/oic/utils/authn/client_saml.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1981 2022-03-08 09:59:02.000000 oic-1.5.0/src/oic/utils/authn/javascript_login.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)      783 2021-02-12 13:09:56.000000 oic-1.5.0/src/oic/utils/authn/ldap_member.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     3217 2022-03-08 09:59:02.000000 oic-1.5.0/src/oic/utils/authn/ldapc.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     2626 2021-02-12 13:09:56.000000 oic-1.5.0/src/oic/utils/authn/multi_auth.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    14778 2022-03-08 09:59:02.000000 oic-1.5.0/src/oic/utils/authn/saml.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    13839 2022-03-08 09:59:02.000000 oic-1.5.0/src/oic/utils/authn/user.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     7069 2022-03-08 09:59:02.000000 oic-1.5.0/src/oic/utils/authn/user_cas.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1951 2022-03-08 09:59:02.000000 oic-1.5.0/src/oic/utils/authz.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)      507 2021-02-12 13:09:56.000000 oic-1.5.0/src/oic/utils/claims.py
--rwxr-xr-x   0 tomas     (1000) tomas     (1000)     6200 2022-03-08 09:59:02.000000 oic-1.5.0/src/oic/utils/client_management.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     3768 2021-02-12 13:09:56.000000 oic-1.5.0/src/oic/utils/clientdb.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    19258 2022-03-08 09:59:02.000000 oic-1.5.0/src/oic/utils/http_util.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     3615 2021-02-12 13:09:56.000000 oic-1.5.0/src/oic/utils/jwt.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    37032 2022-03-08 09:59:06.000000 oic-1.5.0/src/oic/utils/keyio.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1679 2021-02-12 13:09:56.000000 oic-1.5.0/src/oic/utils/restrict.py
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2022-12-14 13:46:18.698082 oic-1.5.0/src/oic/utils/rp/
--rw-r--r--   0 tomas     (1000) tomas     (1000)    15154 2022-03-08 09:59:02.000000 oic-1.5.0/src/oic/utils/rp/__init__.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    12618 2022-03-08 09:59:02.000000 oic-1.5.0/src/oic/utils/rp/oauth2.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1765 2022-03-08 09:59:02.000000 oic-1.5.0/src/oic/utils/sanitize.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    32421 2022-03-08 09:59:06.000000 oic-1.5.0/src/oic/utils/sdb.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     6122 2022-03-08 09:59:02.000000 oic-1.5.0/src/oic/utils/session_backend.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     4618 2022-11-17 17:11:12.000000 oic-1.5.0/src/oic/utils/settings.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1601 2022-03-08 09:59:02.000000 oic-1.5.0/src/oic/utils/shelve_wrapper.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     3635 2022-03-08 09:59:02.000000 oic-1.5.0/src/oic/utils/stateless.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1640 2021-02-12 13:09:56.000000 oic-1.5.0/src/oic/utils/template_render.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    10293 2022-03-08 09:59:06.000000 oic-1.5.0/src/oic/utils/time_util.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     4535 2021-02-12 13:09:56.000000 oic-1.5.0/src/oic/utils/token_handler.py
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2022-12-14 13:46:18.698082 oic-1.5.0/src/oic/utils/userinfo/
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1316 2021-02-12 13:09:56.000000 oic-1.5.0/src/oic/utils/userinfo/__init__.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     2307 2022-03-08 09:59:06.000000 oic-1.5.0/src/oic/utils/userinfo/aa_info.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     5012 2022-03-08 09:59:02.000000 oic-1.5.0/src/oic/utils/userinfo/distaggr.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     3797 2022-03-08 09:59:02.000000 oic-1.5.0/src/oic/utils/userinfo/ldap_info.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)    10239 2022-03-08 09:59:02.000000 oic-1.5.0/src/oic/utils/webfinger.py
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2022-12-14 13:46:18.678082 oic-1.5.0/src/oic.egg-info/
--rw-r--r--   0 tomas     (1000) tomas     (1000)     5417 2022-12-14 13:46:18.000000 oic-1.5.0/src/oic.egg-info/PKG-INFO
--rw-r--r--   0 tomas     (1000) tomas     (1000)     2138 2022-12-14 13:46:18.000000 oic-1.5.0/src/oic.egg-info/SOURCES.txt
--rw-r--r--   0 tomas     (1000) tomas     (1000)        1 2022-12-14 13:46:18.000000 oic-1.5.0/src/oic.egg-info/dependency_links.txt
--rw-r--r--   0 tomas     (1000) tomas     (1000)       74 2022-12-14 13:46:18.000000 oic-1.5.0/src/oic.egg-info/entry_points.txt
--rw-r--r--   0 tomas     (1000) tomas     (1000)        1 2021-06-14 15:48:45.000000 oic-1.5.0/src/oic.egg-info/not-zip-safe
--rw-r--r--   0 tomas     (1000) tomas     (1000)      357 2022-12-14 13:46:18.000000 oic-1.5.0/src/oic.egg-info/requires.txt
--rw-r--r--   0 tomas     (1000) tomas     (1000)       95 2022-12-14 13:46:18.000000 oic-1.5.0/src/oic.egg-info/top_level.txt
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-15 07:01:49.541509 oic-1.6.0/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)      563 2021-02-12 13:09:56.000000 oic-1.6.0/LICENSE.txt
+-rw-r--r--   0 tomas     (1000) tomas     (1000)       25 2021-02-12 13:09:56.000000 oic-1.6.0/MANIFEST.in
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     5407 2023-05-15 07:01:49.541509 oic-1.6.0/PKG-INFO
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     4493 2023-03-27 11:11:37.000000 oic-1.6.0/README.rst
+-rw-r--r--   0 tomas     (1000) tomas     (1000)      281 2023-05-15 07:01:49.541509 oic-1.6.0/setup.cfg
+-rwxr-xr-x   0 tomas     (1000) tomas     (1000)     3310 2023-05-02 08:00:09.000000 oic-1.6.0/setup.py
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-15 07:01:49.509509 oic-1.6.0/src/
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-15 07:01:49.513509 oic-1.6.0/src/oic/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1450 2023-05-15 07:00:07.000000 oic-1.6.0/src/oic/__init__.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1492 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/exception.py
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-15 07:01:49.517509 oic-1.6.0/src/oic/extension/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)       22 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/extension/__init__.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    13270 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/extension/client.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     3802 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/extension/device_flow.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     2232 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/extension/heart.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     8286 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/extension/message.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     4191 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/extension/pop.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     2817 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/extension/popjwt.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     5495 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/extension/proof_of_possesion.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    29599 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/extension/provider.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     5033 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/extension/signed_http_req.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)      256 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/extension/single.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     2430 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/extension/sts.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     5217 2023-05-02 08:00:09.000000 oic-1.6.0/src/oic/extension/token.py
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-15 07:01:49.521509 oic-1.6.0/src/oic/oauth2/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    41235 2023-05-02 08:00:09.000000 oic-1.6.0/src/oic/oauth2/__init__.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     5967 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/oauth2/base.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    11396 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/oauth2/consumer.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1111 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/oauth2/exception.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     4766 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/oauth2/grant.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    39288 2023-05-02 08:00:09.000000 oic-1.6.0/src/oic/oauth2/message.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    38987 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/oauth2/provider.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     7251 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/oauth2/util.py
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-15 07:01:49.521509 oic-1.6.0/src/oic/oic/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    65757 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/oic/__init__.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     7820 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/oic/claims_provider.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    18940 2023-05-02 08:00:12.000000 oic-1.6.0/src/oic/oic/consumer.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    40833 2023-05-02 08:00:09.000000 oic-1.6.0/src/oic/oic/message.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    83873 2023-05-02 08:00:09.000000 oic-1.6.0/src/oic/oic/provider.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)        0 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/py.typed
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-15 07:01:49.529509 oic-1.6.0/src/oic/utils/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1063 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/__init__.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     5983 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/aes.py
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-15 07:01:49.529509 oic-1.6.0/src/oic/utils/authn/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)       23 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/utils/authn/__init__.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     7098 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/authn/authn_context.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    18164 2022-03-08 09:59:02.000000 oic-1.6.0/src/oic/utils/authn/client.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1635 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/utils/authn/client_saml.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1981 2022-03-08 09:59:02.000000 oic-1.6.0/src/oic/utils/authn/javascript_login.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)      783 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/utils/authn/ldap_member.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     3217 2022-03-08 09:59:02.000000 oic-1.6.0/src/oic/utils/authn/ldapc.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     2626 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/utils/authn/multi_auth.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    14777 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/authn/saml.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    13839 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/authn/user.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     7248 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/authn/user_cas.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1951 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/authz.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)      507 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/utils/claims.py
+-rwxr-xr-x   0 tomas     (1000) tomas     (1000)     6200 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/client_management.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     3901 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/clientdb.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    19258 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/http_util.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     3615 2023-05-02 08:00:09.000000 oic-1.6.0/src/oic/utils/jwt.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    37029 2023-05-02 08:00:09.000000 oic-1.6.0/src/oic/utils/keyio.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1679 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/utils/restrict.py
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-15 07:01:49.529509 oic-1.6.0/src/oic/utils/rp/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    15154 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/rp/__init__.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    12618 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/rp/oauth2.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1765 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/sanitize.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    32421 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/sdb.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     6122 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/session_backend.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     2807 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/settings.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1601 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/shelve_wrapper.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     3635 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/stateless.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1640 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/utils/template_render.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    10293 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/time_util.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     4535 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/utils/token_handler.py
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-15 07:01:49.533509 oic-1.6.0/src/oic/utils/userinfo/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1316 2021-02-12 13:09:56.000000 oic-1.6.0/src/oic/utils/userinfo/__init__.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     2307 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/userinfo/aa_info.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     5011 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/userinfo/distaggr.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     3797 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/userinfo/ldap_info.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    10239 2023-03-27 11:11:37.000000 oic-1.6.0/src/oic/utils/webfinger.py
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-15 07:01:49.513509 oic-1.6.0/src/oic.egg-info/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     5407 2023-05-15 07:01:49.000000 oic-1.6.0/src/oic.egg-info/PKG-INFO
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     3066 2023-05-15 07:01:49.000000 oic-1.6.0/src/oic.egg-info/SOURCES.txt
+-rw-r--r--   0 tomas     (1000) tomas     (1000)        1 2023-05-15 07:01:49.000000 oic-1.6.0/src/oic.egg-info/dependency_links.txt
+-rw-r--r--   0 tomas     (1000) tomas     (1000)       74 2023-05-15 07:01:49.000000 oic-1.6.0/src/oic.egg-info/entry_points.txt
+-rw-r--r--   0 tomas     (1000) tomas     (1000)        1 2021-06-14 15:48:45.000000 oic-1.6.0/src/oic.egg-info/not-zip-safe
+-rw-r--r--   0 tomas     (1000) tomas     (1000)      410 2023-05-15 07:01:49.000000 oic-1.6.0/src/oic.egg-info/requires.txt
+-rw-r--r--   0 tomas     (1000) tomas     (1000)       95 2023-05-15 07:01:49.000000 oic-1.6.0/src/oic.egg-info/top_level.txt
+drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-15 07:01:49.541509 oic-1.6.0/tests/
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1672 2021-02-12 13:09:56.000000 oic-1.6.0/tests/test_aes.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     2518 2021-02-12 13:09:56.000000 oic-1.6.0/tests/test_authn_context.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1041 2021-02-12 13:09:56.000000 oic-1.6.0/tests/test_authn_user.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1163 2021-02-12 13:09:56.000000 oic-1.6.0/tests/test_claims.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     5260 2023-05-02 08:00:09.000000 oic-1.6.0/tests/test_claims_provider.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    12801 2023-05-02 08:00:09.000000 oic-1.6.0/tests/test_client.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1285 2021-02-12 13:09:56.000000 oic-1.6.0/tests/test_client_management.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     4543 2023-03-27 11:11:37.000000 oic-1.6.0/tests/test_clientdb.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     4372 2021-02-12 13:09:56.000000 oic-1.6.0/tests/test_grant.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     7590 2023-03-27 11:11:37.000000 oic-1.6.0/tests/test_http_util.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1522 2023-05-02 08:00:09.000000 oic-1.6.0/tests/test_jwt.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    19265 2023-05-02 08:00:09.000000 oic-1.6.0/tests/test_keyio.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    27204 2023-03-27 11:11:37.000000 oic-1.6.0/tests/test_oauth2.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    11031 2023-03-27 11:11:37.000000 oic-1.6.0/tests/test_oauth2_consumer.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    30827 2023-05-02 08:00:09.000000 oic-1.6.0/tests/test_oauth2_message.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    32548 2023-03-27 11:11:37.000000 oic-1.6.0/tests/test_oauth2_provider.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    52202 2023-05-02 08:00:09.000000 oic-1.6.0/tests/test_oic.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    43996 2023-05-02 08:00:12.000000 oic-1.6.0/tests/test_oic_consumer.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    12012 2023-03-27 11:11:37.000000 oic-1.6.0/tests/test_oic_consumer_logout.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    47073 2023-05-02 08:00:09.000000 oic-1.6.0/tests/test_oic_message.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    76101 2023-05-02 08:00:09.000000 oic-1.6.0/tests/test_oic_provider.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    40165 2023-03-27 11:11:37.000000 oic-1.6.0/tests/test_oic_provider_logout.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     4670 2021-02-12 13:09:56.000000 oic-1.6.0/tests/test_pop.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     7936 2021-02-12 13:09:56.000000 oic-1.6.0/tests/test_popjwt.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     2725 2023-03-27 11:11:37.000000 oic-1.6.0/tests/test_sanitize.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    27871 2021-02-12 13:09:56.000000 oic-1.6.0/tests/test_sdb.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     1595 2021-02-12 13:09:56.000000 oic-1.6.0/tests/test_shelve_wrapper.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     4871 2023-03-27 11:11:37.000000 oic-1.6.0/tests/test_signed_http_request.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)      914 2021-02-12 13:09:56.000000 oic-1.6.0/tests/test_stateless.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     6728 2021-02-12 13:09:56.000000 oic-1.6.0/tests/test_time_util.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    16929 2023-05-02 08:00:09.000000 oic-1.6.0/tests/test_token.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     4695 2023-05-02 08:00:09.000000 oic-1.6.0/tests/test_token_handler.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     4270 2023-03-27 11:11:37.000000 oic-1.6.0/tests/test_user.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    10676 2023-03-27 11:11:37.000000 oic-1.6.0/tests/test_util.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     7150 2021-02-12 13:09:56.000000 oic-1.6.0/tests/test_webfinger.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)     8586 2023-05-02 08:00:09.000000 oic-1.6.0/tests/test_x_client.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    11688 2021-02-12 13:09:56.000000 oic-1.6.0/tests/test_x_dynreg.py
+-rw-r--r--   0 tomas     (1000) tomas     (1000)    20499 2023-05-02 08:00:09.000000 oic-1.6.0/tests/test_x_provider.py
```

### Comparing `oic-1.5.0/LICENSE.txt` & `oic-1.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/PKG-INFO` & `oic-1.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: oic
-Version: 1.5.0
+Version: 1.6.0
 Summary: Python implementation of OAuth2 and OpenID Connect
-Home-page: https://github.com/OpenIDC/pyoidc/
+Home-page: https://github.com/CZ-NIC/pyoidc/
 Author: Roland Hedberg
 Author-email: roland@catalogix.se
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -33,56 +33,56 @@
 
 .. image:: https://img.shields.io/pypi/v/oic.svg
     :target: https://pypi.python.org/pypi/oic
 
 .. image:: https://readthedocs.org/projects/pyoidc/badge/?version=latest
     :target: http://pyoidc.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://codecov.io/gh/OpenIDC/pyoidc/branch/master/graph/badge.svg
-  :target: https://codecov.io/gh/OpenIDC/pyoidc
+.. image:: https://codecov.io/gh/CZ-NIC/pyoidc/branch/master/graph/badge.svg
+  :target: https://codecov.io/gh/CZ-NIC/pyoidc
 
 .. image:: https://api.codacy.com/project/badge/Grade/2038cfa7c56b480db6ae18b8320d7157
-    :target: https://www.codacy.com/app/tpazderka/pyoidc?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=OpenIDC/pyoidc&amp;utm_campaign=Badge_Grade
+    :target: https://www.codacy.com/app/tpazderka/pyoidc?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=CZ-NIC/pyoidc&amp;utm_campaign=Badge_Grade
 
 A Python OpenID Connect implementation
 ======================================
 
 This is a complete implementation of OpenID Connect as specified in the `OpenID
 Connect Core specification`_. And as a side effect, a complete implementation
 of OAuth2.0 too.
 
 Please see the `CHANGELOG.md`_ to review the latest changes.
 
 .. _OpenID Connect Core specification: http://openid.net/specs/openid-connect-core-1_0.html
-.. _CHANGELOG.md: https://github.com/OpenIDC/pyoidc/blob/master/CHANGELOG.md
+.. _CHANGELOG.md: https://github.com/CZ-NIC/pyoidc/blob/master/CHANGELOG.md
 
 Documentation
 ==============
 
 The `documentation`_ is graciously hosted by `Read the Docs`_. Unfortunately,
 the documentation has been largely left unmaintained and `there are various
 issues`_. However, the maintainers are trying to remedy this lately with some
 new momentum. Please help us by submitting pull requests if you can help
 improve the documentation.
 
 .. _documentation: http://pyoidc.rtfd.io
 .. _Read the Docs: https://readthedocs.org/
-.. _there are various issues: https://github.com/OpenIDC/pyoidc/issues?q=is%3Aopen+is%3Aissue+label%3Adocumentation
+.. _there are various issues: https://github.com/CZ-NIC/pyoidc/issues?q=is%3Aopen+is%3Aissue+label%3Adocumentation
 
 Examples
 ========
 
 Unfortunately, the current examples included in this repository are
 unmaintained and `there are many issues`_. We're currently in the process of
 creating a working canonical example implementation, however, until that time,
 the current examples largely do not work. Please help us by submitting pull
 requests that may bring these examples back into a working condition if you
 get something working locally.
 
-.. _there are many issues: https://github.com/OpenIDC/pyoidc/issues?q=is%3Aopen+is%3Aissue+label%3Aexamples
+.. _there are many issues: https://github.com/CZ-NIC/pyoidc/issues?q=is%3Aopen+is%3Aissue+label%3Aexamples
 
 Acknowledgements
 ================
 
 Cudos to Vladislav Mladenov and Christian Mainka both at
 Horst Görtz Institute for IT-Security, Ruhr-University Bochum, Germany
 for helping me making the implementation more secure.
@@ -102,15 +102,15 @@
 .. _@schlenk: https://github.com/schlenk
 
 Contribute
 ==========
 
 `Fork the repository`_, clone your copy and `install pipenv`_.
 
-.. _Fork the repository: https://github.com/OpenIDC/pyoidc#fork-destination-box
+.. _Fork the repository: https://github.com/CZ-NIC/pyoidc#fork-destination-box
 .. _install pipenv: https://pipenv.readthedocs.io/en/latest/
 
 Then just run:
 
 .. code:: bash
 
     $ make install
@@ -122,16 +122,16 @@
     $ make test
 
 This will not affect your system level Python installation. Please review `our
 issues`_ to see what needs working on. Do not hesitate to ask questions if
 something is unclear. We mark easy issues as `newcomer-friendly`_, so they are
 a good place to start if you want to contribute.
 
-.. _our issues: https://github.com/OpenIDC/pyoidc/issues
-.. _newcomer-friendly: https://github.com/OpenIDC/pyoidc/issues?q=is%3Aopen+is%3Aissue+label%3Anewcomer-friendly
+.. _our issues: https://github.com/CZ-NIC/pyoidc/issues
+.. _newcomer-friendly: https://github.com/CZ-NIC/pyoidc/issues?q=is%3Aopen+is%3Aissue+label%3Anewcomer-friendly
 
 Windows
 -------
 
 If you happen to work in a Windows environment, the above will not work out of the box due to the lack
 of a ``GNU Make`` on Windows. In addition one of the dependencies for ``ldap_authn`` is not available as a prebuilt
 wheel from pypi, so use these slightly modified instructions.
```

### Comparing `oic-1.5.0/README.rst` & `oic-1.6.0/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -6,56 +6,56 @@
 
 .. image:: https://img.shields.io/pypi/v/oic.svg
     :target: https://pypi.python.org/pypi/oic
 
 .. image:: https://readthedocs.org/projects/pyoidc/badge/?version=latest
     :target: http://pyoidc.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://codecov.io/gh/OpenIDC/pyoidc/branch/master/graph/badge.svg
-  :target: https://codecov.io/gh/OpenIDC/pyoidc
+.. image:: https://codecov.io/gh/CZ-NIC/pyoidc/branch/master/graph/badge.svg
+  :target: https://codecov.io/gh/CZ-NIC/pyoidc
 
 .. image:: https://api.codacy.com/project/badge/Grade/2038cfa7c56b480db6ae18b8320d7157
-    :target: https://www.codacy.com/app/tpazderka/pyoidc?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=OpenIDC/pyoidc&amp;utm_campaign=Badge_Grade
+    :target: https://www.codacy.com/app/tpazderka/pyoidc?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=CZ-NIC/pyoidc&amp;utm_campaign=Badge_Grade
 
 A Python OpenID Connect implementation
 ======================================
 
 This is a complete implementation of OpenID Connect as specified in the `OpenID
 Connect Core specification`_. And as a side effect, a complete implementation
 of OAuth2.0 too.
 
 Please see the `CHANGELOG.md`_ to review the latest changes.
 
 .. _OpenID Connect Core specification: http://openid.net/specs/openid-connect-core-1_0.html
-.. _CHANGELOG.md: https://github.com/OpenIDC/pyoidc/blob/master/CHANGELOG.md
+.. _CHANGELOG.md: https://github.com/CZ-NIC/pyoidc/blob/master/CHANGELOG.md
 
 Documentation
 ==============
 
 The `documentation`_ is graciously hosted by `Read the Docs`_. Unfortunately,
 the documentation has been largely left unmaintained and `there are various
 issues`_. However, the maintainers are trying to remedy this lately with some
 new momentum. Please help us by submitting pull requests if you can help
 improve the documentation.
 
 .. _documentation: http://pyoidc.rtfd.io
 .. _Read the Docs: https://readthedocs.org/
-.. _there are various issues: https://github.com/OpenIDC/pyoidc/issues?q=is%3Aopen+is%3Aissue+label%3Adocumentation
+.. _there are various issues: https://github.com/CZ-NIC/pyoidc/issues?q=is%3Aopen+is%3Aissue+label%3Adocumentation
 
 Examples
 ========
 
 Unfortunately, the current examples included in this repository are
 unmaintained and `there are many issues`_. We're currently in the process of
 creating a working canonical example implementation, however, until that time,
 the current examples largely do not work. Please help us by submitting pull
 requests that may bring these examples back into a working condition if you
 get something working locally.
 
-.. _there are many issues: https://github.com/OpenIDC/pyoidc/issues?q=is%3Aopen+is%3Aissue+label%3Aexamples
+.. _there are many issues: https://github.com/CZ-NIC/pyoidc/issues?q=is%3Aopen+is%3Aissue+label%3Aexamples
 
 Acknowledgements
 ================
 
 Cudos to Vladislav Mladenov and Christian Mainka both at
 Horst Görtz Institute for IT-Security, Ruhr-University Bochum, Germany
 for helping me making the implementation more secure.
@@ -75,15 +75,15 @@
 .. _@schlenk: https://github.com/schlenk
 
 Contribute
 ==========
 
 `Fork the repository`_, clone your copy and `install pipenv`_.
 
-.. _Fork the repository: https://github.com/OpenIDC/pyoidc#fork-destination-box
+.. _Fork the repository: https://github.com/CZ-NIC/pyoidc#fork-destination-box
 .. _install pipenv: https://pipenv.readthedocs.io/en/latest/
 
 Then just run:
 
 .. code:: bash
 
     $ make install
@@ -95,16 +95,16 @@
     $ make test
 
 This will not affect your system level Python installation. Please review `our
 issues`_ to see what needs working on. Do not hesitate to ask questions if
 something is unclear. We mark easy issues as `newcomer-friendly`_, so they are
 a good place to start if you want to contribute.
 
-.. _our issues: https://github.com/OpenIDC/pyoidc/issues
-.. _newcomer-friendly: https://github.com/OpenIDC/pyoidc/issues?q=is%3Aopen+is%3Aissue+label%3Anewcomer-friendly
+.. _our issues: https://github.com/CZ-NIC/pyoidc/issues
+.. _newcomer-friendly: https://github.com/CZ-NIC/pyoidc/issues?q=is%3Aopen+is%3Aissue+label%3Anewcomer-friendly
 
 Windows
 -------
 
 If you happen to work in a Windows environment, the above will not work out of the box due to the lack
 of a ``GNU Make`` on Windows. In addition one of the dependencies for ``ldap_authn`` is not available as a prebuilt
 wheel from pypi, so use these slightly modified instructions.
```

### Comparing `oic-1.5.0/setup.py` & `oic-1.6.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     name="oic",
     version=version,
     description="Python implementation of OAuth2 and OpenID Connect",
     long_description=open('README.rst', encoding='utf-8').read(),
     author="Roland Hedberg",
     author_email="roland@catalogix.se",
     license="Apache 2.0",
-    url='https://github.com/OpenIDC/pyoidc/',
+    url='https://github.com/CZ-NIC/pyoidc/',
     packages=[
         "oic", "oic/oauth2", "oic/oic", "oic/utils", "oic/utils/authn",
         "oic/utils/userinfo", 'oic/utils/rp', 'oic/extension'
     ],
     entry_points={
         'console_scripts': [
             'oic-client-management = oic.utils.client_management:run'
@@ -74,27 +74,28 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries :: Python Modules"],
     python_requires='~=3.7',
     extras_require={
         'develop': ["cherrypy==3.2.4", "pyOpenSSL"],
         'testing': tests_requires,
-        'docs': ['Sphinx', 'sphinx-autobuild', 'alabaster'],
+        'docs': ['Sphinx', 'sphinx-autobuild', 'alabaster', 'autodoc_pydantic'],
         'quality': ['pylama', 'isort', 'eradicate', 'mypy', 'black', 'bandit', 'readme_renderer[md]'],
         'types': ['types-requests'],
         'ldap_authn': ['python-ldap'],
         'examples': ['beaker'],
     },
     install_requires=[
         "requests",
         "pycryptodomex",
+        "pydantic",
         "pyjwkest>=1.3.6",
         "mako",
         "cryptography",
         "defusedxml",
-        "typing_extensions",
+        'typing_extensions; python_version<"3.8"',
     ],
     tests_require=tests_requires,
     long_description_content_type="text/x-rst",
     zip_safe=False,
     cmdclass={'test': PyTest},
 )
```

### Comparing `oic-1.5.0/src/oic/__init__.py` & `oic-1.6.0/src/oic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         warnings.warn(
             "No good random number generator available on this platform. "
             "Security tokens will be weak and guessable.",
             RuntimeWarning,
         )
 
 __author__ = "Roland Hedberg"
-__version__ = "1.5.0"
+__version__ = "1.6.0"
 
 
 OIDCONF_PATTERN = "%s/.well-known/openid-configuration"
 CC_METHOD = {"S256": hashlib.sha256, "S384": hashlib.sha384, "S512": hashlib.sha512}
 
 
 def rndstr(size=16):
```

### Comparing `oic-1.5.0/src/oic/exception.py` & `oic-1.6.0/src/oic/exception.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/extension/client.py` & `oic-1.6.0/src/oic/extension/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,14 @@
         method="GET",
         request_args=None,
         extra_args=None,
         http_args=None,
         response_cls=None,
         **kwargs,
     ):
-
         url, body, ht_args, _ = self.request_info(
             request, method, request_args, extra_args, **kwargs
         )
 
         if http_args is None:
             http_args = ht_args
         else:
```

### Comparing `oic-1.5.0/src/oic/extension/device_flow.py` & `oic-1.6.0/src/oic/extension/device_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
         self.client_id2device: Dict[str, str] = {}
         self.device2user: Dict[str, str] = {}
         self.user_auth: Dict[str, bool] = {}
         self.device_code_expire_at: Dict[str, int] = {}
         self.device_code_life_time = 900  # 15 minutes
 
     def device_endpoint(self, request, authn=None):
-
         _req = AuthorizationRequest(**request)
         device_code = rndstr(10)
         user_code = rndstr(6)
 
         self.device2user[device_code] = user_code
         self.user_auth[user_code] = False
         self.client_id2device[_req["client_id"]] = device_code
```

### Comparing `oic-1.5.0/src/oic/extension/heart.py` & `oic-1.6.0/src/oic/extension/heart.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/extension/message.py` & `oic-1.6.0/src/oic/extension/message.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/extension/pop.py` & `oic-1.6.0/src/oic/extension/pop.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/extension/popjwt.py` & `oic-1.6.0/src/oic/extension/popjwt.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/extension/proof_of_possesion.py` & `oic-1.6.0/src/oic/extension/proof_of_possesion.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/extension/provider.py` & `oic-1.6.0/src/oic/extension/provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,14 @@
         hostname="",
         config=None,
         behavior=None,
         lifetime_policy=None,
         message_factory=ExtensionMessageFactory,
         **kwargs,
     ):
-
         if not name.endswith("/"):
             name += "/"
 
         try:
             args = {"server_cls": kwargs["server_cls"]}
         except KeyError:
             args = {}
```

### Comparing `oic-1.5.0/src/oic/extension/signed_http_req.py` & `oic-1.6.0/src/oic/extension/signed_http_req.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/extension/sts.py` & `oic-1.6.0/src/oic/extension/sts.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/extension/token.py` & `oic-1.6.0/src/oic/extension/token.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/oauth2/__init__.py` & `oic-1.6.0/src/oic/oauth2/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -405,25 +405,23 @@
     def construct_Message(
         self,
         request: Type[Message] = Message,
         request_args=None,
         extra_args=None,
         **kwargs,
     ) -> Message:
-
         return self.construct_request(request, request_args, extra_args)
 
     def construct_AuthorizationRequest(
         self,
         request: Optional[Type[AuthorizationRequest]] = None,
         request_args=None,
         extra_args=None,
         **kwargs,
     ) -> AuthorizationRequest:
-
         if request is None:
             request = self.message_factory.get_request_type("authorization_endpoint")
         if request_args is not None:
             try:  # change default
                 new = request_args["redirect_uri"]
                 if new:
                     self.redirect_uris = [new]
@@ -449,15 +447,14 @@
                 Type[ExtensionTokenRequest],
             ]
         ] = None,
         request_args=None,
         extra_args=None,
         **kwargs,
     ) -> AccessTokenRequest:
-
         if request is None:
             request = self.message_factory.get_request_type("token_endpoint")
         if request_args is None:
             request_args = {}
         if not issubclass(
             request,
             (
@@ -493,15 +490,14 @@
     def construct_RefreshAccessTokenRequest(
         self,
         request: Optional[Type[RefreshAccessTokenRequest]] = None,
         request_args=None,
         extra_args=None,
         **kwargs,
     ) -> RefreshAccessTokenRequest:
-
         if request is None:
             request = self.message_factory.get_request_type("refresh_endpoint")
         if request_args is None:
             request_args = {}
 
         token = self.get_token(also_expired=True, **kwargs)
 
@@ -517,15 +513,14 @@
     def construct_ResourceRequest(
         self,
         request: Optional[Type[ResourceRequest]] = None,
         request_args=None,
         extra_args=None,
         **kwargs,
     ) -> ResourceRequest:
-
         if request is None:
             request = self.message_factory.get_request_type("resource_endpoint")
         if request_args is None:
             request_args = {}
 
         token = self.get_token(**kwargs)
 
@@ -558,15 +553,14 @@
         request: Type[Message],
         method="POST",
         request_args=None,
         extra_args=None,
         lax=False,
         **kwargs,
     ) -> Tuple[str, str, Dict, Message]:
-
         if request_args is None:
             request_args = {}
 
         try:
             cls = getattr(self, "construct_%s" % request.__name__)
             cis = cls(request_args=request_args, extra_args=extra_args, **kwargs)
         except AttributeError:
@@ -718,15 +712,14 @@
                 if "sid" in resp["id_token"]:
                     session_update(self.sso_db, _state, "smid", resp["id_token"]["sid"])
         return resp
 
     def init_authentication_method(
         self, cis, authn_method, request_args=None, http_args=None, **kwargs
     ):
-
         if http_args is None:
             http_args = {}
         if request_args is None:
             request_args = {}
 
         if authn_method:
             return self.client_authn_method[authn_method](self).construct(
@@ -739,30 +732,24 @@
         self,
         reqresp: requests.Response,
         response: Optional[Type[Message]] = None,
         body_type: Optional[ENCODINGS] = None,
         state="",
         **kwargs,
     ) -> Union[Message, requests.Response]:
-
         # Handle the early return stuff
         if reqresp.status_code in [302, 303]:  # redirect
             return reqresp
         elif reqresp.status_code == 500:
             logger.error("(%d) %s" % (reqresp.status_code, sanitize(reqresp.text)))
             raise ParseError("ERROR: Something went wrong: %s" % reqresp.text)
 
-        if reqresp.status_code in SUCCESSFUL:
-            verified_body_type = verify_header(reqresp, body_type)
-        elif (
-            reqresp.status_code in [400, 401]
-            and response
-            and issubclass(response, ErrorResponse)
+        if reqresp.status_code in SUCCESSFUL or (
+            reqresp.status_code in [400, 401] and response
         ):
-            # This is okay if we are expecting an error response, do not log
             verified_body_type = verify_header(reqresp, body_type)
         else:
             # Any other error
             logger.error("(%d) %s" % (reqresp.status_code, sanitize(reqresp.text)))
             raise HttpError(
                 "HTTP ERROR: %s [%s] on %s"
                 % (reqresp.text, reqresp.status_code, reqresp.url)
@@ -841,15 +828,14 @@
         body_type="",
         method="GET",
         request_args=None,
         extra_args=None,
         http_args=None,
         **kwargs,
     ) -> AuthorizationResponse:
-
         request = self.message_factory.get_request_type("authorization_endpoint")
         response_cls = self.message_factory.get_response_type("authorization_endpoint")
 
         if state:
             try:
                 request_args["state"] = state
             except TypeError:
@@ -901,15 +887,14 @@
         method="POST",
         request_args=None,
         extra_args=None,
         http_args=None,
         authn_method="",
         **kwargs,
     ) -> AccessTokenResponse:
-
         request = self.message_factory.get_request_type("token_endpoint")
         response_cls = self.message_factory.get_response_type("token_endpoint")
 
         if extra_args is None:
             extra_args = {}
         kwargs["authn_endpoint"] = "token"
         if http_args is not None and "password" in http_args:
@@ -958,15 +943,14 @@
         method="POST",
         request_args=None,
         extra_args=None,
         http_args=None,
         authn_method="",
         **kwargs,
     ) -> AccessTokenResponse:
-
         request = self.message_factory.get_request_type("refresh_endpoint")
         response_cls = self.message_factory.get_response_type("refresh_endpoint")
 
         token = self.get_token(also_expired=True, state=state, **kwargs)
         kwargs["authn_endpoint"] = "refresh"
         url, body, ht_args, csi = self.request_info(
             request,
@@ -1007,15 +991,14 @@
         method="POST",
         request_args=None,
         extra_args=None,
         http_args=None,
         response: Optional[Type[Message]] = None,
         authn_method="",
     ) -> Message:
-
         url, body, ht_args, _ = self.request_info(
             request,
             method=method,
             request_args=request_args,
             extra_args=extra_args,
             scope=scope,
             state=state,
@@ -1031,15 +1014,14 @@
         return self.request_and_return(
             url, response, method, body, body_type, state=state, http_args=http_args
         )
 
     def fetch_protected_resource(
         self, uri, method="GET", headers=None, state="", **kwargs
     ):
-
         if "token" in kwargs and kwargs["token"]:
             token = kwargs["token"]
             request_args = {"access_token": token}
         else:
             try:
                 token = self.get_token(state=state, **kwargs)
             except ExpiredToken:
@@ -1152,15 +1134,14 @@
     def provider_config(
         self,
         issuer: str,
         keys: bool = True,
         endpoints: bool = True,
         serv_pattern: str = OIDCONF_PATTERN,
     ) -> ASConfigurationResponse:
-
         response_cls = self.message_factory.get_response_type("configuration_endpoint")
         if issuer.endswith("/"):
             _issuer = issuer[:-1]
         else:
             _issuer = issuer
 
         url = serv_pattern % _issuer
@@ -1251,15 +1232,14 @@
         self,
         request: Type[Message] = AuthorizationRequest,
         txt: str = "",
         keyjar: Optional[KeyJar] = None,
         verify: bool = True,
         **kwargs,
     ) -> Message:
-
         if not keyjar:
             keyjar = self.keyjar
 
         areq = request().deserialize(txt, "jwt", keyjar=keyjar, verify=verify, **kwargs)
         if verify:
             areq.verify()
         return areq
```

### Comparing `oic-1.5.0/src/oic/oauth2/base.py` & `oic-1.6.0/src/oic/oauth2/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,9 +164,8 @@
         self, filename, ignore_discard=False, ignore_expires=False
     ):
         self.cookiejar.load(filename, ignore_discard, ignore_expires)
 
     def save_cookies_to_file(
         self, filename, ignore_discard=False, ignore_expires=False
     ):
-
         self.cookiejar.save(filename, ignore_discard, ignore_expires)
```

### Comparing `oic-1.5.0/src/oic/oauth2/consumer.py` & `oic-1.6.0/src/oic/oauth2/consumer.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/oauth2/exception.py` & `oic-1.6.0/src/oic/oauth2/exception.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/oauth2/grant.py` & `oic-1.6.0/src/oic/oauth2/grant.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/oauth2/message.py` & `oic-1.6.0/src/oic/oauth2/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -479,15 +479,14 @@
         :param algorithm: The signature algorithm to use
         :return: A signed JWT
         """
         _jws = JWS(self.to_json(lev), alg=algorithm)
         return _jws.sign_compact(key)
 
     def _add_key(self, keyjar, issuer, key, key_type="", kid="", no_kid_issuer=None):
-
         if issuer not in keyjar:
             logger.error('Issuer "{}" not in keyjar'.format(issuer))
             return
 
         logger.debug(
             "Key set summary for {}: {}".format(issuer, key_summary(keyjar, issuer))
         )
```

### Comparing `oic-1.5.0/src/oic/oauth2/provider.py` & `oic-1.6.0/src/oic/oauth2/provider.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/oauth2/util.py` & `oic-1.6.0/src/oic/oauth2/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 import logging
+import sys
 from http import cookiejar as http_cookiejar
 from http.cookiejar import http2time  # type: ignore
 from typing import Any
 from typing import Dict
 from typing import Optional
 from urllib.parse import parse_qs
 from urllib.parse import urlsplit
 from urllib.parse import urlunsplit
 
-from typing_extensions import Literal
-
 from oic.exception import UnSupported
 from oic.oauth2.exception import TimeFormatError
 from oic.utils.sanitize import sanitize
 
+if sys.version_info >= (3, 8):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+
 logger = logging.getLogger(__name__)
 
 __author__ = "roland"
 
 URL_ENCODED = "application/x-www-form-urlencoded"
 JSON_ENCODED = "application/json"
```

### Comparing `oic-1.5.0/src/oic/oic/__init__.py` & `oic-1.6.0/src/oic/oic/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -497,15 +497,14 @@
             return webname[len(self.base_url) :]
         else:
             raise ValueError("Invalid webname, must start with base_url")
 
     def construct_AuthorizationRequest(
         self, request=None, request_args=None, extra_args=None, **kwargs
     ):
-
         if request_args is not None:
             if "nonce" not in request_args:
                 _rt = request_args["response_type"]
                 if "token" in _rt or "id_token" in _rt:
                     request_args["nonce"] = rndstr(32)
         elif "response_type" in kwargs:
             if "token" in kwargs["response_type"]:
@@ -570,15 +569,14 @@
                 areq["request_uri"] = _webname
 
         return areq
 
     def construct_UserInfoRequest(
         self, request=None, request_args=None, extra_args=None, **kwargs
     ):
-
         if request is None:
             request = self.message_factory.get_request_type("userinfo_endpoint")
         if request_args is None:
             request_args = {}
 
         if "access_token" in request_args:
             pass
@@ -604,15 +602,14 @@
         self, request=None, request_args=None, extra_args=None, **kwargs
     ):
         if request is None:
             request = self.message_factory.get_request_type("refreshsession_endpoint")
         return self.construct_request(request, request_args, extra_args)
 
     def _id_token_based(self, request, request_args=None, extra_args=None, **kwargs):
-
         if request_args is None:
             request_args = {}
 
         try:
             _prop = kwargs["prop"]
         except KeyError:
             _prop = "id_token"
@@ -650,15 +647,14 @@
         self,
         request=None,
         request_args=None,
         extra_args=None,
         prop="id_token_hint",
         **kwargs,
     ):
-
         if request is None:
             request = self.message_factory.get_request_type("endsession_endpoint")
         if request_args is None:
             request_args = {}
 
         if "state" in request_args and "state" not in kwargs:
             kwargs["state"] = request_args["state"]
@@ -765,15 +761,14 @@
         state="",
         body_type="json",
         method="GET",
         request_args=None,
         extra_args=None,
         http_args=None,
     ):
-
         request = self.message_factory.get_request_type("checksession_endpoint")
         response_cls = self.message_factory.get_response_type("checksession_endpoint")
 
         url, body, ht_args, csi = self.request_info(
             request,
             method=method,
             request_args=request_args,
@@ -940,15 +935,14 @@
         h_args = dict([(k, v) for k, v in kwargs.items() if k in HTTP_ARGS])
 
         return path, body, method, h_args
 
     def do_user_info_request(
         self, method="POST", state="", scope="openid", request="openid", **kwargs
     ):
-
         kwargs["request"] = request
         path, body, method, h_args = self.user_info_request(
             method, state, scope, **kwargs
         )
 
         logger.debug(
             "[do_user_info_request] PATH:%s BODY:%s H_ARGS: %s"
@@ -1030,15 +1024,14 @@
         self.store_response(res, _txt)
 
         return res
 
     def get_userinfo_claims(
         self, access_token, endpoint, method="POST", schema_class=OpenIDSchema, **kwargs
     ):
-
         uir = UserInfoRequest(access_token=access_token)
 
         h_args = dict([(k, v) for k, v in kwargs.items() if k in HTTP_ARGS])
 
         if "authn_method" in kwargs:
             http_args = self.init_authentication_method(**kwargs)
         else:
```

### Comparing `oic-1.5.0/src/oic/oic/claims_provider.py` & `oic-1.6.0/src/oic/oic/claims_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,14 @@
 
         self.srvmethod = OICCServer(keyjar=keyjar)
         self.dist_claims_mode = dist_claims_mode
         self.info_store: Dict[str, Any] = {}
         self.claims_userinfo_endpoint = ""
 
     def _aggregation(self, info):
-
         jwt_key = self.keyjar.get_signing_key()
         cresp = UserClaimsResponse(
             jwt=info.to_jwt(key=jwt_key, algorithm="RS256"),
             claims_names=list(info.keys()),
         )
 
         logger.info("RESPONSE: %s" % (sanitize(cresp.to_dict()),))
@@ -204,28 +203,26 @@
         self.request2endpoint["UserClaimsRequest"] = "userclaims_endpoint"
         self.response2error = RESPONSE2ERROR.copy()
         self.response2error["UserClaimsResponse"] = ["ErrorResponse"]
 
     def construct_UserClaimsRequest(
         self, request=UserClaimsRequest, request_args=None, extra_args=None, **kwargs
     ):
-
         return self.construct_request(request, request_args, extra_args)
 
     def do_claims_request(
         self,
         request=UserClaimsRequest,
         request_resp=UserClaimsResponse,
         body_type="json",
         method="POST",
         request_args=None,
         extra_args=None,
         http_args=None,
     ):
-
         url, body, ht_args, _ = self.request_info(
             request, method=method, request_args=request_args, extra_args=extra_args
         )
 
         if http_args is None:
             http_args = ht_args
         else:
```

### Comparing `oic-1.5.0/src/oic/oic/consumer.py` & `oic-1.6.0/src/oic/oic/consumer.py`

 * *Files 2% similar despite different names*

```diff
@@ -457,18 +457,27 @@
             aresp = atr = None
 
         # Verify the IdToken if it was present
         if idt is not None:
             self.verify_id_token(idt, self.authz_req.get(_state or atr["state"]))
         return aresp, atr, idt
 
-    def complete(self, state):
+    def complete(
+        self,
+        state,
+        authn_method: str = "client_secret_basic",
+        session_state: Optional[str] = None,
+    ):
         """
         Do the access token request, the last step in a code flow.
 
+        'session_state' is an optional parameter that can be provided if the Authorization Server support OIDC Session
+        Management.
+        If provided, it is used as the key in the session database to store the consumer data.
+
         If Implicit flow was used then this method is never used.
         """
         args = {"redirect_uri": self.redirect_uris[0]}
         if "password" in self.consumer_config and self.consumer_config["password"]:
             logger.info("basic auth")
             http_args = {"password": self.consumer_config["password"]}
         elif self.client_secret:
@@ -481,23 +490,31 @@
                     "secret_type": self.secret_type,
                 }
             )
         else:
             raise PyoidcError("Nothing to authenticate with")
 
         resp = self.do_access_token_request(
-            state=state, request_args=args, http_args=http_args
+            state=state,
+            request_args=args,
+            http_args=http_args,
+            authn_method=authn_method,
         )
 
         logger.info("Access Token Response: %s" % sanitize(resp))
 
         if resp.type() == "ErrorResponse":
             raise TokenError(resp.error, resp)
 
-        self._backup(state)
+        if session_state is not None:
+            # Use session_state from Authorization server, as per §2
+            # from https://openid.net/specs/openid-connect-session-1_0.html
+            self._backup(session_state)
+        else:
+            self._backup(state)
 
         return resp
 
     def refresh_token(self):
         pass
 
     def get_user_info(self, state):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `oic-1.5.0/src/oic/oic/message.py` & `oic-1.6.0/src/oic/oic/message.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/oic/provider.py` & `oic-1.6.0/src/oic/oic/provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -401,15 +401,14 @@
         access_token=None,
         user_info=None,
         auth_time=0,
         exp=None,
         extra_claims=None,
         **kwargs,
     ):
-
         if alg == "":
             alg = self.jwx_def["signing_alg"]["id_token"]
 
         if alg:
             logger.debug("Signing alg: %s [%s]" % (alg, alg2keytype(alg)))
         else:
             alg = "none"
```

### Comparing `oic-1.5.0/src/oic/utils/__init__.py` & `oic-1.6.0/src/oic/utils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import traceback
 
 __author__ = "rohe0002"
 
 
-def tobytes(value):
+def tobytes(value) -> bytes:
     """Convert value to bytes."""
     if isinstance(value, bytes):
         return value
     else:
         if isinstance(value, str):
             return value.encode()
         else:
```

### Comparing `oic-1.5.0/src/oic/utils/aes.py` & `oic-1.6.0/src/oic/utils/aes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 #!/usr/bin/env python
+import sys
 from base64 import b64decode
 from base64 import b64encode
+from typing import Dict
 from typing import Union
 from typing import cast
 
 from Cryptodome import Random
 from Cryptodome.Cipher import AES
 from Cryptodome.Cipher._mode_ccm import CcmMode
 from Cryptodome.Cipher._mode_eax import EaxMode
 from Cryptodome.Cipher._mode_gcm import GcmMode
 from Cryptodome.Cipher._mode_ocb import OcbMode
 from Cryptodome.Cipher._mode_siv import SivMode
 
 from oic.utils import tobytes
 
+if sys.version_info >= (3, 8):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+
 __author__ = "rolandh"
 
-POSTFIX_MODE = {"cbc": AES.MODE_CBC, "cfb": AES.MODE_CFB, "ecb": AES.MODE_CFB}
+POSTFIX_MODE: Dict[str, Union[Literal[2], Literal[3]]] = {
+    "cbc": AES.MODE_CBC,
+    "cfb": AES.MODE_CFB,
+    "ecb": AES.MODE_CFB,
+}
 
 BLOCK_SIZE = 16
 
 
 class AESError(Exception):
     pass
```

### Comparing `oic-1.5.0/src/oic/utils/authn/authn_context.py` & `oic-1.6.0/src/oic/utils/authn/authn_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,15 +204,15 @@
     :param callback: function to execute for the callback URL at the OP, see UserAuthnMethod.verify and its subclasses
     (e.g. SAMLAuthnMethod) for signature
     :param next_module_instance: an object instance of the module next in the chain after the module whose verify method
     is the callback -- do not use this parameter!! If you want a multi auth chain see the convenience function
     setup_multi_auth (in multi_auth.py)
     :return: function encapsulating the specified callback which properly handles a multi auth chain.
     """
-    # This has to be here ...
+
     def auth_verify(environ, start_response, logger=None):
         kwargs = extract_from_request(environ)
 
         response, auth_is_complete = callback(**kwargs)
 
         if auth_is_complete and next_module_instance:
             response = next_module_instance(**kwargs)
```

### Comparing `oic-1.5.0/src/oic/utils/authn/client.py` & `oic-1.6.0/src/oic/utils/authn/client.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/utils/authn/client_saml.py` & `oic-1.6.0/src/oic/utils/authn/client_saml.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/utils/authn/javascript_login.py` & `oic-1.6.0/src/oic/utils/authn/javascript_login.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/utils/authn/ldap_member.py` & `oic-1.6.0/src/oic/utils/authn/ldap_member.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/utils/authn/ldapc.py` & `oic-1.6.0/src/oic/utils/authn/ldapc.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/utils/authn/multi_auth.py` & `oic-1.6.0/src/oic/utils/authn/multi_auth.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/utils/authn/saml.py` & `oic-1.6.0/src/oic/utils/authn/saml.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,14 @@
         self.sp = Saml2Client(config=config)
         mte = lookup.get_template("unauthorized.mako")
         argv = {"message": "You are not authorized!"}
         self.not_authorized = mte.render(**argv)
         self.samlcache = self.sp_conf.SAML_CACHE  # type: ignore
 
     def __call__(self, query="", end_point_index=None, *args, **kwargs):
-
         (done, response) = self._pick_idp(query, end_point_index)
         if done == 0:
             entity_id = response
             # Do the AuthnRequest
             resp = self._redirect_to_auth(self.sp, entity_id, query, end_point_index)
             return resp
         return response
```

### Comparing `oic-1.5.0/src/oic/utils/authn/user.py` & `oic-1.6.0/src/oic/utils/authn/user.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/utils/authn/user_cas.py` & `oic-1.6.0/src/oic/utils/authn/user_cas.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,30 +37,34 @@
     CONST_NONCE = "nonce"
     # Parameter name for queries to be sent back on the URL, after successful
     # authentication.
     CONST_QUERY = "query"
     # The name for the CAS cookie, containing query parameters and nonce.
     CONST_CAS_COOKIE = "cascookie"
 
-    def __init__(self, srv, cas_server, service_url, return_to, extra_validation=None):
+    def __init__(
+        self, srv, cas_server, service_url, return_to, extra_validation=None, timeout=5
+    ):
         """
         Construct the class.
 
         :param srv: Usually none, but otherwise the oic server.
         :param cas_server: Base URL to the cas server.
         :param service_url: BASE url to the service that will use CAS. In
         this case the oic server's verify URL.
         :param return_to: The URL to return to after a successful
         authentication.
+        :param timeout: Timeout for requests library.
         """
         UserAuthnMethod.__init__(self, srv)
         self.cas_server = cas_server
         self.service_url = service_url
         self.return_to = return_to
         self.extra_validation = extra_validation
+        self.timeout = timeout
 
     def create_redirect(self, query):
         """
         Perform the redirect to the CAS server.
 
         :rtype : Response
         :param query: All query parameters to be added to the return_to URL
@@ -97,15 +101,19 @@
 
         :rtype : String
         :param ticket: Onetime CAS ticket to be validated.
         :param service_url: The URL the CAS server redirected to.
         :return: Uid if the login was successful otherwise None.
         """
         data = {self.CONST_TICKET: ticket, self.CONST_SERVICE: service_url}
-        resp = requests.get(self.cas_server + self.CONST_CAS_VERIFY_TICKET, params=data)
+        resp = requests.get(
+            self.cas_server + self.CONST_CAS_VERIFY_TICKET,
+            params=data,
+            timeout=self.timeout,
+        )
         root = ET.fromstring(resp.content)
         for l1 in root:
             if self.CONST_AUTHSUCCESS in l1.tag:
                 for l2 in l1:
                     if self.CONST_USER in l2.tag:
                         if self.extra_validation is not None:
                             if self.extra_validation(l2.text):
```

### Comparing `oic-1.5.0/src/oic/utils/authz.py` & `oic-1.6.0/src/oic/utils/authz.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/utils/client_management.py` & `oic-1.6.0/src/oic/utils/client_management.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/utils/clientdb.py` & `oic-1.6.0/src/oic/utils/clientdb.py`

 * *Files 14% similar despite different names*

```diff
@@ -70,23 +70,24 @@
         """Return number of contained keys."""
         return len(self.keys())
 
 
 class MDQClient(BaseClientDatabase):
     """Implementation of remote client database."""
 
-    def __init__(self, url):
-        """Set the remote storage url."""
+    def __init__(self, url, timeout=5):
+        """Set the remote storage url and timeout for requests."""
         self.url = url
+        self.timeout = timeout
         self.headers = {"Accept": "application/json", "Accept-Encoding": "gzip"}
 
     def __getitem__(self, item):
         """Retrieve a single entity."""
         mdx_url = urljoin(self.url, "entities/{}".format(quote(item, safe="")))
-        response = requests.get(mdx_url, headers=self.headers)
+        response = requests.get(mdx_url, headers=self.headers, timeout=self.timeout)
         if response.status_code == 200:
             return response.json()
         else:
             raise NoClientInfoReceivedError(
                 "{} {}".format(response.status_code, response.reason)
             )
 
@@ -97,26 +98,26 @@
     def __delitem__(self, item):
         """Remote management is readonly."""
         raise RuntimeError("MDQClient is readonly.")
 
     def keys(self):
         """Get all registered entitites."""
         mdx_url = urljoin(self.url, "entities")
-        response = requests.get(mdx_url, headers=self.headers)
+        response = requests.get(mdx_url, headers=self.headers, timeout=self.timeout)
         if response.status_code == 200:
             return [item["client_id"] for item in response.json()]
         else:
             raise NoClientInfoReceivedError(
                 "{} {}".format(response.status_code, response.reason)
             )
 
     def items(self):
         """Geting all registered entities."""
         mdx_url = urljoin(self.url, "entities")
-        response = requests.get(mdx_url, headers=self.headers)
+        response = requests.get(mdx_url, headers=self.headers, timeout=self.timeout)
         if response.status_code == 200:
             return response.json()
         else:
             raise NoClientInfoReceivedError(
                 "{} {}".format(response.status_code, response.reason)
             )
```

### Comparing `oic-1.5.0/src/oic/utils/http_util.py` & `oic-1.6.0/src/oic/utils/http_util.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/utils/jwt.py` & `oic-1.6.0/src/oic/utils/jwt.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/utils/keyio.py` & `oic-1.6.0/src/oic/utils/keyio.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,21 +181,21 @@
 
         self.last_updated = time.time()
 
     def do_remote(self):
         if self.source is None:
             # Nothing to do
             return False
-        args = {"verify": self.verify_ssl, "timeout": self.timeout}
+        args = {"verify": self.verify_ssl}
         if self.etag:
             args["headers"] = {"If-None-Match": self.etag}
 
         try:
             logger.debug("KeyBundle fetch keys from: %s", self.source)
-            r = requests.get(self.source, **args)
+            r = requests.get(self.source, timeout=self.timeout, **args)
         except Exception as err:
             logger.error(err)
             raise_exception(UpdateFailed, REMOTE_FAILED.format(self.source, str(err)))
 
         if r.status_code == 304:  # file has not changed
             self.time_out = time.time() + self.cache_time
             self.last_updated = time.time()
```

### Comparing `oic-1.5.0/src/oic/utils/restrict.py` & `oic-1.6.0/src/oic/utils/restrict.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/utils/rp/__init__.py` & `oic-1.6.0/src/oic/utils/rp/__init__.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/utils/rp/oauth2.py` & `oic-1.6.0/src/oic/utils/rp/oauth2.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/utils/sanitize.py` & `oic-1.6.0/src/oic/utils/sanitize.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/utils/sdb.py` & `oic-1.6.0/src/oic/utils/sdb.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/utils/session_backend.py` & `oic-1.6.0/src/oic/utils/session_backend.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/utils/shelve_wrapper.py` & `oic-1.6.0/src/oic/utils/shelve_wrapper.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/utils/stateless.py` & `oic-1.6.0/src/oic/utils/stateless.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/utils/template_render.py` & `oic-1.6.0/src/oic/utils/template_render.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/utils/time_util.py` & `oic-1.6.0/src/oic/utils/time_util.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/utils/token_handler.py` & `oic-1.6.0/src/oic/utils/token_handler.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/utils/userinfo/__init__.py` & `oic-1.6.0/src/oic/utils/userinfo/__init__.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/utils/userinfo/aa_info.py` & `oic-1.6.0/src/oic/utils/userinfo/aa_info.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/utils/userinfo/distaggr.py` & `oic-1.6.0/src/oic/utils/userinfo/distaggr.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,14 @@
                 except KeyError:
                     pass
                 cc.userclaims_endpoint = specs["userclaims_endpoint"]
             res[cid] = cc
         return res
 
     def _collect_distributed(self, srv, cc, sub, what, alias=""):
-
         try:
             resp = cc.do_claims_request(request_args={"sub": sub, "claims_names": what})
         except Exception:
             raise
 
         result: Dict[str, Any] = {"_claims_names": {}, "_claims_sources": {}}
```

### Comparing `oic-1.5.0/src/oic/utils/userinfo/ldap_info.py` & `oic-1.6.0/src/oic/utils/userinfo/ldap_info.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic/utils/webfinger.py` & `oic-1.6.0/src/oic/utils/webfinger.py`

 * *Files identical despite different names*

### Comparing `oic-1.5.0/src/oic.egg-info/PKG-INFO` & `oic-1.6.0/src/oic.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: oic
-Version: 1.5.0
+Version: 1.6.0
 Summary: Python implementation of OAuth2 and OpenID Connect
-Home-page: https://github.com/OpenIDC/pyoidc/
+Home-page: https://github.com/CZ-NIC/pyoidc/
 Author: Roland Hedberg
 Author-email: roland@catalogix.se
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -33,56 +33,56 @@
 
 .. image:: https://img.shields.io/pypi/v/oic.svg
     :target: https://pypi.python.org/pypi/oic
 
 .. image:: https://readthedocs.org/projects/pyoidc/badge/?version=latest
     :target: http://pyoidc.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://codecov.io/gh/OpenIDC/pyoidc/branch/master/graph/badge.svg
-  :target: https://codecov.io/gh/OpenIDC/pyoidc
+.. image:: https://codecov.io/gh/CZ-NIC/pyoidc/branch/master/graph/badge.svg
+  :target: https://codecov.io/gh/CZ-NIC/pyoidc
 
 .. image:: https://api.codacy.com/project/badge/Grade/2038cfa7c56b480db6ae18b8320d7157
-    :target: https://www.codacy.com/app/tpazderka/pyoidc?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=OpenIDC/pyoidc&amp;utm_campaign=Badge_Grade
+    :target: https://www.codacy.com/app/tpazderka/pyoidc?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=CZ-NIC/pyoidc&amp;utm_campaign=Badge_Grade
 
 A Python OpenID Connect implementation
 ======================================
 
 This is a complete implementation of OpenID Connect as specified in the `OpenID
 Connect Core specification`_. And as a side effect, a complete implementation
 of OAuth2.0 too.
 
 Please see the `CHANGELOG.md`_ to review the latest changes.
 
 .. _OpenID Connect Core specification: http://openid.net/specs/openid-connect-core-1_0.html
-.. _CHANGELOG.md: https://github.com/OpenIDC/pyoidc/blob/master/CHANGELOG.md
+.. _CHANGELOG.md: https://github.com/CZ-NIC/pyoidc/blob/master/CHANGELOG.md
 
 Documentation
 ==============
 
 The `documentation`_ is graciously hosted by `Read the Docs`_. Unfortunately,
 the documentation has been largely left unmaintained and `there are various
 issues`_. However, the maintainers are trying to remedy this lately with some
 new momentum. Please help us by submitting pull requests if you can help
 improve the documentation.
 
 .. _documentation: http://pyoidc.rtfd.io
 .. _Read the Docs: https://readthedocs.org/
-.. _there are various issues: https://github.com/OpenIDC/pyoidc/issues?q=is%3Aopen+is%3Aissue+label%3Adocumentation
+.. _there are various issues: https://github.com/CZ-NIC/pyoidc/issues?q=is%3Aopen+is%3Aissue+label%3Adocumentation
 
 Examples
 ========
 
 Unfortunately, the current examples included in this repository are
 unmaintained and `there are many issues`_. We're currently in the process of
 creating a working canonical example implementation, however, until that time,
 the current examples largely do not work. Please help us by submitting pull
 requests that may bring these examples back into a working condition if you
 get something working locally.
 
-.. _there are many issues: https://github.com/OpenIDC/pyoidc/issues?q=is%3Aopen+is%3Aissue+label%3Aexamples
+.. _there are many issues: https://github.com/CZ-NIC/pyoidc/issues?q=is%3Aopen+is%3Aissue+label%3Aexamples
 
 Acknowledgements
 ================
 
 Cudos to Vladislav Mladenov and Christian Mainka both at
 Horst Görtz Institute for IT-Security, Ruhr-University Bochum, Germany
 for helping me making the implementation more secure.
@@ -102,15 +102,15 @@
 .. _@schlenk: https://github.com/schlenk
 
 Contribute
 ==========
 
 `Fork the repository`_, clone your copy and `install pipenv`_.
 
-.. _Fork the repository: https://github.com/OpenIDC/pyoidc#fork-destination-box
+.. _Fork the repository: https://github.com/CZ-NIC/pyoidc#fork-destination-box
 .. _install pipenv: https://pipenv.readthedocs.io/en/latest/
 
 Then just run:
 
 .. code:: bash
 
     $ make install
@@ -122,16 +122,16 @@
     $ make test
 
 This will not affect your system level Python installation. Please review `our
 issues`_ to see what needs working on. Do not hesitate to ask questions if
 something is unclear. We mark easy issues as `newcomer-friendly`_, so they are
 a good place to start if you want to contribute.
 
-.. _our issues: https://github.com/OpenIDC/pyoidc/issues
-.. _newcomer-friendly: https://github.com/OpenIDC/pyoidc/issues?q=is%3Aopen+is%3Aissue+label%3Anewcomer-friendly
+.. _our issues: https://github.com/CZ-NIC/pyoidc/issues
+.. _newcomer-friendly: https://github.com/CZ-NIC/pyoidc/issues?q=is%3Aopen+is%3Aissue+label%3Anewcomer-friendly
 
 Windows
 -------
 
 If you happen to work in a Windows environment, the above will not work out of the box due to the lack
 of a ``GNU Make`` on Windows. In addition one of the dependencies for ``ldap_authn`` is not available as a prebuilt
 wheel from pypi, so use these slightly modified instructions.
```

### Comparing `oic-1.5.0/src/oic.egg-info/SOURCES.txt` & `oic-1.6.0/src/oic.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -71,8 +71,46 @@
 src/oic/utils/authn/user.py
 src/oic/utils/authn/user_cas.py
 src/oic/utils/rp/__init__.py
 src/oic/utils/rp/oauth2.py
 src/oic/utils/userinfo/__init__.py
 src/oic/utils/userinfo/aa_info.py
 src/oic/utils/userinfo/distaggr.py
-src/oic/utils/userinfo/ldap_info.py
+src/oic/utils/userinfo/ldap_info.py
+tests/test_aes.py
+tests/test_authn_context.py
+tests/test_authn_user.py
+tests/test_claims.py
+tests/test_claims_provider.py
+tests/test_client.py
+tests/test_client_management.py
+tests/test_clientdb.py
+tests/test_grant.py
+tests/test_http_util.py
+tests/test_jwt.py
+tests/test_keyio.py
+tests/test_oauth2.py
+tests/test_oauth2_consumer.py
+tests/test_oauth2_message.py
+tests/test_oauth2_provider.py
+tests/test_oic.py
+tests/test_oic_consumer.py
+tests/test_oic_consumer_logout.py
+tests/test_oic_message.py
+tests/test_oic_provider.py
+tests/test_oic_provider_logout.py
+tests/test_pop.py
+tests/test_popjwt.py
+tests/test_sanitize.py
+tests/test_sdb.py
+tests/test_shelve_wrapper.py
+tests/test_signed_http_request.py
+tests/test_stateless.py
+tests/test_time_util.py
+tests/test_token.py
+tests/test_token_handler.py
+tests/test_user.py
+tests/test_util.py
+tests/test_webfinger.py
+tests/test_x_client.py
+tests/test_x_dynreg.py
+tests/test_x_provider.py
```

