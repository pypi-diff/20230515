# Comparing `tmp/cpggen-1.1.4.tar.gz` & `tmp/cpggen-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpggen-1.1.4.tar", max compression
+gzip compressed data, was "cpggen-1.1.5.tar", max compression
```

## Comparing `cpggen-1.1.4.tar` & `cpggen-1.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-05-12 21:35:17.130652 cpggen-1.1.4/LICENSE
--rw-r--r--   0        0        0    11907 2023-05-12 21:35:17.130652 cpggen-1.1.4/README.md
--rw-r--r--   0        0        0        0 2023-05-12 21:35:17.134652 cpggen-1.1.4/cpggen/__init__.py
--rw-r--r--   0        0        0    20677 2023-05-12 21:35:17.134652 cpggen-1.1.4/cpggen/cli.py
--rw-r--r--   0        0        0    39149 2023-05-12 21:35:17.134652 cpggen-1.1.4/cpggen/executor.py
--rw-r--r--   0        0        0     1078 2023-05-12 21:35:17.134652 cpggen-1.1.4/cpggen/logger.py
--rw-r--r--   0        0        0    14556 2023-05-12 21:35:17.134652 cpggen-1.1.4/cpggen/utils.py
--rw-r--r--   0        0        0     1326 2023-05-12 21:35:17.134652 cpggen-1.1.4/pyproject.toml
--rw-r--r--   0        0        0    13279 1970-01-01 00:00:00.000000 cpggen-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-15 09:59:59.282099 cpggen-1.1.5/LICENSE
+-rw-r--r--   0        0        0    12219 2023-05-15 09:59:59.282099 cpggen-1.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-15 09:59:59.286099 cpggen-1.1.5/cpggen/__init__.py
+-rw-r--r--   0        0        0    21377 2023-05-15 09:59:59.286099 cpggen-1.1.5/cpggen/cli.py
+-rw-r--r--   0        0        0    39366 2023-05-15 09:59:59.286099 cpggen-1.1.5/cpggen/executor.py
+-rw-r--r--   0        0        0     1078 2023-05-15 09:59:59.286099 cpggen-1.1.5/cpggen/logger.py
+-rw-r--r--   0        0        0    14556 2023-05-15 09:59:59.286099 cpggen-1.1.5/cpggen/utils.py
+-rw-r--r--   0        0        0     1326 2023-05-15 09:59:59.286099 cpggen-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0    13591 1970-01-01 00:00:00.000000 cpggen-1.1.5/PKG-INFO
```

### Comparing `cpggen-1.1.4/LICENSE` & `cpggen-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cpggen-1.1.4/README.md` & `cpggen-1.1.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -27,23 +27,23 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - Joern with all the CPG frontends
 - cpggen with Python 3.10
 - cdxgen with Node.js 18 - Generates SBoM
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.1.4/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.1.5/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v1.1.4/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v1.1.5/cpggen.exe
 .\cpggen.exe --help
 ```
 
 NOTE: On Windows, antivirus and antimalware could prevent this single executable from functioning properly. Depending on the system, administrative privileges might also be required. Use container-based execution as a fallback.
 
 ### OCI Artifacts via ORAS cli
 
@@ -176,14 +176,22 @@
 
 Pass `--slice` argument to extract intra-procedural slices from the CPG. By default, slices would be based on `Usages`. Pass `--slice-mode DataFlow` to create a sliced CPG based on `DataFlow`.
 
 ```bash
 cpggen -i ~/work/sandbox/crAPI -o ~/work/sandbox/crAPI/cpg_out --slice
 ```
 
+### Creating vectors
+
+Pass `--vectors` argument to extract vector representations of code from CPG in json format.
+
+```bash
+cpggen -i ~/work/sandbox/crAPI -o ~/work/sandbox/crAPI/cpg_out --vectors
+```
+
 ### Artifacts produced
 
 Upon successful completion, cpggen would produce the following artifacts in the directory specified under `out_dir`
 
 - {name}-{lang}-cpg.bin.zip - Code Property Graph for the given language type
 - {name}-{lang}-cpg.bom.xml - SBoM in CycloneDX XML format
 - {name}-{lang}-cpg.bom.json - SBoM in CycloneDX json format
@@ -203,16 +211,18 @@
 curl "http://127.0.0.1:7072/cpg?src=/Volumes/Work/sandbox/vulnerable-aws-koa-app&out_dir=/tmp/cpg_out&lang=js"
 ```
 
 ```
 curl "http://127.0.0.1:7072/cpg?url=https://github.com/HooliCorp/vulnerable-aws-koa-app&out_dir=/tmp/cpg_out&lang=js"
 ```
 
+Package url with slicing.
+
 ```
-curl "http://127.0.0.1:7072/cpg?url=pkg:maven/org.apache.commons/commons-io@1.3.2&out_dir=/tmp/cpg_out"
+curl "http://127.0.0.1:7072/cpg?url=pkg:maven/org.apache.commons/commons-io@1.3.2&out_dir=/tmp/cpg_out&slice=true"
 ```
 
 ## Languages supported
 
 | Language    | Requires build | Maturity |
 | ----------- | -------------- | -------- |
 | C           | No             | High     |
@@ -265,14 +275,15 @@
                         Export output directory
   --verbose             Run cpggen in verbose mode
   --skip-sbom           Do not generate SBoM
   --slice               Extract intra-procedural slices from the CPG
   --slice-mode {Usages,DataFlow}
                         Mode used for CPG slicing
   --use-parse           Use joern-parse command instead of invoking the language frontends. Useful when default overlays are important
+  --vectors             Extract vector representations of code from CPG
 ```
 
 ## Environment variables
 
 | Name                    | Purpose                                                                    |
 | ----------------------- | -------------------------------------------------------------------------- |
 | JOERN_HOME              | Joern installation directory                                               |
```

### Comparing `cpggen-1.1.4/cpggen/cli.py` & `cpggen-1.1.5/cpggen/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -213,43 +213,43 @@
         url = q.get("url")
     if q.get("src"):
         src = q.get("src")
     if q.get("out_dir"):
         cpg_out_dir = q.get("out_dir")
     if q.get("lang"):
         languages = q.get("lang")
-    if q.get("export", "") in ("true", "1"):
+    if q.get("export", "") in ("True", "true", "1"):
         export = True
-    if q.get("slice", "") in ("true", "1"):
+    if q.get("slice", "") in ("True", "true", "1"):
         slice = True
-    if q.get("vectors", "") in ("true", "1"):
+    if q.get("vectors", "") in ("True", "true", "1"):
         vectors = True
     if q.get("slice_mode"):
         slice_mode = q.get("slice_mode")
-    if q.get("auto_build", "") in ("false", "0"):
+    if q.get("auto_build", "") in ("False", "false", "0"):
         auto_build = False
-    if q.get("skip_sbom", "") in ("false", "0"):
+    if q.get("skip_sbom", "") in ("False", "false", "0"):
         skip_sbom = False
     if not url and params.get("url"):
         url = params.get("url")
     if not src and params.get("src"):
         src = params.get("src")
     if not languages and params.get("lang"):
         languages = params.get("lang")
     if not cpg_out_dir and params.get("out_dir"):
         cpg_out_dir = params.get("out_dir")
-    if params.get("auto_build", "") in ("false", "0"):
+    if params.get("auto_build", "") in ("False", "false", "0"):
         auto_build = False
-    if params.get("skip_sbom", "") in ("false", "0"):
+    if params.get("skip_sbom", "") in ("False", "false", "0"):
         skip_sbom = False
-    if params.get("export", "") in ("true", "1"):
+    if params.get("export", "") in ("True", "true", "1"):
         export = True
-    if params.get("slice", "") in ("true", "1"):
+    if params.get("slice", "") in ("True", "true", "1"):
         slice = True
-    if params.get("vectors", "") in ("true", "1"):
+    if params.get("vectors", "") in ("True", "true", "1"):
         vectors = True
     if params.get("slice_mode"):
         slice_mode = params.get("slice_mode")
     if not src and not url:
         return {"error": "true", "message": "path or url is required"}, 500
     # If src contains url, then reassign
     if not url and (
@@ -365,45 +365,63 @@
     slice_mode=None,
     url=None,
     vectors=False,
 ):
     if __name__ in ("__main__", "cpggen.cli"):
         with Pool(processes=os.cpu_count(), initializer=init_worker) as pool:
             try:
+                ret = []
+                exec_results = []
                 for lang in languages:
                     LOG.debug(f"Generating CPG for the language {lang} at {src}")
-                    pool.apply_async(
-                        executor.exec_tool,
-                        (
-                            lang,
-                            src,
-                            cpg_out_dir,
-                            src,
-                            joern_home,
-                            use_container,
-                            use_parse,
-                            auto_build,
-                            {
-                                "skip_sbom": skip_sbom,
-                                "slice_mode": slice_mode,
-                                "for_export": export,
-                                "for_slice": slice,
-                                "for_vectors": vectors,
-                                "url": url,
-                            },
-                        ),
+                    exec_results.append(
+                        pool.apply_async(
+                            executor.exec_tool,
+                            (
+                                lang,
+                                src,
+                                cpg_out_dir,
+                                src,
+                                joern_home,
+                                use_container,
+                                use_parse,
+                                auto_build,
+                                {
+                                    "skip_sbom": skip_sbom,
+                                    "slice_mode": slice_mode,
+                                    "for_export": export,
+                                    "for_slice": slice,
+                                    "for_vectors": vectors,
+                                    "url": url,
+                                },
+                            ),
+                        )
                     )
+                for res in exec_results:
+                    manifests_list = res.get()
+                    if manifests_list:
+                        ret += manifests_list
                 pool.close()
+                return ret
             except KeyboardInterrupt:
                 pool.terminate()
             pool.join()
+    return None
 
 
 def collect_cpg_manifests(cpg_out_dir):
-    return utils.find_files(cpg_out_dir, ".manifest.json")
+    cpg_manifests = []
+    if os.path.isfile(cpg_out_dir):
+        cpg_out_dir = os.path.dirname(cpg_out_dir)
+    mfiles = utils.find_files(cpg_out_dir, ".manifest.json") if cpg_out_dir else []
+    for amanifest in mfiles:
+        with open(amanifest) as mfp:
+            manifest_obj = json.load(mfp)
+            cpg_manifests.append(manifest_obj)
+    return cpg_manifests
 
 
 def fix_export_repr(export_repr, export_format):
     if export_format == "neo4jcsv":
         if export_repr != "cpg":
             LOG.warn(
                 "cpg is the only supported export representation for neo4jcsv format"
@@ -421,81 +439,81 @@
     export,
     export_repr,
     export_format,
     export_out_dir,
     slice,
     slice_mode,
     vectors,
+    cpg_manifests=None,
 ):
     if __name__ in ("__main__", "cpggen.cli"):
         with Pool(processes=os.cpu_count(), initializer=init_worker) as pool:
             try:
                 export_tool = "export"
                 if slice:
                     export_tool = "slice"
                 elif vectors:
                     export_tool = "vectors"
-                cpg_manifests = collect_cpg_manifests(cpg_out_dir)
-                for amanifest in cpg_manifests:
-                    with open(amanifest) as mfp:
-                        manifest_obj = json.load(mfp)
-                        if not manifest_obj or not manifest_obj.get("cpg"):
-                            continue
-                        app_export_out_dir = os.path.join(
-                            export_out_dir, manifest_obj["app"]
-                        )
-                        try:
-                            # joern-export annoyingly will not overwrite directories
-                            # but would expect first level directories to exist
-                            if os.path.exists(app_export_out_dir):
-                                try:
-                                    shutil.rmtree(app_export_out_dir)
-                                except Exception:
-                                    # Ignore remove errors
-                                    pass
-                            os.makedirs(export_out_dir, exist_ok=True)
-                        except Exception:
-                            # Ignore errors
-                            pass
-                        cpg_path = manifest_obj["cpg"]
-                        # In case of GitHub action we need to fix the cpg_path to prefix GITHUB_WORKSPACE
-                        # since the manifest would only have relative path
-                        if os.getenv("GITHUB_WORKSPACE") and not cpg_path.startswith(
-                            os.getenv("GITHUB_WORKSPACE")
-                        ):
-                            cpg_path = os.path.join(
-                                os.getenv("GITHUB_WORKSPACE"), cpg_path
-                            )
-                        if export:
-                            LOG.debug(
-                                f"""Exporting CPG for the app {manifest_obj["app"]} from {cpg_path} to {app_export_out_dir}"""
-                            )
-                        pool.apply_async(
-                            executor.exec_tool,
-                            (
-                                export_tool,
-                                cpg_path,
-                                app_export_out_dir,
-                                cpg_out_dir,
-                                joern_home,
-                                use_container,
-                                use_parse,
-                                False,
-                                {
-                                    "export_repr": fix_export_repr(
-                                        export_repr, export_format
-                                    )
-                                    if export
-                                    else None,
-                                    "export_format": export_format if export else None,
-                                    "slice_mode": slice_mode if slice else None,
-                                    "slice_out": manifest_obj.get("slice_out"),
-                                },
-                            ),
+                # Collect the CPG manifests if none was provided.
+                # This could result in duplicate executions
+                if not cpg_manifests:
+                    cpg_manifests = collect_cpg_manifests(cpg_out_dir)
+                for manifest_obj in cpg_manifests:
+                    if not manifest_obj or not manifest_obj.get("cpg"):
+                        continue
+                    app_export_out_dir = os.path.join(
+                        export_out_dir, manifest_obj["app"]
+                    )
+                    try:
+                        # joern-export annoyingly will not overwrite directories
+                        # but would expect first level directories to exist
+                        if os.path.exists(app_export_out_dir):
+                            try:
+                                shutil.rmtree(app_export_out_dir)
+                            except Exception:
+                                # Ignore remove errors
+                                pass
+                        os.makedirs(export_out_dir, exist_ok=True)
+                    except Exception:
+                        # Ignore errors
+                        pass
+                    cpg_path = manifest_obj["cpg"]
+                    # In case of GitHub action we need to fix the cpg_path to prefix GITHUB_WORKSPACE
+                    # since the manifest would only have relative path
+                    if os.getenv("GITHUB_WORKSPACE") and not cpg_path.startswith(
+                        os.getenv("GITHUB_WORKSPACE")
+                    ):
+                        cpg_path = os.path.join(os.getenv("GITHUB_WORKSPACE"), cpg_path)
+                    if export:
+                        LOG.debug(
+                            f"""Exporting CPG for the app {manifest_obj["app"]} from {cpg_path} to {app_export_out_dir}"""
                         )
+                    pool.apply_async(
+                        executor.exec_tool,
+                        (
+                            export_tool,
+                            cpg_path,
+                            app_export_out_dir,
+                            cpg_out_dir,
+                            joern_home,
+                            use_container,
+                            use_parse,
+                            False,
+                            {
+                                "export_repr": fix_export_repr(
+                                    export_repr, export_format
+                                )
+                                if export
+                                else None,
+                                "export_format": export_format if export else None,
+                                "slice_mode": slice_mode if slice else None,
+                                "slice_out": manifest_obj.get("slice_out"),
+                            },
+                        ),
+                    )
                 pool.close()
             except KeyboardInterrupt:
                 pool.terminate()
             pool.join()
 
 
 def main():
@@ -570,15 +588,15 @@
             export_out_dir = tempfile.mkdtemp(prefix="cpggen_export_out")
     if not languages or languages == "autodetect":
         languages = utils.detect_project_type(src)
     else:
         languages = languages.split(",")
     if cpg_out_dir and not os.path.exists(cpg_out_dir):
         os.makedirs(cpg_out_dir, exist_ok=True)
-    cpg(
+    cpg_manifests = cpg(
         src,
         cpg_out_dir,
         languages,
         joern_home=joern_home,
         use_container=use_container,
         use_parse=use_parse,
         auto_build=args.auto_build,
@@ -599,14 +617,15 @@
             export=args.export,
             export_repr=args.export_repr,
             export_format=args.export_format,
             export_out_dir=export_out_dir,
             slice=args.slice,
             slice_mode=args.slice_mode,
             vectors=args.vectors,
+            cpg_manifests=cpg_manifests,
         )
     if is_temp_dir:
         try:
             shutil.rmtree(src)
         except Exception:
             # Ignore cleanup errors
             pass
```

### Comparing `cpggen-1.1.4/cpggen/executor.py` & `cpggen-1.1.5/cpggen/executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,14 +279,19 @@
     except Exception as e:
         LOG.error(e)
 
 
 def dot_convert(export_out_dir, env):
     if check_command("dot"):
         dot_files = find_files(export_out_dir, ".dot", False, False)
+        if len(dot_files) > 5:
+            LOG.info(
+                f"{len(dot_files)} dot files generated after export. Skipping dot2png conversion ..."
+            )
+            return
         for df in dot_files:
             convert_cmd_with_args = cpg_tools_map["dot2png"] % dict(
                 dot_file=df, png_out=df.replace(".dot", ".png")
             )
             try:
                 subprocess.run(
                     convert_cmd_with_args.split(" "),
@@ -550,16 +555,14 @@
                             f"{os.path.basename(amodule)}-{tool_lang_simple}-cpg.bin.zip",
                         )
                     )
                 )
                 if tool_lang in ("export", "vectors"):
                     cpg_out = os.path.abspath(cpg_out_dir)
                 elif tool_lang == "slice":
-                    if not slice_out:
-                        slice_out = cpg_out.replace(".bin.zip", ".slices")
                     cpg_out = src
                 else:
                     sbom_out = (
                         cpg_out.replace(".bin.zip", ".bom.xml")
                         if cpg_out.endswith(".bin.zip")
                         else f"{cpg_out}.bom.xml"
                     )
@@ -580,15 +583,17 @@
                     cpg_out=cpg_out,
                     joern_home=joern_home,
                     home_dir=str(Path.home()),
                     uber_jar=uber_jar,
                     csharp_artifacts=csharp_artifacts,
                     memory=os.getenv("CPGGEN_MEMORY", max_memory),
                     tool_lang=tool_lang,
-                    parse_lang=joern_parse_lang_map.get(tool_lang, tool_lang),
+                    parse_lang=joern_parse_lang_map.get(
+                        tool_lang_simple, tool_lang_simple
+                    ),
                     sbom_out=sbom_out,
                     cpggen_bin_dir=os.getenv("CPGGEN_BIN_DIR", "/usr/local/bin"),
                     bin_ext=bin_ext,
                     exe_ext=exe_ext,
                     only_bat_ext=only_bat_ext,
                     android_jar=f' {os.getenv("JIMPLE_ANDROID_JAR", "").strip()}'
                     if os.getenv("JIMPLE_ANDROID_JAR")
@@ -712,15 +717,15 @@
                                     f"Unable to {tool_lang} {src} to {check_dir}. Try running joern-{tool_lang} manually using the command {' '.join(cmd_list_with_args)}"
                                 )
                     except Exception as e:
                         LOG.warn(f"Unable to {tool_lang} {src} to {cpg_out_dir}")
                         LOG.error(e)
                     progress.update(task, completed=100, total=100)
                     continue
-                LOG.info(
+                LOG.debug(
                     '⚡︎ Generating CPG for the {} app "{}" - "{}"'.format(
                         tool_lang,
                         os.path.basename(amodule),
                         " ".join(cmd_list_with_args),
                     )
                 )
                 cwd = amodule
@@ -755,15 +760,18 @@
                                 LOG.debug(cp.stdout)
                             if cp.stderr:
                                 LOG.debug(cp.stderr)
                     except Exception:
                         # Ignore SBoM errors
                         pass
                 progress.update(
-                    task, description="Generating CPG", completed=20, total=100
+                    task,
+                    description=f"Generating {tool_lang_simple} CPG",
+                    completed=20,
+                    total=100,
                 )
                 cp = subprocess.run(
                     cmd_list_with_args,
                     stdout=stdout,
                     stderr=stderr,
                     cwd=cwd,
                     env=env,
```

### Comparing `cpggen-1.1.4/cpggen/logger.py` & `cpggen-1.1.5/cpggen/logger.py`

 * *Files identical despite different names*

### Comparing `cpggen-1.1.4/cpggen/utils.py` & `cpggen-1.1.5/cpggen/utils.py`

 * *Files identical despite different names*

### Comparing `cpggen-1.1.4/pyproject.toml` & `cpggen-1.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cpggen"
-version = "1.1.4"
+version = "1.1.5"
 description = "Generate CPG for multiple languages for use with joern"
 authors = ["Team AppThreat <cloud@appthreat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "cpggen"}]
 homepage = "https://github.com/AppThreat/cpggen"
 repository = "https://github.com/AppThreat/cpggen"
```

### Comparing `cpggen-1.1.4/PKG-INFO` & `cpggen-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpggen
-Version: 1.1.4
+Version: 1.1.5
 Summary: Generate CPG for multiple languages for use with joern
 Home-page: https://github.com/AppThreat/cpggen
 License: Apache-2.0
 Keywords: joern,code analysis,static analysis,cpg,code property graph
 Author: Team AppThreat
 Author-email: cloud@appthreat.com
 Requires-Python: >=3.8.1,<3.12
@@ -60,23 +60,23 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - Joern with all the CPG frontends
 - cpggen with Python 3.10
 - cdxgen with Node.js 18 - Generates SBoM
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.1.4/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.1.5/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v1.1.4/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v1.1.5/cpggen.exe
 .\cpggen.exe --help
 ```
 
 NOTE: On Windows, antivirus and antimalware could prevent this single executable from functioning properly. Depending on the system, administrative privileges might also be required. Use container-based execution as a fallback.
 
 ### OCI Artifacts via ORAS cli
 
@@ -209,14 +209,22 @@
 
 Pass `--slice` argument to extract intra-procedural slices from the CPG. By default, slices would be based on `Usages`. Pass `--slice-mode DataFlow` to create a sliced CPG based on `DataFlow`.
 
 ```bash
 cpggen -i ~/work/sandbox/crAPI -o ~/work/sandbox/crAPI/cpg_out --slice
 ```
 
+### Creating vectors
+
+Pass `--vectors` argument to extract vector representations of code from CPG in json format.
+
+```bash
+cpggen -i ~/work/sandbox/crAPI -o ~/work/sandbox/crAPI/cpg_out --vectors
+```
+
 ### Artifacts produced
 
 Upon successful completion, cpggen would produce the following artifacts in the directory specified under `out_dir`
 
 - {name}-{lang}-cpg.bin.zip - Code Property Graph for the given language type
 - {name}-{lang}-cpg.bom.xml - SBoM in CycloneDX XML format
 - {name}-{lang}-cpg.bom.json - SBoM in CycloneDX json format
@@ -236,16 +244,18 @@
 curl "http://127.0.0.1:7072/cpg?src=/Volumes/Work/sandbox/vulnerable-aws-koa-app&out_dir=/tmp/cpg_out&lang=js"
 ```
 
 ```
 curl "http://127.0.0.1:7072/cpg?url=https://github.com/HooliCorp/vulnerable-aws-koa-app&out_dir=/tmp/cpg_out&lang=js"
 ```
 
+Package url with slicing.
+
 ```
-curl "http://127.0.0.1:7072/cpg?url=pkg:maven/org.apache.commons/commons-io@1.3.2&out_dir=/tmp/cpg_out"
+curl "http://127.0.0.1:7072/cpg?url=pkg:maven/org.apache.commons/commons-io@1.3.2&out_dir=/tmp/cpg_out&slice=true"
 ```
 
 ## Languages supported
 
 | Language    | Requires build | Maturity |
 | ----------- | -------------- | -------- |
 | C           | No             | High     |
@@ -298,14 +308,15 @@
                         Export output directory
   --verbose             Run cpggen in verbose mode
   --skip-sbom           Do not generate SBoM
   --slice               Extract intra-procedural slices from the CPG
   --slice-mode {Usages,DataFlow}
                         Mode used for CPG slicing
   --use-parse           Use joern-parse command instead of invoking the language frontends. Useful when default overlays are important
+  --vectors             Extract vector representations of code from CPG
 ```
 
 ## Environment variables
 
 | Name                    | Purpose                                                                    |
 | ----------------------- | -------------------------------------------------------------------------- |
 | JOERN_HOME              | Joern installation directory                                               |
```

