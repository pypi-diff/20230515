# Comparing `tmp/nso-oc-2.49.0.tar.gz` & `tmp/nso-oc-2.50.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nso-oc-2.49.0.tar", last modified: Wed May 10 14:40:05 2023, max compression
+gzip compressed data, was "nso-oc-2.50.0.tar", last modified: Mon May 15 14:50:23 2023, max compression
```

## Comparing `nso-oc-2.49.0.tar` & `nso-oc-2.50.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:40:05.329871 nso-oc-2.49.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-10 14:39:29.000000 nso-oc-2.49.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-10 14:39:29.000000 nso-oc-2.49.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-10 14:40:05.329871 nso-oc-2.49.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-10 14:39:29.000000 nso-oc-2.49.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:40:05.329871 nso-oc-2.49.0/nso_oc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-10 14:40:05.000000 nso-oc-2.49.0/nso_oc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-10 14:40:05.000000 nso-oc-2.49.0/nso_oc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 14:40:05.000000 nso-oc-2.49.0/nso_oc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-10 14:40:05.000000 nso-oc-2.49.0/nso_oc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-10 14:40:05.000000 nso-oc-2.49.0/nso_oc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-10 14:40:05.000000 nso-oc-2.49.0/nso_oc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:40:05.329871 nso-oc-2.49.0/package_nso_to_oc/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-10 14:39:30.000000 nso-oc-2.49.0/package_nso_to_oc/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-10 14:39:30.000000 nso-oc-2.49.0/package_nso_to_oc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-05-10 14:39:30.000000 nso-oc-2.49.0/package_nso_to_oc/common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3569 2023-05-10 14:39:30.000000 nso-oc-2.49.0/package_nso_to_oc/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:40:05.329871 nso-oc-2.49.0/package_nso_to_oc/xe/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-10 14:39:30.000000 nso-oc-2.49.0/package_nso_to_oc/xe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6207 2023-05-10 14:39:30.000000 nso-oc-2.49.0/package_nso_to_oc/xe/common_xe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-10 14:39:30.000000 nso-oc-2.49.0/package_nso_to_oc/xe/main_xe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30058 2023-05-10 14:39:30.000000 nso-oc-2.49.0/package_nso_to_oc/xe/xe_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)    36678 2023-05-10 14:39:30.000000 nso-oc-2.49.0/package_nso_to_oc/xe/xe_bgp.py
--rw-r--r--   0 runner    (1001) docker     (123)    63410 2023-05-10 14:39:30.000000 nso-oc-2.49.0/package_nso_to_oc/xe/xe_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    42084 2023-05-10 14:39:30.000000 nso-oc-2.49.0/package_nso_to_oc/xe/xe_network_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)    39884 2023-05-10 14:39:30.000000 nso-oc-2.49.0/package_nso_to_oc/xe/xe_ospfv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    29881 2023-05-10 14:39:30.000000 nso-oc-2.49.0/package_nso_to_oc/xe/xe_routing_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-05-10 14:39:30.000000 nso-oc-2.49.0/package_nso_to_oc/xe/xe_static_route.py
--rw-r--r--   0 runner    (1001) docker     (123)    32957 2023-05-10 14:39:30.000000 nso-oc-2.49.0/package_nso_to_oc/xe/xe_stp.py
--rw-r--r--   0 runner    (1001) docker     (123)    93881 2023-05-10 14:39:30.000000 nso-oc-2.49.0/package_nso_to_oc/xe/xe_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-10 14:39:30.000000 nso-oc-2.49.0/package_nso_to_oc/xe/xe_vlans.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:40:05.329871 nso-oc-2.49.0/package_nso_to_oc/xr/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-10 14:39:30.000000 nso-oc-2.49.0/package_nso_to_oc/xr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-10 14:39:30.000000 nso-oc-2.49.0/package_nso_to_oc/xr/common_xr.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-10 14:39:30.000000 nso-oc-2.49.0/package_nso_to_oc/xr/main_xr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23665 2023-05-10 14:39:30.000000 nso-oc-2.49.0/package_nso_to_oc/xr/xr_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-05-10 14:39:30.000000 nso-oc-2.49.0/package_nso_to_oc/xr/xr_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-05-10 14:39:30.000000 nso-oc-2.49.0/package_nso_to_oc/xr/xr_system.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-10 14:39:30.000000 nso-oc-2.49.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-10 14:40:05.333871 nso-oc-2.49.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-10 14:39:30.000000 nso-oc-2.49.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:50:23.741520 nso-oc-2.50.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-15 14:49:51.000000 nso-oc-2.50.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-15 14:49:51.000000 nso-oc-2.50.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-15 14:50:23.741520 nso-oc-2.50.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-15 14:49:51.000000 nso-oc-2.50.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:50:23.737519 nso-oc-2.50.0/nso_oc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-15 14:50:23.000000 nso-oc-2.50.0/nso_oc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-15 14:50:23.000000 nso-oc-2.50.0/nso_oc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 14:50:23.000000 nso-oc-2.50.0/nso_oc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-15 14:50:23.000000 nso-oc-2.50.0/nso_oc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 14:50:23.000000 nso-oc-2.50.0/nso_oc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 14:50:23.000000 nso-oc-2.50.0/nso_oc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:50:23.737519 nso-oc-2.50.0/package_nso_to_oc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3569 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:50:23.741520 nso-oc-2.50.0/package_nso_to_oc/xe/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6207 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xe/common_xe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xe/main_xe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30058 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xe/xe_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36678 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xe/xe_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63506 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xe/xe_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42084 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xe/xe_network_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39884 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xe/xe_ospfv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29881 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xe/xe_routing_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xe/xe_static_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32957 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xe/xe_stp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93881 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xe/xe_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xe/xe_vlans.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:50:23.741520 nso-oc-2.50.0/package_nso_to_oc/xr/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xr/common_xr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xr/main_xr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23665 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xr/xr_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xr/xr_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xr/xr_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-15 14:49:51.000000 nso-oc-2.50.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-15 14:50:23.741520 nso-oc-2.50.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-15 14:49:51.000000 nso-oc-2.50.0/setup.py
```

### Comparing `nso-oc-2.49.0/LICENSE` & `nso-oc-2.50.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nso-oc-2.49.0/PKG-INFO` & `nso-oc-2.50.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nso-oc
-Version: 2.49.0
+Version: 2.50.0
 Summary: Cisco NSO OpenConfig Tools
 Home-page: https://github.com/model-driven-devops/nso-oc-services
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NSO NED device configuration to OpenConfig
```

### Comparing `nso-oc-2.49.0/README.md` & `nso-oc-2.50.0/README.md`

 * *Files identical despite different names*

### Comparing `nso-oc-2.49.0/nso_oc.egg-info/PKG-INFO` & `nso-oc-2.50.0/nso_oc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nso-oc
-Version: 2.49.0
+Version: 2.50.0
 Summary: Cisco NSO OpenConfig Tools
 Home-page: https://github.com/model-driven-devops/nso-oc-services
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NSO NED device configuration to OpenConfig
```

### Comparing `nso-oc-2.49.0/nso_oc.egg-info/SOURCES.txt` & `nso-oc-2.50.0/nso_oc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nso-oc-2.49.0/package_nso_to_oc/README.md` & `nso-oc-2.50.0/package_nso_to_oc/README.md`

 * *Files identical despite different names*

### Comparing `nso-oc-2.49.0/package_nso_to_oc/common.py` & `nso-oc-2.50.0/package_nso_to_oc/common.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.49.0/package_nso_to_oc/main.py` & `nso-oc-2.50.0/package_nso_to_oc/main.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.49.0/package_nso_to_oc/xe/common_xe.py` & `nso-oc-2.50.0/package_nso_to_oc/xe/common_xe.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.49.0/package_nso_to_oc/xe/main_xe.py` & `nso-oc-2.50.0/package_nso_to_oc/xe/main_xe.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.49.0/package_nso_to_oc/xe/xe_acls.py` & `nso-oc-2.50.0/package_nso_to_oc/xe/xe_acls.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.49.0/package_nso_to_oc/xe/xe_bgp.py` & `nso-oc-2.50.0/package_nso_to_oc/xe/xe_bgp.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.49.0/package_nso_to_oc/xe/xe_interfaces.py` & `nso-oc-2.50.0/package_nso_to_oc/xe/xe_interfaces.py`

 * *Files 3% similar despite different names*

```diff
@@ -238,47 +238,23 @@
                                 openconfig_interface: dict) -> None:
     """IPv4 interface configurations"""
     oc_ipv4_structure = {"openconfig-if-ip:ipv4": {"openconfig-if-ip:addresses": {"openconfig-if-ip:address": []},
                                                    "openconfig-if-ip:config": {}}}
     if (nso_before_interface.get("ip") and not nso_before_interface.get("ip", {}).get("no-address")) or (
             nso_before_interface.get("vrrp")):
         openconfig_interface.update(oc_ipv4_structure)
-        ipv4_address_structure = {}
-        if (nso_before_interface["ip"].get(
-                "address", {}).get("primary", {}).get("address") and nso_before_interface["ip"].get("address", {}).get(
-            "primary", {}).get("mask")):
-            prefix = ipaddress.IPv4Network(
-                f'{nso_before_interface["ip"].get("address", {}).get("primary", {}).get("address")}/{nso_before_interface["ip"].get("address", {}).get("primary", {}).get("mask")}',
-                strict=False)
-            mask = prefix.prefixlen
-            ip = nso_before_interface["ip"].get("address", {}).get("primary", {}).get("address")
-            del nso_leftover_interface["ip"]["address"]["primary"]
-            ipv4_address_structure.update({"openconfig-if-ip:ip": ip,
-                                           "openconfig-if-ip:config": {"openconfig-if-ip:ip": ip,
-                                                                       "openconfig-if-ip:prefix-length": mask}})
-        if len(ipv4_address_structure) > 0:
-            openconfig_interface["openconfig-if-ip:ipv4"]["openconfig-if-ip:addresses"][
-                "openconfig-if-ip:address"].append(ipv4_address_structure)
-        if type(nso_before_interface["ip"].get(
-                "address", {}).get("dhcp", "")) is dict:
-            openconfig_interface["openconfig-if-ip:ipv4"]["openconfig-if-ip:config"][
-                "openconfig-if-ip:dhcp-client"] = True
-            del \
-                nso_before_interface["ip"]["address"]
-        else:
-            openconfig_interface["openconfig-if-ip:ipv4"]["openconfig-if-ip:config"][
-                "openconfig-if-ip:dhcp-client"] = False
-        # VRRP
-        if nso_before_interface.get("vrrp"):
-            vrrp_dict = xe_configure_vrrp_interfaces(nso_before_interface, nso_leftover_interface)
-            ipv4_address_structure.update(vrrp_dict)
-        # HSRP
-        if nso_before_interface.get("standby", {}).get("standby-list"):
-            hsrp_dict = xe_configure_hsrp_interfaces(nso_before_interface, nso_leftover_interface)
-            ipv4_address_structure.update(hsrp_dict)
+        ip_and_masks = []
+
+        if nso_before_interface["ip"].get("address", {}).get("primary"):
+            ip_and_masks.append(nso_before_interface["ip"]["address"]["primary"])
+        if len(nso_before_interface["ip"].get("address", {}).get("secondary", [])) > 0:
+            ip_and_masks.extend(nso_before_interface["ip"]["address"]["secondary"])
+
+        process_ip_address(ip_and_masks, openconfig_interface, nso_before_interface, nso_leftover_interface, "openconfig-if-ip")
+
         # IP MTU
         if nso_before_interface.get("ip", {}).get("mtu"):
             openconfig_interface["openconfig-if-ip:ipv4"]["openconfig-if-ip:config"][
                 "openconfig-if-ip:mtu"] = nso_before_interface.get("ip", {}).get("mtu")
 
             del nso_leftover_interface["ip"]["mtu"]
         # adjust TCP MSS
@@ -327,56 +303,99 @@
             del nso_leftover_interface["ip"]["nat"]["inside"]
         elif nso_before_interface.get("ip", {}).get("nat", {}).get("outside"):
             openconfig_interface["openconfig-if-ip:ipv4"]["openconfig-if-ip:config"]["openconfig-if-ip-mdd-ext:nat"] = {
                 "openconfig-if-ip-mdd-ext:nat-choice": "outside"}
             del nso_leftover_interface["ip"]["nat"]["outside"]
 
 
+def process_ip_address(ip_and_masks, openconfig_interface, nso_before_interface, nso_leftover_interface, key_prefix):
+    vrrp_leftovers = []
+    hsrp_leftovers = []
+
+    for index, ip_and_mask in enumerate(ip_and_masks):
+        ipv4_address_structure = {}
+
+        if (ip_and_mask.get("address") and ip_and_mask.get("mask")):
+            prefix = ipaddress.IPv4Network(
+                f'{ip_and_mask.get("address")}/{ip_and_mask.get("mask")}',
+                strict=False)
+            mask = prefix.prefixlen
+            ip = ip_and_mask.get("address")
+            ipv4_address_structure.update({f"{key_prefix}:ip": ip,
+                                           f"{key_prefix}:config": {f"{key_prefix}:ip": ip,
+                                                                       f"{key_prefix}:prefix-length": mask}})
+        if len(ipv4_address_structure) > 0:
+            openconfig_interface[f"{key_prefix}:ipv4"][f"{key_prefix}:addresses"][
+                f"{key_prefix}:address"].append(ipv4_address_structure)
+        
+        process_vrrp_hsrp(vrrp_leftovers, hsrp_leftovers, index, nso_before_interface, nso_leftover_interface, ipv4_address_structure)
+    
+    if len(vrrp_leftovers) > 0:
+        nso_leftover_interface["vrrp"] = vrrp_leftovers
+    elif "vrrp" in nso_leftover_interface and len(vrrp_leftovers) == 0:
+        del nso_leftover_interface["vrrp"]
+    if len(hsrp_leftovers) > 0:
+        nso_leftover_interface["standby"]["standby-list"] = hsrp_leftovers
+    elif "standby" in nso_leftover_interface and len(hsrp_leftovers) == 0:
+        del nso_leftover_interface["standby"]
+
+    ip_address = nso_leftover_interface.get("ip", {}).get("address", {})
+
+    if ip_address.get("primary"):
+        del nso_leftover_interface["ip"]["address"]["primary"]
+    if ip_address.get("secondary"):
+        del nso_leftover_interface["ip"]["address"]["secondary"]
+    if type(nso_before_interface["ip"].get("address", {}).get("dhcp", "")) is dict:
+        openconfig_interface[f"{key_prefix}:ipv4"][f"{key_prefix}:config"][
+            f"{key_prefix}:dhcp-client"] = True
+        del \
+            nso_before_interface["ip"]["address"]
+    else:
+        openconfig_interface[f"{key_prefix}:ipv4"][f"{key_prefix}:config"][
+            f"{key_prefix}:dhcp-client"] = False
+
+
+def process_vrrp_hsrp(vrrp_leftovers, hsrp_leftovers, index, nso_before_interface, nso_leftover_interface, ipv4_address_structure):
+    vrrp_before = nso_before_interface.get("vrrp")
+    hsrp_before = nso_before_interface.get("standby", {}).get("standby-list")
+
+    # VRRP
+    if vrrp_before and len(vrrp_before) > index:
+        (vrrp_dict, vrrp_leftover) = xe_configure_vrrp_interfaces(nso_before_interface, nso_leftover_interface, index)
+        ipv4_address_structure.update(vrrp_dict)
+
+        if vrrp_leftover:
+            vrrp_leftovers.append(vrrp_leftover)
+    # HSRP
+    if hsrp_before and len(hsrp_before) > index:
+        (hsrp_dict, hsrp_leftover) = xe_configure_hsrp_interfaces(nso_before_interface, nso_leftover_interface, index)
+        ipv4_address_structure.update(hsrp_dict)
+
+        if hsrp_leftover:
+            hsrp_leftovers.append(hsrp_leftover)
+
+
 def xe_configure_tunnel_ipv4_interface(nso_before_interface: dict, nso_leftover_interface: dict,
                                        openconfig_interface: dict) -> None:
     """Tunnel IPv4 interface configurations"""
     oc_ipv4_structure = {
         "openconfig-if-tunnel:ipv4": {"openconfig-if-tunnel:addresses": {"openconfig-if-tunnel:address": []},
                                       "openconfig-if-tunnel:config": {}}}
     if (nso_before_interface.get("ip") and not nso_before_interface.get("ip", {}).get("no-address")) or (
             nso_before_interface.get("vrrp")):
         openconfig_interface.update(oc_ipv4_structure)
-        ipv4_address_structure = {}
-        if (nso_before_interface["ip"].get(
-                "address", {}).get("primary", {}).get("address") and nso_before_interface["ip"].get("address", {}).get(
-            "primary", {}).get("mask")):
-            prefix = ipaddress.IPv4Network(
-                f'{nso_before_interface["ip"].get("address", {}).get("primary", {}).get("address")}/{nso_before_interface["ip"].get("address", {}).get("primary", {}).get("mask")}',
-                strict=False)
-            mask = prefix.prefixlen
-            ip = nso_before_interface["ip"].get("address", {}).get("primary", {}).get("address")
-            del nso_leftover_interface["ip"]["address"]["primary"]
-            ipv4_address_structure.update({"openconfig-if-tunnel:ip": ip,
-                                           "openconfig-if-tunnel:config": {"openconfig-if-tunnel:ip": ip,
-                                                                           "openconfig-if-tunnel:prefix-length": mask}})
-        if len(ipv4_address_structure) > 0:
-            openconfig_interface["openconfig-if-tunnel:ipv4"]["openconfig-if-tunnel:addresses"][
-                "openconfig-if-tunnel:address"].append(ipv4_address_structure)
-        if type(nso_before_interface["ip"].get(
-                "address", {}).get("dhcp", "")) is dict:
-            openconfig_interface["openconfig-if-tunnel:ipv4"]["openconfig-if-tunnel:config"][
-                "openconfig-if-tunnel:dhcp-client"] = True
-            del \
-                nso_before_interface["ip"]["address"]
-        else:
-            openconfig_interface["openconfig-if-tunnel:ipv4"]["openconfig-if-tunnel:config"][
-                "openconfig-if-tunnel:dhcp-client"] = False
-        # VRRP
-        if nso_before_interface.get("vrrp"):
-            vrrp_dict = xe_configure_vrrp_interfaces(nso_before_interface, nso_leftover_interface)
-            ipv4_address_structure.update(vrrp_dict)
-        # HSRP
-        if nso_before_interface.get("standby", {}).get("standby-list"):
-            hsrp_dict = xe_configure_hsrp_interfaces(nso_before_interface, nso_leftover_interface)
-            ipv4_address_structure.update(hsrp_dict)
+        ip_and_masks = []
+
+        if nso_before_interface["ip"].get("address", {}).get("primary"):
+            ip_and_masks.append(nso_before_interface["ip"]["address"]["primary"])
+        if len(nso_before_interface["ip"].get("address", {}).get("secondary", [])) > 0:
+            ip_and_masks.extend(nso_before_interface["ip"]["address"]["secondary"])
+
+        process_ip_address(ip_and_masks, openconfig_interface, nso_before_interface, nso_leftover_interface, "openconfig-if-tunnel")
+
         # IP MTU
         if nso_before_interface.get("ip", {}).get("mtu"):
             openconfig_interface["openconfig-if-tunnel:ipv4"]["openconfig-if-tunnel:config"][
                 "openconfig-if-tunnel:mtu"] = nso_before_interface.get("ip", {}).get("mtu")
 
             del nso_leftover_interface["ip"]["mtu"]
         # adjust TCP MSS
@@ -425,15 +444,15 @@
                 "openconfig-if-ip-mdd-ext:nat-choice": "inside"}
             del nso_leftover_interface["ip"]["nat"]["inside"]
         elif nso_before_interface.get("ip", {}).get("nat", {}).get("outside"):
             openconfig_interface["openconfig-if-tunnel:ipv4"]["openconfig-if-tunnel:config"][
                 "openconfig-if-ip-mdd-ext:nat"] = {
                 "openconfig-if-ip-mdd-ext:nat-choice": "outside"}
             del nso_leftover_interface["ip"]["nat"]["outside"]
-
+        
 
 def configure_software_loopback(config_before: dict, config_leftover: dict, interface_data: dict) -> None:
     """Configure Loopbacks"""
     for interface_directory in interface_data.values():
         path_oc_sub_if = ["openconfig-interfaces:interfaces", "openconfig-interfaces:interface",
                           interface_directory["oc_interface_index"], "openconfig-interfaces:subinterfaces",
                           "openconfig-interfaces:subinterface", interface_directory["oc_sub_interface_place_counter"]]
@@ -729,106 +748,128 @@
         openconfig_interface["openconfig-if-ethernet:ethernet"]["openconfig-if-ethernet-mdd-ext:storm-control"][
             "openconfig-if-ethernet-mdd-ext:unicast"]["openconfig-if-ethernet-mdd-ext:level"][
             "openconfig-if-ethernet-mdd-ext:config"]["openconfig-if-ethernet-mdd-ext:pps"] = nso_before_interface.get("storm-control", {}).get("unicast", {}).get("level-bps-pps", {}).get("level", {}).get("pps")
         del config_leftover["tailf-ned-cisco-ios:interface"][v["nso_interface_type"]][v["nso_interface_index"]][
                 "storm-control"]["unicast"]["level-bps-pps"]["level"]["pps"]
 
 
-def xe_configure_vrrp_interfaces(nso_before_interface: dict, nso_leftover_interface: dict) -> dict:
+def xe_configure_vrrp_interfaces(nso_before_interface: dict, nso_leftover_interface: dict, index: int) -> tuple:
     """Configure VRRP"""
-    updated_vrrp = []
-
     service_vrrp = {"openconfig-if-ip:vrrp": {"openconfig-if-ip:vrrp-group": []}}
-    for number, group in enumerate(nso_before_interface.get("vrrp")):
-        if group.get("id"):
-            # Group
-            service_vrrp_group = {"openconfig-if-ip:virtual-router-id": group.get("id"),
-                                  "openconfig-if-ip:config": {"openconfig-if-ip:virtual-router-id": group.get("id")}}
-            del nso_leftover_interface["vrrp"][number]["id"]
-            # Preempt delay
-            if group.get("preempt", {}).get("delay", {}).get("minimum"):
-                service_vrrp_group["openconfig-if-ip:config"]["openconfig-if-ip:preempt-delay"] = group.get("preempt",
-                                                                                                            {}).get(
-                    "delay", {}).get("minimum")
-                del nso_leftover_interface["vrrp"][number]["preempt"]["delay"]
-            # Preempt
-            if group.get("preempt"):
-                service_vrrp_group["openconfig-if-ip:config"]["openconfig-if-ip:preempt"] = True
-                del nso_leftover_interface["vrrp"][number]["preempt"]
-            # Priority
-            if group.get("priority"):
-                service_vrrp_group["openconfig-if-ip:config"]["openconfig-if-ip:priority"] = group.get("priority")
-                del nso_leftover_interface["vrrp"][number]["priority"]
-            # VRRP Address
-            if group.get("ip", {}).get("address"):
-                service_vrrp_group["openconfig-if-ip:config"]["openconfig-if-ip:virtual-address"] = []
-                service_vrrp_group["openconfig-if-ip:config"]["openconfig-if-ip:virtual-address"].append(
-                    group.get("ip", {}).get("address"))
-                del nso_leftover_interface["vrrp"][number]["ip"]
-            # Timers advertise
-            if group.get("timers", {}).get("advertise", {}).get("seconds"):
-                service_vrrp_group["openconfig-if-ip:config"]["openconfig-if-ip:advertisement-interval"] = int(
-                    group.get("timers", {}).get("advertise").get("seconds")) * 100
-                del nso_leftover_interface["vrrp"][number]["timers"]["advertise"]
-            service_vrrp["openconfig-if-ip:vrrp"]["openconfig-if-ip:vrrp-group"].append(service_vrrp_group)
-            # Clean up
-            if nso_leftover_interface["vrrp"][number] and len(nso_leftover_interface["vrrp"][number]) > 0:
-                updated_vrrp.append(nso_leftover_interface["vrrp"][number])
-    nso_leftover_interface["vrrp"] = updated_vrrp
+    vrrp_leftover = None
+    group = nso_before_interface["vrrp"][index]
+    current_vrrp = nso_leftover_interface["vrrp"][index]
+
+    if group.get("id"):
+        # Group
+        service_vrrp_group = {"openconfig-if-ip:virtual-router-id": group.get("id"),
+                                "openconfig-if-ip:config": {"openconfig-if-ip:virtual-router-id": group.get("id")}}
+        del current_vrrp["id"]
+        # Preempt delay
+        if group.get("preempt", {}).get("delay", {}).get("minimum"):
+            service_vrrp_group["openconfig-if-ip:config"]["openconfig-if-ip:preempt-delay"] = group.get("preempt",
+                                                                                                        {}).get(
+                "delay", {}).get("minimum")
+            del current_vrrp["preempt"]["delay"]
+        # Preempt
+        if group.get("preempt"):
+            service_vrrp_group["openconfig-if-ip:config"]["openconfig-if-ip:preempt"] = True
+            del current_vrrp["preempt"]
+        # Priority
+        if group.get("priority"):
+            service_vrrp_group["openconfig-if-ip:config"]["openconfig-if-ip:priority"] = group.get("priority")
+            del current_vrrp["priority"]
+        # VRRP Address
+        if group.get("ip", {}).get("address"):
+            service_vrrp_group["openconfig-if-ip:config"]["openconfig-if-ip:virtual-address"] = []
+            service_vrrp_group["openconfig-if-ip:config"]["openconfig-if-ip:virtual-address"].append(
+                group.get("ip", {}).get("address"))
+        for secondary_address in group.get("ip", {}).get("secondary-address", []):
+            service_vrrp_group["openconfig-if-ip:config"]["openconfig-if-ip:virtual-address"].append(
+                secondary_address["address"])
+        if current_vrrp.get("ip"):
+            del current_vrrp["ip"]
+        # Timers advertise
+        if group.get("timers", {}).get("advertise", {}).get("seconds"):
+            service_vrrp_group["openconfig-if-ip:config"]["openconfig-if-ip:advertisement-interval"] = int(
+                group.get("timers", {}).get("advertise").get("seconds")) * 100
+            del current_vrrp["timers"]["advertise"]
+
+            if len(current_vrrp["timers"]) == 0:
+                del current_vrrp["timers"]
+        service_vrrp["openconfig-if-ip:vrrp"]["openconfig-if-ip:vrrp-group"].append(service_vrrp_group)
+        # Keep object if it contains more properties
+        if current_vrrp and len(current_vrrp) > 0:
+            vrrp_leftover = current_vrrp
     
-    return service_vrrp
+    return (service_vrrp, vrrp_leftover)
 
 
-def xe_configure_hsrp_interfaces(nso_before_interface: dict, nso_leftover_interface: dict) -> dict:
+def xe_configure_hsrp_interfaces(nso_before_interface: dict, nso_leftover_interface: dict, index: int) -> tuple:
     """Configure HSRP"""
     service_hsrp = {"openconfig-if-ip-mdd-ext:hsrp": {"openconfig-if-ip-mdd-ext:hsrp-group": []}}
-    for number, group in enumerate(nso_before_interface.get("standby", {}).get("standby-list")):
-        if group.get("group-number"):
-            # Group
-            service_hsrp_group = {"openconfig-if-ip-mdd-ext:group-number": group.get("group-number"),
-                                  "openconfig-if-ip-mdd-ext:config": {
-                                      "openconfig-if-ip-mdd-ext:group-number": group.get("group-number")}}
-            del nso_leftover_interface["standby"]["standby-list"][number]["group-number"]
-            # Preempt delay
-            if group.get("preempt", {}).get("delay", {}).get("minimum"):
-                service_hsrp_group["openconfig-if-ip-mdd-ext:config"][
-                    "openconfig-if-ip-mdd-ext:preempt-delay"] = group.get("preempt",
-                                                                          {}).get(
-                    "delay", {}).get("minimum")
-                del nso_leftover_interface["standby"]["standby-list"][number]["preempt"]["delay"]
-            # Preempt
-            if group.get("preempt"):
-                service_hsrp_group["openconfig-if-ip-mdd-ext:config"]["openconfig-if-ip-mdd-ext:preempt"] = True
-                del nso_leftover_interface["standby"]["standby-list"][number]["preempt"]
-            # Priority
-            if group.get("priority"):
-                service_hsrp_group["openconfig-if-ip-mdd-ext:config"]["openconfig-if-ip-mdd-ext:priority"] = group.get(
-                    "priority")
-                del nso_leftover_interface["standby"]["standby-list"][number]["priority"]
-            # VRRP Address
-            if group.get("ip", {}).get("address"):
-                service_hsrp_group["openconfig-if-ip-mdd-ext:config"]["openconfig-if-ip-mdd-ext:virtual-address"] = []
-                service_hsrp_group["openconfig-if-ip-mdd-ext:config"][
-                    "openconfig-if-ip-mdd-ext:virtual-address"].append(
-                    group.get("ip", {}).get("address"))
-                del nso_leftover_interface["standby"]["standby-list"][number]["ip"]
-            # Timers
-            if group.get("timers", {}).get("hello-interval", {}).get("seconds") and group.get("timers", {}).get(
-                    "hold-time", {}).get("seconds"):
-                service_hsrp_group["openconfig-if-ip-mdd-ext:config"].update({"openconfig-if-ip-mdd-ext:timers": {
-                    "openconfig-if-ip-mdd-ext:hello-interval": int(
-                        group.get("timers", {}).get("hello-interval").get("seconds")),
-                    "openconfig-if-ip-mdd-ext:holdtime": int(group.get("timers", {}).get("hold-time").get("seconds"))
-                }})
-                del nso_leftover_interface["standby"]["standby-list"][number]["timers"]["hello-interval"]
-                del nso_leftover_interface["standby"]["standby-list"][number]["timers"]["hold-time"]
-
-            service_hsrp["openconfig-if-ip-mdd-ext:hsrp"]["openconfig-if-ip-mdd-ext:hsrp-group"].append(
-                service_hsrp_group)
-    return service_hsrp
+    hsrp_leftover = None
+    group = nso_before_interface["standby"]["standby-list"][index]
+    current_standby = nso_leftover_interface["standby"]["standby-list"][index]
+
+    if group.get("group-number"):
+        # Group
+        service_hsrp_group = {"openconfig-if-ip-mdd-ext:group-number": group.get("group-number"),
+                                "openconfig-if-ip-mdd-ext:config": {
+                                    "openconfig-if-ip-mdd-ext:group-number": group.get("group-number")}}
+        del current_standby["group-number"]
+        # Preempt delay
+        if group.get("preempt", {}).get("delay", {}).get("minimum"):
+            service_hsrp_group["openconfig-if-ip-mdd-ext:config"][
+                "openconfig-if-ip-mdd-ext:preempt-delay"] = group.get("preempt",
+                                                                        {}).get(
+                "delay", {}).get("minimum")
+            del current_standby["preempt"]["delay"]
+        # Preempt
+        if group.get("preempt"):
+            service_hsrp_group["openconfig-if-ip-mdd-ext:config"]["openconfig-if-ip-mdd-ext:preempt"] = True
+            del current_standby["preempt"]
+        # Priority
+        if group.get("priority"):
+            service_hsrp_group["openconfig-if-ip-mdd-ext:config"]["openconfig-if-ip-mdd-ext:priority"] = group.get(
+                "priority")
+            del current_standby["priority"]
+        # VRRP Address
+        if group.get("ip", {}).get("address"):
+            service_hsrp_group["openconfig-if-ip-mdd-ext:config"]["openconfig-if-ip-mdd-ext:virtual-address"] = []
+            service_hsrp_group["openconfig-if-ip-mdd-ext:config"][
+                "openconfig-if-ip-mdd-ext:virtual-address"].append(
+                group.get("ip", {}).get("address"))
+        for secondary_address in group.get("ip", {}).get("secondary", []):
+            service_hsrp_group["openconfig-if-ip-mdd-ext:config"][
+                "openconfig-if-ip-mdd-ext:virtual-address"].append(secondary_address["address"])
+        if current_standby.get("ip"):
+            del current_standby["ip"]
+        # Timers
+        if group.get("timers", {}).get("hello-interval", {}).get("seconds") and group.get("timers", {}).get(
+                "hold-time", {}).get("seconds"):
+            service_hsrp_group["openconfig-if-ip-mdd-ext:config"].update({"openconfig-if-ip-mdd-ext:timers": {
+                "openconfig-if-ip-mdd-ext:hello-interval": int(
+                    group.get("timers", {}).get("hello-interval").get("seconds")),
+                "openconfig-if-ip-mdd-ext:holdtime": int(group.get("timers", {}).get("hold-time").get("seconds"))
+            }})
+            del current_standby["timers"]["hello-interval"]
+            del current_standby["timers"]["hold-time"]
+
+            if len(current_standby["timers"]) == 0:
+                del current_standby["timers"]
+
+        service_hsrp["openconfig-if-ip-mdd-ext:hsrp"]["openconfig-if-ip-mdd-ext:hsrp-group"].append(
+            service_hsrp_group)
+        
+        # Keep object if it contains more properties
+        if current_standby and len(current_standby) > 0:
+            hsrp_leftover = current_standby
+
+    return (service_hsrp, hsrp_leftover)
 
 
 def configure_csmacd(config_before: dict, config_leftover: dict, interface_data: dict) -> None:
     """
     Iterate through interface_data
     Call up the config_before["tailf-ned-cisco-ios:interface"][v["nso_interface_type"]][v["nso_interface_index"]]
     Add need OC config to openconfig_interfaces["openconfig-interfaces:interfaces"]["openconfig-interfaces:interface"][v["oc_interface_index"]]
```

### Comparing `nso-oc-2.49.0/package_nso_to_oc/xe/xe_network_instances.py` & `nso-oc-2.50.0/package_nso_to_oc/xe/xe_network_instances.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.49.0/package_nso_to_oc/xe/xe_ospfv2.py` & `nso-oc-2.50.0/package_nso_to_oc/xe/xe_ospfv2.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.49.0/package_nso_to_oc/xe/xe_routing_policy.py` & `nso-oc-2.50.0/package_nso_to_oc/xe/xe_routing_policy.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.49.0/package_nso_to_oc/xe/xe_static_route.py` & `nso-oc-2.50.0/package_nso_to_oc/xe/xe_static_route.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.49.0/package_nso_to_oc/xe/xe_stp.py` & `nso-oc-2.50.0/package_nso_to_oc/xe/xe_stp.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.49.0/package_nso_to_oc/xe/xe_system.py` & `nso-oc-2.50.0/package_nso_to_oc/xe/xe_system.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.49.0/package_nso_to_oc/xe/xe_vlans.py` & `nso-oc-2.50.0/package_nso_to_oc/xe/xe_vlans.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.49.0/package_nso_to_oc/xr/common_xr.py` & `nso-oc-2.50.0/package_nso_to_oc/xr/common_xr.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.49.0/package_nso_to_oc/xr/main_xr.py` & `nso-oc-2.50.0/package_nso_to_oc/xr/main_xr.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.49.0/package_nso_to_oc/xr/xr_acls.py` & `nso-oc-2.50.0/package_nso_to_oc/xr/xr_acls.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.49.0/package_nso_to_oc/xr/xr_interfaces.py` & `nso-oc-2.50.0/package_nso_to_oc/xr/xr_interfaces.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.49.0/package_nso_to_oc/xr/xr_system.py` & `nso-oc-2.50.0/package_nso_to_oc/xr/xr_system.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.49.0/setup.py` & `nso-oc-2.50.0/setup.py`

 * *Files identical despite different names*

