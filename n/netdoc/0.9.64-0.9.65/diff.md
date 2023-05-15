# Comparing `tmp/netdoc-0.9.64.tar.gz` & `tmp/netdoc-0.9.65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netdoc-0.9.64.tar", last modified: Wed May 10 09:45:15 2023, max compression
+gzip compressed data, was "netdoc-0.9.65.tar", last modified: Mon May 15 13:20:12 2023, max compression
```

## Comparing `netdoc-0.9.64.tar` & `netdoc-0.9.65.tar`

### file list

```diff
@@ -1,189 +1,189 @@
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 09:45:15.087573 netdoc-0.9.64/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.64/LICENSE
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      241 2023-04-05 08:40:22.000000 netdoc-0.9.64/MANIFEST.in
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      469 2023-05-10 09:45:15.087573 netdoc-0.9.64/PKG-INFO
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     9982 2023-05-05 13:07:59.000000 netdoc-0.9.64/README.md
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 09:45:14.795567 netdoc-0.9.64/netdoc/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2218 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/__init__.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 09:45:14.815568 netdoc-0.9.64/netdoc/api/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/api/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2812 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/api/serializers.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      597 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/api/urls.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1207 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/api/views.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 09:45:14.819568 netdoc-0.9.64/netdoc/discoverers/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/discoverers/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6978 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/discoverers/netmiko_cisco_ios.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5160 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/discoverers/netmiko_cisco_nxos.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6520 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/discoverers/netmiko_cisco_xr.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6406 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/discoverers/netmiko_hp_comware.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4511 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/discoverers/netmiko_linux.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3613 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/filtersets.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6587 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/forms.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 09:45:14.843568 netdoc-0.9.64/netdoc/ingestors/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1206 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_ios_hostname.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3710 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_ios_show_cdp_neighbors_detail.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2014 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_ios_show_etherchannel_summary.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2457 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_ios_show_interfaces.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1705 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_ios_show_interfaces_switchport.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      912 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_ios_show_inventory.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1544 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_ios_show_ip_arp.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1951 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_ios_show_ip_interface.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2678 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_ios_show_ip_route.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3959 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_ios_show_lldp_neighbors_detail.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1660 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_ios_show_mac_address_table.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      886 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_ios_show_vlan.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1010 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_ios_show_vrf.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1239 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_nxos_hostname.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3677 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_nxos_show_cdp_neighbors_detail.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2349 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_nxos_show_interface.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1986 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_nxos_show_interface_switchport.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      914 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_nxos_show_inventory.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1539 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_nxos_show_ip_arp.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2000 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_nxos_show_ip_interface.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2851 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_nxos_show_ip_route_vrf_all.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3936 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_nxos_show_lldp_neighbors_detail.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1509 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_nxos_show_mac_address_table.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2020 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_nxos_show_port_channel_summary.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      888 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_nxos_show_vlan.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      909 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_nxos_show_vrf.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      915 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_xr_admin_show_inventory.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1205 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_xr_hostname.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1529 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_xr_show_arp.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3673 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_xr_show_cdp_neighbors_detail.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2347 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_xr_show_interfaces.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1802 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_xr_show_ipv4_interface.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2921 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_xr_show_lldp_neighbors.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2785 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_xr_show_route.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      980 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_xr_show_vrf_all_detail.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1562 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_hp_comware_display_arp.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      894 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_hp_comware_display_device_manuinfo.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2980 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_hp_comware_display_interface.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1385 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_hp_comware_display_ip_interface.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2702 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_hp_comware_display_ip_routing_table.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1038 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1687 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance_instance_name.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2035 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_hp_comware_display_link_aggregation_verbose.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2962 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_list.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3964 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_verbose.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1514 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_hp_comware_display_mac_address.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      895 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_hp_comware_display_vlan_all.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      899 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_hp_comware_display_vlan_brief.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1203 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_hp_comware_hostname.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1539 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_linux_arp__an.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1008 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_linux_hostname.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1412 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_linux_ip_address_show.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1933 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_linux_ip_link_show.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2526 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_linux_ip_route_show.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      711 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/ingestors/netmiko_linux_ip_vrf_show.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 09:45:14.843568 netdoc-0.9.64/netdoc/migrations/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    13632 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/migrations/0001_initial.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1800 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/migrations/0002_alter_arptableentry_custom_field_data_and_more.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3399 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/migrations/0003_alter_arptableentry_options_alter_credential_options_and_more.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3022 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/migrations/0004_alter_macaddresstableentry_options_and_more.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      577 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/migrations/0005_diagram_include_global_vrf_alter_diagram_details.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      453 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/migrations/0006_alter_routetableentry_metric.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      419 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/migrations/0007_discoverylog_supported.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/migrations/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    15079 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/models.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2805 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/navigation.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2988 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/nornir_inventory.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 09:45:14.843568 netdoc-0.9.64/netdoc/reports/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5880 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/reports/NetDoc.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 09:45:14.855569 netdoc-0.9.64/netdoc/schemas/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/schemas/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1937 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/schemas/arptableentry.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4719 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/schemas/cable.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1739 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/schemas/credential.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6493 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/schemas/device.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1508 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/schemas/devicerole.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1714 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/schemas/devicetype.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3905 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/schemas/discoverable.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3176 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/schemas/discoverylog.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     9789 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/schemas/interface.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1362 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/schemas/ipaddress.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1978 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/schemas/macaddresstableentry.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1453 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/schemas/manufacturer.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2015 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/schemas/prefix.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3018 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/schemas/routetableentry.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      884 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/schemas/site.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1623 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/schemas/vlan.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2476 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/schemas/vrf.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 09:45:14.855569 netdoc-0.9.64/netdoc/scripts/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    13085 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/scripts/NetDoc.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 09:45:14.767567 netdoc-0.9.64/netdoc/static/
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 09:45:14.767567 netdoc-0.9.64/netdoc/static/netdoc/
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 09:45:14.867569 netdoc-0.9.64/netdoc/static/netdoc/css/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.64/netdoc/static/netdoc/css/LICENSE
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      494 2023-04-05 08:40:22.000000 netdoc-0.9.64/netdoc/static/netdoc/css/README.md
--rw-rw-r--   0 andrea    (1000) andrea    (1000)   220164 2023-04-05 08:40:22.000000 netdoc-0.9.64/netdoc/static/netdoc/css/vis-network.min.css
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 09:45:14.931570 netdoc-0.9.64/netdoc/static/netdoc/img/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.64/netdoc/static/netdoc/img/LICENSE
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      305 2023-04-05 08:40:22.000000 netdoc-0.9.64/netdoc/static/netdoc/img/README.md
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     7415 2023-04-05 08:40:22.000000 netdoc-0.9.64/netdoc/static/netdoc/img/access-switch.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5648 2023-04-05 08:40:22.000000 netdoc-0.9.64/netdoc/static/netdoc/img/backup.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    28633 2023-04-05 08:40:22.000000 netdoc-0.9.64/netdoc/static/netdoc/img/circuit.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     8387 2023-04-05 08:40:22.000000 netdoc-0.9.64/netdoc/static/netdoc/img/core-switch.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     9522 2023-04-05 08:40:22.000000 netdoc-0.9.64/netdoc/static/netdoc/img/distribution-switch.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    15596 2023-04-05 08:40:22.000000 netdoc-0.9.64/netdoc/static/netdoc/img/firewall.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1614 2023-04-05 08:40:22.000000 netdoc-0.9.64/netdoc/static/netdoc/img/internal-switch.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5537 2023-04-05 08:40:22.000000 netdoc-0.9.64/netdoc/static/netdoc/img/isp-cpe-material.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5079 2023-04-05 08:40:22.000000 netdoc-0.9.64/netdoc/static/netdoc/img/non-racked-devices.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    15857 2023-04-05 08:40:22.000000 netdoc-0.9.64/netdoc/static/netdoc/img/power-feed.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    18685 2023-04-05 08:40:22.000000 netdoc-0.9.64/netdoc/static/netdoc/img/power-panel.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4710 2023-04-05 08:40:22.000000 netdoc-0.9.64/netdoc/static/netdoc/img/power-units.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    34335 2023-04-05 08:40:22.000000 netdoc-0.9.64/netdoc/static/netdoc/img/provider-networks.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    13504 2023-04-05 08:40:22.000000 netdoc-0.9.64/netdoc/static/netdoc/img/router.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4484 2023-04-05 08:40:22.000000 netdoc-0.9.64/netdoc/static/netdoc/img/server.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5648 2023-04-05 08:40:22.000000 netdoc-0.9.64/netdoc/static/netdoc/img/storage.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     8308 2023-04-05 08:40:22.000000 netdoc-0.9.64/netdoc/static/netdoc/img/unknown.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     7415 2023-04-05 08:40:22.000000 netdoc-0.9.64/netdoc/static/netdoc/img/wan-network.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6975 2023-04-05 08:40:22.000000 netdoc-0.9.64/netdoc/static/netdoc/img/wireless-ap.png
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 09:45:14.967571 netdoc-0.9.64/netdoc/static/netdoc/js/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.64/netdoc/static/netdoc/js/LICENSE
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      494 2023-04-05 08:40:22.000000 netdoc-0.9.64/netdoc/static/netdoc/js/README.md
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4198 2023-04-05 14:32:29.000000 netdoc-0.9.64/netdoc/static/netdoc/js/diagram.js
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1739 2023-04-05 08:40:22.000000 netdoc-0.9.64/netdoc/static/netdoc/js/netdoc.js
--rw-rw-r--   0 andrea    (1000) andrea    (1000)   702066 2023-04-05 08:40:22.000000 netdoc-0.9.64/netdoc/static/netdoc/js/vis-network.min.js
--rw-rw-r--   0 andrea    (1000) andrea    (1000)  1930592 2023-04-05 08:40:22.000000 netdoc-0.9.64/netdoc/static/netdoc/js/vis-network.min.js.map
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     8272 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/tables.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3912 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/tasks.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 09:45:14.767567 netdoc-0.9.64/netdoc/templates/
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 09:45:15.059573 netdoc-0.9.64/netdoc/templates/netdoc/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3038 2023-04-10 16:21:20.000000 netdoc-0.9.64/netdoc/templates/netdoc/arptableentry.html
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 09:45:15.071573 netdoc-0.9.64/netdoc/templates/netdoc/buttons/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      451 2023-04-10 16:17:25.000000 netdoc-0.9.64/netdoc/templates/netdoc/buttons/discover.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      337 2023-04-10 16:17:25.000000 netdoc-0.9.64/netdoc/templates/netdoc/buttons/export.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1669 2023-04-10 16:21:17.000000 netdoc-0.9.64/netdoc/templates/netdoc/credential.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1439 2023-04-10 16:29:06.000000 netdoc-0.9.64/netdoc/templates/netdoc/diagram.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2654 2023-04-10 16:23:32.000000 netdoc-0.9.64/netdoc/templates/netdoc/discoverable.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1217 2023-04-10 16:26:08.000000 netdoc-0.9.64/netdoc/templates/netdoc/discoverable_bulk_discover.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      638 2023-04-10 16:26:30.000000 netdoc-0.9.64/netdoc/templates/netdoc/discoverable_discover.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1006 2023-04-10 16:23:40.000000 netdoc-0.9.64/netdoc/templates/netdoc/discoverable_list.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5123 2023-04-10 16:23:17.000000 netdoc-0.9.64/netdoc/templates/netdoc/discoverylog.html
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 09:45:15.079573 netdoc-0.9.64/netdoc/templates/netdoc/htmx/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1005 2023-04-10 16:17:25.000000 netdoc-0.9.64/netdoc/templates/netdoc/htmx/discover_form.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1025 2023-04-10 16:17:25.000000 netdoc-0.9.64/netdoc/templates/netdoc/htmx/logexport_form.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3046 2023-04-10 16:20:47.000000 netdoc-0.9.64/netdoc/templates/netdoc/macaddresstableentry.html
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 09:45:15.083573 netdoc-0.9.64/netdoc/templatetags/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/templatetags/__init__.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 09:45:15.087573 netdoc-0.9.64/netdoc/templatetags/__pycache__/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      148 2023-05-05 14:53:12.000000 netdoc-0.9.64/netdoc/templatetags/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1048 2023-05-05 14:53:12.000000 netdoc-0.9.64/netdoc/templatetags/__pycache__/netdoc_buttons.cpython-310.pyc
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      890 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/templatetags/netdoc_buttons.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 09:45:15.087573 netdoc-0.9.64/netdoc/tests/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/tests/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    17018 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/tests/test.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    11615 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/topologies.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5128 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/urls.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    28388 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/utils.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    18479 2023-05-10 09:45:12.000000 netdoc-0.9.64/netdoc/views.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 09:45:14.807568 netdoc-0.9.64/netdoc.egg-info/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      469 2023-05-10 09:45:14.000000 netdoc-0.9.64/netdoc.egg-info/PKG-INFO
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6963 2023-05-10 09:45:14.000000 netdoc-0.9.64/netdoc.egg-info/SOURCES.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2023-05-10 09:45:14.000000 netdoc-0.9.64/netdoc.egg-info/dependency_links.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2023-04-05 14:49:45.000000 netdoc-0.9.64/netdoc.egg-info/not-zip-safe
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      132 2023-05-10 09:45:14.000000 netdoc-0.9.64/netdoc.egg-info/requires.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        7 2023-05-10 09:45:14.000000 netdoc-0.9.64/netdoc.egg-info/top_level.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      103 2023-05-10 09:45:15.087573 netdoc-0.9.64/setup.cfg
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1272 2023-05-10 09:45:12.000000 netdoc-0.9.64/setup.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-15 13:20:12.586912 netdoc-0.9.65/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.65/LICENSE
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      241 2023-04-05 08:40:22.000000 netdoc-0.9.65/MANIFEST.in
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      469 2023-05-15 13:20:12.586912 netdoc-0.9.65/PKG-INFO
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     9982 2023-05-05 13:07:59.000000 netdoc-0.9.65/README.md
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-15 13:20:12.466909 netdoc-0.9.65/netdoc/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2218 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/__init__.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-15 13:20:12.482910 netdoc-0.9.65/netdoc/api/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/api/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2812 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/api/serializers.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      597 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/api/urls.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1207 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/api/views.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-15 13:20:12.486909 netdoc-0.9.65/netdoc/discoverers/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/discoverers/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6978 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/discoverers/netmiko_cisco_ios.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5160 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/discoverers/netmiko_cisco_nxos.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6520 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/discoverers/netmiko_cisco_xr.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6406 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/discoverers/netmiko_hp_comware.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4511 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/discoverers/netmiko_linux.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3613 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/filtersets.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6587 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/forms.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-15 13:20:12.506910 netdoc-0.9.65/netdoc/ingestors/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1206 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_ios_hostname.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3710 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_ios_show_cdp_neighbors_detail.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2014 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_ios_show_etherchannel_summary.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2457 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_ios_show_interfaces.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1705 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_ios_show_interfaces_switchport.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      912 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_ios_show_inventory.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1544 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_ios_show_ip_arp.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1951 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_ios_show_ip_interface.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2678 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_ios_show_ip_route.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3959 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_ios_show_lldp_neighbors_detail.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1660 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_ios_show_mac_address_table.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      886 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_ios_show_vlan.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1010 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_ios_show_vrf.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1239 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_nxos_hostname.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3677 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_nxos_show_cdp_neighbors_detail.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2349 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_nxos_show_interface.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1986 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_nxos_show_interface_switchport.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      914 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_nxos_show_inventory.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1539 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_nxos_show_ip_arp.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2000 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_nxos_show_ip_interface.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2851 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_nxos_show_ip_route_vrf_all.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3936 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_nxos_show_lldp_neighbors_detail.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1509 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_nxos_show_mac_address_table.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2020 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_nxos_show_port_channel_summary.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      888 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_nxos_show_vlan.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      909 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_nxos_show_vrf.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      915 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_xr_admin_show_inventory.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1205 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_xr_hostname.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1529 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_xr_show_arp.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3673 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_xr_show_cdp_neighbors_detail.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2347 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_xr_show_interfaces.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1802 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_xr_show_ipv4_interface.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2921 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_xr_show_lldp_neighbors.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2785 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_xr_show_route.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      980 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_xr_show_vrf_all_detail.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1562 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_hp_comware_display_arp.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      894 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_hp_comware_display_device_manuinfo.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2980 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_hp_comware_display_interface.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1385 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_hp_comware_display_ip_interface.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2702 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_hp_comware_display_ip_routing_table.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1038 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1687 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance_instance_name.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2035 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_hp_comware_display_link_aggregation_verbose.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2962 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_list.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3964 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_verbose.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1514 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_hp_comware_display_mac_address.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      895 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_hp_comware_display_vlan_all.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      899 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_hp_comware_display_vlan_brief.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1203 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_hp_comware_hostname.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1539 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_linux_arp__an.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1008 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_linux_hostname.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1412 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_linux_ip_address_show.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1933 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_linux_ip_link_show.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2526 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_linux_ip_route_show.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      711 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/ingestors/netmiko_linux_ip_vrf_show.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-15 13:20:12.510910 netdoc-0.9.65/netdoc/migrations/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    13632 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/migrations/0001_initial.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1800 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/migrations/0002_alter_arptableentry_custom_field_data_and_more.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3399 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/migrations/0003_alter_arptableentry_options_alter_credential_options_and_more.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3022 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/migrations/0004_alter_macaddresstableentry_options_and_more.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      577 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/migrations/0005_diagram_include_global_vrf_alter_diagram_details.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      453 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/migrations/0006_alter_routetableentry_metric.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      419 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/migrations/0007_discoverylog_supported.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/migrations/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    15079 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/models.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2805 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/navigation.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2988 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/nornir_inventory.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-15 13:20:12.510910 netdoc-0.9.65/netdoc/reports/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5880 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/reports/NetDoc.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-15 13:20:12.530911 netdoc-0.9.65/netdoc/schemas/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/schemas/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1937 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/schemas/arptableentry.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4719 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/schemas/cable.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1739 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/schemas/credential.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6493 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/schemas/device.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1508 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/schemas/devicerole.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1714 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/schemas/devicetype.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3905 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/schemas/discoverable.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3176 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/schemas/discoverylog.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     9788 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/schemas/interface.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1362 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/schemas/ipaddress.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1978 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/schemas/macaddresstableentry.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1453 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/schemas/manufacturer.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2015 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/schemas/prefix.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3018 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/schemas/routetableentry.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      884 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/schemas/site.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1623 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/schemas/vlan.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2476 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/schemas/vrf.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-15 13:20:12.530911 netdoc-0.9.65/netdoc/scripts/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    13085 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/scripts/NetDoc.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-15 13:20:12.454909 netdoc-0.9.65/netdoc/static/
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-15 13:20:12.458909 netdoc-0.9.65/netdoc/static/netdoc/
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-15 13:20:12.530911 netdoc-0.9.65/netdoc/static/netdoc/css/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.65/netdoc/static/netdoc/css/LICENSE
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      494 2023-04-05 08:40:22.000000 netdoc-0.9.65/netdoc/static/netdoc/css/README.md
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)   220164 2023-04-05 08:40:22.000000 netdoc-0.9.65/netdoc/static/netdoc/css/vis-network.min.css
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-15 13:20:12.542911 netdoc-0.9.65/netdoc/static/netdoc/img/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.65/netdoc/static/netdoc/img/LICENSE
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      305 2023-04-05 08:40:22.000000 netdoc-0.9.65/netdoc/static/netdoc/img/README.md
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     7415 2023-04-05 08:40:22.000000 netdoc-0.9.65/netdoc/static/netdoc/img/access-switch.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5648 2023-04-05 08:40:22.000000 netdoc-0.9.65/netdoc/static/netdoc/img/backup.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    28633 2023-04-05 08:40:22.000000 netdoc-0.9.65/netdoc/static/netdoc/img/circuit.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     8387 2023-04-05 08:40:22.000000 netdoc-0.9.65/netdoc/static/netdoc/img/core-switch.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     9522 2023-04-05 08:40:22.000000 netdoc-0.9.65/netdoc/static/netdoc/img/distribution-switch.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    15596 2023-04-05 08:40:22.000000 netdoc-0.9.65/netdoc/static/netdoc/img/firewall.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1614 2023-04-05 08:40:22.000000 netdoc-0.9.65/netdoc/static/netdoc/img/internal-switch.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5537 2023-04-05 08:40:22.000000 netdoc-0.9.65/netdoc/static/netdoc/img/isp-cpe-material.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5079 2023-04-05 08:40:22.000000 netdoc-0.9.65/netdoc/static/netdoc/img/non-racked-devices.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    15857 2023-04-05 08:40:22.000000 netdoc-0.9.65/netdoc/static/netdoc/img/power-feed.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    18685 2023-04-05 08:40:22.000000 netdoc-0.9.65/netdoc/static/netdoc/img/power-panel.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4710 2023-04-05 08:40:22.000000 netdoc-0.9.65/netdoc/static/netdoc/img/power-units.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    34335 2023-04-05 08:40:22.000000 netdoc-0.9.65/netdoc/static/netdoc/img/provider-networks.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    13504 2023-04-05 08:40:22.000000 netdoc-0.9.65/netdoc/static/netdoc/img/router.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4484 2023-04-05 08:40:22.000000 netdoc-0.9.65/netdoc/static/netdoc/img/server.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5648 2023-04-05 08:40:22.000000 netdoc-0.9.65/netdoc/static/netdoc/img/storage.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     8308 2023-04-05 08:40:22.000000 netdoc-0.9.65/netdoc/static/netdoc/img/unknown.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     7415 2023-04-05 08:40:22.000000 netdoc-0.9.65/netdoc/static/netdoc/img/wan-network.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6975 2023-04-05 08:40:22.000000 netdoc-0.9.65/netdoc/static/netdoc/img/wireless-ap.png
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-15 13:20:12.554911 netdoc-0.9.65/netdoc/static/netdoc/js/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.65/netdoc/static/netdoc/js/LICENSE
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      494 2023-04-05 08:40:22.000000 netdoc-0.9.65/netdoc/static/netdoc/js/README.md
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4198 2023-04-05 14:32:29.000000 netdoc-0.9.65/netdoc/static/netdoc/js/diagram.js
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1739 2023-04-05 08:40:22.000000 netdoc-0.9.65/netdoc/static/netdoc/js/netdoc.js
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)   702066 2023-04-05 08:40:22.000000 netdoc-0.9.65/netdoc/static/netdoc/js/vis-network.min.js
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)  1930592 2023-04-05 08:40:22.000000 netdoc-0.9.65/netdoc/static/netdoc/js/vis-network.min.js.map
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     8272 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/tables.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3912 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/tasks.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-15 13:20:12.458909 netdoc-0.9.65/netdoc/templates/
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-15 13:20:12.582912 netdoc-0.9.65/netdoc/templates/netdoc/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3038 2023-04-10 16:21:20.000000 netdoc-0.9.65/netdoc/templates/netdoc/arptableentry.html
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-15 13:20:12.582912 netdoc-0.9.65/netdoc/templates/netdoc/buttons/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      451 2023-04-10 16:17:25.000000 netdoc-0.9.65/netdoc/templates/netdoc/buttons/discover.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      337 2023-04-10 16:17:25.000000 netdoc-0.9.65/netdoc/templates/netdoc/buttons/export.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1669 2023-04-10 16:21:17.000000 netdoc-0.9.65/netdoc/templates/netdoc/credential.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1439 2023-04-10 16:29:06.000000 netdoc-0.9.65/netdoc/templates/netdoc/diagram.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2654 2023-04-10 16:23:32.000000 netdoc-0.9.65/netdoc/templates/netdoc/discoverable.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1217 2023-04-10 16:26:08.000000 netdoc-0.9.65/netdoc/templates/netdoc/discoverable_bulk_discover.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      638 2023-04-10 16:26:30.000000 netdoc-0.9.65/netdoc/templates/netdoc/discoverable_discover.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1006 2023-04-10 16:23:40.000000 netdoc-0.9.65/netdoc/templates/netdoc/discoverable_list.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5123 2023-04-10 16:23:17.000000 netdoc-0.9.65/netdoc/templates/netdoc/discoverylog.html
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-15 13:20:12.582912 netdoc-0.9.65/netdoc/templates/netdoc/htmx/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1005 2023-04-10 16:17:25.000000 netdoc-0.9.65/netdoc/templates/netdoc/htmx/discover_form.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1025 2023-04-10 16:17:25.000000 netdoc-0.9.65/netdoc/templates/netdoc/htmx/logexport_form.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3046 2023-04-10 16:20:47.000000 netdoc-0.9.65/netdoc/templates/netdoc/macaddresstableentry.html
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-15 13:20:12.582912 netdoc-0.9.65/netdoc/templatetags/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/templatetags/__init__.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-15 13:20:12.582912 netdoc-0.9.65/netdoc/templatetags/__pycache__/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      148 2023-05-10 09:50:17.000000 netdoc-0.9.65/netdoc/templatetags/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1048 2023-05-10 09:50:17.000000 netdoc-0.9.65/netdoc/templatetags/__pycache__/netdoc_buttons.cpython-310.pyc
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      890 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/templatetags/netdoc_buttons.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-15 13:20:12.582912 netdoc-0.9.65/netdoc/tests/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/tests/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    17018 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/tests/test.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    11615 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/topologies.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5128 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/urls.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    28388 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/utils.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    18479 2023-05-15 13:20:10.000000 netdoc-0.9.65/netdoc/views.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-15 13:20:12.482910 netdoc-0.9.65/netdoc.egg-info/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      469 2023-05-15 13:20:12.000000 netdoc-0.9.65/netdoc.egg-info/PKG-INFO
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6963 2023-05-15 13:20:12.000000 netdoc-0.9.65/netdoc.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2023-05-15 13:20:12.000000 netdoc-0.9.65/netdoc.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2023-04-05 14:49:45.000000 netdoc-0.9.65/netdoc.egg-info/not-zip-safe
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      161 2023-05-15 13:20:12.000000 netdoc-0.9.65/netdoc.egg-info/requires.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        7 2023-05-15 13:20:12.000000 netdoc-0.9.65/netdoc.egg-info/top_level.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      103 2023-05-15 13:20:12.586912 netdoc-0.9.65/setup.cfg
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1301 2023-05-15 13:20:10.000000 netdoc-0.9.65/setup.py
```

### Comparing `netdoc-0.9.64/LICENSE` & `netdoc-0.9.65/LICENSE`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/README.md` & `netdoc-0.9.65/README.md`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/__init__.py` & `netdoc-0.9.65/netdoc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Main class."""
 __author__ = "Andrea Dainese"
 __contact__ = "andrea@adainese.it"
 __copyright__ = "Copyright 2022, Andrea Dainese"
 __license__ = "GPLv3"
-__version__ = "0.9.64"
+__version__ = "0.9.65"
 
 import os
 import pkgutil
 import shutil
 
 from django.conf import settings
```

### Comparing `netdoc-0.9.64/netdoc/api/serializers.py` & `netdoc-0.9.65/netdoc/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/api/urls.py` & `netdoc-0.9.65/netdoc/api/urls.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/api/views.py` & `netdoc-0.9.65/netdoc/api/views.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/discoverers/netmiko_cisco_ios.py` & `netdoc-0.9.65/netdoc/discoverers/netmiko_cisco_ios.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/discoverers/netmiko_cisco_nxos.py` & `netdoc-0.9.65/netdoc/discoverers/netmiko_cisco_nxos.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/discoverers/netmiko_cisco_xr.py` & `netdoc-0.9.65/netdoc/discoverers/netmiko_cisco_xr.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/discoverers/netmiko_hp_comware.py` & `netdoc-0.9.65/netdoc/discoverers/netmiko_hp_comware.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/discoverers/netmiko_linux.py` & `netdoc-0.9.65/netdoc/discoverers/netmiko_linux.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/filtersets.py` & `netdoc-0.9.65/netdoc/filtersets.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/forms.py` & `netdoc-0.9.65/netdoc/forms.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_ios_hostname.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_ios_hostname.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_ios_show_cdp_neighbors_detail.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_ios_show_cdp_neighbors_detail.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_ios_show_etherchannel_summary.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_ios_show_etherchannel_summary.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_ios_show_interfaces.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_ios_show_interfaces.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_ios_show_interfaces_switchport.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_ios_show_interfaces_switchport.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_ios_show_inventory.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_ios_show_inventory.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_ios_show_ip_arp.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_ios_show_ip_arp.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_ios_show_ip_interface.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_ios_show_ip_interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_ios_show_ip_route.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_ios_show_ip_route.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_ios_show_lldp_neighbors_detail.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_ios_show_lldp_neighbors_detail.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_ios_show_mac_address_table.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_ios_show_mac_address_table.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_ios_show_vlan.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_ios_show_vlan.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_ios_show_vrf.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_ios_show_vrf.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_nxos_hostname.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_nxos_hostname.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_nxos_show_cdp_neighbors_detail.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_nxos_show_cdp_neighbors_detail.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_nxos_show_interface.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_nxos_show_interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_nxos_show_interface_switchport.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_nxos_show_interface_switchport.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_nxos_show_inventory.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_nxos_show_inventory.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_nxos_show_ip_arp.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_nxos_show_ip_arp.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_nxos_show_ip_interface.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_nxos_show_ip_interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_nxos_show_ip_route_vrf_all.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_nxos_show_ip_route_vrf_all.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_nxos_show_lldp_neighbors_detail.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_nxos_show_lldp_neighbors_detail.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_nxos_show_mac_address_table.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_nxos_show_mac_address_table.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_nxos_show_port_channel_summary.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_nxos_show_port_channel_summary.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_nxos_show_vlan.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_nxos_show_vlan.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_nxos_show_vrf.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_nxos_show_vrf.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_xr_admin_show_inventory.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_xr_admin_show_inventory.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_xr_hostname.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_xr_hostname.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_xr_show_arp.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_xr_show_arp.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_xr_show_cdp_neighbors_detail.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_xr_show_cdp_neighbors_detail.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_xr_show_interfaces.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_xr_show_interfaces.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_xr_show_ipv4_interface.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_xr_show_ipv4_interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_xr_show_lldp_neighbors.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_xr_show_lldp_neighbors.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_xr_show_route.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_xr_show_route.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_cisco_xr_show_vrf_all_detail.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_cisco_xr_show_vrf_all_detail.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_hp_comware_display_arp.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_hp_comware_display_arp.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_hp_comware_display_device_manuinfo.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_hp_comware_display_device_manuinfo.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_hp_comware_display_interface.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_hp_comware_display_interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_hp_comware_display_ip_interface.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_hp_comware_display_ip_interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_hp_comware_display_ip_routing_table.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_hp_comware_display_ip_routing_table.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance_instance_name.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance_instance_name.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_hp_comware_display_link_aggregation_verbose.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_hp_comware_display_link_aggregation_verbose.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_list.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_list.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_verbose.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_verbose.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_hp_comware_display_mac_address.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_hp_comware_display_mac_address.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_hp_comware_display_vlan_all.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_hp_comware_display_vlan_all.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_hp_comware_display_vlan_brief.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_hp_comware_display_vlan_brief.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_hp_comware_hostname.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_hp_comware_hostname.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_linux_arp__an.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_linux_arp__an.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_linux_hostname.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_linux_hostname.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_linux_ip_address_show.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_linux_ip_address_show.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_linux_ip_link_show.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_linux_ip_link_show.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_linux_ip_route_show.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_linux_ip_route_show.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/ingestors/netmiko_linux_ip_vrf_show.py` & `netdoc-0.9.65/netdoc/ingestors/netmiko_linux_ip_vrf_show.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/migrations/0001_initial.py` & `netdoc-0.9.65/netdoc/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/migrations/0002_alter_arptableentry_custom_field_data_and_more.py` & `netdoc-0.9.65/netdoc/migrations/0002_alter_arptableentry_custom_field_data_and_more.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/migrations/0003_alter_arptableentry_options_alter_credential_options_and_more.py` & `netdoc-0.9.65/netdoc/migrations/0003_alter_arptableentry_options_alter_credential_options_and_more.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/migrations/0004_alter_macaddresstableentry_options_and_more.py` & `netdoc-0.9.65/netdoc/migrations/0004_alter_macaddresstableentry_options_and_more.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/migrations/0005_diagram_include_global_vrf_alter_diagram_details.py` & `netdoc-0.9.65/netdoc/migrations/0005_diagram_include_global_vrf_alter_diagram_details.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/models.py` & `netdoc-0.9.65/netdoc/models.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/navigation.py` & `netdoc-0.9.65/netdoc/navigation.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/nornir_inventory.py` & `netdoc-0.9.65/netdoc/nornir_inventory.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/reports/NetDoc.py` & `netdoc-0.9.65/netdoc/reports/NetDoc.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/schemas/arptableentry.py` & `netdoc-0.9.65/netdoc/schemas/arptableentry.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/schemas/cable.py` & `netdoc-0.9.65/netdoc/schemas/cable.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/schemas/credential.py` & `netdoc-0.9.65/netdoc/schemas/credential.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/schemas/device.py` & `netdoc-0.9.65/netdoc/schemas/device.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/schemas/devicerole.py` & `netdoc-0.9.65/netdoc/schemas/devicerole.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/schemas/devicetype.py` & `netdoc-0.9.65/netdoc/schemas/devicetype.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/schemas/discoverable.py` & `netdoc-0.9.65/netdoc/schemas/discoverable.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/schemas/discoverylog.py` & `netdoc-0.9.65/netdoc/schemas/discoverylog.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/schemas/interface.py` & `netdoc-0.9.65/netdoc/schemas/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,15 +216,15 @@
         for vid in tagged_vlans:
             if vid not in current_tagged_vlan_list:
                 vlans_to_be_added.append(vid)
 
         # Find VLANs to be removed
         for vid in current_tagged_vlan_list:
             if vid not in tagged_vlans:
-                vlans_to_be_removed.append(vlan)
+                vlans_to_be_removed.append(vid)
 
         # Find missing VLANs
         for tagged_vlan in tagged_vlans:
             if tagged_vlan not in existent_vlan_list:
                 # VLAN needs to be created and added to interface (tagged)
                 vlans_to_be_created.append(
                     VLAN_model(
```

### Comparing `netdoc-0.9.64/netdoc/schemas/ipaddress.py` & `netdoc-0.9.65/netdoc/schemas/ipaddress.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/schemas/macaddresstableentry.py` & `netdoc-0.9.65/netdoc/schemas/macaddresstableentry.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/schemas/manufacturer.py` & `netdoc-0.9.65/netdoc/schemas/manufacturer.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/schemas/prefix.py` & `netdoc-0.9.65/netdoc/schemas/prefix.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/schemas/routetableentry.py` & `netdoc-0.9.65/netdoc/schemas/routetableentry.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/schemas/site.py` & `netdoc-0.9.65/netdoc/schemas/site.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/schemas/vlan.py` & `netdoc-0.9.65/netdoc/schemas/vlan.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/schemas/vrf.py` & `netdoc-0.9.65/netdoc/schemas/vrf.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/scripts/NetDoc.py` & `netdoc-0.9.65/netdoc/scripts/NetDoc.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/static/netdoc/css/LICENSE` & `netdoc-0.9.65/netdoc/static/netdoc/css/LICENSE`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/static/netdoc/css/vis-network.min.css` & `netdoc-0.9.65/netdoc/static/netdoc/css/vis-network.min.css`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/static/netdoc/img/LICENSE` & `netdoc-0.9.65/netdoc/static/netdoc/img/LICENSE`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/static/netdoc/img/access-switch.png` & `netdoc-0.9.65/netdoc/static/netdoc/img/access-switch.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/static/netdoc/img/backup.png` & `netdoc-0.9.65/netdoc/static/netdoc/img/backup.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/static/netdoc/img/circuit.png` & `netdoc-0.9.65/netdoc/static/netdoc/img/circuit.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/static/netdoc/img/core-switch.png` & `netdoc-0.9.65/netdoc/static/netdoc/img/core-switch.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/static/netdoc/img/distribution-switch.png` & `netdoc-0.9.65/netdoc/static/netdoc/img/distribution-switch.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/static/netdoc/img/firewall.png` & `netdoc-0.9.65/netdoc/static/netdoc/img/firewall.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/static/netdoc/img/internal-switch.png` & `netdoc-0.9.65/netdoc/static/netdoc/img/internal-switch.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/static/netdoc/img/isp-cpe-material.png` & `netdoc-0.9.65/netdoc/static/netdoc/img/isp-cpe-material.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/static/netdoc/img/non-racked-devices.png` & `netdoc-0.9.65/netdoc/static/netdoc/img/non-racked-devices.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/static/netdoc/img/power-feed.png` & `netdoc-0.9.65/netdoc/static/netdoc/img/power-feed.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/static/netdoc/img/power-panel.png` & `netdoc-0.9.65/netdoc/static/netdoc/img/power-panel.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/static/netdoc/img/power-units.png` & `netdoc-0.9.65/netdoc/static/netdoc/img/power-units.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/static/netdoc/img/provider-networks.png` & `netdoc-0.9.65/netdoc/static/netdoc/img/provider-networks.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/static/netdoc/img/router.png` & `netdoc-0.9.65/netdoc/static/netdoc/img/router.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/static/netdoc/img/server.png` & `netdoc-0.9.65/netdoc/static/netdoc/img/server.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/static/netdoc/img/storage.png` & `netdoc-0.9.65/netdoc/static/netdoc/img/storage.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/static/netdoc/img/unknown.png` & `netdoc-0.9.65/netdoc/static/netdoc/img/unknown.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/static/netdoc/img/wan-network.png` & `netdoc-0.9.65/netdoc/static/netdoc/img/wan-network.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/static/netdoc/img/wireless-ap.png` & `netdoc-0.9.65/netdoc/static/netdoc/img/wireless-ap.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/static/netdoc/js/LICENSE` & `netdoc-0.9.65/netdoc/static/netdoc/js/LICENSE`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/static/netdoc/js/diagram.js` & `netdoc-0.9.65/netdoc/static/netdoc/js/diagram.js`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/static/netdoc/js/netdoc.js` & `netdoc-0.9.65/netdoc/static/netdoc/js/netdoc.js`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/static/netdoc/js/vis-network.min.js` & `netdoc-0.9.65/netdoc/static/netdoc/js/vis-network.min.js`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/static/netdoc/js/vis-network.min.js.map` & `netdoc-0.9.65/netdoc/static/netdoc/js/vis-network.min.js.map`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/tables.py` & `netdoc-0.9.65/netdoc/tables.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/tasks.py` & `netdoc-0.9.65/netdoc/tasks.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/templates/netdoc/arptableentry.html` & `netdoc-0.9.65/netdoc/templates/netdoc/arptableentry.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/templates/netdoc/credential.html` & `netdoc-0.9.65/netdoc/templates/netdoc/credential.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/templates/netdoc/diagram.html` & `netdoc-0.9.65/netdoc/templates/netdoc/diagram.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/templates/netdoc/discoverable.html` & `netdoc-0.9.65/netdoc/templates/netdoc/discoverable.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/templates/netdoc/discoverable_bulk_discover.html` & `netdoc-0.9.65/netdoc/templates/netdoc/discoverable_bulk_discover.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/templates/netdoc/discoverable_discover.html` & `netdoc-0.9.65/netdoc/templates/netdoc/discoverable_discover.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/templates/netdoc/discoverable_list.html` & `netdoc-0.9.65/netdoc/templates/netdoc/discoverable_list.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/templates/netdoc/discoverylog.html` & `netdoc-0.9.65/netdoc/templates/netdoc/discoverylog.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/templates/netdoc/htmx/discover_form.html` & `netdoc-0.9.65/netdoc/templates/netdoc/htmx/discover_form.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/templates/netdoc/htmx/logexport_form.html` & `netdoc-0.9.65/netdoc/templates/netdoc/htmx/logexport_form.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/templates/netdoc/macaddresstableentry.html` & `netdoc-0.9.65/netdoc/templates/netdoc/macaddresstableentry.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/templatetags/__pycache__/netdoc_buttons.cpython-310.pyc` & `netdoc-0.9.65/netdoc/templatetags/__pycache__/netdoc_buttons.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri May  5 14:52:59 2023 UTC, .py size: 890 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4b18 5564 7a03 0000  o.......K.Udz...
+00000000: 6f0d 0d0a 0000 0000 a867 5b64 7a03 0000  o........g[dz...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 5a00 6401 5a01 6402 5a02 6403 5a03 6404  Z.d.Z.d.Z.d.Z.d.
 00000040: 5a04 6405 6406 6c05 6d06 5a06 0100 6405  Z.d.d.l.m.Z...d.
 00000050: 6407 6c07 6d08 5a08 0100 6405 6408 6c09  d.l.m.Z...d.d.l.
 00000060: 6d0a 5a0a 0100 6506 a00b a100 5a0c 650c  m.Z...e.....Z.e.
 00000070: a00d 6409 a101 640a 640b 8400 8301 5a0e  ..d...d.d.....Z.
```

### Comparing `netdoc-0.9.64/netdoc/templatetags/netdoc_buttons.py` & `netdoc-0.9.65/netdoc/templatetags/netdoc_buttons.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/tests/test.py` & `netdoc-0.9.65/netdoc/tests/test.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/topologies.py` & `netdoc-0.9.65/netdoc/topologies.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/urls.py` & `netdoc-0.9.65/netdoc/urls.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/utils.py` & `netdoc-0.9.65/netdoc/utils.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc/views.py` & `netdoc-0.9.65/netdoc/views.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/netdoc.egg-info/SOURCES.txt` & `netdoc-0.9.65/netdoc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.64/setup.py` & `netdoc-0.9.65/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,36 +9,36 @@
     twine upload dist/*
 """
 
 __author__ = "Andrea Dainese"
 __contact__ = "andrea@adainese.it"
 __copyright__ = "Copyright 2022, Andrea Dainese"
 __license__ = "GPLv3"
-__version__ = "0.9.64"
+__version__ = "0.9.65"
 
 from setuptools import find_packages, setup
 
 setup(
     name="netdoc",
     version=__version__,
     description="Network Documentation plugin for NetBox",
     url="https://github.com/dainok/netdoc",
     author="Andrea Dainese",
     author_email="andrea@adainese.it",
     license="GNU v3.0",
     install_requires=[
-        "jsonschema",
+        "jsonschema==3.2.0",
         "python-slugify",
         "netmiko==4.1.2",
         "nornir==3.3.0",
         "nornir_netmiko==0.2.0",
         "nornir_utils",
-        "ipaddress",
-        "macaddress",
-        "ouilookup",
+        "ipaddress==1.0.23",
+        "macaddress==2.0.2",
+        "ouilookup==0.2.4",
         "n2g==0.3.3",
     ],
     packages=find_packages(),
     include_package_data=True,
     zip_safe=False,
     classifiers=[
         "Programming Language :: Python",
```

