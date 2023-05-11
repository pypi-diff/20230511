# Comparing `tmp/inhandtest-0.0.42.tar.gz` & `tmp/inhandtest-0.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\inhandtest-0.0.42.tar", last modified: Sat May  6 07:40:04 2023, max compression
+gzip compressed data, was "dist\inhandtest-0.0.43.tar", last modified: Thu May 11 07:12:01 2023, max compression
```

## Comparing `inhandtest-0.0.42.tar` & `inhandtest-0.0.43.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 07:40:04.000000 inhandtest-0.0.42/
--rw-rw-rw-   0        0        0      535 2023-05-06 07:40:04.000000 inhandtest-0.0.42/PKG-INFO
--rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.42/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 07:40:04.000000 inhandtest-0.0.42/inhandtest/
--rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.42/inhandtest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:40:04.000000 inhandtest-0.0.42/inhandtest/base_page/
--rw-rw-rw-   0        0        0      134 2023-03-15 06:05:35.000000 inhandtest-0.0.42/inhandtest/base_page/__init__.py
--rw-rw-rw-   0        0        0    37327 2023-05-06 07:36:45.000000 inhandtest-0.0.42/inhandtest/base_page/_ig902_contents_locators.py
--rw-rw-rw-   0        0        0    61990 2023-03-31 06:55:18.000000 inhandtest-0.0.42/inhandtest/base_page/_vg710_contents_locators.py
--rw-rw-rw-   0        0        0    43975 2023-05-06 07:36:45.000000 inhandtest-0.0.42/inhandtest/base_page/base_page.py
--rw-rw-rw-   0        0        0    10436 2023-04-18 03:34:40.000000 inhandtest-0.0.42/inhandtest/base_page/table_tr.py
--rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.42/inhandtest/exception.py
--rw-rw-rw-   0        0        0     3890 2023-03-30 10:08:49.000000 inhandtest-0.0.42/inhandtest/file.py
--rw-rw-rw-   0        0        0    11861 2023-05-06 01:56:01.000000 inhandtest-0.0.42/inhandtest/inmodbus.py
--rw-rw-rw-   0        0        0     4880 2023-04-27 01:05:22.000000 inhandtest-0.0.42/inhandtest/inmongodb.py
--rw-rw-rw-   0        0        0    22049 2023-03-30 10:08:49.000000 inhandtest-0.0.42/inhandtest/inmqtt.py
--rw-rw-rw-   0        0        0    45529 2023-04-24 06:54:53.000000 inhandtest-0.0.42/inhandtest/inrequest.py
--rw-rw-rw-   0        0        0     7583 2023-05-06 07:36:44.000000 inhandtest-0.0.42/inhandtest/inserial.py
--rw-rw-rw-   0        0        0    12335 2023-04-06 06:40:29.000000 inhandtest-0.0.42/inhandtest/insocket.py
--rw-rw-rw-   0        0        0     6213 2023-05-06 01:08:13.000000 inhandtest-0.0.42/inhandtest/inssh.py
--rw-rw-rw-   0        0        0     1144 2023-03-30 10:18:47.000000 inhandtest-0.0.42/inhandtest/ip.py
--rw-rw-rw-   0        0        0    11606 2023-05-06 06:45:39.000000 inhandtest-0.0.42/inhandtest/mail.py
--rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.42/inhandtest/pytest_email.html
--rw-rw-rw-   0        0        0    32728 2023-05-06 01:14:17.000000 inhandtest-0.0.42/inhandtest/telnet.py
--rw-rw-rw-   0        0        0    25206 2023-05-06 07:30:45.000000 inhandtest-0.0.42/inhandtest/tools.py
--rw-rw-rw-   0        0        0      123 2023-05-06 01:36:21.000000 inhandtest-0.0.42/requirements.txt
--rw-rw-rw-   0        0        0     1438 2023-05-06 07:38:40.000000 inhandtest-0.0.42/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 07:12:01.000000 inhandtest-0.0.43/
+-rw-rw-rw-   0        0        0      535 2023-05-11 07:12:01.000000 inhandtest-0.0.43/PKG-INFO
+-rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.43/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 07:12:01.000000 inhandtest-0.0.43/inhandtest/
+-rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.43/inhandtest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 07:12:01.000000 inhandtest-0.0.43/inhandtest/base_page/
+-rw-rw-rw-   0        0        0      134 2023-03-15 06:05:35.000000 inhandtest-0.0.43/inhandtest/base_page/__init__.py
+-rw-rw-rw-   0        0        0    39362 2023-05-10 08:44:26.000000 inhandtest-0.0.43/inhandtest/base_page/_ig902_contents_locators.py
+-rw-rw-rw-   0        0        0    27870 2023-05-10 08:56:15.000000 inhandtest-0.0.43/inhandtest/base_page/_ir3XX_contents_locators.py
+-rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.43/inhandtest/base_page/_vg710_contents_locators.py
+-rw-rw-rw-   0        0        0    46619 2023-05-11 07:10:20.000000 inhandtest-0.0.43/inhandtest/base_page/base_page.py
+-rw-rw-rw-   0        0        0    10957 2023-05-09 09:49:30.000000 inhandtest-0.0.43/inhandtest/base_page/table_tr.py
+-rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.43/inhandtest/exception.py
+-rw-rw-rw-   0        0        0     3890 2023-03-30 10:08:49.000000 inhandtest-0.0.43/inhandtest/file.py
+-rw-rw-rw-   0        0        0    11861 2023-05-06 01:56:01.000000 inhandtest-0.0.43/inhandtest/inmodbus.py
+-rw-rw-rw-   0        0        0     4880 2023-04-27 01:05:22.000000 inhandtest-0.0.43/inhandtest/inmongodb.py
+-rw-rw-rw-   0        0        0    22049 2023-03-30 10:08:49.000000 inhandtest-0.0.43/inhandtest/inmqtt.py
+-rw-rw-rw-   0        0        0    46254 2023-05-11 06:59:24.000000 inhandtest-0.0.43/inhandtest/inrequest.py
+-rw-rw-rw-   0        0        0     7583 2023-05-06 07:36:44.000000 inhandtest-0.0.43/inhandtest/inserial.py
+-rw-rw-rw-   0        0        0    12335 2023-04-06 06:40:29.000000 inhandtest-0.0.43/inhandtest/insocket.py
+-rw-rw-rw-   0        0        0     6213 2023-05-06 01:08:13.000000 inhandtest-0.0.43/inhandtest/inssh.py
+-rw-rw-rw-   0        0        0     1144 2023-03-30 10:18:47.000000 inhandtest-0.0.43/inhandtest/ip.py
+-rw-rw-rw-   0        0        0    11620 2023-05-08 10:30:07.000000 inhandtest-0.0.43/inhandtest/mail.py
+-rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.43/inhandtest/pytest_email.html
+-rw-rw-rw-   0        0        0    32728 2023-05-06 01:14:17.000000 inhandtest-0.0.43/inhandtest/telnet.py
+-rw-rw-rw-   0        0        0    25276 2023-05-08 10:30:07.000000 inhandtest-0.0.43/inhandtest/tools.py
+-rw-rw-rw-   0        0        0      123 2023-05-06 01:36:21.000000 inhandtest-0.0.43/requirements.txt
+-rw-rw-rw-   0        0        0     1438 2023-05-11 07:11:42.000000 inhandtest-0.0.43/setup.py
```

### Comparing `inhandtest-0.0.42/PKG-INFO` & `inhandtest-0.0.43/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: inhandtest
-Version: 0.0.42
+Version: 0.0.43
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 License: UNKNOWN
 Description: 方便inhand测试同事在自动化测试时，对通用协议或者常用工具及方法做封装，需要使用时即在线安装；
         映翰通出品，追尾必究！
```

### Comparing `inhandtest-0.0.42/README.md` & `inhandtest-0.0.43/README.md`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.42/inhandtest/base_page/_ig902_contents_locators.py` & `inhandtest-0.0.43/inhandtest/base_page/_ig902_contents_locators.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,24 +23,26 @@
                                    'network_service_dns': 'DNS', "gps_configure": "GPS Configure",
                                    "gps_ip_forwarding": "GPS IP Forwarding",
                                    "gps_serial_forwarding": "GPS Serial Forwarding",
                                    'network_service_host': 'Host List', 'network_routing': 'Routing',
                                    'network_routing_status': 'Routing Status',
                                    'network_routing_static': 'Static Routing', 'network_firewall': 'Firewall',
                                    'network_firewall_acl': 'ACL', 'network_firewall_nat': 'NAT',
-                                   'l2tp_status': 'Status', 'l2tp_client': 'L2TP Client', 'l2tp_service': 'L2TP Service',
+                                   'l2tp_status': 'Status', 'l2tp_client': 'L2TP Client',
+                                   'l2tp_service': 'L2TP Service',
                                    'edge': 'Edge Computing', 'python_edge': 'Python Edge Computing',
                                    'docker_manager': 'Docker Manager', 'cloud_edge_computing': 'Cloud Edge Computing',
                                    'device_supervisor': 'Device Supervisor', 'measure_monitor': 'Measure Monitor',
                                    'monitoring_list': 'Monitoring List', 'group': 'Group',
                                    'alarm': 'Alarm', 'realtime_alarms': 'Realtime Alarms', 'alarm_rules': 'Alarm Rules',
                                    'history_alarms': 'History Alarms', 'alarm_label': 'Alarm Label',
                                    'cloud': 'Cloud', 'mqtt_cloud_service': 'MQTT Cloud Service',
                                    'whitehawk_energy_manager': 'Whitehawk Energy Manager', 'protocol': 'Protocol',
-                                   'parameter_settings': 'Parameter Settings', 'custom_quickfunctions': 'Custom QuickFunctions',
+                                   'parameter_settings': 'Parameter Settings',
+                                   'custom_quickfunctions': 'Custom QuickFunctions',
                                    'system': 'System', 'system_time': 'System Time', 'system_log': 'Log',
                                    'system_config': 'Configuration Management', 'system_cloud': 'InHand Cloud',
                                    'system_firmware': 'Firmware Upgrade', 'system_tools': 'Access Tools',
                                    'system_user_management': 'User Management', 'system_reboot': 'Reboot',
                                    'system_network_tools': 'Network Tools', 'logout': 'Logout',
                                    'system_3rd_party': '3rd Party Notification', 'logout_submit': 'Confirm',
                                    'configuration': ' Configuration', 'trigger_condition': 'Trigger Condition',
@@ -82,18 +84,20 @@
                            "dhcp": "DHCP Server", "dns": "DNS Server", "gps": "GPS Configure",
                            "host_list": "MAC Address", "routing_status": "Distance/Metric",
                            "static_routing": "Track ID", "acl": "Access Control Strategy",
                            "nat": "Network Address Translation(NAT) Rules",
                            "l2tp_status": "Local Session ID", "l2tp_client": "L2TPv3 Session",
                            "l2tp_service": "Enable L2TP Server", "python_edge_computing": "Python Engine",
                            "docker_manager": "Enable Docker Manager", "cloud_edge_computing": "Azure IoT Edge",
-                           "azure_iot_edge": "Enable Security Daemon",  "aws_iot_greengrass": "Enable AWS IoT Greengrass",
+                           "azure_iot_edge": "Enable Security Daemon",
+                           "aws_iot_greengrass": "Enable AWS IoT Greengrass",
                            "measure_monitor": "Controller List", "alarm": "Realtime Alarms",
                            "cloud": "MQTT Cloud Service", "mqtt_cloud_service": "Enable Cloud",
-                           "whitehawk_energy_manager": "Enable Whitehawk Energy Manager", "protocol": "Modbus TCP Slave",
+                           "whitehawk_energy_manager": "Enable Whitehawk Energy Manager",
+                           "protocol": "Modbus TCP Slave",
                            "parameter_settings": "Serial Port Settings", "custom_quickfunctions": "QuickFunction List",
                            "system_time": "Enable SNTP Clients", "log": "View Recent",
                            "log_configure": "Send to the remote log server",
                            "configuration_management": "Configuration Files Operations",
                            "inhand_cloud": "InHand Connect Service", "firmware_upgrade": "Select Firmware",
                            "access_tools": "Enable HTTPS", "user_management": "User Permissions",
                            "reboot": "Immediately Reboot", "network_tools": "Traceroute",
@@ -127,19 +131,27 @@
 
     @property
     def overview_menu(self) -> Locator:
         return self.page.locator('//*[@id="root"]/div/section/section/header/div/div/div[1]/div[2]/div/ul/li[2]/a')
 
     @property
     def network_menu(self) -> Locator:
-        return self.page.locator(f'a:has-text("{self.__locale.get("network")}")')
+        return self.page.locator('//*[@id="root"]/div/section/section/header/div/div/div[1]/div[2]/div/ul/li[4]/a')
+
+    @property
+    def edge_menu(self) -> Locator:
+        return self.page.locator('//*[@id="root"]/div/section/section/header/div/div/div[1]/div[2]/div/ul/li[6]/a')
+
+    @property
+    def system_menu(self) -> Locator:
+        return self.page.locator('//*[@id="root"]/div/section/section/header/div/div/div[1]/div[2]/div/ul/li[8]/a')
 
     @property
     def network_interface_menu(self) -> Locator:
-        return self.page.locator(f'text={self.__locale.get("network_interface")}')
+        return self.page.locator(f'div:text-is("{self.__locale.get("network_interface")}")')
 
     @property
     def network_interface_cellular_menu(self) -> Locator:
         return self.page.locator(f'a:has-text("{self.__locale.get("network_interface_cellular")}")')
 
     @property
     def network_interface_ethernet_menu(self) -> Locator:
@@ -163,15 +175,15 @@
 
     @property
     def network_interface_502_lan_menu(self) -> Locator:
         return self.page.locator('a:has-text("LAN")')
 
     @property
     def network_service_menu(self) -> Locator:
-        return self.page.locator(f'text={self.__locale.get("network_service")}')
+        return self.page.locator(f'div:text-is("{self.__locale.get("network_service")}")')
 
     @property
     def network_service_dhcp_menu(self) -> Locator:
         return self.page.locator(f'a:has-text("{self.__locale.get("network_service_dhcp")}")')
 
     @property
     def network_service_dns_menu(self) -> Locator:
@@ -183,27 +195,27 @@
 
     @property
     def network_service_host_menu(self) -> Locator:
         return self.page.locator(f'a:has-text("{self.__locale.get("network_service_host")}")')
 
     @property
     def network_routing_menu(self) -> Locator:
-        return self.page.locator(f'text={self.__locale.get("network_routing")}')
+        return self.page.locator(f'div:text-is("{self.__locale.get("network_routing")}")')
 
     @property
     def network_routing_status_menu(self) -> Locator:
         return self.page.locator(f'a:has-text("{self.__locale.get("network_routing_status")}")')
 
     @property
     def network_routing_static_menu(self) -> Locator:
         return self.page.locator(f'a:has-text("{self.__locale.get("network_routing_static")}")')
 
     @property
     def network_firewall_menu(self) -> Locator:
-        return self.page.locator(f'text={self.__locale.get("network_firewall")}')
+        return self.page.locator(f'div:text-is("{self.__locale.get("network_firewall")}")')
 
     @property
     def network_firewall_acl_menu(self) -> Locator:
         return self.page.locator(f'a:has-text("{self.__locale.get("network_firewall_acl")}")')
 
     @property
     def network_firewall_nat_menu(self) -> Locator:
@@ -214,40 +226,36 @@
         return self.page.locator('div:text-is("VPN")')
 
     @property
     def network_vpn_l2tp_menu(self) -> Locator:
         return self.page.locator('a:has-text("L2TP")')
 
     @property
-    def edge_menu(self) -> Locator:
-        return self.page.locator(f'a:has-text("{self.__locale.get("edge")}")')
-
-    @property
     def python_edge_menu(self) -> Locator:
         return self.page.locator(f'a:has-text("{self.__locale.get("python_edge")}")')
 
     @property
     def docker_manager_menu(self) -> Locator:
         return self.page.locator(f'a:has-text("{self.__locale.get("docker_manager")}")')
 
     @property
     def cloud_edge_computing_menu(self) -> Locator:
         return self.page.locator(f'a:has-text("{self.__locale.get("cloud_edge_computing")}")')
-    
+
     @property
     def cloud_edge_computing_azure_iot_edge_menu(self) -> Locator:
         return self.page.locator('div:text-is("Azure IoT Edge")')
-    
+
     @property
     def cloud_edge_computing_aws_iot_greengrass_menu(self) -> Locator:
         return self.page.locator('div:text-is("AWS IoT Greengrass")')
 
     @property
     def device_supervisor_menu(self) -> Locator:
-        return self.page.locator(f'text={self.__locale.get("device_supervisor")}')
+        return self.page.locator(f'div:text-is("{self.__locale.get("device_supervisor")}")')
 
     @property
     def measure_monitor_menu(self) -> Locator:
         return self.page.locator(
             f'.ant-menu.ant-menu-sub.ant-menu-inline >> a:has-text("{self.__locale.get("measure_monitor")}")')
 
     @property
@@ -272,18 +280,14 @@
 
     @property
     def custom_quickfunctions_menu(self) -> Locator:
         return self.page.locator(
             f'.ant-menu.ant-menu-sub.ant-menu-inline >> a:has-text("{self.__locale.get("custom_quickfunctions")}")')
 
     @property
-    def system_menu(self) -> Locator:
-        return self.page.locator(f'a:has-text("{self.__locale.get("system")}")')
-
-    @property
     def system_time_menu(self) -> Locator:
         return self.page.locator(f'a:has-text("{self.__locale.get("system_time")}")')
 
     @property
     def system_log_menu(self) -> Locator:
         return self.page.locator(f'a:has-text("{self.__locale.get("system_log")}")')
 
@@ -323,134 +327,156 @@
     def tags_menu(self) -> dict:
         return {
             'overview': {
                 'menu': self.overview_menu,
                 'visible_locator': [self.content_span_text('overview')],
             },
             'network': {
-                'default': 'network_interface_cellular',
+                'default': 'network_interface',
                 'menu': self.network_menu,
-                # interface
-                'network_interface_cellular': {
-                    'menu': self.network_interface_cellular_menu,
-                    'visible_locator': [self.content_span_text('cellular')],
-                    'wait_locator': [self.content_span_text('cellular')]},
-                'network_interface_ethernet': {
-                    'default': 'gigabitethernet_01',
-                    'menu': self.network_interface_ethernet_menu,
-                    'visible_locator': [self.content_span_text('ethernet')],
-                    'wait_locator': [self.content_span_text('ethernet')],
-                    'gigabitethernet_01': {
-                        'menu': self.page.locator(f'div:text-is("{self.__locale.get("gigabitethernet")} 0/1")'),
-                    },
-                    'gigabitethernet_02': {
-                        'menu': self.page.locator(f'div:text-is("{self.__locale.get("gigabitethernet")} 0/2")'),
-                    }
-                },
-                'network_interface_bridge': {
-                    'menu': self.network_interface_bridge_menu,
-                    'visible_locator': [self.content_span_text('bridge')],
-                    'wait_locator': [self.content_span_text('bridge')]},
-                'network_interface_wlan': {
-                    'menu': self.network_interface_wlan_menu,
-                    'visible_locator': [self.content_span_text('"wlan')],
-                    'wait_locator': [self.content_span_text('"wlan')]},
-                'network_interface_loopback': {
-                    'menu': self.network_interface_loopback_menu,
-                    'visible_locator': [self.content_span_text('loopback')],
-                    'wait_locator': [self.content_span_text('loopback')]},
-                # service
-                'network_service_dhcp': {
-                    'menu': [self.network_service_menu, self.network_service_dhcp_menu],
-                    'visible_locator': [self.content_span_text('dhcp')],
-                    'wait_locator': [self.content_span_text('dhcp')]},
-                'network_service_dns': {
-                    'menu': [self.network_service_menu, self.network_service_dns_menu],
-                    'visible_locator': [self.content_span_text('dns')],
-                    'wait_locator': [self.content_span_text('dns')]},
-                'network_service_gps': {
-                    'default': 'gps_configure',
-                    'menu': [self.network_service_menu, self.network_service_gps_menu],
-                    'visible_locator': [self.content_span_text('gps')],
-                    'wait_locator': [self.content_span_text('gps')],
-                    'gps_configure': {
-                        'menu': self.page.locator(f'div:text-is("{self.__locale.get("gps_configure")}")'),
-                        'visible_locator': [self.page.locator('.ant-form-item-no-colon')],
-                        'wait_locator': [self.page.locator('.ant-form-item-no-colon')],
-                    },
-                    'gps_ip_forwarding': {
-                        'menu': self.page.locator(f'div:text-is("{self.__locale.get("gps_ip_forwarding")}")'),
-                        'visible_locator': [self.page.locator('#enable')],
-                        'wait_locator': [self.page.locator('#enable')],
-                    },
-                    'gps_serial_forwarding': {
-                        'menu': self.page.locator(f'div:text-is("{self.__locale.get("gps_serial_forwarding")}")'),
-                        'visible_locator': [self.page.locator('#enable')],
-                        'wait_locator': [self.page.locator('#enable')],
-                    },
-                },
-                'network_service_host_list': {
-                    'menu': [self.network_service_menu, self.network_service_host_menu],
-                    'visible_locator': [self.content_span_text('host_list')],
-                    'wait_locator': [self.content_span_text('host_list')]},
-                # routing
-                'network_routing_routing_status': {
-                    'menu': [self.network_routing_menu, self.network_routing_status_menu],
-                    'visible_locator': [self.content_span_text('routing_status')],
-                    'wait_locator': [self.content_span_text('routing_status')]},
-                'network_routing_static_routing': {
-                    'menu': [self.network_routing_menu, self.network_routing_static_menu],
-                    'visible_locator': [self.content_span_text('static_routing')],
-                    'wait_locator': [self.content_span_text('static_routing')]},
-                # firewall
-                'network_firewall_acl': {
-                    'menu': [self.network_firewall_menu, self.network_firewall_acl_menu],
-                    'visible_locator': [self.content_span_text('acl')],
-                    'wait_locator': [self.content_span_text('acl')]},
-                'network_firewall_nat': {
-                    'menu': [self.network_firewall_menu, self.network_firewall_nat_menu],
-                    'visible_locator': [self.content_span_text('nat')],
-                    'wait_locator': [self.content_span_text('nat')]},
-                # vpn
-                'network_vpn_l2tp': {
-                    'default': 'status',
-                    'menu': [self.network_vpn_menu, self.network_vpn_l2tp_menu],
-                    'status': {
-                        'menu': self.page.locator(f'div:text-is("{self.__locale.get("l2tp_status")}")'),
-                        'visible_locator': [self.content_span_text('l2tp_status')],
-                        'wait_locator': [self.content_span_text('l2tp_status')]
-                    },
-                    'client': {
-                        'menu': self.page.locator(f'div:text-is("{self.__locale.get("l2tp_client")}")'),
-                        'visible_locator': [self.content_span_text('l2tp_client')],
-                        'wait_locator': [self.content_span_text('l2tp_client')]
-                    },
-                    'service': {
-                        'menu': self.page.locator(f'div:text-is("{self.__locale.get("l2tp_service")}")'),
-                        'visible_locator': [self.content_span_text('l2tp_service')],
-                        'wait_locator': [self.content_span_text('l2tp_service')]
+                'visible_locator': [self.network_interface_menu],
+                'wait_locator': [self.network_interface_menu],
+                # Network Interface
+                'network_interface': {
+                    'menu': self.network_interface_menu,
+                    'visible_locator': [self.network_interface_cellular_menu],
+                    'wait_locator': [self.network_interface_cellular_menu],
+                    'cellular': {
+                        'menu': self.network_interface_cellular_menu,
+                        'visible_locator': [self.content_span_text('cellular')],
+                        'wait_locator': [self.content_span_text('cellular')]},
+                    'ethernet': {
+                        'default': 'gigabitethernet_01',
+                        'menu': self.network_interface_ethernet_menu,
+                        'visible_locator': [self.content_span_text('ethernet')],
+                        'wait_locator': [self.content_span_text('ethernet')],
+                        'gigabitethernet_01': {
+                            'menu': self.page.locator(f'div:text-is("{self.__locale.get("gigabitethernet")} 0/1")'),
+                        },
+                        'gigabitethernet_02': {
+                            'menu': self.page.locator(f'div:text-is("{self.__locale.get("gigabitethernet")} 0/2")'),
+                        }
+                    },
+                    'bridge': {
+                        'menu': self.network_interface_bridge_menu,
+                        'visible_locator': [self.content_span_text('bridge')],
+                        'wait_locator': [self.content_span_text('bridge')]},
+                    'wlan': {
+                        'menu': self.network_interface_wlan_menu,
+                        'visible_locator': [self.content_span_text('"wlan')],
+                        'wait_locator': [self.content_span_text('"wlan')]},
+                    'loopback': {
+                        'menu': self.network_interface_loopback_menu,
+                        'visible_locator': [self.content_span_text('loopback')],
+                        'wait_locator': [self.content_span_text('loopback')]}},
+                # Network Services
+                'network_services': {
+                    'menu': self.network_service_menu,
+                    'visible_locator': [self.network_service_dhcp_menu],
+                    'wait_locator': [self.network_service_dhcp_menu],
+                    'dhcp': {
+                        'menu': self.network_service_dhcp_menu,
+                        'visible_locator': [self.content_span_text('dhcp')],
+                        'wait_locator': [self.content_span_text('dhcp')]},
+                    'dns': {
+                        'menu': self.network_service_dns_menu,
+                        'visible_locator': [self.content_span_text('dns')],
+                        'wait_locator': [self.content_span_text('dns')]},
+                    'gps': {
+                        'default': 'gps_configure',
+                        'menu': self.network_service_gps_menu,
+                        'visible_locator': [self.content_span_text('gps')],
+                        'wait_locator': [self.content_span_text('gps')],
+                        'gps_configure': {
+                            'menu': self.page.locator(f'div:text-is("{self.__locale.get("gps_configure")}")'),
+                            'visible_locator': [self.page.locator('.ant-form-item-no-colon')],
+                            'wait_locator': [self.page.locator('.ant-form-item-no-colon')],
+                        },
+                        'gps_ip_forwarding': {
+                            'menu': self.page.locator(f'div:text-is("{self.__locale.get("gps_ip_forwarding")}")'),
+                            'visible_locator': [self.page.locator('#enable')],
+                            'wait_locator': [self.page.locator('#enable')],
+                        },
+                        'gps_serial_forwarding': {
+                            'menu': self.page.locator(f'div:text-is("{self.__locale.get("gps_serial_forwarding")}")'),
+                            'visible_locator': [self.page.locator('#enable')],
+                            'wait_locator': [self.page.locator('#enable')],
+                        },
+                    },
+                    'host_list': {
+                        'menu': self.network_service_host_menu,
+                        'visible_locator': [self.content_span_text('host_list')],
+                        'wait_locator': [self.content_span_text('host_list')]}},
+                # Routing
+                'routing': {
+                    'menu': self.network_routing_menu,
+                    'visible_locator': [self.network_routing_status_menu],
+                    'wait_locator': [self.network_routing_status_menu],
+                    'routing_status': {
+                        'menu': self.network_routing_status_menu,
+                        'visible_locator': [self.content_span_text('routing_status')],
+                        'wait_locator': [self.content_span_text('routing_status')]},
+                    'static_routing': {
+                        'menu': self.network_routing_static_menu,
+                        'visible_locator': [self.content_span_text('static_routing')],
+                        'wait_locator': [self.content_span_text('static_routing')]}},
+                # Firewall
+                'firewall': {
+                    'menu': self.network_firewall_menu,
+                    'visible_locator': [self.network_firewall_acl_menu],
+                    'wait_locator': [self.network_firewall_acl_menu],
+                    'acl': {
+                        'menu': self.network_firewall_acl_menu,
+                        'visible_locator': [self.content_span_text('acl')],
+                        'wait_locator': [self.content_span_text('acl')]},
+                    'nat': {
+                        'menu': self.network_firewall_nat_menu,
+                        'visible_locator': [self.content_span_text('nat')],
+                        'wait_locator': [self.content_span_text('nat')]}},
+                # VPN
+                'vpn': {
+                    'menu': self.network_vpn_menu,
+                    'visible_locator': [self.network_vpn_l2tp_menu],
+                    'wait_locator': [self.network_vpn_l2tp_menu],
+                    'l2tp': {
+                        'default': 'status',
+                        'menu': self.network_vpn_l2tp_menu,
+                        'status': {
+                            'menu': self.page.locator(f'div:text-is("{self.__locale.get("l2tp_status")}")'),
+                            'visible_locator': [self.content_span_text('l2tp_status')],
+                            'wait_locator': [self.content_span_text('l2tp_status')]
+                        },
+                        'l2tp_client': {
+                            'menu': self.page.locator(f'div:text-is("{self.__locale.get("l2tp_client")}")'),
+                            'visible_locator': [self.content_span_text('l2tp_client')],
+                            'wait_locator': [self.content_span_text('l2tp_client')]
+                        },
+                        'l2tp_service': {
+                            'menu': self.page.locator(f'div:text-is("{self.__locale.get("l2tp_service")}")'),
+                            'visible_locator': [self.content_span_text('l2tp_service')],
+                            'wait_locator': [self.content_span_text('l2tp_service')]}
                     }
                 }
             },
-            'edge': {
-                'default': 'edge_python_edge',
+            'edge_computing': {
+                'default': 'python_edge_computing',
                 'menu': self.edge_menu,
-                'visible_locator': [self.page.locator(f'span:text-is("APP")')],
-                'wait_locator': [self.page.locator(f'span:text-is("APP")')],
-                'edge_python_edge': {
+                'visible_locator': [self.device_supervisor_menu],
+                'wait_locator': [self.device_supervisor_menu],
+                'python_edge_computing': {
                     'menu': self.python_edge_menu,
                     'visible_locator': [self.content_span_text('python_edge_computing')],
                     'wait_locator': [self.content_span_text('python_edge_computing')]
                 },
-                'edge_docker_manager': {
+                'docker_manager': {
                     'menu': self.docker_manager_menu,
                     'visible_locator': [self.content_span_text('docker_manager')],
                     'wait_locator': [self.content_span_text('docker_manager')]
                 },
-                'edge_cloud_edge_computing': {
+                'cloud_edge_computing': {
                     'default': 'azure_iot_edge',
                     'menu': self.cloud_edge_computing_menu,
                     'visible_locator': [self.content_span_text('cloud_edge_computing')],
                     'wait_locator': [self.content_span_text('cloud_edge_computing')],
                     'azure_iot_edge': {
                         'menu': self.cloud_edge_computing_azure_iot_edge_menu,
                         'visible_locator': [self.content_span_text('azure_iot_edge')],
@@ -458,169 +484,184 @@
                     },
                     'aws_iot_greengrass': {
                         'menu': self.cloud_edge_computing_aws_iot_greengrass_menu,
                         'visible_locator': [self.content_span_text('aws_iot_greengrass')],
                         'wait_locator': [self.content_span_text('aws_iot_greengrass')],
                     }
                 },
-                # device supervisor
-                'edge_device_supervisor_measure_monitor': {
-                    'default': 'monitoring_list',
-                    'menu': [self.device_supervisor_menu, self.measure_monitor_menu],
-                    'monitoring_list': {
-                        'menu': self.page.locator(f'div:text-is("{self.__locale.get("monitoring_list")}")')
-                    },
-                    'group': {
-                        'menu': self.page.locator(f'div:text-is("{self.__locale.get("group")}")')
-                    },
-                },
-                'edge_device_supervisor_alarm': {
-                    'default': 'realtime_alarms',
-                    'menu': [self.device_supervisor_menu, self.alarm_menu],
-                    'visible_locator': [self.content_span_text('alarm')],
-                    'wait_locator': [self.content_span_text('alarm')],
-                    'realtime_alarms': {
-                        'menu': self.page.locator(f'div:text-is("{self.__locale.get("realtime_alarms")}")'),
-                        'visible_locator': [self.page.locator('.ant-table-header.ant-table-hide-scrollbar')],
-                        'wait_locator': [self.page.locator('.ant-table-header.ant-table-hide-scrollbar')]
-                    },
-                    'alarm_rules': {
-                        'menu': self.page.locator(f'div:text-is("{self.__locale.get("alarm_rules")}")'),
-                        'visible_locator': [self.page.locator(f'span:text-is("{self.__locale.get("trigger_condition")}")')],
-                        'wait_locator': [self.page.locator(f'span:text-is("{self.__locale.get("trigger_condition")}")')]
-                    },
-                    'history_alarms': {
-                        'menu': self.page.locator(f'div:text-is("{self.__locale.get("history_alarms")}")'),
-                        'visible_locator': [self.page.locator('span:text-is("~")')],
-                        'wait_locator': [self.page.locator('span:text-is("~")')]
-                    },
-                    'alarm_label': {
-                        'menu': self.page.locator(f'div:text-is("{self.__locale.get("alarm_label")}")'),
-                        'visible_locator': [self.page.locator('.ant-table-selection-column >> nth=0')],
-                        'wait_locator': [self.page.locator('.ant-table-selection-column >> nth=0')]
-                    },
-                },
-                'edge_device_supervisor_cloud': {
-                    'default': 'mqtt_cloud_service',
-                    'menu': [self.device_supervisor_menu, self.cloud_menu],
-                    'visible_locator': [self.content_span_text('cloud')],
-                    'wait_locator': [self.content_span_text('cloud')],
-                    'mqtt_cloud_service': {
-                        'menu': self.page.locator(f'div:text-is("{self.__locale.get("mqtt_cloud_service")}")'),
-                        'visible_locator': [self.content_span_text('mqtt_cloud_service')],
-                        'wait_locator': [self.content_span_text('mqtt_cloud_service')]
-                    },
-                    'whitehawk_energy_manager': {
-                        'menu': self.page.locator(f'div:text-is("{self.__locale.get("whitehawk_energy_manager")}")'),
-                        'visible_locator': [self.content_span_text('whitehawk_energy_manager')],
-                        'wait_locator': [self.content_span_text('whitehawk_energy_manager')]
-                    }
-                },
-                'edge_device_supervisor_protocol': {
-                    'default': 'modbus_tcp_slave',
-                    'menu': [self.device_supervisor_menu, self.protocol_menu],
-                    'modbus_tcp_slave': {
-                        'menu': self.page.locator(f'div:text-is("Modbus TCP Slave")'),
-                        'visible_locator': [self.page.locator(f'text=Modbus TCP Slave{self.__locale.get("configuration")}')],
-                        'wait_locator': [self.page.locator(f'text=Modbus TCP Slave{self.__locale.get("configuration")}')],
-                    },
-                    'iec_104_server': {
-                        'menu': self.page.locator(f'div:text-is("IEC 104 Server")'),
-                        'visible_locator': [self.page.locator(f'text=IEC 104 Server{self.__locale.get("configuration")}')],
-                        'wait_locator': [self.page.locator(f'text=IEC 104 Server{self.__locale.get("configuration")}')],
-                    },
-                    'opcua_server': {
-                        'menu': self.page.locator(f'div:text-is("OPCUA Server")'),
-                        'visible_locator': [self.page.locator(f'text=OPCUA Server{self.__locale.get("configuration")}')],
-                        'wait_locator': [self.page.locator(f'text=OPCUA Server{self.__locale.get("configuration")}')],
-                    },
-                    'modbus_rtu_slave': {
-                        'menu': self.page.locator(f'div:text-is("Modbus RTU Slave")'),
-                        'visible_locator': [self.page.locator(f'text=Modbus RTU Slave{self.__locale.get("configuration")}')],
-                        'wait_locator': [self.page.locator(f'text=Modbus RTU Slave{self.__locale.get("configuration")}')],
-                    },
-                },
-                'edge_device_supervisor_parameter_settings': {
-                    'menu': [self.device_supervisor_menu, self.parameter_settings_menu],
-                    'visible_locator': [self.content_span_text('parameter_settings')],
-                    'wait_locator': [self.content_span_text('parameter_settings')]
-                },
-                'edge_device_supervisor_custom_quickfunctions': {
-                    'menu': [self.device_supervisor_menu, self.custom_quickfunctions_menu],
-                    'visible_locator': [self.content_span_text('custom_quickfunctions')],
-                    'wait_locator': [self.content_span_text('custom_quickfunctions')]
+                # Device Supervisor
+                'device_supervisor': {
+                    'menu': self.device_supervisor_menu,
+                    'visible_locator': [self.measure_monitor_menu],
+                    'wait_locator': [self.measure_monitor_menu],
+                    'measure_monitor': {
+                        'default': 'monitoring_list',
+                        'menu': self.measure_monitor_menu,
+                        'monitoring_list': {
+                            'menu': self.page.locator(f'div:text-is("{self.__locale.get("monitoring_list")}")')
+                        },
+                        'group': {
+                            'menu': self.page.locator(f'div:text-is("{self.__locale.get("group")}")')
+                        },
+                    },
+                    'alarm': {
+                        'default': 'realtime_alarms',
+                        'menu': self.alarm_menu,
+                        'visible_locator': [self.content_span_text('alarm')],
+                        'wait_locator': [self.content_span_text('alarm')],
+                        'realtime_alarms': {
+                            'menu': self.page.locator(f'div:text-is("{self.__locale.get("realtime_alarms")}")'),
+                            'visible_locator': [self.page.locator('.ant-table-header.ant-table-hide-scrollbar')],
+                            'wait_locator': [self.page.locator('.ant-table-header.ant-table-hide-scrollbar')]
+                        },
+                        'alarm_rules': {
+                            'menu': self.page.locator(f'div:text-is("{self.__locale.get("alarm_rules")}")'),
+                            'visible_locator': [
+                                self.page.locator(f'span:text-is("{self.__locale.get("trigger_condition")}")')],
+                            'wait_locator': [
+                                self.page.locator(f'span:text-is("{self.__locale.get("trigger_condition")}")')]
+                        },
+                        'history_alarms': {
+                            'menu': self.page.locator(f'div:text-is("{self.__locale.get("history_alarms")}")'),
+                            'visible_locator': [self.page.locator('span:text-is("~")')],
+                            'wait_locator': [self.page.locator('span:text-is("~")')]
+                        },
+                        'alarm_label': {
+                            'menu': self.page.locator(f'div:text-is("{self.__locale.get("alarm_label")}")'),
+                            'visible_locator': [self.page.locator('.ant-table-selection-column >> nth=0')],
+                            'wait_locator': [self.page.locator('.ant-table-selection-column >> nth=0')]
+                        },
+                    },
+                    'cloud': {
+                        'default': 'mqtt_cloud_service',
+                        'menu': self.cloud_menu,
+                        'visible_locator': [self.content_span_text('cloud')],
+                        'wait_locator': [self.content_span_text('cloud')],
+                        'mqtt_cloud_service': {
+                            'menu': self.page.locator(f'div:text-is("{self.__locale.get("mqtt_cloud_service")}")'),
+                            'visible_locator': [self.content_span_text('mqtt_cloud_service')],
+                            'wait_locator': [self.content_span_text('mqtt_cloud_service')]
+                        },
+                        'whitehawk_energy_manager': {
+                            'menu': self.page.locator(
+                                f'div:text-is("{self.__locale.get("whitehawk_energy_manager")}")'),
+                            'visible_locator': [self.content_span_text('whitehawk_energy_manager')],
+                            'wait_locator': [self.content_span_text('whitehawk_energy_manager')]
+                        }
+                    },
+                    'protocol': {
+                        'default': 'modbus_tcp_slave',
+                        'menu': self.protocol_menu,
+                        'modbus_tcp_slave': {
+                            'menu': self.page.locator(f'div:text-is("Modbus TCP Slave")'),
+                            'visible_locator': [
+                                self.page.locator(f'text=Modbus TCP Slave{self.__locale.get("configuration")}')],
+                            'wait_locator': [
+                                self.page.locator(f'text=Modbus TCP Slave{self.__locale.get("configuration")}')],
+                        },
+                        'iec_104_server': {
+                            'menu': self.page.locator(f'div:text-is("IEC 104 Server")'),
+                            'visible_locator': [
+                                self.page.locator(f'text=IEC 104 Server{self.__locale.get("configuration")}')],
+                            'wait_locator': [
+                                self.page.locator(f'text=IEC 104 Server{self.__locale.get("configuration")}')],
+                        },
+                        'opcua_server': {
+                            'menu': self.page.locator(f'div:text-is("OPCUA Server")'),
+                            'visible_locator': [
+                                self.page.locator(f'text=OPCUA Server{self.__locale.get("configuration")}')],
+                            'wait_locator': [
+                                self.page.locator(f'text=OPCUA Server{self.__locale.get("configuration")}')],
+                        },
+                        'modbus_rtu_slave': {
+                            'menu': self.page.locator(f'div:text-is("Modbus RTU Slave")'),
+                            'visible_locator': [
+                                self.page.locator(f'text=Modbus RTU Slave{self.__locale.get("configuration")}')],
+                            'wait_locator': [
+                                self.page.locator(f'text=Modbus RTU Slave{self.__locale.get("configuration")}')],
+                        },
+                    },
+                    'parameter_settings': {
+                        'menu': self.parameter_settings_menu,
+                        'visible_locator': [self.content_span_text('parameter_settings')],
+                        'wait_locator': [self.content_span_text('parameter_settings')]
+                    },
+                    'custom_quickfunctions': {
+                        'menu': self.custom_quickfunctions_menu,
+                        'visible_locator': [self.content_span_text('custom_quickfunctions')],
+                        'wait_locator': [self.content_span_text('custom_quickfunctions')]}
                 }
             },
             'system': {
                 'default': 'system_time',
                 'menu': self.system_menu,
                 'system_time': {
                     'menu': self.system_time_menu,
                     'visible_locator': [self.content_span_text('system_time')],
                     'wait_locator': [self.content_span_text('system_time')],
                 },
-                'system_log': {
+                'log': {
                     'default': 'log',
                     'menu': self.system_log_menu,
                     'log': {
                         'menu': self.page.locator('.ant-tabs-tab >> nth=0'),
                         'visible_locator': [self.content_span_text('log')],
                         'wait_locator': [self.content_span_text('log')],
                     },
                     'configure': {
                         'menu': self.page.locator('.ant-tabs-tab >> nth=1'),
                         'visible_locator': [self.content_span_text('log_configure')],
                         'wait_locator': [self.content_span_text('log_configure')],
                     }
                 },
-                'system_configuration_management': {
+                'configuration_management': {
                     'menu': self.system_config_menu,
                     'visible_locator': [self.content_span_text('configuration_management')],
                     'wait_locator': [self.content_span_text('configuration_management')],
                 },
-                'system_inhand_cloud': {
+                'inhand_cloud': {
                     'default': 'inhand_connect_service',
                     'menu': self.system_cloud_menu,
                     'visible_locator': [self.content_span_text('inhand_cloud')],
                     'wait_locator': [self.content_span_text('inhand_cloud')],
                     'inhand_connect_service': {
                         'menu': self.page.locator(f'div:text-is("InHand Connect Service")'),
                     },
                     'inhand_device_manager': {
                         'menu': self.page.locator(f'div:text-is("InHand Device Manager")'),
                     },
                     'inhand_iscada_cloud': {
                         'menu': self.page.locator(f'div:text-is("InHand iSCADA Cloud")'),
                     }
                 },
-                'system_firmware_upgrade': {
+                'firmware_upgrade': {
                     'menu': self.system_firmware_menu,
                     'visible_locator': [self.content_span_text('firmware_upgrade')],
                     'wait_locator': [self.content_span_text('firmware_upgrade')],
                 },
-                'system_access_tools': {
+                'access_tools': {
                     'menu': self.system_tools_menu,
                     'visible_locator': [self.content_span_text('access_tools')],
                     'wait_locator': [self.content_span_text('access_tools')],
                 },
-                'system_user_management': {
+                'user_management': {
                     'menu': self.system_user_management_menu,
                     'visible_locator': [self.content_span_text('user_management')],
                     'wait_locator': [self.content_span_text('user_management')],
                 },
-                'system_reboot': {
+                'reboot': {
                     'menu': self.system_reboot_menu,
                     'visible_locator': [self.content_span_text('reboot')],
                     'wait_locator': [self.content_span_text('reboot')],
                 },
-                'system_network_tools': {
+                'network_tools': {
                     'menu': self.system_network_tools_menu,
                     'visible_locator': [self.content_span_text('network_tools')],
                     'wait_locator': [self.content_span_text('network_tools')],
                 },
-                'system_3rd_party_notification': {
+                '3rd_party_notification': {
                     'menu': self.system_3rd_party_menu,
                     'visible_locator': [self.content_span_text('3rd_party_notification')],
                     'wait_locator': [self.content_span_text('3rd_party_notification')],
                 }
             },
         }
```

### Comparing `inhandtest-0.0.42/inhandtest/base_page/_vg710_contents_locators.py` & `inhandtest-0.0.43/inhandtest/base_page/_vg710_contents_locators.py`

 * *Files 6% similar despite different names*

```diff
@@ -151,830 +151,879 @@
     @property
     def wizards_menu(self) -> Locator:
         return self.page.locator('#ulLista_wizards')
 
     @property
     def tags_menu(self) -> dict:
         return {
-            'administration_system': {
-                'default': 'status',
-                'menu': [self.administration_menu, self.page.locator('#status_system')],
-                'mouse_move': (200, 0),
-                'visible_locator': [self.content_span_text('system')],
-                'status': {
-                    'menu': self.page.locator('#Span_status_system_tdstatus_system'),
-                    'visible_locator': [self.frame.locator(f'//td[text()="{self.__locale.get("bootloader")}"]')],
-                    'wait_locator': [self.frame.locator('//tr[@id="rtime"]')],
+            'administration': {
+                'default': 'system.status',
+                'menu': [self.administration_menu],
+                'system': {
+                    'default': 'status',
+                    'menu': [self.page.locator('#status_system')],
+                    'mouse_move': (200, 0),
+                    'visible_locator': [self.content_span_text('system')],
+                    'status': {
+                        'menu': self.page.locator('#Span_status_system_tdstatus_system'),
+                        'visible_locator': [
+                            self.frame.locator(f'//td[text()="{self.__locale.get("bootloader")}"]')],
+                        'wait_locator': [self.frame.locator('//tr[@id="rtime"]')],
+                    },
+                    'basic_setup': {
+                        'menu': self.page.locator('#Span_status_system_tdsetup_system'),
+                        'visible_locator': [self.frame.locator('#_f_language')],
+                        'wait_locator': [self.frame.locator('#_f_language')]},
+                    'advanced_setup': {
+                        'menu': self.page.locator('#Span_status_system_tdadv_setup_system'),
+                        'visible_locator': [self.frame.locator('#_f_sfe')],
+                        'wait_locator': [self.frame.locator('#_f_sfe')]}
                 },
-                'basic_setup': {
-                    'menu': self.page.locator('#Span_status_system_tdsetup_system'),
-                    'visible_locator': [self.frame.locator('#_f_language')],
-                    'wait_locator': [self.frame.locator('#_f_language')]},
-                'advanced_setup': {
-                    'menu': self.page.locator('#Span_status_system_tdadv_setup_system'),
-                    'visible_locator': [self.frame.locator('#_f_sfe')],
-                    'wait_locator': [self.frame.locator('#_f_sfe')]}
-            },
-            'administration_system_time': {
-                'default': 'system_time',
-                'menu': [self.administration_menu, self.page.locator('#setup_time')],
-                'mouse_move': (200, 0),
-                'visible_locator': [self.content_span_text('system_time')],
                 'system_time': {
-                    'menu': self.page.locator('#Span_setup_time_tdsetup_time'),
-                    'visible_locator': [self.frame.locator('#_f_tm_sel')],
-                    'wait_locator': [self.frame.locator('#_f_tm_sel')]},
-                'sntp_client': {
-                    'menu': self.page.locator("#Span_setup_time_tdsetup_sntp"),
-                    'visible_locator': [self.frame.locator('#_f_sntp_enable')],
-                    'wait_locator': [self.frame.locator('#bs-grid')]},
-                'ntp_server': {
-                    'menu': self.page.locator("#Span_setup_time_tdsetup_ntp_server"),
-                    'visible_locator': [self.frame.locator('#_f_ntp_enable')],
-                    'wait_locator': [self.frame.locator('#_f_ntp_enable')]}},
-            'administration_management_services': {
-                'default': 'management_services',
-                'menu': [self.administration_menu, self.page.locator('#setup_service')],
-                'mouse_move': (200, 0),
-                'visible_locator': [self.content_span_text('management_s')],
+                    'default': 'system_time',
+                    'menu': [self.page.locator('#setup_time')],
+                    'mouse_move': (200, 0),
+                    'visible_locator': [self.content_span_text('system_time')],
+                    'system_time': {
+                        'menu': self.page.locator('#Span_setup_time_tdsetup_time'),
+                        'visible_locator': [self.frame.locator('#_f_tm_sel')],
+                        'wait_locator': [self.frame.locator('#_f_tm_sel')]},
+                    'sntp_client': {
+                        'menu': self.page.locator("#Span_setup_time_tdsetup_sntp"),
+                        'visible_locator': [self.frame.locator('#_f_sntp_enable')],
+                        'wait_locator': [self.frame.locator('#bs-grid')]},
+                    'ntp_server': {
+                        'menu': self.page.locator("#Span_setup_time_tdsetup_ntp_server"),
+                        'visible_locator': [self.frame.locator('#_f_ntp_enable')],
+                        'wait_locator': [self.frame.locator('#_f_ntp_enable')]}
+
+                },
                 'management_services': {
-                    'menu': self.page.locator('Span_setup_service_tdsetup_service'),
-                    'visible_locator': [self.frame.locator('#_f_http_enable')],
-                    'wait_locator': [self.frame.locator('#_f_http_enable')]}},
-            'administration_user_management': {
-                'default': 'user_management',
-                'menu': [self.administration_menu, self.page.locator('#setup_create_user')],
-                'mouse_move': (200, 0),
-                'visible_locator': [self.content_span_text('user_m')],
+                    'default': 'management_services',
+                    'menu': [self.page.locator('#setup_service')],
+                    'mouse_move': (200, 0),
+                    'visible_locator': [self.content_span_text('management_s')],
+                    'management_services': {
+                        'menu': self.page.locator('#Span_setup_service_tdsetup_service'),
+                        'visible_locator': [self.frame.locator('#_f_http_enable')],
+                        'wait_locator': [self.frame.locator('#_f_http_enable')]}},
                 'user_management': {
-                    'menu': self.page.locator('#Span_setup_create_user_tdsetup_create_user'),
-                    'visible_locator': [self.frame.locator('#_f_adm_user')],
-                    'wait_locator': [self.frame.locator('#_f_adm_user')]}},
-            'administration_aaa': {
-                'default': 'radius',
-                'menu': [self.administration_menu, self.page.locator('#setup_radius')],
-                'mouse_move': (200, 0),
-                'visible_locator': [self.content_span_text('aaa')],
-                'radius': {
-                    'menu': self.page.locator('Span_setup_radius_tdsetup_radius'),
-                    'visible_locator': [self.frame.locator(
-                        f'//td[text()="{self.__locale.get("source_interface")}"][@class="co4"]')],
-                    'wait_locator': [self.frame.locator('#aaa-grid')]},
-                'tacacs+': {
-                    'menu': self.page.locator('Span_setup_radius_tdsetup_tacacs'),
-                    'visible_locator': [self.frame.locator(f'//title[text()="{self.model} -> Tacacs+"]')],
-                    'wait_locator': [self.frame.locator('#aaa-grid')]},
-                'ldap': {
-                    'menu': self.page.locator('Span_setup_radius_tdsetup_ldap'),
-                    'visible_locator': [self.frame.locator(f'//title[text()="{self.model} -> LDAP"]')],
-                    'wait_locator': [self.frame.locator('#aaa-grid')]},
-                'aaa_settings': {
-                    'menu': self.page.locator('Span_setup_radius_tdsetup_aaa'),
-                    'visible_locator': [self.frame.locator(f'#a1_telnet_first')],
-                    'wait_locator': [self.frame.locator('#aaa-grid')]}},
-            'administration_config_management': {
-                'default': 'config_management',
-                'menu': [self.administration_menu, self.page.locator('#admin_config')],
-                'mouse_move': (200, 0),
-                'visible_locator': [self.content_span_text('config_m')],
+                    'default': 'user_management',
+                    'menu': [self.page.locator('#setup_create_user')],
+                    'mouse_move': (200, 0),
+                    'visible_locator': [self.content_span_text('user_m')],
+                    'user_management': {
+                        'menu': self.page.locator('#Span_setup_create_user_tdsetup_create_user'),
+                        'visible_locator': [self.frame.locator('#_f_adm_user')],
+                        'wait_locator': [self.frame.locator('#_f_adm_user')]}},
+                'aaa': {
+                    'default': 'radius',
+                    'menu': [self.page.locator('#setup_radius')],
+                    'mouse_move': (200, 0),
+                    'visible_locator': [self.content_span_text('aaa')],
+                    'radius': {
+                        'menu': self.page.locator('#Span_setup_radius_tdsetup_radius'),
+                        'visible_locator': [self.frame.locator(
+                            f'//td[text()="{self.__locale.get("source_interface")}"][@class="co4"]')],
+                        'wait_locator': [self.frame.locator('#aaa-grid')]},
+                    'tacacs+': {
+                        'menu': self.page.locator('#Span_setup_radius_tdsetup_tacacs'),
+                        'visible_locator': [self.page.locator(f'//title[text()="{self.model} -> Tacacs+"]')],
+                        'wait_locator': [self.frame.locator('#aaa-grid')]},
+                    'ldap': {
+                        'menu': self.page.locator('#Span_setup_radius_tdsetup_ldap'),
+                        'visible_locator': [self.page.locator(f'//title[text()="{self.model} -> LDAP"]')],
+                        'wait_locator': [self.frame.locator('#aaa-grid')]},
+                    'aaa_settings': {
+                        'menu': self.page.locator('#Span_setup_radius_tdsetup_aaa'),
+                        'visible_locator': [self.frame.locator(f'#aaa-grid_head1')],
+                        'wait_locator': [self.frame.locator('#aaa-grid')]}},
                 'config_management': {
-                    'menu': self.page.locator('#Span_admin_config_tdadmin_config'),
-                    'visible_locator': [self.frame.locator('#reset-button')],
-                    'wait_locator': [self.frame.locator('#reset-button')]}},
-            'administration_device_manager': {
-                'default': 'status',
-                'menu': [self.administration_menu, self.page.locator('#dn_stat')],
-                'mouse_move': (200, 0),
-                'visible_locator': [self.content_span_text('device_m')],
-                'status': {
-                    'menu': self.page.locator('#Span_dn_stat_tddn_stat'),
-                    'visible_locator': [
-                        self.frame.locator(f'//td[text()="{self.__locale.get("device_manager")}"]')],
-                    'wait_locator': [self.frame.locator('#refresh-button')]},
+                    'default': 'config_management',
+                    'menu': [self.page.locator('#admin_config')],
+                    'mouse_move': (200, 0),
+                    'visible_locator': [self.content_span_text('config_m')],
+                    'config_management': {
+                        'menu': self.page.locator('#Span_admin_config_tdadmin_config'),
+                        'visible_locator': [self.frame.locator('#reset-button')],
+                        'wait_locator': [self.frame.locator('#reset-button')]}},
                 'device_manager': {
-                    'menu': self.page.locator('#Span_dn_stat_tddn_config'),
-                    'visible_locator': [self.frame.locator('#_f_mqtt_enable')],
-                    'wait_locator': [self.frame.locator('#_f_mqtt_enable')]}},
-            'administration_snmp': {
-                'default': 'snmp',
-                'mouse_move': (200, 0),
-                'menu': [self.administration_menu, self.page.locator('#setup_snmp')],
-                'visible_locator': [self.content_span_text('snmp')],
+                    'default': 'status',
+                    'menu': [self.page.locator('#dn_stat')],
+                    'mouse_move': (200, 0),
+                    'visible_locator': [self.content_span_text('device_m')],
+                    'status': {
+                        'menu': self.page.locator('#Span_dn_stat_tddn_stat'),
+                        'visible_locator': [
+                            self.frame.locator(f'//td[text()="{self.__locale.get("device_manager")}"]')],
+                        'wait_locator': [self.frame.locator('#refresh-button')]},
+                    'device_manager': {
+                        'menu': self.page.locator('#Span_dn_stat_tddn_config'),
+                        'visible_locator': [self.frame.locator('#_f_mqtt_enable')],
+                        'wait_locator': [self.frame.locator('#_f_mqtt_enable')]}},
                 'snmp': {
-                    'menu': self.page.locator('#Span_setup_snmp_tdsetup_snmp'),
-                    'visible_locator': [self.frame.locator('#_f_snmpd_enable')],
-                    'wait_locator': [self.frame.locator('#_f_snmpd_enable')]},
-                'snmptrap': {
-                    'menu': self.page.locator('#Span_setup_snmp_tdsetup_snmptrap'),
-                    'visible_locator': [self.frame.locator('#trapman-grid')],
-                    'wait_locator': [self.frame.locator('#trapman-grid')]},
-                'snmpmibs': {
-                    'menu': self.page.locator('#Span_setup_snmp_tdsetup_snmpmibs'),
-                    'visible_locator': [self.frame.locator('#_snmp_mib_file')],
-                    'wait_locator': [self.frame.locator('#_snmp_mib_file')]}},
-            'administration_alarm': {
-                'default': 'status',
-                'mouse_move': (200, 0),
-                'menu': [self.administration_menu, self.page.locator('#status_alarm')],
-                'visible_locator': [self.content_span_text('alarm')],
-                'status': {
-                    'menu': self.page.locator('#Span_status_alarm_tdstatus_alarm'),
-                    'visible_locator': [self.frame.locator('#clear-all')],
-                    'wait_locator': [self.frame.locator('#alarmlog-grid')]},
-                'alarm_input': {
-                    'menu': self.page.locator('#Span_status_alarm_tdsetup_alarm_in'),
-                    'visible_locator': [self.frame.locator('#_f_in_0')],
-                    'wait_locator': [self.frame.locator('#_f_in_0')]},
-                'alarm_output': {
-                    'menu': self.page.locator('#Span_status_alarm_tdsetup_alarm_out'),
-                    'visible_locator': [self.frame.locator('#test-button')],
-                    'wait_locator': [self.frame.locator('#email-alarm')]},
-                'alarm_map': {
-                    'menu': self.page.locator('#Span_status_alarm_tdsetup_alarm_map'),
-                    'visible_locator': [self.frame.locator('#_all_email')],
-                    'wait_locator': [self.frame.locator('#adm_grid')]}},
-            'administration_log': {
-                'default': 'log',
-                'mouse_move': (200, 0),
-                'menu': [self.administration_menu, self.page.locator('#status_log')],
-                'visible_locator': [self.content_span_text('log')],
+                    'default': 'snmp',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#setup_snmp')],
+                    'visible_locator': [self.content_span_text('snmp')],
+                    'snmp': {
+                        'menu': self.page.locator('#Span_setup_snmp_tdsetup_snmp'),
+                        'visible_locator': [self.frame.locator('#_f_snmpd_enable')],
+                        'wait_locator': [self.frame.locator('#_f_snmpd_enable')]},
+                    'snmptrap': {
+                        'menu': self.page.locator('#Span_setup_snmp_tdsetup_snmptrap'),
+                        'visible_locator': [self.frame.locator('#trapman-grid')],
+                        'wait_locator': [self.frame.locator('#trapman-grid')]},
+                    'snmpmibs': {
+                        'menu': self.page.locator('#Span_setup_snmp_tdsetup_snmpmibs'),
+                        'visible_locator': [self.frame.locator('#_snmp_mib_file')],
+                        'wait_locator': [self.frame.locator('#_snmp_mib_file')]}},
+                'alarm': {
+                    'default': 'status',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#status_alarm')],
+                    'visible_locator': [self.content_span_text('alarm')],
+                    'status': {
+                        'menu': self.page.locator('#Span_status_alarm_tdstatus_alarm'),
+                        'visible_locator': [self.frame.locator('#clear-all')],
+                        'wait_locator': [self.frame.locator('#alarmlog-grid')]},
+                    'alarm_input': {
+                        'menu': self.page.locator('#Span_status_alarm_tdsetup_alarm_in'),
+                        'visible_locator': [self.frame.locator('#_f_in_0')],
+                        'wait_locator': [self.frame.locator('#_f_in_0')]},
+                    'alarm_output': {
+                        'menu': self.page.locator('#Span_status_alarm_tdsetup_alarm_out'),
+                        'visible_locator': [self.frame.locator('#test-button')],
+                        'wait_locator': [self.frame.locator('#email-alarm')]},
+                    'alarm_map': {
+                        'menu': self.page.locator('#Span_status_alarm_tdsetup_alarm_map'),
+                        'visible_locator': [self.frame.locator('#_all_email')],
+                        'wait_locator': [self.frame.locator('#adm_grid')]}},
                 'log': {
-                    'menu': self.page.locator('#Span_status_log_tdstatus_log'),
-                    'visible_locator': [self.frame.locator('#_f_level')],
-                    'wait_locator': [self.frame.locator('#_f_level')]},
-                'system_log': {
-                    'menu': self.page.locator('#Span_status_log_tdadmin_log'),
-                    'visible_locator': [self.frame.locator('#_f_log_remote')],
-                    'wait_locator': [self.frame.locator('#server-grid')]}},
-            'administration_cron_job': {
-                'default': 'cron_job',
-                'mouse_move': (200, 0),
-                'menu': [self.administration_menu, self.page.locator('#scheduler')],
-                'visible_locator': [self.content_span_text('cron_job')],
+                    'default': 'log',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#status_log')],
+                    'visible_locator': [self.content_span_text('log')],
+                    'log': {
+                        'menu': self.page.locator('#Span_status_log_tdstatus_log'),
+                        'visible_locator': [self.frame.locator('#_f_level')],
+                        'wait_locator': [self.frame.locator('#_f_level')]},
+                    'system_log': {
+                        'menu': self.page.locator('#Span_status_log_tdadmin_log'),
+                        'visible_locator': [self.frame.locator('#_f_log_remote')],
+                        'wait_locator': [self.frame.locator('#server-grid')]}},
                 'cron_job': {
-                    'menu': self.page.locator('#Span_scheduler_tdscheduler'),
-                    'visible_locator': [self.frame.locator('#schedule-grid')],
-                    'wait_locator': [self.frame.locator('#schedule-grid')]}},
-            'administration_upgrade': {
-                'mouse_move': (200, 0),
-                'menu': [self.administration_menu, self.page.locator('#upgrd')],
-                'visible_locator': [self.content_span_text('upgrade')],
-                'wait_locator': [self.frame.locator('#file')]},
-            'administration_reboot': {
-                'mouse_move': (200, 0),
-                'menu': [self.administration_menu, self.page.locator('#reboot')],
-                'visible_locator': [self.content_span_text('reboot')]},
-            'network_cellular': {
-                'default': 'status',
-                'mouse_move': (200, 0),
-                'menu': [self.network_menu, self.page.locator('#status_wan1')],
-                'visible_locator': [self.content_span_text('cellular')],
-                'status': {
-                    'menu': self.page.locator('#Span_status_wan1_tdstatus_wan1'),
-                    'visible_locator': [self.frame.locator('#b_connect')],
-                    'wait_locator': [self.frame.locator('#b_connect')]},
+                    'default': 'cron_job',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#scheduler')],
+                    'visible_locator': [self.content_span_text('cron_job')],
+                    'cron_job': {
+                        'menu': self.page.locator('#Span_scheduler_tdscheduler'),
+                        'visible_locator': [self.frame.locator('#schedule-grid')],
+                        'wait_locator': [self.frame.locator('#schedule-grid')]}},
+                'upgrade': {
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#upgrd')],
+                    'visible_locator': [self.content_span_text('upgrade')],
+                    'wait_locator': [self.frame.locator('#file')]},
+                'reboot': {
+                    'menu': [self.page.locator('#reboot')],
+                    'visible_locator': [self.content_span_text('reboot')]},
+            },
+            'network': {
+                'default': 'cellular.status',
+                'menu': [self.network_menu],
                 'cellular': {
-                    'menu': self.page.locator('#Span_status_wan1_tdsetup_wan1'),
-                    'visible_locator': [self.frame.locator('#_f_wan1_enable')],
-                    'wait_locator': [self.frame.locator('#_f_wan1_enable')]}},
-            'network_bridge': {
-                'default': 'status',
-                'mouse_move': (200, 0),
-                'menu': [self.network_menu, self.page.locator('#status_eth')],
-                'visible_locator': [self.content_span_text('bridge')],
-                'status': {
-                    'menu': self.page.locator('#Span_status_eth_tdstatus_eth'),
-                    'visible_locator': [self.frame.locator('#br-title')],
-                    'wait_locator': [self.frame.locator('#br-title')]},
+                    'default': 'status',
+                    'mouse_move': (200, 0),
+                    'menu': self.page.locator('#status_wan1'),
+                    'visible_locator': [self.content_span_text('cellular')],
+                    'status': {
+                        'menu': [self.page.locator('#Span_status_wan1_tdstatus_wan1')],
+                        'visible_locator': [self.frame.locator('#b_connect')],
+                        'wait_locator': [self.frame.locator('#b_connect')]},
+                    'cellular': {
+                        'menu': self.page.locator('#Span_status_wan1_tdsetup_wan1'),
+                        'visible_locator': [self.frame.locator('#_f_wan1_enable')],
+                        'wait_locator': [self.frame.locator('#_f_wan1_enable')]}},
                 'bridge': {
-                    'menu': self.page.locator('#Span_status_eth_tdsetup_bridge'),
-                    'visible_locator': [self.frame.locator('#bridge-grid')],
-                    'wait_locator': [self.frame.locator('#bridge-grid')]}},
-            'network_vlan': {
-                'default': 'vlan_trunk',
-                'mouse_move': (200, 0),
-                'menu': [self.network_menu, self.page.locator('#setup_vlan_portmode')],
-                'visible_locator': [self.content_span_text('vlan')],
-                'vlan_trunk': {
-                    'menu': self.page.locator('#Span_setup_vlan_portmode_tdsetup_vlan_portmode'),
-                    'visible_locator': [self.frame.locator('#ifacl-grid')],
-                    'wait_locator': [self.frame.locator('#ifacl-grid')]},
-                'configure_vlan_parameters': {
-                    'menu': self.page.locator('#Span_setup_vlan_portmode_tdsetup_vlan'),
-                    'visible_locator': [self.frame.locator('#vlan-grid')],
-                    'wait_locator': [self.frame.locator('#vlan-grid')]}},
-            'network_adsl_dialup_pppoe': {
-                'default': 'status',
-                'mouse_move': (200, 0),
-                'menu': [self.network_menu, self.page.locator('#status_pppoe')],
-                'visible_locator': [self.content_span_text('adsl')],
-                'status': {
-                    'menu': self.page.locator('#Span_setup_vlan_portmode_tdsetup_vlan_portmode'),
-                    'wait_locator': [self.frame.locator('#refresh-button')]},
-                'adsl_dialup_pppoe': {
-                    'menu': self.page.locator('#Span_status_pppoe_tdsetup_pppoe'),
-                    'visible_locator': [self.frame.locator('#dialpool-grid')],
-                    'wait_locator': [self.frame.locator('#dialpool-grid')]}},
-            'network_wi_fi': {
-                'default': 'status',
-                'mouse_move': (200, 0),
-                'menu': [self.network_menu, self.page.locator('#status_wlan0')],
-                'visible_locator': [self.content_span_text('wifi')],
-                'status': {
-                    'menu': self.page.locator('#Span_status_wlan0_tdstatus_wlan0'),
-                    'visible_locator': [self.frame.locator('#wifi-2g-grid')],
-                    'wait_locator': [self.frame.locator('#wifi-5g-grid')]},
-                'wi_fi_24g': {
-                    'menu': self.page.locator('#Span_status_wlan0_tdsetup_wlan0'),
-                    'wait_locator': [self.frame.locator('#_f_wl0_enable')]},
-                'wi_fi_5g': {
-                    'menu': self.page.locator('#Span_status_wlan0_tdsetup_wlan1'),
-                    'wait_locator': [self.frame.locator('#_f_wl0_enable')]},
-                'advanced': {
-                    'menu': self.page.locator('#Span_status_wlan0_tdsetup_adv_wlan0'),
-                    'visible_locator': [self.frame.locator('#_bridge_mode')],
-                    'wait_locator': [self.frame.locator('#_bridge_mode')]}},
-            'network_bluetooth': {
-                'default': 'bluetooth',
-                'mouse_move': (200, 0),
-                'menu': [self.network_menu, self.page.locator('#setup_bluetooth')],
-                'visible_locator': [self.content_span_text('bluetooth')],
+                    'default': 'status',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#status_eth')],
+                    'visible_locator': [self.content_span_text('bridge')],
+                    'status': {
+                        'menu': self.page.locator('#Span_status_eth_tdstatus_eth'),
+                        'visible_locator': [self.frame.locator('#br-title')],
+                        'wait_locator': [self.frame.locator('#br-title')]},
+                    'bridge': {
+                        'menu': self.page.locator('#Span_status_eth_tdsetup_bridge'),
+                        'visible_locator': [self.frame.locator('#bridge-grid')],
+                        'wait_locator': [self.frame.locator('#bridge-grid')]}},
+                'vlan': {
+                    'default': 'vlan_trunk',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#setup_vlan_portmode')],
+                    'visible_locator': [self.content_span_text('vlan')],
+                    'vlan_trunk': {
+                        'menu': self.page.locator('#Span_setup_vlan_portmode_tdsetup_vlan_portmode'),
+                        'visible_locator': [self.frame.locator('#ifacl-grid')],
+                        'wait_locator': [self.frame.locator('#ifacl-grid')]},
+                    'configure_vlan_parameters': {
+                        'menu': self.page.locator('#Span_setup_vlan_portmode_tdsetup_vlan'),
+                        'visible_locator': [self.frame.locator('#vlan-grid')],
+                        'wait_locator': [self.frame.locator('#vlan-grid')]}},
+                'adsl_dialup(pppoe)': {
+                    'default': 'status',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#status_pppoe')],
+                    'visible_locator': [self.content_span_text('adsl')],
+                    'status': {
+                        'menu': self.page.locator('#Span_status_pppoe_tdstatus_pppoe'),
+                        'wait_locator': [self.frame.locator('#refresh-button')]},
+                    'adsl_dialup(pppoe)': {
+                        'menu': self.page.locator('#Span_status_pppoe_tdsetup_pppoe'),
+                        'visible_locator': [self.frame.locator('#dialpool-grid')],
+                        'wait_locator': [self.frame.locator('#dialpool-grid')]}},
+                'wi_fi': {
+                    'default': 'status',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#status_wlan0')],
+                    'visible_locator': [self.content_span_text('wifi')],
+                    'status': {
+                        'menu': self.page.locator('#Span_status_wlan0_tdstatus_wlan0'),
+                        'visible_locator': [self.frame.locator('#wifi-2g-grid')],
+                        'wait_locator': [self.frame.locator('#wifi-5g-grid')]},
+                    'wi_fi_24g': {
+                        'menu': self.page.locator('#Span_status_wlan0_tdsetup_wlan0'),
+                        'wait_locator': [self.frame.locator('#_f_wl0_enable')]},
+                    'wi_fi_5g': {
+                        'menu': self.page.locator('#Span_status_wlan0_tdsetup_wlan1'),
+                        'wait_locator': [self.frame.locator('#_f_wl0_enable')]},
+                    'advanced': {
+                        'menu': self.page.locator('#Span_status_wlan0_tdsetup_adv_wlan0'),
+                        'visible_locator': [self.frame.locator('#_bridge_mode')],
+                        'wait_locator': [self.frame.locator('#_bridge_mode')]}},
                 'bluetooth': {
-                    'menu': self.page.locator('#Span_setup_bluetooth_tdsetup_bluetooth'),
-                    'visible_locator': [self.frame.locator('#_bluetooth_enable')],
-                    'wait_locator': [self.frame.locator('#_bluetooth_enable')]}},
-            'network_captive_portal': {
-                'default': 'captive_portal',
-                'mouse_move': (200, 0),
-                'menu': [self.network_menu, self.page.locator('#setup_portal_nc')],
-                'visible_locator': [self.content_span_text('captive_')],
+                    'default': 'bluetooth_management',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#setup_bluetooth')],
+                    'visible_locator': [self.content_span_text('bluetooth')],
+                    'bluetooth_management': {
+                        'menu': self.page.locator('#Span_setup_bluetooth_tdsetup_bluetooth'),
+                        'visible_locator': [self.frame.locator('#_bluetooth_enable')],
+                        'wait_locator': [self.frame.locator('#_bluetooth_enable')]}},
                 'captive_portal': {
-                    'menu': self.page.locator('#Span_setup_portal_nc_tdsetup_portal_nc'),
-                    'visible_locator': [self.frame.locator('#_f_enable')],
-                    'wait_locator': [self.frame.locator('#_f_enable')]}},
-            'network_loopback': {
-                'default': 'loopback',
-                'mouse_move': (200, 0),
-                'menu': [self.network_menu, self.page.locator('#setup_lo0')],
-                'visible_locator': [self.content_span_text('look_back')],
+                    'default': 'captive_portal',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#setup_portal_nc')],
+                    'visible_locator': [self.content_span_text('captive_')],
+                    'captive_portal': {
+                        'menu': self.page.locator('#Span_setup_portal_nc_tdsetup_portal_nc'),
+                        'visible_locator': [self.frame.locator('#_f_enable')],
+                        'wait_locator': [self.frame.locator('#_f_enable')]}},
                 'loopback': {
-                    'menu': self.page.locator('#Span_setup_lo0_tdsetup_lo0'),
-                    'visible_locator': [self.frame.locator('#mip-grid')],
-                    'wait_locator': [self.frame.locator('#mip-grid')]}},
-            'network_layer2_switch': {
-                'default': 'status',
-                'mouse_move': (200, 0),
-                'menu': [self.network_menu, self.page.locator('#status_port')],
-                'visible_locator': [self.content_span_text('layer')],
-                'status': {
-                    'menu': self.page.locator('#Span_status_port_tdstatus_port'),
-                    'visible_locator': [self.frame.locator('#intf-grid')],
-                    'wait_locator': [self.frame.locator('#intf-grid')]}},
-            'network_ip_passthrough': {
-                'default': 'ip_passthrough',
-                'mouse_move': (200, 0),
-                'menu': [self.network_menu, self.page.locator('#setup_ippassth')],
-                'visible_locator': [self.content_span_text('ip_passthrough')],
+                    'default': 'loopback',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#setup_lo0')],
+                    'visible_locator': [self.content_span_text('look_back')],
+                    'loopback': {
+                        'menu': self.page.locator('#Span_setup_lo0_tdsetup_lo0'),
+                        'visible_locator': [self.frame.locator('#mip-grid')],
+                        'wait_locator': [self.frame.locator('#mip-grid')]}},
+                'layer2_switch': {
+                    'default': 'status',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#status_port')],
+                    'visible_locator': [self.content_span_text('layer')],
+                    'status': {
+                        'menu': self.page.locator('#Span_status_port_tdstatus_port'),
+                        'visible_locator': [self.frame.locator('#intf-grid')],
+                        'wait_locator': [self.frame.locator('#intf-grid')]}},
                 'ip_passthrough': {
-                    'menu': self.page.locator('#Span_setup_ippassth_tdsetup_ippassth'),
-                    'visible_locator': [self.frame.locator('#_f_ippassth_enable')],
-                    'wait_locator': [self.frame.locator('#_f_ippassth_enable')]}},
-            'services_dhcp': {
-                'default': 'status',
-                'mouse_move': (200, 0),
-                'menu': [self.services_menu, self.page.locator('#status_dhcp')],
-                'visible_locator': [self.content_span_text('dhcp')],
-                'status': {
-                    'menu': self.page.locator('#Span_status_dhcp_tdstatus_dhcp'),
-                    'visible_locator': [self.frame.locator('#dev-grid')],
-                    'wait_locator': [self.frame.locator('#dev-grid')]},
-                'dhcp_server': {
-                    'menu': self.page.locator('#Span_status_dhcp_tdsetup_dhcp'),
-                    'visible_locator': [self.frame.locator('#interface-grid')],
-                    'wait_locator': [self.frame.locator('#interface-grid')]},
-                'dhcp_relay': {
-                    'menu': self.page.locator('#Span_status_dhcp_tdsetup_dhcprelay'),
-                    'visible_locator': [self.frame.locator('#_f_dhcprelay_enable')],
-                    'wait_locator': [self.frame.locator('#_f_dhcprelay_enable')]},
-                'dhcp_client': {
-                    'menu': self.page.locator('#Span_status_dhcp_tdsetup_dhcpc'),
-                    'wait_locator': [self.frame.locator('//table[@class="fields"]')]}},
-            'services_dns': {
-                'default': 'dns_server',
-                'mouse_move': (200, 0),
-                'menu': [self.services_menu, self.page.locator('#setup_dns')],
-                'visible_locator': [self.content_span_text('dns')],
-                'dns_server': {
-                    'menu': self.page.locator('#Span_setup_dns_tdsetup_dns'),
-                    'visible_locator': [self.frame.locator('#_f_dns_1')],
-                    'wait_locator': [self.frame.locator('#_f_dns_1')]},
-                'dns_relay': {
-                    'menu': self.page.locator('#Span_setup_dns_tdsetup_dnsrelay'),
-                    'visible_locator': [self.frame.locator('#_f_dnsrelay_enable')],
-                    'wait_locator': [self.frame.locator('#dnsrelay-grid')]}},
-            'services_ddns': {
-                'default': 'status',
-                'mouse_move': (200, 0),
-                'menu': [self.services_menu, self.page.locator('#status_ddns')],
-                'visible_locator': [self.content_span_text('ddns')],
-                'status': {
-                    'menu': self.page.locator('#Span_status_ddns_tdstatus_ddns'),
-                    'wait_locator': [self.frame.locator('#refresh-button')]},
+                    'default': 'ip_passthrough',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#setup_ippassth')],
+                    'visible_locator': [self.content_span_text('ip_passthrough')],
+                    'ip_passthrough': {
+                        'menu': self.page.locator('#Span_setup_ippassth_tdsetup_ippassth'),
+                        'visible_locator': [self.frame.locator('#_f_ippassth_enable')],
+                        'wait_locator': [self.frame.locator('#_f_ippassth_enable')]}},
+
+            },
+            'services': {
+                'default': 'dhcp.status',
+                'menu': [self.services_menu],
+                'dhcp': {
+                    'default': 'status',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#status_dhcp')],
+                    'visible_locator': [self.content_span_text('dhcp')],
+                    'status': {
+                        'menu': self.page.locator('#Span_status_dhcp_tdstatus_dhcp'),
+                        'visible_locator': [self.frame.locator('#dev-grid')],
+                        'wait_locator': [self.frame.locator('#dev-grid')]},
+                    'dhcp_server': {
+                        'menu': self.page.locator('#Span_status_dhcp_tdsetup_dhcp'),
+                        'visible_locator': [self.frame.locator('#interface-grid')],
+                        'wait_locator': [self.frame.locator('#interface-grid')]},
+                    'dhcp_relay': {
+                        'menu': self.page.locator('#Span_status_dhcp_tdsetup_dhcprelay'),
+                        'visible_locator': [self.frame.locator('#_f_dhcprelay_enable')],
+                        'wait_locator': [self.frame.locator('#_f_dhcprelay_enable')]},
+                    'dhcp_client': {
+                        'menu': self.page.locator('#Span_status_dhcp_tdsetup_dhcpc'),
+                        'wait_locator': [self.frame.locator('//table[@class="fields"]')]}},
+                'dns': {
+                    'default': 'dns_server',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#setup_dns')],
+                    'visible_locator': [self.content_span_text('dns')],
+                    'dns_server': {
+                        'menu': self.page.locator('#Span_setup_dns_tdsetup_dns'),
+                        'visible_locator': [self.frame.locator('#_f_dns_1')],
+                        'wait_locator': [self.frame.locator('#_f_dns_1')]},
+                    'dns_relay': {
+                        'menu': self.page.locator('#Span_setup_dns_tdsetup_dnsrelay'),
+                        'visible_locator': [self.frame.locator('#_f_dnsrelay_enable')],
+                        'wait_locator': [self.frame.locator('#dnsrelay-grid')]}},
                 'ddns': {
-                    'menu': self.page.locator('#Span_status_ddns_tdsetup_ddns'),
-                    'visible_locator': [self.frame.locator('#method-grid')],
-                    'wait_locator': [self.frame.locator('#method-grid')]}},
-            'services_sms': {
-                'default': 'basic',
-                'mouse_move': (200, 0),
-                'menu': [self.services_menu, self.page.locator('#setup_sms_basic')],
-                'visible_locator': [self.content_span_text('sms')],
-                'basic': {
-                    'menu': self.page.locator('#Span_setup_sms_basic_tdsetup_sms_basic'),
-                    'visible_locator': [self.frame.locator('#_f_sms_enable')],
-                    'wait_locator': [self.frame.locator('#_f_sms_enable')]}},
-            'services_gnss': {
-                'default': 'position',
-                'mouse_move': (200, 0),
-                'menu': [self.services_menu, self.page.locator('#status_gps')],
-                'visible_locator': [self.content_span_text('gnss')],
-                'position': {
-                    'menu': self.page.locator('#Span_status_gps_tdstatus_gps'),
-                    'wait_locator': [self.frame.locator('#gps-time-title')]},
-                'gnss_settings': {
-                    'menu': self.page.locator('#Span_status_gps_tdsetup_gps_enable'),
-                    'visible_locator': [self.frame.locator('#_f_enable_gps')],
-                    'wait_locator': [self.frame.locator('#_f_enable_gps')]},
-                'gnss_ip_forwarding': {
-                    'menu': self.page.locator('#Span_status_gps_tdsetup_gps_tcp'),
-                    'visible_locator': [self.frame.locator('#_f_enable_gps')],
-                    'wait_locator': [self.frame.locator('#_f_enable_gps')]},
-                'gnss_serial_forwarding': {
-                    'menu': self.page.locator('#Span_status_gps_tdsetup_gps_serial'),
-                    'visible_locator': [self.frame.locator('#_f_s_enable')],
-                    'wait_locator': [self.frame.locator('#_f_s_enable')]}},
-            'services_qos': {
-                'default': 'traffic_control',
-                'mouse_move': (200, 0),
-                'menu': [self.services_menu, self.page.locator('#setup_traffic')],
-                'visible_locator': [self.content_span_text('qos')],
-                'traffic_control': {
-                    'menu': self.page.locator('#Span_setup_traffic_tdsetup_traffic'),
-                    'visible_locator': [self.frame.locator('#tcl-grid')],
-                    'wait_locator': [self.frame.locator('#tcl-grid')]}},
-            'services_data_usage': {
-                'default': 'status',
-                'mouse_move': (200, 0),
-                'menu': [self.services_menu, self.page.locator('#status_data_usage')],
-                'visible_locator': [self.content_span_text('data_usage')],
-                'status': {
-                    'menu': self.page.locator('#Span_status_data_usage_tdstatus_data_usage'),
-                    'wait_locator': [self.frame.locator('#previous_day_sim1-grid')]},
+                    'default': 'status',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#status_ddns')],
+                    'visible_locator': [self.content_span_text('ddns')],
+                    'status': {
+                        'menu': self.page.locator('#Span_status_ddns_tdstatus_ddns'),
+                        'wait_locator': [self.frame.locator('#refresh-button')]},
+                    'ddns': {
+                        'menu': self.page.locator('#Span_status_ddns_tdsetup_ddns'),
+                        'visible_locator': [self.frame.locator('#method-grid')],
+                        'wait_locator': [self.frame.locator('#method-grid')]}},
+                'sms': {
+                    'default': 'basic',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#setup_sms_basic')],
+                    'visible_locator': [self.content_span_text('sms')],
+                    'basic': {
+                        'menu': self.page.locator('#Span_setup_sms_basic_tdsetup_sms_basic'),
+                        'visible_locator': [self.frame.locator('#_f_sms_enable')],
+                        'wait_locator': [self.frame.locator('#_f_sms_enable')]}},
+                'gnss': {
+                    'default': 'position',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#status_gps')],
+                    'visible_locator': [self.content_span_text('gnss')],
+                    'position': {
+                        'menu': self.page.locator('#Span_status_gps_tdstatus_gps'),
+                        'wait_locator': [self.frame.locator('#gps-time-title')]},
+                    'gnss_settings': {
+                        'menu': self.page.locator('#Span_status_gps_tdsetup_gps_enable'),
+                        'visible_locator': [self.frame.locator('#_f_enable_gps')],
+                        'wait_locator': [self.frame.locator('#_f_enable_gps')]},
+                    'gnss_ip_forwarding': {
+                        'menu': self.page.locator('#Span_status_gps_tdsetup_gps_tcp'),
+                        'visible_locator': [self.frame.locator('#_f_tcp_enable')],
+                        'wait_locator': [self.frame.locator('#_f_tcp_enable')]},
+                    'gnss_serial_forwarding': {
+                        'menu': self.page.locator('#Span_status_gps_tdsetup_gps_serial'),
+                        'visible_locator': [self.frame.locator('#_f_s_enable')],
+                        'wait_locator': [self.frame.locator('#_f_s_enable')]}},
+                'qos': {
+                    'default': 'traffic_control',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#setup_traffic')],
+                    'visible_locator': [self.content_span_text('qos')],
+                    'traffic_control': {
+                        'menu': self.page.locator('#Span_setup_traffic_tdsetup_traffic'),
+                        'visible_locator': [self.frame.locator('#tcl-grid')],
+                        'wait_locator': [self.frame.locator('#tcl-grid')]}},
                 'data_usage': {
-                    'menu': self.page.locator('#Span_status_data_usage_tdsetup_data_usage'),
-                    'visible_locator': [self.frame.locator('#_f_datausage_enable')],
-                    'wait_locator': [self.frame.locator('#_f_datausage_enable')]}},
-            'services_obd': {
-                'default': 'status',
-                'mouse_move': (200, 0),
-                'menu': [self.services_menu, self.page.locator('#status_obd')],
-                'visible_locator': [self.content_span_text('obd')],
-                'status': {
-                    'menu': self.page.locator('#Span_status_obd_tdstatus_obd'),
-                    'wait_locator': [self.frame.locator('#refresh-button')]},
+                    'default': 'status',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#status_data_usage')],
+                    'visible_locator': [self.content_span_text('data_usage')],
+                    'status': {
+                        'menu': self.page.locator('#Span_status_data_usage_tdstatus_data_usage'),
+                        'wait_locator': [self.frame.locator('#previous_day_sim1-grid')]},
+                    'data_usage': {
+                        'menu': self.page.locator('#Span_status_data_usage_tdsetup_data_usage'),
+                        'visible_locator': [self.frame.locator('#_f_datausage_enable')],
+                        'wait_locator': [self.frame.locator('#_f_datausage_enable')]}},
                 'obd': {
-                    'menu': self.page.locator('#Span_status_obd_tdsetup_obd'),
-                    'wait_locator': [self.frame.locator('#obd-status')]}},
-            'services_power_management': {
-                'default': 'power_management',
-                'mouse_move': (200, 0),
-                'menu': [self.services_menu, self.page.locator('#setup_power_management')],
-                'visible_locator': [self.content_span_text('power_management')],
+                    'default': 'status',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#status_obd')],
+                    'visible_locator': [self.content_span_text('obd')],
+                    'status': {
+                        'menu': self.page.locator('#Span_status_obd_tdstatus_obd'),
+                        'wait_locator': [self.frame.locator('#refresh-button')]},
+                    'obd': {
+                        'menu': self.page.locator('#Span_status_obd_tdsetup_obd'),
+                        'wait_locator': [self.frame.locator('#canbus_title')]}},
                 'power_management': {
-                    'menu': self.page.locator('#Span_setup_power_management_tdsetup_power_management'),
-                    'wait_locator': [self.frame.locator('#_f_power_off_voltage')]}},
-            'link_backup_sla': {
-                'default': 'status',
-                'mouse_move': (200, 0),
-                'menu': [self.link_backup_menu, self.page.locator('#status_sla')],
-                'visible_locator': [self.content_span_text('sla')],
-                'status': {
-                    'menu': self.page.locator('#Span_status_sla_tdstatus_sla'),
-                    'visible_locator': [self.frame.locator('#stat_sla-grid')],
-                    'wait_locator': [self.frame.locator('#stat_sla-grid')]},
+                    'default': 'power_management',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#setup_power_management')],
+                    'visible_locator': [self.content_span_text('power_management')],
+                    'power_management': {
+                        'menu': self.page.locator('#Span_setup_power_management_tdsetup_power_management'),
+                        'wait_locator': [self.frame.locator('#_f_power_off_voltage')]}},
+            },
+            'link_backup': {
+                'default': 'sla.status',
+                'menu': [self.link_backup_menu],
                 'sla': {
-                    'menu': self.page.locator('#Span_status_sla_tdsetup_sla'),
-                    'visible_locator': [self.frame.locator('#sla-grid')],
-                    'wait_locator': [self.frame.locator('#sla-grid')]}},
-            'link_backup_track': {
-                'default': 'status',
-                'mouse_move': (200, 0),
-                'menu': [self.link_backup_menu, self.page.locator('#status_track')],
-                'visible_locator': [self.content_span_text('track')],
-                'status': {
-                    'menu': self.page.locator('#Span_status_track_tdstatus_track'),
-                    'visible_locator': [self.frame.locator('#stat_track-grid')],
-                    'wait_locator': [self.frame.locator('#stat_track-grid')]},
+                    'default': 'status',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#status_sla')],
+                    'visible_locator': [self.content_span_text('sla')],
+                    'status': {
+                        'menu': self.page.locator('#Span_status_sla_tdstatus_sla'),
+                        'visible_locator': [self.frame.locator('#stat_sla-grid')],
+                        'wait_locator': [self.frame.locator('#stat_sla-grid')]},
+                    'sla': {
+                        'menu': self.page.locator('#Span_status_sla_tdsetup_sla'),
+                        'visible_locator': [self.frame.locator('#sla-grid')],
+                        'wait_locator': [self.frame.locator('#sla-grid')]}},
                 'track': {
-                    'menu': self.page.locator('#Span_status_track_tdsetup_track'),
-                    'visible_locator': [self.frame.locator('#track-grid')],
-                    'wait_locator': [self.frame.locator('#track-grid')]}},
-            'link_backup_vrrp': {
-                'default': 'status',
-                'mouse_move': (200, 0),
-                'menu': [self.link_backup_menu, self.page.locator('#status_vrrp')],
-                'visible_locator': [self.content_span_text('vrrp')],
-                'status': {
-                    'menu': self.page.locator('#Span_status_vrrp_tdstatus_vrrp'),
-                    'wait_locator': [self.frame.locator('#vrrp-grid')]},
+                    'default': 'status',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#status_track')],
+                    'visible_locator': [self.content_span_text('track')],
+                    'status': {
+                        'menu': self.page.locator('#Span_status_track_tdstatus_track'),
+                        'visible_locator': [self.frame.locator('#stat_track-grid')],
+                        'wait_locator': [self.frame.locator('#stat_track-grid')]},
+                    'track': {
+                        'menu': self.page.locator('#Span_status_track_tdsetup_track'),
+                        'visible_locator': [self.frame.locator('#track-grid')],
+                        'wait_locator': [self.frame.locator('#track-grid')]}},
                 'vrrp': {
-                    'menu': self.page.locator('#Span_status_vrrp_tdsetup_vrrp'),
-                    'wait_locator': [self.frame.locator('#vrrp-grid')]}},
-            'link_backup_interface_backup': {
-                'default': 'status',
-                'mouse_move': (200, 0),
-                'menu': [self.link_backup_menu, self.page.locator('#status_if_backup')],
-                'visible_locator': [self.content_span_text('interface_back')],
-                'status': {
-                    'menu': self.page.locator('#Span_status_if_backup_tdstatus_if_backup'),
-                    'wait_locator': [self.frame.locator('#backup-grid')]},
+                    'default': 'status',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#status_vrrp')],
+                    'visible_locator': [self.content_span_text('vrrp')],
+                    'status': {
+                        'menu': self.page.locator('#Span_status_vrrp_tdstatus_vrrp'),
+                        'wait_locator': [self.frame.locator('#vrrp-grid')]},
+                    'vrrp': {
+                        'menu': self.page.locator('#Span_status_vrrp_tdsetup_vrrp'),
+                        'wait_locator': [self.frame.locator('#vrrp-grid')]}},
                 'interface_backup': {
-                    'menu': self.page.locator('#Span_status_if_backup_tdsetup_if_backup'),
-                    'visible_locator': [self.frame.locator('#backup-grid')],
-                    'wait_locator': [self.frame.locator('#backup-grid')]}},
-            'routing_static_routing': {
-                'default': 'route_table',
-                'mouse_move': (200, 0),
-                'menu': [self.routing_menu, self.page.locator('#status_route')],
-                'visible_locator': [self.content_span_text('static_routing')],
-                'route_table': {
-                    'menu': self.page.locator('#Span_status_route_tdstatus_route'),
-                    'visible_locator': [self.frame.locator('#_state')],
-                    'wait_locator': [self.frame.locator('#statsroute-grid')]},
+                    'default': 'status',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#status_if_backup')],
+                    'visible_locator': [self.content_span_text('interface_back')],
+                    'status': {
+                        'menu': self.page.locator('#Span_status_if_backup_tdstatus_if_backup'),
+                        'wait_locator': [self.frame.locator('#backup-grid')]},
+                    'interface_backup': {
+                        'menu': self.page.locator('#Span_status_if_backup_tdsetup_if_backup'),
+                        'visible_locator': [self.frame.locator('#backup-grid')],
+                        'wait_locator': [self.frame.locator('#backup-grid')]}},
+            },
+            'routing': {
+                'default': 'static_routing.route_table',
+                'menu': [self.routing_menu],
                 'static_routing': {
-                    'menu': self.page.locator('#Span_status_route_tdsetup_static_route'),
-                    'visible_locator': [self.frame.locator('#_f_route_type')],
-                    'wait_locator': [self.frame.locator('#route-grid')]}},
-            'routing_dynamic_routing': {
-                'default': 'route_table',
-                'mouse_move': (200, 0),
-                'menu': [self.routing_menu, self.page.locator('#dyn_status_route')],
-                'visible_locator': [self.content_span_text('dynamic_r')],
-                'route_table': {
-                    'menu': self.page.locator('#Span_dyn_status_route_tddyn_status_route'),
-                    'visible_locator': [self.frame.locator('#_state')],
-                    'wait_locator': [self.frame.locator('#statsroute-grid')]},
-                'rip': {
-                    'menu': self.page.locator('#Span_dyn_status_route_tdsetup_dyn_rip'),
-                    'visible_locator': [self.frame.locator('#_f_rip_enable')],
-                    'wait_locator': [self.frame.locator('#_f_rip_enable')]},
-                'osgf': {
-                    'menu': self.page.locator('#Span_dyn_status_route_tdsetup_dyn_ospf'),
-                    'visible_locator': [self.frame.locator('#_f_ospf_enable')],
-                    'wait_locator': [self.frame.locator('#_f_ospf_enable')]},
-                'bgp': {
-                    'menu': self.page.locator('#Span_dyn_status_route_tdsetup_dyn_bgp'),
-                    'visible_locator': [self.frame.locator('#_f_bgp_enable')],
-                    'wait_locator': [self.frame.locator('#_f_bgp_enable')]},
-                'filtering_route': {
-                    'menu': self.page.locator('#Span_dyn_status_route_tdsetup_dyn_rib'),
-                    'visible_locator': [self.frame.locator('#acl-grid')],
-                    'wait_locator': [self.frame.locator('#acl-grid')]}},
-            'routing_multicast_routing': {
-                'default': 'basic',
-                'mouse_move': (200, 0),
-                'menu': [self.routing_menu, self.page.locator('#setup_mcast_route')],
-                'visible_locator': [self.content_span_text('multicast_r')],
-                'basic': {
-                    'menu': self.page.locator('#Span_setup_mcast_route_tdsetup_mcast_route'),
-                    'visible_locator': [self.frame.locator('#_f_mroute_enable')],
-                    'wait_locator': [self.frame.locator('#mroutetab-grid')]},
-                'igmp': {
-                    'menu': self.page.locator('#Span_setup_mcast_route_tdsetup_mroute_igmp'),
-                    'visible_locator': [self.frame.locator('#_igmpproxy_upstream')],
-                    'wait_locator': [self.frame.locator('#igmpdownstream-grid')]}},
-            'firewall_acl': {
-                'default': 'acl',
-                'mouse_move': (200, 0),
-                'menu': [self.firewall_menu, self.page.locator('#setup_acl')],
-                'visible_locator': [self.content_span_text('acl')],
+                    'default': 'route_table',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#status_route')],
+                    'visible_locator': [self.content_span_text('static_routing')],
+                    'route_table': {
+                        'menu': self.page.locator('#Span_status_route_tdstatus_route'),
+                        'visible_locator': [self.frame.locator('#_state')],
+                        'wait_locator': [self.frame.locator('#statsroute-grid')]},
+                    'static_routing': {
+                        'menu': self.page.locator('#Span_status_route_tdsetup_static_route'),
+                        'visible_locator': [self.frame.locator('#_f_route_type')],
+                        'wait_locator': [self.frame.locator('#route-grid')]}},
+                'dynamic_routing': {
+                    'default': 'route_table',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#dyn_status_route')],
+                    'visible_locator': [self.content_span_text('dynamic_r')],
+                    'route_table': {
+                        'menu': self.page.locator('#Span_dyn_status_route_tddyn_status_route'),
+                        'visible_locator': [self.frame.locator('#_state')],
+                        'wait_locator': [self.frame.locator('#statsroute-grid')]},
+                    'rip': {
+                        'menu': self.page.locator('#Span_dyn_status_route_tdsetup_dyn_rip'),
+                        'visible_locator': [self.frame.locator('#_f_rip_enable')],
+                        'wait_locator': [self.frame.locator('#_f_rip_enable')]},
+                    'ospf': {
+                        'menu': self.page.locator('#Span_dyn_status_route_tdsetup_dyn_ospf'),
+                        'visible_locator': [self.frame.locator('#_f_ospf_enable')],
+                        'wait_locator': [self.frame.locator('#_f_ospf_enable')]},
+                    'bgp': {
+                        'menu': self.page.locator('#Span_dyn_status_route_tdsetup_dyn_bgp'),
+                        'visible_locator': [self.frame.locator('#_f_bgp_enable')],
+                        'wait_locator': [self.frame.locator('#_f_bgp_enable')]},
+                    'filtering_route': {
+                        'menu': self.page.locator('#Span_dyn_status_route_tdsetup_dyn_rib'),
+                        'visible_locator': [self.frame.locator('#prefix-grid')],
+                        'wait_locator': [self.frame.locator('#prefix-grid')]}},
+                'multicast_routing': {
+                    'default': 'basic',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#setup_mcast_route')],
+                    'visible_locator': [self.content_span_text('multicast_r')],
+                    'basic': {
+                        'menu': self.page.locator('#Span_setup_mcast_route_tdsetup_mcast_route'),
+                        'visible_locator': [self.frame.locator('#_f_mroute_enable')],
+                        'wait_locator': [self.frame.locator('#mroutetab-grid')]},
+                    'igmp': {
+                        'menu': self.page.locator('#Span_setup_mcast_route_tdsetup_mroute_igmp'),
+                        'visible_locator': [self.frame.locator('#_igmpproxy_upstream')],
+                        'wait_locator': [self.frame.locator('#igmpdownstream-grid')]}},
+            },
+            'firewall': {
+                'default': 'acl.acl',
+                'menu': [self.firewall_menu],
                 'acl': {
-                    'menu': self.page.locator('#Span_setup_acl_tdsetup_acl'),
-                    'visible_locator': [self.frame.locator('#_f_strict')],
-                    'wait_locator': [self.frame.locator('#acl-grid')]}},
-            'firewall_nat': {
-                'default': 'nat',
-                'mouse_move': (200, 0),
-                'menu': [self.firewall_menu, self.page.locator('#setup_nat')],
-                'visible_locator': [self.content_span_text('nat')],
+                    'default': 'acl',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#setup_acl')],
+                    'visible_locator': [self.content_span_text('acl')],
+                    'acl': {
+                        'menu': self.page.locator('#Span_setup_acl_tdsetup_acl'),
+                        'visible_locator': [self.frame.locator('#interface-grid')],
+                        'wait_locator': [self.frame.locator('#interface-grid')]}},
                 'nat': {
-                    'menu': self.page.locator('#Span_setup_nat_tdsetup_nat'),
-                    'visible_locator': [self.frame.locator('#nat-grid')],
-                    'wait_locator': [self.frame.locator('#nat-grid')]}},
-            'firewall_mac_ip_binding': {
-                'default': 'mac_ip_binding',
-                'mouse_move': (200, 0),
-                'menu': [self.firewall_menu, self.page.locator('#setup_mac_ip_bind')],
-                'visible_locator': [self.content_span_text('mac_ip')],
+                    'default': 'nat',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#setup_nat')],
+                    'visible_locator': [self.content_span_text('nat')],
+                    'nat': {
+                        'menu': self.page.locator('#Span_setup_nat_tdsetup_nat'),
+                        'visible_locator': [self.frame.locator('#nat-grid')],
+                        'wait_locator': [self.frame.locator('#nat-grid')]}},
                 'mac_ip_binding': {
-                    'menu': self.page.locator('#Span_setup_mac_ip_bind_tdsetup_mac_ip_bind'),
-                    'visible_locator': [self.frame.locator('#_f_mac_ip_enable')],
-                    'wait_locator': [self.frame.locator('#_f_mac_ip_enable')]}},
-            'firewall_url_filter': {
-                'default': 'url_filter',
-                'mouse_move': (200, 0),
-                'menu': [self.firewall_menu, self.page.locator('#setup_urlfilter')],
-                'visible_locator': [self.content_span_text('url_filter')],
-                'url_filter': {
-                    'menu': self.page.locator('#Span_setup_urlfilter_tdsetup_urlfilter'),
-                    'visible_locator': [self.frame.locator('#urlfilter-grid')],
-                    'wait_locator': [self.frame.locator('#urlfilter-grid')]}},
-            'firewall_advanced': {
-                'default': 'url_filter',
-                'mouse_move': (200, 0),
-                'menu': [self.firewall_menu, self.page.locator('#setup_fw_adv')],
-                'visible_locator': [self.content_span_text('advanced')],
+                    'default': 'mac_ip_binding',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#setup_mac_ip_bind')],
+                    'visible_locator': [self.content_span_text('mac_ip')],
+                    'mac_ip_binding': {
+                        'menu': self.page.locator('#Span_setup_mac_ip_bind_tdsetup_mac_ip_bind'),
+                        'visible_locator': [self.frame.locator('#_f_mac_ip_enable')],
+                        'wait_locator': [self.frame.locator('#_f_mac_ip_enable')]}},
                 'url_filter': {
-                    'menu': self.page.locator('#Span_setup_fw_adv_tdsetup_fw_adv'),
-                    'visible_locator': [self.frame.locator('#_br_nf_c_ipt')],
-                    'wait_locator': [self.frame.locator('#_br_nf_c_ipt')]}},
-            'vpn_ipsec': {
-                'default': 'status',
-                'mouse_move': (200, 0),
-                'menu': [self.vpn_menu, self.page.locator('#vpn_ipsec_status')],
-                'visible_locator': [self.content_span_text('ipsec')],
-                'status': {
-                    'menu': self.page.locator('#Span_vpn_ipsec_status_tdvpn_ipsec_status'),
-                    'visible_locator': [self.frame.locator('#ike-grid')],
-                    'wait_locator': [self.frame.locator('#ipsec-grid')]},
-                'ipsec_setting': {
-                    'menu': self.page.locator('#Span_vpn_ipsec_status_tdvpn_ipsec_setting'),
-                    'visible_locator': [self.frame.locator('#_f_ipsec_enable')],
-                    'wait_locator': [self.frame.locator('#_f_ipsec_enable')]},
-                'ipsec_extern_setting': {
-                    'menu': self.page.locator('#Span_vpn_ipsec_status_tdvpn_ipsec_extern'),
-                    'visible_locator': [self.frame.locator('#profile-grid')],
-                    'wait_locator': [self.frame.locator('#profile-grid')]}},
-            'vpn_gre': {
-                'default': 'gre',
-                'mouse_move': (200, 0),
-                'menu': [self.vpn_menu, self.page.locator('#vpn_gre')],
-                'visible_locator': [self.content_span_text('gre')],
+                    'default': 'url_filter',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#setup_urlfilter')],
+                    'visible_locator': [self.content_span_text('url_filter')],
+                    'url_filter': {
+                        'menu': self.page.locator('#Span_setup_urlfilter_tdsetup_urlfilter'),
+                        'visible_locator': [self.frame.locator('#urlfilter-grid')],
+                        'wait_locator': [self.frame.locator('#urlfilter-grid')]}},
+                'advanced': {
+                    'default': 'advanced',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#setup_fw_adv')],
+                    'visible_locator': [self.content_span_text('advanced')],
+                    'advanced': {
+                        'menu': self.page.locator('#Span_setup_fw_adv_tdsetup_fw_adv'),
+                        'visible_locator': [self.frame.locator('#_br_nf_c_ipt')],
+                        'wait_locator': [self.frame.locator('#_br_nf_c_ipt')]}},
+            },
+            'vpn': {
+                'default': 'ipsec.status',
+                'menu': [self.vpn_menu],
+                'ipsec': {
+                    'default': 'status',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#vpn_ipsec_status')],
+                    'visible_locator': [self.content_span_text('ipsec')],
+                    'status': {
+                        'menu': self.page.locator('#Span_vpn_ipsec_status_tdvpn_ipsec_status'),
+                        'visible_locator': [self.frame.locator('#ike-grid')],
+                        'wait_locator': [self.frame.locator('#ipsec-grid')]},
+                    'ipsec_setting': {
+                        'menu': self.page.locator('#Span_vpn_ipsec_status_tdvpn_ipsec_setting'),
+                        'visible_locator': [self.frame.locator('#_f_ipsec_enable')],
+                        'wait_locator': [self.frame.locator('#_f_ipsec_enable')]},
+                    'ipsec_extern_setting': {
+                        'menu': self.page.locator('#Span_vpn_ipsec_status_tdvpn_ipsec_extern'),
+                        'visible_locator': [self.frame.locator('#profile-grid')],
+                        'wait_locator': [self.frame.locator('#profile-grid')]}},
                 'gre': {
-                    'menu': self.page.locator('#Span_vpn_gre_tdvpn_gre'),
-                    'visible_locator': [self.frame.locator('#gre-grid')],
-                    'wait_locator': [self.frame.locator('#gre-grid')]}},
-            'vpn_l2tp': {
-                'default': 'status',
-                'mouse_move': (200, 0),
-                'menu': [self.vpn_menu, self.page.locator('#status_l2tp')],
-                'visible_locator': [self.content_span_text('l2tp')],
-                'status': {
-                    'menu': self.page.locator('#Span_status_l2tp_tdstatus_l2tp'),
-                    'visible_locator': [self.frame.locator('#stat_l2tp-grid')],
-                    'wait_locator': [self.frame.locator('#stat_l2tp-grid')]},
-                'l2tp_client': {
-                    'menu': self.page.locator('#Span_status_l2tp_tdvpn_l2tpc'),
-                    'visible_locator': [self.frame.locator('#l2tpclass-grid')],
-                    'wait_locator': [self.frame.locator('#l2tpclass-grid')]},
-                'l2tp_server': {
-                    'menu': self.page.locator('#Span_status_l2tp_tdvpn_l2tps'),
-                    'visible_locator': [self.frame.locator('#_f_l2tps_enable')],
-                    'wait_locator': [self.frame.locator('#_f_l2tps_enable')]}},
-            'vpn_openvpn': {
-                'default': 'status',
-                'mouse_move': (200, 0),
-                'menu': [self.vpn_menu, self.page.locator('#status_openvpn')],
-                'visible_locator': [self.content_span_text('openvpn')],
-                'status': {
-                    'menu': self.page.locator('#Span_status_openvpn_tdstatus_openvpn'),
-                    'visible_locator': [self.frame.locator('#stat_openvpn-grid')],
-                    'wait_locator': [self.frame.locator('#stat_openvpn-grid')]},
-                'openvpn_client': {
-                    'menu': self.page.locator('#Span_status_openvpn_tdopenvpn_client'),
-                    'visible_locator': [self.frame.locator('#l2tpclass-grid')],
-                    'wait_locator': [self.frame.locator('#openvpn-client-grid')]},
-                'openvpn_server': {
-                    'menu': self.page.locator('#Span_status_openvpn_tdopenvpn_server'),
-                    'visible_locator': [self.frame.locator('#_f_openvpn_enable')],
-                    'wait_locator': [self.frame.locator('#_f_openvpn_enable')]}},
-            'vpn_certificate_management': {
-                'default': 'certificate_management',
-                'mouse_move': (200, 0),
-                'menu': [self.vpn_menu, self.page.locator('#vpn_cert')],
-                'visible_locator': [self.content_span_text('certificate')],
+                    'default': 'gre',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#vpn_gre')],
+                    'visible_locator': [self.content_span_text('gre')],
+                    'gre': {
+                        'menu': self.page.locator('#Span_vpn_gre_tdvpn_gre'),
+                        'visible_locator': [self.frame.locator('#gre-grid')],
+                        'wait_locator': [self.frame.locator('#gre-grid')]}},
+                'l2tp': {
+                    'default': 'status',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#status_l2tp')],
+                    'visible_locator': [self.content_span_text('l2tp')],
+                    'status': {
+                        'menu': self.page.locator('#Span_status_l2tp_tdstatus_l2tp'),
+                        'visible_locator': [self.frame.locator('#stat_l2tp-grid')],
+                        'wait_locator': [self.frame.locator('#stat_l2tp-grid')]},
+                    'l2tp_client': {
+                        'menu': self.page.locator('#Span_status_l2tp_tdvpn_l2tpc'),
+                        'visible_locator': [self.frame.locator('#l2tpclass-grid')],
+                        'wait_locator': [self.frame.locator('#l2tpclass-grid')]},
+                    'l2tp_server': {
+                        'menu': self.page.locator('#Span_status_l2tp_tdvpn_l2tps'),
+                        'visible_locator': [self.frame.locator('#_f_l2tps_enable')],
+                        'wait_locator': [self.frame.locator('#_f_l2tps_enable')]}},
+                'openvpn': {
+                    'default': 'status',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#status_openvpn')],
+                    'visible_locator': [self.content_span_text('openvpn')],
+                    'status': {
+                        'menu': self.page.locator('#Span_status_openvpn_tdstatus_openvpn'),
+                        'visible_locator': [self.frame.locator('#stat_openvpn-grid')],
+                        'wait_locator': [self.frame.locator('#stat_openvpn-grid')]},
+                    'openvpn_client': {
+                        'menu': self.page.locator('#Span_status_openvpn_tdopenvpn_client'),
+                        'visible_locator': [self.frame.locator('#l2tpclass-grid')],
+                        'wait_locator': [self.frame.locator('#openvpn-client-grid')]},
+                    'openvpn_server': {
+                        'menu': self.page.locator('#Span_status_openvpn_tdopenvpn_server'),
+                        'visible_locator': [self.frame.locator('#_f_openvpn_enable')],
+                        'wait_locator': [self.frame.locator('#_f_openvpn_enable')]}},
                 'certificate_management': {
-                    'menu': self.page.locator('#Span_vpn_cert_tdvpn_cert'),
-                    'visible_locator': [self.frame.locator('#_f_scep_enable')],
-                    'wait_locator': [self.frame.locator('#_f_scep_enable')]},
-                'root_ca': {
-                    'menu': self.page.locator('#Span_vpn_cert_tdvpn_rootca'),
-                    'visible_locator': [self.frame.locator('#ca-import-button')],
-                    'wait_locator': [self.frame.locator('#rootca-grid')]}},
-
-            'app_app': {
-                'default': 'status',
-                'mouse_move': (200, 0),
-                'menu': [self.app_menu, self.page.locator('#status_python_sdk')],
-                'visible_locator': [self.content_span_text('app')],
-                'status': {
-                    'menu': self.page.locator('#Span_status_python_sdk_tdstatus_python_sdk'),
-                    'wait_locator': [self.frame.locator('#pypp-stat-grid')]},
-                'app_management': {
-                    'menu': self.page.locator('#Span_status_python_sdk_tdsetup_python_install'),
-                    'visible_locator': [self.frame.locator('#_f_python_enable')],
-                    'wait_locator': [self.frame.locator('#pyapp-grid')]}},
-            'app_docker': {
-                'default': 'docker_management',
-                'mouse_move': (200, 0),
-                'menu': [self.app_menu, self.page.locator('#status_docker')],
-                'visible_locator': [self.content_span_text('docker')],
-                'docker_management': {
-                    'menu': self.page.locator('#Span_status_docker_tdstatus_docker'),
-                    'visible_locator': [self.frame.locator('#_dk_enable')],
-                    'wait_locator': [self.frame.locator('#docker_log')]}},
-            'app_third_party_platform': {
-                'default': 'status',
-                'mouse_move': (200, 0),
-                'menu': [self.app_menu, self.page.locator('#status_3rd')],
-                'visible_locator': [self.content_span_text('third_party')],
-                'status': {
-                    'menu': self.page.locator('#Span_status_3rd_tdstatus_3rd'),
-                    'wait_locator': [self.frame.locator('#tcp-title')]},
-                'mqtt': {
-                    'menu': self.page.locator('#Span_status_3rd_tdsetup_3rd_party_platform_mqtt'),
-                    'wait_locator': [self.frame.locator('#_third_enable')]},
-                'tcp_udp': {
-                    'menu': self.page.locator('#Span_status_3rd_tdsetup_3rd_party_platform_tcp'),
-                    'wait_locator': [self.frame.locator('#_third_enable')]}},
-            'app_local_mqtt_broker': {
-                'default': 'local_mqtt_broker',
-                'mouse_move': (200, 0),
-                'menu': [self.app_menu, self.page.locator('#setup_local_mqtt_broker')],
-                'visible_locator': [self.content_span_text('local_mqtt')],
+                    'default': 'certificate_management',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#vpn_cert')],
+                    'visible_locator': [self.content_span_text('certificate')],
+                    'certificate_management': {
+                        'menu': self.page.locator('#Span_vpn_cert_tdvpn_cert'),
+                        'visible_locator': [self.frame.locator('#_f_scep_enable')],
+                        'wait_locator': [self.frame.locator('#_f_scep_enable')]},
+                    'root_ca': {
+                        'menu': self.page.locator('#Span_vpn_cert_tdvpn_rootca'),
+                        'visible_locator': [self.frame.locator('#ca-import-button')],
+                        'wait_locator': [self.frame.locator('#rootca-grid')]}},
+            },
+            'app': {
+                'default': 'app.status',
+                'menu': [self.app_menu],
+                'app': {
+                    'default': 'status',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#status_python_sdk')],
+                    'visible_locator': [self.content_span_text('app')],
+                    'status': {
+                        'menu': self.page.locator('#Span_status_python_sdk_tdstatus_python_sdk'),
+                        'wait_locator': [self.frame.locator('#pypp-stat-grid')]},
+                    'app_management': {
+                        'menu': self.page.locator('#Span_status_python_sdk_tdsetup_python_install'),
+                        'visible_locator': [self.frame.locator('#_f_python_enable')],
+                        'wait_locator': [self.frame.locator('#pyapp-grid')]}},
+                'docker': {
+                    'default': 'docker_management',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#status_docker')],
+                    'visible_locator': [self.content_span_text('docker')],
+                    'docker_management': {
+                        'menu': self.page.locator('#Span_status_docker_tdstatus_docker'),
+                        'visible_locator': [self.frame.locator('#_dk_enable')],
+                        'wait_locator': [self.frame.locator('#docker_log')]}},
+                'third_party_platform': {
+                    'default': 'status',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#status_3rd')],
+                    'visible_locator': [self.content_span_text('third_party')],
+                    'status': {
+                        'menu': self.page.locator('#Span_status_3rd_tdstatus_3rd'),
+                        'wait_locator': [self.frame.locator('#tcp-title')]},
+                    'mqtt': {
+                        'menu': self.page.locator('#Span_status_3rd_tdsetup_3rd_party_platform_mqtt'),
+                        'wait_locator': [self.frame.locator('#_third_enable')]},
+                    'tcp/udp': {
+                        'menu': self.page.locator('#Span_status_3rd_tdsetup_3rd_party_platform_tcp'),
+                        'wait_locator': [self.frame.locator('#_third_enable')]}},
                 'local_mqtt_broker': {
-                    'menu': self.page.locator('#Span_setup_local_mqtt_broker_tdsetup_local_mqtt_broker'),
-                    'visible_locator': [self.frame.locator('#_local_broker_enable')],
-                    'wait_locator': [self.frame.locator('#_local_broker_enable')]}},
-            'app_rest_api': {
-                'default': 'rest_api_management',
-                'mouse_move': (200, 0),
-                'menu': [self.app_menu, self.page.locator('#setup_restapi')],
-                'visible_locator': [self.content_span_text('rest_api')],
-                'rest_api_management': {
-                    'menu': self.page.locator('#Span_setup_restapi_tdsetup_restapi'),
-                    'visible_locator': [self.frame.locator('#_restapi_mode')],
-                    'wait_locator': [self.frame.locator('#_restapi_mode')]}},
-            'app_azure_iot_edge': {
-                'default': 'azure_iot_edge_management',
-                'mouse_move': (200, 0),
-                'menu': [self.app_menu, self.page.locator('#setup_azure_iotedge')],
-                'visible_locator': [self.content_span_text('azure_iot')],
-                'azure_iot_edge_management': {
-                    'menu': self.page.locator('#Span_setup_azure_iotedge_tdsetup_azure_iotedge_mgmt'),
-                    'visible_locator': [self.frame.locator('#_azure_iotedge_enable')],
-                    'wait_locator': [self.frame.locator('#conf_export')]}},
-            'app_user_data': {
-                'default': 'status',
-                'mouse_move': (200, 0),
-                'menu': [self.app_menu, self.page.locator('#status_user_data')],
-                'visible_locator': [self.content_span_text('user_data')],
-                'status': {
-                    'menu': self.page.locator('#Span_status_user_data_tdstatus_user_data'),
-                    'wait_locator': [self.frame.locator('#userdata-grid')]},
-                'user_data_management': {
-                    'menu': self.page.locator('#Span_status_user_data_tdsetup_user_data'),
-                    'wait_locator': [self.frame.locator('#userdata-grid')]}},
-            'industrial_dtu': {
-                'default': 'serial_port',
-                'mouse_move': (200, 0),
-                'menu': [self.industrial_menu, self.page.locator('#setup_serial')],
-                'visible_locator': [self.content_span_text('dtu')],
-                'serial_port': {
-                    'menu': self.page.locator('#Span_setup_serial_tdsetup_serial'),
-                    'wait_locator': [self.frame.locator('#serial1_title')]},
-                'dtu_1': {
-                    'menu': self.page.locator('#Span_setup_serial_tdsetup_dtu1'),
-                    'wait_locator': [self.frame.locator('#_f_dtu_enable')]},
-                'dtu_2': {
-                    'menu': self.page.locator('#Span_setup_serial_tdsetup_dtu2'),
-                    'wait_locator': [self.frame.locator('#_f_dtu_enable')]}},
-            'industrial_io': {
-                'default': 'status',
-                'mouse_move': (200, 0),
-                'menu': [self.industrial_menu, self.page.locator('#status_serial_io')],
-                'visible_locator': [self.content_span_text('io')],
-                'status': {
-                    'menu': self.page.locator('#Span_status_serial_io_tdstatus_serial_io'),
-                    'wait_locator': [self.frame.locator('#io-title')]},
-                'io_control': {
-                    'menu': self.page.locator('#Span_status_serial_io_tdsetup_serial_io_vg9'),
-                    'wait_locator': [self.frame.locator('#_digital_input_up1')]}},
-            'industrial_1_wire': {
-                'default': 'status',
-                'mouse_move': (200, 0),
-                'menu': [self.industrial_menu, self.page.locator('#status_1wire')],
-                'visible_locator': [self.content_span_text('1_wire')],
-                'status': {
-                    'menu': self.page.locator('#Span_status_1wire_tdstatus_1wire'),
-                    'wait_locator': [self.frame.locator('#onewire-section')]}},
-            'tools_ping': {
-                'default': 'ping',
-                'mouse_move': (200, 0),
-                'menu': [self.tools_menu, self.page.locator('#tools_ping')],
-                'visible_locator': [self.content_span_text('ping')],
+                    'default': 'local_mqtt_broker_management',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#setup_local_mqtt_broker')],
+                    'visible_locator': [self.content_span_text('local_mqtt')],
+                    'local_mqtt_broker_management': {
+                        'menu': self.page.locator('#Span_setup_local_mqtt_broker_tdsetup_local_mqtt_broker'),
+                        'visible_locator': [self.frame.locator('#_local_broker_enable')],
+                        'wait_locator': [self.frame.locator('#_local_broker_enable')]}},
+                'rest_api': {
+                    'default': 'rest_api_management',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#setup_restapi')],
+                    'visible_locator': [self.content_span_text('rest_api')],
+                    'rest_api_management': {
+                        'menu': self.page.locator('#Span_setup_restapi_tdsetup_restapi'),
+                        'visible_locator': [self.frame.locator('#_restapi_mode')],
+                        'wait_locator': [self.frame.locator('#_restapi_mode')]}},
+                'azure_iot_edge': {
+                    'default': 'azure_iot_edge_management',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#setup_azure_iotedge')],
+                    'visible_locator': [self.content_span_text('azure_iot')],
+                    'azure_iot_edge_management': {
+                        'menu': self.page.locator('#Span_setup_azure_iotedge_tdsetup_azure_iotedge_mgmt'),
+                        'visible_locator': [self.frame.locator('#_azure_iotedge_enable')],
+                        'wait_locator': [self.frame.locator('#conf_export')]}},
+                'user_data': {
+                    'default': 'status',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#status_user_data')],
+                    'visible_locator': [self.content_span_text('user_data')],
+                    'status': {
+                        'menu': self.page.locator('#Span_status_user_data_tdstatus_user_data'),
+                        'wait_locator': [self.frame.locator('#userdata-grid')]},
+                    'user_data_management': {
+                        'menu': self.page.locator('#Span_status_user_data_tdsetup_user_data'),
+                        'wait_locator': [self.frame.locator('#userdata-grid')]}},
+            },
+            'industrial': {
+                'default': 'dtu.serial_port',
+                'menu': [self.industrial_menu],
+                'dtu': {
+                    'default': 'serial_port',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#setup_serial')],
+                    'visible_locator': [self.content_span_text('dtu')],
+                    'serial_port': {
+                        'menu': self.page.locator('#Span_setup_serial_tdsetup_serial'),
+                        'wait_locator': [self.frame.locator('#serial1_title')]},
+                    'dtu_1': {
+                        'menu': self.page.locator('#Span_setup_serial_tdsetup_dtu1'),
+                        'wait_locator': [self.frame.locator('#_f_dtu_enable')]},
+                    'dtu_2': {
+                        'menu': self.page.locator('#Span_setup_serial_tdsetup_dtu2'),
+                        'wait_locator': [self.frame.locator('#_f_dtu_enable')]},
+                    'dtu_3': {
+                        'menu': self.page.locator('#Span_setup_serial_tdsetup_dtu3'),
+                        'wait_locator': [self.frame.locator('#_f_dtu_enable')]}
+                },
+                'io': {
+                    'default': 'status',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#status_serial_io')],
+                    'visible_locator': [self.content_span_text('io')],
+                    'status': {
+                        'menu': self.page.locator('#Span_status_serial_io_tdstatus_serial_io'),
+                        'wait_locator': [self.frame.locator('#io-title')]},
+                    'i/o_control': {
+                        'menu': self.page.locator('#Span_status_serial_io_tdsetup_serial_io_vg9'),
+                        'wait_locator': [self.frame.locator('#_digital_input_up1')]}},
+                '1_wire': {
+                    'default': 'status',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#status_1wire')],
+                    'visible_locator': [self.content_span_text('1_wire')],
+                    'status': {
+                        'menu': self.page.locator('#Span_status_1wire_tdstatus_1wire'),
+                        'wait_locator': [self.frame.locator('#onewire-section')]}},
+            },
+            'tools': {
+                'default': 'ping.ping',
+                'menu': [self.tools_menu],
                 'ping': {
-                    'menu': self.page.locator('#Span_tools_ping_tdtools_ping'),
-                    'visible_locator': [self.frame.locator('#_f_addr')],
-                    'wait_locator': [self.frame.locator('#_f_addr')]}},
-            'tools_traceroute': {
-                'default': 'traceroute',
-                'mouse_move': (200, 0),
-                'menu': [self.tools_menu, self.page.locator('#tools_trace')],
-                'visible_locator': [self.content_span_text('traceroute')],
+                    'default': 'ping',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#tools_ping')],
+                    'visible_locator': [self.content_span_text('ping')],
+                    'ping': {
+                        'menu': self.page.locator('#Span_tools_ping_tdtools_ping'),
+                        'visible_locator': [self.frame.locator('#_f_addr')],
+                        'wait_locator': [self.frame.locator('#_f_addr')]}},
                 'traceroute': {
-                    'menu': self.page.locator('#Span_tools_trace_tdtools_trace'),
-                    'visible_locator': [self.frame.locator('#_f_addr')],
-                    'wait_locator': [self.frame.locator('#_f_addr')]}},
-            'tools_tcpdump': {
-                'default': 'tcpdump',
-                'mouse_move': (200, 0),
-                'menu': [self.tools_menu, self.page.locator('#tools_tcpdump')],
-                'visible_locator': [self.content_span_text('tcpdump')],
+                    'default': 'traceroute',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#tools_trace')],
+                    'visible_locator': [self.content_span_text('traceroute')],
+                    'traceroute': {
+                        'menu': self.page.locator('#Span_tools_trace_tdtools_trace'),
+                        'visible_locator': [self.frame.locator('#_f_addr')],
+                        'wait_locator': [self.frame.locator('#_f_addr')]}},
                 'tcpdump': {
-                    'menu': self.page.locator('#Span_tools_tcpdump_tdtools_tcpdump'),
-                    'visible_locator': [self.frame.locator('#_f_iface')],
-                    'wait_locator': [self.frame.locator('#_f_iface')]}},
-            'tools_link_speed_test': {
-                'default': 'link_speed_test',
-                'mouse_move': (200, 0),
-                'menu': [self.tools_menu, self.page.locator('#tools_tcpdump')],
-                'visible_locator': [self.content_span_text('link_speed')],
+                    'default': 'tcpdump',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#tools_tcpdump')],
+                    'visible_locator': [self.content_span_text('tcpdump')],
+                    'tcpdump': {
+                        'menu': self.page.locator('#Span_tools_tcpdump_tdtools_tcpdump'),
+                        'visible_locator': [self.frame.locator('#_f_iface')],
+                        'wait_locator': [self.frame.locator('#_f_iface')]}},
                 'link_speed_test': {
-                    'menu': self.page.locator('#Span_tools_speed_tdtools_speed'),
-                    'visible_locator': [self.frame.locator('#speed-up-button')],
-                    'wait_locator': [self.frame.locator('#speed-up-button')]}},
-            'wizards_new_lan': {
-                'default': 'new_lan',
-                'mouse_move': (200, 0),
-                'menu': [self.wizards_menu, self.page.locator('#wizards_lan')],
-                'visible_locator': [self.content_span_text('new_lan')],
+                    'default': 'link_speed_test',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#tools_speed')],
+                    'visible_locator': [self.content_span_text('link_speed')],
+                    'link_speed_test': {
+                        'menu': self.page.locator('#Span_tools_speed_tdtools_speed'),
+                        'visible_locator': [self.frame.locator('#speed-up-button')],
+                        'wait_locator': [self.frame.locator('#speed-up-button')]}},
+
+            },
+            'wizards': {
+                'default': 'new_lan.new_lan',
+                'menu': [self.wizards_menu],
                 'new_lan': {
-                    'menu': self.page.locator('#Span_wizards_lan_tdwizards_lan'),
-                    'visible_locator': [self.frame.locator('#_f_iface')],
-                    'wait_locator': [self.frame.locator('#_f_iface')]}},
-            'wizards_new_wan': {
-                'default': 'new_wan',
-                'mouse_move': (200, 0),
-                'menu': [self.wizards_menu, self.page.locator('#wizards_wan0')],
-                'visible_locator': [self.content_span_text('new_wan')],
+                    'default': 'new_lan',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#wizards_lan')],
+                    'visible_locator': [self.content_span_text('new_lan')],
+                    'new_lan': {
+                        'menu': self.page.locator('#Span_wizards_lan_tdwizards_lan'),
+                        'visible_locator': [self.frame.locator('#_f_iface')],
+                        'wait_locator': [self.frame.locator('#_f_iface')]}},
                 'new_wan': {
-                    'menu': self.page.locator('#Span_wizards_wan0_tdwizards_wan0'),
-                    'visible_locator': [self.frame.locator('#_f_iface')],
-                    'wait_locator': [self.frame.locator('#_f_iface')]}},
-            'wizards_new_cellular': {
-                'default': 'new_cellular',
-                'mouse_move': (200, 0),
-                'menu': [self.wizards_menu, self.page.locator('#wizards_wan1')],
-                'visible_locator': [self.content_span_text('new_cellular')],
+                    'default': 'new_wan',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#wizards_wan0')],
+                    'visible_locator': [self.content_span_text('new_wan')],
+                    'new_wan': {
+                        'menu': self.page.locator('#Span_wizards_wan0_tdwizards_wan0'),
+                        'visible_locator': [self.frame.locator('#_f_iface')],
+                        'wait_locator': [self.frame.locator('#_f_iface')]}},
                 'new_cellular': {
-                    'menu': self.page.locator('#Span_wizards_wan1_tdwizards_wan1'),
-                    'visible_locator': [self.frame.locator('#_wan1_ppp_para')],
-                    'wait_locator': [self.frame.locator('#_wan1_ppp_para')]}},
-            'wizards_new_ipsec_tunnel': {
-                'default': 'new_ipsec_tunnel',
-                'mouse_move': (200, 0),
-                'menu': [self.wizards_menu, self.page.locator('#wizards_ipsec')],
-                'visible_locator': [self.content_span_text('new_ipsec_tunnel')],
+                    'default': 'new_cellular',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#wizards_wan1')],
+                    'visible_locator': [self.content_span_text('new_cellular')],
+                    'new_cellular': {
+                        'menu': self.page.locator('#Span_wizards_wan1_tdwizards_wan1'),
+                        'visible_locator': [self.frame.locator('#_wan1_ppp_para')],
+                        'wait_locator': [self.frame.locator('#_wan1_ppp_para')]}},
                 'new_ipsec_tunnel': {
-                    'menu': self.page.locator('#Span_wizards_ipsec_tdwizards_ipsec'),
-                    'visible_locator': [self.frame.locator('#_f_tunnel_id')],
-                    'wait_locator': [self.frame.locator('#_f_tunnel_id')]}},
-            'wizards_ipsec_expert_config': {
-                'default': 'ipsec_expert_config',
-                'mouse_move': (200, 0),
-                'menu': [self.wizards_menu, self.page.locator('#wizards_ipsec_expert_conf')],
-                'visible_locator': [self.content_span_text('ipsec_expert')],
+                    'default': 'new_ipsec_tunnel',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#wizards_ipsec')],
+                    'visible_locator': [self.content_span_text('new_ipsec_tunnel')],
+                    'new_ipsec_tunnel': {
+                        'menu': self.page.locator('#Span_wizards_ipsec_tdwizards_ipsec'),
+                        'visible_locator': [self.frame.locator('#_f_tunnel_id')],
+                        'wait_locator': [self.frame.locator('#_f_tunnel_id')]}},
                 'ipsec_expert_config': {
-                    'menu': self.page.locator('#Span_wizards_ipsec_expert_conf_tdwizards_ipsec_expert_conf'),
-                    'visible_locator': [self.frame.locator('#secrets_import')],
-                    'wait_locator': [self.frame.locator('#secrets_import')]}},
-            'wizards_new_l2tpv2_tunnel': {
-                'default': 'new_l2tpv2_tunnel',
-                'mouse_move': (200, 0),
-                'menu': [self.wizards_menu, self.page.locator('#wizards_l2tp')],
-                'visible_locator': [self.content_span_text('l2tpv2')],
+                    'default': 'ipsec_expert_config',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#wizards_ipsec_expert_conf')],
+                    'visible_locator': [self.content_span_text('ipsec_expert')],
+                    'ipsec_expert_config': {
+                        'menu': self.page.locator('#Span_wizards_ipsec_expert_conf_tdwizards_ipsec_expert_conf'),
+                        'visible_locator': [self.frame.locator('#secrets_import')],
+                        'wait_locator': [self.frame.locator('#secrets_import')]}},
                 'new_l2tpv2_tunnel': {
-                    'menu': self.page.locator('#Span_wizards_l2tp_tdwizards_l2tp'),
-                    'visible_locator': [self.frame.locator('#_f_tunnel_id')],
-                    'wait_locator': [self.frame.locator('#_f_tunnel_id')]}},
-            'wizards_new_port_mapping': {
-                'default': 'new_port_mapping',
-                'mouse_move': (200, 0),
-                'menu': [self.wizards_menu, self.page.locator('#wizards_portmapping')],
-                'visible_locator': [self.content_span_text('new_port_m')],
+                    'default': 'new_l2tpv2_tunnel',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#wizards_l2tp')],
+                    'visible_locator': [self.content_span_text('l2tpv2')],
+                    'new_l2tpv2_tunnel': {
+                        'menu': self.page.locator('#Span_wizards_l2tp_tdwizards_l2tp'),
+                        'visible_locator': [self.frame.locator('#_f_tunnel_id')],
+                        'wait_locator': [self.frame.locator('#_f_tunnel_id')]}},
                 'new_port_mapping': {
-                    'menu': self.page.locator('#Span_wizards_portmapping_tdwizards_portmapping'),
-                    'visible_locator': [self.frame.locator('#_f_proto')],
-                    'wait_locator': [self.frame.locator('#_f_proto')]},
-
+                    'default': 'new_port_mapping',
+                    'mouse_move': (200, 0),
+                    'menu': [self.page.locator('#wizards_portmapping')],
+                    'visible_locator': [self.content_span_text('new_port_m')],
+                    'new_port_mapping': {
+                        'menu': self.page.locator('#Span_wizards_portmapping_tdwizards_portmapping'),
+                        'visible_locator': [self.frame.locator('#_f_proto')],
+                        'wait_locator': [self.frame.locator('#_f_proto')]}},
             }}
```

### Comparing `inhandtest-0.0.42/inhandtest/base_page/base_page.py` & `inhandtest-0.0.43/inhandtest/base_page/base_page.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,62 +11,59 @@
 from os import path
 from inhandtest.base_page._ig902_contents_locators import IGContentsLocators
 from typing import List
 from inhandtest.exception import ModelError
 from inhandtest.tools import loop_inspector
 from playwright.sync_api import Page, Locator, expect, TimeoutError, sync_playwright
 from inhandtest.base_page._vg710_contents_locators import VGContentsLocators
+from inhandtest.base_page._ir3XX_contents_locators import Ir3XXContentsLocators
 from inhandtest.base_page.table_tr import Table
 import allure
 import logging
 import re
 
 
 class BasePage:
 
-    def __init__(self, host: str, username: str, password: str, protocol='https', page: Page = None,
-                 port=443, model='VG710', language='en', **kwargs):
+    def __init__(self, host: str, username: str, password: str, protocol='https',
+                 port=443, model='VG710', language='en',  page: Page = None, **kwargs):
         """
 
         :param host:  设备主机地址
         :param username: 用户名
         :param password: 密码
         :param protocol: 协议
         :param port: 端口
-        :param model: 'VG710'|'ER805'|'ER605'|'IR302'|'IG502'|'IG902'
+        :param model: 'VG710'|'ER805'|'ER605'|'IR302'|'IG502'|'IG902'|'IR305'|'IR615'
         :param page: 当page为None时，自动打开浏览器及页面，否则使用传入的page
         :param kwargs:
                       browser: 当没有传入page时，可以选择浏览器
-                      dialog_massages: dict
-                      tip_messages: dict
-                      text_messages: dict
-                      title_messages: dict
+                      locale: dict 国际化
         """
         self.page = page
         self.host = host
         self.model = model.upper()
         self.protocol = protocol
         self.port = port
         self.__username = username
         self.__password = password
         self.language = language
         self.__browser_type = kwargs.get('browser')
-        self.__http_credentials_model = ('VG710', )   # 需要使用http认证的设备, 没有登录页面 只有登录弹窗
+        self.__http_credentials_model = ('VG710',)  # 需要使用http认证的设备, 没有登录页面 只有登录弹窗
         if self.__browser_type is None:
             self.__new_page()
         if self.model == 'VG710':
             self.content_locator = VGContentsLocators(self.page, language).tags_menu
         elif self.model == 'IG902':
             self.content_locator = IGContentsLocators(self.page, language).tags_menu
+        elif self.model in ('IR302', 'IR305', 'IR615'):
+            self.content_locator = Ir3XXContentsLocators(self.page, language).tags_menu
         else:
             raise ModelError(f'not support this mode {model}')
-        self.__dialog_massages = kwargs.get('dialog_massages')
-        self.__tip_messages = kwargs.get('tip_messages')
-        self.__text_messages = kwargs.get('text_messages')
-        self.__title_messages = kwargs.get('title_messages')
+        self.locale = kwargs.get('locale').get(language) if kwargs.get('locale') else None
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
 
@@ -80,15 +77,15 @@
                     'wait_locator': self.page.locator('.inStarCloud')}
         elif self.model in ('IG902', 'IG502'):
             return {'username': self.page.locator('#username'), 'password': self.page.locator('#password'),
                     'submit': self.page.locator('//button[@type="submit"]'),
                     'wait_locator': self.page.locator('#logo')}
         elif self.model == 'IR302':
             return {'username': self.page.locator('#username'), 'password': self.page.locator('#passwd'),
-                    'submit': self.page.locator('.login_button"]'),
+                    'submit': self.page.locator('.login_button'),
                     'wait_locator': self.page.locator('#logo')}
         else:
             raise Exception(f'not support this model {self.model}')
 
     def __new_page(self):
         def dialog_(dialog):
             logging.info(f'dialog message is {dialog.message}, accepted')
@@ -185,62 +182,65 @@
         return response_info.value.json()
 
     @allure.step('进入菜单{menu}')
     def access_menu(self, menu: str, wait_time=None) -> None:
         """进入菜单，多个菜单使用点号隔开，不限多少层级   menu_locator 存放在 base_locators 里面，
             定义menu = {'system': {'locator': '#menu_id', 'wait_locator': '#wait_locator_id'},
                                'status':{'locator': '#status_id', 'wait_locator': '#wait_locator_id'}}
+            定义菜单时所有菜单的点号都需要省略，如2.4g 写成24g；空格写成下划线，如wi-fi 2.4g 写成wi-fi_24g
+            中划线写成下划线，如wi-fi-2.4g 写成wi_fi_24g
 
-        :param menu: 'system'| 'system.status'
+
+        :param menu: 'system'| 'system.status' 菜单名称全部来自与设备的英文版本，点号需要省略不写， 其他不变，大小写均可以
+                     菜单中原有的点号都需要忽略，如wi-fi 2.4g 需要传入wi-fi_24g 或 wi-fi 2.4g 或 wi-fi_2.4g
         :param wait_time: 当操作完菜单后是否需要等待时间 单位毫秒
         :return:
         """
 
-        def access(menu_one: str, locators: dict):
+        def access(menu_one: str, locators: dict, level: int):
             visible = False
             if locators.get(menu_one).get('visible_locator'):
                 visible = True
                 for visible_locator in locators.get(menu_one).get('visible_locator'):
                     if not visible_locator.is_visible():
                         visible = False
                         break
                 else:
                     self.page.wait_for_timeout(500)  # 当元素可见时也再多等待500ms
             if not visible:
                 menus = locators.get(menu_one).get('menu') if isinstance(locators.get(menu_one).get('menu'),
                                                                          list) else [locators.get(menu_one).get('menu')]
                 for menu_1 in menus:
                     self.click(menu_1)
-                logging.info(f'select menu {menu_one}')
+                logging.info(f'select {level} level menu {menu_one}')
                 if locators.get(menu_one).get('mouse_move'):
                     self.page.mouse.move(locators.get(menu_one).get('mouse_move')[0],
                                          locators.get(menu_one).get('mouse_move')[1])
                 if locators.get(menu_one).get('wait_locator'):
                     for wait_locator in locators.get(menu_one).get('wait_locator'):
-                        logging.info(wait_locator)
                         wait_locator.wait_for(state='visible')
-                        logging.info(wait_locator.is_visible())
                     self.page.wait_for_timeout(500)  # 多等500ms
 
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
+                menu = menu.replace(' ', '_').replace('-', '_').lower()
                 menu = default_change(menu, self.content_locator).split('.')
                 content_locator_ = self.content_locator
-                for menu_ in menu:
-                    access(menu_, content_locator_)
+                for menu_, level in zip(menu, range(1, len(menu)+1)):
+                    access(menu_, content_locator_, level)
                     content_locator_ = content_locator_.get(menu_)
             except Exception:
                 raise f'not support this menu {menu}'
             if wait_time:
                 self.page.wait_for_timeout(wait_time)
 
     @allure.step('{log_desc} 输入{value}')
@@ -251,14 +251,15 @@
 
         :param value: 输入的值
         :param log_desc: 功能描述，用英文 如 Static Routing Destination
         :param force: 强制写入
         :return:
         """
         if value is not None:
+            locator.clear()
             locator.fill(str(value), force=force)
             locator.blur()  # 鼠标移出输入框
             if log_desc:
                 logging.info(f'Device {self.host} fill {log_desc} {value}')
 
     @allure.step('点击 {log_desc}')
     def click(self, locator: Locator, log_desc=None, dialog_message: str = None, tip_messages: str or list = None,
@@ -497,15 +498,15 @@
         :param f:  是一个操作函数，执行后会有dialog弹窗出现
         :param message: 校验的信息, 支持模糊匹配
         :return:
         """
         if message:
             with self.page.expect_event('dialog') as dialog_info:
                 f()
-            assert self.__dialog_massages.get(message) in dialog_info.value.message, \
+            assert self.locale.get(message) in dialog_info.value.message, \
                 f'{self.host} assert {message} dialog error'
 
     @allure.step("校验tip messages")
     def tip_messages(self, messages: str or list = None, timeout=30) -> None:
         """ 某些提交操作会出现文本的提示，提示在过几秒钟后会消失，对于该类消息的验证使用该方法，
             使用时需要在base_locator tip_messages 且返回字典数据
 
@@ -514,42 +515,42 @@
                             该项校验 页面元素必须停留时间1秒及更多时间，否则不容易检测到导致报错
         :param timeout: 校验超时时间
         :return:
         """
         if messages:
             tip_messages = [messages] if isinstance(messages, str) else messages
             for message in tip_messages:
-                message = self.__tip_messages.get(message)  # 国际化转换
+                message = self.locale.get(message)  # 国际化转换
                 expect(self.page.get_by_text(re.compile(message, re.IGNORECASE))).to_be_visible(timeout=timeout * 1000)
                 expect(self.page.get_by_text(re.compile(message, re.IGNORECASE))).to_be_hidden(timeout=timeout * 1000)
 
     @allure.step("校验text messages")
     def text_messages(self, messages: str or list = None, timeout=10) -> None:
         """ 对文本内容做验证，如在输入框输入错误内容时出现的文本，该类文本会一直存在
         :param messages: str or list 文本内容，如果有多个，使用列表传入
         :param timeout: 校验超时时间
         :return:
         """
         if messages:
             text_messages = [messages] if isinstance(messages, str) else messages
             for message in text_messages:
-                message = self.__text_messages.get(message)  # 国际化转换
+                message = self.locale.get(message)  # 国际化转换
                 expect(self.page.get_by_text(re.compile(message, re.IGNORECASE))).to_be_visible(timeout=timeout * 1000)
 
     @allure.step("校验元素Title")
     def title_messages(self, messages: str or list = None, timeout=10) -> None:
         """ 对元素的属性title做内容验证，
         :param messages: str or list 文本内容，如果有多个，使用列表传入
         :param timeout: 校验超时时间
         :return:
         """
         if messages:
             text_messages = [messages] if isinstance(messages, str) else messages
             for message in text_messages:
-                message = self.__title_messages.get(message)  # 国际化转换
+                message = self.locale.get(message)  # 国际化转换
                 expect(self.page.get_by_title(re.compile(message, re.IGNORECASE))).to_be_visible(timeout=timeout * 1000)
 
     @allure.step('设置页面翻页')
     def page_refresh(self, refresh_time: str, select_locator: Locator) -> None:
         """
         :param refresh_time: str
                         '0'|'3'|'4'|'5'|'10'|'15'|'30'|'60'|'120'|'180'|'240'|'300'|'600'|'900'|'1200'|'1800'
@@ -600,28 +601,27 @@
                 :param locators:  列表 嵌套 长度为2的元组，元组的第一项为操作项名称， 第二项为对应的一个字典
                     [($param1, {"locator": $locator1, "type": $type1, "relation": [($param2, $value2)], "param": {$key1: $value1}}),
                     ($param2, {"locator": $locator2, "type": $type2, "relation": [($param3, $value3),……], "param": {$key2: $value2}}),
                     ($param3, {"locator": $locator2, "type": 'table_tr', "relation": [($param3, $value3),……], "param": {$key2: $value2},
                                 "columns": list, 'unique_columns': list}),]
                     $param: 操作项的名称，如 'language'|'sim'|'status'
                     $locator: 操作项的元素定位， locator or [locator,locator,...]
-                    $type: 操作项的类型 fill|select|select_label|select_index|button|check|upload_file|download_file|text_visible|error_tips|locators_title|
-                                     multi_select|multi_select_label|multi_select_index|multi_check|multi_fill|table_tr,
-                            select|select_label|select_index: select选择不同的选择方式，以_连接，不拼接则默认为 'value'
-                            multi_select指一个参数有多个select,支持multi_select_label|multi_select_index, multi_check同理,
-                                        对应操作项的多个locator及value用[]传入
+                    $type: 操作项的类型 fill|select|button|check|upload_file|download_file|text_visible|error_tips|locators_title|
+                                     multi_select|multi_check|multi_fill|table_tr,
+                            select value值可以是label|Value
+                            multi_select指一个参数有多个select, 对应操作项的多个locator及value用[]传入
                     "relation":[($param, $value)]: 操作项的关联项，若有多个则首个为最先操作的关联项，其中$param为关联项的名称，$value为关联项的预期值
                     "param":{$key, $value}: 参数转换，如大小写转换{"ab":"AB"} {"wan":"Wan"}等.
                 :param action_dict: 要做操作的参数名称与对应的值{$param1: $value1, $param2: $value2}
                 :return:
                 """
         relations = []
 
         def operation(param, param_locator, value):
-            if param_locator.get('type') == 'fill':
+            if param_locator.get('type') == 'text':
                 self.fill(param_locator.get('locator'), value, param)
             elif param_locator.get('type') == 'select':
                 if param_locator.get('param') and value in param_locator.get('param').keys():
                     value = param_locator.get('param').get(value)
                 self.select_option(param_locator.get('locator'), value, param)
             elif param_locator.get('type') == 'button':
                 if value:
@@ -750,14 +750,54 @@
                     except TypeError:
                         logging.info(f'get inner_text failed')
                         return False
                 else:
                     raise KeyError(f'not support the key {key}')
         return True
 
+    @allure.step("获取页面元素文本值")
+    def get_text(self, keys: str or list or tuple, locators: list) -> str or dict or None:
+        """获取页面元素文本值
+
+        :param keys: None or str or list or tuple, 需要获取对应文本的元素的关键字
+        :param locators: [($param1, {"locator": $locator1, "type": $type1}),
+                         type: 支持的类型有：'text'|'fill'|'select'
+                         该select 为select标签的文本值， ER805 和ER605 直接使用text
+        :return: 当key为None时，返回None
+                 当key为str时，只能获取某一个字段的信息，同时使用str返回
+                 当key为列表或者元组时， 使用字典返回相关关键字的信息
+        """
+        result = {}
+        if keys:
+            keys = [keys] if isinstance(keys, str) else keys
+            for key in keys:
+                filter_key = list(filter(lambda x: x[0] == key, locators))
+                if len(filter_key) == 1:
+                    option = filter_key[0]
+                    locator = option[1].get('locator')
+                    if locator.count() != 0:
+                        if option[1].get('type') == 'select':
+                            value = locator.first.text_content()
+                        elif option[1].get('type') == 'fill':
+                            value = locator.first.input_value()
+                        else:
+                            value = locator.first.inner_text()
+                    else:
+                        raise
+                    result[key] = value
+                else:
+                    raise KeyError(f'not support the key {key}')
+        if result:
+            if len(result.keys()) == 1:
+                return result.get(keys[0])
+            else:
+                return result
+        else:
+            return None
+
     @allure.step("PC Ping")
     @loop_inspector('PC Ping', timeout=120, interval=10)
     def pc_ping(self, host_or_ip: str or list or tuple = 'www.baidu.com', number: int = 4, src=None,
                 lost_packets=False, assert_result=True) -> bool:
         """ 验证在PC机上ping某个地址是否丢包， 仅判断丢包
 
         :param lost_packets:
@@ -777,23 +817,23 @@
                 if assert_result:
                     result = os.popen(command).read()
                     logging.info(result)
                     if lost_packets:  # 判断需要丢包
                         send = re.findall(r'已发送 = (.*?)，', result, re.S)[0]
                         accept = re.findall(r'已接收 = (.*?)，', result, re.S)[0]
                         if send == accept:
-                            if '无法访问目标主机' not in result:
+                            if '无法访问' not in result:
                                 logging.info(f'PC {src} ping {host} does not loss packet')
                                 tag_result = False
                     else:  # 判断不丢包
                         if '丢失 = 0' not in result:
                             logging.info(f'PC {src} ping {host} loss packet')
                             tag_result = False
                         else:
-                            if '无法访问目标主机' in result:
+                            if '无法访问' in result:
                                 logging.info(f'PC {src} ping {host} loss packet')
                                 tag_result = False
                 else:
                     os.popen(command)
                 if not tag_result:
                     break
         return tag_result
@@ -804,21 +844,28 @@
             self.__browser.close()
             self.__playwright.stop()
 
 
 if __name__ == '__main__':
     logging.basicConfig(format='%(asctime)s %(levelname)s %(message)s', level=logging.INFO,
                         stream=sys.stdout)
-    with BasePage('10.5.24.96', 'adm', '123456', model='IG902') as my_page:
-        my_page.access_menu('system.system_network_tools')
-        my_page.page.wait_for_timeout(5 * 1000)
+    with BasePage('10.5.47.197', 'adm', '123456', 'https', 443, model='vg710') as my_page:
+        system = ('link speed test', )
+        my_page.access_menu(f'wizards.new port mapping')
+        my_page.page.wait_for_timeout(2 * 1000)
+        # a = my_page.get_text('language', [('language', {'locator': my_page.page.frame_locator('#window_content').locator('#_f_hostname'), 'type': 'fill'})])
+        # print(a)
+    # with BasePage('10.5.24.96', 'adm', '123456', model='IG902') as my_page:
+    #     my_page.access_menu('edge_computing.device_supervisor.measure_monitor')
+    #     my_page.page.wait_for_timeout(1000)
+    #     my_page.access_menu('edge_computing.device_supervisor.protocol')
+    #     my_page.page.wait_for_timeout(1000)
         # user_table = Table(
         #     [('mode', 'input'), ('status', 'input'), ('ssid', 'input'),  ('mac', 'input'),
         #      ('auth', 'input'), ('encry', 'input'), ('network', 'input'), ('gateway', 'input'), ('dns', 'input'), ('time', 'input')],
         #     my_base.page.frame_locator('#window_content').locator('#wifi-2g-grid'),
         #     ['mode', 'status', 'ssid', 'mac', 'auth', 'encry', 'network', 'gateway', 'dns', 'time'], None)
         # a = user_table.exists([{'mode': "'${value}'!='AP'", 'ssid': 'inhand-visitor-2g'}])
         # print(a)
         # print(user_table.exist(locale={'disable': 'Disabled'}, mode="'${value}'!='AP'", ssid='inhand-visitor-2g', status='disable'))
         # user_table.delete(name='test2', value='222')
         # my_base.page.wait_for_timeout(5 * 1000)
-
```

### Comparing `inhandtest-0.0.42/inhandtest/base_page/table_tr.py` & `inhandtest-0.0.43/inhandtest/base_page/table_tr.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         self.table_locator = table_locator
         self.unique_columns = unique_columns  # 重复列名
         self.tr = self.table_locator.locator('//tbody').locator('//tr')
         self.locale = locale
         self.log_desc = log_desc
 
     def __filter_td_index(self, contain_check=False, **kwargs):
+        self.table_locator.wait_for(state='visible')
         expect_result = []
         for input_key, input_value in kwargs.items():
             if not contain_check:
                 result = list(filter(lambda a: a[0] == input_key and a[1] != 'check' and a[0] in self.unique_columns,
                                      self.columns))  # 排除掉check
             else:
                 result = list(filter(lambda a: a[0] == input_key, self.columns))
@@ -45,14 +46,15 @@
                 expect_result.append((self.columns.index(result[0]), input_value, result[0][1]))  # 找出td是第几个，也及值
         return expect_result
 
     def __edit_add(self, **kwargs):
         for column in self.__filter_td_index(True, **kwargs):
             if column[1] is not None:
                 if column[2] == 'input':
+                    self.tr.locator('//td').locator(f'.fi{column[0] + 1}').first.clear()
                     self.tr.locator('//td').locator(f'.fi{column[0] + 1}').first.fill(str(column[1]))
                 elif column[2] == 'select':
                     option = self.locale.get(
                         column[1]) if self.locale and self.locale.get(
                         column[1]) else str(column[1])
                     self.tr.locator('//td').locator(f'.fi{column[0] + 1}').first.select_option(option)
                 elif column[2] == 'check':
@@ -108,15 +110,17 @@
     def add(self, **kwargs) -> None:
         """ add 前是不查找是否存在的，直接加
         :param kwargs str, 待添加列 及对应值
         :return:
         """
         self.__edit_add(**kwargs)
         for i in range(0, self.tr.get_by_role('button').count()):
-            if 'onAdd()' in self.tr.get_by_role('button').nth(i).get_attribute('onclick') and self.tr.get_by_role(
+            action_attribute = self.tr.get_by_role('button').nth(i).get_attribute('onclick')
+            if action_attribute in (
+                'TGO(this).onAdd()', 'TGO(this).footerAdd()', 'footerAdd()') and self.tr.get_by_role(
                     'button').nth(i).is_enabled():
                 self.tr.get_by_role('button').nth(i).click()
                 if self.log_desc is not None:
                     logging.info(f'add table {self.log_desc} success')
                 break
 
     def delete(self, **kwargs) -> None:
@@ -125,15 +129,15 @@
         :return:
         """
         find_tr = self.exist(find_one=True, **kwargs)
         if find_tr is not None:
             self.tr.nth(find_tr).locator('//td').nth(0).click()
             for i in range(0, self.tr.get_by_role('button').count()):
                 action_attribute = self.tr.get_by_role('button').nth(i).get_attribute('onclick')
-                if action_attribute in ("TGO(this).onDelete()", "TGO(this).footerDel()"):
+                if action_attribute in ("TGO(this).onDelete()", "TGO(this).footerDel()", "footerDel()", 'delete_save(this)'):
                     if not self.tr.get_by_role('button').nth(i).is_disabled():
                         self.tr.get_by_role('button').nth(i).click()
                         if self.log_desc is not None:
                             logging.info(f'delete table {self.log_desc} success')
                         break
                     else:
                         logging.error(f'the data in the row {find_tr} cannot be deleted')
@@ -143,22 +147,22 @@
     def delete_all(self) -> None:
         nth = 1
         while self.tr.count() >= nth + 2:
             self.tr.nth(nth).locator('//td').nth(0).click()
             try:
                 for i in range(0, self.tr.get_by_role('button').count()):
                     action_attribute = self.tr.get_by_role('button').nth(i).get_attribute('onclick')
-                    if action_attribute in ("TGO(this).onDelete()", "TGO(this).footerDel()"):
+                    if action_attribute in ("TGO(this).onDelete()", "TGO(this).footerDel()", 'footerDel()', 'delete_save(this)'):
                         if not self.tr.get_by_role('button').nth(i).is_disabled():
                             self.tr.get_by_role('button').nth(i).click()
                             break
                         else:
-                            raise TimeoutError      # 第一行的数据不能删除，走到第二行去
+                            raise TimeoutError  # 第一行的数据不能删除，走到第二行去
                 else:
-                    break     # 所有行都走完了却没有删除按钮，也需要退出去
+                    break  # 所有行都走完了却没有删除按钮，也需要退出去
             except TimeoutError:
                 nth = nth + 1
         logging.info('table resource all delete')
 
     def edit(self, old: dict, new: dict) -> None:
         """
         :param old ,dict, 待变更列数据
@@ -166,15 +170,18 @@
         :return:
         """
         find_tr = self.exist(find_one=True, **old)
         if find_tr is not None:
             self.tr.nth(find_tr).locator('//td').nth(0).click()
             self.__edit_add(**new)
             for i in range(0, self.tr.get_by_role('button').count()):
-                if 'onOK()' in self.tr.get_by_role('button').nth(i).get_attribute('onclick') and self.tr.get_by_role(
+                action_attribute = self.tr.get_by_role('button').nth(i).get_attribute('onclick')
+
+                if action_attribute in ("TGO(this).onOK()", "TGO(this).footerOK()", 'footerOK()', 'footerModify()',
+                                        "TGO(this).footerModify()",) and self.tr.get_by_role(
                         'button').nth(i).is_enabled():
                     self.tr.get_by_role('button').nth(i).click()
                     if self.log_desc is not None:
                         logging.info(f'edit table {self.log_desc} success')
                     break
         else:
             logging.warning(f'not found the resource {old}')
```

### Comparing `inhandtest-0.0.42/inhandtest/exception.py` & `inhandtest-0.0.43/inhandtest/exception.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.42/inhandtest/file.py` & `inhandtest-0.0.43/inhandtest/file.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.42/inhandtest/inmodbus.py` & `inhandtest-0.0.43/inhandtest/inmodbus.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.42/inhandtest/inmongodb.py` & `inhandtest-0.0.43/inhandtest/inmongodb.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.42/inhandtest/inmqtt.py` & `inhandtest-0.0.43/inhandtest/inmqtt.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.42/inhandtest/inrequest.py` & `inhandtest-0.0.43/inhandtest/inrequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,34 +62,40 @@
                                        version: 固件版本
                                        hwVersion: 硬件版本 'V1.0'
                                        bootVersion:  Bootloader版本  '1.1.3.r4956'
                                        sn: 序列号
                                        address
                                        id: 设备id
                                        name: 设备名字
+                                       ip: 设备连接平台的ip地址
+                                       protocol: 设备连接平台的协议
+                                       config_sync: 设备配置同步状态
         :param sn: 列表
         :return: [{'sn': $sn, 'online': 1, 'iccid': '', 'imei'}]
         """
         result = []
         for sn_ in sn:
             response = self.api.send_request('api/devices', method='get',
                                              param={"verbose": 100, "limit": 10, "cursor": 0,
                                                     'serial_number': sn_}).json()
             if response.get('total') == 1:
                 res = response.get('result')[0]
+                config_sync = res.get('config').get('sync') if res.get('config') else None
                 result.append(
                     {'sn': sn_, 'online': res.get('online'), 'iccid': res.get('info').get('iccid'),
                      'imei': res.get('info').get('imei'), 'imsi': res.get('info').get('imsi'),
                      'version': res.get('info').get('swVersion'), 'hwVersion': res.get('info').get('hwVersion'),
                      'bootVersion': res.get('info').get('bootVersion'), 'address': res.get('address'),
-                     'id': res.get('_id'), 'name': res.get('name')})
+                     'id': res.get('_id'), 'name': res.get('name'), 'ip': res.get('pubIp'),
+                     'protocol': res.get('protocol'), 'config_sync': config_sync})
             else:
                 result.append(
                     {'sn': sn_, 'online': None, 'iccid': None, 'imei': None, 'imsi': None, 'version': None,
-                     'hwVersion': None, 'bootVersion': None, 'address': None, 'id': None, 'name': None})
+                     'hwVersion': None, 'bootVersion': None, 'address': None, 'id': None, 'name': None, 'ip': None,
+                     'protocol': None, 'config_sync': None})
         return result
 
     def add_device(self, sn: str) -> None:
         """添加设备，
 
         :param sn: 设备序列号
         :return:
@@ -115,14 +121,17 @@
                         imei:
                         imsi:
                         version: 固件版本
                         hwVersion: 硬件版本 'V1.0'
                         bootVersion:  Bootloader版本  '1.1.3.r4956'
                         sn: 序列号
                         address
+                        ip: 设备连接平台的ip地址
+                        protocol: 设备连接平台的协议 ex: 'mqtt' or 'ovdp'
+                        config_sync: 设备配置同步状态 ex: 2  同成功
         :param timeout: 校验信息，最大超时时间
         :param interval: 校验信息，校验间隔时间
         :return: True or False
         """
         if state:
 
             for i in range(0, timeout, interval):
```

### Comparing `inhandtest-0.0.42/inhandtest/inserial.py` & `inhandtest-0.0.43/inhandtest/inserial.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.42/inhandtest/insocket.py` & `inhandtest-0.0.43/inhandtest/insocket.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.42/inhandtest/inssh.py` & `inhandtest-0.0.43/inhandtest/inssh.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.42/inhandtest/ip.py` & `inhandtest-0.0.43/inhandtest/ip.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.42/inhandtest/mail.py` & `inhandtest-0.0.43/inhandtest/mail.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     kill_windows_port(render.get('host'), [port, port + 1])  # port+1 是https端口
     # 启动本地服务，分享报告
     p = subprocess.Popen(f'npx anywhere -h {render.get("host")} -p {port}', cwd=render.get('allure_results_path'),
                          shell=True,
                          stdout=subprocess.PIPE, stderr=subprocess.STDOUT, encoding='gbk')
     while True:
         output = p.stdout.readline()
-        print(output)
+        logging.info(output)
         if len(re.findall(r'Running at (.*)/', output)) < 1:  # 无论是否启动成功，都会退出循环
             break
     # 读取报告中的summary.json文件，获取测试结果
     summary = json.load(
         open(os.path.join(render.get('allure_results_path'), 'widgets', 'summary.json'), 'r', encoding='utf-8'))
     html_file_path = os.path.join(os.path.dirname(__file__), 'pytest_email.html')
     from emails.template import JinjaTemplate as Te
@@ -63,15 +63,15 @@
     render.update({'report_url': f'http://{render.get("host")}:{port}'})
     # 发送邮件
     if mail_to:
         r = message.send(mail_to, smtp={'host': 'smtp.exmail.qq.com', 'port': 465, 'user': mail_from[0], 'ssl': True,
                                         'password': mail_from[1]},
                          render=render)
         assert r.status_code == 250, 'send email failed'
-        print(f'send {mail_to} test result success!')
+        logging.info(f'send {mail_to} test result success!')
 
 
 @loop_inspector('receive last email', 120, 5)
 def receive_last_mail(receiver: tuple, mail_from: tuple, subject: str, **kwargs):
     """收取符合条件的邮件做校验，如果匹配到多个邮件，只校验最近的一封邮件
        当邮箱中邮件较多时，会耗时很长，所以建议匹配未读的邮件进行分析，分析完后，将邮件标记为已读
```

### Comparing `inhandtest-0.0.42/inhandtest/pytest_email.html` & `inhandtest-0.0.43/inhandtest/pytest_email.html`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.42/inhandtest/telnet.py` & `inhandtest-0.0.43/inhandtest/telnet.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.42/inhandtest/tools.py` & `inhandtest-0.0.43/inhandtest/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,14 +229,15 @@
             except (psutil.NoSuchProcess, psutil.AccessDenied, psutil.ZombieProcess):
                 continue
             for conn in conn_list:
                 if conn.status == psutil.CONN_LISTEN and conn.laddr.port == one_port:
                     logging.info(f"process {proc.pid} already use port {one_port}")
                     # 终止进程
                     proc.kill()
+                    logging.info(f"kill process {proc.pid} success")
 
     [kill_one_port(port_) for port_ in port] if isinstance(port, list) else kill_one_port(port)
 
 
 def windows_cmd(command: str or list, expect: str or list or dict = None, last_read_replace: dict = None):
     """输入一条或多条命令, 且支持对执行时最后一条命令返回的结果做断言
```

### Comparing `inhandtest-0.0.42/setup.py` & `inhandtest-0.0.43/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 setup
 
 """
 from distutils.core import setup
 
 setup(
     name='inhandtest',
-    version='0.0.42',
+    version='0.0.43',
     author='liwei',
     author_email='liwei@inhand.com.cn',
     description='inhand test tools, so easy',
     maintainer='liwei',
     maintainer_email='liwei@inhand.com.cn',
     # py_modules=['inhandtest.tools', 'inhandtest.telnet', 'inhandtest.inmodbus', 'inhandtest.inmqtt', 'inhandtest.file',
     #             'inhandtest.inrequest', 'inhandtest.inssh', 'inhandtest.base_page'],
```

