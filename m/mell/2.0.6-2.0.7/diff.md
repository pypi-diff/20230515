# Comparing `tmp/mell-2.0.6.tar.gz` & `tmp/mell-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mell-2.0.6.tar", last modified: Tue May  2 13:40:44 2023, max compression
+gzip compressed data, was "mell-2.0.7.tar", last modified: Sun May 14 23:12:26 2023, max compression
```

## Comparing `mell-2.0.6.tar` & `mell-2.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-02 13:40:44.027508 mell-2.0.6/
--rw-rw-r--   0 diego     (1000) diego     (1000)     9172 2023-05-02 13:40:44.027508 mell-2.0.6/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)     8743 2023-05-02 13:39:44.000000 mell-2.0.6/README.md
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-02 13:40:44.023508 mell-2.0.6/mell/
--rw-rw-r--   0 diego     (1000) diego     (1000)       14 2023-04-26 20:43:44.000000 mell-2.0.6/mell/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      215 2023-05-02 13:40:41.000000 mell-2.0.6/mell/consts.py
--rwxrwxr-x   0 diego     (1000) diego     (1000)    25557 2023-04-27 15:32:46.000000 mell-2.0.6/mell/main.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-02 13:40:44.023508 mell-2.0.6/mell.egg-info/
--rw-rw-r--   0 diego     (1000) diego     (1000)     9172 2023-05-02 13:40:43.000000 mell-2.0.6/mell.egg-info/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)      316 2023-05-02 13:40:44.000000 mell-2.0.6/mell.egg-info/SOURCES.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        1 2023-05-02 13:40:43.000000 mell-2.0.6/mell.egg-info/dependency_links.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       40 2023-05-02 13:40:43.000000 mell-2.0.6/mell.egg-info/entry_points.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       15 2023-05-02 13:40:43.000000 mell-2.0.6/mell.egg-info/requires.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        5 2023-05-02 13:40:43.000000 mell-2.0.6/mell.egg-info/top_level.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       38 2023-05-02 13:40:44.027508 mell-2.0.6/setup.cfg
--rw-rw-r--   0 diego     (1000) diego     (1000)      834 2023-04-26 21:18:03.000000 mell-2.0.6/setup.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-02 13:40:44.027508 mell-2.0.6/tests/
--rw-rw-r--   0 diego     (1000) diego     (1000)     1156 2023-04-29 14:53:17.000000 mell-2.0.6/tests/test_logic.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     2103 2023-04-29 14:55:06.000000 mell-2.0.6/tests/test_metadata.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     1785 2023-04-29 14:55:27.000000 mell-2.0.6/tests/test_news.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     1959 2023-04-29 14:28:44.000000 mell-2.0.6/tests/test_plugin.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-14 23:12:26.193937 mell-2.0.7/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     6800 2023-05-14 23:12:26.193937 mell-2.0.7/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)     6371 2023-05-14 22:36:20.000000 mell-2.0.7/README.md
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-14 23:12:26.189937 mell-2.0.7/mell/
+-rw-rw-r--   0 diego     (1000) diego     (1000)       14 2023-04-26 20:43:44.000000 mell-2.0.7/mell/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      215 2023-05-14 22:53:36.000000 mell-2.0.7/mell/consts.py
+-rwxrwxr-x   0 diego     (1000) diego     (1000)    26486 2023-05-14 22:33:45.000000 mell-2.0.7/mell/main.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-14 23:12:26.189937 mell-2.0.7/mell.egg-info/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     6800 2023-05-14 23:12:26.000000 mell-2.0.7/mell.egg-info/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)      325 2023-05-14 23:12:26.000000 mell-2.0.7/mell.egg-info/SOURCES.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        1 2023-05-14 23:12:26.000000 mell-2.0.7/mell.egg-info/dependency_links.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       40 2023-05-14 23:12:26.000000 mell-2.0.7/mell.egg-info/entry_points.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       15 2023-05-14 23:12:26.000000 mell-2.0.7/mell.egg-info/requires.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        5 2023-05-14 23:12:26.000000 mell-2.0.7/mell.egg-info/top_level.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       38 2023-05-14 23:12:26.193937 mell-2.0.7/setup.cfg
+-rw-rw-r--   0 diego     (1000) diego     (1000)      834 2023-04-26 21:18:03.000000 mell-2.0.7/setup.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2023-05-14 23:12:26.189937 mell-2.0.7/tests/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1964 2023-05-14 21:50:51.000000 mell-2.0.7/tests/test_generators.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2103 2023-04-29 14:55:06.000000 mell-2.0.7/tests/test_metadata.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1180 2023-05-14 22:29:12.000000 mell-2.0.7/tests/test_migrations.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1832 2023-05-14 21:53:05.000000 mell-2.0.7/tests/test_news.py
```

### Comparing `mell-2.0.6/mell/main.py` & `mell-2.0.7/mell/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import json
 import glob
 import time
 import sys
 import os
 import re
 
+
 LOG_LEVEL = 2
 
 def debug(*args):
     if LOG_LEVEL <= 0:
         print("DEBUG:", *args)
 
 def info(*args):
@@ -39,15 +40,15 @@
 def run_new_root(args):
 
     info("Creating a new root structure at", args.new_root)
 
     if os.path.exists(args.new_root):
         error(f"Can't create a root structure, a folder with this name already exists: {args.new_root}")
         
-    for foldernames in [("style", "asset"), ("style", "template"), ("style", "plugin"), ("style", "static"), ("style", "logic"), ("meta",), ("generate",)]:
+    for foldernames in [("style", "assets"), ("style", "templates"), ("style", "generators"), ("style", "statics"), ("style", "migrations"), ("meta",), ("output",)]:
         path = os.path.join(args.new_root, *foldernames)
         info(f"  {path}")
         os.makedirs(path)
     
     sys.exit(0)
 
 def run_new_style(args):
@@ -55,54 +56,54 @@
     folderpath = os.path.join(args.root, args.new_style)
 
     info("Creating a new style structure at", folderpath)
     
     if os.path.exists(folderpath):
         error(f"Can't create a style structure, a folder with this name already exists: {folderpath}")
         
-    for foldernames in ["asset", "template", "plugin", "static", "logic"]:
+    for foldernames in ["assets", "templates", "generators", "statics", "migrations"]:
         path = os.path.join(folderpath, foldernames)
         info(f"  {path}")
         os.makedirs(path)
     
     sys.exit(0)
 
-def run_new_plugin(args):
+def run_new_generator(args):
 
-    filepath = os.path.join(args.plugin, f"{args.new_plugin}.py")
-    info("Creating a new plugin script")
+    filepath = os.path.join(args.generators, f"{args.new_generator}.py")
+    info("Creating a new generator script")
     
     if os.path.exists(filepath):
-        error("Can't create the plugin. A plugin with this name already exists at", filepath)
+        error("Can't create the generator. A file with this name already exists at", filepath)
     
     info(f"  {filepath}")
     dirname = os.path.dirname(filepath)
     os.makedirs(dirname, exist_ok=True)
 
     with open(filepath, 'w') as fout:
-        fout.write("def plugin(args, meta, inflator):\n    pass\n\n")
+        fout.write("def generate(args, meta, inflator):\n    pass\n\n")
     
     sys.exit(0)
 
-def run_new_logic(args):
+def run_new_migration(args):
 
-    info("Creating a new logic script")
+    info("Creating a new migration script")
     
     timestamp = int(time.time())
-    filepath = os.path.join(args.logic, f"{timestamp}.{args.new_logic}.py")
+    filepath = os.path.join(args.migrations, f"{timestamp}.{args.new_migration}.py")
 
     if os.path.exists(filepath):
-        error("Can't create the plugin. A plugin with this name already exists at", filepath)
+        error("Can't create migration. A file with this name already exists at", filepath)
     
     info(f"  {filepath}")
     dirname = os.path.dirname(filepath)
     os.makedirs(dirname, exist_ok=True)
 
     with open(filepath, 'w') as fout:
-        fout.write("def logic(args, meta):\n    pass\n\n")
+        fout.write("def migrate(args, meta):\n    pass\n\n")
     
     sys.exit(0)
 
 def parse_args():
 
     parser = argparse.ArgumentParser(
                         prog='mell',
@@ -126,26 +127,26 @@
                         default=None,
                         dest='quiet',
                         help="display only warning messages and above",
                         action='store_true')
 
     parser.add_argument('--set',
                         default=[],
-                        nargs=2,
+                        nargs='*',
                         dest='set',
-                        help="customize the value of individual properties in the metadata",
+                        help="customize the value of individual properties in the metadata (before migrations)",
                         action='append')
 
     parser.add_argument('--do',
                         type=str,
                         metavar='NAME',
                         default=None,
-                        choices=['nothing', 'clean', 'static', 'template', 'plugin'],
+                        choices=['nothing', 'statics', 'templates', 'generators'],
                         dest='do',
-                        help="define one or more action to be executed [nothing, clean, static, template, plugin]",
+                        help="define one or more action to be executed [nothing, statics, templates, generators]",
                         action='append')
 
     parser.add_argument('--root',
                         type=str,
                         metavar='PATH',
                         default=None,
                         dest='root',
@@ -153,77 +154,77 @@
                         action='store')
     
     parser.add_argument('--style',
                         type=str,
                         metavar='PATH',
                         default=None,
                         dest='style',
-                        help="style folder that contains asset, template, plugin, and static [<root>/style]",
+                        help="style folder containing assets, templates, generators, migrations, and statics [<root>/style]",
                         action='store')
 
-    parser.add_argument('--template',
+    parser.add_argument('--templates',
                         type=str,
                         metavar='PATH',
                         default=None,
-                        dest='template',
+                        dest='templates',
                         help="folder to read the template files [<style>/template]",
                         action='store')
 
-    parser.add_argument('--static',
+    parser.add_argument('--statics',
                         type=str,
                         metavar='PATH',
                         default=None,
-                        dest='static',
+                        dest='statics',
                         help="folder to read the static files [<style>/static]",
                         action='store')
 
-    parser.add_argument('--plugin',
+    parser.add_argument('--generators',
                         type=str,
                         metavar='PATH',
                         default=None,
-                        dest='plugin',
-                        help="folder to read the plugins [<style>/plugin]",
+                        dest='generators',
+                        help="folder to read the generators [<style>/generators]",
                         action='store')
 
-    parser.add_argument('--asset',
+    parser.add_argument('--assets',
                         type=str,
                         metavar='PATH',
                         default=None,
-                        dest='asset',
-                        help="folder holding the asset files [<style>/asset]",
+                        dest='assets',
+                        help="folder holding the asset files [<style>/assets]",
                         action='store')
 
-    parser.add_argument('--logic',
+    parser.add_argument('--migrations',
                         type=str,
                         metavar='PATH',
                         default=None,
-                        dest='logic',
-                        help="folder holding the logic files [<style>/logic]",
+                        dest='migrations',
+                        help="folder holding the migration files [<style>/migrations]",
                         action='store')
 
     parser.add_argument('--meta',
                         type=str,
                         metavar='PATH',
                         default=None,
                         dest='meta',
                         help="folder to read the metadata files [<root>/meta]",
                         action='store')
 
-    parser.add_argument('--generate',
+    parser.add_argument('--output',
                         type=str,
                         metavar='PATH',
                         default=None,
                         dest=None,
-                        help="folder to generate the output files [<root>/generate]",
+                        help="folder to generate the output files [<root>/output]",
                         action='store')
 
     parser.add_argument('-M', '--show-metadata',
                         default=False,
                         dest='show_metadata',
-                        help="display the metadata, after execution of the logic scripts",
+                        help="display the metadata, after executing the migration scripts",
                         action='store_true')
 
     parser.add_argument('-P', '--show-parameter',
                         default=False,
                         dest='show_parameters',
                         help="display all command line parameters and their values, received or not",
                         action='store_true')
@@ -240,30 +241,35 @@
                         type=str,
                         metavar='NAME',
                         default=None,
                         dest="new_style",
                         help="create a new style folder using the recommended structure",
                         action='store')
     
-    parser.add_argument('--new-plugin',
+    parser.add_argument('--new-generator',
                         type=str,
                         metavar='NAME',
                         default=None,
-                        dest="new_plugin",
-                        help="create a new plugin script using the name provided",
+                        dest="new_generator",
+                        help="create a new generator script using the name provided",
                         action='store')
     
-    parser.add_argument('--new-logic',
+    parser.add_argument('--new-migration',
                         type=str,
                         metavar='NAME',
                         default=None,
-                        dest="new_logic",
-                        help="create a new logic script using the name provided",
+                        dest="new_migration",
+                        help="create a new migration script using the name provided",
                         action='store')
     
+    parser.add_argument('--clean',
+                        dest="clean",
+                        help="clean the output folder before generating the files",
+                        action='store_true')
+    
     parser.add_argument('--version',
                         action='version', 
                         version=f'{consts.name} {consts.version}')
     
     parser.add_argument('--block_start',
                         type=str,
                         metavar='STR',
@@ -313,40 +319,40 @@
                         action='store')
 
     args = parser.parse_args()
 
     if args.root is None:
         args.root = '.'
 
-    if args.generate is None:
-        args.generate = os.path.join(args.root, 'generate')
+    if args.output is None:
+        args.output = os.path.join(args.root, 'output')
 
     if args.meta is None:
         args.meta = os.path.join(args.root, 'meta')
 
     if args.style is None:
         args.style = os.path.join(args.root, 'style')
 
-    if args.static is None:
-        args.static = os.path.join(args.style, 'static')
+    if args.statics is None:
+        args.statics = os.path.join(args.style, 'statics')
 
-    if args.template is None:
-        args.template = os.path.join(args.style, 'template')
+    if args.templates is None:
+        args.templates = os.path.join(args.style, 'templates')
 
-    if args.plugin is None:
-        args.plugin = os.path.join(args.style, 'plugin')
+    if args.generators is None:
+        args.generators = os.path.join(args.style, 'generators')
 
-    if args.asset is None:
-        args.asset = os.path.join(args.style, 'asset')
+    if args.assets is None:
+        args.assets = os.path.join(args.style, 'assets')
 
-    if args.logic is None:
-        args.logic = os.path.join(args.style, 'logic')
+    if args.migrations is None:
+        args.migrations = os.path.join(args.style, 'migrations')
 
     if args.do is None:
-        args.do = ['clean', 'static', 'template', 'plugin']
+        args.do = ['statics', 'templates', 'generators']
 
     global LOG_LEVEL
     
     if args.quiet and args.verbose:
         error("You can't use quiet (-q) and verbose (-v) modes at the same time")
 
     elif args.quiet:
@@ -357,19 +363,19 @@
 
     if args.new_root:
         run_new_root(args)
     
     if args.new_style:
         run_new_style(args)
 
-    if args.new_plugin:
-        run_new_plugin(args)
+    if args.new_generator:
+        run_new_generator(args)
 
-    if args.new_logic:
-        run_new_logic(args)
+    if args.new_migration:
+        run_new_migration(args)
 
     if args.metadata is None:
         parser.print_help()
         sys.exit(0)
     
     return args
 
@@ -429,15 +435,14 @@
         else:
             return Meta(value)
 
 
 class Meta:
 
     def __init__(self, value):
-
         self.__dict__['value'] = value
     
     def __iter__(self):
 
         v = self.value
         if v is None:
             raise IndexError("Trying to iterate over a metadata that does not exist.")
@@ -466,15 +471,16 @@
 
     def __getattr__(self, index):
 
         v = self.value
         if v is None:
             return Meta(None)
         elif index in v:
-            return Meta(v[index])
+            child_value = v[index]
+            return Meta(child_value) if isinstance(child_value, (list, dict)) else child_value
         else:
             return Meta(None)
     
     def __getitem__(self, index):
         
         v = self.value
         if v is None:
@@ -514,16 +520,16 @@
         return str(v)
 
 
 class Inflater:
 
     def __init__(self, args):
         self.args = args
-        self.template_env = self._create_env(args.template)
-        self.asset_env = self._create_env(args.asset)
+        self.template_env = self._create_env(args.templates)
+        self.asset_env = self._create_env(args.assets)
     
     def _create_env(self, folderpath):
         if not os.path.exists(folderpath):
             return None
 
         return Environment(
             block_start_string=self.args.block_start,
@@ -553,125 +559,142 @@
                 raise IOError("Missing template folder")
             template = self.template_env.get_template(relpath)
         
         text = template.render(args=self.args, meta=meta, inflater=self)
 
         if to_file is not None:
 
-            filepath_out = os.path.join(self.args.generate, to_file)
+            filepath_out = os.path.join(self.args.output, to_file)
             folderpath_out = os.path.dirname(filepath_out)
             
             os.makedirs(folderpath_out, exist_ok=True)
             
             with open(filepath_out, "w") as fout:
                 fout.write(text)
 
         return text
         
-def do_nothing(args, inflater, meta):
+def do_action_nothing(args, inflater, meta):
     pass
 
-def do_clean(args, inflater, meta):
+def do_clean(args):
 
-    info("Cleaning generate directory")
+    if not args.clean:
+        return
 
-    if os.path.exists(args.generate):
-        if os.path.isdir(args.generate):
-            for filepath in glob.glob(os.path.join(args.generate, '*')):
+    info("Cleaning output directory")
+
+    if os.path.exists(args.output):
+        if os.path.isdir(args.output):
+            for filepath in glob.glob(os.path.join(args.output, '*')):
                 debug("  Removing:", filepath)
                 if os.path.isdir(filepath):
                     shutil.rmtree(filepath)
                 else:
                     os.remove(filepath)
         else:
-            os.remove(args.generate)
+            os.remove(args.output)
     
-def do_static(args, inflater, meta):
+def do_action_statics(args, inflater, meta):
 
     info("Copying static data")
 
-    for filepath in glob.glob(os.path.join(args.static, '**'), recursive=True):
+    for filepath in glob.glob(os.path.join(args.statics, '**'), recursive=True):
         if os.path.isfile(filepath):
-            relpath = os.path.relpath(filepath, args.static)
-            filepath_out = os.path.join(args.generate, relpath)
+            relpath = os.path.relpath(filepath, args.statics)
+            filepath_out = os.path.join(args.output, relpath)
             debug(f"{filepath} -> {filepath_out}")
 
             folderpath_out = os.path.dirname(filepath_out)
             os.makedirs(folderpath_out, exist_ok=True)
             shutil.copy2(filepath, filepath_out)
 
-def do_template(args, inflater:Inflater, meta:Meta):
+def do_action_templates(args, inflater:Inflater, meta:Meta):
 
     info("Generating template based files")
 
-    for filepath in glob.glob(os.path.join(args.template, "**"), recursive=True):
+    for filepath in glob.glob(os.path.join(args.templates, "**"), recursive=True):
         if os.path.isfile(filepath):
-            relpath = os.path.relpath(filepath, args.template)
+            relpath = os.path.relpath(filepath, args.templates)
             debug("  ", relpath)
 
             inflater.inflate(relpath, meta, to_file=relpath, from_asset=False)
 
 
-def do_plugin(args, inflater, meta):
+def do_action_generators(args, inflater, meta):
     
-    info("Executing plugin files")
+    info("Executing generator files")
 
-    rootpath = os.path.dirname(args.plugin)
+    rootpath = os.path.dirname(args.generators)
 
-    for filepath in glob.glob(os.path.join(args.plugin, '**', '*.py'), recursive=True):
+    for filepath in glob.glob(os.path.join(args.generators, '*.py'), recursive=True):
         if os.path.isfile(filepath):
-            plugin_name = os.path.relpath(filepath, rootpath).replace('\\', '.').replace('/', '.')
+            generator_name = os.path.relpath(filepath, rootpath).replace('\\', '.').replace('/', '.')
             debug("  ", filepath)
             
-            plugin_spec = importlib.util.spec_from_file_location(plugin_name, filepath)
-            plugin = importlib.util.module_from_spec(plugin_spec)
-            plugin_spec.loader.exec_module(plugin)
-            plugin.plugin(args, meta, inflater)
+            generator_spec = importlib.util.spec_from_file_location(generator_name, filepath)
+            generator = importlib.util.module_from_spec(generator_spec)
+            generator_spec.loader.exec_module(generator)
+            generator.generate(args, meta, inflater)
 
-def get_logic_files(args):
+def get_sorted_script_files(folderpath):
 
     filepaths = []
 
-    for filepath in glob.glob(os.path.join(args.logic, '**', '*.py'), recursive=True):
+    for filepath in glob.glob(os.path.join(folderpath, '*.py'), recursive=True):
         if os.path.isfile(filepath):
             filename = os.path.basename(filepath)
             cells = filename.split('.', 1)
             if len(cells) == 2:
                 try:
                     timestamp = int(cells[0])
                     filepaths.append((timestamp, filepath))
                 except ValueError:
                     pass
     
     filepaths.sort()
     return filepaths
 
-def do_logic_scripts(args, meta):
+def do_migrations(args, meta):
     
-    info("Executing logic files")
+    info("Executing migration files")
     
-    rootpath = os.path.dirname(args.logic)
-    filepaths = get_logic_files(args)
+    rootpath = os.path.dirname(args.migrations)
+    filepaths = get_sorted_script_files(args.migrations)
     
     for _, filepath in filepaths:
-        logic_name = os.path.relpath(filepath, rootpath).replace('\\', '.').replace('/', '.')
-        debug("  ", filepath)
+        migration_name = os.path.relpath(filepath, rootpath).replace('\\', '.').replace('/', '.')
+        debug("  Applying migration ", filepath)
         
-        plugin_spec = importlib.util.spec_from_file_location(logic_name, filepath)
-        plugin = importlib.util.module_from_spec(plugin_spec)
-        plugin_spec.loader.exec_module(plugin)
-        plugin.logic(args, meta)
+        migration_spec = importlib.util.spec_from_file_location(migration_name, filepath)
+        migration = importlib.util.module_from_spec(migration_spec)
+        migration_spec.loader.exec_module(migration)
+        migration.migrate(args, meta)
 
 def do_set_values(args, meta):
 
     info("Applying set")
     
     r = re.compile('\[(\d+)\]')
 
-    for address, value in args.set:
+    value_types = {
+        'str':str, 
+        'int': int, 
+        'float': float, 
+        'bytes':bytes, 
+        'bool':bool
+    }
+
+    for set in args.set:
+
+        value_type = str if len(set) < 3 else value_types[set[2]]
+
+        address = set[0]
+        value = value_type(set[1])
+
         property_names = address.split('.')
         property_names = [re.split(r, x) for x in property_names]
         property_names = [x if i % 2 == 0 else int(x) for y in property_names for i,x in enumerate(y) if x]
 
         current = meta.value
 
         try:
@@ -740,15 +763,15 @@
 
     if args.show_parameters:
         print("Parameters:")
         print(json.dumps(args.__dict__, indent=2))
 
 def do_action(name, args, inflater, meta):
 
-    globals()['do_' + name](args, inflater, meta)
+    globals()['do_action_' + name](args, inflater, meta)
 
 def do_load_meta(args):
     if os.path.exists(args.meta):
         return Meta(load_metadata(args, args.metadata))
 
     if args.metadata:
         error(f"Folder meta does not exist - {args.meta}")
@@ -762,23 +785,24 @@
     
     args = parse_args()
 
     info("Loading the metadata")
     meta = do_load_meta(args)
     
     do_set_values(args, meta)
-    do_logic_scripts(args, meta)
+    do_migrations(args, meta)
 
     do_show_metadata(args, meta)
     do_show_parameters(args)
 
     info("Loading the inflater")
     inflater = do_load_inflater(args)
 
     info("Executing actions")
+    do_clean(args)
     for name in args.do:
         do_action(name, args, inflater, meta)
 
     info("Bye!")
 
 
 if __name__ == "__main__":
```

### Comparing `mell-2.0.6/setup.py` & `mell-2.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `mell-2.0.6/tests/test_logic.py` & `mell-2.0.7/tests/test_migrations.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 from utils import MellHelper, unindent
 
 
-def test_logic():
+def test_migrations():
 
     expected_output = unindent(8, """
         Metadata:
         {
           "users": [
             {
               "name": "Diego",
@@ -16,19 +16,19 @@
               "name": "Quelle",
               "email": "quelle@company.com"
             }
           ]
         }
         """)
 
-    logic_name = 'add_email'
-    logic_program = unindent(8, """
-        def logic(args, meta):
+    migration_name = 'add_email'
+    migration_script = unindent(8, """
+        def migrate(args, meta):
             for user in meta.users:
-                user.email = user.name.value.lower() + "@company.com"
+                user.email = user.name.lower() + "@company.com"
         """)
 
     meta_name = 'users'
     meta_data = unindent(8, """
         {
           "users": [
             {
@@ -37,17 +37,17 @@
             {
               "name":"Quelle"
             }
           ]
         }
         """)
 
-    p = MellHelper('logic')
+    p = MellHelper('migrations')
     p.create_project()
     p.create_metadata(meta_name, meta_data)
-    p.create_logic(logic_name, logic_program)
+    p.create_migration(migration_name, migration_script)
 
     status, stdout, stderr = p.exec(f'--root {p.root_path} --show-metadata users')
 
     assert status == 0
     assert stderr == ''
     assert stdout == expected_output
```

### Comparing `mell-2.0.6/tests/test_metadata.py` & `mell-2.0.7/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `mell-2.0.6/tests/test_news.py` & `mell-2.0.7/tests/test_news.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,61 +11,61 @@
     
     assert returncode == 0
 
     assert file_count(p.root_path    ) == 3
 
     assert file_count(p.style_path   ) == 5
     assert file_count(p.meta_path    ) == 0
-    assert file_count(p.generate_path) == 0
+    assert file_count(p.output_path) == 0
 
-    assert file_count(p.template_path) == 0
-    assert file_count(p.asset_path   ) == 0
-    assert file_count(p.logic_path   ) == 0
-    assert file_count(p.plugin_path  ) == 0
-    assert file_count(p.static_path  ) == 0
+    assert file_count(p.templates_path) == 0
+    assert file_count(p.assets_path   ) == 0
+    assert file_count(p.migrations_path   ) == 0
+    assert file_count(p.generators_path  ) == 0
+    assert file_count(p.statics_path  ) == 0
 
-def test_new_plugin():
+def test_new_generator():
 
-    p = MellHelper("new_plugin")
-    name = 'new_plugin'
+    p = MellHelper("new_generator")
+    name = 'new_generator'
 
     p.delete()
     
     assert p.exec(f'--new {p.root_path}')[0] == 0
-    assert p.exec(f'--style {p.style_path} --new-plugin {name}')[0] == 0
-    assert file_count(p.plugin_path) == 1
+    assert p.exec(f'--style {p.style_path} --new-generator {name}')[0] == 0
+    assert file_count(p.generators_path) == 1
 
-def test_new_logic():
+def test_new_migration():
     
-    p = MellHelper("new_logic")
-    name = 'new_logic'
+    p = MellHelper("new_migration")
+    name = 'new_migration'
 
     p.delete()
     
     assert p.exec(f'--new {p.root_path}')[0] == 0
-    assert p.exec(f'--style {p.style_path} --new-logic {name}')[0] == 0
-    assert file_count(p.logic_path) == 1
+    assert p.exec(f'--style {p.style_path} --new-migration {name}')[0] == 0
+    assert file_count(p.migrations_path) == 1
 
 def test_new_style():
 
     p = MellHelper("new_style")
     name = 'new_style2'
 
     p.delete()
     
     assert p.exec(f'--new {p.root_path}')[0] == 0
     assert p.exec(f'--root {p.root_path} --new-style {name}')[0] == 0
 
     p.set_style(name)
     
-    assert file_count(p.root_path    ) == 4
+    assert file_count(p.root_path) == 4
 
-    assert file_count(p.style_path   ) == 5
-    assert file_count(p.meta_path    ) == 0
-    assert file_count(p.generate_path) == 0
-
-    assert file_count(p.template_path) == 0
-    assert file_count(p.asset_path   ) == 0
-    assert file_count(p.logic_path   ) == 0
-    assert file_count(p.plugin_path  ) == 0
-    assert file_count(p.static_path  ) == 0
+    assert file_count(p.style_path ) == 5
+    assert file_count(p.meta_path  ) == 0
+    assert file_count(p.output_path) == 0
+
+    assert file_count(p.templates_path ) == 0
+    assert file_count(p.assets_path    ) == 0
+    assert file_count(p.migrations_path) == 0
+    assert file_count(p.generators_path) == 0
+    assert file_count(p.statics_path   ) == 0
```

### Comparing `mell-2.0.6/tests/test_plugin.py` & `mell-2.0.7/tests/test_generators.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from utils import MellHelper, unindent
 
-def test_plugin():
+
+def test_generators():
 
     metaname = 'data'
 
     metadata = unindent(8, """
         {
             "projects":[
                 {
@@ -26,16 +27,16 @@
         }
         """)
     
     asset_template = unindent(8, """
         Project '|= meta.name =|' will last |= meta.duration_in_months =| month(s) and cost USD |= meta.cost_in_usd =|.
         """)
     
-    plugin_program = unindent(8, """
-        def plugin(args, meta, inflater):
+    generator_script = unindent(8, """
+        def generate(args, meta, inflater):
             for i, project in enumerate(meta.projects):
                 inflater.inflate('project.txt', project, to_file=f'project_{i}.txt')
         """)
 
     project_0 = unindent(8, """
         Project 'Thoculi' will last 3 month(s) and cost USD 1000000.00.""")
 
@@ -44,18 +45,18 @@
 
     project_2 = unindent(8, """
         Project 'Gold' will last 2 month(s) and cost USD 2000000.00.""")
 
     p = MellHelper("plugin")
     p.create_project()
     p.create_metadata(metaname, metadata)
-    p.create_plugin('projects', plugin_program)
+    p.create_generator('projects', generator_script)
     p.create_asset('project.txt', asset_template)
     status, stdout, stderr = p.exec(f'--root {p.root_path} {metaname}')
 
     assert status == 0
     assert stderr == ''
     assert stdout == ''
 
-    assert p.read_generated_file('project_0.txt') == project_0
-    assert p.read_generated_file('project_1.txt') == project_1
-    assert p.read_generated_file('project_2.txt') == project_2
+    assert p.read_output_file('project_0.txt') == project_0
+    assert p.read_output_file('project_1.txt') == project_1
+    assert p.read_output_file('project_2.txt') == project_2
```

