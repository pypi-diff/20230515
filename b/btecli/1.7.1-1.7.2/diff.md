# Comparing `tmp/btecli-1.7.1.tar.gz` & `tmp/btecli-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btecli-1.7.1.tar", last modified: Fri May 12 20:58:43 2023, max compression
+gzip compressed data, was "btecli-1.7.2.tar", last modified: Mon May 15 00:17:25 2023, max compression
```

## Comparing `btecli-1.7.1.tar` & `btecli-1.7.2.tar`

### file list

```diff
@@ -1,56 +1,58 @@
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:58:43.069913 btecli-1.7.1/
--rw-r--r--   0 etejeda    (501) staff       (20)     1312 2023-05-10 18:51:52.000000 btecli-1.7.1/.gitignore
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.1/HISTORY.md
--rw-r--r--   0 etejeda    (501) staff       (20)    35149 2023-05-10 17:31:13.000000 btecli-1.7.1/LICENSE
--rw-r--r--   0 etejeda    (501) staff       (20)       72 2023-05-12 20:58:43.069570 btecli-1.7.1/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)     7703 2023-05-11 11:59:50.000000 btecli-1.7.1/README.md
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:58:43.057683 btecli-1.7.1/btecli/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.1/btecli/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)    10909 2023-05-12 20:58:36.000000 btecli-1.7.1/btecli/cli.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:58:43.059918 btecli-1.7.1/btecli/lib/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.1/btecli/lib/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:58:43.060887 btecli-1.7.1/btecli/lib/cryptography/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.1/btecli/lib/cryptography/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     4586 2023-05-10 17:31:13.000000 btecli-1.7.1/btecli/lib/cryptography/aes.py
--rw-r--r--   0 etejeda    (501) staff       (20)     1837 2023-05-10 17:31:13.000000 btecli-1.7.1/btecli/lib/cryptography/wincred.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:58:43.061346 btecli-1.7.1/btecli/lib/defaults/
--rw-r--r--   0 etejeda    (501) staff       (20)      413 2023-05-10 17:31:13.000000 btecli-1.7.1/btecli/lib/defaults/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:58:43.061832 btecli-1.7.1/btecli/lib/dictutils/
--rw-r--r--   0 etejeda    (501) staff       (20)      424 2023-05-11 01:14:27.000000 btecli-1.7.1/btecli/lib/dictutils/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:58:43.062399 btecli-1.7.1/btecli/lib/formatting/
--rw-r--r--   0 etejeda    (501) staff       (20)      651 2023-05-10 17:31:13.000000 btecli-1.7.1/btecli/lib/formatting/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:58:43.063063 btecli-1.7.1/btecli/lib/input/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.1/btecli/lib/input/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)      272 2023-05-10 17:31:13.000000 btecli-1.7.1/btecli/lib/input/streams.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:58:43.063467 btecli-1.7.1/btecli/lib/logger/
--rw-r--r--   0 etejeda    (501) staff       (20)      660 2023-05-10 17:31:13.000000 btecli-1.7.1/btecli/lib/logger/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:58:43.064097 btecli-1.7.1/btecli/lib/options/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.1/btecli/lib/options/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     1140 2023-05-10 17:31:13.000000 btecli-1.7.1/btecli/lib/options/mexclusive.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:58:43.065987 btecli-1.7.1/btecli/lib/plugin/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.1/btecli/lib/plugin/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     3251 2023-05-12 18:51:57.000000 btecli-1.7.1/btecli/lib/plugin/finder.py
--rw-r--r--   0 etejeda    (501) staff       (20)     2013 2023-05-12 18:51:56.000000 btecli-1.7.1/btecli/lib/plugin/metadata.py
--rw-r--r--   0 etejeda    (501) staff       (20)     7626 2023-05-12 18:51:58.000000 btecli-1.7.1/btecli/lib/plugin/plugins.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:58:43.066788 btecli-1.7.1/btecli/lib/proc/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.1/btecli/lib/proc/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     5063 2023-05-12 18:51:53.000000 btecli-1.7.1/btecli/lib/proc/local_invocation.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:58:43.068518 btecli-1.7.1/btecli/lib/shell/
--rw-r--r--   0 etejeda    (501) staff       (20)     2455 2023-05-12 18:51:54.000000 btecli-1.7.1/btecli/lib/shell/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)      129 2023-05-10 17:31:13.000000 btecli-1.7.1/btecli/lib/shell/bash_init.py
--rw-r--r--   0 etejeda    (501) staff       (20)      836 2023-05-10 17:31:13.000000 btecli-1.7.1/btecli/lib/shell/which.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:58:43.059563 btecli-1.7.1/btecli.egg-info/
--rw-r--r--   0 etejeda    (501) staff       (20)       72 2023-05-12 20:58:42.000000 btecli-1.7.1/btecli.egg-info/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)      976 2023-05-12 20:58:42.000000 btecli-1.7.1/btecli.egg-info/SOURCES.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-12 20:58:42.000000 btecli-1.7.1/btecli.egg-info/dependency_links.txt
--rw-r--r--   0 etejeda    (501) staff       (20)       40 2023-05-12 20:58:42.000000 btecli-1.7.1/btecli.egg-info/entry_points.txt
--rw-r--r--   0 etejeda    (501) staff       (20)      252 2023-05-12 20:58:42.000000 btecli-1.7.1/btecli.egg-info/requires.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        7 2023-05-12 20:58:42.000000 btecli-1.7.1/btecli.egg-info/top_level.txt
--rw-r--r--   0 etejeda    (501) staff       (20)      259 2023-05-10 17:31:13.000000 btecli-1.7.1/ecli.config.yaml.example
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:58:43.052405 btecli-1.7.1/resources/
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:58:43.069022 btecli-1.7.1/resources/icons/
--rw-r--r--   0 etejeda    (501) staff       (20)     9662 2023-05-10 17:31:13.000000 btecli-1.7.1/resources/icons/admin.ico
--rw-r--r--   0 etejeda    (501) staff       (20)       38 2023-05-12 20:58:43.070016 btecli-1.7.1/setup.cfg
--rw-r--r--   0 etejeda    (501) staff       (20)     2372 2023-05-10 17:31:13.000000 btecli-1.7.1/setup.iss
--rw-r--r--   0 etejeda    (501) staff       (20)     1201 2023-05-12 20:58:31.000000 btecli-1.7.1/setup.py
--rw-r--r--   0 etejeda    (501) staff       (20)      743 2023-05-12 20:58:25.000000 btecli-1.7.1/version.rc
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-15 00:17:25.472223 btecli-1.7.2/
+-rw-r--r--   0 etejeda    (501) staff       (20)     1312 2023-05-10 18:51:52.000000 btecli-1.7.2/.gitignore
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.2/HISTORY.md
+-rw-r--r--   0 etejeda    (501) staff       (20)    35149 2023-05-10 17:31:13.000000 btecli-1.7.2/LICENSE
+-rw-r--r--   0 etejeda    (501) staff       (20)     8647 2023-05-15 00:17:25.472575 btecli-1.7.2/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)     7703 2023-05-11 11:59:50.000000 btecli-1.7.2/README.md
+-rw-r--r--   0 etejeda    (501) staff       (20)        5 2023-05-15 00:14:22.000000 btecli-1.7.2/VERSION.txt
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-15 00:17:25.456904 btecli-1.7.2/btecli/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.2/btecli/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)    11075 2023-05-15 00:12:09.000000 btecli-1.7.2/btecli/cli.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-15 00:17:25.459812 btecli-1.7.2/btecli/lib/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.2/btecli/lib/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-15 00:17:25.461053 btecli-1.7.2/btecli/lib/cryptography/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.2/btecli/lib/cryptography/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     4586 2023-05-10 17:31:13.000000 btecli-1.7.2/btecli/lib/cryptography/aes.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     1837 2023-05-10 17:31:13.000000 btecli-1.7.2/btecli/lib/cryptography/wincred.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-15 00:17:25.461778 btecli-1.7.2/btecli/lib/defaults/
+-rw-r--r--   0 etejeda    (501) staff       (20)      413 2023-05-10 17:31:13.000000 btecli-1.7.2/btecli/lib/defaults/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-15 00:17:25.462301 btecli-1.7.2/btecli/lib/dictutils/
+-rw-r--r--   0 etejeda    (501) staff       (20)      424 2023-05-11 01:14:27.000000 btecli-1.7.2/btecli/lib/dictutils/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-15 00:17:25.462707 btecli-1.7.2/btecli/lib/formatting/
+-rw-r--r--   0 etejeda    (501) staff       (20)      651 2023-05-10 17:31:13.000000 btecli-1.7.2/btecli/lib/formatting/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-15 00:17:25.463953 btecli-1.7.2/btecli/lib/input/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.2/btecli/lib/input/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      272 2023-05-10 17:31:13.000000 btecli-1.7.2/btecli/lib/input/streams.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-15 00:17:25.464581 btecli-1.7.2/btecli/lib/logger/
+-rw-r--r--   0 etejeda    (501) staff       (20)      660 2023-05-10 17:31:13.000000 btecli-1.7.2/btecli/lib/logger/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-15 00:17:25.465759 btecli-1.7.2/btecli/lib/options/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.2/btecli/lib/options/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     1140 2023-05-10 17:31:13.000000 btecli-1.7.2/btecli/lib/options/mexclusive.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-15 00:17:25.468006 btecli-1.7.2/btecli/lib/plugin/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.2/btecli/lib/plugin/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     3251 2023-05-12 18:51:57.000000 btecli-1.7.2/btecli/lib/plugin/finder.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     2013 2023-05-12 18:51:56.000000 btecli-1.7.2/btecli/lib/plugin/metadata.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     7626 2023-05-12 18:51:58.000000 btecli-1.7.2/btecli/lib/plugin/plugins.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-15 00:17:25.469077 btecli-1.7.2/btecli/lib/proc/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.2/btecli/lib/proc/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     5064 2023-05-15 00:01:43.000000 btecli-1.7.2/btecli/lib/proc/local_invocation.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-15 00:17:25.470953 btecli-1.7.2/btecli/lib/shell/
+-rw-r--r--   0 etejeda    (501) staff       (20)     2455 2023-05-12 18:51:54.000000 btecli-1.7.2/btecli/lib/shell/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      129 2023-05-10 17:31:13.000000 btecli-1.7.2/btecli/lib/shell/bash_init.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      836 2023-05-10 17:31:13.000000 btecli-1.7.2/btecli/lib/shell/which.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-15 00:17:25.459431 btecli-1.7.2/btecli.egg-info/
+-rw-r--r--   0 etejeda    (501) staff       (20)     8647 2023-05-15 00:17:25.000000 btecli-1.7.2/btecli.egg-info/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)     1027 2023-05-15 00:17:25.000000 btecli-1.7.2/btecli.egg-info/SOURCES.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-15 00:17:25.000000 btecli-1.7.2/btecli.egg-info/dependency_links.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)       40 2023-05-15 00:17:25.000000 btecli-1.7.2/btecli.egg-info/entry_points.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-15 00:15:16.000000 btecli-1.7.2/btecli.egg-info/not-zip-safe
+-rw-r--r--   0 etejeda    (501) staff       (20)      375 2023-05-15 00:17:25.000000 btecli-1.7.2/btecli.egg-info/requires.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        7 2023-05-15 00:17:25.000000 btecli-1.7.2/btecli.egg-info/top_level.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)      259 2023-05-10 17:31:13.000000 btecli-1.7.2/ecli.config.yaml.example
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-15 00:17:25.451713 btecli-1.7.2/resources/
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-15 00:17:25.471480 btecli-1.7.2/resources/icons/
+-rw-r--r--   0 etejeda    (501) staff       (20)     9662 2023-05-10 17:31:13.000000 btecli-1.7.2/resources/icons/admin.ico
+-rw-r--r--   0 etejeda    (501) staff       (20)     1666 2023-05-15 00:17:25.474036 btecli-1.7.2/setup.cfg
+-rw-r--r--   0 etejeda    (501) staff       (20)     2372 2023-05-10 17:31:13.000000 btecli-1.7.2/setup.iss
+-rw-r--r--   0 etejeda    (501) staff       (20)      810 2023-05-15 00:04:01.000000 btecli-1.7.2/setup.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      743 2023-05-12 21:09:15.000000 btecli-1.7.2/version.rc
```

### Comparing `btecli-1.7.1/.gitignore` & `btecli-1.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `btecli-1.7.1/LICENSE` & `btecli-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `btecli-1.7.1/README.md` & `btecli-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `btecli-1.7.1/btecli/cli.py` & `btecli-1.7.2/btecli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,27 @@
 import click
 from click_plugins import with_plugins
 from btecli.lib.defaults import default_config
 import getpass
 import logging
 import os
 import sys
+import btecli
 from btecli.lib.logger import Logger
 from btecli.lib.options.mexclusive import MutuallyExclusiveOption
 from btecli.lib.plugin import plugins
 from btecli.lib.input.streams import Streams
 from btecli.lib.dictutils import Struct
 from btconfig import Config
+from getversion import get_module_version
 
 # Private variables
 __author__ = 'Bert Tejeda'
-__version__ = '1.7.1'
+__version__ = get_module_version(btecli)[0]
+__program_name__ = 'ecli'
 # Configuration Files
 config_file_name = 'ecli.config.yaml'
 # Initialize App Config
 config = Config(
     config_file_uri=config_file_name,
     default_value=default_config
 ).read()
@@ -37,14 +40,16 @@
 # Initialize Plugins Library
 cli_plugins = plugins.Plugins(application_path, PluginsFromConfig=config.plugins.paths)
 # Initialize Logger with the name 'main' to make sure any child loggers 
 # do not propagate their messages to the default 'root' logger,
 # less you get duplicate output
 logger = Logger().init_logger('main')
 
+logger.debug(f'{__program_name__} version is {__version__}')
+
 @with_plugins(iter_entry_points('ecli.plugins'))
 @click.group()
 @click.version_option(version=__version__)
 @click.option('--config', type=str, nargs=1,
               help='Specify a config file (default is config.yaml)')
 @click.option('---debug', is_flag=True, help='Enable debug output')
 @click.option('--show-plugin-paths','-lp', is_flag=True,
```

### Comparing `btecli-1.7.1/btecli/lib/cryptography/aes.py` & `btecli-1.7.2/btecli/lib/cryptography/aes.py`

 * *Files identical despite different names*

### Comparing `btecli-1.7.1/btecli/lib/cryptography/wincred.py` & `btecli-1.7.2/btecli/lib/cryptography/wincred.py`

 * *Files identical despite different names*

### Comparing `btecli-1.7.1/btecli/lib/formatting/__init__.py` & `btecli-1.7.2/btecli/lib/formatting/__init__.py`

 * *Files identical despite different names*

### Comparing `btecli-1.7.1/btecli/lib/logger/__init__.py` & `btecli-1.7.2/btecli/lib/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `btecli-1.7.1/btecli/lib/options/mexclusive.py` & `btecli-1.7.2/btecli/lib/options/mexclusive.py`

 * *Files identical despite different names*

### Comparing `btecli-1.7.1/btecli/lib/plugin/finder.py` & `btecli-1.7.2/btecli/lib/plugin/finder.py`

 * *Files identical despite different names*

### Comparing `btecli-1.7.1/btecli/lib/plugin/metadata.py` & `btecli-1.7.2/btecli/lib/plugin/metadata.py`

 * *Files identical despite different names*

### Comparing `btecli-1.7.1/btecli/lib/plugin/plugins.py` & `btecli-1.7.2/btecli/lib/plugin/plugins.py`

 * *Files identical despite different names*

### Comparing `btecli-1.7.1/btecli/lib/proc/local_invocation.py` & `btecli-1.7.2/btecli/lib/proc/local_invocation.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         debug_enabled = kwargs.get('debug_enabled', False)
         suppress_output = kwargs.get('suppress_output', False)
         exe = shell_map[ext]['invocation'][cmd_invocation]['executable']
         
         # Adjust shell environment
         curr_env = os.environ.copy()
         env_variables = kwargs['env_variables']
-        modified_env = AttrDict.merge(env_variables,curr_env)
+        modified_env = AttrDict.merge(curr_env, env_variables)
 
         if exe is None:
             self.logger.error("Specified executable is invalid, got '%s'" % exe)
             sys.exit(1)           
         executable = which(exe)
         if not executable:
             self.logger.error('No executable found for %s' % exe)
```

### Comparing `btecli-1.7.1/btecli/lib/shell/__init__.py` & `btecli-1.7.2/btecli/lib/shell/__init__.py`

 * *Files identical despite different names*

### Comparing `btecli-1.7.1/btecli/lib/shell/which.py` & `btecli-1.7.2/btecli/lib/shell/which.py`

 * *Files identical despite different names*

### Comparing `btecli-1.7.1/btecli.egg-info/SOURCES.txt` & `btecli-1.7.2/btecli.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 .gitignore
 HISTORY.md
 LICENSE
 README.md
+VERSION.txt
 ecli.config.yaml.example
+setup.cfg
 setup.iss
 setup.py
 version.rc
 btecli/__init__.py
 btecli/cli.py
 btecli.egg-info/PKG-INFO
 btecli.egg-info/SOURCES.txt
 btecli.egg-info/dependency_links.txt
 btecli.egg-info/entry_points.txt
+btecli.egg-info/not-zip-safe
 btecli.egg-info/requires.txt
 btecli.egg-info/top_level.txt
 btecli/lib/__init__.py
 btecli/lib/cryptography/__init__.py
 btecli/lib/cryptography/aes.py
 btecli/lib/cryptography/wincred.py
 btecli/lib/defaults/__init__.py
```

### Comparing `btecli-1.7.1/resources/icons/admin.ico` & `btecli-1.7.2/resources/icons/admin.ico`

 * *Files identical despite different names*

### Comparing `btecli-1.7.1/setup.iss` & `btecli-1.7.2/setup.iss`

 * *Files identical despite different names*

### Comparing `btecli-1.7.1/version.rc` & `btecli-1.7.2/version.rc`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 VSVersionInfo(
     ffi=FixedFileInfo(
-    filevers=(1, 7, 0, 1),
-    prodvers=(1, 7, 0, 1),
+    filevers=(1, 7, 1, 0),
+    prodvers=(1, 7, 1, 0),
     mask=0x3f,
     flags=0x0,
     OS=0x40004,
     fileType=0x1,
     subtype=0x0,
     date=(0, 0)),
     kids=[StringFileInfo([StringTable(
```

