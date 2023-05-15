# Comparing `tmp/cloudinary-1.8.0.tar.gz` & `tmp/cloudinary-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cloudinary-1.8.0.tar", last modified: Wed May  3 14:58:31 2017, max compression
+gzip compressed data, was "dist/cloudinary-1.9.0.tar", last modified: Sat Dec  2 23:41:52 2017, max compression
```

## Comparing `cloudinary-1.8.0.tar` & `cloudinary-1.9.0.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 amir       (502) staff       (20)        0 2017-05-03 14:58:31.000000 cloudinary-1.8.0/
-drwxr-xr-x   0 amir       (502) staff       (20)        0 2017-05-03 14:58:31.000000 cloudinary-1.8.0/cloudinary/
--rw-r--r--   0 amir       (502) staff       (20)    11490 2017-05-03 14:46:04.000000 cloudinary-1.8.0/cloudinary/__init__.py
--rw-r--r--   0 amir       (502) staff       (20)    13362 2017-05-03 11:02:57.000000 cloudinary-1.8.0/cloudinary/api.py
--rw-r--r--   0 amir       (502) staff       (20)     1521 2017-02-22 23:31:06.000000 cloudinary-1.8.0/cloudinary/auth_token.py
--rw-r--r--   0 amir       (502) staff       (20)      932 2017-04-29 21:35:34.000000 cloudinary-1.8.0/cloudinary/compat.py
--rw-r--r--   0 amir       (502) staff       (20)     5082 2016-11-17 00:50:31.000000 cloudinary-1.8.0/cloudinary/forms.py
--rw-r--r--   0 amir       (502) staff       (20)     3984 2016-11-17 02:11:32.000000 cloudinary-1.8.0/cloudinary/models.py
-drwxr-xr-x   0 amir       (502) staff       (20)        0 2017-05-03 14:58:31.000000 cloudinary-1.8.0/cloudinary/poster/
--rw-r--r--   0 amir       (502) staff       (20)     1575 2015-02-02 10:25:54.000000 cloudinary-1.8.0/cloudinary/poster/__init__.py
--rw-r--r--   0 amir       (502) staff       (20)    16005 2016-02-01 13:07:15.000000 cloudinary-1.8.0/cloudinary/poster/encode.py
--rw-r--r--   0 amir       (502) staff       (20)     8184 2016-11-16 20:14:05.000000 cloudinary-1.8.0/cloudinary/poster/streaminghttp.py
--rw-r--r--   0 amir       (502) staff       (20)     1732 2017-05-03 11:02:57.000000 cloudinary-1.8.0/cloudinary/search.py
-drwxr-xr-x   0 amir       (502) staff       (20)        0 2017-05-03 14:58:31.000000 cloudinary-1.8.0/cloudinary/static/
-drwxr-xr-x   0 amir       (502) staff       (20)        0 2017-05-03 14:58:31.000000 cloudinary-1.8.0/cloudinary/static/html/
--rw-r--r--   0 amir       (502) staff       (20)     3899 2017-03-27 13:18:05.000000 cloudinary-1.8.0/cloudinary/static/html/cloudinary_cors.html
-drwxr-xr-x   0 amir       (502) staff       (20)        0 2017-05-03 14:58:31.000000 cloudinary-1.8.0/cloudinary/static/js/
--rw-r--r--   0 amir       (502) staff       (20)     1212 2017-03-27 13:18:05.000000 cloudinary-1.8.0/cloudinary/static/js/canvas-to-blob.min.js
--rw-r--r--   0 amir       (502) staff       (20)   140946 2017-03-27 13:18:05.000000 cloudinary-1.8.0/cloudinary/static/js/jquery.cloudinary.js
--rw-r--r--   0 amir       (502) staff       (20)    12207 2017-03-27 13:18:05.000000 cloudinary-1.8.0/cloudinary/static/js/jquery.fileupload-image.js
--rw-r--r--   0 amir       (502) staff       (20)     6098 2017-03-27 13:18:05.000000 cloudinary-1.8.0/cloudinary/static/js/jquery.fileupload-process.js
--rw-r--r--   0 amir       (502) staff       (20)     4177 2017-03-27 13:18:05.000000 cloudinary-1.8.0/cloudinary/static/js/jquery.fileupload-validate.js
--rw-r--r--   0 amir       (502) staff       (20)    63667 2017-03-27 13:18:05.000000 cloudinary-1.8.0/cloudinary/static/js/jquery.fileupload.js
--rw-r--r--   0 amir       (502) staff       (20)    10724 2017-03-27 13:18:05.000000 cloudinary-1.8.0/cloudinary/static/js/jquery.iframe-transport.js
--rw-r--r--   0 amir       (502) staff       (20)    16089 2017-03-27 13:18:05.000000 cloudinary-1.8.0/cloudinary/static/js/jquery.ui.widget.js
--rw-r--r--   0 amir       (502) staff       (20)    16819 2017-03-27 13:18:05.000000 cloudinary-1.8.0/cloudinary/static/js/load-image.all.min.js
-drwxr-xr-x   0 amir       (502) staff       (20)        0 2017-05-03 14:58:31.000000 cloudinary-1.8.0/cloudinary/templates/
--rw-r--r--   0 amir       (502) staff       (20)      365 2015-02-02 10:25:54.000000 cloudinary-1.8.0/cloudinary/templates/cloudinary_direct_upload.html
--rw-r--r--   0 amir       (502) staff       (20)      861 2016-01-18 14:03:53.000000 cloudinary-1.8.0/cloudinary/templates/cloudinary_includes.html
--rw-r--r--   0 amir       (502) staff       (20)       84 2015-02-02 10:25:54.000000 cloudinary-1.8.0/cloudinary/templates/cloudinary_js_config.html
-drwxr-xr-x   0 amir       (502) staff       (20)        0 2017-05-03 14:58:31.000000 cloudinary-1.8.0/cloudinary/templatetags/
--rw-r--r--   0 amir       (502) staff       (20)        2 2015-02-02 10:25:54.000000 cloudinary-1.8.0/cloudinary/templatetags/__init__.py
--rw-r--r--   0 amir       (502) staff       (20)     2845 2017-04-30 04:04:55.000000 cloudinary-1.8.0/cloudinary/templatetags/cloudinary.py
--rw-r--r--   0 amir       (502) staff       (20)     8991 2016-11-17 00:50:31.000000 cloudinary-1.8.0/cloudinary/uploader.py
--rw-r--r--   0 amir       (502) staff       (20)    29843 2017-04-29 20:31:04.000000 cloudinary-1.8.0/cloudinary/utils.py
-drwxr-xr-x   0 amir       (502) staff       (20)        0 2017-05-03 14:58:31.000000 cloudinary-1.8.0/cloudinary.egg-info/
--rw-r--r--   0 amir       (502) staff       (20)        1 2017-05-03 14:58:31.000000 cloudinary-1.8.0/cloudinary.egg-info/dependency_links.txt
--rw-r--r--   0 amir       (502) staff       (20)        1 2015-02-02 10:25:54.000000 cloudinary-1.8.0/cloudinary.egg-info/not-zip-safe
--rw-r--r--   0 amir       (502) staff       (20)    18226 2017-05-03 14:58:31.000000 cloudinary-1.8.0/cloudinary.egg-info/PKG-INFO
--rw-r--r--   0 amir       (502) staff       (20)       17 2017-05-03 14:58:31.000000 cloudinary-1.8.0/cloudinary.egg-info/requires.txt
--rw-r--r--   0 amir       (502) staff       (20)     1210 2017-05-03 14:58:31.000000 cloudinary-1.8.0/cloudinary.egg-info/SOURCES.txt
--rw-r--r--   0 amir       (502) staff       (20)       11 2017-05-03 14:58:31.000000 cloudinary-1.8.0/cloudinary.egg-info/top_level.txt
--rw-r--r--   0 amir       (502) staff       (20)      107 2015-02-02 10:25:54.000000 cloudinary-1.8.0/LICENSE.txt
--rw-r--r--   0 amir       (502) staff       (20)      127 2016-11-17 00:50:31.000000 cloudinary-1.8.0/MANIFEST.in
--rw-r--r--   0 amir       (502) staff       (20)    18226 2017-05-03 14:58:31.000000 cloudinary-1.8.0/PKG-INFO
--rw-r--r--   0 amir       (502) staff       (20)    13113 2016-11-17 00:50:31.000000 cloudinary-1.8.0/README.rst
--rw-r--r--   0 amir       (502) staff       (20)       59 2017-05-03 14:58:31.000000 cloudinary-1.8.0/setup.cfg
--rw-r--r--   0 amir       (502) staff       (20)     2180 2017-05-03 14:46:04.000000 cloudinary-1.8.0/setup.py
+drwxr-xr-x   0 amir       (501) staff       (20)        0 2017-12-02 23:41:52.000000 cloudinary-1.9.0/
+-rw-r--r--   0 amir       (501) staff       (20)      107 2017-08-09 04:12:31.000000 cloudinary-1.9.0/LICENSE.txt
+-rw-r--r--   0 amir       (501) staff       (20)      127 2017-08-09 04:12:31.000000 cloudinary-1.9.0/MANIFEST.in
+-rw-r--r--   0 amir       (501) staff       (20)    18345 2017-12-02 23:41:52.000000 cloudinary-1.9.0/PKG-INFO
+-rw-r--r--   0 amir       (501) staff       (20)    13113 2017-08-09 09:08:38.000000 cloudinary-1.9.0/README.rst
+-rw-r--r--   0 amir       (501) staff       (20)      309 2017-11-27 10:10:31.000000 cloudinary-1.9.0/branches.txt
+drwxr-xr-x   0 amir       (501) staff       (20)        0 2017-12-02 23:41:52.000000 cloudinary-1.9.0/cloudinary/
+-rw-r--r--   0 amir       (501) staff       (20)    11490 2017-12-02 23:19:13.000000 cloudinary-1.9.0/cloudinary/__init__.py
+-rw-r--r--   0 amir       (501) staff       (20)    14566 2017-12-02 22:12:22.000000 cloudinary-1.9.0/cloudinary/api.py
+-rw-r--r--   0 amir       (501) staff       (20)     1521 2017-11-29 06:32:21.000000 cloudinary-1.9.0/cloudinary/auth_token.py
+-rw-r--r--   0 amir       (501) staff       (20)      932 2017-11-29 06:32:21.000000 cloudinary-1.9.0/cloudinary/compat.py
+-rw-r--r--   0 amir       (501) staff       (20)     5082 2017-11-29 06:32:21.000000 cloudinary-1.9.0/cloudinary/forms.py
+-rw-r--r--   0 amir       (501) staff       (20)     3984 2017-11-29 09:43:34.000000 cloudinary-1.9.0/cloudinary/models.py
+drwxr-xr-x   0 amir       (501) staff       (20)        0 2017-12-02 23:41:52.000000 cloudinary-1.9.0/cloudinary/poster/
+-rw-r--r--   0 amir       (501) staff       (20)     1575 2017-11-29 06:32:21.000000 cloudinary-1.9.0/cloudinary/poster/__init__.py
+-rw-r--r--   0 amir       (501) staff       (20)    16005 2017-11-29 06:32:21.000000 cloudinary-1.9.0/cloudinary/poster/encode.py
+-rw-r--r--   0 amir       (501) staff       (20)     8184 2017-11-29 06:32:21.000000 cloudinary-1.9.0/cloudinary/poster/streaminghttp.py
+-rw-r--r--   0 amir       (501) staff       (20)     1732 2017-11-29 06:32:21.000000 cloudinary-1.9.0/cloudinary/search.py
+drwxr-xr-x   0 amir       (501) staff       (20)        0 2017-12-02 23:41:52.000000 cloudinary-1.9.0/cloudinary/static/
+drwxr-xr-x   0 amir       (501) staff       (20)        0 2017-12-02 23:41:52.000000 cloudinary-1.9.0/cloudinary/static/html/
+-rw-r--r--   0 amir       (501) staff       (20)     3899 2017-11-14 10:33:44.000000 cloudinary-1.9.0/cloudinary/static/html/cloudinary_cors.html
+drwxr-xr-x   0 amir       (501) staff       (20)        0 2017-12-02 23:41:52.000000 cloudinary-1.9.0/cloudinary/static/js/
+-rw-r--r--   0 amir       (501) staff       (20)     1273 2017-11-14 10:33:44.000000 cloudinary-1.9.0/cloudinary/static/js/canvas-to-blob.min.js
+-rw-r--r--   0 amir       (501) staff       (20)   146802 2017-11-14 10:33:44.000000 cloudinary-1.9.0/cloudinary/static/js/jquery.cloudinary.js
+-rw-r--r--   0 amir       (501) staff       (20)    12299 2017-11-14 10:33:44.000000 cloudinary-1.9.0/cloudinary/static/js/jquery.fileupload-image.js
+-rw-r--r--   0 amir       (501) staff       (20)     6161 2017-11-14 10:33:44.000000 cloudinary-1.9.0/cloudinary/static/js/jquery.fileupload-process.js
+-rw-r--r--   0 amir       (501) staff       (20)     4248 2017-11-14 10:33:44.000000 cloudinary-1.9.0/cloudinary/static/js/jquery.fileupload-validate.js
+-rw-r--r--   0 amir       (501) staff       (20)    63855 2017-11-14 10:33:44.000000 cloudinary-1.9.0/cloudinary/static/js/jquery.fileupload.js
+-rw-r--r--   0 amir       (501) staff       (20)    10891 2017-11-14 10:33:44.000000 cloudinary-1.9.0/cloudinary/static/js/jquery.iframe-transport.js
+-rw-r--r--   0 amir       (501) staff       (20)    16089 2017-11-14 10:33:44.000000 cloudinary-1.9.0/cloudinary/static/js/jquery.ui.widget.js
+-rw-r--r--   0 amir       (501) staff       (20)    17734 2017-11-14 10:33:44.000000 cloudinary-1.9.0/cloudinary/static/js/load-image.all.min.js
+drwxr-xr-x   0 amir       (501) staff       (20)        0 2017-12-02 23:41:52.000000 cloudinary-1.9.0/cloudinary/templates/
+-rw-r--r--   0 amir       (501) staff       (20)      365 2017-08-09 04:12:31.000000 cloudinary-1.9.0/cloudinary/templates/cloudinary_direct_upload.html
+-rw-r--r--   0 amir       (501) staff       (20)      861 2017-08-09 04:12:31.000000 cloudinary-1.9.0/cloudinary/templates/cloudinary_includes.html
+-rw-r--r--   0 amir       (501) staff       (20)       84 2017-08-09 04:12:31.000000 cloudinary-1.9.0/cloudinary/templates/cloudinary_js_config.html
+drwxr-xr-x   0 amir       (501) staff       (20)        0 2017-12-02 23:41:52.000000 cloudinary-1.9.0/cloudinary/templatetags/
+-rw-r--r--   0 amir       (501) staff       (20)        2 2017-08-09 04:12:31.000000 cloudinary-1.9.0/cloudinary/templatetags/__init__.py
+-rw-r--r--   0 amir       (501) staff       (20)     2845 2017-11-29 06:32:21.000000 cloudinary-1.9.0/cloudinary/templatetags/cloudinary.py
+-rw-r--r--   0 amir       (501) staff       (20)     9079 2017-12-01 15:18:14.000000 cloudinary-1.9.0/cloudinary/uploader.py
+-rw-r--r--   0 amir       (501) staff       (20)    29888 2017-12-01 15:18:14.000000 cloudinary-1.9.0/cloudinary/utils.py
+drwxr-xr-x   0 amir       (501) staff       (20)        0 2017-12-02 23:41:52.000000 cloudinary-1.9.0/cloudinary.egg-info/
+-rw-r--r--   0 amir       (501) staff       (20)    18345 2017-12-02 23:41:52.000000 cloudinary-1.9.0/cloudinary.egg-info/PKG-INFO
+-rw-r--r--   0 amir       (501) staff       (20)     1223 2017-12-02 23:41:52.000000 cloudinary-1.9.0/cloudinary.egg-info/SOURCES.txt
+-rw-r--r--   0 amir       (501) staff       (20)        1 2017-12-02 23:41:52.000000 cloudinary-1.9.0/cloudinary.egg-info/dependency_links.txt
+-rw-r--r--   0 amir       (501) staff       (20)        1 2017-12-02 23:31:45.000000 cloudinary-1.9.0/cloudinary.egg-info/not-zip-safe
+-rw-r--r--   0 amir       (501) staff       (20)       25 2017-12-02 23:41:52.000000 cloudinary-1.9.0/cloudinary.egg-info/requires.txt
+-rw-r--r--   0 amir       (501) staff       (20)       11 2017-12-02 23:41:52.000000 cloudinary-1.9.0/cloudinary.egg-info/top_level.txt
+-rw-r--r--   0 amir       (501) staff       (20)       38 2017-12-02 23:41:52.000000 cloudinary-1.9.0/setup.cfg
+-rw-r--r--   0 amir       (501) staff       (20)     2289 2017-12-02 23:19:13.000000 cloudinary-1.9.0/setup.py
```

### Comparing `cloudinary-1.8.0/cloudinary/__init__.py` & `cloudinary-1.9.0/cloudinary/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 CF_SHARED_CDN = "d3jpl91pxevbkh.cloudfront.net"
 OLD_AKAMAI_SHARED_CDN = "cloudinary-a.akamaihd.net"
 AKAMAI_SHARED_CDN = "res.cloudinary.com"
 SHARED_CDN = AKAMAI_SHARED_CDN
 CL_BLANK = "data:image/gif;base64,R0lGODlhAQABAIAAAAAAAP///yH5BAEAAAAALAAAAAABAAEAAAIBRAA7"
 
-VERSION = "1.8.0"
+VERSION = "1.9.0"
 USER_AGENT = "CloudinaryPython/" + VERSION
 """ :const: USER_AGENT """
 
 USER_PLATFORM = ""
 """
 Additional information to be passed with the USER_AGENT, e.g. "CloudinaryMagento/1.0.1".
 This value is set in platform-specific implementations that use cloudinary_php.
```

### Comparing `cloudinary-1.8.0/cloudinary/api.py` & `cloudinary-1.9.0/cloudinary/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import json
 import socket
 
 import cloudinary
 from six import string_types
 
 import urllib3
+import certifi
+
 from cloudinary import utils
 from urllib3.exceptions import HTTPError
 
 logger = cloudinary.logger
 
 class Error(Exception): pass
 class NotFound(Error): pass
@@ -36,15 +38,18 @@
     def __init__(self, result, response, **kwargs):
         super(Response, self).__init__(**kwargs)
         self.update(result)
         self.rate_limit_allowed = int(response.headers["x-featureratelimit-limit"])
         self.rate_limit_reset_at = email.utils.parsedate(response.headers["x-featureratelimit-reset"])
         self.rate_limit_remaining = int(response.headers["x-featureratelimit-remaining"])
 
-_http = urllib3.PoolManager()
+_http = urllib3.PoolManager(
+        cert_reqs='CERT_REQUIRED',
+        ca_certs=certifi.where()
+        )
 
 
 def ping(**options):
     return call_api("get", ["ping"], {}, **options)
 
 
 def usage(**options):
@@ -150,14 +155,38 @@
 def delete_derived_resources(derived_resource_ids, **options):
     uri = ["derived_resources"]
     params = [("derived_resource_ids[]", derived_resource_id) for derived_resource_id in derived_resource_ids]
 
     return call_api("delete", uri, params, **options)
 
 
+def delete_derived_by_transformation(public_ids, transformations, resource_type='image', type='upload', invalidate=None, **options):
+    """
+    Delete derived resources of public ids, identified by transformations
+    
+    :param public_ids: the base resources
+    :type public_ids: list of string
+    :param transformations: the transformation of derived resources, optionally including the format
+    :type transformations: list of (dict or string)
+    :param invalidate: (optional) True to invalidate the resources after deletion
+    :type invalidate: bool
+    :return: a list of the public ids for which derived resources were deleted
+    :rtype: dict
+    """
+    uri = ["resources", resource_type, type]
+    if not isinstance(public_ids, list):
+        public_ids = [public_ids]
+    params = [("public_ids[]", public_id) for public_id in public_ids]
+    params.append(("transformations", utils.build_eager(transformations)))
+    params.append(("keep_original", True))
+    if invalidate is not None:
+        params.append(('invalidate', invalidate))
+    return call_api("delete", uri, params, **options)
+
+
 def tags(**options):
     resource_type = options.pop("resource_type", "image")
     uri = ["tags", resource_type]
     return call_api("get", uri, only(options, "next_cursor", "max_results", "prefix"), **options)
 
 
 def transformations(**options):
```

### Comparing `cloudinary-1.8.0/cloudinary/auth_token.py` & `cloudinary-1.9.0/cloudinary/auth_token.py`

 * *Files identical despite different names*

### Comparing `cloudinary-1.8.0/cloudinary/compat.py` & `cloudinary-1.9.0/cloudinary/compat.py`

 * *Files identical despite different names*

### Comparing `cloudinary-1.8.0/cloudinary/forms.py` & `cloudinary-1.9.0/cloudinary/forms.py`

 * *Files identical despite different names*

### Comparing `cloudinary-1.8.0/cloudinary/models.py` & `cloudinary-1.9.0/cloudinary/models.py`

 * *Files identical despite different names*

### Comparing `cloudinary-1.8.0/cloudinary/poster/__init__.py` & `cloudinary-1.9.0/cloudinary/poster/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudinary-1.8.0/cloudinary/poster/encode.py` & `cloudinary-1.9.0/cloudinary/poster/encode.py`

 * *Files identical despite different names*

### Comparing `cloudinary-1.8.0/cloudinary/poster/streaminghttp.py` & `cloudinary-1.9.0/cloudinary/poster/streaminghttp.py`

 * *Files identical despite different names*

### Comparing `cloudinary-1.8.0/cloudinary/search.py` & `cloudinary-1.9.0/cloudinary/search.py`

 * *Files identical despite different names*

### Comparing `cloudinary-1.8.0/cloudinary/static/html/cloudinary_cors.html` & `cloudinary-1.9.0/cloudinary/static/html/cloudinary_cors.html`

 * *Files identical despite different names*

### Comparing `cloudinary-1.8.0/cloudinary/static/js/jquery.cloudinary.js` & `cloudinary-1.9.0/cloudinary/static/js/jquery.cloudinary.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -37,50 +37,93 @@
         return results;
     }
 })(this, function(jQuery) {
 
     /*
      * Includes common utility methods and shims
      */
-    var ArrayParam, BaseUtil, ClientHintsMetaTag, Cloudinary, CloudinaryJQuery, Condition, Configuration, Expression, ExpressionParam, HtmlTag, ImageTag, Layer, LayerParam, Param, RangeParam, RawParam, SubtitlesLayer, TextLayer, Transformation, TransformationBase, TransformationParam, Util, VideoTag, addClass, allStrings, camelCase, cloneDeep, cloudinary, compact, contains, convertKeys, crc32, defaults, difference, functions, getAttribute, getData, hasClass, identity, isEmpty, isNumberLike, isString, m, merge, parameters, reWords, removeAttribute, setAttribute, setAttributes, setData, smartEscape, snakeCase, utf8_encode, webp, width, withCamelCaseKeys, withSnakeCaseKeys, without;
+
+    /**
+     * Return true if all items in list are strings
+     * @function Util.allString
+     * @param {Array} list - an array of items
+     */
+    var ArrayParam, BaseUtil, ClientHintsMetaTag, Cloudinary, CloudinaryJQuery, Condition, Configuration, Expression, ExpressionParam, FetchLayer, HtmlTag, ImageTag, Layer, LayerParam, Param, RangeParam, RawParam, SubtitlesLayer, TextLayer, Transformation, TransformationBase, TransformationParam, Util, VideoTag, addClass, allStrings, base64Encode, base64EncodeURL, camelCase, cloneDeep, cloudinary, compact, contains, convertKeys, crc32, defaults, difference, funcTag, functions, getAttribute, getData, hasClass, identity, isEmpty, isFunction, isNumberLike, isObject, isString, m, merge, objToString, objectProto, parameters, reWords, removeAttribute, setAttribute, setAttributes, setData, smartEscape, snakeCase, utf8_encode, webp, width, withCamelCaseKeys, withSnakeCaseKeys, without;
     allStrings = function(list) {
         var item, j, len;
         for (j = 0, len = list.length; j < len; j++) {
             item = list[j];
             if (!Util.isString(item)) {
                 return false;
             }
         }
         return true;
     };
+
+    /**
+     * Creates a new array without the given item.
+     * @function Util.without
+     * @param {Array} array - original array
+     * @param {*} item - the item to exclude from the new array
+     * @return {Array} a new array made of the original array's items except for `item`
+     */
     without = function(array, item) {
         var i, length, newArray;
         newArray = [];
         i = -1;
         length = array.length;
         while (++i < length) {
             if (array[i] !== item) {
                 newArray.push(array[i]);
             }
         }
         return newArray;
     };
+
+    /**
+     * Return true is value is a number or a string representation of a number.
+     * @function Util.isNumberLike
+     * @param {*} value
+     * @returns {boolean} true if value is a number
+     * @example
+     *    Util.isNumber(0) // true
+     *    Util.isNumber("1.3") // true
+     *    Util.isNumber("") // false
+     *    Util.isNumber(undefined) // false
+     */
     isNumberLike = function(value) {
         return (value != null) && !isNaN(parseFloat(value));
     };
+
+    /**
+     * Escape all characters matching unsafe in the given string
+     * @function Util.smartEscape
+     * @param {string} string - source string to escape
+     * @param {RegExp} unsafe - characters that must be escaped
+     * @return {string} escaped string
+     */
     smartEscape = function(string, unsafe) {
         if (unsafe == null) {
             unsafe = /([^a-zA-Z0-9_.\-\/:]+)/g;
         }
         return string.replace(unsafe, function(match) {
             return match.split("").map(function(c) {
                 return "%" + c.charCodeAt(0).toString(16).toUpperCase();
             }).join("");
         });
     };
+
+    /**
+     * Assign values from sources if they are not defined in the destination.
+     * Once a value is set it does not change
+     * @function Util.defaults
+     * @param {Object} destination - the object to assign defaults to
+     * @param {...Object} source - the source object(s) to assign defaults from
+     * @return {Object} destination after it was modified
+     */
     defaults = function() {
         var destination, sources;
         destination = arguments[0], sources = 2 <= arguments.length ? slice.call(arguments, 1) : [];
         return sources.reduce(function(dest, source) {
             var key, value;
             for (key in source) {
                 value = source[key];
@@ -88,21 +131,81 @@
                     dest[key] = value;
                 }
             }
             return dest;
         }, destination);
     };
 
+    /*********** lodash functions */
+    objectProto = Object.prototype;
+
+    /**
+     * Used to resolve the [`toStringTag`](http://ecma-international.org/ecma-262/6.0/#sec-object.prototype.tostring)
+     * of values.
+     */
+    objToString = objectProto.toString;
+
+    /**
+     * Checks if `value` is the [language type](https://es5.github.io/#x8) of `Object`.
+     * (e.g. arrays, functions, objects, regexes, `new Number(0)`, and `new String('')`)
+     *
+     * @param {*} value The value to check.
+     * @returns {boolean} Returns `true` if `value` is an object, else `false`.
+     * @example
+     *
+    #isObject({});
+     * // => true
+     *
+    #isObject([1, 2, 3]);
+     * // => true
+     *
+    #isObject(1);
+     * // => false
+     */
+    isObject = function(value) {
+        var type;
+        type = typeof value;
+        return !!value && (type === 'object' || type === 'function');
+    };
+    funcTag = '[object Function]';
+
+    /**
+     * Checks if `value` is classified as a `Function` object.
+     * @function Util.isFunction
+     * @param {*} value The value to check.
+     * @returns {boolean} Returns `true` if `value` is correctly classified, else `false`.
+     * @example
+     *
+     * function Foo(){};  
+     * isFunction(Foo);
+     * // => true
+     *
+     * isFunction(/abc/);
+     * // => false
+     */
+    isFunction = function(value) {
+        return isObject(value) && objToString.call(value) === funcTag;
+    };
+
+    /*********** lodash functions */
+
     /** Used to match words to create compound words. */
     reWords = (function() {
         var lower, upper;
         upper = '[A-Z]';
         lower = '[a-z]+';
         return RegExp(upper + '+(?=' + upper + lower + ')|' + upper + '?' + lower + '|' + upper + '+|[0-9]+', 'g');
     })();
+
+    /**
+     * Convert string to camelCase
+     * @function Util.camelCase
+     * @param {string} string - the string to convert
+     * @return {string} in camelCase format
+     */
     camelCase = function(source) {
         var i, word, words;
         words = source.match(reWords);
         words = (function() {
             var j, len, results;
             results = [];
             for (i = j = 0, len = words.length; j < len; i = ++j) {
@@ -114,14 +217,21 @@
                     results.push(word);
                 }
             }
             return results;
         })();
         return words.join('');
     };
+
+    /**
+     * Convert string to snake_case
+     * @function Util.snakeCase
+     * @param {string} string - the string to convert
+     * @return {string} in snake_case format
+     */
     snakeCase = function(source) {
         var i, word, words;
         words = source.match(reWords);
         words = (function() {
             var j, len, results;
             results = [];
             for (i = j = 0, len = words.length; j < len; i = ++j) {
@@ -143,72 +253,73 @@
             key = converter(key);
             if (!Util.isEmpty(key)) {
                 result[key] = value;
             }
         }
         return result;
     };
+
+    /**
+     * Create a copy of the source object with all keys in camelCase
+     * @function Util.withCamelCaseKeys
+     * @param {Object} value - the object to copy
+     * @return {Object} a new object
+     */
     withCamelCaseKeys = function(source) {
         return convertKeys(source, Util.camelCase);
     };
+
+    /**
+     * Create a copy of the source object with all keys in snake_case
+     * @function Util.withSnakeCaseKeys
+     * @param {Object} value - the object to copy
+     * @return {Object} a new object
+     */
     withSnakeCaseKeys = function(source) {
         return convertKeys(source, Util.snakeCase);
     };
-    BaseUtil = {
+    base64Encode = typeof btoa !== 'undefined' && isFunction(btoa) ? btoa : typeof Buffer !== 'undefined' && isFunction(Buffer) ? function(input) {
+        if (!(input instanceof Buffer)) {
+            input = new Buffer.from(String(input), 'binary');
+        }
+        return input.toString('base64');
+    } : function(input) {
+        throw new Error("No base64 encoding function found");
+    };
 
-        /**
-         * Return true if all items in list are strings
-         * @param {Array} list - an array of items
-         */
+    /**
+     * Returns the Base64-decoded version of url.<br>
+     * This method delegates to `btoa` if present. Otherwise it tries `Buffer`.
+     * @function Util.base64EncodeURL
+     * @param {string} url - the url to encode. the value is URIdecoded and then re-encoded before converting to base64 representation
+     * @return {string} the base64 representation of the URL
+     */
+    base64EncodeURL = function(input) {
+        var error1, ignore;
+        try {
+            input = decodeURI(input);
+        } catch (error1) {
+            ignore = error1;
+        }
+        input = encodeURI(input);
+        return base64Encode(input);
+    };
+    BaseUtil = {
         allStrings: allStrings,
-
-        /**
-         * Convert string to camelCase
-         * @param {string} string - the string to convert
-         * @return {string} in camelCase format
-         */
         camelCase: camelCase,
         convertKeys: convertKeys,
-
-        /**
-         * Assign values from sources if they are not defined in the destination.
-         * Once a value is set it does not change
-         * @param {Object} destination - the object to assign defaults to
-         * @param {...Object} source - the source object(s) to assign defaults from
-         * @return {Object} destination after it was modified
-         */
         defaults: defaults,
-
-        /**
-         * Convert string to snake_case
-         * @param {string} string - the string to convert
-         * @return {string} in snake_case format
-         */
         snakeCase: snakeCase,
-
-        /**
-         * Creates a new array without the given item.
-         * @param {Array} array - original array
-         * @param {*} item - the item to exclude from the new array
-         * @return {Array} a new array made of the original array's items except for `item`
-         */
         without: without,
-
-        /**
-         * Return true is value is a number or a string representation of a number.
-         * @example
-         *    Util.isNumber(0) // true
-         *    Util.isNumber("1.3") // true
-         *    Util.isNumber("") // false
-         *    Util.isNumber(undefined) // false
-         */
+        isFunction: isFunction,
         isNumberLike: isNumberLike,
         smartEscape: smartEscape,
         withCamelCaseKeys: withCamelCaseKeys,
-        withSnakeCaseKeys: withSnakeCaseKeys
+        withSnakeCaseKeys: withSnakeCaseKeys,
+        base64EncodeURL: base64EncodeURL
     };
 
     /**
      * Includes utility methods and lodash / jQuery shims
      */
 
     /**
@@ -224,132 +335,233 @@
         return jQuery(element).data(name);
     };
 
     /**
      * Set data in the DOM element.
      *
      * This method will use jQuery's `data()` method if it is available, otherwise it will set the `data-` attribute
+     * @function Util.setData
      * @param {Element} element - the element to set the data in
      * @param {string} name - the name of the data item
      * @param {*} value - the value to be set
      *
      */
     setData = function(element, name, value) {
         return jQuery(element).data(name, value);
     };
 
     /**
      * Get attribute from the DOM element.
      *
      * This method will use jQuery's `attr()` method if it is available, otherwise it will get the attribute directly
+     * @function Util.getAttribute
      * @param {Element} element - the element to set the attribute for
      * @param {string} name - the name of the attribute
      * @returns {*} the value of the attribute
      *
      */
     getAttribute = function(element, name) {
         return jQuery(element).attr(name);
     };
 
     /**
      * Set attribute in the DOM element.
      *
      * This method will use jQuery's `attr()` method if it is available, otherwise it will set the attribute directly
+     * @function Util.setAttribute
      * @param {Element} element - the element to set the attribute for
      * @param {string} name - the name of the attribute
      * @param {*} value - the value to be set
-     *
      */
     setAttribute = function(element, name, value) {
         return jQuery(element).attr(name, value);
     };
+
+    /**
+     * Remove an attribute in the DOM element.
+     *
+     * @function Util.removeAttribute
+     * @param {Element} element - the element to set the attribute for
+     * @param {string} name - the name of the attribute
+     */
     removeAttribute = function(element, name) {
         return jQuery(element).removeAttr(name);
     };
+
+    /**
+     * Set a group of attributes to the element
+     * @function Util.setAttributes
+     * @param {Element} element - the element to set the attributes for
+     * @param {Object} attributes - a hash of attribute names and values
+     */
     setAttributes = function(element, attributes) {
         return jQuery(element).attr(attributes);
     };
+
+    /**
+      * Checks if element has a css class
+      * @function Util.hasClass
+      * @param {Element} element - the element to check
+      * @param {string} name - the class name
+      @returns {boolean} true if the element has the class
+     */
     hasClass = function(element, name) {
         return jQuery(element).hasClass(name);
     };
+
+    /**
+     * Add class to the element
+     * @function Util.addClass
+     * @param {Element} element - the element
+     * @param {string} name - the class name to add
+     */
     addClass = function(element, name) {
         return jQuery(element).addClass(name);
     };
     width = function(element) {
         return jQuery(element).width();
     };
+
+    /**
+     * Returns true if item is empty:
+     * <ul>
+     *   <li>item is null or undefined</li>
+     *   <li>item is an array or string of length 0</li>
+     *   <li>item is an object with no keys</li>
+     * </ul>
+     * @function Util.isEmpty
+     * @param item
+     * @returns {boolean} true if item is empty
+     */
     isEmpty = function(item) {
         return (item == null) || (jQuery.isArray(item) || Util.isString(item)) && item.length === 0 || (jQuery.isPlainObject(item) && jQuery.isEmptyObject(item));
     };
+
+    /**
+     * Returns true if item is a string
+     * @param item
+     * @returns {boolean} true if item is a string
+     */
     isString = function(item) {
         return typeof item === 'string' || (item != null ? item.toString() : void 0) === '[object String]';
     };
+
+    /**
+     * Recursively assign source properties to destination
+     * @function Util.merge
+     * @param {Object} destination - the object to assign to
+     * @param {...Object} [sources] The source objects.
+     */
     merge = function() {
         var args, i;
         args = (function() {
             var j, len, results;
             results = [];
             for (j = 0, len = arguments.length; j < len; j++) {
                 i = arguments[j];
                 results.push(i);
             }
             return results;
         }).apply(this, arguments);
         args.unshift(true);
         return jQuery.extend.apply(this, args);
     };
+
+    /**
+     * Creates a new array from the parameter with "falsey" values removed
+     * @function Util.compact
+     * @param {Array} array - the array to remove values from
+     * @return {Array} a new array without falsey values
+     */
     compact = function(arr) {
         var item, j, len, results;
         results = [];
         for (j = 0, len = arr.length; j < len; j++) {
             item = arr[j];
             if (item) {
                 results.push(item);
             }
         }
         return results;
     };
+
+    /**
+     * Create a new copy of the given object, including all internal objects.
+     * @function Util.cloneDeep
+     * @param {Object} value - the object to clone
+     * @return {Object} a new deep copy of the object
+     */
     cloneDeep = function() {
         var args;
         args = jQuery.makeArray(arguments);
         args.unshift({});
         args.unshift(true);
         return jQuery.extend.apply(this, args);
     };
+
+    /**
+     * Check if a given item is included in the given array
+     * @function Util.contains
+     * @param {Array} array - the array to search in
+     * @param {*} item - the item to search for
+     * @return {boolean} true if the item is included in the array
+     */
     contains = function(arr, item) {
         var i, j, len;
         for (j = 0, len = arr.length; j < len; j++) {
             i = arr[j];
             if (i === item) {
                 return true;
             }
         }
         return false;
     };
+
+    /**
+     * Returns values in the given array that are not included in the other array
+     * @function Util.difference
+     * @param {Array} arr - the array to select from
+     * @param {Array} values - values to filter from arr
+     * @return {Array} the filtered values
+     */
     difference = function(arr, values) {
         var item, j, len, results;
         results = [];
         for (j = 0, len = arr.length; j < len; j++) {
             item = arr[j];
             if (!contains(values, item)) {
                 results.push(item);
             }
         }
         return results;
     };
+
+    /**
+     * Returns a list of all the function names in obj
+     * @function Util.functions
+     * @param {Object} object - the object to inspect
+     * @return {Array} a list of functions of object
+     */
     functions = function(object) {
         var i, results;
         results = [];
         for (i in object) {
             if (jQuery.isFunction(object[i])) {
                 results.push(i);
             }
         }
         return results;
     };
+
+    /**
+     * Returns the provided value. This functions is used as a default predicate function.
+     * @function Util.identity
+     * @param {*} value
+     * @return {*} the provided value
+     */
     identity = function(value) {
         return value;
     };
 
     /**
      * @class Util
      */
@@ -366,79 +578,30 @@
         isString: isString,
         isArray: jQuery.isArray,
         isEmpty: isEmpty,
 
         /**
          * Assign source properties to destination.
          * If the property is an object it is assigned as a whole, overriding the destination object.
+         * @function Util.assign
          * @param {Object} destination - the object to assign to
          */
         assign: jQuery.extend,
-
-        /**
-         * Recursively assign source properties to destination
-         * @param {Object} destination - the object to assign to
-         * @param {...Object} [sources] The source objects.
-         */
         merge: merge,
-
-        /**
-         * Create a new copy of the given object, including all internal objects.
-         * @param {Object} value - the object to clone
-         * @return {Object} a new deep copy of the object
-         */
         cloneDeep: cloneDeep,
-
-        /**
-         * Creates a new array from the parameter with "falsey" values removed
-         * @param {Array} array - the array to remove values from
-         * @return {Array} a new array without falsey values
-         */
         compact: compact,
-
-        /**
-         * Check if a given item is included in the given array
-         * @param {Array} array - the array to search in
-         * @param {*} item - the item to search for
-         * @return {boolean} true if the item is included in the array
-         */
         contains: contains,
-
-        /**
-         * Returns values in the given array that are not included in the other array
-         * @param {Array} arr - the array to select from
-         * @param {Array} values - values to filter from arr
-         * @return {Array} the filtered values
-         */
         difference: difference,
-
-        /**
-         * Returns true if argument is a function.
-         * @param {*} value - the value to check
-         * @return {boolean} true if the value is a function
-         */
-        isFunction: jQuery.isFunction,
-
-        /**
-         * Returns a list of all the function names in obj
-         * @param {Object} object - the object to inspect
-         * @return {Array} a list of functions of object
-         */
         functions: functions,
-
-        /**
-         * Returns the provided value. This functions is used as a default predicate function.
-         * @param {*} value
-         * @return {*} the provided value
-         */
         identity: identity,
         isPlainObject: jQuery.isPlainObject,
 
         /**
          * Remove leading or trailing spaces from text
+         * @function Util.trim
          * @param {string} text
          * @return {string} the `text` without leading or trailing spaces
          */
         trim: jQuery.trim
     });
 
     /**
@@ -596,14 +759,51 @@
             components.push(this.getFullPublicId());
             return Util.compact(components).join(":");
         };
 
         return Layer;
 
     })();
+    FetchLayer = (function(superClass) {
+        extend(FetchLayer, superClass);
+
+
+        /**
+         * @constructor FetchLayer
+         * @param {Object|string} options - layer parameters or a url
+         */
+
+        function FetchLayer(options) {
+            FetchLayer.__super__.constructor.call(this, options);
+            if (Util.isString(options)) {
+                this.options.url = options;
+            } else if (options != null ? options.url : void 0) {
+                this.options.url = options.url;
+            }
+        }
+
+        FetchLayer.prototype.url = function(url) {
+            this.options.url = url;
+            return this;
+        };
+
+
+        /**
+         * generate the string representation of the layer
+         * @function FetchLayer#toString
+         * @return {String}
+         */
+
+        FetchLayer.prototype.toString = function() {
+            return "fetch:" + (cloudinary.Util.base64EncodeURL(this.options.url));
+        };
+
+        return FetchLayer;
+
+    })(Layer);
     TextLayer = (function(superClass) {
         extend(TextLayer, superClass);
 
 
         /**
          * @constructor TextLayer
          * @param {Object} options - layer parameters
@@ -1129,17 +1329,21 @@
             var layerOptions, result;
             layerOptions = this.origValue;
             if (cloudinary.Util.isPlainObject(layerOptions)) {
                 if (layerOptions.resource_type === "text" || (layerOptions.text != null)) {
                     result = new cloudinary.TextLayer(layerOptions).toString();
                 } else if (layerOptions.resource_type === "subtitles") {
                     result = new cloudinary.SubtitlesLayer(layerOptions).toString();
+                } else if (layerOptions.resource_type === "fetch") {
+                    result = new cloudinary.Layer(layerOptions).toString();
                 } else {
                     result = new cloudinary.Layer(layerOptions).toString();
                 }
+            } else if (/^fetch:.+/.test(layerOptions)) {
+                result = new FetchLayer(layerOptions.substr(6)).toString();
             } else {
                 result = layerOptions;
             }
             return result;
         };
 
         LAYER_KEYWORD_PARAMS = [
@@ -1782,15 +1986,15 @@
          * @requires Node.js
          */
 
         Configuration.prototype.fromEnvironment = function() {
             var cloudinary_url, j, k, len, query, ref1, ref2, ref3, uri, uriRegex, v, value;
             cloudinary_url = typeof process !== "undefined" && process !== null ? (ref1 = process.env) != null ? ref1.CLOUDINARY_URL : void 0 : void 0;
             if (cloudinary_url != null) {
-                uriRegex = /cloudinary:\/\/(?:(\w+)(?:\:(\w+))?@)?([\w\.-]+)(?:\/([^?]*))?(?:\?(.+))?/;
+                uriRegex = /cloudinary:\/\/(?:(\w+)(?:\:([\w-]+))?@)?([\w\.-]+)(?:\/([^?]*))?(?:\?(.+))?/;
                 uri = uriRegex.exec(cloudinary_url);
                 if (uri) {
                     if (uri[3] != null) {
                         this.configuration['cloud_name'] = uri[3];
                     }
                     if (uri[1] != null) {
                         this.configuration['api_key'] = uri[1];
@@ -4504,14 +4708,15 @@
         Transformation: Transformation,
         Configuration: Configuration,
         HtmlTag: HtmlTag,
         ImageTag: ImageTag,
         VideoTag: VideoTag,
         ClientHintsMetaTag: ClientHintsMetaTag,
         Layer: Layer,
+        FetchLayer: FetchLayer,
         TextLayer: TextLayer,
         SubtitlesLayer: SubtitlesLayer,
         Cloudinary: Cloudinary,
         VERSION: "2.3.0",
         CloudinaryJQuery: CloudinaryJQuery
     };
     return cloudinary;
```

### Comparing `cloudinary-1.8.0/cloudinary/static/js/jquery.fileupload-image.js` & `cloudinary-1.9.0/cloudinary/static/js/jquery.fileupload-image.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -2,39 +2,41 @@
  * jQuery File Upload Image Preview & Resize Plugin
  * https://github.com/blueimp/jQuery-File-Upload
  *
  * Copyright 2013, Sebastian Tschan
  * https://blueimp.net
  *
  * Licensed under the MIT license:
- * http://www.opensource.org/licenses/MIT
+ * https://opensource.org/licenses/MIT
  */
 
 /* jshint nomen:false */
 /* global define, require, window, Blob */
 
 ;
 (function(factory) {
     'use strict';
     if (typeof define === 'function' && define.amd) {
         // Register as an anonymous AMD module:
         define([
             'jquery',
             'load-image',
             'load-image-meta',
+            'load-image-scale',
             'load-image-exif',
             'canvas-to-blob',
             './jquery.fileupload-process'
         ], factory);
     } else if (typeof exports === 'object') {
         // Node/CommonJS:
         factory(
             require('jquery'),
             require('blueimp-load-image/js/load-image'),
             require('blueimp-load-image/js/load-image-meta'),
+            require('blueimp-load-image/js/load-image-scale'),
             require('blueimp-load-image/js/load-image-exif'),
             require('blueimp-canvas-to-blob'),
             require('./jquery.fileupload-process')
         );
     } else {
         // Browser globals:
         factory(
```

### Comparing `cloudinary-1.8.0/cloudinary/static/js/jquery.fileupload-process.js` & `cloudinary-1.9.0/cloudinary/static/js/jquery.fileupload-process.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -2,15 +2,15 @@
  * jQuery File Upload Processing Plugin
  * https://github.com/blueimp/jQuery-File-Upload
  *
  * Copyright 2012, Sebastian Tschan
  * https://blueimp.net
  *
  * Licensed under the MIT license:
- * http://www.opensource.org/licenses/MIT
+ * https://opensource.org/licenses/MIT
  */
 
 /* jshint nomen:false */
 /* global define, require, window */
 
 ;
 (function(factory) {
@@ -19,15 +19,18 @@
         // Register as an anonymous AMD module:
         define([
             'jquery',
             './jquery.fileupload'
         ], factory);
     } else if (typeof exports === 'object') {
         // Node/CommonJS:
-        factory(require('jquery'));
+        factory(
+            require('jquery'),
+            require('./jquery.fileupload')
+        );
     } else {
         // Browser globals:
         factory(
             window.jQuery
         );
     }
 }(function($) {
```

### Comparing `cloudinary-1.8.0/cloudinary/static/js/jquery.fileupload-validate.js` & `cloudinary-1.9.0/cloudinary/static/js/jquery.fileupload-validate.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -2,15 +2,15 @@
  * jQuery File Upload Validation Plugin
  * https://github.com/blueimp/jQuery-File-Upload
  *
  * Copyright 2013, Sebastian Tschan
  * https://blueimp.net
  *
  * Licensed under the MIT license:
- * http://www.opensource.org/licenses/MIT
+ * https://opensource.org/licenses/MIT
  */
 
 /* global define, require, window */
 
 ;
 (function(factory) {
     'use strict';
@@ -18,15 +18,18 @@
         // Register as an anonymous AMD module:
         define([
             'jquery',
             './jquery.fileupload-process'
         ], factory);
     } else if (typeof exports === 'object') {
         // Node/CommonJS:
-        factory(require('jquery'));
+        factory(
+            require('jquery'),
+            require('./jquery.fileupload-process')
+        );
     } else {
         // Browser globals:
         factory(
             window.jQuery
         );
     }
 }(function($) {
```

### Comparing `cloudinary-1.8.0/cloudinary/static/js/jquery.fileupload.js` & `cloudinary-1.9.0/cloudinary/static/js/jquery.fileupload.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -2,28 +2,28 @@
  * jQuery File Upload Plugin
  * https://github.com/blueimp/jQuery-File-Upload
  *
  * Copyright 2010, Sebastian Tschan
  * https://blueimp.net
  *
  * Licensed under the MIT license:
- * http://www.opensource.org/licenses/MIT
+ * https://opensource.org/licenses/MIT
  */
 
 /* jshint nomen:false */
 /* global define, require, window, document, location, Blob, FormData */
 
 ;
 (function(factory) {
     'use strict';
     if (typeof define === 'function' && define.amd) {
         // Register as an anonymous AMD module:
         define([
             'jquery',
-            'jquery.ui.widget'
+            'jquery-ui/ui/widget'
         ], factory);
     } else if (typeof exports === 'object') {
         // Node/CommonJS:
         factory(
             require('jquery'),
             require('./vendor/jquery.ui.widget')
         );
@@ -738,15 +738,15 @@
                 ub = options.uploadedBytes,
                 mcs = options.maxChunkSize || fs,
                 slice = this._blobSlice,
                 dfd = $.Deferred(),
                 promise = dfd.promise(),
                 jqXHR,
                 upload;
-            if (!(this._isXHRUpload(options) && slice && (ub || mcs < fs)) ||
+            if (!(this._isXHRUpload(options) && slice && (ub || ($.type(mcs) === 'function' ? mcs(options) : mcs) < fs)) ||
                 options.data) {
                 return false;
             }
             if (testOnly) {
                 return true;
             }
             if (ub >= fs) {
@@ -761,15 +761,15 @@
             upload = function() {
                 // Clone the options object for each chunk upload:
                 var o = $.extend({}, options),
                     currentLoaded = o._progress.loaded;
                 o.blob = slice.call(
                     file,
                     ub,
-                    ub + mcs,
+                    ub + ($.type(mcs) === 'function' ? mcs(o) : mcs),
                     file.type
                 );
                 // Store the current chunk size, as the blob itself
                 // will be dereferenced after data processing:
                 o.chunkSize = o.blob.size;
                 // Expose the chunk bytes position range:
                 o.contentRange = 'bytes ' + ub + '-' +
@@ -1092,14 +1092,16 @@
                 this.element = inputClone;
             }
         },
 
         _handleFileTreeEntry: function(entry, path) {
             var that = this,
                 dfd = $.Deferred(),
+                entries = [],
+                dirReader,
                 errorHandler = function(e) {
                     if (e && !e.entry) {
                         e.entry = entry;
                     }
                     // Since $.when returns immediately if one
                     // Deferred is rejected, we use resolve instead.
                     // This allows valid files and invalid items
@@ -1119,16 +1121,15 @@
                         if (!results.length) {
                             successHandler(entries);
                         } else {
                             entries = entries.concat(results);
                             readEntries();
                         }
                     }, errorHandler);
-                },
-                dirReader, entries = [];
+                };
             path = path || '';
             if (entry.isFile) {
                 if (entry._file) {
                     // Workaround for Chrome bug #149735
                     entry._file.relativePath = path;
                     dfd.resolve(entry._file);
                 } else {
@@ -1333,14 +1334,18 @@
 
         _destroyEventHandlers: function() {
             this._off(this.options.dropZone, 'dragenter dragleave dragover drop');
             this._off(this.options.pasteZone, 'paste');
             this._off(this.options.fileInput, 'change');
         },
 
+        _destroy: function() {
+            this._destroyEventHandlers();
+        },
+
         _setOption: function(key, value) {
             var reinit = $.inArray(key, this._specialOptions) !== -1;
             if (reinit) {
                 this._destroyEventHandlers();
             }
             this._super(key, value);
             if (reinit) {
```

### Comparing `cloudinary-1.8.0/cloudinary/static/js/jquery.iframe-transport.js` & `cloudinary-1.9.0/cloudinary/static/js/jquery.iframe-transport.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -2,18 +2,18 @@
  * jQuery Iframe Transport Plugin
  * https://github.com/blueimp/jQuery-File-Upload
  *
  * Copyright 2011, Sebastian Tschan
  * https://blueimp.net
  *
  * Licensed under the MIT license:
- * http://www.opensource.org/licenses/MIT
+ * https://opensource.org/licenses/MIT
  */
 
-/* global define, require, window, document */
+/* global define, require, window, document, JSON */
 
 ;
 (function(factory) {
     'use strict';
     if (typeof define === 'function' && define.amd) {
         // Register as an anonymous AMD module:
         define(['jquery'], factory);
@@ -24,15 +24,22 @@
         // Browser globals:
         factory(window.jQuery);
     }
 }(function($) {
     'use strict';
 
     // Helper variable to create unique names for the transport iframes:
-    var counter = 0;
+    var counter = 0,
+        jsonAPI = $,
+        jsonParse = 'parseJSON';
+
+    if ('JSON' in window && 'parse' in JSON) {
+        jsonAPI = JSON;
+        jsonParse = 'parse';
+    }
 
     // The iframe transport accepts four additional options:
     // options.fileInput: a jQuery collection of file input fields
     // options.paramName: the parameter name for the file form data,
     //  overrides the name property of the file input field(s),
     //  can be a string or an array of strings.
     // options.formData: an array of objects with name and value properties,
@@ -195,15 +202,15 @@
     // https://github.com/blueimp/jQuery-File-Upload/wiki/Setup#content-type-negotiation
     $.ajaxSetup({
         converters: {
             'iframe text': function(iframe) {
                 return iframe && $(iframe[0].body).text();
             },
             'iframe json': function(iframe) {
-                return iframe && $.parseJSON($(iframe[0].body).text());
+                return iframe && jsonAPI[jsonParse]($(iframe[0].body).text());
             },
             'iframe html': function(iframe) {
                 return iframe && $(iframe[0].body).html();
             },
             'iframe xml': function(iframe) {
                 var xmlDoc = iframe && iframe[0];
                 return xmlDoc && $.isXMLDoc(xmlDoc) ? xmlDoc :
```

### Comparing `cloudinary-1.8.0/cloudinary/static/js/jquery.ui.widget.js` & `cloudinary-1.9.0/cloudinary/static/js/jquery.ui.widget.js`

 * *Files identical despite different names*

### Comparing `cloudinary-1.8.0/cloudinary/static/js/load-image.all.min.js` & `cloudinary-1.9.0/cloudinary/static/js/load-image.all.min.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,150 +1,174 @@
 ! function(e) {
     "use strict";
 
     function t(e, i, a) {
-        var o, r = document.createElement("img");
-        if (r.onerror = function(o) {
-                return t.onerror(r, o, e, i, a)
-            }, r.onload = function(o) {
-                return t.onload(r, o, e, i, a)
-            }, t.isInstanceOf("Blob", e) || t.isInstanceOf("File", e)) o = r._objectURL = t.createObjectURL(e);
-        else {
-            if ("string" != typeof e) return !1;
-            o = e, a && a.crossOrigin && (r.crossOrigin = a.crossOrigin)
-        }
-        return o ? (r.src = o, r) : t.readFile(e, function(e) {
+        var o, n = document.createElement("img");
+        return n.onerror = function(o) {
+            return t.onerror(n, o, e, i, a)
+        }, n.onload = function(o) {
+            return t.onload(n, o, e, i, a)
+        }, "string" == typeof e ? (t.fetchBlob(e, function(i) {
+            i ? (e = i, o = t.createObjectURL(e)) : (o = e, a && a.crossOrigin && (n.crossOrigin = a.crossOrigin)), n.src = o
+        }, a), n) : t.isInstanceOf("Blob", e) || t.isInstanceOf("File", e) ? (o = n._objectURL = t.createObjectURL(e)) ? (n.src = o, n) : t.readFile(e, function(e) {
             var t = e.target;
-            t && t.result ? r.src = t.result : i && i(e)
-        })
+            t && t.result ? n.src = t.result : i && i(e)
+        }) : void 0
     }
 
     function i(e, i) {
         !e._objectURL || i && i.noRevoke || (t.revokeObjectURL(e._objectURL), delete e._objectURL)
     }
-    var a = window.createObjectURL && window || window.URL && URL.revokeObjectURL && URL || window.webkitURL && webkitURL;
-    t.isInstanceOf = function(e, t) {
+    var a = e.createObjectURL && e || e.URL && URL.revokeObjectURL && URL || e.webkitURL && webkitURL;
+    t.fetchBlob = function(e, t, i) {
+        t()
+    }, t.isInstanceOf = function(e, t) {
         return Object.prototype.toString.call(t) === "[object " + e + "]"
-    }, t.transform = function(e, i, a, o, r) {
-        a(t.scale(e, i, r), r)
-    }, t.onerror = function(e, t, a, o, r) {
-        i(e, r), o && o.call(e, t)
-    }, t.onload = function(e, a, o, r, n) {
-        i(e, n), r && t.transform(e, n, r, o, {})
-    }, t.transformCoordinates = function() {}, t.getTransformedOptions = function(e, t) {
-        var i, a, o, r, n = t.aspectRatio;
-        if (!n) return t;
+    }, t.transform = function(e, t, i, a, o) {
+        i(e, o)
+    }, t.onerror = function(e, t, a, o, n) {
+        i(e, n), o && o.call(e, t)
+    }, t.onload = function(e, a, o, n, r) {
+        i(e, r), n && t.transform(e, r, n, o, {})
+    }, t.createObjectURL = function(e) {
+        return !!a && a.createObjectURL(e)
+    }, t.revokeObjectURL = function(e) {
+        return !!a && a.revokeObjectURL(e)
+    }, t.readFile = function(t, i, a) {
+        if (e.FileReader) {
+            var o = new FileReader;
+            if (o.onload = o.onerror = i, a = a || "readAsDataURL", o[a]) return o[a](t), o
+        }
+        return !1
+    }, "function" == typeof define && define.amd ? define(function() {
+        return t
+    }) : "object" == typeof module && module.exports ? module.exports = t : e.loadImage = t
+}("undefined" != typeof window && window || this),
+function(e) {
+    "use strict";
+    "function" == typeof define && define.amd ? define(["./load-image"], e) : e("object" == typeof module && module.exports ? require("./load-image") : window.loadImage)
+}(function(e) {
+    "use strict";
+    var t = e.transform;
+    e.transform = function(i, a, o, n, r) {
+        t.call(e, e.scale(i, a, r), a, o, n, r)
+    }, e.transformCoordinates = function() {}, e.getTransformedOptions = function(e, t) {
+        var i, a, o, n, r = t.aspectRatio;
+        if (!r) return t;
         i = {};
         for (a in t) t.hasOwnProperty(a) && (i[a] = t[a]);
-        return i.crop = !0, o = e.naturalWidth || e.width, r = e.naturalHeight || e.height, o / r > n ? (i.maxWidth = r * n, i.maxHeight = r) : (i.maxWidth = o, i.maxHeight = o / n), i
-    }, t.renderImageToCanvas = function(e, t, i, a, o, r, n, s, l, d) {
-        return e.getContext("2d").drawImage(t, i, a, o, r, n, s, l, d), e
-    }, t.hasCanvasOption = function(e) {
+        return i.crop = !0, o = e.naturalWidth || e.width, n = e.naturalHeight || e.height, o / n > r ? (i.maxWidth = n * r, i.maxHeight = n) : (i.maxWidth = o, i.maxHeight = o / r), i
+    }, e.renderImageToCanvas = function(e, t, i, a, o, n, r, s, l, d) {
+        return e.getContext("2d").drawImage(t, i, a, o, n, r, s, l, d), e
+    }, e.hasCanvasOption = function(e) {
         return e.canvas || e.crop || !!e.aspectRatio
-    }, t.scale = function(e, i, a) {
+    }, e.scale = function(t, i, a) {
         function o() {
             var e = Math.max((l || v) / v, (d || P) / P);
             e > 1 && (v *= e, P *= e)
         }
 
-        function r() {
-            var e = Math.min((n || v) / v, (s || P) / P);
+        function n() {
+            var e = Math.min((r || v) / v, (s || P) / P);
             e < 1 && (v *= e, P *= e)
         }
         i = i || {};
-        var n, s, l, d, u, c, f, g, h, m, p, S = document.createElement("canvas"),
-            b = e.getContext || t.hasCanvasOption(i) && S.getContext,
-            x = e.naturalWidth || e.width,
-            y = e.naturalHeight || e.height,
-            v = x,
-            P = y;
-        if (b && (i = t.getTransformedOptions(e, i, a), f = i.left || 0, g = i.top || 0, i.sourceWidth ? (u = i.sourceWidth, void 0 !== i.right && void 0 === i.left && (f = x - u - i.right)) : u = x - f - (i.right || 0), i.sourceHeight ? (c = i.sourceHeight, void 0 !== i.bottom && void 0 === i.top && (g = y - c - i.bottom)) : c = y - g - (i.bottom || 0), v = u, P = c), n = i.maxWidth, s = i.maxHeight, l = i.minWidth, d = i.minHeight, b && n && s && i.crop ? (v = n, P = s, p = u / c - n / s, p < 0 ? (c = s * u / n, void 0 === i.top && void 0 === i.bottom && (g = (y - c) / 2)) : p > 0 && (u = n * c / s, void 0 === i.left && void 0 === i.right && (f = (x - u) / 2))) : ((i.contain || i.cover) && (l = n = n || l, d = s = s || d), i.cover ? (r(), o()) : (o(), r())), b) {
-            if (h = i.pixelRatio, h > 1 && (S.style.width = v + "px", S.style.height = P + "px", v *= h, P *= h, S.getContext("2d").scale(h, h)), m = i.downsamplingRatio, m > 0 && m < 1 && v < u && P < c)
-                for (; u * m > v;) S.width = u * m, S.height = c * m, t.renderImageToCanvas(S, e, f, g, u, c, 0, 0, S.width, S.height), u = S.width, c = S.height, e = document.createElement("canvas"), e.width = u, e.height = c, t.renderImageToCanvas(e, S, 0, 0, u, c, 0, 0, u, c);
-            return S.width = v, S.height = P, t.transformCoordinates(S, i), t.renderImageToCanvas(S, e, f, g, u, c, 0, 0, v, P)
-        }
-        return e.width = v, e.height = P, e
-    }, t.createObjectURL = function(e) {
-        return !!a && a.createObjectURL(e)
-    }, t.revokeObjectURL = function(e) {
-        return !!a && a.revokeObjectURL(e)
-    }, t.readFile = function(e, t, i) {
-        if (window.FileReader) {
-            var a = new FileReader;
-            if (a.onload = a.onerror = t, i = i || "readAsDataURL", a[i]) return a[i](e), a
+        var r, s, l, d, c, u, f, g, h, m, p, S = document.createElement("canvas"),
+            b = t.getContext || e.hasCanvasOption(i) && S.getContext,
+            y = t.naturalWidth || t.width,
+            x = t.naturalHeight || t.height,
+            v = y,
+            P = x;
+        if (b && (f = (i = e.getTransformedOptions(t, i, a)).left || 0, g = i.top || 0, i.sourceWidth ? (c = i.sourceWidth, void 0 !== i.right && void 0 === i.left && (f = y - c - i.right)) : c = y - f - (i.right || 0), i.sourceHeight ? (u = i.sourceHeight, void 0 !== i.bottom && void 0 === i.top && (g = x - u - i.bottom)) : u = x - g - (i.bottom || 0), v = c, P = u), r = i.maxWidth, s = i.maxHeight, l = i.minWidth, d = i.minHeight, b && r && s && i.crop ? (v = r, P = s, (p = c / u - r / s) < 0 ? (u = s * c / r, void 0 === i.top && void 0 === i.bottom && (g = (x - u) / 2)) : p > 0 && (c = r * u / s, void 0 === i.left && void 0 === i.right && (f = (y - c) / 2))) : ((i.contain || i.cover) && (l = r = r || l, d = s = s || d), i.cover ? (n(), o()) : (o(), n())), b) {
+            if ((h = i.pixelRatio) > 1 && (S.style.width = v + "px", S.style.height = P + "px", v *= h, P *= h, S.getContext("2d").scale(h, h)), (m = i.downsamplingRatio) > 0 && m < 1 && v < c && P < u)
+                for (; c * m > v;) S.width = c * m, S.height = u * m, e.renderImageToCanvas(S, t, f, g, c, u, 0, 0, S.width, S.height), f = 0, g = 0, c = S.width, u = S.height, (t = document.createElement("canvas")).width = c, t.height = u, e.renderImageToCanvas(t, S, 0, 0, c, u, 0, 0, c, u);
+            return S.width = v, S.height = P, e.transformCoordinates(S, i), e.renderImageToCanvas(S, t, f, g, c, u, 0, 0, v, P)
         }
-        return !1
-    }, "function" == typeof define && define.amd ? define(function() {
-        return t
-    }) : "object" == typeof module && module.exports ? module.exports = t : e.loadImage = t
-}(window),
+        return t.width = v, t.height = P, t
+    }
+}),
 function(e) {
     "use strict";
     "function" == typeof define && define.amd ? define(["./load-image"], e) : e("object" == typeof module && module.exports ? require("./load-image") : window.loadImage)
 }(function(e) {
     "use strict";
-    var t = window.Blob && (Blob.prototype.slice || Blob.prototype.webkitSlice || Blob.prototype.mozSlice);
+    var t = "undefined" != typeof Blob && (Blob.prototype.slice || Blob.prototype.webkitSlice || Blob.prototype.mozSlice);
     e.blobSlice = t && function() {
-        var e = this.slice || this.webkitSlice || this.mozSlice;
-        return e.apply(this, arguments)
+        return (this.slice || this.webkitSlice || this.mozSlice).apply(this, arguments)
     }, e.metaDataParsers = {
         jpeg: {
             65505: []
         }
     }, e.parseMetaData = function(t, i, a, o) {
         a = a || {}, o = o || {};
-        var r = this,
-            n = a.maxMetaDataSize || 262144,
-            s = !(window.DataView && t && t.size >= 12 && "image/jpeg" === t.type && e.blobSlice);
-        !s && e.readFile(e.blobSlice.call(t, 0, n), function(t) {
+        var n = this,
+            r = a.maxMetaDataSize || 262144;
+        !!("undefined" != typeof DataView && t && t.size >= 12 && "image/jpeg" === t.type && e.blobSlice) && e.readFile(e.blobSlice.call(t, 0, r), function(t) {
             if (t.target.error) return console.log(t.target.error), void i(o);
-            var n, s, l, d, u = t.target.result,
-                c = new DataView(u),
+            var r, s, l, d, c = t.target.result,
+                u = new DataView(c),
                 f = 2,
-                g = c.byteLength - 4,
+                g = u.byteLength - 4,
                 h = f;
-            if (65496 === c.getUint16(0)) {
-                for (; f < g && (n = c.getUint16(f), n >= 65504 && n <= 65519 || 65534 === n);) {
-                    if (s = c.getUint16(f + 2) + 2, f + s > c.byteLength) {
+            if (65496 === u.getUint16(0)) {
+                for (; f < g && ((r = u.getUint16(f)) >= 65504 && r <= 65519 || 65534 === r);) {
+                    if (s = u.getUint16(f + 2) + 2, f + s > u.byteLength) {
                         console.log("Invalid meta data: Invalid segment size.");
                         break
                     }
-                    if (l = e.metaDataParsers.jpeg[n])
-                        for (d = 0; d < l.length; d += 1) l[d].call(r, c, f, s, o, a);
-                    f += s, h = f
-                }!a.disableImageHead && h > 6 && (u.slice ? o.imageHead = u.slice(0, h) : o.imageHead = new Uint8Array(u).subarray(0, h))
+                    if (l = e.metaDataParsers.jpeg[r])
+                        for (d = 0; d < l.length; d += 1) l[d].call(n, u, f, s, o, a);
+                    h = f += s
+                }!a.disableImageHead && h > 6 && (c.slice ? o.imageHead = c.slice(0, h) : o.imageHead = new Uint8Array(c).subarray(0, h))
             } else console.log("Invalid JPEG file: Missing JPEG marker.");
             i(o)
         }, "readAsArrayBuffer") || i(o)
     }, e.hasMetaOption = function(e) {
-        return e.meta
+        return e && e.meta
     };
     var i = e.transform;
-    e.transform = function(t, a, o, r, n) {
-        e.hasMetaOption(a || {}) ? e.parseMetaData(r, function(n) {
-            i.call(e, t, a, o, r, n)
-        }, a, n) : i.apply(e, arguments)
+    e.transform = function(t, a, o, n, r) {
+        e.hasMetaOption(a) ? e.parseMetaData(n, function(r) {
+            i.call(e, t, a, o, n, r)
+        }, a, r) : i.apply(e, arguments)
     }
 }),
 function(e) {
     "use strict";
     "function" == typeof define && define.amd ? define(["./load-image", "./load-image-meta"], e) : "object" == typeof module && module.exports ? e(require("./load-image"), require("./load-image-meta")) : e(window.loadImage)
 }(function(e) {
     "use strict";
+    "undefined" != typeof fetch && "undefined" != typeof Request && (e.fetchBlob = function(t, i, a) {
+        if (e.hasMetaOption(a)) return fetch(new Request(t, a)).then(function(e) {
+            return e.blob()
+        }).then(i).catch(function(e) {
+            console.log(e), i()
+        });
+        i()
+    })
+}),
+function(e) {
+    "use strict";
+    "function" == typeof define && define.amd ? define(["./load-image", "./load-image-meta"], e) : "object" == typeof module && module.exports ? e(require("./load-image"), require("./load-image-meta")) : e(window.loadImage)
+}(function(e) {
+    "use strict";
     e.ExifMap = function() {
         return this
     }, e.ExifMap.prototype.map = {
         Orientation: 274
     }, e.ExifMap.prototype.get = function(e) {
         return this[e] || this[this.map[e]]
     }, e.getExifThumbnail = function(e, t, i) {
-        var a, o, r;
-        if (!i || t + i > e.byteLength) return void console.log("Invalid Exif data: Invalid thumbnail data.");
-        for (a = [], o = 0; o < i; o += 1) r = e.getUint8(t + o), a.push((r < 16 ? "0" : "") + r.toString(16));
-        return "data:image/jpeg,%" + a.join("%")
+        var a, o, n; {
+            if (i && !(t + i > e.byteLength)) {
+                for (a = [], o = 0; o < i; o += 1) n = e.getUint8(t + o), a.push((n < 16 ? "0" : "") + n.toString(16));
+                return "data:image/jpeg,%" + a.join("%")
+            }
+            console.log("Invalid Exif data: Invalid thumbnail data.")
+        }
     }, e.exifTagTypes = {
         1: {
             getValue: function(e, t) {
                 return e.getUint8(t)
             },
             size: 1
         },
@@ -181,55 +205,61 @@
         },
         10: {
             getValue: function(e, t, i) {
                 return e.getInt32(t, i) / e.getInt32(t + 4, i)
             },
             size: 8
         }
-    }, e.exifTagTypes[7] = e.exifTagTypes[1], e.getExifValue = function(t, i, a, o, r, n) {
-        var s, l, d, u, c, f, g = e.exifTagTypes[o];
-        if (!g) return void console.log("Invalid Exif data: Invalid tag type.");
-        if (s = g.size * r, l = s > 4 ? i + t.getUint32(a + 8, n) : a + 8, l + s > t.byteLength) return void console.log("Invalid Exif data: Invalid data offset.");
-        if (1 === r) return g.getValue(t, l, n);
-        for (d = [], u = 0; u < r; u += 1) d[u] = g.getValue(t, l + u * g.size, n);
-        if (g.ascii) {
-            for (c = "", u = 0; u < d.length && (f = d[u], "\0" !== f); u += 1) c += f;
-            return c
-        }
-        return d
-    }, e.parseExifTag = function(t, i, a, o, r) {
-        var n = t.getUint16(a, o);
-        r.exif[n] = e.getExifValue(t, i, a, t.getUint16(a + 2, o), t.getUint32(a + 4, o), o)
+    }, e.exifTagTypes[7] = e.exifTagTypes[1], e.getExifValue = function(t, i, a, o, n, r) {
+        var s, l, d, c, u, f, g = e.exifTagTypes[o];
+        if (g) {
+            if (s = g.size * n, !((l = s > 4 ? i + t.getUint32(a + 8, r) : a + 8) + s > t.byteLength)) {
+                if (1 === n) return g.getValue(t, l, r);
+                for (d = [], c = 0; c < n; c += 1) d[c] = g.getValue(t, l + c * g.size, r);
+                if (g.ascii) {
+                    for (u = "", c = 0; c < d.length && "\0" !== (f = d[c]); c += 1) u += f;
+                    return u
+                }
+                return d
+            }
+            console.log("Invalid Exif data: Invalid data offset.")
+        } else console.log("Invalid Exif data: Invalid tag type.")
+    }, e.parseExifTag = function(t, i, a, o, n) {
+        var r = t.getUint16(a, o);
+        n.exif[r] = e.getExifValue(t, i, a, t.getUint16(a + 2, o), t.getUint32(a + 4, o), o)
     }, e.parseExifTags = function(e, t, i, a, o) {
-        var r, n, s;
-        if (i + 6 > e.byteLength) return void console.log("Invalid Exif data: Invalid directory offset.");
-        if (r = e.getUint16(i, a), n = i + 2 + 12 * r, n + 4 > e.byteLength) return void console.log("Invalid Exif data: Invalid directory size.");
-        for (s = 0; s < r; s += 1) this.parseExifTag(e, t, i + 2 + 12 * s, a, o);
-        return e.getUint32(n, a)
-    }, e.parseExifData = function(t, i, a, o, r) {
-        if (!r.disableExif) {
-            var n, s, l, d = i + 10;
-            if (1165519206 === t.getUint32(i + 4)) {
-                if (d + 8 > t.byteLength) return void console.log("Invalid Exif data: Invalid segment size.");
-                if (0 !== t.getUint16(i + 8)) return void console.log("Invalid Exif data: Missing byte alignment offset.");
+        var n, r, s;
+        if (i + 6 > e.byteLength) console.log("Invalid Exif data: Invalid directory offset.");
+        else {
+            if (n = e.getUint16(i, a), !((r = i + 2 + 12 * n) + 4 > e.byteLength)) {
+                for (s = 0; s < n; s += 1) this.parseExifTag(e, t, i + 2 + 12 * s, a, o);
+                return e.getUint32(r, a)
+            }
+            console.log("Invalid Exif data: Invalid directory size.")
+        }
+    }, e.parseExifData = function(t, i, a, o, n) {
+        if (!n.disableExif) {
+            var r, s, l, d = i + 10;
+            if (1165519206 === t.getUint32(i + 4))
+                if (d + 8 > t.byteLength) console.log("Invalid Exif data: Invalid segment size.");
+                else if (0 === t.getUint16(i + 8)) {
                 switch (t.getUint16(d)) {
                     case 18761:
-                        n = !0;
+                        r = !0;
                         break;
                     case 19789:
-                        n = !1;
+                        r = !1;
                         break;
                     default:
                         return void console.log("Invalid Exif data: Invalid byte alignment marker.")
                 }
-                if (42 !== t.getUint16(d + 2, n)) return void console.log("Invalid Exif data: Missing TIFF marker.");
-                s = t.getUint32(d + 4, n), o.exif = new e.ExifMap, s = e.parseExifTags(t, d, d + s, n, o), s && !r.disableExifThumbnail && (l = {
+                42 === t.getUint16(d + 2, r) ? (s = t.getUint32(d + 4, r), o.exif = new e.ExifMap, (s = e.parseExifTags(t, d, d + s, r, o)) && !n.disableExifThumbnail && (l = {
                     exif: {}
-                }, s = e.parseExifTags(t, d, d + s, n, l), l.exif[513] && (o.exif.Thumbnail = e.getExifThumbnail(t, d + l.exif[513], l.exif[514]))), o.exif[34665] && !r.disableExifSub && e.parseExifTags(t, d, d + o.exif[34665], n, o), o.exif[34853] && !r.disableExifGps && e.parseExifTags(t, d, d + o.exif[34853], n, o)
-            }
+                }, s = e.parseExifTags(t, d, d + s, r, l), l.exif[513] && (o.exif.Thumbnail = e.getExifThumbnail(t, d + l.exif[513], l.exif[514]))), o.exif[34665] && !n.disableExifSub && e.parseExifTags(t, d, d + o.exif[34665], r, o), o.exif[34853] && !n.disableExifGps && e.parseExifTags(t, d, d + o.exif[34853], r, o)) : console.log("Invalid Exif data: Missing TIFF marker.")
+            } else console.log("Invalid Exif data: Missing byte alignment offset.")
         }
     }, e.metaDataParsers.jpeg[65505].push(e.parseExifData)
 }),
 function(e) {
     "use strict";
     "function" == typeof define && define.amd ? define(["./load-image", "./load-image-exif"], e) : "object" == typeof module && module.exports ? e(require("./load-image"), require("./load-image-exif")) : e(window.loadImage)
 }(function(e) {
@@ -549,86 +579,86 @@
         },
         function(e) {
             var t, i = e.tags,
                 a = e.map;
             for (t in i) i.hasOwnProperty(t) && (a[i[t]] = t)
         }(e.ExifMap.prototype), e.ExifMap.prototype.getAll = function() {
             var e, t, i = {};
-            for (e in this) this.hasOwnProperty(e) && (t = this.tags[e], t && (i[t] = this.getText(t)));
+            for (e in this) this.hasOwnProperty(e) && (t = this.tags[e]) && (i[t] = this.getText(t));
             return i
         }
 }),
 function(e) {
     "use strict";
-    "function" == typeof define && define.amd ? define(["./load-image"], e) : e("object" == typeof module && module.exports ? require("./load-image") : window.loadImage)
+    "function" == typeof define && define.amd ? define(["./load-image", "./load-image-scale", "./load-image-meta"], e) : "object" == typeof module && module.exports ? e(require("./load-image"), require("./load-image-scale"), require("./load-image-meta")) : e(window.loadImage)
 }(function(e) {
     "use strict";
     var t = e.hasCanvasOption,
         i = e.hasMetaOption,
         a = e.transformCoordinates,
         o = e.getTransformedOptions;
     e.hasCanvasOption = function(i) {
         return !!i.orientation || t.call(e, i)
     }, e.hasMetaOption = function(t) {
-        return t.orientation === !0 || i.call(e, t)
+        return t && !0 === t.orientation || i.call(e, t)
     }, e.transformCoordinates = function(t, i) {
         a.call(e, t, i);
         var o = t.getContext("2d"),
-            r = t.width,
-            n = t.height,
+            n = t.width,
+            r = t.height,
             s = t.style.width,
             l = t.style.height,
             d = i.orientation;
-        if (d && !(d > 8)) switch (d > 4 && (t.width = n, t.height = r, t.style.width = l, t.style.height = s), d) {
+        if (d && !(d > 8)) switch (d > 4 && (t.width = r, t.height = n, t.style.width = l, t.style.height = s), d) {
             case 2:
-                o.translate(r, 0), o.scale(-1, 1);
+                o.translate(n, 0), o.scale(-1, 1);
                 break;
             case 3:
-                o.translate(r, n), o.rotate(Math.PI);
+                o.translate(n, r), o.rotate(Math.PI);
                 break;
             case 4:
-                o.translate(0, n), o.scale(1, -1);
+                o.translate(0, r), o.scale(1, -1);
                 break;
             case 5:
                 o.rotate(.5 * Math.PI), o.scale(1, -1);
                 break;
             case 6:
-                o.rotate(.5 * Math.PI), o.translate(0, -n);
+                o.rotate(.5 * Math.PI), o.translate(0, -r);
                 break;
             case 7:
-                o.rotate(.5 * Math.PI), o.translate(r, -n), o.scale(-1, 1);
+                o.rotate(.5 * Math.PI), o.translate(n, -r), o.scale(-1, 1);
                 break;
             case 8:
-                o.rotate(-.5 * Math.PI), o.translate(-r, 0)
+                o.rotate(-.5 * Math.PI), o.translate(-n, 0)
         }
     }, e.getTransformedOptions = function(t, i, a) {
-        var r, n, s = o.call(e, t, i),
+        var n, r, s = o.call(e, t, i),
             l = s.orientation;
-        if (l === !0 && a && a.exif && (l = a.exif.get("Orientation")), !l || l > 8 || 1 === l) return s;
-        r = {};
-        for (n in s) s.hasOwnProperty(n) && (r[n] = s[n]);
-        switch (r.orientation = l, l) {
+        if (!0 === l && a && a.exif && (l = a.exif.get("Orientation")), !l || l > 8 || 1 === l) return s;
+        n = {};
+        for (r in s) s.hasOwnProperty(r) && (n[r] = s[r]);
+        switch (n.orientation = l, l) {
             case 2:
-                r.left = s.right, r.right = s.left;
+                n.left = s.right, n.right = s.left;
                 break;
             case 3:
-                r.left = s.right, r.top = s.bottom, r.right = s.left, r.bottom = s.top;
+                n.left = s.right, n.top = s.bottom, n.right = s.left, n.bottom = s.top;
                 break;
             case 4:
-                r.top = s.bottom, r.bottom = s.top;
+                n.top = s.bottom, n.bottom = s.top;
                 break;
             case 5:
-                r.left = s.top, r.top = s.left, r.right = s.bottom, r.bottom = s.right;
+                n.left = s.top, n.top = s.left, n.right = s.bottom, n.bottom = s.right;
                 break;
             case 6:
-                r.left = s.top, r.top = s.right, r.right = s.bottom, r.bottom = s.left;
+                n.left = s.top, n.top = s.right, n.right = s.bottom, n.bottom = s.left;
                 break;
             case 7:
-                r.left = s.bottom, r.top = s.right, r.right = s.top, r.bottom = s.left;
+                n.left = s.bottom, n.top = s.right, n.right = s.top, n.bottom = s.left;
                 break;
             case 8:
-                r.left = s.bottom, r.top = s.left, r.right = s.top, r.bottom = s.right
+                n.left = s.bottom, n.top = s.left, n.right = s.top, n.bottom = s.right
         }
-        return s.orientation > 4 && (r.maxWidth = s.maxHeight, r.maxHeight = s.maxWidth, r.minWidth = s.minHeight, r.minHeight = s.minWidth, r.sourceWidth = s.sourceHeight, r.sourceHeight = s.sourceWidth), r
+        return n.orientation > 4 && (n.maxWidth = s.maxHeight, n.maxHeight = s.maxWidth, n.minWidth = s.minHeight, n.minHeight = s.minWidth, n.sourceWidth = s.sourceHeight, n.sourceHeight = s.sourceWidth), n
     }
 });
 //# sourceMappingURL=load-image.all.min.js.map
```

### Comparing `cloudinary-1.8.0/cloudinary/templates/cloudinary_includes.html` & `cloudinary-1.9.0/cloudinary/templates/cloudinary_includes.html`

 * *Files identical despite different names*

### Comparing `cloudinary-1.8.0/cloudinary/templatetags/cloudinary.py` & `cloudinary-1.9.0/cloudinary/templatetags/cloudinary.py`

 * *Files identical despite different names*

### Comparing `cloudinary-1.8.0/cloudinary/uploader.py` & `cloudinary-1.9.0/cloudinary/uploader.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import json
 import re
 import socket
 from os.path import getsize
 
 import cloudinary
 import urllib3
+import certifi
 from cloudinary import utils
 from cloudinary.api import Error
 from cloudinary.compat import string_types
 from urllib3.exceptions import HTTPError
 from urllib3 import PoolManager
 
 try:
@@ -24,15 +25,18 @@
     from urllib3.packages.ordered_dict import OrderedDict
 
 if is_appengine_sandbox():
     # AppEngineManager uses AppEngine's URLFetch API behind the scenes
     _http = AppEngineManager()
 else:
     # PoolManager uses a socket-level API behind the scenes
-    _http = PoolManager()
+    _http = PoolManager(
+        cert_reqs='CERT_REQUIRED',
+        ca_certs=certifi.where()
+    )
 
 
 def upload(file, **options):
     params = utils.build_upload_params(**options)
     return call_api("upload", params, file=file, **options)
```

### Comparing `cloudinary-1.8.0/cloudinary/utils.py` & `cloudinary-1.9.0/cloudinary/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -617,15 +617,16 @@
               "detection": options.get("detection"),
               "similarity_search": options.get("similarity_search"),
               "background_removal": options.get("background_removal"),
               "upload_preset": options.get("upload_preset"),
               "phash": options.get("phash"),
               "return_delete_token": options.get("return_delete_token"),
               "auto_tagging": options.get("auto_tagging") and str(options.get("auto_tagging")),
-              "responsive_breakpoints": generate_responsive_breakpoints_string(options.get("responsive_breakpoints"))}
+              "responsive_breakpoints": generate_responsive_breakpoints_string(options.get("responsive_breakpoints")),
+              "async": options.get("async")}
     return params
 
 
 def __process_text_options(layer, layer_parameter):
     font_family = layer.get("font_family")
     font_size = layer.get("font_size")
     keywords = []
```

### Comparing `cloudinary-1.8.0/cloudinary.egg-info/PKG-INFO` & `cloudinary-1.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 1.1
 Name: cloudinary
-Version: 1.8.0
+Version: 1.9.0
 Summary: Python and Django SDK for Cloudinary
 Home-page: http://cloudinary.com
 Author: Cloudinary
 Author-email: info@cloudinary.com
 License: MIT
+Description-Content-Type: UNKNOWN
 Description: Cloudinary
         ==========
         
         Cloudinary is a cloud service that offers a solution to a web
         application's entire image management pipeline.
         
         Easily upload images to the cloud. Automatically perform smart image
@@ -440,29 +441,32 @@
         
         
 Keywords: cloudinary image video upload crop resize filter transformation manipulation cdn
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
+Classifier: Framework :: Django :: 1.4
+Classifier: Framework :: Django :: 1.5
+Classifier: Framework :: Django :: 1.6
+Classifier: Framework :: Django :: 1.7
+Classifier: Framework :: Django :: 1.8
 Classifier: Framework :: Django :: 1.9
 Classifier: Framework :: Django :: 1.10
+Classifier: Framework :: Django :: 1.11
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.0
-Classifier: Programming Language :: Python :: 3.1
-Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Multimedia :: Graphics :: Graphics Conversion
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Sound/Audio :: Conversion
 Classifier: Topic :: Multimedia :: Video
```

### Comparing `cloudinary-1.8.0/cloudinary.egg-info/SOURCES.txt` & `cloudinary-1.9.0/cloudinary.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE.txt
 MANIFEST.in
 README.rst
+branches.txt
 setup.cfg
 setup.py
 cloudinary/__init__.py
 cloudinary/api.py
 cloudinary/auth_token.py
 cloudinary/compat.py
 cloudinary/forms.py
```

### Comparing `cloudinary-1.8.0/PKG-INFO` & `cloudinary-1.9.0/cloudinary.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 1.1
 Name: cloudinary
-Version: 1.8.0
+Version: 1.9.0
 Summary: Python and Django SDK for Cloudinary
 Home-page: http://cloudinary.com
 Author: Cloudinary
 Author-email: info@cloudinary.com
 License: MIT
+Description-Content-Type: UNKNOWN
 Description: Cloudinary
         ==========
         
         Cloudinary is a cloud service that offers a solution to a web
         application's entire image management pipeline.
         
         Easily upload images to the cloud. Automatically perform smart image
@@ -440,29 +441,32 @@
         
         
 Keywords: cloudinary image video upload crop resize filter transformation manipulation cdn
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
+Classifier: Framework :: Django :: 1.4
+Classifier: Framework :: Django :: 1.5
+Classifier: Framework :: Django :: 1.6
+Classifier: Framework :: Django :: 1.7
+Classifier: Framework :: Django :: 1.8
 Classifier: Framework :: Django :: 1.9
 Classifier: Framework :: Django :: 1.10
+Classifier: Framework :: Django :: 1.11
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.0
-Classifier: Programming Language :: Python :: 3.1
-Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Multimedia :: Graphics :: Graphics Conversion
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Sound/Audio :: Conversion
 Classifier: Topic :: Multimedia :: Video
```

### Comparing `cloudinary-1.8.0/README.rst` & `cloudinary-1.9.0/README.rst`

 * *Files identical despite different names*

