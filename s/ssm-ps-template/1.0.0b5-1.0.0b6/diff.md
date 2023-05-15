# Comparing `tmp/ssm-ps-template-1.0.0b5.tar.gz` & `tmp/ssm-ps-template-1.0.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssm-ps-template-1.0.0b5.tar", last modified: Mon May 15 20:12:14 2023, max compression
+gzip compressed data, was "ssm-ps-template-1.0.0b6.tar", last modified: Mon May 15 20:40:05 2023, max compression
```

## Comparing `ssm-ps-template-1.0.0b5.tar` & `ssm-ps-template-1.0.0b6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 20:12:14.152781 ssm-ps-template-1.0.0b5/
--rw-r--r--   0 root         (0) root         (0)     1495 2023-05-15 20:12:03.000000 ssm-ps-template-1.0.0b5/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     8152 2023-05-15 20:12:14.152781 ssm-ps-template-1.0.0b5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5527 2023-05-15 20:12:03.000000 ssm-ps-template-1.0.0b5/README.md
--rw-r--r--   0 root         (0) root         (0)     1857 2023-05-15 20:12:03.000000 ssm-ps-template-1.0.0b5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 20:12:14.152781 ssm-ps-template-1.0.0b5/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 20:12:14.148781 ssm-ps-template-1.0.0b5/ssm_ps_template/
--rw-r--r--   0 root         (0) root         (0)      165 2023-05-15 20:12:03.000000 ssm-ps-template-1.0.0b5/ssm_ps_template/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2333 2023-05-15 20:12:03.000000 ssm-ps-template-1.0.0b5/ssm_ps_template/__main__.py
--rw-r--r--   0 root         (0) root         (0)     2182 2023-05-15 20:12:03.000000 ssm-ps-template-1.0.0b5/ssm_ps_template/config.py
--rw-r--r--   0 root         (0) root         (0)     5644 2023-05-15 20:12:03.000000 ssm-ps-template-1.0.0b5/ssm_ps_template/discover.py
--rw-r--r--   0 root         (0) root         (0)     1558 2023-05-15 20:12:03.000000 ssm-ps-template-1.0.0b5/ssm_ps_template/render.py
--rw-r--r--   0 root         (0) root         (0)     2820 2023-05-15 20:12:03.000000 ssm-ps-template-1.0.0b5/ssm_ps_template/ssm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 20:12:14.152781 ssm-ps-template-1.0.0b5/ssm_ps_template.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8152 2023-05-15 20:12:14.000000 ssm-ps-template-1.0.0b5/ssm_ps_template.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      496 2023-05-15 20:12:14.000000 ssm-ps-template-1.0.0b5/ssm_ps_template.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 20:12:14.000000 ssm-ps-template-1.0.0b5/ssm_ps_template.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-05-15 20:12:14.000000 ssm-ps-template-1.0.0b5/ssm_ps_template.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      246 2023-05-15 20:12:14.000000 ssm-ps-template-1.0.0b5/ssm_ps_template.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-15 20:12:14.000000 ssm-ps-template-1.0.0b5/ssm_ps_template.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 20:12:14.152781 ssm-ps-template-1.0.0b5/tests/
--rw-r--r--   0 root         (0) root         (0)     2254 2023-05-15 20:12:03.000000 ssm-ps-template-1.0.0b5/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)      405 2023-05-15 20:12:03.000000 ssm-ps-template-1.0.0b5/tests/test_discover.py
--rw-r--r--   0 root         (0) root         (0)     1593 2023-05-15 20:12:03.000000 ssm-ps-template-1.0.0b5/tests/test_render.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 20:40:05.817200 ssm-ps-template-1.0.0b6/
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-05-15 20:39:56.000000 ssm-ps-template-1.0.0b6/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     8152 2023-05-15 20:40:05.817200 ssm-ps-template-1.0.0b6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5527 2023-05-15 20:39:56.000000 ssm-ps-template-1.0.0b6/README.md
+-rw-r--r--   0 root         (0) root         (0)     1857 2023-05-15 20:39:56.000000 ssm-ps-template-1.0.0b6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 20:40:05.817200 ssm-ps-template-1.0.0b6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 20:40:05.817200 ssm-ps-template-1.0.0b6/ssm_ps_template/
+-rw-r--r--   0 root         (0) root         (0)      165 2023-05-15 20:39:56.000000 ssm-ps-template-1.0.0b6/ssm_ps_template/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2312 2023-05-15 20:39:56.000000 ssm-ps-template-1.0.0b6/ssm_ps_template/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     2161 2023-05-15 20:39:56.000000 ssm-ps-template-1.0.0b6/ssm_ps_template/config.py
+-rw-r--r--   0 root         (0) root         (0)     5644 2023-05-15 20:39:56.000000 ssm-ps-template-1.0.0b6/ssm_ps_template/discover.py
+-rw-r--r--   0 root         (0) root         (0)     1558 2023-05-15 20:39:56.000000 ssm-ps-template-1.0.0b6/ssm_ps_template/render.py
+-rw-r--r--   0 root         (0) root         (0)     2727 2023-05-15 20:39:56.000000 ssm-ps-template-1.0.0b6/ssm_ps_template/ssm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 20:40:05.817200 ssm-ps-template-1.0.0b6/ssm_ps_template.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8152 2023-05-15 20:40:05.000000 ssm-ps-template-1.0.0b6/ssm_ps_template.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      496 2023-05-15 20:40:05.000000 ssm-ps-template-1.0.0b6/ssm_ps_template.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 20:40:05.000000 ssm-ps-template-1.0.0b6/ssm_ps_template.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-05-15 20:40:05.000000 ssm-ps-template-1.0.0b6/ssm_ps_template.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      246 2023-05-15 20:40:05.000000 ssm-ps-template-1.0.0b6/ssm_ps_template.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-15 20:40:05.000000 ssm-ps-template-1.0.0b6/ssm_ps_template.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 20:40:05.817200 ssm-ps-template-1.0.0b6/tests/
+-rw-r--r--   0 root         (0) root         (0)     2254 2023-05-15 20:39:56.000000 ssm-ps-template-1.0.0b6/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)      405 2023-05-15 20:39:56.000000 ssm-ps-template-1.0.0b6/tests/test_discover.py
+-rw-r--r--   0 root         (0) root         (0)     1593 2023-05-15 20:39:56.000000 ssm-ps-template-1.0.0b6/tests/test_render.py
```

### Comparing `ssm-ps-template-1.0.0b5/LICENSE.txt` & `ssm-ps-template-1.0.0b6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-1.0.0b5/PKG-INFO` & `ssm-ps-template-1.0.0b6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-ps-template
-Version: 1.0.0b5
+Version: 1.0.0b6
 Summary: CLI for rendering configuration templates with SSM Parameter Store as a data source
 Author-email: "Gavin M. Roy" <gavinmroy@gmail.com>
 License: Copyright (c) 2023 Gavin M. Roy
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
```

### Comparing `ssm-ps-template-1.0.0b5/README.md` & `ssm-ps-template-1.0.0b6/README.md`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-1.0.0b5/pyproject.toml` & `ssm-ps-template-1.0.0b6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ssm-ps-template"
-version = "1.0.0b5"
+version = "1.0.0b6"
 description = "CLI for rendering configuration templates with SSM Parameter Store as a data source"
 authors = [
     {name = "Gavin M. Roy", email="gavinmroy@gmail.com"}
 ]
 classifiers = [
     "Topic :: Software Development",
     "License :: OSI Approved :: BSD License",
```

### Comparing `ssm-ps-template-1.0.0b5/ssm_ps_template/__main__.py` & `ssm-ps-template-1.0.0b6/ssm_ps_template/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 
     start_time = time.time()
     for template in args.config[0].templates:
         variable_discovery = discover.Variables(template.source)
         variables = sorted(variable_discovery.discover())
 
         try:
-            values = parameter_store.fetch_variables(variables,
-                                                     template.prefix)
+            values = parameter_store.fetch_variables(
+                variables, args.prefix or template.prefix)
         except (exceptions.ClientError,
                 exceptions.UnauthorizedSSOTokenError) as err:
             LOGGER.error('Error fetching parameters: %s', err)
             sys.exit(1)
 
         renderer = render.Renderer(source=template.source, variables=variables)
         with template.destination.open('w') as handle:
```

### Comparing `ssm-ps-template-1.0.0b5/ssm_ps_template/config.py` & `ssm-ps-template-1.0.0b6/ssm_ps_template/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 def _load_configuration(value: dict) -> Configuration:
     templates = []
     try:
         for template in value['templates'] or []:
             templates.append(_entry_to_template(
                 source=template['source'],
                 destination=template['destination'],
-                prefix=value.get('prefix', template.get('prefix'))))
+                prefix=template.get('prefix')))
     except KeyError as error:
         raise argparse.ArgumentTypeError(
             f'Failed to load configuration due to invalid key: {error}')
     return Configuration(
         templates=templates,
         profile=value.get('profile'),
         region=value.get('region'),
```

### Comparing `ssm-ps-template-1.0.0b5/ssm_ps_template/discover.py` & `ssm-ps-template-1.0.0b6/ssm_ps_template/discover.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-1.0.0b5/ssm_ps_template/render.py` & `ssm-ps-template-1.0.0b6/ssm_ps_template/render.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-1.0.0b5/ssm_ps_template/ssm.py` & `ssm-ps-template-1.0.0b6/ssm_ps_template/ssm.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,42 +12,41 @@
     def __init__(self,
                  profile: typing.Optional[str] = None,
                  region: typing.Optional[str] = None):
         self._session = boto3.Session(profile_name=profile, region_name=region)
         self._client = self._session.client('ssm')
         self._ssm = boto3.client('ssm')
 
-    def fetch_variables(self, variables: list,
-                        prefix: typing.Optional[str]) -> typing.Dict[str, str]:
+    def fetch_variables(self,
+                        variables: list,
+                        prefix: str) -> typing.Dict[str, str]:
         # Build the variables
         names = [
             '/'.join([prefix.rstrip('/'), v])
             if prefix and not v.startswith('/') else v for v in variables
         ]
 
         paths = [name for name in names if name.endswith('/')]
         names = [name for name in names if not name.endswith('/')]
 
         LOGGER.debug('Fetching %r', names)
 
         values = {}
         while names:
-            response = self._client.get_parameters(Names=names[:10],
-                                                   WithDecryption=True)
-
+            response = self._client.get_parameters(
+                Names=names[:10], WithDecryption=True)
             for param in response['Parameters']:
                 values = self.add_parameter(param, prefix, variables, values)
             names = names[10:]
 
         path_values = flatdict.FlatDict(delimiter='/')
         for path in paths:
             paginator = self._client.get_paginator('get_parameters_by_path')
-            for page in paginator.paginate(Path=path,
-                                           Recursive=True,
-                                           WithDecryption=True):
+            for page in paginator.paginate(
+                    Path=path, Recursive=True, WithDecryption=True):
                 for param in page['Parameters']:
                     LOGGER.debug('Param %r', param)
                     path_values = self.add_parameter(param, prefix, variables,
                                                      path_values)
         for key, value in path_values.as_dict().items():
             values[f'{key}/'] = value
```

### Comparing `ssm-ps-template-1.0.0b5/ssm_ps_template.egg-info/PKG-INFO` & `ssm-ps-template-1.0.0b6/ssm_ps_template.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-ps-template
-Version: 1.0.0b5
+Version: 1.0.0b6
 Summary: CLI for rendering configuration templates with SSM Parameter Store as a data source
 Author-email: "Gavin M. Roy" <gavinmroy@gmail.com>
 License: Copyright (c) 2023 Gavin M. Roy
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
```

### Comparing `ssm-ps-template-1.0.0b5/tests/test_config.py` & `ssm-ps-template-1.0.0b6/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-1.0.0b5/tests/test_render.py` & `ssm-ps-template-1.0.0b6/tests/test_render.py`

 * *Files identical despite different names*

