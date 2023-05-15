# Comparing `tmp/ssm-ps-template-1.0.0b4.tar.gz` & `tmp/ssm-ps-template-1.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssm-ps-template-1.0.0b4.tar", last modified: Mon May 15 15:14:10 2023, max compression
+gzip compressed data, was "ssm-ps-template-1.0.0b5.tar", last modified: Mon May 15 20:12:14 2023, max compression
```

## Comparing `ssm-ps-template-1.0.0b4.tar` & `ssm-ps-template-1.0.0b5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 15:14:10.639861 ssm-ps-template-1.0.0b4/
--rw-r--r--   0 root         (0) root         (0)     1495 2023-05-15 15:13:59.000000 ssm-ps-template-1.0.0b4/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     8152 2023-05-15 15:14:10.639861 ssm-ps-template-1.0.0b4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5527 2023-05-15 15:13:59.000000 ssm-ps-template-1.0.0b4/README.md
--rw-r--r--   0 root         (0) root         (0)     1857 2023-05-15 15:13:59.000000 ssm-ps-template-1.0.0b4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 15:14:10.639861 ssm-ps-template-1.0.0b4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 15:14:10.635861 ssm-ps-template-1.0.0b4/ssm_ps_template/
--rw-r--r--   0 root         (0) root         (0)      165 2023-05-15 15:13:59.000000 ssm-ps-template-1.0.0b4/ssm_ps_template/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2247 2023-05-15 15:13:59.000000 ssm-ps-template-1.0.0b4/ssm_ps_template/__main__.py
--rw-r--r--   0 root         (0) root         (0)     2080 2023-05-15 15:13:59.000000 ssm-ps-template-1.0.0b4/ssm_ps_template/config.py
--rw-r--r--   0 root         (0) root         (0)     5644 2023-05-15 15:13:59.000000 ssm-ps-template-1.0.0b4/ssm_ps_template/discover.py
--rw-r--r--   0 root         (0) root         (0)     1558 2023-05-15 15:13:59.000000 ssm-ps-template-1.0.0b4/ssm_ps_template/render.py
--rw-r--r--   0 root         (0) root         (0)     2820 2023-05-15 15:13:59.000000 ssm-ps-template-1.0.0b4/ssm_ps_template/ssm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 15:14:10.635861 ssm-ps-template-1.0.0b4/ssm_ps_template.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8152 2023-05-15 15:14:10.000000 ssm-ps-template-1.0.0b4/ssm_ps_template.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      496 2023-05-15 15:14:10.000000 ssm-ps-template-1.0.0b4/ssm_ps_template.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 15:14:10.000000 ssm-ps-template-1.0.0b4/ssm_ps_template.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-05-15 15:14:10.000000 ssm-ps-template-1.0.0b4/ssm_ps_template.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      246 2023-05-15 15:14:10.000000 ssm-ps-template-1.0.0b4/ssm_ps_template.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-15 15:14:10.000000 ssm-ps-template-1.0.0b4/ssm_ps_template.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 15:14:10.639861 ssm-ps-template-1.0.0b4/tests/
--rw-r--r--   0 root         (0) root         (0)     2244 2023-05-15 15:13:59.000000 ssm-ps-template-1.0.0b4/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)      405 2023-05-15 15:13:59.000000 ssm-ps-template-1.0.0b4/tests/test_discover.py
--rw-r--r--   0 root         (0) root         (0)     1593 2023-05-15 15:13:59.000000 ssm-ps-template-1.0.0b4/tests/test_render.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 20:12:14.152781 ssm-ps-template-1.0.0b5/
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-05-15 20:12:03.000000 ssm-ps-template-1.0.0b5/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     8152 2023-05-15 20:12:14.152781 ssm-ps-template-1.0.0b5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5527 2023-05-15 20:12:03.000000 ssm-ps-template-1.0.0b5/README.md
+-rw-r--r--   0 root         (0) root         (0)     1857 2023-05-15 20:12:03.000000 ssm-ps-template-1.0.0b5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 20:12:14.152781 ssm-ps-template-1.0.0b5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 20:12:14.148781 ssm-ps-template-1.0.0b5/ssm_ps_template/
+-rw-r--r--   0 root         (0) root         (0)      165 2023-05-15 20:12:03.000000 ssm-ps-template-1.0.0b5/ssm_ps_template/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2333 2023-05-15 20:12:03.000000 ssm-ps-template-1.0.0b5/ssm_ps_template/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     2182 2023-05-15 20:12:03.000000 ssm-ps-template-1.0.0b5/ssm_ps_template/config.py
+-rw-r--r--   0 root         (0) root         (0)     5644 2023-05-15 20:12:03.000000 ssm-ps-template-1.0.0b5/ssm_ps_template/discover.py
+-rw-r--r--   0 root         (0) root         (0)     1558 2023-05-15 20:12:03.000000 ssm-ps-template-1.0.0b5/ssm_ps_template/render.py
+-rw-r--r--   0 root         (0) root         (0)     2820 2023-05-15 20:12:03.000000 ssm-ps-template-1.0.0b5/ssm_ps_template/ssm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 20:12:14.152781 ssm-ps-template-1.0.0b5/ssm_ps_template.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8152 2023-05-15 20:12:14.000000 ssm-ps-template-1.0.0b5/ssm_ps_template.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      496 2023-05-15 20:12:14.000000 ssm-ps-template-1.0.0b5/ssm_ps_template.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 20:12:14.000000 ssm-ps-template-1.0.0b5/ssm_ps_template.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-05-15 20:12:14.000000 ssm-ps-template-1.0.0b5/ssm_ps_template.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      246 2023-05-15 20:12:14.000000 ssm-ps-template-1.0.0b5/ssm_ps_template.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-15 20:12:14.000000 ssm-ps-template-1.0.0b5/ssm_ps_template.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 20:12:14.152781 ssm-ps-template-1.0.0b5/tests/
+-rw-r--r--   0 root         (0) root         (0)     2254 2023-05-15 20:12:03.000000 ssm-ps-template-1.0.0b5/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)      405 2023-05-15 20:12:03.000000 ssm-ps-template-1.0.0b5/tests/test_discover.py
+-rw-r--r--   0 root         (0) root         (0)     1593 2023-05-15 20:12:03.000000 ssm-ps-template-1.0.0b5/tests/test_render.py
```

### Comparing `ssm-ps-template-1.0.0b4/LICENSE.txt` & `ssm-ps-template-1.0.0b5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-1.0.0b4/PKG-INFO` & `ssm-ps-template-1.0.0b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-ps-template
-Version: 1.0.0b4
+Version: 1.0.0b5
 Summary: CLI for rendering configuration templates with SSM Parameter Store as a data source
 Author-email: "Gavin M. Roy" <gavinmroy@gmail.com>
 License: Copyright (c) 2023 Gavin M. Roy
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
```

### Comparing `ssm-ps-template-1.0.0b4/README.md` & `ssm-ps-template-1.0.0b5/README.md`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-1.0.0b4/pyproject.toml` & `ssm-ps-template-1.0.0b5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ssm-ps-template"
-version = "1.0.0b4"
+version = "1.0.0b5"
 description = "CLI for rendering configuration templates with SSM Parameter Store as a data source"
 authors = [
     {name = "Gavin M. Roy", email="gavinmroy@gmail.com"}
 ]
 classifiers = [
     "Topic :: Software Development",
     "License :: OSI Approved :: BSD License",
```

### Comparing `ssm-ps-template-1.0.0b4/ssm_ps_template/__main__.py` & `ssm-ps-template-1.0.0b5/ssm_ps_template/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,15 +35,17 @@
     for template in args.config[0].templates:
         variable_discovery = discover.Variables(template.source)
         variables = sorted(variable_discovery.discover())
 
         try:
             values = parameter_store.fetch_variables(variables,
                                                      template.prefix)
-        except (exceptions.ClientError, exceptions.UnauthorizedSSOTokenError):
+        except (exceptions.ClientError,
+                exceptions.UnauthorizedSSOTokenError) as err:
+            LOGGER.error('Error fetching parameters: %s', err)
             sys.exit(1)
 
         renderer = render.Renderer(source=template.source, variables=variables)
         with template.destination.open('w') as handle:
             handle.write(renderer.render(values))
 
         LOGGER.info('Rendered %s in %0.2f seconds', template.destination,
```

### Comparing `ssm-ps-template-1.0.0b4/ssm_ps_template/config.py` & `ssm-ps-template-1.0.0b5/ssm_ps_template/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,35 +20,39 @@
     templates: list[Template]
     profile: typing.Optional[str]
     region: typing.Optional[str]
     verbose: bool
 
 
 def _load_configuration(value: dict) -> Configuration:
+    templates = []
     try:
-        return Configuration(
-            templates=[
-                _entry_to_template(prefix=value.get('prefix'), **template)
-                for template in value['templates']],
-            profile=value.get('profile'),
-            region=value.get('region'),
-            verbose=value.get('verbose', False))
+        for template in value['templates'] or []:
+            templates.append(_entry_to_template(
+                source=template['source'],
+                destination=template['destination'],
+                prefix=value.get('prefix', template.get('prefix'))))
     except KeyError as error:
         raise argparse.ArgumentTypeError(
             f'Failed to load configuration due to invalid key: {error}')
+    return Configuration(
+        templates=templates,
+        profile=value.get('profile'),
+        region=value.get('region'),
+        verbose=value.get('verbose', False))
 
 
-def _entry_to_template(prefix: typing.Optional[str], **kwargs) -> Template:
+def _entry_to_template(**kwargs) -> Template:
     source = pathlib.Path(kwargs['source'])
     if not source.exists():
         raise argparse.ArgumentTypeError(
             f'Specified template {source} does not exist')
     return Template(source=source,
                     destination=pathlib.Path(kwargs['destination']),
-                    prefix=kwargs.get('prefix', prefix))
+                    prefix=kwargs['prefix'])
 
 
 def configuration_file(value: str) -> Configuration:
     """Load the configuration from the specified path"""
     path = pathlib.Path(value)
     if not path.exists():
         raise argparse.ArgumentTypeError(f'{value} does not exist')
```

### Comparing `ssm-ps-template-1.0.0b4/ssm_ps_template/discover.py` & `ssm-ps-template-1.0.0b5/ssm_ps_template/discover.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-1.0.0b4/ssm_ps_template/render.py` & `ssm-ps-template-1.0.0b5/ssm_ps_template/render.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-1.0.0b4/ssm_ps_template/ssm.py` & `ssm-ps-template-1.0.0b5/ssm_ps_template/ssm.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-1.0.0b4/ssm_ps_template.egg-info/PKG-INFO` & `ssm-ps-template-1.0.0b5/ssm_ps_template.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-ps-template
-Version: 1.0.0b4
+Version: 1.0.0b5
 Summary: CLI for rendering configuration templates with SSM Parameter Store as a data source
 Author-email: "Gavin M. Roy" <gavinmroy@gmail.com>
 License: Copyright (c) 2023 Gavin M. Roy
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
```

### Comparing `ssm-ps-template-1.0.0b4/tests/test_config.py` & `ssm-ps-template-1.0.0b5/tests/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
     def setUp(self) -> None:
         self.expectation = config.Configuration(
             templates=[
                 config.Template(
                     source=pathlib.Path('tests/templates/case1a.tmpl'),
                     destination=pathlib.Path('build/case1a.out'),
-                    prefix=None),
+                    prefix='/foo/bar/baz'),
                 config.Template(
                     source=pathlib.Path('tests/templates/case1b.tmpl'),
                     destination=pathlib.Path('build/case1b.out'),
                     prefix=None)],
             profile=None,
             region=None,
             verbose=False)
```

### Comparing `ssm-ps-template-1.0.0b4/tests/test_render.py` & `ssm-ps-template-1.0.0b5/tests/test_render.py`

 * *Files identical despite different names*

