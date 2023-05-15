# Comparing `tmp/conniosdk-0.31-py3-none-any.whl.zip` & `tmp/conniosdk-0.32-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,52 +1,44 @@
-Zip file size: 73425 bytes, number of entries: 50
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-06 07:44 connio/__init__.py
--rw-r--r--  2.0 unx      497 b- defN 23-Jan-06 07:44 connio/compat.py
--rw-r--r--  2.0 unx     6054 b- defN 23-Jan-06 07:44 connio/mqtt.py
--rw-r--r--  2.0 unx     2323 b- defN 23-Jan-06 07:44 connio/request_validator.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jan-06 07:44 connio/base/__init__.py
--rw-r--r--  2.0 unx     8271 b- defN 23-Jan-06 07:44 connio/base/deserialize.py
--rw-r--r--  2.0 unx     1519 b- defN 23-Jan-06 07:44 connio/base/domain.py
--rw-r--r--  2.0 unx     2552 b- defN 23-Jan-06 07:44 connio/base/exceptions.py
--rw-r--r--  2.0 unx      184 b- defN 23-Jan-06 07:44 connio/base/instance_context.py
--rw-r--r--  2.0 unx      185 b- defN 23-Jan-06 07:44 connio/base/instance_resource.py
--rw-r--r--  2.0 unx      180 b- defN 23-Jan-06 07:44 connio/base/list_resource.py
--rw-r--r--  2.0 unx      636 b- defN 23-Jan-06 07:44 connio/base/obsolete.py
--rw-r--r--  2.0 unx     4684 b- defN 23-Jan-06 07:44 connio/base/page.py
--rw-r--r--  2.0 unx     6392 b- defN 23-Jan-06 07:44 connio/base/serialize.py
--rw-r--r--  2.0 unx      255 b- defN 23-Jan-06 07:44 connio/base/values.py
--rw-r--r--  2.0 unx     6342 b- defN 23-Jan-06 07:44 connio/base/version.py
--rw-r--r--  2.0 unx      403 b- defN 23-Jan-06 07:44 connio/http/__init__.py
--rw-r--r--  2.0 unx     2809 b- defN 23-Jan-06 07:44 connio/http/http_client.py
--rw-r--r--  2.0 unx     2636 b- defN 23-Jan-06 07:44 connio/http/request.py
--rw-r--r--  2.0 unx      375 b- defN 23-Jan-06 07:44 connio/http/response.py
--rw-r--r--  2.0 unx     4017 b- defN 23-Jan-06 07:44 connio/http/validation_client.py
--rw-r--r--  2.0 unx     5206 b- defN 23-Jan-06 07:44 connio/jwt/__init__.py
--rw-r--r--  2.0 unx     1118 b- defN 23-Jan-06 07:44 connio/jwt/compat.py
--rw-r--r--  2.0 unx     2143 b- defN 23-Jan-06 07:44 connio/jwt/access_token/__init__.py
--rw-r--r--  2.0 unx     5841 b- defN 23-Jan-06 07:44 connio/jwt/access_token/grants.py
--rw-r--r--  2.0 unx     3891 b- defN 23-Jan-06 07:44 connio/jwt/client/__init__.py
--rw-r--r--  2.0 unx     5584 b- defN 23-Jan-06 07:44 connio/jwt/taskrouter/__init__.py
--rw-r--r--  2.0 unx     4281 b- defN 23-Jan-06 07:44 connio/jwt/taskrouter/capabilities.py
--rw-r--r--  2.0 unx     3140 b- defN 23-Jan-06 07:44 connio/jwt/validation/__init__.py
--rw-r--r--  2.0 unx     4601 b- defN 23-Jan-06 07:44 connio/rest/__init__.py
--rw-r--r--  2.0 unx     1280 b- defN 23-Jan-06 07:44 connio/rest/api/__init__.py
--rw-r--r--  2.0 unx     3353 b- defN 23-Jan-06 07:44 connio/rest/api/v3/__init__.py
--rw-r--r--  2.0 unx    19909 b- defN 23-Jan-06 07:44 connio/rest/api/v3/account/__init__.py
--rw-r--r--  2.0 unx    17384 b- defN 23-Jan-06 07:44 connio/rest/api/v3/account/alert.py
--rw-r--r--  2.0 unx    16706 b- defN 23-Jan-06 07:44 connio/rest/api/v3/account/apiclient.py
--rw-r--r--  2.0 unx     7844 b- defN 23-Jan-06 07:44 connio/rest/api/v3/account/apikey.py
--rw-r--r--  2.0 unx    18129 b- defN 23-Jan-06 07:44 connio/rest/api/v3/account/app.py
--rw-r--r--  2.0 unx    17868 b- defN 23-Jan-06 07:44 connio/rest/api/v3/account/appprofile.py
--rw-r--r--  2.0 unx    10282 b- defN 23-Jan-06 07:44 connio/rest/api/v3/account/dataconnector.py
--rw-r--r--  2.0 unx    22686 b- defN 23-Jan-06 07:44 connio/rest/api/v3/account/device.py
--rw-r--r--  2.0 unx    17949 b- defN 23-Jan-06 07:44 connio/rest/api/v3/account/deviceprofile.py
--rw-r--r--  2.0 unx    17665 b- defN 23-Jan-06 07:44 connio/rest/api/v3/account/method.py
--rw-r--r--  2.0 unx    23009 b- defN 23-Jan-06 07:44 connio/rest/api/v3/account/propertyy.py
--rw-r--r--  2.0 unx    16506 b- defN 23-Jan-06 07:44 connio/rest/api/v3/account/user.py
--rw-r--r--  2.0 unx      765 b- defN 23-Jan-06 07:44 connio/rest/api/v3/helpers/__init__.py
--rw-r--r--  2.0 unx    14777 b- defN 23-Jan-06 07:44 connio/rest/api/v3/sysuser/__init__.py
--rw-r--r--  2.0 unx      282 b- defN 23-Jan-06 07:45 conniosdk-0.31.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-06 07:45 conniosdk-0.31.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Jan-06 07:45 conniosdk-0.31.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     4266 b- defN 23-Jan-06 07:45 conniosdk-0.31.dist-info/RECORD
-50 files, 316970 bytes uncompressed, 66647 bytes compressed:  79.0%
+Zip file size: 63519 bytes, number of entries: 42
+-rw-r--r--  2.0 unx       92 b- defN 23-May-15 10:39 connio/__init__.py
+-rw-r--r--  2.0 unx      497 b- defN 23-May-15 10:39 connio/compat.py
+-rw-r--r--  2.0 unx     6054 b- defN 23-May-15 10:39 connio/mqtt.py
+-rw-r--r--  2.0 unx     2323 b- defN 23-May-15 10:39 connio/request_validator.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-15 10:39 connio/base/__init__.py
+-rw-r--r--  2.0 unx     8312 b- defN 23-May-15 10:39 connio/base/deserialize.py
+-rw-r--r--  2.0 unx     1519 b- defN 23-May-15 10:39 connio/base/domain.py
+-rw-r--r--  2.0 unx     2552 b- defN 23-May-15 10:39 connio/base/exceptions.py
+-rw-r--r--  2.0 unx      184 b- defN 23-May-15 10:39 connio/base/instance_context.py
+-rw-r--r--  2.0 unx      185 b- defN 23-May-15 10:39 connio/base/instance_resource.py
+-rw-r--r--  2.0 unx      180 b- defN 23-May-15 10:39 connio/base/list_resource.py
+-rw-r--r--  2.0 unx      636 b- defN 23-May-15 10:39 connio/base/obsolete.py
+-rw-r--r--  2.0 unx     4684 b- defN 23-May-15 10:39 connio/base/page.py
+-rw-r--r--  2.0 unx     6392 b- defN 23-May-15 10:39 connio/base/serialize.py
+-rw-r--r--  2.0 unx      255 b- defN 23-May-15 10:39 connio/base/values.py
+-rw-r--r--  2.0 unx     6342 b- defN 23-May-15 10:39 connio/base/version.py
+-rw-r--r--  2.0 unx      403 b- defN 23-May-15 10:39 connio/http/__init__.py
+-rw-r--r--  2.0 unx     2745 b- defN 23-May-15 10:39 connio/http/http_client.py
+-rw-r--r--  2.0 unx     2636 b- defN 23-May-15 10:39 connio/http/request.py
+-rw-r--r--  2.0 unx      375 b- defN 23-May-15 10:39 connio/http/response.py
+-rw-r--r--  2.0 unx     4017 b- defN 23-May-15 10:39 connio/http/validation_client.py
+-rw-r--r--  2.0 unx     4601 b- defN 23-May-15 10:39 connio/rest/__init__.py
+-rw-r--r--  2.0 unx     1280 b- defN 23-May-15 10:39 connio/rest/api/__init__.py
+-rw-r--r--  2.0 unx     3353 b- defN 23-May-15 10:39 connio/rest/api/v3/__init__.py
+-rw-r--r--  2.0 unx    19909 b- defN 23-May-15 10:39 connio/rest/api/v3/account/__init__.py
+-rw-r--r--  2.0 unx    17384 b- defN 23-May-15 10:39 connio/rest/api/v3/account/alert.py
+-rw-r--r--  2.0 unx    16706 b- defN 23-May-15 10:39 connio/rest/api/v3/account/apiclient.py
+-rw-r--r--  2.0 unx     7844 b- defN 23-May-15 10:39 connio/rest/api/v3/account/apikey.py
+-rw-r--r--  2.0 unx    18129 b- defN 23-May-15 10:39 connio/rest/api/v3/account/app.py
+-rw-r--r--  2.0 unx    17868 b- defN 23-May-15 10:39 connio/rest/api/v3/account/appprofile.py
+-rw-r--r--  2.0 unx    10282 b- defN 23-May-15 10:39 connio/rest/api/v3/account/dataconnector.py
+-rw-r--r--  2.0 unx    22686 b- defN 23-May-15 10:39 connio/rest/api/v3/account/device.py
+-rw-r--r--  2.0 unx    17949 b- defN 23-May-15 10:39 connio/rest/api/v3/account/deviceprofile.py
+-rw-r--r--  2.0 unx    17706 b- defN 23-May-15 10:39 connio/rest/api/v3/account/method.py
+-rw-r--r--  2.0 unx    23434 b- defN 23-May-15 10:39 connio/rest/api/v3/account/propertyy.py
+-rw-r--r--  2.0 unx    16506 b- defN 23-May-15 10:39 connio/rest/api/v3/account/user.py
+-rw-r--r--  2.0 unx      765 b- defN 23-May-15 10:39 connio/rest/api/v3/helpers/__init__.py
+-rw-r--r--  2.0 unx    14777 b- defN 23-May-15 10:39 connio/rest/api/v3/sysuser/__init__.py
+-rw-r--r--  2.0 unx      240 b- defN 23-May-15 10:40 conniosdk-0.32.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-15 10:40 conniosdk-0.32.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-May-15 10:40 conniosdk-0.32.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3568 b- defN 23-May-15 10:40 conniosdk-0.32.dist-info/RECORD
+42 files, 285469 bytes uncompressed, 57833 bytes compressed:  79.7%
```

## zipnote {}

```diff
@@ -57,38 +57,14 @@
 
 Filename: connio/http/response.py
 Comment: 
 
 Filename: connio/http/validation_client.py
 Comment: 
 
-Filename: connio/jwt/__init__.py
-Comment: 
-
-Filename: connio/jwt/compat.py
-Comment: 
-
-Filename: connio/jwt/access_token/__init__.py
-Comment: 
-
-Filename: connio/jwt/access_token/grants.py
-Comment: 
-
-Filename: connio/jwt/client/__init__.py
-Comment: 
-
-Filename: connio/jwt/taskrouter/__init__.py
-Comment: 
-
-Filename: connio/jwt/taskrouter/capabilities.py
-Comment: 
-
-Filename: connio/jwt/validation/__init__.py
-Comment: 
-
 Filename: connio/rest/__init__.py
 Comment: 
 
 Filename: connio/rest/api/__init__.py
 Comment: 
 
 Filename: connio/rest/api/v3/__init__.py
@@ -132,20 +108,20 @@
 
 Filename: connio/rest/api/v3/helpers/__init__.py
 Comment: 
 
 Filename: connio/rest/api/v3/sysuser/__init__.py
 Comment: 
 
-Filename: conniosdk-0.31.dist-info/METADATA
+Filename: conniosdk-0.32.dist-info/METADATA
 Comment: 
 
-Filename: conniosdk-0.31.dist-info/WHEEL
+Filename: conniosdk-0.32.dist-info/WHEEL
 Comment: 
 
-Filename: conniosdk-0.31.dist-info/top_level.txt
+Filename: conniosdk-0.32.dist-info/top_level.txt
 Comment: 
 
-Filename: conniosdk-0.31.dist-info/RECORD
+Filename: conniosdk-0.32.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## connio/base/deserialize.py

```diff
@@ -2,61 +2,61 @@
 from decimal import Decimal, BasicContext
 from email.utils import parsedate
 from connio.rest.api.v3.account.__init__ import AccountInstance
 from connio.rest.api.v3.account.propertyy import PropertyInstance
 from connio.rest.api.v3.account.method import MethodInstance
 from connio.rest.api.v3.account.device import DeviceInstance
 from connio.base import values
-import pytz
+
 
 ISO8601_DATE_FORMAT = '%Y-%m-%d'
 ISO8601_DATETIME_FORMAT = '%Y-%m-%dT%H:%M:%S.%fZ'
 ISO8601_DATETIME_FORMAT2 = '%Y-%m-%dT%H:%M:%SZ'
 RFC2822_DATETIME_SPLIT_INDEX = 6
 
 def iso8601_date(s):
     """
     Parses an ISO 8601 date string and returns a UTC date object or the string
     if the parsing failed.
     :param s: ISO 8601-formatted date string (2015-01-25)
     :return:
     """
     try:
-        return datetime.datetime.strptime(s, ISO8601_DATE_FORMAT).replace(tzinfo=pytz.utc).date()
+        return datetime.datetime.strptime(s, ISO8601_DATE_FORMAT).replace(tzinfo=datetime.timezone.utc).date()
     except (TypeError, ValueError):
         return s
 
 
 def iso8601_datetime(s):
     """
     Parses an ISO 8601 datetime string and returns a UTC datetime object,
     or the string if parsing failed.
     :param s: ISO 8601-formatted datetime string (2015-01-25T12:34:56.133Z)
     :return: datetime or str
     """
     try:
-        return datetime.datetime.strptime(s, ISO8601_DATETIME_FORMAT).replace(tzinfo=pytz.utc)
+        return datetime.datetime.strptime(s, ISO8601_DATETIME_FORMAT).replace(tzinfo=datetime.timezone.utc)
     except (TypeError, ValueError):
         try:
-            return datetime.datetime.strptime(s, ISO8601_DATETIME_FORMAT2).replace(tzinfo=pytz.utc)
+            return datetime.datetime.strptime(s, ISO8601_DATETIME_FORMAT2).replace(tzinfo=datetime.timezone.utc)
         except (TypeError, ValueError):
             return s
 
 
 def rfc2822_datetime(s):
     """
     Parses an RFC 2822 date string and returns a UTC datetime object,
     or the string if parsing failed.
     :param s: RFC 2822-formatted string date
     :return: datetime or str
     """
     date_tuple = parsedate(s)
     if date_tuple is None:
         return None
-    return datetime.datetime(*date_tuple[:RFC2822_DATETIME_SPLIT_INDEX]).replace(tzinfo=pytz.utc)
+    return datetime.datetime(*date_tuple[:RFC2822_DATETIME_SPLIT_INDEX]).replace(tzinfo=datetime.timezone.utc)
 
 
 def decimal(d):
     """
     Parses a decimal string into a Decimal
     :param d: decimal string
     :return: Decimal
```

## connio/http/http_client.py

```diff
@@ -44,33 +44,32 @@
             'params': params,
             'json': data,
             'headers': headers,
             'auth': auth,
             'hooks': self.request_hooks
         }
 
-        if params:
-            _logger.debug('{method} Request: {url}?{query}'.format(query=urlencode(params), **kwargs))
-            _logger.debug('PARAMS: {params}'.format(**kwargs))
-        else:
-            _logger.debug('{method} Request: {url}'.format(**kwargs))
-        if data:
-            _logger.debug('PAYLOAD: {json}'.format(**kwargs))
+        #if params:
+        #    _logger.debug('{method} Request: {url}?{query}'.format(query=urlencode(params), **kwargs))
+        #    _logger.debug('PARAMS: {params}'.format(**kwargs))
+        #else:
+        #    _logger.debug('{method} Request: {url}'.format(**kwargs))
+        #if data:
+        #    _logger.debug('PAYLOAD: {json}'.format(**kwargs))
 
         self.last_response = None
         session = self.session or Session()
         request = Request(**kwargs)
         self.last_request = ConnioRequest(**kwargs)
 
         prepped_request = session.prepare_request(request)
         response = session.send(
             prepped_request,
             allow_redirects=allow_redirects,
             timeout=timeout,
         )
         
-        _logger.debug(u'{method} Response: {status} {text}'.format(
-            method=method, status=response.status_code, text=response.text))
+        _logger.debug(f'{method} Response: {response.status_code} {url}')
 
         self.last_response = Response(int(response.status_code), response.text)
 
         return self.last_response
```

## connio/rest/api/v3/account/method.py

```diff
@@ -278,28 +278,29 @@
         Delete Method Instance
         """
         return self._version.delete(
             'DELETE',
             self._uri
         )
 
-    def update(self, name=values.unset, friendly_name=values.unset, method_impl=values.unset):
+    def update(self, name=values.unset, friendly_name=values.unset, method_impl=values.unset, tags=values.unset):
         """
         Update the MethodInstance
 
         :param unicode name: Given name of the entity
         :param unicode friendly_name: A human readable description of this resource
 
         :returns: Updated MethodInstance
         :rtype: connio.rest.api.v3.account.method.MethodInstance
         """
         data = values.of({
             'name': name,
             'friendlyName': friendly_name,
             'methodImpl': serialize.methodImplementation(method_impl),
+            'tags': tags
         })
 
         payload = self._version.update(
             'PUT',
             self._uri,
             data=data,
         )
@@ -515,28 +516,29 @@
         :rtype: connio.rest.api.v3.account.method.MethodInstance
         """
         return self._proxy.fetch()
 
     def delete(self):
         return self._proxy.delete()
 
-    def update(self, name=values.unset, friendly_name=values.unset, method_impl=values.unset):
+    def update(self, name=values.unset, friendly_name=values.unset, method_impl=values.unset, tags=values.unset):
         """
         Update the MethodInstance
 
         :param unicode name: Name of the resource
         :param unicode friendly_name: A human readable description of this resource
 
         :returns: Updated MethodInstance
         :rtype: connio.rest.api.v3.account.method.MethodInstance
         """
         return self._proxy.update(            
             name=name,
             friendly_name=friendly_name,
             method_impl=method_impl,
+            tags=tags
         )
 
     def __getitem__(self, key):
         return self._properties[key]
 
     def __repr__(self):
         """
@@ -549,10 +551,9 @@
         return '<Connio.Api.V3.MethodInstance {}>'.format(context)
 
     def __eq__(self, other):
         return(
             self.access_type == other.access_type and
             self.description == other.description and
             self.friendly_name == other.friendly_name and
-            self.locked == other.locked and
             self.method_impl == other.method_impl
         )
```

## connio/rest/api/v3/account/propertyy.py

```diff
@@ -1,14 +1,15 @@
 
 from connio.base import values
 from connio.base.instance_context import InstanceContext
 from connio.base.instance_resource import InstanceResource
 from connio.base.list_resource import ListResource
 from connio.base.page import Page
 
+
 class PropertyList(ListResource):
     """  """
 
     def __init__(self, version, account_id, owner_id, tags=values.unset):
         """
         Initialize the PropertyList
 
@@ -20,36 +21,36 @@
         """
         super(PropertyList, self).__init__(version)
 
         # Path Solution
         self._solution = {'account_id': account_id, 'owner_id': owner_id, 'tags': tags}
         uri = f'/accounts/{account_id}/properties?owner={owner_id}'
 
-        if(tags is not values.unset):
+        if (tags is not values.unset):
             uri += '&tags='
 
             for tag in tags:
                 uri += f'{tag},'
 
             uri = uri[:-1]
 
         self._uri = uri
 
     def create(self, name, data_type, access_type, publish_type, friendly_name=values.unset, description=values.unset,
-                tags=values.unset, measurement=values.unset, retention=values.unset, boundaries=values.unset, locked=values.unset):
+               tags=values.unset, measurement=values.unset, retention=values.unset, boundaries=values.unset, locked=values.unset):
         """
         Create a new PropertyInstance
 
         :param unicode name: A name uniquely identifying this property within account context
         :param unicode owner_id: Property owner's id
         :param unicode type: Property data type
         :param unicode friendly_name: A human readable description of the application
         :param unicode description: A description of this property
         :param unicode tags: Tags associated with this property
-        
+
         :returns: Newly created PropertyInstance
         :rtype: connio.rest.api.v3.account.property.PropertyInstance
         """
         from connio.base import serialize
 
         data = values.of({
             'name': name,
@@ -57,26 +58,26 @@
             'friendlyName': friendly_name,
             'description': description,
             'tags': tags,
             'type': data_type,
             'access': access_type,
             'publish': publish_type,
             'measurement': serialize.measurement(measurement),
-            'boundaries': serialize.boundaries(boundaries),        
+            'boundaries': serialize.boundaries(boundaries),
             'retention': serialize.retention(retention),
             'locked': locked,
         })
 
         payload = self._version.create(
             'POST',
             self._uri,
             data=data,
         )
 
-        return PropertyInstance(self._version, payload, account_id=self._solution['account_id'], )    
+        return PropertyInstance(self._version, payload, account_id=self._solution['account_id'], )
 
     def stream(self, friendly_name=values.unset, limit=None, page_size=None):
         """
         Streams PropertyInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
         The results are returned as a generator, so this operation is memory efficient.
@@ -115,15 +116,15 @@
         :returns: Generator that will yield up to limit results
         :rtype: list[connio.rest.api.v3.account.property.PropertyInstance]
         """
         return list(self.stream(
             friendly_name=friendly_name,
             limit=limit,
             page_size=page_size,
-            
+
         ))
 
     def page(self, friendly_name=values.unset, page_number=values.unset,
              page_size=values.unset):
         """
         Retrieve a single page of PropertyInstance records from the API.
         Request is executed immediately
@@ -282,25 +283,26 @@
 
         return PropertyInstance(
             self._version,
             payload,
             account_id=self._solution['account_id'],
             id=self._solution['id'],
         )
+
     def delete(self):
         """
         Delete the Property Instance
         """
 
         self._version.delete(
             'DELETE',
             self._uri
         )
 
-    def update(self, name=values.unset, friendly_name=values.unset, measurement=values.unset, tags=values.unset):
+    def update(self, name=values.unset, access_type=values.unset, friendly_name=values.unset, measurement=values.unset, tags=values.unset, retention=values.unset, boundaries=values.unset, publish=values.unset):
         """
         Update the PropertyInstance
 
         :param unicode name: Given name of the entity
         :param unicode friendly_name: A human readable description of this resource
 
         :returns: Updated PropertyInstance
@@ -308,15 +310,19 @@
         """
         from connio.base import serialize
 
         data = values.of({
             'name': name,
             'friendlyName': friendly_name,
             'measurement': serialize.measurement(measurement),
-            'tags': tags
+            'retention': serialize.retention(retention),
+            'boundaries': serialize.boundaries(boundaries),
+            'tags': tags,
+            'publish': publish,
+            'access': access_type
         })
 
         payload = self._version.update(
             'PUT',
             self._uri,
             data=data,
         )
@@ -334,14 +340,15 @@
 
         :returns: Machine friendly representation
         :rtype: str
         """
         context = ' '.join('{}={}'.format(k, v) for k, v in self._solution.items())
         return '<Connio.Api.V3.PropertyContext {}>'.format(context)
 
+
 class PropertyInstance(InstanceResource):
     """  """
 
     class MeasurementUnit(object):
         def __init__(self, label, symbol):
             self.label = label
             self.symbol = symbol
@@ -415,21 +422,23 @@
             CHANGED = "changed"
             CHANGED_BY_X = "changedx"
 
         def __init__(self, when=values.unset, value=values.unset, props=values.unset):
             self.when = when
             self.value = value
             self._properties = props
+
         def __eq__(self, other):
             if type(self) is not type(other):
                 return False
             return (
                 self.when == other.when and
                 self.value == other.value
             )
+
     class Retention(object):
         class RetentionType:
             MOSTRECENT = "mostrecent"
             HISTORICAL = "historical"
 
         def __init__(self, type=values.unset, context=values.unset, lifetime=values.unset, capacity=values.unset, condition=values.unset, props=values.unset):
             self.type = type
@@ -445,15 +454,15 @@
             return (
                 self.capacity == other.capacity and
                 self.type == other.type and
                 self.context == other.context and
                 self.lifetime == other.lifetime and
                 self.condition == other.condition
 
-                )
+            )
 
     def __init__(self, version, payload, account_id, id=None):
         """
         Initialize the PropertyInstance
 
         :returns: connio.rest.api.v3.account.property.PropertyInstance
         :rtype: connio.rest.api.v3.account.property.PropertyInstance
@@ -473,15 +482,15 @@
             'data_type': payload['type'],
             'access_type': payload['access'],
             'publish_type': payload['publish'],
             'retention': deserialize.retention(payload.get('retention')),
             'measurement': deserialize.measurement(payload.get('measurement')),
             'boundaries': deserialize.boundaries(payload.get('boundaries')),
             'inherited': payload['inherited'],
-            'locked': payload['locked'],        
+            'locked': payload['locked'],
             'date_created': deserialize.iso8601_datetime(payload['dateCreated']),
             'date_updated': deserialize.iso8601_datetime(payload['dateModified']),
         })
 
         # Context
         self._context = None
         self._solution = {'account_id': account_id, 'id': id or self._properties['id'], }
@@ -659,29 +668,33 @@
     def delete(self):
         """
         Delete property instance
         """
 
         return self._proxy.delete()
 
-    def update(self, friendly_name=values.unset, name=values.unset, measurement=values.unset, tags=values.unset):
+    def update(self, friendly_name=values.unset, access_type=values.unset, name=values.unset, measurement=values.unset, tags=values.unset, retention=values.unset, boundaries=values.unset, publish=values.unset):
         """
         Update the PropertyInstance
 
         :param unicode name: Name of the resource
         :param unicode friendly_name: A human readable description of this resource
 
         :returns: Updated PropertyInstance
         :rtype: connio.rest.api.v3.account.property.PropertyInstance
         """
         return self._proxy.update(
             friendly_name=friendly_name,
             name=name,
             measurement=measurement,
-            tags=tags
+            tags=tags,
+            retention=retention,
+            boundaries=boundaries,
+            publish=publish,
+            access_type=access_type
         )
 
     def __getitem__(self, key):
         return self._properties[key]
 
     def __eq__(self, other):
         if type(self) is not type(other):
@@ -694,17 +707,16 @@
             self.tags == other.tags and
             self.data_type == other.data_type and
             self.access_type == other.access_type and
             self.publish_type == other.publish_type and
             self.retention == other.retention and
             self.boundaries == other.boundaries and
             self.measurement == other.measurement and
-            self.locked == other.locked and
             self.inherited == other.inherited
-            )
+        )
 
     def __repr__(self):
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         :rtype: str
```

## Comparing `conniosdk-0.31.dist-info/RECORD` & `conniosdk-0.32.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,42 @@
 connio/__init__.py,sha256=eAQQjys9UpTS4X-QQu0JNX1Q8AT29Pt9ia-GIyIrtGw,92
 connio/compat.py,sha256=wwaagRDY7MRZidjcjw4zsvcrdW5XR3SOtd4ElwDWreg,497
 connio/mqtt.py,sha256=hV0ovCYNZsD_vRerXQgHG3Thk5DnP9Wc366ELh7snFU,6054
 connio/request_validator.py,sha256=EIldM0-pIlQ82OC6V4e5qEbdMpVGFBmSV_kjxUeAp-4,2323
 connio/base/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-connio/base/deserialize.py,sha256=wYtOEx-SxvPGkOZxgLX_c65gdWlIDwieiIlSuPA3S-A,8271
+connio/base/deserialize.py,sha256=pfxdF0DZLKQ0t3wCmb_MeAfDJooVAMDF6yImLhG6-tY,8312
 connio/base/domain.py,sha256=eQQj5nlyjUAG_OcarK-1Fps3etwOWl2eEBbGota-azA,1519
 connio/base/exceptions.py,sha256=zy0oUyS5ONJ0iP247pawMQtw8wX1kjQCSMc23FAXZP0,2552
 connio/base/instance_context.py,sha256=vK1QRsnow1l2XaMllv75ABx8DsO03GPQMNRbXf7eY9I,184
 connio/base/instance_resource.py,sha256=rcTRsriVKgLu6aaOOhBqs4IfI-skR8dXPcmf38I85Cs,185
 connio/base/list_resource.py,sha256=JJCMsjojJf51dJsK986zw93RnsQl7dnopFY-tINxzl0,180
 connio/base/obsolete.py,sha256=mrS5WSpQdYW45ZaFxFfhmmvtGVcyTZAdWnYhXCKkDDw,636
 connio/base/page.py,sha256=qwNfyaaAKNCKQ1HDpgPpd-VLcmWLaw0kBvPgkJOT98Y,4684
 connio/base/serialize.py,sha256=p3aBI3KPnbNBcHyiaaH-onod9XH_RAyl3cYKAK3tvGg,6392
 connio/base/values.py,sha256=AXZogycx8UBXapsQfB8NVzEcRSM6MvNIFJFEvm0y8j0,255
 connio/base/version.py,sha256=ZZTpeUtwvuGYi_cmtYiAKkw-KRC9qaPVf5zWBf0d-z8,6342
 connio/http/__init__.py,sha256=Xpd-zeYja2sxrMkFzEV3ophHNEchyVXyf_73NxBEplI,403
-connio/http/http_client.py,sha256=qPpysTAPzpIsfvSsgeCpyOGE9817AEEzfFrzzqHJSvY,2809
+connio/http/http_client.py,sha256=oQLT--xWHO9NM8q9AmEjdMHlKnwd84dHb96EGvb11ss,2745
 connio/http/request.py,sha256=wNPnmArjEf_HUfWPr5vVJDjU9CbAe0n2jb_o7o7TQoE,2636
 connio/http/response.py,sha256=7ssIl8aftT8r5TI0OMbnIov4ET4LEhzODe2LSbF7uoo,375
 connio/http/validation_client.py,sha256=VxPY9_4yOAxi0wD8YETkQvTheAY7c_YXFRLs98oeGDY,4017
-connio/jwt/__init__.py,sha256=O45lzbEMp71WWfwX6WniMbEbNOwJcwGWEaWDUtH-ECc,5206
-connio/jwt/compat.py,sha256=U7Fj0xdLttm7TSprbZwkPFxiRav7HmQ8CR3syF0asi8,1118
-connio/jwt/access_token/__init__.py,sha256=YFCEJ2zZzUmoNV16L1Oe9ZvPMKues2-6MnSAjkDVbVI,2143
-connio/jwt/access_token/grants.py,sha256=-IMKUxFWH6VviojjGT3bDVGp4IBXsFgtZAHac5WOjyA,5841
-connio/jwt/client/__init__.py,sha256=nu8nyDtVGNnV9BdFafeJ0CLRql6K36UNvMoCTI1neO4,3891
-connio/jwt/taskrouter/__init__.py,sha256=x77SfMExJNw7r-gXMKJwBmZQPlSPsVi_moltDOl-BGk,5584
-connio/jwt/taskrouter/capabilities.py,sha256=SjPw9BF3s0fot1jqRn1V4EyAtOM9PjdOI1Ik1nh1JV0,4281
-connio/jwt/validation/__init__.py,sha256=b6Mo8uFmW2uvILQP3IZL-femI_4xokrrxodTgysXPSM,3140
 connio/rest/__init__.py,sha256=4XzIpJ1qL-GOTIHxu0U-XwseWGMmjNcPu4CSzIzywfk,4601
 connio/rest/api/__init__.py,sha256=-dku619BUh-RDBsmxWl68cK_Es3q74CS0aW98ykbs5Q,1280
 connio/rest/api/v3/__init__.py,sha256=EXg1GwJC6lSXl2VoRbH8a6LKULz-tgnjwKUtkqzAAhU,3353
 connio/rest/api/v3/account/__init__.py,sha256=a4n2kT_Ww6g1Xq7GGp0naPoSNrLgnOTO_igVdlzA9p4,19909
 connio/rest/api/v3/account/alert.py,sha256=Ep4GLHpldY7vAbE-pQ5hcf5CGeMd1vvaonPbYooCWHQ,17384
 connio/rest/api/v3/account/apiclient.py,sha256=csnFlbQ4kVHl_RCdPG36CuamdZPnzHJNcwwpZplQqv0,16706
 connio/rest/api/v3/account/apikey.py,sha256=u5401V9aPQszXaMqnC_80NkMgDyNtEL_GpqqVaFxCUk,7844
 connio/rest/api/v3/account/app.py,sha256=Oqe4N7RNKXVUAP0p2FkD-ddCvmBpk72TNxaTcyTjvoA,18129
 connio/rest/api/v3/account/appprofile.py,sha256=aAopXtskewv1_lPLNqHnPP9vchi8q4NfypB5YtLOEds,17868
 connio/rest/api/v3/account/dataconnector.py,sha256=RadWkaErK9cT8lboW66p88_ZqO0ZqUnTaKcIxPxM1U4,10282
 connio/rest/api/v3/account/device.py,sha256=V2jBqznHy3d-1g-cqqF-vjUIfU-GAJxV1LNNBWU0-2A,22686
 connio/rest/api/v3/account/deviceprofile.py,sha256=iZdkPx3ELM576XSg2hgcS7q5q1_McuNXt97tM6FIL-A,17949
-connio/rest/api/v3/account/method.py,sha256=QoT8DIGr2i5GAuGsIQiWKZWIx-PtsMhkEoM9VcvLMYQ,17665
-connio/rest/api/v3/account/propertyy.py,sha256=zVeTzDjQeqvbGVLe3YqBfVW0D7xr6v7lFwxhHKAmTS8,23009
+connio/rest/api/v3/account/method.py,sha256=kBfZMoh-ZuF308fBBSTCcSaKBZ1L2qW2WWej8ZVBiAo,17706
+connio/rest/api/v3/account/propertyy.py,sha256=20xw7pWxsHaM-CZR_4KZ9wBHpytRetQdGotS4WaWZzw,23434
 connio/rest/api/v3/account/user.py,sha256=tGOGpmWFcTNo5AUj55Bblv0yj9w-H73c_yE8VorUFvA,16506
 connio/rest/api/v3/helpers/__init__.py,sha256=jvyIyPSbB_W1OfQAfcfU7U56WwFjGolhqalRYDsMsXc,765
 connio/rest/api/v3/sysuser/__init__.py,sha256=BoUrEdWXTtQT9iZsKTjGI5E0bOD2HEj8gN1qXo9JkEc,14777
-conniosdk-0.31.dist-info/METADATA,sha256=fVqLJ6qlOUlKywggMIdsPFivx5HzJy9wi85F-uZ2g7o,282
-conniosdk-0.31.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-conniosdk-0.31.dist-info/top_level.txt,sha256=pEc3eVyv8DDXpe1mNVxQJuhOBEIl7Wtk4dyjxQesvvM,7
-conniosdk-0.31.dist-info/RECORD,,
+conniosdk-0.32.dist-info/METADATA,sha256=P2RaKbSRw4YNCTJVyD8DCtWp5fHWPGOu2JxHOTOXCpU,240
+conniosdk-0.32.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+conniosdk-0.32.dist-info/top_level.txt,sha256=pEc3eVyv8DDXpe1mNVxQJuhOBEIl7Wtk4dyjxQesvvM,7
+conniosdk-0.32.dist-info/RECORD,,
```

