# Comparing `tmp/prophecy-build-tool-1.0.5.0.tar.gz` & `tmp/prophecy-build-tool-1.1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prophecy-build-tool-1.0.5.0.tar", last modified: Wed Apr 26 12:33:38 2023, max compression
+gzip compressed data, was "prophecy-build-tool-1.1.0.0.tar", last modified: Mon May 15 11:22:34 2023, max compression
```

## Comparing `prophecy-build-tool-1.0.5.0.tar` & `prophecy-build-tool-1.1.0.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 ashishpatel   (501) staff       (20)        0 2023-04-26 12:33:38.272828 prophecy-build-tool-1.0.5.0/
--rw-r--r--   0 ashishpatel   (501) staff       (20)    11357 2023-02-21 12:57:27.000000 prophecy-build-tool-1.0.5.0/LICENSE
--rw-r--r--   0 ashishpatel   (501) staff       (20)     5941 2023-04-26 12:33:38.272896 prophecy-build-tool-1.0.5.0/PKG-INFO
--rw-r--r--   0 ashishpatel   (501) staff       (20)     5318 2023-04-26 12:33:20.000000 prophecy-build-tool-1.0.5.0/README.md
--rw-r--r--   0 ashishpatel   (501) staff       (20)      419 2023-04-26 12:33:20.000000 prophecy-build-tool-1.0.5.0/pyproject.toml
--rw-r--r--   0 ashishpatel   (501) staff       (20)      239 2023-04-26 12:33:38.273183 prophecy-build-tool-1.0.5.0/setup.cfg
--rw-r--r--   0 ashishpatel   (501) staff       (20)     1182 2023-04-26 12:33:20.000000 prophecy-build-tool-1.0.5.0/setup.py
-drwxr-xr-x   0 ashishpatel   (501) staff       (20)        0 2023-04-26 12:33:38.270364 prophecy-build-tool-1.0.5.0/src/
-drwxr-xr-x   0 ashishpatel   (501) staff       (20)        0 2023-04-26 12:33:38.271749 prophecy-build-tool-1.0.5.0/src/pbt/
--rw-r--r--   0 ashishpatel   (501) staff       (20)     2283 2023-04-26 12:33:20.000000 prophecy-build-tool-1.0.5.0/src/pbt/__init__.py
--rw-r--r--   0 ashishpatel   (501) staff       (20)     1941 2023-04-26 12:33:20.000000 prophecy-build-tool-1.0.5.0/src/pbt/process.py
--rw-r--r--   0 ashishpatel   (501) staff       (20)    33775 2023-04-26 12:33:20.000000 prophecy-build-tool-1.0.5.0/src/pbt/prophecy_build_tool.py
-drwxr-xr-x   0 ashishpatel   (501) staff       (20)        0 2023-04-26 12:33:38.272562 prophecy-build-tool-1.0.5.0/src/prophecy_build_tool.egg-info/
--rw-r--r--   0 ashishpatel   (501) staff       (20)     5941 2023-04-26 12:33:38.000000 prophecy-build-tool-1.0.5.0/src/prophecy_build_tool.egg-info/PKG-INFO
--rw-r--r--   0 ashishpatel   (501) staff       (20)      424 2023-04-26 12:33:38.000000 prophecy-build-tool-1.0.5.0/src/prophecy_build_tool.egg-info/SOURCES.txt
--rw-r--r--   0 ashishpatel   (501) staff       (20)        1 2023-04-26 12:33:38.000000 prophecy-build-tool-1.0.5.0/src/prophecy_build_tool.egg-info/dependency_links.txt
--rw-r--r--   0 ashishpatel   (501) staff       (20)       33 2023-04-26 12:33:38.000000 prophecy-build-tool-1.0.5.0/src/prophecy_build_tool.egg-info/entry_points.txt
--rw-r--r--   0 ashishpatel   (501) staff       (20)       77 2023-04-26 12:33:38.000000 prophecy-build-tool-1.0.5.0/src/prophecy_build_tool.egg-info/requires.txt
--rw-r--r--   0 ashishpatel   (501) staff       (20)        4 2023-04-26 12:33:38.000000 prophecy-build-tool-1.0.5.0/src/prophecy_build_tool.egg-info/top_level.txt
-drwxr-xr-x   0 ashishpatel   (501) staff       (20)        0 2023-04-26 12:33:38.272709 prophecy-build-tool-1.0.5.0/test/
--rw-r--r--   0 ashishpatel   (501) staff       (20)     2133 2023-04-26 12:33:20.000000 prophecy-build-tool-1.0.5.0/test/test_build.py
+drwxr-xr-x   0 ashishpatel   (501) staff       (20)        0 2023-05-15 11:22:34.908846 prophecy-build-tool-1.1.0.0/
+-rw-r--r--   0 ashishpatel   (501) staff       (20)    11357 2023-02-21 12:57:27.000000 prophecy-build-tool-1.1.0.0/LICENSE
+-rw-r--r--   0 ashishpatel   (501) staff       (20)     5941 2023-05-15 11:22:34.908913 prophecy-build-tool-1.1.0.0/PKG-INFO
+-rw-r--r--   0 ashishpatel   (501) staff       (20)     5318 2023-04-26 12:33:20.000000 prophecy-build-tool-1.1.0.0/README.md
+-rw-r--r--   0 ashishpatel   (501) staff       (20)      419 2023-04-26 12:33:20.000000 prophecy-build-tool-1.1.0.0/pyproject.toml
+-rw-r--r--   0 ashishpatel   (501) staff       (20)      239 2023-05-15 11:22:34.909161 prophecy-build-tool-1.1.0.0/setup.cfg
+-rw-r--r--   0 ashishpatel   (501) staff       (20)     1182 2023-05-15 11:21:47.000000 prophecy-build-tool-1.1.0.0/setup.py
+drwxr-xr-x   0 ashishpatel   (501) staff       (20)        0 2023-05-15 11:22:34.905246 prophecy-build-tool-1.1.0.0/src/
+drwxr-xr-x   0 ashishpatel   (501) staff       (20)        0 2023-05-15 11:22:34.906833 prophecy-build-tool-1.1.0.0/src/pbt/
+-rw-r--r--   0 ashishpatel   (501) staff       (20)     2471 2023-05-15 11:21:47.000000 prophecy-build-tool-1.1.0.0/src/pbt/__init__.py
+-rw-r--r--   0 ashishpatel   (501) staff       (20)     1941 2023-04-26 12:33:20.000000 prophecy-build-tool-1.1.0.0/src/pbt/process.py
+-rw-r--r--   0 ashishpatel   (501) staff       (20)    36939 2023-05-15 11:21:47.000000 prophecy-build-tool-1.1.0.0/src/pbt/prophecy_build_tool.py
+drwxr-xr-x   0 ashishpatel   (501) staff       (20)        0 2023-05-15 11:22:34.908221 prophecy-build-tool-1.1.0.0/src/prophecy_build_tool.egg-info/
+-rw-r--r--   0 ashishpatel   (501) staff       (20)     5941 2023-05-15 11:22:34.000000 prophecy-build-tool-1.1.0.0/src/prophecy_build_tool.egg-info/PKG-INFO
+-rw-r--r--   0 ashishpatel   (501) staff       (20)      444 2023-05-15 11:22:34.000000 prophecy-build-tool-1.1.0.0/src/prophecy_build_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 ashishpatel   (501) staff       (20)        1 2023-05-15 11:22:34.000000 prophecy-build-tool-1.1.0.0/src/prophecy_build_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 ashishpatel   (501) staff       (20)       33 2023-05-15 11:22:34.000000 prophecy-build-tool-1.1.0.0/src/prophecy_build_tool.egg-info/entry_points.txt
+-rw-r--r--   0 ashishpatel   (501) staff       (20)       77 2023-05-15 11:22:34.000000 prophecy-build-tool-1.1.0.0/src/prophecy_build_tool.egg-info/requires.txt
+-rw-r--r--   0 ashishpatel   (501) staff       (20)        4 2023-05-15 11:22:34.000000 prophecy-build-tool-1.1.0.0/src/prophecy_build_tool.egg-info/top_level.txt
+drwxr-xr-x   0 ashishpatel   (501) staff       (20)        0 2023-05-15 11:22:34.908608 prophecy-build-tool-1.1.0.0/test/
+-rw-r--r--   0 ashishpatel   (501) staff       (20)     2186 2023-05-15 11:21:47.000000 prophecy-build-tool-1.1.0.0/test/test_build.py
+-rw-r--r--   0 ashishpatel   (501) staff       (20)     7868 2023-05-15 11:21:47.000000 prophecy-build-tool-1.1.0.0/test/test_deploy.py
```

### Comparing `prophecy-build-tool-1.0.5.0/LICENSE` & `prophecy-build-tool-1.1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.0.5.0/PKG-INFO` & `prophecy-build-tool-1.1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prophecy-build-tool
-Version: 1.0.5.0
+Version: 1.1.0.0
 Summary: Prophecy-build-tool (PBT) provides utilities to build and distribute projects created from the Prophecy IDE.
 Home-page: https://github.com/SimpleDataLabsInc/prophecy-build-tool
 Author: Prophecy
 Author-email: maciej@prophecy.io
 Project-URL: Bug Tracker, https://github.com/SimpleDataLabsInc/prophecy-build-tool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `prophecy-build-tool-1.0.5.0/README.md` & `prophecy-build-tool-1.1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.0.5.0/setup.py` & `prophecy-build-tool-1.1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as _in:
     long_description = _in.read()
 
 setuptools.setup(
     name="prophecy-build-tool",
-    version="1.0.5.0",
+    version="1.1.0.0",
     author="Prophecy",
     author_email="maciej@prophecy.io",
     description="Prophecy-build-tool (PBT) provides utilities to build and distribute projects created from the "
     "Prophecy IDE.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SimpleDataLabsInc/prophecy-build-tool",
```

### Comparing `prophecy-build-tool-1.0.5.0/src/pbt/__init__.py` & `prophecy-build-tool-1.1.0.0/src/pbt/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,26 +63,32 @@
     default="",
 )
 @click.option(
     "--fabric-ids",
     help="Fabric IDs(comma separated) which can be used to filter jobs for deployments",
     default="",
 )
+@click.option(
+    "--job-ids",
+    help="Job IDs(comma separated) which can be used to filter jobs for deployment",
+    default="",
+)
 @click.option("--skip-builds", is_flag=True, default=False, help="Flag to skip building Pipelines")
 def deploy(
     path,
     dependent_projects_path,
     release_version,
     project_id,
     prophecy_url,
     fabric_ids,
+    job_ids,
     skip_builds,
 ):
     pbt = ProphecyBuildTool(path, dependent_projects_path, release_version, project_id, prophecy_url)
-    pbt.deploy(fabric_ids, skip_builds)
+    pbt.deploy(fabric_ids=fabric_ids, skip_builds=skip_builds, job_ids=job_ids)
 
 
 @cli.command()
 @click.option(
     "--path",
     help="Path to the directory containing the pbt_project.yml file",
     required=True,
```

### Comparing `prophecy-build-tool-1.0.5.0/src/pbt/process.py` & `prophecy-build-tool-1.1.0.0/src/pbt/process.py`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.0.5.0/src/pbt/prophecy_build_tool.py` & `prophecy-build-tool-1.1.0.0/src/pbt/prophecy_build_tool.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,14 +62,45 @@
         self.project_id = (
             project_id if project_id else os.getenv("PROJECT_ID_PLACEHOLDER", "__PROJECT_ID_PLACEHOLDER__")
         )
         self.prophecy_url = (
             prophecy_url if prophecy_url else os.getenv("PROPHECY_URL_PLACEHOLDER", "__PROPHECY_URL_PLACEHOLDER__")
         )
 
+    def get_databricks_job_json_path(self, path_job):
+        path_job_absolute = os.path.join(os.path.join(self.path_root, path_job), "code")
+        return os.path.join(path_job_absolute, "databricks-job.json")
+
+    def get_prophecy_job_json_path(self, path_job):
+        path_job_absolute = os.path.join(os.path.join(self.path_root, path_job), "code")
+        return os.path.join(path_job_absolute, "prophecy-job.json")
+
+    # find all the pipelines which are needed to be build for the jobs
+    def generate_pipeline_deps(self):
+        all_jobs_deps = []
+        for job_idx, (path_job, job) in enumerate(self.jobs.items()):
+            prophecy_job_definition = self.get_prophecy_job_json_path(path_job)
+            with open(prophecy_job_definition, "r") as _in:
+                job_definition = json.load(_in)
+
+            pipeline_deps = [
+                x["properties"]["pipelineId"]
+                for x in job_definition["processes"].values()
+                if x["component"] == "Pipeline"
+            ]
+            all_jobs_deps.extend(pipeline_deps)
+
+        unique_deps = set(all_jobs_deps)
+        print(
+            f"\n[bold blue][INFO]: Total Unique pipelines dependencies found: {len(unique_deps)}\n {unique_deps}[/bold blue]"
+        )
+        pipelines_to_build = {k: v for k, v in self.pipelines.items() if k in unique_deps}
+        print(f"\n[INFO]: Total Filtered pipelines to build: {len(pipelines_to_build)}")
+        return pipelines_to_build
+
     def get_python_commands(self, cwd):
         if (
             Process.process_sequential(
                 [
                     Process(
                         ["python3", "--version"],
                         cwd,
@@ -129,21 +160,23 @@
             sys.exit(1)
         else:
             sys.exit(0)
 
     def build(self, pipelines, exit_on_build_failure=True):
         if not pipelines:  # if pipelines not provided run for all pipelines
             pipelines = self.pipelines
-        else:  # else filter pipelines
+        elif isinstance(pipelines, str):  # elif filter pipelines provided as string
             pipeline_filter = [x.strip() for x in pipelines.split(",")]
             print("\n[bold blue]Filtering pipelines: %s [/bold blue]" % str(pipeline_filter))
             pipelines = {k: v for k, v in self.pipelines.items() if k.split("/")[1] in pipeline_filter}
             if not pipelines:  # empty no matching pipeline found
                 print("\n[bold yellow]No matching pipelines found for given pipelines names: %s" % (pipeline_filter))
                 raise Exception()
+        else:  # pipelines are provided
+            print(f"\n[INFO]: Building given custom pipelines: {pipelines}")
 
         print("\n[bold blue]Building %s pipelines [/bold blue]" % len(pipelines))
         overall_build_status = True
         for pipeline_i, (path_pipeline, pipeline) in enumerate(pipelines.items()):
             print("\n  Building pipeline %s [%s/%s]" % (path_pipeline, pipeline_i + 1, len(pipelines)))
 
             path_pipeline_absolute = os.path.join(os.path.join(self.path_root, path_pipeline), "code")
@@ -196,46 +229,74 @@
                 overall_build_status = False
 
         if not overall_build_status and exit_on_build_failure:
             sys.exit(1)
         else:
             return overall_build_status, self.pipelines_build_path
 
-    def deploy(self, fabric_ids: str = "", skip_builds: bool = False):
+    def deploy(self, fabric_ids: str = "", skip_builds: bool = False, job_ids=None):
+        # not allowed to pass job_id and fabric_ids filter together ( as only job_id support incremental build and
+        # deploy), fabric_ids filter builds all pipelines by default and then deploy after filtering
+        if job_ids and fabric_ids:
+            print(f"[ERROR]: Can't combine filters, Please pass either --fabric_ids or --job_ids")
+            raise Exception()
+
+        if job_ids and skip_builds:
+            print(
+                f"[ERROR]: Can't skip builds for job_id filter,\nas it only builds depending pipelines ,\nPlease "
+                f"pass either --skip-builds or --job_id filter"
+            )
+            raise Exception()
+
         fabric_ids = list(i.strip() for i in fabric_ids.split(r",")) if fabric_ids else list()
+        job_ids = list(i.strip() for i in job_ids.split(r",")) if job_ids else list()
+
+        if not fabric_ids and not job_ids:
+            print("Deploying jobs for all Fabrics")
+        elif job_ids:  # job_id filter is provided
+            print(f"Deploying jobs only for given Job IDs: {str(job_ids)}")
+        else:
+            print("Deploying jobs only for given Fabric IDs: %s" % (str(fabric_ids)))
 
         self._verify_databricks_configs()
         config = EnvironmentVariableConfigProvider().get_config()
 
         self.api_client = _get_api_client(config)
 
         self.dbfs_service = DbfsService(self.api_client)
         self.jobs_service = JobsService(self.api_client)
 
-        if not skip_builds:
+        if not skip_builds and not job_ids:  # build all pipelines
             self.build(dict())
+        elif job_ids:
+            filtered_jobs = {k: v for k, v in self.jobs.items() if k.split("/")[1] in job_ids}
+            if len(filtered_jobs) == 0:
+                print(
+                    f"[ERROR]: No Job IDs matches with passed --job_id filter {str(job_ids)}\nAvailable Job IDs are: {self.jobs.keys()}"
+                )
+                raise Exception()
+            else:
+                self.jobs = filtered_jobs
+                self.jobs_count = len(self.jobs)
+            print("[INFO]: Generating depending pipelines for all jobs as '--job-ids' flag is passed.")
+            pipelines_to_build = self.generate_pipeline_deps()
+            self.build(pipelines_to_build)
         else:
             print("[SKIP]: Skipping builds for all pipelines as '--skip-builds' flag is passed.")
 
         print("\n[bold blue] Deploying %s jobs [/bold blue]" % self.jobs_count)
 
         pipelines_upload_failures = collections.defaultdict(list)
         job_update_failures = dict()
 
-        if not fabric_ids:
-            print("Deploying jobs for all Fabrics")
-        else:
-            print("Deploying jobs only for given Fabric IDs: %s" % (str(fabric_ids)))
-
         for job_idx, (path_job, job) in enumerate(self.jobs.items()):
             pipelines_upload_failures_job = collections.defaultdict(list)
             print("\n[START]:  Deploying job %s [%s/%s]" % (path_job, job_idx + 1, self.jobs_count))
 
-            path_job_absolute = os.path.join(os.path.join(self.path_root, path_job), "code")
-            path_job_definition = os.path.join(path_job_absolute, "databricks-job.json")
+            path_job_definition = self.get_databricks_job_json_path(path_job)
 
             with open(path_job_definition, "r") as _in:
                 data = _in.read()
                 data = (
                     data.replace("__PROJECT_RELEASE_VERSION_PLACEHOLDER__", self.project_release)
                     .replace("__PROJECT_ID_PLACEHOLDER__", self.project_id)
                     .replace("__PROPHECY_URL_PLACEHOLDER__", self.prophecy_url)
```

### Comparing `prophecy-build-tool-1.0.5.0/src/prophecy_build_tool.egg-info/PKG-INFO` & `prophecy-build-tool-1.1.0.0/src/prophecy_build_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prophecy-build-tool
-Version: 1.0.5.0
+Version: 1.1.0.0
 Summary: Prophecy-build-tool (PBT) provides utilities to build and distribute projects created from the Prophecy IDE.
 Home-page: https://github.com/SimpleDataLabsInc/prophecy-build-tool
 Author: Prophecy
 Author-email: maciej@prophecy.io
 Project-URL: Bug Tracker, https://github.com/SimpleDataLabsInc/prophecy-build-tool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `prophecy-build-tool-1.0.5.0/test/test_build.py` & `prophecy-build-tool-1.1.0.0/test/test_build.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,26 +5,27 @@
 PROJECT_PATH = str(os.getcwd()) + "/test/resources/HelloWorld"
 
 
 def test_build_path_default():
     runner = CliRunner()
     result = runner.invoke(build, ["--path", PROJECT_PATH])
     assert result.exit_code == 0
-    assert "Found 3 pipelines" in result.output
-    assert "Building 3 pipelines" in result.output
+    assert "Found 4 pipelines" in result.output
+    assert "Building 4 pipelines" in result.output
     assert "Building pipeline pipelines/customers_orders" in result.output
     assert "Building pipeline pipelines/join_agg_sort" in result.output
     assert "Building pipeline pipelines/report_top_customers" in result.output
+    assert "Building pipeline pipelines/farmers-markets-irs" in result.output
 
 
 def test_build_path_pipeline_filter():
     runner = CliRunner()
     result = runner.invoke(build, ["--path", PROJECT_PATH, "--pipelines", "customers_orders,join_agg_sort"])
     assert result.exit_code == 0
-    assert "Found 3 pipelines" in result.output
+    assert "Found 4 pipelines" in result.output
     assert "Building 2 pipelines" in result.output
     assert "Filtering pipelines: ['customers_orders', 'join_agg_sort']" in result.output
     assert "Building pipeline pipelines/customers_orders" in result.output
     assert "Building pipeline pipelines/join_agg_sort" in result.output
 
 
 def test_build_path_pipeline_with_invalid_filter():
@@ -34,21 +35,20 @@
         [
             "--path",
             PROJECT_PATH,
             "--pipelines",
             "customers_orders,INVALID_PIPELINE_NAME",
         ],
     )
-    print(result.output)
     assert result.exit_code == 0
-    assert "Found 3 pipelines" in result.output
+    assert "Found 4 pipelines" in result.output
     assert "Building 1 pipelines" in result.output
     assert "Filtering pipelines: ['customers_orders', 'INVALID_PIPELINE_NAME']" in result.output
     assert "Building pipeline pipelines/customers_orders" in result.output
 
 
 def test_build_path_pipeline_invalid_filter_only():
     runner = CliRunner()
     result = runner.invoke(build, ["--path", PROJECT_PATH, "--pipelines", "INVALID_PIPELINE_NAME"])
     assert result.exit_code == 1
-    assert "Found 3 pipelines" in result.output
+    assert "Found 4 pipelines" in result.output
     assert "No matching pipelines found for given pipelines names: ['INVALID_PIPELINE_NAME']" in result.output
```

