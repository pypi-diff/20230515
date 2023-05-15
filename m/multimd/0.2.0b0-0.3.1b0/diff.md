# Comparing `tmp/multimd-0.2.0b0.tar.gz` & `tmp/multimd-0.3.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multimd-0.2.0b0.tar", max compression
+gzip compressed data, was "multimd-0.3.1b0.tar", max compression
```

## Comparing `multimd-0.2.0b0.tar` & `multimd-0.3.1b0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     2780 2023-05-10 20:57:34.352203 multimd-0.2.0b0/README.md
--rw-r--r--   0        0        0    35121 2023-05-10 20:57:34.348455 multimd-0.2.0b0/multimd/LICENSE.txt
--rw-r--r--   0        0        0     2780 2023-05-10 20:57:34.352793 multimd-0.2.0b0/multimd/README.md
--rw-r--r--   0        0        0       94 2023-05-10 20:57:34.346350 multimd-0.2.0b0/multimd/__init__.py
--rw-r--r--   0        0        0      132 2023-05-10 20:57:34.348975 multimd-0.2.0b0/multimd/__main__.py
--rw-r--r--   0        0        0     1868 2023-05-10 20:57:34.345987 multimd-0.2.0b0/multimd/mmdbuild.py
--rw-r--r--   0        0        0     2029 2023-05-10 20:57:34.346742 multimd-0.2.0b0/multimd/mmdcli.py
--rw-r--r--   0        0        0     5043 2023-05-10 20:57:34.344303 multimd-0.2.0b0/multimd/mmdtoc.py
--rw-r--r--   0        0        0      707 2023-05-10 20:56:54.204845 multimd-0.2.0b0/pyproject.toml
--rw-r--r--   0        0        0     3790 1970-01-01 00:00:00.000000 multimd-0.2.0b0/setup.py
--rw-r--r--   0        0        0     3676 1970-01-01 00:00:00.000000 multimd-0.2.0b0/PKG-INFO
+-rw-r--r--   0        0        0     2774 2023-05-14 20:08:40.340143 multimd-0.3.1b0/README.md
+-rw-r--r--   0        0        0    35121 2023-05-15 16:56:51.757748 multimd-0.3.1b0/multimd/LICENSE.txt
+-rw-r--r--   0        0        0     2774 2023-05-15 16:57:34.231747 multimd-0.3.1b0/multimd/README.md
+-rw-r--r--   0        0        0       88 2023-05-15 16:56:51.756184 multimd-0.3.1b0/multimd/__init__.py
+-rw-r--r--   0        0        0      126 2023-05-15 16:56:51.758378 multimd-0.3.1b0/multimd/__main__.py
+-rw-r--r--   0        0        0     1859 2023-05-15 16:56:51.754576 multimd-0.3.1b0/multimd/build.py
+-rw-r--r--   0        0        0     1955 2023-05-15 16:56:51.756772 multimd-0.3.1b0/multimd/cli.py
+-rw-r--r--   0        0        0     5045 2023-05-15 16:56:51.755513 multimd-0.3.1b0/multimd/toc.py
+-rw-r--r--   0        0        0      703 2023-05-14 21:07:43.771016 multimd-0.3.1b0/pyproject.toml
+-rw-r--r--   0        0        0     3670 1970-01-01 00:00:00.000000 multimd-0.3.1b0/PKG-INFO
```

### Comparing `multimd-0.2.0b0/README.md` & `multimd-0.3.1b0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -67,17 +67,17 @@
     /full/path/to/README.md
 ~~~
 
 
 There is also an easy-to-use `Python` API.
 
 ~~~python
-from multimd import MMDBuilder, Path
+from multimd import Builder, Path
 
-mybuilder = MMDBuilder(
+mybuilder = Builder(
     src   = Path("/full/path/to/readme"),
     dest  = Path("/full/path/to/README.md"),
     erase = True
 )
 mybuilder.build()
 ~~~
```

### Comparing `multimd-0.2.0b0/multimd/LICENSE.txt` & `multimd-0.3.1b0/multimd/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `multimd-0.2.0b0/multimd/README.md` & `multimd-0.3.1b0/multimd/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -67,17 +67,17 @@
     /full/path/to/README.md
 ~~~
 
 
 There is also an easy-to-use `Python` API.
 
 ~~~python
-from multimd import MMDBuilder, Path
+from multimd import Builder, Path
 
-mybuilder = MMDBuilder(
+mybuilder = Builder(
     src   = Path("/full/path/to/readme"),
     dest  = Path("/full/path/to/README.md"),
     erase = True
 )
 mybuilder.build()
 ~~~
```

### Comparing `multimd-0.2.0b0/multimd/mmdbuild.py` & `multimd-0.3.1b0/multimd/build.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 # This module allows to make a single path::``MD`` file from several single
 # ones (using or not an "automatic" merging).
 ###
 
 
 from pathlib import Path
 
-from .mmdtoc import *
+from .toc import *
 
 
 # ------------------------------------ #
 # -- SINGLE MD FROM MULTI SINGLE MD -- #
 # ------------------------------------ #
 
 ###
 # This class finds all the single path::``MD`` files and then builds a final
 # single one with all the chunks found.
 ###
-class MMDBuilder():
+class Builder():
 
 ###
 # prototype::
 #     src   : the path of the directory containing the path::``MD`` chunks.
 #     dest  : the path of the single final path::``MD`` file to build.
 #     erase : set to ``True``, this argument allows to erase an existing
 #             final file to build a new one.
@@ -44,15 +44,15 @@
 #     :action: this method finds the single path::``MD`` files, and then merges
 #              all the ¨md codes found to build the final path::``MD`` file.
 ###
     def build(self) -> None:
 # All the MD codes.
         mdcode = []
 
-        for onefile in MMDTOC(self.src).extract():
+        for onefile in TOC(self.src).extract():
             mdcode.append(
                 onefile.read_text(encoding = 'utf-8')
                        .strip()
             )
 
         mdcode = ('\n'*3).join(mdcode)
```

### Comparing `multimd-0.2.0b0/multimd/mmdcli.py` & `multimd-0.3.1b0/multimd/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 #!/usr/bin/env python3
 
 ###
 # This module implements the [C]-ommand [L]-ine [I]-nterface of ¨multimd.
 ###
 
-from typing import Tuple
 
-from pathlib import Path
+from typing import Tuple
 
 import                        typer
 from typing_extensions import Annotated
 
-from .mmdbuild import MMDBuilder
+from .build import Builder
 
 
 # --------- #
 # -- CLI -- #
 # --------- #
 
-mmd_CLI = typer.Typer()
+CLI = typer.Typer()
 
 ###
 # prototype::
-#     src_dest : a 2 dimensional tuple giving the path of the source
-#                directory with the MD chunks to be merged, and
-#                the path of the final MD file to build.
+#     src_dest : a couple of paths giving the source directory with
+#                the MD chunks to be merged, and the final MD file
+#                to build.
 #     erase    : set to ``True``, this argument allows to erase
 #                an existing final file before building the new one.
 #
 #     :action: :see: mmdbuild.MMDBuilder
 ###
-@mmd_CLI.command(
+@CLI.command(
     context_settings = dict(
         help_option_names = ['--help', '-h']
     ),
     help = "Merging MD chunks into a single MD file."
 )
-def _mmd_CLI(
+def _CLI(
     src_dest: Annotated[
         Tuple[Path,Path],
         typer.Argument(
             help = "Path of the source directory with "
                    "the MD chunks to be merged, followed "
                    "by the path of the final MD file to build."
     )],
@@ -59,15 +58,15 @@
     dest_message = src_dest[1]
 
     for i, p in enumerate(src_dest):
         if not p.is_absolute():
             src_dest[i] = cwd / p
 
 # Let's call our worker.
-    MMDBuilder(
+    Builder(
         erase = erase,
         *src_dest
     ).build()
 
 # Let's talk to the user.
     if Path(dest_message).is_absolute():
         message = f"""
```

### Comparing `multimd-0.2.0b0/multimd/mmdtoc.py` & `multimd-0.3.1b0/multimd/toc.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 #     2) If there is no path::``about.yaml`` file, a search is made only
 #        in path::``maindir``.
 #
 #
 # warning::
 #     Unlike the 1st mode, the 2nd one doesn't do searches in subfolders.
 ###
-class MMDTOC():
+class TOC():
 
 ###
 # prototype::
 #     maindir : the path of the directory to analyze.
 ###
     def __init__(
         self,
@@ -92,15 +92,15 @@
 # No files found at this moment.
         if strpaths == []:
             for fileordir in curdir.iterdir():
                 if not fileordir.is_file():
                     continue
 
                 if fileordir.suffix == MD_FILE_SUFFIX:
-                    strpaths.append(fileordir)
+                    strpaths.append(str(fileordir))
 
             strpaths = natsorted(strpaths)
 
 # No files found.
         if strpaths == []:
             raise IOError(
                 f'no file found inside ``{curdir}``.'
```

### Comparing `multimd-0.2.0b0/pyproject.toml` & `multimd-0.3.1b0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name         = "multimd"
-version      = "0.2.0-beta"
+version      = "0.3.1-beta"
 description  = 'This project makes it possible to write separated pieces of `MD` files that will be merged to produce one single final `MD` file.'
 readme       = "README.md"
 authors      = ["Christophe BAL"]
 maintainers  = ["Christophe BAL"]
 license      = "GNU License Version 3"
 repository   = "https://github.com/bc-tools/for-dev/tree/main/multimd"
 
 [tool.poetry.scripts]
-multimd = "multimd.__main__:mmd_CLI"
+multimd = "multimd.__main__:CLI"
 
 [tool.poetry.dependencies]
 python  = "^3.8"
 natsort = "^8.2"
 rich    = "^13.3.5"
 typer   = "^0.9"
```

### Comparing `multimd-0.2.0b0/PKG-INFO` & `multimd-0.3.1b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multimd
-Version: 0.2.0b0
+Version: 0.3.1b0
 Summary: This project makes it possible to write separated pieces of `MD` files that will be merged to produce one single final `MD` file.
 Home-page: https://github.com/bc-tools/for-dev/tree/main/multimd
 License: GNU License Version 3
 Author: Christophe BAL
 Maintainer: Christophe BAL
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
@@ -88,17 +88,17 @@
     /full/path/to/README.md
 ~~~
 
 
 There is also an easy-to-use `Python` API.
 
 ~~~python
-from multimd import MMDBuilder, Path
+from multimd import Builder, Path
 
-mybuilder = MMDBuilder(
+mybuilder = Builder(
     src   = Path("/full/path/to/readme"),
     dest  = Path("/full/path/to/README.md"),
     erase = True
 )
 mybuilder.build()
 ~~~
```

