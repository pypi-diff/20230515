# Comparing `tmp/bpy_addon_build-0.1.0.tar.gz` & `tmp/bpy_addon_build-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpy_addon_build-0.1.0.tar", max compression
+gzip compressed data, was "bpy_addon_build-0.1.1.tar", max compression
```

## Comparing `bpy_addon_build-0.1.0.tar` & `bpy_addon_build-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0     4884 2023-05-14 20:50:12.031540 bpy_addon_build-0.1.0/bpy_addon_build/__init__.py
--rw-r--r--   0        0        0      666 2023-05-14 20:30:55.184639 bpy_addon_build-0.1.0/bpy_addon_build/yaml_conf.py
--rw-r--r--   0        0        0      469 2023-05-14 21:06:31.656679 bpy_addon_build-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 bpy_addon_build-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4757 2023-05-14 23:04:40.989141 bpy_addon_build-0.1.1/bpy_addon_build/__init__.py
+-rw-r--r--   0        0        0      550 2023-05-14 22:58:32.318576 bpy_addon_build-0.1.1/bpy_addon_build/actions.py
+-rw-r--r--   0        0        0      666 2023-05-14 20:30:55.184639 bpy_addon_build-0.1.1/bpy_addon_build/yaml_conf.py
+-rw-r--r--   0        0        0      550 2023-05-14 23:06:12.276625 bpy_addon_build-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      634 1970-01-01 00:00:00.000000 bpy_addon_build-0.1.1/PKG-INFO
```

### Comparing `bpy_addon_build-0.1.0/bpy_addon_build/__init__.py` & `bpy_addon_build-0.1.1/bpy_addon_build/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,77 +1,66 @@
-import argparse
 import os
 import shutil
 import time
 from pathlib import Path
-from typing import Dict, List
+from typing import Dict, List, Optional
 from rich.console import Console
+from docopt import docopt
+from . import actions
 
 from . import yaml_conf
 
+# Current working directory
 WORKING_DIR: Path = Path(os.getcwd())
 
 # All file paths on Windows, MacOS, and Linux based on the Blender Docs
 # We use ~ for user directories, and we expand these later on in the code
 BLENDER_ADDON_DIR: List[str] = [
     "~/AppData/Roaming/Blender Foundation/Blender/{0}/scripts/addons",
     "~/Library/Application Support/Blender/{0}/scripts/addons",
     "~/.config/blender/{0}/scripts/addons",
 ]
+
+# Rich console
 console = Console()
 
 
-def init_argparse() -> argparse.ArgumentParser:
-    parser = argparse.ArgumentParser(
-        usage="%(prog)s [OPTION] [FILE]...",
-        description="Build Blender addons 10 times faster",
-    )
-    parser.add_argument(
-        "-v", "--version", action="version", version=f"{parser.prog} version 0.1.0"
-    )
-    parser.add_argument(
-        "--during-build",
-        action="store",
-        dest="db",
-        help="Defines an action to do in addition to default",
-    )
-    parser.add_argument("files", nargs="*")
-    return parser
+USAGE = """
+Usage:
+    bpy-addon-build (-h | --help)
+    bpy-addon-build (-b | --during-build) <action> [<file>]
+    bpy-addon-build [<file>]
+
+Options:
+  -h --help     Show this screen.
+  -b --during-build      Execute a set of actions in addition to the default action
+"""
 
 
+# Parse a file from a Path
 def parse_file(file: Path) -> yaml_conf.BpyBuildYaml:
     with open(file, "r") as f:
         yaml_config: yaml_conf.BpyBuildYaml = yaml_conf.BpyBuildYaml(f, file)
         return yaml_config
 
 
-def execute_action(action: Dict[str, str], inter_dir: Path):
-    if "create_file" in action:
-        file_path = inter_dir / Path(action["create_file"])
-        with open(file_path, "w") as f:
-            f.write("")
-
-
+# Main function
 def main():
-    parser = init_argparse()
-    args = parser.parse_args()
+    args = docopt(USAGE)
     bpy_build_yaml: Path = WORKING_DIR / Path("bpy-build.yaml")
-
-    if not args.files:
+    if not args["<file>"]:
         if bpy_build_yaml.exists():
             pass
         else:
             console.print(
                 "Can't find bpy-build.yaml, maybe pass it directly?", style="bold red"
             )
             return
     else:
-        for file in args.files:
-            bpy_build_yaml = Path(file).resolve()
-            break
+        bpy_build_yaml = Path(args["<file>"]).resolve()
 
     yaml_conf = parse_file(bpy_build_yaml)
     build_dir = bpy_build_yaml.parents[0] / Path("build")
     built_zip = build_dir / Path(yaml_conf.build_name + ".zip")
 
     # Check if the addon folder exists
     if not yaml_conf.addon_folder.exists():
@@ -85,63 +74,69 @@
     if not build_dir.exists():
         build_dir.mkdir()
 
     # Remove the built zip so we don't get errors
     if built_zip.exists():
         os.remove(built_zip)
 
+    # If there are build actions
     if len(yaml_conf.during_build):
+        # Copy the folder
         with console.status("[bold green]Copying...") as _:
             inter_dir: Path = build_dir / Path("inter")
             if inter_dir.exists():
                 shutil.rmtree(inter_dir)
             shutil.copytree(yaml_conf.addon_folder, inter_dir)
 
+        # Perform actions
         with console.status("[bold green]Executing Build Actions...") as _:
+            # Peform default action
             if "default" in yaml_conf.during_build:
                 for action in yaml_conf.during_build["default"]:
-                    execute_action(action, inter_dir)
-            else:
-                if args.db in yaml_conf.during_build:
-                    for action in yaml_conf.during_build[args.db]:
-                        execute_action(action, inter_dir)
-
+                    actions.execute_action(action, inter_dir)
+            # Perform extra action
+            if args["--during-build"] and args["<action>"] in yaml_conf.during_build:
+                for action in yaml_conf.during_build[args["<action>"]]:
+                    actions.execute_action(action, inter_dir)
+        # Rebuild
         with console.status("[bold green]Building...") as _:
             time.sleep(2)
             shutil.make_archive(str(build_dir / yaml_conf.build_name), "zip", inter_dir)
     else:
+        # Build addon
         with console.status("[bold green]Building...") as _:
             time.sleep(2)
             shutil.make_archive(
                 str(build_dir / yaml_conf.build_name), "zip", yaml_conf.addon_folder
             )
 
     # Install addon
     with console.status("[bold green] Installing...") as _:
         for path in map(Path, yaml_conf.install_versions):
+            # Expand the ~ in the path
             path = path.expanduser()
             if not path.exists():
-                path_exists = False
-                for test_path in BLENDER_ADDON_DIR:
-                    new_path = Path(test_path.format(str(path))).expanduser()
-                    if new_path.exists():
-                        path = new_path
-                        path_exists = True
-                        break
-                if not path_exists:
+                found: Optional[Path] = next(
+                    (
+                        Path(test_path.format(str(path))).expanduser()
+                        for test_path in BLENDER_ADDON_DIR
+                        if Path(test_path.format(str(path))).expanduser().exists()
+                    ),
+                    None,
+                )
+                if found:
+                    path = found
+                else:
                     console.print(
                         f"Path {str(path)} doesn't exist, skipping...",
                         style="bold yellow",
                     )
                     continue
-
             edited_path: Path = path / Path(yaml_conf.build_name)
-            if not edited_path.exists():
-                edited_path.mkdir()
-            else:
-                shutil.rmtree(edited_path)
+            shutil.rmtree(edited_path, ignore_errors=True)
+            edited_path.mkdir(exist_ok=True)
             shutil.unpack_archive(built_zip, edited_path)
-            time.sleep(2)
+            time.sleep(1)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `bpy_addon_build-0.1.0/bpy_addon_build/yaml_conf.py` & `bpy_addon_build-0.1.1/bpy_addon_build/yaml_conf.py`

 * *Files identical despite different names*

### Comparing `bpy_addon_build-0.1.0/PKG-INFO` & `bpy_addon_build-0.1.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: bpy-addon-build
-Version: 0.1.0
-Summary: A build system to make building and testing Blender addons 10 times easier`
+Version: 0.1.1
+Summary: A build system to make building and testing Blender addons 10 times easier
+Home-page: https://github.com/StandingPadAnimations/bpy-build
 License: MIT
 Author: StandingPad
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: docopt (>=0.6.2,<0.7.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
```

