# Comparing `tmp/rustack-esu-0.1.8.tar.gz` & `tmp/rustack-esu-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rustack-esu-0.1.8.tar", last modified: Tue Feb 14 07:43:46 2023, max compression
+gzip compressed data, was "rustack-esu-0.1.9.tar", last modified: Mon Mar 13 09:30:19 2023, max compression
```

## Comparing `rustack-esu-0.1.8.tar` & `rustack-esu-0.1.9.tar`

### file list

```diff
@@ -1,38 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 07:43:46.394266 rustack-esu-0.1.8/
--rwxr-xr-x   0 runner    (1001) docker     (122)     1067 2023-02-14 07:43:39.000000 rustack-esu-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     4203 2023-02-14 07:43:46.394266 rustack-esu-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2428 2023-02-14 07:43:39.000000 rustack-esu-0.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 07:43:46.390266 rustack-esu-0.1.8/esu/
--rwxr-xr-x   0 runner    (1001) docker     (122)      715 2023-02-14 07:43:39.000000 rustack-esu-0.1.8/esu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5487 2023-02-14 07:43:39.000000 rustack-esu-0.1.8/esu/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1887 2023-02-14 07:43:39.000000 rustack-esu-0.1.8/esu/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3947 2023-02-14 07:43:39.000000 rustack-esu-0.1.8/esu/disk.py
--rw-r--r--   0 runner    (1001) docker     (122)     3179 2023-02-14 07:43:39.000000 rustack-esu-0.1.8/esu/dns.py
--rw-r--r--   0 runner    (1001) docker     (122)     3635 2023-02-14 07:43:39.000000 rustack-esu-0.1.8/esu/dns_record.py
--rw-r--r--   0 runner    (1001) docker     (122)     3489 2023-02-14 07:43:39.000000 rustack-esu-0.1.8/esu/firewall_template.py
--rw-r--r--   0 runner    (1001) docker     (122)     3992 2023-02-14 07:43:39.000000 rustack-esu-0.1.8/esu/firewall_template_rule.py
--rw-r--r--   0 runner    (1001) docker     (122)      315 2023-02-14 07:43:39.000000 rustack-esu-0.1.8/esu/hypervisor.py
--rw-r--r--   0 runner    (1001) docker     (122)     4237 2023-02-14 07:43:39.000000 rustack-esu-0.1.8/esu/lbaas.py
--rw-r--r--   0 runner    (1001) docker     (122)     4499 2023-02-14 07:43:39.000000 rustack-esu-0.1.8/esu/lbaas_pool.py
--rw-r--r--   0 runner    (1001) docker     (122)      336 2023-02-14 07:43:39.000000 rustack-esu-0.1.8/esu/lbaas_pool_member.py
--rw-r--r--   0 runner    (1001) docker     (122)     2741 2023-02-14 07:43:39.000000 rustack-esu-0.1.8/esu/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     4102 2023-02-14 07:43:39.000000 rustack-esu-0.1.8/esu/network.py
--rw-r--r--   0 runner    (1001) docker     (122)     5349 2023-02-14 07:43:39.000000 rustack-esu-0.1.8/esu/port.py
--rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-02-14 07:43:39.000000 rustack-esu-0.1.8/esu/project.py
--rw-r--r--   0 runner    (1001) docker     (122)     4190 2023-02-14 07:43:39.000000 rustack-esu-0.1.8/esu/router.py
--rw-r--r--   0 runner    (1001) docker     (122)     3130 2023-02-14 07:43:39.000000 rustack-esu-0.1.8/esu/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (122)     1249 2023-02-14 07:43:39.000000 rustack-esu-0.1.8/esu/storage_profile.py
--rw-r--r--   0 runner    (1001) docker     (122)      574 2023-02-14 07:43:39.000000 rustack-esu-0.1.8/esu/subnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     2080 2023-02-14 07:43:39.000000 rustack-esu-0.1.8/esu/template.py
--rw-r--r--   0 runner    (1001) docker     (122)      841 2023-02-14 07:43:39.000000 rustack-esu-0.1.8/esu/template_field.py
--rw-r--r--   0 runner    (1001) docker     (122)     8131 2023-02-14 07:43:39.000000 rustack-esu-0.1.8/esu/vdc.py
--rw-r--r--   0 runner    (1001) docker     (122)     8924 2023-02-14 07:43:39.000000 rustack-esu-0.1.8/esu/vm.py
--rw-r--r--   0 runner    (1001) docker     (122)      342 2023-02-14 07:43:39.000000 rustack-esu-0.1.8/esu/vm_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 07:43:46.390266 rustack-esu-0.1.8/rustack_esu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4203 2023-02-14 07:43:46.000000 rustack-esu-0.1.8/rustack_esu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      615 2023-02-14 07:43:46.000000 rustack-esu-0.1.8/rustack_esu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-14 07:43:46.000000 rustack-esu-0.1.8/rustack_esu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      185 2023-02-14 07:43:46.000000 rustack-esu-0.1.8/rustack_esu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        4 2023-02-14 07:43:46.000000 rustack-esu-0.1.8/rustack_esu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-14 07:43:46.394266 rustack-esu-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1956 2023-02-14 07:43:39.000000 rustack-esu-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 09:30:19.105345 rustack-esu-0.1.9/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1067 2023-03-13 09:30:07.000000 rustack-esu-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     4203 2023-03-13 09:30:19.105345 rustack-esu-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2428 2023-03-13 09:30:07.000000 rustack-esu-0.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 09:30:19.105345 rustack-esu-0.1.9/esu/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      715 2023-03-13 09:30:07.000000 rustack-esu-0.1.9/esu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5559 2023-03-13 09:30:07.000000 rustack-esu-0.1.9/esu/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1887 2023-03-13 09:30:07.000000 rustack-esu-0.1.9/esu/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3947 2023-03-13 09:30:07.000000 rustack-esu-0.1.9/esu/disk.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3186 2023-03-13 09:30:07.000000 rustack-esu-0.1.9/esu/dns.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3635 2023-03-13 09:30:07.000000 rustack-esu-0.1.9/esu/dns_record.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3489 2023-03-13 09:30:07.000000 rustack-esu-0.1.9/esu/firewall_template.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3990 2023-03-13 09:30:07.000000 rustack-esu-0.1.9/esu/firewall_template_rule.py
+-rw-r--r--   0 runner    (1001) docker     (122)      315 2023-03-13 09:30:07.000000 rustack-esu-0.1.9/esu/hypervisor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4244 2023-03-13 09:30:07.000000 rustack-esu-0.1.9/esu/lbaas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4904 2023-03-13 09:30:07.000000 rustack-esu-0.1.9/esu/lbaas_pool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2741 2023-03-13 09:30:07.000000 rustack-esu-0.1.9/esu/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4102 2023-03-13 09:30:07.000000 rustack-esu-0.1.9/esu/network.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6755 2023-03-13 09:30:07.000000 rustack-esu-0.1.9/esu/port.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-03-13 09:30:07.000000 rustack-esu-0.1.9/esu/project.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4190 2023-03-13 09:30:07.000000 rustack-esu-0.1.9/esu/router.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2953 2023-03-13 09:30:07.000000 rustack-esu-0.1.9/esu/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1249 2023-03-13 09:30:07.000000 rustack-esu-0.1.9/esu/storage_profile.py
+-rw-r--r--   0 runner    (1001) docker     (122)      574 2023-03-13 09:30:07.000000 rustack-esu-0.1.9/esu/subnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2080 2023-03-13 09:30:07.000000 rustack-esu-0.1.9/esu/template.py
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-03-13 09:30:07.000000 rustack-esu-0.1.9/esu/template_field.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8131 2023-03-13 09:30:07.000000 rustack-esu-0.1.9/esu/vdc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9183 2023-03-13 09:30:07.000000 rustack-esu-0.1.9/esu/vm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      342 2023-03-13 09:30:07.000000 rustack-esu-0.1.9/esu/vm_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 09:30:19.105345 rustack-esu-0.1.9/rustack_esu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4203 2023-03-13 09:30:18.000000 rustack-esu-0.1.9/rustack_esu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      590 2023-03-13 09:30:19.000000 rustack-esu-0.1.9/rustack_esu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-13 09:30:18.000000 rustack-esu-0.1.9/rustack_esu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      185 2023-03-13 09:30:18.000000 rustack-esu-0.1.9/rustack_esu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        4 2023-03-13 09:30:18.000000 rustack-esu-0.1.9/rustack_esu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-13 09:30:19.105345 rustack-esu-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1956 2023-03-13 09:30:07.000000 rustack-esu-0.1.9/setup.py
```

### Comparing `rustack-esu-0.1.8/LICENSE` & `rustack-esu-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rustack-esu-0.1.8/PKG-INFO` & `rustack-esu-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: rustack-esu
-Version: 0.1.8
+Version: 0.1.9
 Summary: RUSTACK-ESU Cloud API Wrapper
 Home-page: https://github.com/pilat/rustack-esu
 Author: Vladimir K Urushev
 Author-email: urushev@yandex.ru
 Maintainer: Vladimir K Urushev
 Maintainer-email: urushev@yandex.ru
 License: MIT
-Download-URL: https://github.com/pilat/rustack-esu/tarball/0.1.8
+Download-URL: https://github.com/pilat/rustack-esu/tarball/0.1.9
 Description: |PyPI Version| |Build Status| |Codecov Badge|
         
         ===========
         rustack-esu
         ===========
         
         **rustack-esu** является Python библиотекой для работы с публичным облаком
```

### Comparing `rustack-esu-0.1.8/README.rst` & `rustack-esu-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `rustack-esu-0.1.8/esu/__init__.py` & `rustack-esu-0.1.9/esu/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 from .subnet import Subnet
 from .template import Template
 from .template_field import TemplateField
 from .vdc import Vdc
 from .vm import Vm
 from .vm_metadata import VmMetadata
 
-__version__ = '0.1.8'
+__version__ = '0.1.9'
```

### Comparing `rustack-esu-0.1.8/esu/base.py` & `rustack-esu-0.1.9/esu/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,14 +22,18 @@
     pass
 
 
 class ObjectHasNoId(BaseEx):
     pass
 
 
+class PortAlreadyConnected(BaseEx):
+    pass
+
+
 class Field:
     def __init__(self, class_name=None, *, allow_none=False):
         self._class_name = class_name
         self._allow_none = allow_none
 
     @property
     def cls(self):
@@ -76,27 +80,27 @@
         instance._fill()
 
         return instance
 
     def __repr__(self):
         return '{} ({})'.format(self.__class__, self.id)
 
-    def _call(self, method, resource, **kwargs):
+    def _call(self, http_method, resource, **kwargs):
         headers = {
             'Authorization': 'Bearer {}'.format(self.token),
             'Content-Type': 'application/json',
             'Accept-Language': 'ru-ru'
         }
 
         url = '{}/{}'.format(self.endpoint_url, resource)
         request_params = dict(url=url, headers=headers, timeout=30)
-        method = method.lower()
+        http_method = http_method.lower()
 
-        request_params['params' if method == 'get' else 'json'] = kwargs
-        method_ = getattr(requests, method)
+        request_params['params' if http_method == 'get' else 'json'] = kwargs
+        method_ = getattr(requests, http_method)
         resp = method_(**request_params)
 
         answer = None
         if resp.status_code == 404:
             raise NotFoundEx('Resource not found')
 
         resp.raise_for_status()
```

### Comparing `rustack-esu-0.1.8/esu/client.py` & `rustack-esu-0.1.9/esu/client.py`

 * *Files identical despite different names*

### Comparing `rustack-esu-0.1.8/esu/disk.py` & `rustack-esu-0.1.9/esu/disk.py`

 * *Files identical despite different names*

### Comparing `rustack-esu-0.1.8/esu/dns.py` & `rustack-esu-0.1.9/esu/dns.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,13 +83,13 @@
         self.id = None
 
     def get_dns_records(self):
         """
         Получить список днс записей, доступных в рамках данного Dns.
 
         Returns:
-            list: Список объектов :class:`esu.Vm`
+            list: Список объектов :class:`esu.DnsRecord`
         """
         if self.id is None:
             raise ObjectHasNoId
 
         return self._get_list('v1/dns/{}/record'.format(self.id), DnsRecord)
```

### Comparing `rustack-esu-0.1.8/esu/dns_record.py` & `rustack-esu-0.1.9/esu/dns_record.py`

 * *Files identical despite different names*

### Comparing `rustack-esu-0.1.8/esu/firewall_template.py` & `rustack-esu-0.1.9/esu/firewall_template.py`

 * *Files identical despite different names*

### Comparing `rustack-esu-0.1.8/esu/firewall_template_rule.py` & `rustack-esu-0.1.9/esu/firewall_template_rule.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 from esu.base import BaseAPI, Field, ObjectAlreadyHasId, ObjectHasNoId
 
 
 class FirewallTemplateRule(BaseAPI):
     """
     Args:
-        id (str): Идентификатор шаблона брандмауэра
-        name (str): Имя шаблона брандмауэра
-        firewall_id (str): Объект класса :class:`esu.FirewallTemplate`.
+        id (str): Идентификатор правила брандмауэра
+        name (str): Имя правила брандмауэра
+        firewall (str): Объект класса :class:`esu.FirewallTemplate`.
                 Проект, к которому относится данное правило брандмауэра
-        direction (str): direction шаблона брандмауэра
-        destination_ip (str): destination_ip шаблона брандмауэра
-        dst_port_range_max (str): dst_port_range_max шаблона брандмауэра
-        dst_port_range_min (str): dst_port_range_min шаблона брандмауэра
-        protocol (str): protocol шаблона брандмауэра
+        direction (str): направление правила брандмауэра
+        destination_ip (str): destination_ip правила брандмауэра
+        dst_port_range_max (str): dst_port_range_max правила брандмауэра
+        dst_port_range_min (str): dst_port_range_min правила брандмауэра
+        protocol (str): protocol правила брандмауэра
         token (str): Токен для доступа к API. Если не передан, будет
                          использована переменная окружения **ESU_API_TOKEN**
 
     .. note:: Поля ``direction``, ``name`` и ``protocol`` необходимы для
               создания.
 
     """
     class Meta:
         id = Field()
         name = Field()
-        firewall_id = Field('esu.FirewallTemplate')
+        firewall = Field('esu.FirewallTemplate')
         direction = Field()
         destination_ip = Field()
         dst_port_range_max = Field()
         dst_port_range_min = Field()
         protocol = Field()
 
     @classmethod
-    def get_object(cls, firewall_id, rule_id, token=None):
+    def get_object(cls, firewall, rule_id, token=None):
         """
         Получить объект правил брандмауэра по его ID
 
         Args:
             id (str): Идентификатор шаблона брандмауэра
             token (str): Токен для доступа к API. Если не передан, будет
                          использована переменная окружения **ESU_API_TOKEN**
 
         Returns:
             object: Возвращает объект шаблона брандмауэра
             :class:`esu.FirewallTemplateRule`
         """
-        firewall_rule = cls(token=token, id=rule_id, firewall_id=firewall_id)
+        firewall_rule = cls(token=token, id=rule_id, firewall=firewall)
         firewall_rule._get_object(
-            'v1/firewall/{}/rule'.format(firewall_rule.firewall_id),
+            'v1/firewall/{}/rule'.format(firewall_rule.firewall.id),
             firewall_rule.id)
         return firewall_rule
 
     def create(self):
         """
         Создать объект
 
@@ -74,15 +74,15 @@
         if self.id is None:
             raise ObjectHasNoId
 
         self._commit()
 
     def _commit(self):
         self._commit_object(
-            'v1/firewall/{}/rule'.format(self.firewall_id),
+            'v1/firewall/{}/rule'.format(self.firewall.id),
             name=self.name,
             destination_ip=self.destination_ip,
             direction=self.direction,
             dst_port_range_max=self.dst_port_range_max,
             dst_port_range_min=self.dst_port_range_min,
             protocol=self.protocol,
         )
@@ -94,10 +94,10 @@
         Raises:
             ObjectHasNoId: Когда производится попытка удалить несуществующий
                            объект
         """
         if self.id is None:
             raise ObjectHasNoId
 
-        self._destroy_object('v1/firewall/{}/rule'.format(self.firewall_id),
+        self._destroy_object('v1/firewall/{}/rule'.format(self.firewall.id),
                              self.id)
         self.id = None
```

### Comparing `rustack-esu-0.1.8/esu/lbaas.py` & `rustack-esu-0.1.9/esu/lbaas.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,13 +100,13 @@
         self.id = None
 
     def get_lbaas_pool(self):
         """
         Получить список пулов балансировщика, доступных в рамках данного Lbaas.
 
         Returns:
-            list: Список объектов :class:`esu.Vm`
+            list: Список объектов :class:`esu.LbassPool`
         """
         if self.id is None:
             raise ObjectHasNoId
 
         return self._get_list('v1/lbaas/{}/pool'.format(self.id), LbaasPool)
```

### Comparing `rustack-esu-0.1.8/esu/lbaas_pool.py` & `rustack-esu-0.1.9/esu/lbaas_pool.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 from esu.base import BaseAPI, Field, FieldList, ObjectAlreadyHasId, \
     ObjectHasNoId
 
 
+class LbaasPoolMember(BaseAPI):
+    """
+    Args:
+        port (str): Порт участника пула балансировщика
+        vm (object): Объект :class:`esu.Vm`
+        weight (str): Вес участника пула балансировщика
+    """
+    class Meta:
+        port = Field()
+        vm = Field('esu.Vm')
+        weight = Field()
+
+
 class LbaasPool(BaseAPI):
     """
     Args:
         id (str): Идентификатор Lbaas Pool
         name (str): Имя Lbaas Pool
         lbaas_id (object): Объект класса :class:`esu.Lbaas`. Проект, к
                           которому относится данный Lbaas Pool
@@ -24,38 +37,38 @@
     .. note:: Поля ``members`` и ``port`` необходимы для
               создания.
 
     """
     class Meta:
         id = Field()
         name = Field()
-        lbaas_id = Field('esu.Project')
-        connlimit = Field('esu.Project')
-        cookie_name = Field('esu.Project')
-        members = FieldList('esu.LbaasPoolMember')
-        method = Field('esu.Project')
-        port = Field('esu.Project')
-        protocol = Field('esu.Project')
-        session_persistence = Field('esu.Project')
+        lbaas = Field('esu.Lbaas')
+        connlimit = Field()
+        cookie_name = Field()
+        members = FieldList(LbaasPoolMember)
+        method = Field()
+        port = Field()
+        protocol = Field()
+        session_persistence = Field()
 
     @classmethod
-    def get_object(cls, lbaas_id, pool_id, token=None):
+    def get_object(cls, lbaas, pool_id, token=None):
         """
         Получить объект пула балансировщика по его ID
 
         Args:
             id (str): Идентификатор Lbaas Pool
             token (str): Токен для доступа к API. Если не передан, будет
                          использована переменная окружения **ESU_API_TOKEN**
 
         Returns:
             object: Возвращает объект LbaasPool :class:`esu.LbaasPool`
         """
-        pool = cls(token=token, id=pool_id, lbaas_id=lbaas_id)
-        pool._get_object('v1/lbaas/{}/pool'.format(pool.lbaas_id), pool.id)
+        pool = cls(token=token, id=pool_id, lbaas=lbaas)
+        pool._get_object('v1/lbaas/{}/pool'.format(pool.lbaas.id), pool.id)
         return pool
 
     def create(self):
         """
         Создать объект
 
         Raises:
@@ -82,33 +95,35 @@
 
     def _commit(self):
         members = [{
             'port': o.port,
             'vm': o.vm.id,
             'weight': o.weight
         } for o in self.members]
+        pull = {
+            'members': members,
+            'method': self.method,
+            'port': self.port,
+            'protocol': self.protocol,
+            'session_persistence': self.session_persistence,
+            'name': self.name,
+        }
+        if self.connlimit is not None:
+            pull['connlimit'] = self.connlimit
+        if self.cookie_name is not None:
+            pull['cookie_name'] = self.cookie_name
 
-        self._commit_object(
-            'v1/lbaas/{}/pool'.format(self.lbaas_id),
-            connlimit=self.connlimit,
-            members=members,
-            cookie_name=self.cookie_name,
-            method=self.method,
-            port=self.port,
-            protocol=self.protocol,
-            session_persistence=self.session_persistence,
-            name=self.name,
-        )
+        self._commit_object('v1/lbaas/{}/pool'.format(self.lbaas.id), **pull)
 
     def destroy(self):
         """
         Удалить объект
 
         Raises:
             ObjectHasNoId: Когда производится попытка удалить несуществующий
                            объект
         """
         if self.id is None:
             raise ObjectHasNoId
 
-        self._destroy_object('v1/lbaas/{}/pool'.format(self.lbaas_id), self.id)
+        self._destroy_object('v1/lbaas/{}/pool'.format(self.lbaas.id), self.id)
         self.id = None
```

### Comparing `rustack-esu-0.1.8/esu/manager.py` & `rustack-esu-0.1.9/esu/manager.py`

 * *Files identical despite different names*

### Comparing `rustack-esu-0.1.8/esu/network.py` & `rustack-esu-0.1.9/esu/network.py`

 * *Files identical despite different names*

### Comparing `rustack-esu-0.1.8/esu/port.py` & `rustack-esu-0.1.9/esu/port.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,24 @@
 from esu.base import BaseAPI, Field, FieldList, ObjectAlreadyHasId, \
-    ObjectHasNoId
+    ObjectHasNoId, PortAlreadyConnected
+
+
+class ConnectedObject(BaseAPI):
+    """
+    Args:
+        id (str): Идентификатор подключённого объекта
+        type (object): Тип объекта
+        name (object): Имя подключённого объекта
+        vdc (str): Объект :class:`esu.Vdc`
+    """
+    class Meta:
+        id = Field(allow_none=True)
+        type = Field()
+        name = Field()
+        vdc = Field('esu.Vdc', allow_none=True)
 
 
 class Port(BaseAPI):
     """
     Args:
         id (str): Идентификатор порта
         ip_address (str): IP адрес
@@ -26,17 +41,19 @@
               При создании подключения плавающего IP обязательных полей нет
     """
     class Meta:
         id = Field()
         ip_address = Field()
         type = Field()
         vdc = Field("esu.Vdc")
-        fw_templates = FieldList('esu.FirewallTemplate')
+        fw_templates = FieldList('esu.FirewallTemplate', allow_none=True)
         network = Field('esu.Network')
-        device = Field()
+        connected = Field(ConnectedObject, allow_none=True)
+        vm = Field('esu.Vm')
+        router = Field('esu.Router', allow_none=True)
 
     @classmethod
     def get_object(cls, id, token=None):
         """
         Получить объект порта по его ID
 
         Args:
@@ -88,27 +105,50 @@
                            объект
         """
         if self.id is None:
             raise ObjectHasNoId
 
         self._commit()
 
-    #pylint: disable=import-outside-toplevel
     def _commit(self):
-        from esu import Router, Vm
-
         port = {
             'ip_address': self.ip_address or '0.0.0.0',
-            'network': self.network.id,
+            'fw_templates': [o.id for o in self.fw_templates or []]
         }
-        if isinstance(self.device, Vm):
-            port['vm'] = self.device.id
-            port['fw_templates'] = [o.id for o in self.fw_templates or []]
-        elif isinstance(self.device, Router):
-            port['router'] = self.device.id
+
+        if self.id is None:
+            port['network'] = self.network.id
+            if self.vm is not None:
+                port['vm'] = self.vm.id
+            elif self.router is not None:
+                port['router'] = self.router.id
+
+        self._commit_object('v1/port', **port)
+
+    def connect(self):
+        """
+        Подключить
+
+        Raises:
+            ObjectHasNoId: Если производится попытка присоединить
+                           несуществующий объект
+
+            PortAlreadyConnected: Если производится попытка
+                                  присоединить уже присоединенный порт
+        """
+        if self.id is None:
+            raise ObjectHasNoId
+
+        if self.connected is not None:
+            raise PortAlreadyConnected
+
+        if self.vm is not None:
+            port = {'vm': self.vm.id}
+        elif self.router is not None:
+            port = {'router': self.router.id}
 
         self._commit_object('v1/port', **port)
 
     def disconnect(self):
         """
         Отключить порт
 
@@ -116,16 +156,18 @@
             ObjectHasNoId: Если производится попытка сохранить несуществующий
                            объект
         """
         if self.id is None:
             raise ObjectHasNoId
 
         self._call('PATCH', 'v1/port/{}/disconnect'.format(self.id))
-        self.device = None
         self._fill()
+        self.connected = None
+        self.vm = None
+        self.router = None
 
     def destroy(self):
         """
         Удалить объект
 
         Raises:
             ObjectHasNoId: Когда производится попытка удалить несуществующий
```

### Comparing `rustack-esu-0.1.8/esu/project.py` & `rustack-esu-0.1.9/esu/project.py`

 * *Files identical despite different names*

### Comparing `rustack-esu-0.1.8/esu/router.py` & `rustack-esu-0.1.9/esu/router.py`

 * *Files identical despite different names*

### Comparing `rustack-esu-0.1.8/esu/snapshot.py` & `rustack-esu-0.1.9/esu/snapshot.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 class Snapshot(BaseAPI):
     """
     Args:
         id (str): Идентификатор снапшота
         name (str): Имя снапшота
-        description (str): описание для шаблона брандмауэра
+        description (str): описание для снапшота
         vm (object): Объект класса :class:`esu.Vm`. Сервер, к которому
                       относится данный снапшот
 
     .. note:: Поле ``name`` и ``vm`` необходимо для создания
 
               Поля ``description`` опцональны при создании
 
@@ -21,30 +21,28 @@
     class Meta:
         id = Field()
         name = Field()
         vm = Field("esu.Vm")
         description = Field()
 
     @classmethod
-    def get_object(cls, id, vm, token=None):
+    def get_object(cls, id, token=None):
         """
         Получить объект порта по его ID
 
         Args:
             id (str): Идентификатор снапшота
-            vm (str): Идентификатор vm
             token (str): Токен для доступа к API. Если не передан, будет
                          использована переменная окружения **ESU_API_TOKEN**
 
         Returns:
             object: Возвращает объект порта :class:`esu.Port`
         """
-        snapshot = cls(token=token, id=id, vm=vm)
-        snapshot._get_object('v1/vm/{}/snapshot'.format(snapshot.vm.id),
-                             snapshot.id)
+        snapshot = cls(token=token, id=id)
+        snapshot._get_object('v2/snapshot', snapshot.id)
         return snapshot
 
     def create(self):
         """
         Создать объект
 
         Raises:
@@ -68,23 +66,23 @@
             raise ObjectHasNoId
 
         self._commit()
 
     #pylint: disable=import-outside-toplevel
     def _commit(self):
         description = self.description or ''
-        self._commit_object('v1/vm/{}/snapshot'.format(self.vm.id),
-                            name=self.name, description=description)
+        self._commit_object('v2/snapshot', name=self.name,
+                            description=description, vm=self.vm.id)
 
     def destroy(self):
         """
         Удалить объект
 
         Raises:
             ObjectHasNoId: Когда производится попытка удалить несуществующий
                            объект
         """
         if self.id is None:
             raise ObjectHasNoId
 
-        self._destroy_object('v1/vm/{}/snapshot'.format(self.vm.id), self.id)
+        self._destroy_object('v2/snapshot', self.id)
         self.id = None
```

### Comparing `rustack-esu-0.1.8/esu/storage_profile.py` & `rustack-esu-0.1.9/esu/storage_profile.py`

 * *Files identical despite different names*

### Comparing `rustack-esu-0.1.8/esu/subnet.py` & `rustack-esu-0.1.9/esu/subnet.py`

 * *Files identical despite different names*

### Comparing `rustack-esu-0.1.8/esu/template.py` & `rustack-esu-0.1.9/esu/template.py`

 * *Files identical despite different names*

### Comparing `rustack-esu-0.1.8/esu/template_field.py` & `rustack-esu-0.1.9/esu/template_field.py`

 * *Files identical despite different names*

### Comparing `rustack-esu-0.1.8/esu/vdc.py` & `rustack-esu-0.1.9/esu/vdc.py`

 * *Files identical despite different names*

### Comparing `rustack-esu-0.1.8/esu/vm.py` & `rustack-esu-0.1.9/esu/vm.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,15 @@
         power = Field()
         vdc = Field('esu.Vdc')
         template = Field('esu.Template')
         metadata = FieldList('esu.VmMetadata')
         ports = FieldList('esu.Port')
         disks = FieldList('esu.Disk')
         floating = Field('esu.Port', allow_none=True)
+        hotadd_feature = Field()
 
     @classmethod
     def get_object(cls, id, token=None):
         """
         Получить объект виртуального сервера по его ID
 
         Args:
@@ -99,43 +100,43 @@
     def _commit(self):
         vm = {
             'vdc': self.vdc.id,
             'template': self.template.id,
             'name': self.name,
             'cpu': self.cpu,
             'ram': self.ram,
-            'description': self.description or ''
+            'description': self.description or '',
+            'ports': [{
+                'id': o.id,
+            } if o.id else {
+                'network': o.network.id,
+                'fw_templates': [o2.id for o2 in o.fw_templates or []]
+            } for o in self.ports],
+            'disks': [{
+                'name': o.name,
+                'size': o.size,
+                'storage_profile': o.storage_profile.id
+            } for o in self.disks]
         }
 
-        vm['ports'] = [{
-            'id': o.id,
-        }if o.id else \
-        {
-            'network': o.network.id,
-            'fw_templates': [o2.id for o2 in o.fw_templates or []]
-        } for o in self.ports]
-
-        vm['disks'] = [{
-            'name': o.name,
-            'size': o.size,
-            'storage_profile': o.storage_profile.id
-        } for o in self.disks]
-
         if self.id is None:
             vm['metadata'] = [{
                 'field': o.field.id,
                 'value': o.value
             } for o in self.metadata]
 
         floating = None
         if self.floating:
             # keep/change or get a new IP
             floating = self.floating.id or '0.0.0.0'
         vm['floating'] = floating
 
+        if self.hotadd_feature:
+            vm['hotadd_feature'] = True
+
         self._commit_object('v1/vm', **vm)
 
     def destroy(self):
         """
         Удалить объект
 
         Raises:
@@ -237,7 +238,11 @@
 
         Returns:
             str: Адрес VNC консоли
         """
         vnc = self._call('POST', 'v1/vm/{}/vnc'.format(self.id))
         uri = vnc['url']
         return '{}{}'.format(self.endpoint_url, uri)
+
+    def revert(self, snapshot):
+        vm = self._call('POST', 'v2/snapshot/{}/revert'.format(snapshot.id))
+        return vm
```

### Comparing `rustack-esu-0.1.8/rustack_esu.egg-info/PKG-INFO` & `rustack-esu-0.1.9/rustack_esu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: rustack-esu
-Version: 0.1.8
+Version: 0.1.9
 Summary: RUSTACK-ESU Cloud API Wrapper
 Home-page: https://github.com/pilat/rustack-esu
 Author: Vladimir K Urushev
 Author-email: urushev@yandex.ru
 Maintainer: Vladimir K Urushev
 Maintainer-email: urushev@yandex.ru
 License: MIT
-Download-URL: https://github.com/pilat/rustack-esu/tarball/0.1.8
+Download-URL: https://github.com/pilat/rustack-esu/tarball/0.1.9
 Description: |PyPI Version| |Build Status| |Codecov Badge|
         
         ===========
         rustack-esu
         ===========
         
         **rustack-esu** является Python библиотекой для работы с публичным облаком
```

### Comparing `rustack-esu-0.1.8/rustack_esu.egg-info/SOURCES.txt` & `rustack-esu-0.1.9/rustack_esu.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 esu/dns.py
 esu/dns_record.py
 esu/firewall_template.py
 esu/firewall_template_rule.py
 esu/hypervisor.py
 esu/lbaas.py
 esu/lbaas_pool.py
-esu/lbaas_pool_member.py
 esu/manager.py
 esu/network.py
 esu/port.py
 esu/project.py
 esu/router.py
 esu/snapshot.py
 esu/storage_profile.py
```

### Comparing `rustack-esu-0.1.8/setup.py` & `rustack-esu-0.1.9/setup.py`

 * *Files identical despite different names*

