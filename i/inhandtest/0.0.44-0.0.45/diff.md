# Comparing `tmp/inhandtest-0.0.44.tar.gz` & `tmp/inhandtest-0.0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\inhandtest-0.0.44.tar", last modified: Thu May 11 09:23:18 2023, max compression
+gzip compressed data, was "dist\inhandtest-0.0.45.tar", last modified: Mon May 15 10:20:08 2023, max compression
```

## Comparing `inhandtest-0.0.44.tar` & `inhandtest-0.0.45.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 09:23:18.000000 inhandtest-0.0.44/
--rw-rw-rw-   0        0        0      535 2023-05-11 09:23:18.000000 inhandtest-0.0.44/PKG-INFO
--rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.44/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 09:23:18.000000 inhandtest-0.0.44/inhandtest/
--rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.44/inhandtest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 09:23:18.000000 inhandtest-0.0.44/inhandtest/base_page/
--rw-rw-rw-   0        0        0      134 2023-03-15 06:05:35.000000 inhandtest-0.0.44/inhandtest/base_page/__init__.py
--rw-rw-rw-   0        0        0    39362 2023-05-10 08:44:26.000000 inhandtest-0.0.44/inhandtest/base_page/_ig902_contents_locators.py
--rw-rw-rw-   0        0        0    27870 2023-05-10 08:56:15.000000 inhandtest-0.0.44/inhandtest/base_page/_ir3XX_contents_locators.py
--rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.44/inhandtest/base_page/_vg710_contents_locators.py
--rw-rw-rw-   0        0        0    46619 2023-05-11 07:10:20.000000 inhandtest-0.0.44/inhandtest/base_page/base_page.py
--rw-rw-rw-   0        0        0    10957 2023-05-09 09:49:30.000000 inhandtest-0.0.44/inhandtest/base_page/table_tr.py
--rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.44/inhandtest/exception.py
--rw-rw-rw-   0        0        0     3890 2023-03-30 10:08:49.000000 inhandtest-0.0.44/inhandtest/file.py
--rw-rw-rw-   0        0        0    11861 2023-05-06 01:56:01.000000 inhandtest-0.0.44/inhandtest/inmodbus.py
--rw-rw-rw-   0        0        0     4880 2023-04-27 01:05:22.000000 inhandtest-0.0.44/inhandtest/inmongodb.py
--rw-rw-rw-   0        0        0    22049 2023-03-30 10:08:49.000000 inhandtest-0.0.44/inhandtest/inmqtt.py
--rw-rw-rw-   0        0        0    47101 2023-05-11 09:21:27.000000 inhandtest-0.0.44/inhandtest/inrequest.py
--rw-rw-rw-   0        0        0     7583 2023-05-06 07:36:44.000000 inhandtest-0.0.44/inhandtest/inserial.py
--rw-rw-rw-   0        0        0    12335 2023-04-06 06:40:29.000000 inhandtest-0.0.44/inhandtest/insocket.py
--rw-rw-rw-   0        0        0     6213 2023-05-06 01:08:13.000000 inhandtest-0.0.44/inhandtest/inssh.py
--rw-rw-rw-   0        0        0     1144 2023-03-30 10:18:47.000000 inhandtest-0.0.44/inhandtest/ip.py
--rw-rw-rw-   0        0        0    11620 2023-05-08 10:30:07.000000 inhandtest-0.0.44/inhandtest/mail.py
--rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.44/inhandtest/pytest_email.html
--rw-rw-rw-   0        0        0    32728 2023-05-06 01:14:17.000000 inhandtest-0.0.44/inhandtest/telnet.py
--rw-rw-rw-   0        0        0    25276 2023-05-08 10:30:07.000000 inhandtest-0.0.44/inhandtest/tools.py
--rw-rw-rw-   0        0        0      123 2023-05-06 01:36:21.000000 inhandtest-0.0.44/requirements.txt
--rw-rw-rw-   0        0        0     1438 2023-05-11 09:22:27.000000 inhandtest-0.0.44/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 10:20:08.000000 inhandtest-0.0.45/
+-rw-rw-rw-   0        0        0      535 2023-05-15 10:20:08.000000 inhandtest-0.0.45/PKG-INFO
+-rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.45/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 10:20:08.000000 inhandtest-0.0.45/inhandtest/
+-rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.45/inhandtest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 10:20:08.000000 inhandtest-0.0.45/inhandtest/base_page/
+-rw-rw-rw-   0        0        0      134 2023-03-15 06:05:35.000000 inhandtest-0.0.45/inhandtest/base_page/__init__.py
+-rw-rw-rw-   0        0        0    38524 2023-05-15 06:31:20.000000 inhandtest-0.0.45/inhandtest/base_page/_ig_contents_locators.py
+-rw-rw-rw-   0        0        0    27870 2023-05-10 08:56:15.000000 inhandtest-0.0.45/inhandtest/base_page/_ir3XX_contents_locators.py
+-rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.45/inhandtest/base_page/_vg710_contents_locators.py
+-rw-rw-rw-   0        0        0    49374 2023-05-15 08:48:06.000000 inhandtest-0.0.45/inhandtest/base_page/base_page.py
+-rw-rw-rw-   0        0        0    10957 2023-05-09 09:49:30.000000 inhandtest-0.0.45/inhandtest/base_page/table_tr.py
+-rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.45/inhandtest/exception.py
+-rw-rw-rw-   0        0        0     3890 2023-03-30 10:08:49.000000 inhandtest-0.0.45/inhandtest/file.py
+-rw-rw-rw-   0        0        0    11861 2023-05-06 01:56:01.000000 inhandtest-0.0.45/inhandtest/inmodbus.py
+-rw-rw-rw-   0        0        0     4880 2023-04-27 01:05:22.000000 inhandtest-0.0.45/inhandtest/inmongodb.py
+-rw-rw-rw-   0        0        0    22049 2023-03-30 10:08:49.000000 inhandtest-0.0.45/inhandtest/inmqtt.py
+-rw-rw-rw-   0        0        0    48029 2023-05-15 10:04:52.000000 inhandtest-0.0.45/inhandtest/inrequest.py
+-rw-rw-rw-   0        0        0     7583 2023-05-06 07:36:44.000000 inhandtest-0.0.45/inhandtest/inserial.py
+-rw-rw-rw-   0        0        0    12335 2023-04-06 06:40:29.000000 inhandtest-0.0.45/inhandtest/insocket.py
+-rw-rw-rw-   0        0        0     6076 2023-05-15 10:19:14.000000 inhandtest-0.0.45/inhandtest/inssh.py
+-rw-rw-rw-   0        0        0     1144 2023-03-30 10:18:47.000000 inhandtest-0.0.45/inhandtest/ip.py
+-rw-rw-rw-   0        0        0    11620 2023-05-08 10:30:07.000000 inhandtest-0.0.45/inhandtest/mail.py
+-rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.45/inhandtest/pytest_email.html
+-rw-rw-rw-   0        0        0    32728 2023-05-06 01:14:17.000000 inhandtest-0.0.45/inhandtest/telnet.py
+-rw-rw-rw-   0        0        0    25281 2023-05-12 08:18:46.000000 inhandtest-0.0.45/inhandtest/tools.py
+-rw-rw-rw-   0        0        0      137 2023-05-15 07:42:26.000000 inhandtest-0.0.45/requirements.txt
+-rw-rw-rw-   0        0        0     1450 2023-05-15 10:19:56.000000 inhandtest-0.0.45/setup.py
```

### Comparing `inhandtest-0.0.44/PKG-INFO` & `inhandtest-0.0.45/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: inhandtest
-Version: 0.0.44
+Version: 0.0.45
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 License: UNKNOWN
 Description: 方便inhand测试同事在自动化测试时，对通用协议或者常用工具及方法做封装，需要使用时即在线安装；
         映翰通出品，追尾必究！
```

### Comparing `inhandtest-0.0.44/README.md` & `inhandtest-0.0.45/README.md`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.44/inhandtest/base_page/_ig902_contents_locators.py` & `inhandtest-0.0.45/inhandtest/base_page/_ig_contents_locators.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 # -*- coding: utf-8 -*-
 # @Time   : 2023/3/31 14:40
 # @Author : zhangzhongtian
-# @File   : _ig902_contents_locators.py
+# @File   : _ig_contents_locators.py
 """
-_ig902_contents_locators
+_ig_contents_locators
 
 """
 from playwright.sync_api import Locator, Page
 
 
 class IGContentsLocators:
 
     def __init__(self, page: Page, language='en', model='IG902'):
+        """
+
+        :param page:
+        :param language:
+        :param model: 当前匹配IG902  IG502
+        """
         self.page = page
         self.language = language
         self.model = model.upper()
         if language == 'en':
             self.__locale: dict = {'network': 'Network', 'network_interface': 'Network Interface',
-                                   'network_interface_cellular': 'Cellular', 'network_interface_ethernet': 'Ethernet',
-                                   'network_interface_bridge': 'Bridge', 'network_interface_loopback': 'Loopback',
-                                   'network_service': 'Network Services', 'network_service_dhcp': 'DHCP',
-                                   'network_service_dns': 'DNS', "gps_configure": "GPS Configure",
+                                   'cellular': 'Cellular', 'ethernet': 'Ethernet',
+                                   'performance': 'Performance And Storage',
+                                   'bridge': 'Bridge', 'loopback': 'Loopback',
+                                   'network_service': 'Network Services', 'dhcp': 'DHCP',
+                                   'dns': 'DNS', "gps_configure": "GPS Configure", 'gps': 'Status',
                                    "gps_ip_forwarding": "GPS IP Forwarding",
                                    "gps_serial_forwarding": "GPS Serial Forwarding",
-                                   'network_service_host': 'Host List', 'network_routing': 'Routing',
-                                   'network_routing_status': 'Routing Status',
-                                   'network_routing_static': 'Static Routing', 'network_firewall': 'Firewall',
-                                   'network_firewall_acl': 'ACL', 'network_firewall_nat': 'NAT',
-                                   'l2tp_status': 'Status', 'l2tp_client': 'L2TP Client',
+                                   'host_list': 'Host List', 'routing': 'Routing',
+                                   'routing_status': 'Routing Status',
+                                   'routing_static': 'Static Routing', 'firewall': 'Firewall',
+                                   'acl': 'ACL', 'nat': 'NAT',
+                                   'status': 'Status', 'l2tp_client': 'L2TP Client',
                                    'l2tp_service': 'L2TP Service',
                                    'edge': 'Edge Computing', 'python_edge': 'Python Edge Computing',
                                    'docker_manager': 'Docker Manager', 'cloud_edge_computing': 'Cloud Edge Computing',
                                    'device_supervisor': 'Device Supervisor', 'measure_monitor': 'Measure Monitor',
                                    'monitoring_list': 'Monitoring List', 'group': 'Group',
                                    'alarm': 'Alarm', 'realtime_alarms': 'Realtime Alarms', 'alarm_rules': 'Alarm Rules',
                                    'history_alarms': 'History Alarms', 'alarm_label': 'Alarm Label',
@@ -39,198 +46,151 @@
                                    'whitehawk_energy_manager': 'Whitehawk Energy Manager', 'protocol': 'Protocol',
                                    'parameter_settings': 'Parameter Settings',
                                    'custom_quickfunctions': 'Custom QuickFunctions',
                                    'system': 'System', 'system_time': 'System Time', 'system_log': 'Log',
                                    'system_config': 'Configuration Management', 'system_cloud': 'InHand Cloud',
                                    'system_firmware': 'Firmware Upgrade', 'system_tools': 'Access Tools',
                                    'system_user_management': 'User Management', 'system_reboot': 'Reboot',
-                                   'system_network_tools': 'Network Tools', 'logout': 'Logout',
-                                   'system_3rd_party': '3rd Party Notification', 'logout_submit': 'Confirm',
+                                   'system_network_tools': 'Network Tools',
+                                   'system_3rd_party': '3rd Party Notification',
                                    'configuration': ' Configuration', 'trigger_condition': 'Trigger Condition',
                                    'gigabitethernet': 'Gigabitethernet',
                                    }
         else:
-            self.__locale: dict = {'network': '网络', 'network_interface': '网络接口',
-                                   'network_interface_cellular': '蜂窝网', 'network_interface_ethernet': '以太网',
-                                   'network_interface_bridge': '桥接口', 'network_interface_loopback': '环回接口',
-                                   'network_service': '网络服务', 'network_service_dhcp': 'DHCP服务',
-                                   'network_service_dns': 'DNS服务', "gps_configure": "GPS 配置",
+            self.__locale: dict = {'network': '网络', 'network_interface': '网络接口', 'performance': '性能与存储',
+                                   'cellular': '蜂窝网', 'ethernet': '以太网',
+                                   'bridge': '桥接口', 'loopback': '环回接口',
+                                   'network_service': '网络服务', 'dhcp': 'DHCP服务',
+                                   'dns': 'DNS服务', "gps_configure": "GPS 配置", 'gps': 'GPS',
                                    "gps_ip_forwarding": "GPS IP转发",
-                                   "gps_serial_forwarding": "GPS 串口转发", 'network_service_host': '主机列表',
-                                   'network_routing': '路由', 'network_routing_status': '路由状态',
-                                   'network_routing_static': '静态路由', 'network_firewall': '防火墙',
-                                   'network_firewall_acl': '访问控制列表', 'network_firewall_nat': '网络地址转换',
-                                   'l2tp_status': '状态', 'l2tp_client': 'L2TP客户端', 'l2tp_service': 'L2TP服务器',
+                                   "gps_serial_forwarding": "GPS 串口转发", 'host_list': '主机列表',
+                                   'routing': '路由', 'routing_status': '路由状态',
+                                   'routing_static': '静态路由', 'firewall': '防火墙',
+                                   'acl': '访问控制列表', 'nat': '网络地址转换',
+                                   'status': '状态', 'l2tp_client': 'L2TP客户端', 'l2tp_service': 'L2TP服务器',
                                    'edge': '边缘计算', 'python_edge': 'Python边缘计算', 'docker_manager': 'Docker 管理',
                                    'cloud_edge_computing': '公有云边缘计算', 'device_supervisor': '设备监控',
                                    'measure_monitor': '测点监控', 'monitoring_list': '监控列表', 'group': '分组',
                                    'alarm': '告警', 'realtime_alarms': '实时告警', 'alarm_rules': '告警规则',
                                    'history_alarms': '历史告警', 'alarm_label': '告警标签',
                                    'cloud': '云服务', 'mqtt_cloud_service': 'MQTT云服务',
                                    'whitehawk_energy_manager': '白鹰能源管家', 'protocol': '协议转换',
                                    'parameter_settings': '参数设置', 'custom_quickfunctions': '自定义快函数',
                                    'system': '系统管理', 'system_time': '系统时间', 'system_log': '系统日志',
                                    'system_config': '配置管理', 'system_cloud': '设备云平台',
                                    'system_firmware': '固件升级', 'system_tools': '管理工具',
                                    'system_user_management': '用户管理', 'system_reboot': '重启',
                                    'system_network_tools': '工具', 'system_3rd_party': '第三方软件声明',
-                                   'logout': '退出登录', 'logout_submit': '确 认', 'configuration': '配置',
+                                   'configuration': '配置',
                                    'trigger_condition': '触发条件', 'gigabitethernet': '千兆以太网口',
                                    }
 
-    def content_span_text(self, menu) -> Locator:
-        one_menu = {"en": {"overview": "Performance And Storage", "cellular": "Enable Cellular",
-                           "ethernet": "Gigabitethernet 0/1", "bridge": "Bridge Member",
-                           "wlan": "Wireless Connection Status", "loopback": "127.0.0.1",
-                           "dhcp": "DHCP Server", "dns": "DNS Server", "gps": "GPS Configure",
-                           "host_list": "MAC Address", "routing_status": "Distance/Metric",
-                           "static_routing": "Track ID", "acl": "Access Control Strategy",
-                           "nat": "Network Address Translation(NAT) Rules",
-                           "l2tp_status": "Local Session ID", "l2tp_client": "L2TPv3 Session",
-                           "l2tp_service": "Enable L2TP Server", "python_edge_computing": "Python Engine",
-                           "docker_manager": "Enable Docker Manager", "cloud_edge_computing": "Azure IoT Edge",
-                           "azure_iot_edge": "Enable Security Daemon",
-                           "aws_iot_greengrass": "Enable AWS IoT Greengrass",
-                           "measure_monitor": "Controller List", "alarm": "Realtime Alarms",
-                           "cloud": "MQTT Cloud Service", "mqtt_cloud_service": "Enable Cloud",
-                           "whitehawk_energy_manager": "Enable Whitehawk Energy Manager",
-                           "protocol": "Modbus TCP Slave",
-                           "parameter_settings": "Serial Port Settings", "custom_quickfunctions": "QuickFunction List",
-                           "system_time": "Enable SNTP Clients", "log": "View Recent",
-                           "log_configure": "Send to the remote log server",
-                           "configuration_management": "Configuration Files Operations",
-                           "inhand_cloud": "InHand Connect Service", "firmware_upgrade": "Select Firmware",
-                           "access_tools": "Enable HTTPS", "user_management": "User Permissions",
-                           "reboot": "Immediately Reboot", "network_tools": "Traceroute",
-                           "3rd_party_notification": "Third Party Software Notifications and Licenses"
-                           },
-                    'cn': {"overview": "性能与存储", "cellular": "启用蜂窝网", "ethernet": "千兆以太网口 0/1",
-                           "bridge": "网桥成员", "wlan": "无线连接状态", "loopback": "127.0.0.1",
-                           "dhcp": "DHCP 服务器", "dns": "域名服务器", "gps": "GPS 配置", "host_list": "MAC地址",
-                           "routing_status": "距离/度量", "static_routing": "Track标识", "acl": "访问控制策略",
-                           "nat": "网络地址转换(NAT)规则", "l2tp": "L2TP客户端", "l2tp_status": "本地隧道会话ID",
-                           "l2tp_client": "L2TPv3会话", "l2tp_service": "启用L2TP服务器",
-                           "python_edge_computing": "Python边缘计算引擎", "docker_manager": "启用Docker管理器",
-                           "cloud_edge_computing": "Azure IoT Edge", "azure_iot_edge": "启用安全守护程序",
-                           "aws_iot_greengrass": "启用AWS IoT Greengrass", "measure_monitor": "控制器列表",
-                           "alarm": "实时告警", "cloud": "MQTT云服务", "mqtt_cloud_service": "启用云服务",
-                           "whitehawk_energy_manager": "启用白鹰能源管家", "protocol": "Modbus TCP Slave",
-                           "parameter_settings": "串口设置", "custom_quickfunctions": "快函数列表",
-                           "system_time": "启用SNTP客户端", "log": "查看最新的",
-                           "log_configure": "发送到远程日志服务器", "configuration_management": "配置文件操作",
-                           "inhand_cloud": "InHand Connect Service", "firmware_upgrade": "选择固件",
-                           "access_tools": "启用HTTPS", "user_management": "用户权限",
-                           "reboot": "立即重启", "network_tools": "路由探测",
-                           "3rd_party_notification": "Third Party Software Notifications and Licenses"
-
-                           }}
-        if self.language == 'en':
-            span_text = one_menu.get('en').get(menu)
-        else:
-            span_text = one_menu.get('cn').get(menu)
-        return self.page.locator(f'text={span_text}')
+    def content_target(self, locale) -> Locator:
+        if self.__locale.get(locale):
+            locale = self.__locale.get(locale)
+        return self.page.locator(f'//span[@class="ant-breadcrumb-link"]/span[text()="{locale}"]')
 
     @property
     def overview_menu(self) -> Locator:
-        return self.page.locator('//*[@id="root"]/div/section/section/header/div/div/div[1]/div[2]/div/ul/li[2]/a')
+        return self.page.locator('//a[@href="/overview"]')
 
     @property
     def network_menu(self) -> Locator:
-        return self.page.locator('//*[@id="root"]/div/section/section/header/div/div/div[1]/div[2]/div/ul/li[4]/a')
+        return self.page.locator('//a[@href="/network"]')
 
     @property
     def edge_menu(self) -> Locator:
-        return self.page.locator('//*[@id="root"]/div/section/section/header/div/div/div[1]/div[2]/div/ul/li[6]/a')
+        return self.page.locator('//li[@role="menuitem"]/a[@href="/edge-computing"]')
 
     @property
     def system_menu(self) -> Locator:
-        return self.page.locator('//*[@id="root"]/div/section/section/header/div/div/div[1]/div[2]/div/ul/li[8]/a')
+        return self.page.locator('//li[@role="menuitem"]/a[@href="/system"]')
 
     @property
     def network_interface_menu(self) -> Locator:
         return self.page.locator(f'div:text-is("{self.__locale.get("network_interface")}")')
 
     @property
-    def network_interface_cellular_menu(self) -> Locator:
-        return self.page.locator(f'a:has-text("{self.__locale.get("network_interface_cellular")}")')
+    def cellular_menu(self) -> Locator:
+        return self.page.locator(f'a:has-text("{self.__locale.get("cellular")}")')
 
     @property
-    def network_interface_ethernet_menu(self) -> Locator:
-        return self.page.locator(f'a:has-text("{self.__locale.get("network_interface_ethernet")}")')
+    def ethernet_menu(self) -> Locator:
+        return self.page.locator(f'a:has-text("{self.__locale.get("ethernet")}")')
 
     @property
-    def network_interface_bridge_menu(self) -> Locator:
-        return self.page.locator(f'a:has-text("{self.__locale.get("network_interface_bridge")}")')
+    def bridge_menu(self) -> Locator:
+        return self.page.locator(f'a:has-text("{self.__locale.get("bridge")}")')
 
     @property
-    def network_interface_wlan_menu(self) -> Locator:
+    def wlan_menu(self) -> Locator:
         return self.page.locator('a:has-text("WLAN")')
 
     @property
-    def network_interface_loopback_menu(self) -> Locator:
-        return self.page.locator(f'a:has-text("{self.__locale.get("network_interface_loopback")}")')
+    def loopback_menu(self) -> Locator:
+        return self.page.locator(f'a:has-text("{self.__locale.get("loopback")}")')
 
     @property
-    def network_interface_502_wan_menu(self) -> Locator:
+    def wan_menu_502(self) -> Locator:
         return self.page.locator('a:has-text("WAN")')
 
     @property
-    def network_interface_502_lan_menu(self) -> Locator:
+    def lan_menu_502(self) -> Locator:
         return self.page.locator('a:has-text("LAN")')
 
     @property
     def network_service_menu(self) -> Locator:
         return self.page.locator(f'div:text-is("{self.__locale.get("network_service")}")')
 
     @property
-    def network_service_dhcp_menu(self) -> Locator:
-        return self.page.locator(f'a:has-text("{self.__locale.get("network_service_dhcp")}")')
+    def dhcp_menu(self) -> Locator:
+        return self.page.locator(f'a:has-text("{self.__locale.get("dhcp")}")')
 
     @property
-    def network_service_dns_menu(self) -> Locator:
-        return self.page.locator(f'a:has-text("{self.__locale.get("network_service_dns")}")')
+    def dns_menu(self) -> Locator:
+        return self.page.locator(f'a:has-text("{self.__locale.get("dns")}")')
 
     @property
-    def network_service_gps_menu(self) -> Locator:
+    def gps_menu(self) -> Locator:
         return self.page.locator('a:has-text("GPS")')
 
     @property
-    def network_service_host_menu(self) -> Locator:
-        return self.page.locator(f'a:has-text("{self.__locale.get("network_service_host")}")')
+    def host_list_menu(self) -> Locator:
+        return self.page.locator(f'a:has-text("{self.__locale.get("host_list")}")')
 
     @property
-    def network_routing_menu(self) -> Locator:
-        return self.page.locator(f'div:text-is("{self.__locale.get("network_routing")}")')
+    def routing_menu(self) -> Locator:
+        return self.page.locator(f'div:text-is("{self.__locale.get("routing")}")')
 
     @property
-    def network_routing_status_menu(self) -> Locator:
-        return self.page.locator(f'a:has-text("{self.__locale.get("network_routing_status")}")')
+    def routing_status_menu(self) -> Locator:
+        return self.page.locator(f'a:has-text("{self.__locale.get("routing_status")}")')
 
     @property
-    def network_routing_static_menu(self) -> Locator:
-        return self.page.locator(f'a:has-text("{self.__locale.get("network_routing_static")}")')
+    def routing_static_menu(self) -> Locator:
+        return self.page.locator(f'a:has-text("{self.__locale.get("routing_static")}")')
 
     @property
-    def network_firewall_menu(self) -> Locator:
-        return self.page.locator(f'div:text-is("{self.__locale.get("network_firewall")}")')
+    def firewall_menu(self) -> Locator:
+        return self.page.locator(f'div:text-is("{self.__locale.get("firewall")}")')
 
     @property
-    def network_firewall_acl_menu(self) -> Locator:
-        return self.page.locator(f'a:has-text("{self.__locale.get("network_firewall_acl")}")')
+    def acl_menu(self) -> Locator:
+        return self.page.locator(f'a:has-text("{self.__locale.get("acl")}")')
 
     @property
-    def network_firewall_nat_menu(self) -> Locator:
-        return self.page.locator(f'a:has-text("{self.__locale.get("network_firewall_nat")}")')
+    def nat_menu(self) -> Locator:
+        return self.page.locator(f'a:has-text("{self.__locale.get("nat")}")')
 
     @property
-    def network_vpn_menu(self) -> Locator:
+    def vpn_menu(self) -> Locator:
         return self.page.locator('div:text-is("VPN")')
 
     @property
-    def network_vpn_l2tp_menu(self) -> Locator:
+    def l2tp_menu(self) -> Locator:
         return self.page.locator('a:has-text("L2TP")')
 
     @property
     def python_edge_menu(self) -> Locator:
         return self.page.locator(f'a:has-text("{self.__locale.get("python_edge")}")')
 
     @property
@@ -238,19 +198,19 @@
         return self.page.locator(f'a:has-text("{self.__locale.get("docker_manager")}")')
 
     @property
     def cloud_edge_computing_menu(self) -> Locator:
         return self.page.locator(f'a:has-text("{self.__locale.get("cloud_edge_computing")}")')
 
     @property
-    def cloud_edge_computing_azure_iot_edge_menu(self) -> Locator:
+    def azure_iot_edge_menu(self) -> Locator:
         return self.page.locator('div:text-is("Azure IoT Edge")')
 
     @property
-    def cloud_edge_computing_aws_iot_greengrass_menu(self) -> Locator:
+    def aws_iot_greengrass_menu(self) -> Locator:
         return self.page.locator('div:text-is("AWS IoT Greengrass")')
 
     @property
     def device_supervisor_menu(self) -> Locator:
         return self.page.locator(f'div:text-is("{self.__locale.get("device_supervisor")}")')
 
     @property
@@ -324,237 +284,288 @@
         return self.page.locator(f'a:has-text("{self.__locale.get("system_3rd_party")}")')
 
     @property
     def tags_menu(self) -> dict:
         return {
             'overview': {
                 'menu': self.overview_menu,
-                'visible_locator': [self.content_span_text('overview')],
+                'visible_locator': [self.page.locator(f'//div[text()="{self.__locale.get("performance")}"]')],
             },
             'network': {
-                'default': 'network_interface',
+                'default': 'network_interface.cellular',
                 'menu': self.network_menu,
-                'visible_locator': [self.network_interface_menu],
-                'wait_locator': [self.network_interface_menu],
-                # Network Interface
+                'visible_locator': [self.page.locator('//span[@class="ant-breadcrumb-link"]/a[@href="/network"]')],
+                'wait_locator': [self.content_target('cellular')],
                 'network_interface': {
+                    'default': 'cellular',
                     'menu': self.network_interface_menu,
-                    'visible_locator': [self.network_interface_cellular_menu],
-                    'wait_locator': [self.network_interface_cellular_menu],
+                    'visible_locator': [self.cellular_menu],
+                    'wait_locator': [self.cellular_menu],
                     'cellular': {
-                        'menu': self.network_interface_cellular_menu,
-                        'visible_locator': [self.content_span_text('cellular')],
-                        'wait_locator': [self.content_span_text('cellular')]},
+                        'menu': self.cellular_menu,
+                        'visible_locator': [self.content_target('cellular')],
+                        'wait_locator': [self.content_target('cellular')]},
                     'ethernet': {
-                        'default': 'gigabitethernet_01',
-                        'menu': self.network_interface_ethernet_menu,
-                        'visible_locator': [self.content_span_text('ethernet')],
-                        'wait_locator': [self.content_span_text('ethernet')],
-                        'gigabitethernet_01': {
+                        'default': 'gigabitethernet_0/1',
+                        'menu': self.ethernet_menu,
+                        'visible_locator': [self.content_target('ethernet')],
+                        'wait_locator': [self.content_target('ethernet')],
+                        'gigabitethernet_0/1': {
                             'menu': self.page.locator(f'div:text-is("{self.__locale.get("gigabitethernet")} 0/1")'),
+                            'attributes': {
+                                self.page.locator(f'div:text-is("{self.__locale.get("gigabitethernet")} 0/1")'): {
+                                    'aria-selected': 'true'}},
+                            'wait_locator': [self.page.locator('#internet')],
                         },
-                        'gigabitethernet_02': {
+                        'gigabitethernet_0/2': {
                             'menu': self.page.locator(f'div:text-is("{self.__locale.get("gigabitethernet")} 0/2")'),
+                            'attributes': {
+                                self.page.locator(f'div:text-is("{self.__locale.get("gigabitethernet")} 0/2")'): {
+                                    'aria-selected': 'true'}},
+                            'wait_locator': [
+                                self.page.locator('.antd-pro-components-description-list-index-term').first],
                         }
                     },
                     'bridge': {
-                        'menu': self.network_interface_bridge_menu,
-                        'visible_locator': [self.content_span_text('bridge')],
-                        'wait_locator': [self.content_span_text('bridge')]},
+                        'menu': self.bridge_menu,
+                        'visible_locator': [self.content_target('bridge')],
+                        'wait_locator': [self.content_target('bridge')]},
                     'wlan': {
-                        'menu': self.network_interface_wlan_menu,
-                        'visible_locator': [self.content_span_text('"wlan')],
-                        'wait_locator': [self.content_span_text('"wlan')]},
+                        'menu': self.wlan_menu,
+                        'visible_locator': [self.content_target('WLAN')],
+                        'wait_locator': [self.content_target('WLAN')]},
+                    'wan': {
+                        'menu': self.wan_menu_502,
+                        'visible_locator': [self.content_target('WAN')],
+                        'wait_locator': [self.content_target('WAN')]},
+                    'lan': {
+                        'menu': self.lan_menu_502,
+                        'visible_locator': [self.content_target('LAN')],
+                        'wait_locator': [self.content_target('LAN')]},
                     'loopback': {
-                        'menu': self.network_interface_loopback_menu,
-                        'visible_locator': [self.content_span_text('loopback')],
-                        'wait_locator': [self.content_span_text('loopback')]}},
+                        'menu': self.loopback_menu,
+                        'visible_locator': [self.content_target('loopback')],
+                        'wait_locator': [self.content_target('loopback')]}},
                 # Network Services
                 'network_services': {
                     'menu': self.network_service_menu,
-                    'visible_locator': [self.network_service_dhcp_menu],
-                    'wait_locator': [self.network_service_dhcp_menu],
+                    'visible_locator': [self.dhcp_menu],
+                    'wait_locator': [self.dhcp_menu],
                     'dhcp': {
-                        'menu': self.network_service_dhcp_menu,
-                        'visible_locator': [self.content_span_text('dhcp')],
-                        'wait_locator': [self.content_span_text('dhcp')]},
+                        'menu': self.dhcp_menu,
+                        'visible_locator': [self.content_target('dhcp')],
+                        'wait_locator': [self.content_target('dhcp')]},
                     'dns': {
-                        'menu': self.network_service_dns_menu,
-                        'visible_locator': [self.content_span_text('dns')],
-                        'wait_locator': [self.content_span_text('dns')]},
+                        'menu': self.dns_menu,
+                        'visible_locator': [self.content_target('dns')],
+                        'wait_locator': [self.content_target('dns')]},
                     'gps': {
                         'default': 'gps_configure',
-                        'menu': self.network_service_gps_menu,
-                        'visible_locator': [self.content_span_text('gps')],
-                        'wait_locator': [self.content_span_text('gps')],
+                        'menu': self.gps_menu,
+                        'visible_locator': [self.content_target('gps')],
+                        'wait_locator': [self.content_target('gps')],
                         'gps_configure': {
                             'menu': self.page.locator(f'div:text-is("{self.__locale.get("gps_configure")}")'),
-                            'visible_locator': [self.page.locator('.ant-form-item-no-colon')],
+                            'attributes': {self.page.locator(f'div:text-is("{self.__locale.get("gps_configure")}")'): {
+                                'aria-selected': 'true'}},
                             'wait_locator': [self.page.locator('.ant-form-item-no-colon')],
                         },
                         'gps_ip_forwarding': {
                             'menu': self.page.locator(f'div:text-is("{self.__locale.get("gps_ip_forwarding")}")'),
-                            'visible_locator': [self.page.locator('#enable')],
+                            'attributes': {
+                                self.page.locator(f'div:text-is("{self.__locale.get("gps_ip_forwarding")}")'): {
+                                    'aria-selected': 'true'}},
                             'wait_locator': [self.page.locator('#enable')],
                         },
                         'gps_serial_forwarding': {
                             'menu': self.page.locator(f'div:text-is("{self.__locale.get("gps_serial_forwarding")}")'),
-                            'visible_locator': [self.page.locator('#enable')],
+                            'attributes': {
+                                self.page.locator(f'div:text-is("{self.__locale.get("gps_serial_forwarding")}")'): {
+                                    'aria-selected': 'true'}},
                             'wait_locator': [self.page.locator('#enable')],
                         },
                     },
                     'host_list': {
-                        'menu': self.network_service_host_menu,
-                        'visible_locator': [self.content_span_text('host_list')],
-                        'wait_locator': [self.content_span_text('host_list')]}},
+                        'menu': self.host_list_menu,
+                        'visible_locator': [self.content_target('host_list')],
+                        'wait_locator': [self.content_target('host_list')]}},
                 # Routing
                 'routing': {
-                    'menu': self.network_routing_menu,
-                    'visible_locator': [self.network_routing_status_menu],
-                    'wait_locator': [self.network_routing_status_menu],
+                    'menu': self.routing_menu,
+                    'visible_locator': [self.routing_status_menu],
+                    'wait_locator': [self.routing_status_menu],
                     'routing_status': {
-                        'menu': self.network_routing_status_menu,
-                        'visible_locator': [self.content_span_text('routing_status')],
-                        'wait_locator': [self.content_span_text('routing_status')]},
+                        'menu': self.routing_status_menu,
+                        'visible_locator': [self.content_target('routing_status')],
+                        'wait_locator': [self.content_target('routing_status')]},
                     'static_routing': {
-                        'menu': self.network_routing_static_menu,
-                        'visible_locator': [self.content_span_text('static_routing')],
-                        'wait_locator': [self.content_span_text('static_routing')]}},
+                        'menu': self.routing_static_menu,
+                        'visible_locator': [self.content_target('routing_static')],
+                        'wait_locator': [self.content_target('routing_static')]}},
                 # Firewall
                 'firewall': {
-                    'menu': self.network_firewall_menu,
-                    'visible_locator': [self.network_firewall_acl_menu],
-                    'wait_locator': [self.network_firewall_acl_menu],
+                    'menu': self.firewall_menu,
+                    'visible_locator': [self.acl_menu],
+                    'wait_locator': [self.acl_menu],
                     'acl': {
-                        'menu': self.network_firewall_acl_menu,
-                        'visible_locator': [self.content_span_text('acl')],
-                        'wait_locator': [self.content_span_text('acl')]},
+                        'menu': self.acl_menu,
+                        'visible_locator': [self.content_target('acl')],
+                        'wait_locator': [self.content_target('acl')]},
                     'nat': {
-                        'menu': self.network_firewall_nat_menu,
-                        'visible_locator': [self.content_span_text('nat')],
-                        'wait_locator': [self.content_span_text('nat')]}},
+                        'menu': self.nat_menu,
+                        'visible_locator': [self.content_target('nat')],
+                        'wait_locator': [self.content_target('nat')]}},
                 # VPN
                 'vpn': {
-                    'menu': self.network_vpn_menu,
-                    'visible_locator': [self.network_vpn_l2tp_menu],
-                    'wait_locator': [self.network_vpn_l2tp_menu],
+                    'menu': self.vpn_menu,
+                    'visible_locator': [self.l2tp_menu],
+                    'wait_locator': [self.l2tp_menu],
                     'l2tp': {
                         'default': 'status',
-                        'menu': self.network_vpn_l2tp_menu,
+                        'menu': self.l2tp_menu,
                         'status': {
-                            'menu': self.page.locator(f'div:text-is("{self.__locale.get("l2tp_status")}")'),
-                            'visible_locator': [self.content_span_text('l2tp_status')],
-                            'wait_locator': [self.content_span_text('l2tp_status')]
+                            'menu': self.page.locator(f'div:text-is("{self.__locale.get("status")}")'),
+                            'attributes': {self.page.locator(f'div:text-is("{self.__locale.get("status")}")'): {
+                                'aria-selected': 'true'}},
+                            'wait_locator': [self.page.locator('.ant-spin-container').first],
                         },
                         'l2tp_client': {
                             'menu': self.page.locator(f'div:text-is("{self.__locale.get("l2tp_client")}")'),
-                            'visible_locator': [self.content_span_text('l2tp_client')],
-                            'wait_locator': [self.content_span_text('l2tp_client')]
+                            'attributes': {self.page.locator(f'div:text-is("{self.__locale.get("l2tp_client")}")'): {
+                                'aria-selected': 'true'}},
+                            'wait_locator': [self.page.locator('.ant-spin-container').first]
                         },
                         'l2tp_service': {
                             'menu': self.page.locator(f'div:text-is("{self.__locale.get("l2tp_service")}")'),
-                            'visible_locator': [self.content_span_text('l2tp_service')],
-                            'wait_locator': [self.content_span_text('l2tp_service')]}
+                            'attributes': {self.page.locator(f'div:text-is("{self.__locale.get("l2tp_service")}")'): {
+                                'aria-selected': 'true'}},
+                            'wait_locator': [self.page.locator('.ant-spin-container').first]}
                     }
                 }
             },
             'edge_computing': {
                 'default': 'python_edge_computing',
                 'menu': self.edge_menu,
-                'visible_locator': [self.device_supervisor_menu],
-                'wait_locator': [self.device_supervisor_menu],
+                'visible_locator': [
+                    self.page.locator('//span[@class="ant-breadcrumb-link"]/a[@href="/edge-computing"]').last],
+                'wait_locator': [self.content_target('python_edge').nth(1)],
                 'python_edge_computing': {
                     'menu': self.python_edge_menu,
-                    'visible_locator': [self.content_span_text('python_edge_computing')],
-                    'wait_locator': [self.content_span_text('python_edge_computing')]
+                    'visible_locator': [self.content_target('python_edge').nth(1)],
+                    'wait_locator': [self.content_target('python_edge').nth(1)]
                 },
                 'docker_manager': {
                     'menu': self.docker_manager_menu,
-                    'visible_locator': [self.content_span_text('docker_manager')],
-                    'wait_locator': [self.content_span_text('docker_manager')]
+                    'visible_locator': [self.content_target('docker_manager').nth(1)],
+                    'wait_locator': [self.content_target('docker_manager').nth(1)]
                 },
                 'cloud_edge_computing': {
                     'default': 'azure_iot_edge',
                     'menu': self.cloud_edge_computing_menu,
-                    'visible_locator': [self.content_span_text('cloud_edge_computing')],
-                    'wait_locator': [self.content_span_text('cloud_edge_computing')],
+                    'visible_locator': [self.content_target('cloud_edge_computing').nth(1)],
+                    'wait_locator': [self.content_target('cloud_edge_computing').nth(1)],
                     'azure_iot_edge': {
-                        'menu': self.cloud_edge_computing_azure_iot_edge_menu,
-                        'visible_locator': [self.content_span_text('azure_iot_edge')],
-                        'wait_locator': [self.content_span_text('azure_iot_edge')],
+                        'menu': self.azure_iot_edge_menu,
+                        'attributes': {self.azure_iot_edge_menu: {'aria-selected': 'true'}},
+                        'wait_locator': [self.page.locator('//button[@id="enable"]').first],
                     },
                     'aws_iot_greengrass': {
-                        'menu': self.cloud_edge_computing_aws_iot_greengrass_menu,
-                        'visible_locator': [self.content_span_text('aws_iot_greengrass')],
-                        'wait_locator': [self.content_span_text('aws_iot_greengrass')],
+                        'menu': self.aws_iot_greengrass_menu,
+                        'attributes': {
+                            self.aws_iot_greengrass_menu: {'aria-selected': 'true'}},
+                        'wait_locator': [self.page.locator('//button[@id="enable"]').first],
                     }
                 },
                 # Device Supervisor
                 'device_supervisor': {
+                    'default': 'measure_monitor.monitoring_list',
                     'menu': self.device_supervisor_menu,
                     'visible_locator': [self.measure_monitor_menu],
                     'wait_locator': [self.measure_monitor_menu],
                     'measure_monitor': {
                         'default': 'monitoring_list',
                         'menu': self.measure_monitor_menu,
+                        'visible_locator': [self.content_target('measure_monitor')],
                         'monitoring_list': {
-                            'menu': self.page.locator(f'div:text-is("{self.__locale.get("monitoring_list")}")')
+                            'menu': self.page.locator(f'div:text-is("{self.__locale.get("monitoring_list")}")'),
+                            'attributes': {
+                                self.page.locator(f'div:text-is("{self.__locale.get("monitoring_list")}")'): {
+                                    'aria-selected': 'true'}},
+                            'wait_locator': [self.page.locator('.ant-input-search-button').first],
                         },
                         'group': {
-                            'menu': self.page.locator(f'div:text-is("{self.__locale.get("group")}")')
+                            'menu': self.page.locator(f'div:text-is("{self.__locale.get("group")}")'),
+                            'attributes': {
+                                self.page.locator(f'div:text-is("{self.__locale.get("group")}")'): {
+                                    'aria-selected': 'true'}},
+                            'wait_locator': [self.page.locator('//i[@class="anticon anticon-plus-circle"]')],
                         },
                     },
                     'alarm': {
                         'default': 'realtime_alarms',
                         'menu': self.alarm_menu,
-                        'visible_locator': [self.content_span_text('alarm')],
-                        'wait_locator': [self.content_span_text('alarm')],
+                        'visible_locator': [self.content_target('alarm')],
+                        'wait_locator': [self.content_target('alarm')],
                         'realtime_alarms': {
                             'menu': self.page.locator(f'div:text-is("{self.__locale.get("realtime_alarms")}")'),
-                            'visible_locator': [self.page.locator('.ant-table-header.ant-table-hide-scrollbar')],
+                            'attributes': {
+                                self.page.locator(f'div:text-is("{self.__locale.get("realtime_alarms")}")'): {
+                                    'aria-selected': 'true'}},
                             'wait_locator': [self.page.locator('.ant-table-header.ant-table-hide-scrollbar')]
                         },
                         'alarm_rules': {
                             'menu': self.page.locator(f'div:text-is("{self.__locale.get("alarm_rules")}")'),
-                            'visible_locator': [
-                                self.page.locator(f'span:text-is("{self.__locale.get("trigger_condition")}")')],
+                            'attributes': {
+                                self.page.locator(f'div:text-is("{self.__locale.get("alarm_rules")}")'): {
+                                    'aria-selected': 'true'}},
                             'wait_locator': [
                                 self.page.locator(f'span:text-is("{self.__locale.get("trigger_condition")}")')]
                         },
                         'history_alarms': {
                             'menu': self.page.locator(f'div:text-is("{self.__locale.get("history_alarms")}")'),
-                            'visible_locator': [self.page.locator('span:text-is("~")')],
+                            'attributes': {
+                                self.page.locator(f'div:text-is("{self.__locale.get("history_alarms")}")'): {
+                                    'aria-selected': 'true'}},
                             'wait_locator': [self.page.locator('span:text-is("~")')]
                         },
                         'alarm_label': {
                             'menu': self.page.locator(f'div:text-is("{self.__locale.get("alarm_label")}")'),
-                            'visible_locator': [self.page.locator('.ant-table-selection-column >> nth=0')],
+                            'attributes': {
+                                self.page.locator(f'div:text-is("{self.__locale.get("alarm_label")}")'): {
+                                    'aria-selected': 'true'}},
                             'wait_locator': [self.page.locator('.ant-table-selection-column >> nth=0')]
                         },
                     },
                     'cloud': {
                         'default': 'mqtt_cloud_service',
                         'menu': self.cloud_menu,
-                        'visible_locator': [self.content_span_text('cloud')],
-                        'wait_locator': [self.content_span_text('cloud')],
+                        'visible_locator': [self.content_target('cloud')],
+                        'wait_locator': [self.content_target('cloud')],
                         'mqtt_cloud_service': {
                             'menu': self.page.locator(f'div:text-is("{self.__locale.get("mqtt_cloud_service")}")'),
-                            'visible_locator': [self.content_span_text('mqtt_cloud_service')],
-                            'wait_locator': [self.content_span_text('mqtt_cloud_service')]
+                            'attributes': {
+                                self.page.locator(f'div:text-is("{self.__locale.get("mqtt_cloud_service")}")'): {
+                                    'aria-selected': 'true'}},
+                            'wait_locator': [self.page.locator('//label[@for="enable.form"]')]
                         },
                         'whitehawk_energy_manager': {
                             'menu': self.page.locator(
                                 f'div:text-is("{self.__locale.get("whitehawk_energy_manager")}")'),
-                            'visible_locator': [self.content_span_text('whitehawk_energy_manager')],
-                            'wait_locator': [self.content_span_text('whitehawk_energy_manager')]
+                            'attributes': {
+                                self.page.locator(
+                                    f'div:text-is("{self.__locale.get("whitehawk_energy_manager")}")'): {
+                                    'aria-selected': 'true'}},
+                            'wait_locator': [self.page.locator('//label[@for="enable.form"]')]
                         }
                     },
                     'protocol': {
                         'default': 'modbus_tcp_slave',
                         'menu': self.protocol_menu,
+                        'visible_locator': [self.content_target('protocol')],
+                        'wait_locator': [self.content_target('protocol')],
                         'modbus_tcp_slave': {
                             'menu': self.page.locator(f'div:text-is("Modbus TCP Slave")'),
                             'visible_locator': [
                                 self.page.locator(f'text=Modbus TCP Slave{self.__locale.get("configuration")}')],
                             'wait_locator': [
                                 self.page.locator(f'text=Modbus TCP Slave{self.__locale.get("configuration")}')],
                         },
@@ -578,90 +589,105 @@
                                 self.page.locator(f'text=Modbus RTU Slave{self.__locale.get("configuration")}')],
                             'wait_locator': [
                                 self.page.locator(f'text=Modbus RTU Slave{self.__locale.get("configuration")}')],
                         },
                     },
                     'parameter_settings': {
                         'menu': self.parameter_settings_menu,
-                        'visible_locator': [self.content_span_text('parameter_settings')],
-                        'wait_locator': [self.content_span_text('parameter_settings')]
+                        'visible_locator': [self.content_target('parameter_settings')],
+                        'wait_locator': [self.content_target('parameter_settings')]
                     },
                     'custom_quickfunctions': {
                         'menu': self.custom_quickfunctions_menu,
-                        'visible_locator': [self.content_span_text('custom_quickfunctions')],
-                        'wait_locator': [self.content_span_text('custom_quickfunctions')]}
+                        'visible_locator': [self.content_target('custom_quickfunctions')],
+                        'wait_locator': [self.content_target('custom_quickfunctions')]}
                 }
             },
             'system': {
                 'default': 'system_time',
                 'menu': self.system_menu,
+                'visible_locator': [self.page.locator('//span[@class="ant-breadcrumb-link"]/a[@href="/system"]')],
+                'wait_locator': [self.content_target('system_time')],
                 'system_time': {
                     'menu': self.system_time_menu,
-                    'visible_locator': [self.content_span_text('system_time')],
-                    'wait_locator': [self.content_span_text('system_time')],
+                    'visible_locator': [self.content_target('system_time')],
+                    'wait_locator': [self.content_target('system_time')],
                 },
                 'log': {
                     'default': 'log',
                     'menu': self.system_log_menu,
+                    'visible_locator': [self.content_target('system_log')],
+                    'wait_locator': [self.content_target('system_log')],
                     'log': {
                         'menu': self.page.locator('.ant-tabs-tab >> nth=0'),
-                        'visible_locator': [self.content_span_text('log')],
-                        'wait_locator': [self.content_span_text('log')],
+                        'attributes': {
+                            self.page.locator('.ant-tabs-tab >> nth=0'): {'aria-selected': 'true'}},
+                        'wait_locator': [self.page.locator('//button[@class="ant-btn"]').first],
                     },
                     'configure': {
                         'menu': self.page.locator('.ant-tabs-tab >> nth=1'),
-                        'visible_locator': [self.content_span_text('log_configure')],
-                        'wait_locator': [self.content_span_text('log_configure')],
+                        'attributes': {
+                            self.page.locator('.ant-tabs-tab >> nth=1'): {'aria-selected': 'true'}},
+                        'wait_locator': [self.page.locator('#log_to_remote_enable')],
                     }
                 },
                 'configuration_management': {
                     'menu': self.system_config_menu,
-                    'visible_locator': [self.content_span_text('configuration_management')],
-                    'wait_locator': [self.content_span_text('configuration_management')],
+                    'visible_locator': [self.content_target('system_config')],
+                    'wait_locator': [self.content_target('system_config')],
                 },
                 'inhand_cloud': {
                     'default': 'inhand_connect_service',
                     'menu': self.system_cloud_menu,
-                    'visible_locator': [self.content_span_text('inhand_cloud')],
-                    'wait_locator': [self.content_span_text('inhand_cloud')],
+                    'visible_locator': [self.content_target('system_cloud')],
+                    'wait_locator': [self.content_target('system_cloud')],
                     'inhand_connect_service': {
                         'menu': self.page.locator(f'div:text-is("InHand Connect Service")'),
+                        'attributes': {
+                            self.page.locator(f'div:text-is("InHand Connect Service")'): {'aria-selected': 'true'}},
+                        'wait_locator': [self.page.locator('//button[@id="enable"]')],
                     },
                     'inhand_device_manager': {
                         'menu': self.page.locator(f'div:text-is("InHand Device Manager")'),
+                        'attributes': {
+                            self.page.locator(f'div:text-is("InHand Device Manager")'): {'aria-selected': 'true'}},
+                        'wait_locator': [self.page.locator('//button[@id="enable"]')],
                     },
                     'inhand_iscada_cloud': {
                         'menu': self.page.locator(f'div:text-is("InHand iSCADA Cloud")'),
+                        'attributes': {
+                            self.page.locator(f'div:text-is("InHand iSCADA Cloud")'): {'aria-selected': 'true'}},
+                        'wait_locator': [self.page.locator('//button[@id="mode"]')],
                     }
                 },
                 'firmware_upgrade': {
                     'menu': self.system_firmware_menu,
-                    'visible_locator': [self.content_span_text('firmware_upgrade')],
-                    'wait_locator': [self.content_span_text('firmware_upgrade')],
+                    'visible_locator': [self.content_target('system_firmware')],
+                    'wait_locator': [self.content_target('system_firmware')],
                 },
                 'access_tools': {
                     'menu': self.system_tools_menu,
-                    'visible_locator': [self.content_span_text('access_tools')],
-                    'wait_locator': [self.content_span_text('access_tools')],
+                    'visible_locator': [self.content_target('system_tools')],
+                    'wait_locator': [self.content_target('system_tools')],
                 },
                 'user_management': {
                     'menu': self.system_user_management_menu,
-                    'visible_locator': [self.content_span_text('user_management')],
-                    'wait_locator': [self.content_span_text('user_management')],
+                    'visible_locator': [self.content_target('system_user_management')],
+                    'wait_locator': [self.content_target('system_user_management')],
                 },
                 'reboot': {
                     'menu': self.system_reboot_menu,
-                    'visible_locator': [self.content_span_text('reboot')],
-                    'wait_locator': [self.content_span_text('reboot')],
+                    'visible_locator': [self.content_target('system_reboot')],
+                    'wait_locator': [self.content_target('system_reboot')],
                 },
                 'network_tools': {
                     'menu': self.system_network_tools_menu,
-                    'visible_locator': [self.content_span_text('network_tools')],
-                    'wait_locator': [self.content_span_text('network_tools')],
+                    'visible_locator': [self.content_target('system_network_tools')],
+                    'wait_locator': [self.content_target('system_network_tools')],
                 },
                 '3rd_party_notification': {
                     'menu': self.system_3rd_party_menu,
-                    'visible_locator': [self.content_span_text('3rd_party_notification')],
-                    'wait_locator': [self.content_span_text('3rd_party_notification')],
+                    'attributes': {self.system_3rd_party_menu.locator('..'): {'class': 'ant-menu-item-selected'}},
+                    'wait_locator': [self.content_target('system_3rd_party')],
                 }
             },
         }
```

### Comparing `inhandtest-0.0.44/inhandtest/base_page/_ir3XX_contents_locators.py` & `inhandtest-0.0.45/inhandtest/base_page/_ir3XX_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.44/inhandtest/base_page/_vg710_contents_locators.py` & `inhandtest-0.0.45/inhandtest/base_page/_vg710_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.44/inhandtest/base_page/base_page.py` & `inhandtest-0.0.45/inhandtest/base_page/base_page.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 base_page
 
 """
 import os.path
 import sys
 from os import path
-from inhandtest.base_page._ig902_contents_locators import IGContentsLocators
+from inhandtest.base_page._ig_contents_locators import IGContentsLocators
 from typing import List
 from inhandtest.exception import ModelError
 from inhandtest.tools import loop_inspector
 from playwright.sync_api import Page, Locator, expect, TimeoutError, sync_playwright
 from inhandtest.base_page._vg710_contents_locators import VGContentsLocators
 from inhandtest.base_page._ir3XX_contents_locators import Ir3XXContentsLocators
 from inhandtest.base_page.table_tr import Table
@@ -21,15 +21,15 @@
 import logging
 import re
 
 
 class BasePage:
 
     def __init__(self, host: str, username: str, password: str, protocol='https',
-                 port=443, model='VG710', language='en',  page: Page = None, **kwargs):
+                 port=443, model='VG710', language='en', page: Page = None, **kwargs):
         """
 
         :param host:  设备主机地址
         :param username: 用户名
         :param password: 密码
         :param protocol: 协议
         :param port: 端口
@@ -45,19 +45,19 @@
         self.protocol = protocol
         self.port = port
         self.__username = username
         self.__password = password
         self.language = language
         self.__browser_type = kwargs.get('browser')
         self.__http_credentials_model = ('VG710',)  # 需要使用http认证的设备, 没有登录页面 只有登录弹窗
-        if self.__browser_type is None:
+        if self.page is None:
             self.__new_page()
         if self.model == 'VG710':
             self.content_locator = VGContentsLocators(self.page, language).tags_menu
-        elif self.model == 'IG902':
+        elif self.model in ('IG902', 'IG502'):
             self.content_locator = IGContentsLocators(self.page, language).tags_menu
         elif self.model in ('IR302', 'IR305', 'IR615'):
             self.content_locator = Ir3XXContentsLocators(self.page, language).tags_menu
         else:
             raise ModelError(f'not support this mode {model}')
         self.locale = kwargs.get('locale').get(language) if kwargs.get('locale') else None
 
@@ -192,56 +192,88 @@
 
         :param menu: 'system'| 'system.status' 菜单名称全部来自与设备的英文版本，点号需要省略不写， 其他不变，大小写均可以
                      菜单中原有的点号都需要忽略，如wi-fi 2.4g 需要传入wi-fi_24g 或 wi-fi 2.4g 或 wi-fi_2.4g
         :param wait_time: 当操作完菜单后是否需要等待时间 单位毫秒
         :return:
         """
 
-        def access(menu_one: str, locators: dict, level: int):
-            visible = False
-            if locators.get(menu_one).get('visible_locator'):
-                visible = True
-                for visible_locator in locators.get(menu_one).get('visible_locator'):
+        def in_current_menu(locators: dict) -> bool:
+            _in_current_menu = False
+            if locators.get('visible_locator'):
+                _in_current_menu = True
+                for visible_locator in locators.get('visible_locator'):
                     if not visible_locator.is_visible():
-                        visible = False
+                        _in_current_menu = False
                         break
-                else:
-                    self.page.wait_for_timeout(500)  # 当元素可见时也再多等待500ms
-            if not visible:
-                menus = locators.get(menu_one).get('menu') if isinstance(locators.get(menu_one).get('menu'),
-                                                                         list) else [locators.get(menu_one).get('menu')]
+            if locators.get('attributes'):
+                for locator, value in locators.get('attributes').items():
+                    if locator.is_visible():
+                        for attr, expect_value in value.items():
+                            if expect_value not in locator.get_attribute(attr):
+                                _in_current_menu = False
+                                break
+                        else:
+                            _in_current_menu = True
+                            continue
+                        break
+                    else:
+                        _in_current_menu = False
+                        break
+            return _in_current_menu
+
+        def access_one_menu(menu_one: str, locators: dict, level: int):  # 进入某一个菜单
+            if not in_current_menu(locators):
+                menus = locators.get('menu') if isinstance(locators.get('menu'), list) else [locators.get('menu')]
                 for menu_1 in menus:
                     self.click(menu_1)
                 logging.info(f'select {level} level menu {menu_one}')
-                if locators.get(menu_one).get('mouse_move'):
-                    self.page.mouse.move(locators.get(menu_one).get('mouse_move')[0],
-                                         locators.get(menu_one).get('mouse_move')[1])
-                if locators.get(menu_one).get('wait_locator'):
-                    for wait_locator in locators.get(menu_one).get('wait_locator'):
+                if locators.get('mouse_move'):
+                    self.page.mouse.move(locators.get('mouse_move')[0], locators.get('mouse_move')[1])
+                if locators.get('wait_locator'):
+                    for wait_locator in locators.get('wait_locator'):
                         wait_locator.wait_for(state='visible')
                     self.page.wait_for_timeout(500)  # 多等500ms
 
+        def access(menus):  # 递归进入菜单
+            new_menus = []
+            click_menus = []
+            menu_content = self.content_locator
+            # 把菜单名、菜单的元素信息、以及菜单等级依次放入列表中
+            for menu_s, level_ in zip(menus, range(1, len(menus) + 1)):
+                menu_content = menu_content.get(menu_s)
+                new_menus.append([menu_s, menu_content, level_])
+            new_menus.reverse()  # 逆序查看是否在当前这个菜单的页面
+            for menu_one, locators, level_ in new_menus:
+                if not in_current_menu(locators):
+                    # 找出需要点击的菜单
+                    click_menus.append((menu_one, locators, level_))
+                else:
+                    break
+            if click_menus:
+                click_menus.reverse()  # 回归原来的顺序
+                for menu_one, locators, level_ in click_menus:
+                    access_one_menu(menu_one, locators, level_)
+            else:
+                logging.info(f'already in {".".join(menu)} menu')
+
         def default_change(menu_old, locators: dict) -> str:
             menu_old_s = menu_old.split('.')
             for menu_old_ in menu_old_s:
                 locators = locators.get(menu_old_)
             default = locators.get('default')
             menu_new = menu_old + '.' + default if default else menu_old
             return menu_new
 
         if menu:
             self.page.bring_to_front()
             self.login()
             try:
                 menu = menu.replace(' ', '_').replace('-', '_').lower()
                 menu = default_change(menu, self.content_locator).split('.')
-                content_locator_ = self.content_locator
-                for menu_, level in zip(menu, range(1, len(menu)+1)):
-                    access(menu_, content_locator_, level)
-                    content_locator_ = content_locator_.get(menu_)
+                access(menu)
             except Exception:
                 raise f'not support this menu {menu}'
             if wait_time:
                 self.page.wait_for_timeout(wait_time)
 
     @allure.step('{log_desc} 输入{value}')
     def fill(self, locator: Locator, value: str or int, log_desc=None, force=False) -> None:
@@ -732,20 +764,23 @@
         """
         if expect_:
             for key in expect_.keys():
                 filter_key = list(filter(lambda x: x[0] == key, locators))
                 if len(filter_key) == 1:
                     option = filter_key[0]
                     locator = option[1].get('locator')
-                    value = '"' + locator.first.inner_text() + '"' if locator.count() != 0 else None
+                    if isinstance(locator, Locator):
+                        value = locator.first.inner_text() if locator.count() != 0 else 'None'
+                    else:
+                        value = str(locator)
                     try:
                         expression = expect_.get(key).replace('${value}', value)
                         if option[1].get('param'):
                             for replace_k, replace_v in option[1].get('param').items():
-                                expression.replace(replace_k, replace_v)
+                                expression = expression.replace(replace_k, replace_v)
                         if eval(expression):
                             logging.info(f'Check {option[0]} , {expression} is true')
                         else:
                             logging.info(f'Check {option[0]} , {expression} is false')
                             return False
                     except TypeError:
                         logging.info(f'get inner_text failed')
@@ -844,28 +879,45 @@
             self.__browser.close()
             self.__playwright.stop()
 
 
 if __name__ == '__main__':
     logging.basicConfig(format='%(asctime)s %(levelname)s %(message)s', level=logging.INFO,
                         stream=sys.stdout)
-    with BasePage('10.5.47.197', 'adm', '123456', 'https', 443, model='vg710') as my_page:
-        system = ('link speed test', )
-        my_page.access_menu(f'wizards.new port mapping')
-        my_page.page.wait_for_timeout(2 * 1000)
+    with BasePage('10.5.24.96', 'adm', '123456', 'https', 443, model='ig902') as my_page:
+        # system = (
+        #     '3rd party notification', '3rd party notification', 'cloud edge computing.azure iot edge',
+        #     'cloud edge computing.aws iot greengrass',
+        #     'device supervisor',
+        #     'device supervisor.measure monitor.group', 'device supervisor.alarm', 'device supervisor.alarm.alarm rules',
+        #     'device supervisor.alarm.history alarms', 'device supervisor.alarm.alarm label', 'device supervisor.cloud',
+        #     'device supervisor.cloud.whitehawk energy manager',
+        #     'device supervisor.protocol', 'device supervisor.protocol.iec 104 server',
+        #     'device supervisor.protocol.opcua server',
+        #     'device supervisor.protocol.modbus rtu slave', 'device supervisor.parameter settings',
+        #     'device supervisor.custom quickfunctions',
+        #     'device supervisor.cloud.whitehawk energy manager',
+        #     'device supervisor.protocol.iec 104 server',)
+        for i in range(0, 1):
+            my_page.access_menu(f'system.inhand_cloud.inhand connect service')
+            my_page.page.wait_for_timeout(2 * 1000)
+            my_page.access_menu(f'system.inhand_cloud.inhand device manager')
+            my_page.access_menu(f'system.inhand_cloud.inhand device manager')
+            my_page.access_menu(f'system.inhand_cloud.inhand iscada cloud')
+            my_page.access_menu(f'system.inhand_cloud.inhand iscada cloud')
         # a = my_page.get_text('language', [('language', {'locator': my_page.page.frame_locator('#window_content').locator('#_f_hostname'), 'type': 'fill'})])
         # print(a)
     # with BasePage('10.5.24.96', 'adm', '123456', model='IG902') as my_page:
     #     my_page.access_menu('edge_computing.device_supervisor.measure_monitor')
     #     my_page.page.wait_for_timeout(1000)
     #     my_page.access_menu('edge_computing.device_supervisor.protocol')
     #     my_page.page.wait_for_timeout(1000)
-        # user_table = Table(
-        #     [('mode', 'input'), ('status', 'input'), ('ssid', 'input'),  ('mac', 'input'),
-        #      ('auth', 'input'), ('encry', 'input'), ('network', 'input'), ('gateway', 'input'), ('dns', 'input'), ('time', 'input')],
-        #     my_base.page.frame_locator('#window_content').locator('#wifi-2g-grid'),
-        #     ['mode', 'status', 'ssid', 'mac', 'auth', 'encry', 'network', 'gateway', 'dns', 'time'], None)
-        # a = user_table.exists([{'mode': "'${value}'!='AP'", 'ssid': 'inhand-visitor-2g'}])
-        # print(a)
-        # print(user_table.exist(locale={'disable': 'Disabled'}, mode="'${value}'!='AP'", ssid='inhand-visitor-2g', status='disable'))
-        # user_table.delete(name='test2', value='222')
-        # my_base.page.wait_for_timeout(5 * 1000)
+    # user_table = Table(
+    #     [('mode', 'input'), ('status', 'input'), ('ssid', 'input'),  ('mac', 'input'),
+    #      ('auth', 'input'), ('encry', 'input'), ('network', 'input'), ('gateway', 'input'), ('dns', 'input'), ('time', 'input')],
+    #     my_base.page.frame_locator('#window_content').locator('#wifi-2g-grid'),
+    #     ['mode', 'status', 'ssid', 'mac', 'auth', 'encry', 'network', 'gateway', 'dns', 'time'], None)
+    # a = user_table.exists([{'mode': "'${value}'!='AP'", 'ssid': 'inhand-visitor-2g'}])
+    # print(a)
+    # print(user_table.exist(locale={'disable': 'Disabled'}, mode="'${value}'!='AP'", ssid='inhand-visitor-2g', status='disable'))
+    # user_table.delete(name='test2', value='222')
+    # my_base.page.wait_for_timeout(5 * 1000)
```

### Comparing `inhandtest-0.0.44/inhandtest/base_page/table_tr.py` & `inhandtest-0.0.45/inhandtest/base_page/table_tr.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.44/inhandtest/exception.py` & `inhandtest-0.0.45/inhandtest/exception.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.44/inhandtest/file.py` & `inhandtest-0.0.45/inhandtest/file.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.44/inhandtest/inmodbus.py` & `inhandtest-0.0.45/inhandtest/inmodbus.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.44/inhandtest/inmongodb.py` & `inhandtest-0.0.45/inhandtest/inmongodb.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.44/inhandtest/inmqtt.py` & `inhandtest-0.0.45/inhandtest/inmqtt.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.44/inhandtest/inrequest.py` & `inhandtest-0.0.45/inhandtest/inrequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
             raise TimeOutError(f'{self.host} {self.username} account not found device {sn}')
 
     def device_state(self, sn: list) -> List[dict]:
         """根据sn 转换属性 属性值有：  online: 在线|离线   1|0
                                        iccid:
                                        imei:
                                        imsi:
+                                       model: 设备型号
                                        version: 固件版本
                                        hwVersion: 硬件版本 'V1.0'
                                        bootVersion:  Bootloader版本  '1.1.3.r4956'
                                        sn: 序列号
                                        address
                                        id: 设备id
                                        name: 设备名字
@@ -82,20 +83,20 @@
                 config_sync = res.get('config').get('sync') if res.get('config') else None
                 result.append(
                     {'sn': sn_, 'online': res.get('online'), 'iccid': res.get('info').get('iccid'),
                      'imei': res.get('info').get('imei'), 'imsi': res.get('info').get('imsi'),
                      'version': res.get('info').get('swVersion'), 'hwVersion': res.get('info').get('hwVersion'),
                      'bootVersion': res.get('info').get('bootVersion'), 'address': res.get('address'),
                      'id': res.get('_id'), 'name': res.get('name'), 'ip': res.get('pubIp'),
-                     'protocol': res.get('protocol'), 'config_sync': config_sync})
+                     'protocol': res.get('protocol'), 'config_sync': config_sync, 'model': res.get('model')})
             else:
                 result.append(
                     {'sn': sn_, 'online': None, 'iccid': None, 'imei': None, 'imsi': None, 'version': None,
                      'hwVersion': None, 'bootVersion': None, 'address': None, 'id': None, 'name': None, 'ip': None,
-                     'protocol': None, 'config_sync': None})
+                     'protocol': None, 'config_sync': None, 'model': None})
         return result
 
     def add_device(self, sn: str) -> None:
         """添加设备，
 
         :param sn: 设备序列号
         :return:
@@ -114,22 +115,24 @@
     def assert_device_state(self, sn: str, state: dict, timeout=120, interval=5) -> None:
         """校验设备基本状态
 
         :param sn: 序列号
         :param state:   支持表达式${value} ex: {'version': "'${value}' in 'V1.1.3.r4956'"}
                         online: 在线|离线   1|0
                         connected: true 只有ics 有该参数
+                        model: 设备型号
                         iccid:
                         imei:
                         imsi:
                         version: 固件版本
                         hwVersion: 硬件版本 'V1.0'
                         bootVersion:  Bootloader版本  '1.1.3.r4956'
                         sn: 序列号
                         address
+                        vip:  只能在ics里面使用
                         ip: 设备连接平台的ip地址
                         protocol: 设备连接平台的协议 ex: 'mqtt' or 'ovdp'
                         config_sync: 设备配置同步状态 ex: 2  同成功
         :param timeout: 校验信息，最大超时时间
         :param interval: 校验信息，校验间隔时间
         :return: True or False
         """
@@ -193,19 +196,26 @@
         """
         response = self.api.send_request('api/devices', method='get',
                                          param={"verbose": 100, "limit": 10, "cursor": 0,
                                                 'serial_number': sn})
         if response.json().get('total') == 1 and response.json().get('result')[0].get('online') == 1:
             device_id = response.json().get('result')[0].get('_id')
             device_name = response.json().get('result')[0].get('name')
-            task_state = self.api.send_request('api2/tasks/run', 'post',
-                                               body={'name': "GET RUNNING CONFIG", 'objectId': device_id,
-                                                     'priority': 30, 'objectName': device_name, 'timeout': 30000,
-                                                     'type': "4"}).json().get('result').get('state')
-            assert task_state == 3, "GET RUNNING CONFIG task status error!"
+            for i in range(0, 3):
+                try:
+                    task_state = self.api.send_request('api2/tasks/run', 'post',
+                                                       body={'name': "GET RUNNING CONFIG", 'objectId': device_id,
+                                                             'priority': 30, 'objectName': device_name, 'timeout': 30000,
+                                                             'type': "4"}).json().get('result').get('state')
+                    assert task_state == 3, "GET RUNNING CONFIG task status error!"
+                    break
+                except Exception as e:
+                    logging.error(f'get running config task status reason is {e}, try {i+2} again')
+            else:
+                raise Exception(f'device {sn} get running config task status failed')
             config_content = self.api.send_request(f'api/devices/{device_id}/config', 'get').json().get('result').get(
                 'content')
             if config:
                 assert set(config.split('\n')).issubset(set(config_content.split('\n'))), f'config {config} not exist'
         else:
             raise ResourceNotFoundError(f'the {sn} device not exist or offline')
 
@@ -269,15 +279,15 @@
                                 break
                             elif job[0].get('state') == -1:
                                 raise UpgradeFailedError(f'upgrade to {file_name} failed!')
                     else:
                         raise UpgradeFailedError('create upgrade task failed!')
                 else:
                     raise TimeOutError('upgrade job check timeout')
-                self.assert_device_state(sn, state={'version': '"${value}" in ' + f'"{file_name}"'})
+                self.assert_device_state(sn, state={'version': '"${value}" in ' + f'"{file_name}"'}, timeout=300)
             else:
                 logging.info(f'{firmware} not is file or version of same ')
         else:
             raise Exception(f'the device {sn} is offline or not exist')
 
     def upgrade_firmware(self, sn: str or list, firmware: str) -> None:
         """ 升级固件，只管下发升级任务，不监督是否升级成功
@@ -325,15 +335,22 @@
 
     def web_remote_online(self, sn: str) -> str:
         """封装远程web访问方法
 
         :param sn: str, 设备序列号
         :return: 远程web管理链接
         """
-        server = 'ngrok.iot.inhand.com.cn:4443' if self.host == 'iot.inhand.com.cn' else 'iot.inhandnetworks.com:4443'
+        if self.host == 'iot.inhand.com.cn':
+            server = 'ngrok.iot.inhand.com.cn:4443'
+        elif self.host == 'iot.inhandnetworks.com':
+            server = 'iot.inhandnetworks.com:4443'
+        elif self.host == 'ics.inhandiot.com':
+            server = 'ics.inhandiot.com:4443'
+        else:
+            server = 'ngrok.ics.inhandnetworks.com:443'
         response = self.api.send_request('api/devices', method='get',
                                          param={"verbose": 100, "limit": 10, "cursor": 0,
                                                 'serial_number': sn})
         if response.json().get('total') == 1 and response.json().get('result')[0].get('online') == 1:
             device_id = response.json().get('result')[0].get('_id')
             device_name = response.json().get('result')[0].get('name')
             body = {"priority": 30, "timeout": 20000, "objectId": device_id, "objectName": device_name,
@@ -494,14 +511,15 @@
                                        imsi:
                                        version: 固件版本
                                        hwVersion: 硬件版本 'V1.0'
                                        bootVersion:  Bootloader版本  '1.1.3.r4956'
                                        sn: 序列号
                                        id: 设备id
                                        name: 设备名称
+                                       vip: 虚拟IP
                                        ip: 设备连接平台的ip地址
                                        protocol: 设备连接平台的协议
                                        config_sync: 设备配置同步状态
         :param sn: 列表
         :return: [{'sn': $sn, 'online': 1, 'iccid': '', 'imei'}]
         """
         result = []
@@ -515,22 +533,22 @@
                 res_info = self.api.send_request(f'api/devices/{res.get("id")}', method='get',
                                                  param={'verbose': 100}).json().get('result')
                 config_sync = res_info.get('config').get('sync') if res_info.get('config') else None
                 result.append(
                     {'sn': sn_, 'online': res.get('online'), 'iccid': res.get('metadata').get('iccid'),
                      'imei': res.get('metadata').get('imei'), 'imsi': res.get('metadata').get('imsi'),
                      'version': res.get('metadata').get('swVersion'), 'hwVersion': res.get('metadata').get('hwVersion'),
-                     'bootVersion': res.get('metadata').get('bootVersion'),
+                     'bootVersion': res.get('metadata').get('bootVersion'), 'vip': res.get('vip'),
                      'id': res.get('id'), 'connected': res.get('connected'), 'name': res.get('name'),
                      'ip': res_info.get('pubIp'), 'protocol': res_info.get('protocol'), 'config_sync': config_sync})
             else:
                 result.append(
                     {'sn': sn_, 'online': None, 'iccid': None, 'imei': None, 'imsi': None, 'version': None,
                      'hwVersion': None, 'bootVersion': None, 'id': None, 'connected': None, 'name': None, 'ip': None,
-                     'protocol': None, 'config_sync': None})
+                     'protocol': None, 'config_sync': None, 'vip': None})
         return result
 
     def send_openvpn_config(self, sn: str) -> None:
         """每次把设备添加到平台上线后，openvpn要连半天，可以主动推送下配置让openvpn连接的更快，
            如果设备已经连接上了openvpn就不在下发了
 
         :param sn: 单个sn
```

### Comparing `inhandtest-0.0.44/inhandtest/inserial.py` & `inhandtest-0.0.45/inhandtest/inserial.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.44/inhandtest/insocket.py` & `inhandtest-0.0.45/inhandtest/insocket.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.44/inhandtest/inssh.py` & `inhandtest-0.0.45/inhandtest/inssh.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,16 +51,14 @@
         :param command: 执行命令, 多条时使用分号隔开
         :return: 返回所有命令执行后的结果
         """
         result = None
         if command:
             stdin, stdout, stderr = self.ssh.exec_command(command)
             logging.info(f'exec command 【{command}】')
-            if stderr.read():
-                raise SSHException(f"exec command【{command}】error, {stderr.read().decode('utf-8')}")
             result = stdout.read().decode("utf-8")
             logging.info(f'command result 【{result}】')
         return result
 
     def download_file(self, remote_file, local_file) -> None:
         """
         从服务器上下载文件
```

### Comparing `inhandtest-0.0.44/inhandtest/ip.py` & `inhandtest-0.0.45/inhandtest/ip.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.44/inhandtest/mail.py` & `inhandtest-0.0.45/inhandtest/mail.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.44/inhandtest/pytest_email.html` & `inhandtest-0.0.45/inhandtest/pytest_email.html`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.44/inhandtest/telnet.py` & `inhandtest-0.0.45/inhandtest/telnet.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.44/inhandtest/tools.py` & `inhandtest-0.0.45/inhandtest/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -385,15 +385,15 @@
     """
     new_old = old
 
     def replace_(replace_str_: str):
         for k_, i_ in zip(replace_value.keys(), range(0, len(replace_value.keys()))):
             replace_str_ = replace_str_.replace(k_, '${' + str(i_) + '}')
         for v_, i_ in zip(replace_value.values(), range(0, len(replace_value.keys()))):
-            replace_str_ = replace_str_.replace('${' + str(i_) + '}', v_)
+            replace_str_ = replace_str_.replace('${' + str(i_) + '}', str(v_))
         return replace_str_
 
     if old and replace_value:
         replace_value = {k: v for k, v in replace_value.items() if v is not None}
         if replace_value:
             if isinstance(old, str):
                 new_old = replace_(old)
```

### Comparing `inhandtest-0.0.44/setup.py` & `inhandtest-0.0.45/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 setup
 
 """
 from distutils.core import setup
 
 setup(
     name='inhandtest',
-    version='0.0.44',
+    version='0.0.45',
     author='liwei',
     author_email='liwei@inhand.com.cn',
     description='inhand test tools, so easy',
     maintainer='liwei',
     maintainer_email='liwei@inhand.com.cn',
     # py_modules=['inhandtest.tools', 'inhandtest.telnet', 'inhandtest.inmodbus', 'inhandtest.inmqtt', 'inhandtest.file',
     #             'inhandtest.inrequest', 'inhandtest.inssh', 'inhandtest.base_page'],
@@ -23,11 +23,11 @@
     package_data={'inhandtest': ['pytest_email.html']},
     url='https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》',
     long_description='方便inhand测试同事在自动化测试时，对通用协议或者常用工具及方法做封装，需要使用时即在线安装；\n映翰通出品，追尾必究！',
     classifiers=[
         "Programming Language :: Python :: 3.7",
     ],
     install_requires=['pytz', 'requests', 'playwright', 'pyserial', 'modbus-tk', 'paho-mqtt', 'urllib3', 'paramiko',
-                      'emails', 'Jinja2', 'pymongo', 'psutil', 'lxml'
+                      'emails', 'Jinja2', 'pymongo', 'psutil', 'lxml', 'dynaconf'
                       # 这里是依赖列表，表示运行这个包的运行某些功能还需要你安装其他的包
                       ],
 )
```

