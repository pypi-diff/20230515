# Comparing `tmp/viggonuvemfiscal-1.0.6.tar.gz` & `tmp/viggonuvemfiscal-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viggonuvemfiscal-1.0.6.tar", last modified: Fri May  5 19:26:33 2023, max compression
+gzip compressed data, was "viggonuvemfiscal-1.1.0.tar", last modified: Mon May 15 19:46:30 2023, max compression
```

## Comparing `viggonuvemfiscal-1.0.6.tar` & `viggonuvemfiscal-1.1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:26:33.372335 viggonuvemfiscal-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 19:25:41.000000 viggonuvemfiscal-1.0.6/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-05 19:25:41.000000 viggonuvemfiscal-1.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-05 19:26:33.372335 viggonuvemfiscal-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-05 19:25:41.000000 viggonuvemfiscal-1.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 19:26:33.372335 viggonuvemfiscal-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-05 19:25:41.000000 viggonuvemfiscal-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:26:33.368335 viggonuvemfiscal-1.0.6/viggonuvemfiscal/
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-05 19:25:41.000000 viggonuvemfiscal-1.0.6/viggonuvemfiscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-05 19:25:41.000000 viggonuvemfiscal-1.0.6/viggonuvemfiscal/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:26:33.368335 viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:25:41.000000 viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:26:33.368335 viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:25:41.000000 viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:26:33.372335 viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-05 19:25:41.000000 viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-05 19:25:41.000000 viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-05 19:25:41.000000 viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-05 19:25:41.000000 viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:26:33.372335 viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-05 19:25:41.000000 viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14896 2023-05-05 19:25:41.000000 viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     9906 2023-05-05 19:25:41.000000 viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-05 19:25:41.000000 viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-05-05 19:25:41.000000 viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:26:33.368335 viggonuvemfiscal-1.0.6/viggonuvemfiscal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-05 19:26:33.000000 viggonuvemfiscal-1.0.6/viggonuvemfiscal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-05 19:26:33.000000 viggonuvemfiscal-1.0.6/viggonuvemfiscal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 19:26:33.000000 viggonuvemfiscal-1.0.6/viggonuvemfiscal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-05 19:26:33.000000 viggonuvemfiscal-1.0.6/viggonuvemfiscal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 19:26:33.000000 viggonuvemfiscal-1.0.6/viggonuvemfiscal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:46:30.043693 viggonuvemfiscal-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 19:45:29.000000 viggonuvemfiscal-1.1.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-15 19:45:29.000000 viggonuvemfiscal-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-15 19:46:30.043693 viggonuvemfiscal-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-15 19:45:29.000000 viggonuvemfiscal-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 19:46:30.043693 viggonuvemfiscal-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-15 19:45:29.000000 viggonuvemfiscal-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:46:30.039693 viggonuvemfiscal-1.1.0/viggonuvemfiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-15 19:45:29.000000 viggonuvemfiscal-1.1.0/viggonuvemfiscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-15 19:45:29.000000 viggonuvemfiscal-1.1.0/viggonuvemfiscal/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:46:30.039693 viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:29.000000 viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:46:30.039693 viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/controle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:29.000000 viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/controle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:46:30.039693 viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-15 19:45:29.000000 viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-15 19:45:29.000000 viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-15 19:45:29.000000 viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-15 19:45:29.000000 viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:46:30.043693 viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-15 19:45:29.000000 viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22598 2023-05-15 19:45:29.000000 viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14694 2023-05-15 19:45:29.000000 viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-15 19:45:29.000000 viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-05-15 19:45:29.000000 viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:46:30.039693 viggonuvemfiscal-1.1.0/viggonuvemfiscal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-15 19:46:29.000000 viggonuvemfiscal-1.1.0/viggonuvemfiscal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-15 19:46:29.000000 viggonuvemfiscal-1.1.0/viggonuvemfiscal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 19:46:29.000000 viggonuvemfiscal-1.1.0/viggonuvemfiscal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-15 19:46:29.000000 viggonuvemfiscal-1.1.0/viggonuvemfiscal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 19:46:29.000000 viggonuvemfiscal-1.1.0/viggonuvemfiscal.egg-info/top_level.txt
```

### Comparing `viggonuvemfiscal-1.0.6/viggonuvemfiscal/__init__.py` & `viggonuvemfiscal-1.1.0/viggonuvemfiscal/__init__.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.0.6/viggonuvemfiscal/resources.py` & `viggonuvemfiscal-1.1.0/viggonuvemfiscal/resources.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/manager.py` & `viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/manager.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/resource.py` & `viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/resource.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/router.py` & `viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/router.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/controller.py` & `viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/controller.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,14 +31,20 @@
 
     def get_nfe_id(self, **kwargs):
         nfe_id = kwargs.get('nfe_id', None)
         if nfe_id is None:
             raise exception.BadRequest('O campo nfe_id é obrigatório.')
         return nfe_id
 
+    def get_nfce_id(self, **kwargs):
+        nfce_id = kwargs.get('nfce_id', None)
+        if nfce_id is None:
+            raise exception.BadRequest('O campo nfce_id é obrigatório.')
+        return nfce_id
+
     def get_endpoint(self, resource):
         return self.BASE_URL_HOMO + resource
 
     def executar_requisicao(
        self, method, endpoint, params={}, json={}, headers={}):
         headers.update(self.get_authorization())
         if method == 'GET':
@@ -227,14 +233,52 @@
 
         response_dict = self.montar_response_dict(response)
 
         return flask.Response(response=utils.to_json(response_dict),
                               status=response.status_code,
                               mimetype="application/json")
 
+    def consultar_configuracao_nfce(self):
+        filters = self._filters_parse()
+        filters = self._filters_cleanup(filters)
+
+        try:
+            filters = self._parse_list_options(filters)
+            cpf_cnpj = self.get_cpf_cnpj(**filters)
+            url = self.get_endpoint(f'/empresas/{cpf_cnpj}/nfce')
+            response = self.executar_requisicao('GET', url)
+        except exception.ViggoCoreException as exc:
+            return flask.Response(response=exc.message,
+                                  status=exc.status)
+
+        response_dict = self.montar_response_dict(response)
+
+        return flask.Response(response=utils.to_json(response_dict),
+                              status=response.status_code,
+                              mimetype="application/json")
+
+    def alterar_configuracao_nfce(self):
+        data = flask.request.get_json()
+
+        try:
+            cpf_cnpj = self.get_cpf_cnpj(**data)
+            url = self.get_endpoint(f'/empresas/{cpf_cnpj}/nfce')
+            data.pop('cpf_cnpj')
+            response = self.executar_requisicao('PUT', url, json=data)
+        except exception.ViggoCoreException as exc:
+            return flask.Response(response=exc.message,
+                                  status=exc.status)
+
+        response_dict = self.montar_response_dict(response)
+
+        return flask.Response(response=utils.to_json(response_dict),
+                              status=response.status_code,
+                              mimetype="application/json")
+
+    # nfe
     def emitir_nfe(self):
         data = flask.request.get_json()
 
         try:
             url = self.get_endpoint('/nfe')
             response = self.executar_requisicao('POST', url, json=data)
         except exception.ViggoCoreException as exc:
@@ -261,15 +305,15 @@
 
         response_dict = self.montar_response_dict(response)
 
         return flask.Response(response=utils.to_json(response_dict),
                               status=response.status_code,
                               mimetype="application/json")
 
-    def consulta_status_do_servico_na_sefaz_autorizadora(self):
+    def consulta_status_do_servico_na_sefaz_autorizadora_nfe(self):
         filters = self._filters_parse()
         filters = self._filters_cleanup(filters)
 
         try:
             filters = self._parse_list_options(filters)
             url = self.get_endpoint('/nfe/sefaz/status')
             response = self.executar_requisicao('GET', url, params=filters)
@@ -369,10 +413,157 @@
             response = self.executar_requisicao('POST', url, json=data)
         except exception.ViggoCoreException as exc:
             return flask.Response(response=exc.message,
                                   status=exc.status)
 
         response_dict = self.montar_response_dict(response)
 
+        return flask.Response(response=utils.to_json(response_dict),
+                              status=response.status_code,
+                              mimetype="application/json")
+
+    # nfce
+    def emitir_nfce(self):
+        data = flask.request.get_json()
+
+        try:
+            url = self.get_endpoint('/nfce')
+            response = self.executar_requisicao('POST', url, json=data)
+        except exception.ViggoCoreException as exc:
+            return flask.Response(response=exc.message,
+                                  status=exc.status)
+
+        response_dict = self.montar_response_dict(response)
+
+        return flask.Response(response=utils.to_json(response_dict),
+                              status=response.status_code,
+                              mimetype="application/json")
+
+    def listar_nfce(self):
+        filters = self._filters_parse()
+        filters = self._filters_cleanup(filters)
+
+        try:
+            filters = self._parse_list_options(filters)
+            url = self.get_endpoint('/nfce')
+            response = self.executar_requisicao('GET', url, params=filters)
+        except exception.ViggoCoreException as exc:
+            return flask.Response(response=exc.message,
+                                  status=exc.status)
+
+        response_dict = self.montar_response_dict(response)
+
+        return flask.Response(response=utils.to_json(response_dict),
+                              status=response.status_code,
+                              mimetype="application/json")
+
+    def consulta_status_do_servico_na_sefaz_autorizadora_nfce(self):
+        filters = self._filters_parse()
+        filters = self._filters_cleanup(filters)
+
+        try:
+            filters = self._parse_list_options(filters)
+            url = self.get_endpoint('/nfce/sefaz/status')
+            response = self.executar_requisicao('GET', url, params=filters)
+        except exception.ViggoCoreException as exc:
+            return flask.Response(response=exc.message,
+                                  status=exc.status)
+
+        response_dict = self.montar_response_dict(response)
+
+        return flask.Response(response=utils.to_json(response_dict),
+                              status=response.status_code,
+                              mimetype="application/json")
+
+    def consultar_nfce(self):
+        filters = self._filters_parse()
+        filters = self._filters_cleanup(filters)
+
+        try:
+            filters = self._parse_list_options(filters)
+            nfce_id = self.get_nfce_id(**filters)
+            url = self.get_endpoint(f'/nfce/{nfce_id}')
+            response = self.executar_requisicao('GET', url)
+        except exception.ViggoCoreException as exc:
+            return flask.Response(response=exc.message,
+                                  status=exc.status)
+
+        response_dict = self.montar_response_dict(response)
+
+        return flask.Response(response=utils.to_json(response_dict),
+                              status=response.status_code,
+                              mimetype="application/json")
+
+    def baixar_xml_nfce(self):
+        filters = self._filters_parse()
+        filters = self._filters_cleanup(filters)
+
+        try:
+            filters = self._parse_list_options(filters)
+            nfce_id = self.get_nfce_id(**filters)
+            url = self.get_endpoint(f'/nfce/{nfce_id}/xml')
+            response = self.executar_requisicao('GET', url)
+        except exception.ViggoCoreException as exc:
+            return flask.Response(response=exc.message,
+                                  status=exc.status)
+
+        response_dict = self.montar_response_dict(response)
+
+        return flask.Response(response=utils.to_json(response_dict),
+                              status=response.status_code,
+                              mimetype="application/json")
+
+    def consultar_cancelamento_nfce(self):
+        filters = self._filters_parse()
+        filters = self._filters_cleanup(filters)
+
+        try:
+            filters = self._parse_list_options(filters)
+            nfce_id = self.get_nfce_id(**filters)
+            url = self.get_endpoint(f'/nfce/{nfce_id}/cancelamento')
+            response = self.executar_requisicao('GET', url)
+        except exception.ViggoCoreException as exc:
+            return flask.Response(response=exc.message,
+                                  status=exc.status)
+
+        response_dict = self.montar_response_dict(response)
+
+        return flask.Response(response=utils.to_json(response_dict),
+                              status=response.status_code,
+                              mimetype="application/json")
+
+    def baixar_xml_cancelamento_nfce(self):
+        filters = self._filters_parse()
+        filters = self._filters_cleanup(filters)
+
+        try:
+            filters = self._parse_list_options(filters)
+            nfce_id = self.get_nfce_id(**filters)
+            url = self.get_endpoint(f'/nfce/{nfce_id}/cancelamento/xml')
+            response = self.executar_requisicao('GET', url)
+        except exception.ViggoCoreException as exc:
+            return flask.Response(response=exc.message,
+                                  status=exc.status)
+
+        response_dict = self.montar_response_dict(response)
+
+        return flask.Response(response=utils.to_json(response_dict),
+                              status=response.status_code,
+                              mimetype="application/json")
+
+    def cancelar_nfce_autorizada(self):
+        data = flask.request.get_json()
+
+        try:
+            nfce_id = self.get_nfce_id(**data)
+            url = self.get_endpoint(f'/nfce/{nfce_id}/cancelamento')
+            data.pop('nfce_id')
+            response = self.executar_requisicao('POST', url, json=data)
+        except exception.ViggoCoreException as exc:
+            return flask.Response(response=exc.message,
+                                  status=exc.status)
+
+        response_dict = self.montar_response_dict(response)
+
         return flask.Response(response=utils.to_json(response_dict),
                               status=response.status_code,
                               mimetype="application/json")
```

### Comparing `viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/router.py` & `viggonuvemfiscal-1.1.0/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/router.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,46 +74,49 @@
             {
                 'action': 'Emitir NFe na Nuvem Fiscal',
                 'method': 'GET',
                 'url': self.collection_url + '/listar_nfe',
                 'callback': 'listar_nfe'
             },
             {
-                'action': 'Consulta do Status do Serviço na SEFAZ Autorizadora',
+                'action': 'Consulta do Status do Serviço na SEFAZ ' +
+                'Autorizadora',
                 'method': 'GET',
-                'url': (self.collection_url +
-                    '/consulta_status_do_servico_na_sefaz_autorizadora'),
-                'callback': 'consulta_status_do_servico_na_sefaz_autorizadora'
+                'url': (
+                    self.collection_url +
+                    '/consulta_status_do_servico_na_sefaz_autorizadora_nfe'),
+                'callback':
+                    'consulta_status_do_servico_na_sefaz_autorizadora_nfe'
             },
             {
                 'action': 'Consultar NFe na Nuvem Fiscal',
                 'method': 'GET',
                 'url': self.collection_url + '/consultar_nfe',
                 'callback': 'consultar_nfe'
             },
             {
                 'action': 'Baixar XML da NFe processada na Nuvem Fiscal',
                 'method': 'GET',
                 'url': self.collection_url + '/baixar_xml_nfe',
                 'callback': 'baixar_xml_nfe'
             },
             {
-                'action': 'Consultar cancelamento da NFe na ' + \
-                    'Nuvem Fiscal',
+                'action': 'Consultar cancelamento da NFe na ' +
+                'Nuvem Fiscal',
                 'method': 'GET',
                 'url': self.collection_url + '/consultar_cancelamento_nfe',
                 'callback': 'consultar_cancelamento_nfe'
             },
             {
-                'action': 'Baixar XML do cancelamento da NFe processada ' +\
-                    'na Nuvem Fiscal',
+                'action': 'Baixar XML do cancelamento da NFe processada ' +
+                'na Nuvem Fiscal',
                 'method': 'GET',
                 'url': self.collection_url + '/baixar_xml_cancelamento_nfe',
                 'callback': 'baixar_xml_cancelamento_nfe'
             },
             {
                 'action': 'Cancelar uma NFe autorizada na Nuvem Fiscal',
                 'method': 'POST',
                 'url': self.collection_url + '/cancelar_nfe_autorizada',
                 'callback': 'cancelar_nfe_autorizada'
             },
-        ]
+        ]
```

### Comparing `viggonuvemfiscal-1.0.6/viggonuvemfiscal.egg-info/SOURCES.txt` & `viggonuvemfiscal-1.1.0/viggonuvemfiscal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

