# Comparing `tmp/ssm-ps-template-1.0.0b3.tar.gz` & `tmp/ssm-ps-template-1.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssm-ps-template-1.0.0b3.tar", last modified: Tue May  9 18:04:37 2023, max compression
+gzip compressed data, was "ssm-ps-template-1.0.0b4.tar", last modified: Mon May 15 15:14:10 2023, max compression
```

## Comparing `ssm-ps-template-1.0.0b3.tar` & `ssm-ps-template-1.0.0b4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 18:04:37.577577 ssm-ps-template-1.0.0b3/
--rw-r--r--   0 root         (0) root         (0)     1495 2023-05-09 18:04:25.000000 ssm-ps-template-1.0.0b3/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     8048 2023-05-09 18:04:37.577577 ssm-ps-template-1.0.0b3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5423 2023-05-09 18:04:25.000000 ssm-ps-template-1.0.0b3/README.md
--rw-r--r--   0 root         (0) root         (0)     1856 2023-05-09 18:04:25.000000 ssm-ps-template-1.0.0b3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 18:04:37.577577 ssm-ps-template-1.0.0b3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 18:04:37.573577 ssm-ps-template-1.0.0b3/ssm_ps_template/
--rw-r--r--   0 root         (0) root         (0)      165 2023-05-09 18:04:25.000000 ssm-ps-template-1.0.0b3/ssm_ps_template/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2177 2023-05-09 18:04:25.000000 ssm-ps-template-1.0.0b3/ssm_ps_template/__main__.py
--rw-r--r--   0 root         (0) root         (0)     2080 2023-05-09 18:04:25.000000 ssm-ps-template-1.0.0b3/ssm_ps_template/config.py
--rw-r--r--   0 root         (0) root         (0)     5644 2023-05-09 18:04:25.000000 ssm-ps-template-1.0.0b3/ssm_ps_template/discover.py
--rw-r--r--   0 root         (0) root         (0)     1558 2023-05-09 18:04:25.000000 ssm-ps-template-1.0.0b3/ssm_ps_template/render.py
--rw-r--r--   0 root         (0) root         (0)     2820 2023-05-09 18:04:25.000000 ssm-ps-template-1.0.0b3/ssm_ps_template/ssm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 18:04:37.577577 ssm-ps-template-1.0.0b3/ssm_ps_template.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8048 2023-05-09 18:04:37.000000 ssm-ps-template-1.0.0b3/ssm_ps_template.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      496 2023-05-09 18:04:37.000000 ssm-ps-template-1.0.0b3/ssm_ps_template.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 18:04:37.000000 ssm-ps-template-1.0.0b3/ssm_ps_template.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-05-09 18:04:37.000000 ssm-ps-template-1.0.0b3/ssm_ps_template.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      246 2023-05-09 18:04:37.000000 ssm-ps-template-1.0.0b3/ssm_ps_template.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-09 18:04:37.000000 ssm-ps-template-1.0.0b3/ssm_ps_template.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 18:04:37.577577 ssm-ps-template-1.0.0b3/tests/
--rw-r--r--   0 root         (0) root         (0)     2244 2023-05-09 18:04:25.000000 ssm-ps-template-1.0.0b3/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)      405 2023-05-09 18:04:25.000000 ssm-ps-template-1.0.0b3/tests/test_discover.py
--rw-r--r--   0 root         (0) root         (0)     1593 2023-05-09 18:04:25.000000 ssm-ps-template-1.0.0b3/tests/test_render.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 15:14:10.639861 ssm-ps-template-1.0.0b4/
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-05-15 15:13:59.000000 ssm-ps-template-1.0.0b4/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     8152 2023-05-15 15:14:10.639861 ssm-ps-template-1.0.0b4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5527 2023-05-15 15:13:59.000000 ssm-ps-template-1.0.0b4/README.md
+-rw-r--r--   0 root         (0) root         (0)     1857 2023-05-15 15:13:59.000000 ssm-ps-template-1.0.0b4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 15:14:10.639861 ssm-ps-template-1.0.0b4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 15:14:10.635861 ssm-ps-template-1.0.0b4/ssm_ps_template/
+-rw-r--r--   0 root         (0) root         (0)      165 2023-05-15 15:13:59.000000 ssm-ps-template-1.0.0b4/ssm_ps_template/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2247 2023-05-15 15:13:59.000000 ssm-ps-template-1.0.0b4/ssm_ps_template/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     2080 2023-05-15 15:13:59.000000 ssm-ps-template-1.0.0b4/ssm_ps_template/config.py
+-rw-r--r--   0 root         (0) root         (0)     5644 2023-05-15 15:13:59.000000 ssm-ps-template-1.0.0b4/ssm_ps_template/discover.py
+-rw-r--r--   0 root         (0) root         (0)     1558 2023-05-15 15:13:59.000000 ssm-ps-template-1.0.0b4/ssm_ps_template/render.py
+-rw-r--r--   0 root         (0) root         (0)     2820 2023-05-15 15:13:59.000000 ssm-ps-template-1.0.0b4/ssm_ps_template/ssm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 15:14:10.635861 ssm-ps-template-1.0.0b4/ssm_ps_template.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8152 2023-05-15 15:14:10.000000 ssm-ps-template-1.0.0b4/ssm_ps_template.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      496 2023-05-15 15:14:10.000000 ssm-ps-template-1.0.0b4/ssm_ps_template.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 15:14:10.000000 ssm-ps-template-1.0.0b4/ssm_ps_template.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-05-15 15:14:10.000000 ssm-ps-template-1.0.0b4/ssm_ps_template.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      246 2023-05-15 15:14:10.000000 ssm-ps-template-1.0.0b4/ssm_ps_template.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-15 15:14:10.000000 ssm-ps-template-1.0.0b4/ssm_ps_template.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 15:14:10.639861 ssm-ps-template-1.0.0b4/tests/
+-rw-r--r--   0 root         (0) root         (0)     2244 2023-05-15 15:13:59.000000 ssm-ps-template-1.0.0b4/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)      405 2023-05-15 15:13:59.000000 ssm-ps-template-1.0.0b4/tests/test_discover.py
+-rw-r--r--   0 root         (0) root         (0)     1593 2023-05-15 15:13:59.000000 ssm-ps-template-1.0.0b4/tests/test_render.py
```

### Comparing `ssm-ps-template-1.0.0b3/LICENSE.txt` & `ssm-ps-template-1.0.0b4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-1.0.0b3/PKG-INFO` & `ssm-ps-template-1.0.0b4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-ps-template
-Version: 1.0.0b3
+Version: 1.0.0b4
 Summary: CLI for rendering configuration templates with SSM Parameter Store as a data source
 Author-email: "Gavin M. Roy" <gavinmroy@gmail.com>
 License: Copyright (c) 2023 Gavin M. Roy
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -149,22 +149,24 @@
 settings: {% set values = settings/ %}
 {{ values | toyaml | indent(2, first=True) }}
 ```
 
 ## Command Line Usage
 
 ```
-usage: ssm-ps-template [-h] [--aws-profile AWS_PROFILE] [--aws-region AWS_REGION] [--prefix] [--verbose] config
+usage: ssm-ps-template [-h] [--aws-profile AWS_PROFILE] [--aws-region AWS_REGION] [--prefix PREFIX] [--verbose] config
+
 Templating for SSM Parameter Store
 
 positional arguments:
   config
 
 optional arguments:
   -h, --help            show this help message and exit
   --aws-profile AWS_PROFILE
                         AWS Profile
   --aws-region AWS_REGION
                         AWS Region
-  --prefix              Default SSM Key Prefix
+  --prefix PREFIX       Default SSM Key Prefix
   --verbose
 ```
+Note that the default SSM prefix can also be set with the `PARAMS_PREFIX` environment variable.
```

### Comparing `ssm-ps-template-1.0.0b3/README.md` & `ssm-ps-template-1.0.0b4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -100,22 +100,24 @@
 settings: {% set values = settings/ %}
 {{ values | toyaml | indent(2, first=True) }}
 ```
 
 ## Command Line Usage
 
 ```
-usage: ssm-ps-template [-h] [--aws-profile AWS_PROFILE] [--aws-region AWS_REGION] [--prefix] [--verbose] config
+usage: ssm-ps-template [-h] [--aws-profile AWS_PROFILE] [--aws-region AWS_REGION] [--prefix PREFIX] [--verbose] config
+
 Templating for SSM Parameter Store
 
 positional arguments:
   config
 
 optional arguments:
   -h, --help            show this help message and exit
   --aws-profile AWS_PROFILE
                         AWS Profile
   --aws-region AWS_REGION
                         AWS Region
-  --prefix              Default SSM Key Prefix
+  --prefix PREFIX       Default SSM Key Prefix
   --verbose
 ```
+Note that the default SSM prefix can also be set with the `PARAMS_PREFIX` environment variable.
```

### Comparing `ssm-ps-template-1.0.0b3/pyproject.toml` & `ssm-ps-template-1.0.0b4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ssm-ps-template"
-version = "1.0.0b3"
+version = "1.0.0b4"
 description = "CLI for rendering configuration templates with SSM Parameter Store as a data source"
 authors = [
     {name = "Gavin M. Roy", email="gavinmroy@gmail.com"}
 ]
 classifiers = [
     "Topic :: Software Development",
     "License :: OSI Approved :: BSD License",
@@ -67,9 +67,9 @@
 [tool.coverage.xml]
 output = "build/coverage.xml"
 
 [tool.flake8]
 application-import-names = "ssm_ps_template"
 count = true
 exclude = ["bak", "build", "docs", "env"]
-import-order-style = "google"
+import-order-style = "pycharm"
 ignore = ["RST306"]
```

### Comparing `ssm-ps-template-1.0.0b3/ssm_ps_template/__main__.py` & `ssm-ps-template-1.0.0b4/ssm_ps_template/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import argparse
-from importlib import metadata
 import logging
+import os
 import sys
 import time
 import typing
+from importlib import metadata
 
 from botocore import exceptions
 
 from ssm_ps_template import config, discover, render, ssm
 
 LOGGER = logging.getLogger(__name__)
 
 
 def parse_cli_arguments() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         description='Templating for SSM Parameter Store')
     parser.add_argument('--aws-profile', action='store', help='AWS Profile')
     parser.add_argument('--aws-region', action='store', help='AWS Region')
-    parser.add_argument('--prefix', action='store_true',
-                        help='Default SSM Key Prefix')
+    parser.add_argument('--prefix', action='store',
+                        help='Default SSM Key Prefix',
+                        default=os.environ.get('PARAMS_PREFIX'))
     parser.add_argument('--verbose', action='store_true')
     parser.add_argument('config', type=config.configuration_file, nargs=1)
     return parser.parse_args()
 
 
 def render_templates(args: argparse.Namespace) -> typing.NoReturn:
     parameter_store = ssm.ParameterStore(
```

### Comparing `ssm-ps-template-1.0.0b3/ssm_ps_template/config.py` & `ssm-ps-template-1.0.0b4/ssm_ps_template/config.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-1.0.0b3/ssm_ps_template/discover.py` & `ssm-ps-template-1.0.0b4/ssm_ps_template/discover.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-1.0.0b3/ssm_ps_template/render.py` & `ssm-ps-template-1.0.0b4/ssm_ps_template/render.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import io
 import logging
 import os
 import pathlib
 import typing
 from urllib import parse
 
-from jinja2 import sandbox
 import yaml
+from jinja2 import sandbox
 
 LOGGER = logging.getLogger(__name__)
 
 
 class Renderer:
 
     def __init__(self, source: pathlib.Path, variables: typing.List[str]):
```

### Comparing `ssm-ps-template-1.0.0b3/ssm_ps_template/ssm.py` & `ssm-ps-template-1.0.0b4/ssm_ps_template/ssm.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-1.0.0b3/ssm_ps_template.egg-info/PKG-INFO` & `ssm-ps-template-1.0.0b4/ssm_ps_template.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-ps-template
-Version: 1.0.0b3
+Version: 1.0.0b4
 Summary: CLI for rendering configuration templates with SSM Parameter Store as a data source
 Author-email: "Gavin M. Roy" <gavinmroy@gmail.com>
 License: Copyright (c) 2023 Gavin M. Roy
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -149,22 +149,24 @@
 settings: {% set values = settings/ %}
 {{ values | toyaml | indent(2, first=True) }}
 ```
 
 ## Command Line Usage
 
 ```
-usage: ssm-ps-template [-h] [--aws-profile AWS_PROFILE] [--aws-region AWS_REGION] [--prefix] [--verbose] config
+usage: ssm-ps-template [-h] [--aws-profile AWS_PROFILE] [--aws-region AWS_REGION] [--prefix PREFIX] [--verbose] config
+
 Templating for SSM Parameter Store
 
 positional arguments:
   config
 
 optional arguments:
   -h, --help            show this help message and exit
   --aws-profile AWS_PROFILE
                         AWS Profile
   --aws-region AWS_REGION
                         AWS Region
-  --prefix              Default SSM Key Prefix
+  --prefix PREFIX       Default SSM Key Prefix
   --verbose
 ```
+Note that the default SSM prefix can also be set with the `PARAMS_PREFIX` environment variable.
```

### Comparing `ssm-ps-template-1.0.0b3/tests/test_config.py` & `ssm-ps-template-1.0.0b4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-1.0.0b3/tests/test_render.py` & `ssm-ps-template-1.0.0b4/tests/test_render.py`

 * *Files identical despite different names*

