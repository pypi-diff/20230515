# Comparing `tmp/garden_ai-0.4.0.tar.gz` & `tmp/garden_ai-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garden_ai-0.4.0.tar", max compression
+gzip compressed data, was "garden_ai-0.4.1.tar", max compression
```

## Comparing `garden_ai-0.4.0.tar` & `garden_ai-0.4.1.tar`

### file list

```diff
@@ -1,32 +1,34 @@
--rw-r--r--   0        0        0     1078 2023-04-27 18:43:36.665809 garden_ai-0.4.0/LICENSE
--rw-r--r--   0        0        0      797 2023-04-27 18:43:36.665809 garden_ai-0.4.0/README.md
--rw-r--r--   0        0        0      391 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/__init__.py
--rw-r--r--   0        0        0       54 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/__main__.py
--rw-r--r--   0        0        0        0 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/app/__init__.py
--rw-r--r--   0        0        0       54 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/app/console.py
--rw-r--r--   0        0        0     9616 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/app/garden.py
--rw-r--r--   0        0        0      484 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/app/main.py
--rw-r--r--   0        0        0     1881 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/app/model.py
--rw-r--r--   0        0        0     7757 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/app/pipeline.py
--rw-r--r--   0        0        0    15473 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/client.py
--rw-r--r--   0        0        0     9398 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/datacite.py
--rw-r--r--   0        0        0        0 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/funcx_bandaid/__init__.py
--rw-r--r--   0        0        0     1247 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/funcx_bandaid/serialization_patch.py
--rw-r--r--   0        0        0     9691 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/gardens.py
--rw-r--r--   0        0        0        0 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/globus_compute/__init__.py
--rw-r--r--   0        0        0     2803 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/globus_compute/containers.py
--rw-r--r--   0        0        0     1451 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/globus_compute/login_manager.py
--rw-r--r--   0        0        0      801 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/globus_compute/remote_functions.py
--rw-r--r--   0        0        0     6244 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/local_data.py
--rw-r--r--   0        0        0        0 2023-04-27 18:43:36.665809 garden_ai-0.4.0/garden_ai/mlflow_bandaid/__init__.py
--rw-r--r--   0        0        0     1064 2023-04-27 18:43:36.669809 garden_ai-0.4.0/garden_ai/mlflow_bandaid/binary_header_provider.py
--rw-r--r--   0        0        0     7053 2023-04-27 18:43:36.669809 garden_ai-0.4.0/garden_ai/mlmodel.py
--rw-r--r--   0        0        0    13740 2023-04-27 18:43:36.669809 garden_ai-0.4.0/garden_ai/pipelines.py
--rw-r--r--   0        0        0    11675 2023-04-27 18:43:36.669809 garden_ai-0.4.0/garden_ai/steps.py
--rw-r--r--   0        0        0     2016 2023-04-27 18:43:36.669809 garden_ai-0.4.0/garden_ai/templates/pipeline
--rw-r--r--   0        0        0        0 2023-04-27 18:43:36.669809 garden_ai-0.4.0/garden_ai/utils/__init__.py
--rw-r--r--   0        0        0     1160 2023-04-27 18:43:36.669809 garden_ai-0.4.0/garden_ai/utils/filesystem.py
--rw-r--r--   0        0        0    10634 2023-04-27 18:43:36.669809 garden_ai-0.4.0/garden_ai/utils/misc.py
--rw-r--r--   0        0        0      136 2023-04-27 18:43:36.669809 garden_ai-0.4.0/garden_ai/version.py
--rw-r--r--   0        0        0     2429 2023-04-27 18:43:53.589881 garden_ai-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2205 1970-01-01 00:00:00.000000 garden_ai-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-15 16:28:06.427582 garden_ai-0.4.1/LICENSE
+-rw-r--r--   0        0        0      797 2023-05-15 16:28:06.431582 garden_ai-0.4.1/README.md
+-rw-r--r--   0        0        0      356 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/__init__.py
+-rw-r--r--   0        0        0       54 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/__main__.py
+-rw-r--r--   0        0        0       97 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/_version.py
+-rw-r--r--   0        0        0        0 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/app/__init__.py
+-rw-r--r--   0        0        0       54 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/app/console.py
+-rw-r--r--   0        0        0    10478 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/app/garden.py
+-rw-r--r--   0        0        0      828 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/app/main.py
+-rw-r--r--   0        0        0     3076 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/app/model.py
+-rw-r--r--   0        0        0     6862 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/app/pipeline.py
+-rw-r--r--   0        0        0    17674 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/client.py
+-rw-r--r--   0        0        0     9398 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/datacite.py
+-rw-r--r--   0        0        0        0 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/funcx_bandaid/__init__.py
+-rw-r--r--   0        0        0     1247 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/funcx_bandaid/serialization_patch.py
+-rw-r--r--   0        0        0    12872 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/gardens.py
+-rw-r--r--   0        0        0        0 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/globus_compute/__init__.py
+-rw-r--r--   0        0        0     2803 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/globus_compute/containers.py
+-rw-r--r--   0        0        0     1451 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/globus_compute/login_manager.py
+-rw-r--r--   0        0        0      801 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/globus_compute/remote_functions.py
+-rw-r--r--   0        0        0        0 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/globus_search/__init__.py
+-rw-r--r--   0        0        0     3011 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/globus_search/garden_search.py
+-rw-r--r--   0        0        0     7498 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/local_data.py
+-rw-r--r--   0        0        0        0 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/mlflow_bandaid/__init__.py
+-rw-r--r--   0        0        0     1064 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/mlflow_bandaid/binary_header_provider.py
+-rw-r--r--   0        0        0     9999 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/mlmodel.py
+-rw-r--r--   0        0        0    15864 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/pipelines.py
+-rw-r--r--   0        0        0    11963 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/steps.py
+-rw-r--r--   0        0        0     2017 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/templates/pipeline
+-rw-r--r--   0        0        0        0 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/utils/__init__.py
+-rw-r--r--   0        0        0     1241 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/utils/filesystem.py
+-rw-r--r--   0        0        0    11588 2023-05-15 16:28:06.431582 garden_ai-0.4.1/garden_ai/utils/misc.py
+-rw-r--r--   0        0        0     2784 2023-05-15 16:28:20.635941 garden_ai-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2384 1970-01-01 00:00:00.000000 garden_ai-0.4.1/PKG-INFO
```

### Comparing `garden_ai-0.4.0/LICENSE` & `garden_ai-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.0/README.md` & `garden_ai-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.0/garden_ai/app/garden.py` & `garden_ai-0.4.1/garden_ai/app/garden.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 
 import rich
 import typer
 from globus_sdk import SearchAPIError
 from rich.prompt import Prompt
 
 from garden_ai import local_data
-from garden_ai.client import GardenClient, GARDEN_INDEX_UUID
+from garden_ai.client import GardenClient
+from garden_ai.globus_search.garden_search import GARDEN_INDEX_UUID
 from garden_ai.gardens import Garden
 from garden_ai.pipelines import RegisteredPipeline
 
 logger = logging.getLogger()
 
 garden_app = typer.Typer(name="garden", no_args_is_help=True)
 
@@ -226,46 +227,65 @@
         ...,
         "-p",
         "--pipeline",
         prompt="Please enter a the UUID or DOI of a pipeline",
         help="The name of the pipeline you want to add",
         rich_help_panel="Required",
     ),
+    pipeline_alias: Optional[str] = typer.Option(
+        None,
+        "-a",
+        "--alias",
+        help=(
+            'Alternate short_name to use when calling this pipeline as a "method" of the'
+            "garden, e.g. ``my_garden.alias(args, endpoint=...)``. Defaults to the variable"
+            "name used when the pipeline was first registered."
+        ),
+    ),
 ):
     """Add a registered pipeline to a garden"""
 
     garden = _get_garden(garden_id)
     to_add = _get_pipeline(pipeline_id)
 
-    if to_add in garden.collect_pipelines():
-        logger.info(f"Pipeline {pipeline_id} is already in Garden {garden_id}")
-        return
-
-    garden.pipeline_ids += [to_add.uuid]
+    if to_add in garden.pipelines:
+        if pipeline_alias:
+            old_name = (
+                garden.pipeline_aliases.get(to_add.short_name) or to_add.short_name
+            )
+            print(
+                f"Pipeline {pipeline_id} is already in Garden {garden_id} as {old_name}. Renaming to {pipeline_alias}."
+            )
+            garden.rename_pipeline(old_name, pipeline_alias)
+    else:
+        garden.pipeline_ids += [to_add.uuid]
+        if pipeline_alias:
+            garden.rename_pipeline(to_add.short_name, pipeline_alias)
     local_data.put_local_garden(garden)
     logger.info(f"Added pipeline {pipeline_id} to Garden {garden_id}")
 
 
 @garden_app.command(no_args_is_help=True)
 def publish(
     garden_id: str = typer.Option(
         ...,
         "-g",
         "--garden",
         prompt="Please enter the UUID or DOI of a garden",
-        help="The name of the garden you want to add a pipeline to",
+        help="The UUID or DOI of the garden you want to publish",
         rich_help_panel="Required",
     ),
 ):
     """Push data about a Garden stored to Globus Search so that other users can search for it"""
 
     client = GardenClient()
     garden = _get_garden(garden_id)
-    garden.doi = client._mint_doi(garden)
-
+    if not garden.doi:
+        garden.doi = client._mint_doi(garden)
+        local_data.put_local_garden(garden)
     try:
         client.publish_garden_metadata(garden)
     except SearchAPIError as e:
         logger.fatal(f"Could not publish garden {garden_id}")
         logger.fatal(e.error_data)
         raise typer.Exit(code=1) from e
```

### Comparing `garden_ai-0.4.0/garden_ai/app/model.py` & `garden_ai-0.4.1/garden_ai/app/model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from pathlib import Path
 from typing import Optional, List
 
 from garden_ai.client import GardenClient
+from garden_ai.mlmodel import DatasetConnection, LocalModel, ModelFlavor
 
 import typer
 import rich
 
 model_app = typer.Typer(name="model", no_args_is_help=True)
 
 
@@ -45,21 +46,53 @@
         "--extra-pip-requirements",
         "-r",
         help=(
             "Additonal package requirmeents. Add multiple like "
             '--extra-pip-requirements "torch=1.3.1" --extra-pip-requirements "pandas<=1.5.0"'
         ),
     ),
+    dataset_url: Optional[str] = typer.Option(
+        None,
+        "--dataset-url",
+        help=(
+            "If you trained this model on a Foundry dataset, include a link to the dataset with this option"
+        ),
+    ),
+    dataset_doi: Optional[str] = typer.Option(
+        None,
+        "--dataset-doi",
+        help=(
+            "If you trained this model on a Foundry dataset, include the doi of the dataset"
+        ),
+    ),
 ):
     """Register a model in Garden. Outputs a full model identifier that you can reference in a Pipeline."""
-    if flavor not in ["sklearn", "tensorflow", "pytorch"]:
+    if flavor not in [f.value for f in ModelFlavor]:
         raise typer.BadParameter(
             f"Sorry, we only support 'sklearn', 'tensorflow', and 'pytorch'. The {flavor} flavor is not yet supported."
         )
 
+    only_one_dataset_option_provided = (dataset_url and not dataset_doi) or (
+        dataset_doi and not dataset_url
+    )
+    if only_one_dataset_option_provided:
+        raise typer.BadParameter(
+            "If you are linking a Foundry dataset, please include both --dataset-url and --dataset-doi"
+        )
+
     client = GardenClient()
-    full_model_name = client.log_model(
-        str(model_path), name, flavor, extra_pip_requirements
+    local_model = LocalModel(
+        local_path=str(model_path),
+        model_name=name,
+        flavor=flavor,
+        extra_pip_requirements=extra_pip_requirements,
+        user_email=client.get_email(),
     )
+    if dataset_doi and dataset_url:
+        dataset_metadata = DatasetConnection(doi=dataset_doi, url=dataset_url)
+        local_model.connections.append(dataset_metadata)
+
+    registered_model = client.register_model(local_model)
+    model_uri = registered_model.model_uri
     rich.print(
-        f"Successfully uploaded your model! The full name to include in your pipeline is '{full_model_name}'"
+        f"Successfully uploaded your model! The full name to include in your pipeline is '{model_uri}'"
     )
```

### Comparing `garden_ai-0.4.0/garden_ai/app/pipeline.py` & `garden_ai-0.4.1/garden_ai/app/pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import logging
-import re
 from datetime import datetime
-from keyword import iskeyword
 from pathlib import Path
 from typing import List, Optional
 
 import jinja2
 import typer
 from rich import print
 from rich.prompt import Prompt
@@ -13,90 +11,60 @@
 from garden_ai import GardenClient, Pipeline, step
 from garden_ai.app.console import console
 
 from garden_ai.utils.filesystem import (
     load_pipeline_from_python_file,
     PipelineLoadException,
 )
+from garden_ai.utils.misc import clean_identifier
 
 logger = logging.getLogger()
 
 pipeline_app = typer.Typer(name="pipeline", no_args_is_help=True)
 
 
-def clean_identifier(name: str) -> str:
-    """Clean the name provided for use as a pipeline's python identifier."""
-    orig = name
-    # Remove invalid characters, replacing with _
-    name = re.sub("[^0-9a-zA-Z_]", "_", name)
-
-    # Remove leading characters until we find a letter
-    name = re.sub("^[^a-zA-Z]+", "", name)
-
-    # Remove doubled/trailing underscores
-    name = re.sub("__+", "_", name).rstrip("_")
-
-    if not name:
-        # name consisted only of invalid characters
-        raise typer.BadParameter(
-            "Invalid shortname. This argument should contain a valid python identifier"
-            "(i.e. something usable as a variable name)."
-        )
-
-    # truncate to sane length, though not strictly necessary
-    name = name[:50]
-
-    if iskeyword(name):
-        name += "_"
-
-    if name != orig:
-        print(f'Generated valid shortname "{name}" from "{orig}".')
-
-    return name
-
-
 def parse_full_name(name: str) -> str:
     """(this will probably eventually use some 3rd party name parsing library)"""
     return name.strip() if name else ""
 
 
-def template_pipeline(shortname: str, pipeline: Pipeline) -> str:
+def template_pipeline(short_name: str, pipeline: Pipeline) -> str:
     """populate jinja2 template with starter code for creating a pipeline"""
     env = jinja2.Environment(loader=jinja2.PackageLoader("garden_ai"))
     template = env.get_template("pipeline")
-    return template.render(shortname=shortname, pipeline=pipeline)
+    return template.render(short_name=short_name, pipeline=pipeline)
 
 
 @pipeline_app.callback()
 def pipeline():
     """
     sub-commands for creating and manipulating Pipelines
     """
     pass
 
 
 @pipeline_app.command(no_args_is_help=True)
 def create(
-    shortname: str = typer.Argument(
+    short_name: str = typer.Argument(
         None,
         help=(
             "A valid python identifier (i.e. variable name) for the new pipeline. "
             "If not provided, one will be generated from your pipeline's title. "
-            "a [shortname].py file will be templated for your pipeline code. "
+            "a [short_name].py file will be templated for your pipeline code. "
         ),
     ),
     directory: Path = typer.Option(
         Path.cwd(),
         dir_okay=True,
         file_okay=False,
         writable=True,
         readable=True,
         resolve_path=True,
         help=(
-            "(Optional) if specified, target directory in which to generate the templated [shortname].py file. "
+            "(Optional) if specified, target directory in which to generate the templated [short_name].py file. "
             "Defaults to current directory."
         ),
     ),
     title: str = typer.Option(
         ...,
         "-t",
         "--title",
@@ -147,15 +115,15 @@
     ),
     verbose: bool = typer.Option(
         False, help="If true, pretty-print Pipeline's metadata when created."
     ),
 ):
     """Scaffold a new pipeline"""
 
-    shortname = clean_identifier(shortname or title)
+    short_name = clean_identifier(short_name or title)
 
     while not authors:
         # repeatedly prompt for at least one author until one is given
         name = parse_full_name(
             Prompt.ask("Please enter at least one author (required)")
         )
         if not name:
@@ -191,22 +159,22 @@
         steps=[dummy_step],  # type: ignore
         tags=tags,
         description=description,
         year=year,
     )
 
     # template file
-    out_dir = Path(directory / shortname)
+    out_dir = Path(directory / short_name)
     if out_dir.exists():
-        logger.fatal(f"Error: {directory / shortname} already exists.")
+        logger.fatal(f"Error: {directory / short_name} already exists.")
         raise typer.Exit(code=1)
     else:
         out_dir.mkdir(parents=True)
         out_file = out_dir / "pipeline.py"
-        contents = template_pipeline(shortname, pipeline)
+        contents = template_pipeline(short_name, pipeline)
         with open(out_file, "w") as f:
             f.write(contents)
         with open(out_dir / "requirements.txt", "w") as f:
             f.write("## Please specify all pipeline dependencies here\n")
 
         print(f"Generated pipeline scaffolding in {out_dir}.")
```

### Comparing `garden_ai-0.4.0/garden_ai/client.py` & `garden_ai-0.4.1/garden_ai/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,36 +13,38 @@
 from globus_sdk import (
     AuthAPIError,
     AuthClient,
     GroupsClient,
     NativeAppAuthClient,
     RefreshTokenAuthorizer,
     SearchClient,
+    GlobusHTTPResponse,
 )
 from globus_sdk.scopes import AuthScopes, ScopeBuilder, SearchScopes
 from globus_sdk.tokenstorage import SimpleJSONFileAdapter
 from mlflow.tracking.request_header.registry import _request_header_provider_registry
 from rich import print
 from rich.prompt import Prompt
 
 import garden_ai.funcx_bandaid.serialization_patch  # type: ignore # noqa: F401
 from garden_ai import local_data
-from garden_ai.gardens import Garden, PipelineNotFoundException
+from garden_ai.gardens import Garden
 from garden_ai.globus_compute.containers import build_container
 from garden_ai.globus_compute.login_manager import ComputeLoginManager
 from garden_ai.globus_compute.remote_functions import register_pipeline
+from garden_ai.globus_search import garden_search
+
+from garden_ai.local_data import GardenNotFoundException, PipelineNotFoundException
 from garden_ai.mlflow_bandaid.binary_header_provider import (
     BinaryContentTypeHeaderProvider,
 )
-from garden_ai.mlmodel import upload_model
+from garden_ai.mlmodel import LocalModel, RegisteredModel, upload_to_model_registry
 from garden_ai.pipelines import Pipeline, RegisteredPipeline
 from garden_ai.utils.misc import extract_email_from_globus_jwt
 
-# garden-dev index
-GARDEN_INDEX_UUID = "58e4df29-4492-4e7d-9317-b27eba62a911"
 GARDEN_ENDPOINT = os.environ.get(
     "GARDEN_ENDPOINT",
     "https://nu3cetwc84.execute-api.us-east-1.amazonaws.com/garden_prod",
 )
 
 COMPUTE_RESOURCE_SERVER_NAME = "funcx_service"
 
@@ -126,16 +128,15 @@
 
     def _do_login_flow(self):
         self.auth_client.oauth2_start_flow(
             requested_scopes=[
                 AuthClient.scopes.openid,
                 AuthClient.scopes.email,
                 GroupsClient.scopes.view_my_groups_and_memberships,
-                SearchClient.scopes.ingest,
-                SearchClient.scopes.search,
+                SearchClient.scopes.all,
                 GardenClient.scopes.action_all,
                 Client.FUNCX_SCOPE,
             ],
             refresh_tokens=True,
         )
         authorize_url = self.auth_client.oauth2_get_authorize_url()
 
@@ -254,30 +255,18 @@
         record = local_data.get_local_pipeline_by_uuid(pipeline.uuid)
         if record:
             logger.info("Found pre-registered pipeline. Reusing DOI.")
             pipeline.doi = record.doi
 
         return pipeline
 
-    def log_model(
-        self,
-        model_path: str,
-        model_name: str,
-        flavor: str,
-        extra_pip_requirements: List[str] = None,
-    ) -> str:
-        email = local_data._get_user_email()
-        full_model_name = upload_model(
-            model_path,
-            model_name,
-            email,
-            flavor,
-            extra_pip_requirements=extra_pip_requirements,
-        )
-        return full_model_name
+    def register_model(self, local_model: LocalModel) -> RegisteredModel:
+        registered_model = upload_to_model_registry(local_model)
+        local_data.put_local_model(registered_model)
+        return registered_model
 
     def _mint_doi(
         self, obj: Union[Garden, Pipeline], force: bool = False, test: bool = True
     ) -> str:
         """Register a new "findable" doi with DataCite via Garden backend.
 
         Expects environment variable GARDEN_ENDPOINT to be set (not including `/doi`).
@@ -396,31 +385,94 @@
         registered._env_vars = {
             "MLFLOW_TRACKING_TOKEN": os.environ["MLFLOW_TRACKING_TOKEN"],
             "MLFLOW_TRACKING_URI": os.environ["MLFLOW_TRACKING_URI"],
         }
 
         return registered
 
-    def publish_garden_metadata(self, garden: Garden):
-        # Takes a garden, and publishes to the GARDEN_INDEX_UUID index.  Polls
-        # to discover status, and returns the Task document:
-        # https://docs.globus.org/api/search/reference/get_task/#task
-        garden_meta = json.loads(garden.expanded_json())
-        gmeta_ingest = {
-            "subject": garden_meta["uuid"],
-            "visible_to": ["all_authenticated_users"],
-            "content": garden_meta,
+    def _fresh_mlflow_vars(self):
+        self._set_up_mlflow_env()
+        return {
+            "MLFLOW_TRACKING_TOKEN": os.environ["MLFLOW_TRACKING_TOKEN"],
+            "MLFLOW_TRACKING_URI": os.environ["MLFLOW_TRACKING_URI"],
         }
 
-        publish_result = self.search_client.create_entry(
-            GARDEN_INDEX_UUID, gmeta_ingest
-        )
+    def get_email(self) -> str:
+        return local_data._get_user_email()
+
+    def get_local_garden(self, identifier: Union[UUID, str]) -> Garden:
+        """Return a registered ``Garden`` corresponding to the given uuid/doi.
+
+        Any ``RegisteredPipelines`` registered to the Garden will be callable
+        as attributes on the garden by their (registered) short_name, e.g.
+            ```python
+                my_garden = client.get_local_garden('garden-doi-or-uuid')
+                #  pipeline would have been registered with short_name='my_pipeline'
+                my_garden.my_pipeline(*args, endpoint='where-to-execute')
+            ```
+        Tip: To access the pipeline by a different name, use ``my_garden.rename_pipeline(old_name, new_name)``.
+        To persist a new name for a pipeline, re-register it to the garden and specify an alias.
+
+        Parameters
+        ----------
+        identifier : Union[UUID, str]
+            The previously registered Garden's DOI or UUID. Raises an
+            exception if not found.
+
+        """
+        is_doi = "/" in str(identifier)
+        if is_doi:
+            registered = local_data.get_local_garden_by_doi(str(identifier))
+        else:
+            registered = local_data.get_local_garden_by_uuid(identifier)
+
+        if registered is None:
+            raise GardenNotFoundException(
+                f"Could not find any Gardens with identifier {identifier}."
+            )
+        self._set_up_mlflow_env()
+        registered._env_vars = {
+            "MLFLOW_TRACKING_TOKEN": os.environ["MLFLOW_TRACKING_TOKEN"],
+            "MLFLOW_TRACKING_URI": os.environ["MLFLOW_TRACKING_URI"],
+        }
+        return registered
 
-        task_result = self.search_client.get_task(publish_result["task_id"])
-        while not task_result["state"] in {"FAILED", "SUCCESS"}:
-            time.sleep(5)
-            task_result = self.search_client.get_task(publish_result["task_id"])
-        return task_result
+    def publish_garden_metadata(self, garden: Garden) -> GlobusHTTPResponse:
+        """
+        Takes a garden, and publishes to the GARDEN_INDEX_UUID index.  Polls
+        to discover status, and returns the Task document.
+        Task document has a task["state"] field that can be FAILED or SUCCESS.
+
+        Returns
+        -------
+        https://docs.globus.org/api/search/reference/get_task/#task
+        """
+        return garden_search.publish_garden_metadata(garden, self.search_client)
 
     def search(self, query: str) -> str:
-        res = self.search_client.search(GARDEN_INDEX_UUID, query, advanced=True)
-        return res.text
+        """
+        Given a Globus Search advanced query, returns JSON Globus Search result string with gardens as entries.
+        """
+        return garden_search.search_gardens(query, self.search_client)
+
+    def get_published_garden(self, identifier: str) -> Garden:
+        """
+        Queries Globus Search for the garden with this DOI.
+
+        Parameters
+        ----------
+        identifier: The doi or uuid of the garden you want.
+
+        Returns
+        -------
+        Garden populated with metadata from remote metadata record.
+
+        """
+        is_doi = "/" in str(identifier)
+        if is_doi:
+            return garden_search.get_remote_garden_by_doi(
+                identifier, self._fresh_mlflow_vars(), self.search_client
+            )
+        else:
+            return garden_search.get_remote_garden_by_uuid(
+                identifier, self._fresh_mlflow_vars(), self.search_client
+            )
```

### Comparing `garden_ai-0.4.0/garden_ai/datacite.py` & `garden_ai-0.4.1/garden_ai/datacite.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.0/garden_ai/funcx_bandaid/serialization_patch.py` & `garden_ai-0.4.1/garden_ai/funcx_bandaid/serialization_patch.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.0/garden_ai/gardens.py` & `garden_ai-0.4.1/garden_ai/gardens.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import json
 import logging
 from datetime import datetime
 from typing import Any, Dict, List, Optional, cast
 from uuid import UUID, uuid4
 
-from pydantic import BaseModel, Field, ValidationError, validator
+from pydantic import BaseModel, Field, PrivateAttr, ValidationError, validator
 
 from garden_ai.utils.misc import JSON, garden_json_encoder
 
 from .datacite import (
     Contributor,
     Creator,
     DataciteSchema,
@@ -20,18 +20,14 @@
     Types,
 )
 from .pipelines import RegisteredPipeline
 
 logger = logging.getLogger()
 
 
-class PipelineNotFoundException(KeyError):
-    """Exception raised when a Garden references an unknown pipeline uuid"""
-
-
 class Garden(BaseModel):
     """Object representation of a Garden™.
 
     Required Attributes
     --------------------
     authors: List[str]
         The main researchers involved in producing the Garden. At least one
@@ -112,33 +108,91 @@
     publisher: str = "Garden"
     year: str = Field(default_factory=lambda: str(datetime.now().year))
     language: str = "en"
     tags: List[str] = Field(default_factory=list, unique_items=True)
     version: str = "0.0.1"
     uuid: UUID = Field(default_factory=uuid4, allow_mutation=False)
     pipeline_ids: List[UUID] = Field(default_factory=list)
+    pipeline_aliases: Dict[str, str] = Field(default_factory=dict)
+    _pipelines: List[RegisteredPipeline] = PrivateAttr(default_factory=list)
+    _env_vars: Dict[str, str] = PrivateAttr(default_factory=dict)
 
     @validator("year")
     def valid_year(cls, year):
         if len(str(year)) != 4:
             raise ValueError("year must be formatted `YYYY`")
         return str(year)
 
-    def collect_pipelines(self) -> List[RegisteredPipeline]:
-        """Collect the full ``RegisteredPipeline`` objects referred to by this garden's pipeline_ids."""
-        from .local_data import get_local_pipeline_by_uuid
+    @property
+    def pipelines(self) -> List[RegisteredPipeline]:
+        """Read-only list of the pipelines registered to a garden.
+
+        Note that these pipelines can also be accessed from the garden as attributes,
+        according to their short_name -- see also ``rename_pipeline``.
+        """
+        if not self._pipelines:
+            self._pipelines = self._collect_pipelines()
+        return self._pipelines
+
+    @property
+    def pipeline_names(self) -> List[str]:
+        """Read-only list of short_names of pipelines registered to a garden."""
+        names = []
+        for pipeline in self.pipelines:
+            name = self.pipeline_aliases.get(pipeline.short_name) or pipeline.short_name
+            names += [name]
+        return names
+
+    def _set_pipelines_from_remote_metadata(self, pipeline_metadata: List[dict]):
+        """
+        Given a list of dicts in RegisteredPipeline format (as from Globus Search),
+        attempt to convert them to RegisteredPipelines and use them to populate _pipelines.
+        """
+        pipelines = []
+        for meta in pipeline_metadata:
+            try:
+                pipeline = RegisteredPipeline(**meta)
+                if pipeline.uuid in self.pipeline_ids:
+                    pipeline._env_vars = self._env_vars
+                    pipelines.append(pipeline)
+                else:
+                    logger.warning(
+                        f"Remote pipeline {pipeline.uuid} not present in pipeline id list."
+                    )
+            except ValidationError as e:
+                logger.warning(
+                    f"Could not parse pipeline: {json.dumps(meta)}. {e.__str__()}"
+                )
+
+        self._pipelines = pipelines
+
+    def _collect_pipelines(self) -> List[RegisteredPipeline]:
+        """
+        Collect the pipeline objects which have been registered to this garden from local database.
+
+        Note: prefer the ``garden.pipelines` computed property to avoid running this many times.
+
+        Returns
+        -------
+        List[RegisteredPipeline]
+        """
+        from .local_data import PipelineNotFoundException, get_local_pipeline_by_uuid
 
         pipelines = []
         for uuid in self.pipeline_ids:
             pipeline = get_local_pipeline_by_uuid(uuid)
             if pipeline is None:
                 raise PipelineNotFoundException(
                     f"Could not find registered pipeline with id {uuid}."
                 )
+            # set env vars for pipeline to use when remotely executing
+            pipeline._env_vars = self._env_vars
+
             pipelines += [pipeline]
+
         return pipelines
 
     def expanded_metadata(self) -> Dict[str, Any]:
         """Helper: build the "complete" metadata dict with nested ``Pipeline`` and ``step`` metadata.
 
         Notes
         ------
@@ -155,15 +209,15 @@
 
         Raises
         ------
         PipelineNotFoundException  if ``garden.pipeline_ids`` references an unknown pipeline id.
         """
 
         data = self.dict()
-        data["pipelines"] = [p.dict() for p in self.collect_pipelines()]
+        data["pipelines"] = [p.expanded_metadata() for p in self.pipelines]
         return data
 
     def expanded_json(self) -> JSON:
         """Helper: return the expanded garden metadata as JSON.
 
         See: ``Garden.expanded_metadata`` method
         """
@@ -192,15 +246,15 @@
             language=self.language,
             relatedIdentifiers=[
                 RelatedIdentifier(
                     relatedIdentifier=p.doi,
                     relatedIdentifierType="DOI",
                     relationType="HasPart",
                 )
-                for p in self.collect_pipelines()
+                for p in self.pipelines
             ],
             version=self.version,
             descriptions=[
                 Description(description=self.description, descriptionType="Other")
             ]
             if self.description
             else None,
@@ -211,15 +265,15 @@
 
         This is useful for catching fields with a default value which would not
         otherwise be valid, (e.g.  `None` for any required field), in particular
         as a sanity check before committing to publishing/registering the user's
         Garden.
 
         This is mostly redundant for any already-set fields, as the validators
-        for those would have (hopefully) already run when they were set. However
+        for those would have (hopefully) already run when they were set. However,
         (because this is still python), it's relatively easy to *modify* some
         fields without ever *assigning* to them, which wouldn't trigger
         validation.
 
         Examples
         --------
         gc = GardenClient()
@@ -240,22 +294,49 @@
         try:
             _ = self.__class__(**self.dict())
         except ValidationError as err:
             logger.error(err)
             raise
 
     def _sync_author_metadata(self):
-        """helper: authors and contributors of steps and Pipelines also appear as contributors in their respective Pipeline and Garden's metadata.
-
-        We'll probably want to tweak the behavior of this at some point once we
-        tease out what we really want `contributor` to entail, but for now this
-        seems like a sane default.
-        """
+        """helper: authors and contributors of steps and Pipelines also appear as contributors in their respective Pipeline and Garden's metadata."""
         known_contributors = set(self.contributors)
         # garden contributors don't need to duplicate garden authors unless they've been explicitly added
         known_authors = set(self.authors) - known_contributors
-        for pipe in self.collect_pipelines():
-            new_contributors = set(pipe.authors) | set(pipe.contributors)
+
+        for pipeline in self.pipelines:
+            new_contributors = set(pipeline.authors) | set(pipeline.contributors)
             known_contributors |= new_contributors - known_authors
 
         self.contributors = list(known_contributors)
         return
+
+    def __getattr__(self, name):
+        #  note: this is only called as a fallback when __getattribute__ raises an exception,
+        #  existing attributes are not affected by overriding this
+        message_extra = ""
+        for pipeline in self.pipelines:
+            short_name = pipeline.short_name
+            alias = self.pipeline_aliases.get(short_name) or short_name
+            if name == alias:
+                return pipeline
+            elif name == short_name:
+                message_extra = f" Did you mean {alias}?"
+
+        raise AttributeError(
+            f"'{self.__class__.__name__}' object has no attribute '{name}'."
+            + message_extra
+        )
+
+    def __dir__(self):
+        # this gets us jupyter/ipython/repl tab-completion of pipeline names
+        return list(super().__dir__()) + self.pipeline_names
+
+    def rename_pipeline(self, old_name: str, new_name: str):
+        if hasattr(self, new_name):
+            raise ValueError(
+                f"Error: found existing {new_name} attribute on this garden."
+            )
+        if not new_name.isidentifier():
+            raise ValueError("new_name must be a valid identifier.")
+        self.pipeline_aliases[old_name] = new_name
+        return
```

### Comparing `garden_ai-0.4.0/garden_ai/globus_compute/containers.py` & `garden_ai-0.4.1/garden_ai/globus_compute/containers.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.0/garden_ai/globus_compute/login_manager.py` & `garden_ai-0.4.1/garden_ai/globus_compute/login_manager.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.0/garden_ai/globus_compute/remote_functions.py` & `garden_ai-0.4.1/garden_ai/globus_compute/remote_functions.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.0/garden_ai/mlflow_bandaid/binary_header_provider.py` & `garden_ai-0.4.1/garden_ai/mlflow_bandaid/binary_header_provider.py`

 * *Files identical despite different names*

### Comparing `garden_ai-0.4.0/garden_ai/pipelines.py` & `garden_ai-0.4.1/garden_ai/pipelines.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import json
 import logging
 import pathlib
 import sys
 from datetime import datetime
 from functools import reduce
 from inspect import signature
+from keyword import iskeyword
 from typing import Any, Dict, List, Optional, Tuple, Union
 from uuid import UUID, uuid4
 
 import dparse  # type: ignore
 import globus_compute_sdk  # type: ignore
 from pydantic import BaseModel, Field, PrivateAttr, validator
 from pydantic.dataclasses import dataclass
@@ -20,22 +21,24 @@
     Contributor,
     Creator,
     DataciteSchema,
     Description,
     Title,
     Types,
 )
+from garden_ai.mlmodel import RegisteredModel
 from garden_ai.steps import DataclassConfig, Step
 from garden_ai.utils.misc import (
     JSON,
     garden_json_encoder,
     read_conda_deps,
     safe_compose,
     validate_pip_lines,
 )
+from garden_ai._version import __version__
 
 logger = logging.getLogger()
 
 
 @dataclass(config=DataclassConfig)
 class Pipeline:
     """
@@ -47,14 +50,15 @@
     next Step. The register method can be used to register
     each Step in the pipeline.
 
     Args:
     authors (List[str]): A list of the authors of the pipeline.
     title (str): The title of the pipeline.
     steps (List[Step]): A list of the steps in the pipeline.
+    model_uris (List[str]): A list of model uris used in the pipeline.
 
     """
 
     title: str = Field(...)
     authors: List[str] = Field(...)
     steps: Tuple[Step, ...] = Field(...)
     contributors: List[str] = Field(default_factory=list, unique_items=True)
@@ -63,29 +67,38 @@
     func_uuid: Optional[UUID] = Field(None)
     description: Optional[str] = Field(None)
     version: str = "0.0.1"
     year: str = Field(default_factory=lambda: str(datetime.now().year))
     tags: List[str] = Field(default_factory=list, unique_items=True)
     requirements_file: Optional[str] = Field(None)
     python_version: Optional[str] = Field(None)
-    pip_dependencies: List[str] = Field(default_factory=list)
+    pip_dependencies: List[str] = Field(default=[f"garden-ai=={__version__}"])
     conda_dependencies: List[str] = Field(default_factory=list)
+    model_uris: List[str] = Field(default_factory=list)
+    short_name: Optional[str] = Field(None)
 
     def _composed_steps(*args, **kwargs):
         """ "This method intentionally left blank"
 
         We define this as a stub here, instead setting it as an attribute in
         `__post_init_post_parse__`, which is the earliest point after we
         validate that the steps are composable that we could modify the Pipeline
         object.
         This indirection is only necessary because `__call__` itself is looked
         up at the class level, so can't be set dynamically for different instances.
         """
         raise NotImplementedError
 
+    @validator("short_name")
+    def is_valid_identifier(cls, name: Optional[str]) -> Optional[str]:
+        if name:
+            assert name.isidentifier(), "short_name must be a valid python identifier"
+            assert not iskeyword(name), "short_name must not be a reserved keyword"
+        return name
+
     @validator("steps")
     def check_steps_composable(cls, steps):
         if len(steps) == 0:
             raise ValueError("Cannot have no steps in a pipeline.")
         try:
             reduce(safe_compose, reversed(steps))
         except TypeError as e:
@@ -123,15 +136,15 @@
                 "environment.yml/yaml."
             )
         return req_file
 
     def _collect_requirements(self):
         """collect requirements to pass to globus compute container service.
 
-        Populates attributes: ``self.python_version, self.pip_dependencies, self.conda_dependencies``
+        Populates attributes: ``self.python_version, self.pip_dependencies, self.conda_dependencies, self.model_uris``
         """
 
         # mapping of python-version-witness: python-version (collected for warning msg below)
         py_versions = {
             "system": ".".join(map(str, sys.version_info[:3])),
             "pipeline": self.python_version,
         }
@@ -154,14 +167,15 @@
                     deps = [d["line"] for d in parsed["dependencies"]]
                     deps.extend(d["line"] for d in parsed["resolved_dependencies"])
                     self.pip_dependencies += set(deps)
 
         for step in self.steps:
             self.conda_dependencies += step.conda_dependencies
             self.pip_dependencies += step.pip_dependencies
+            self.model_uris += step.model_uris
             py_versions[step.__name__] = step.python_version
 
         self.python_version = py_versions["pipeline"] or py_versions["system"]
         self.conda_dependencies = list(set(self.conda_dependencies))
         self.pip_dependencies = list(set(validate_pip_lines(self.pip_dependencies)))
 
         distinct_py_versions = set(
@@ -284,27 +298,28 @@
     Otherwise, all fields should be the same.
     """
 
     uuid: UUID = Field(...)
     doi: str = Field(...)
     func_uuid: Optional[UUID] = Field(...)
     title: str = Field(...)
+    short_name: str = Field(...)
     authors: List[str] = Field(...)
     # NOTE: steps are dicts here, not Step objects
     steps: List[Dict[str, Union[str, None, List]]] = Field(...)
     contributors: List[str] = Field(default_factory=list, unique_items=True)
     description: Optional[str] = Field(None)
     version: str = "0.0.1"
     year: str = Field(default_factory=lambda: str(datetime.now().year))
     tags: List[str] = Field(default_factory=list, unique_items=True)
-    # requirements_file: Optional[str] = Field(None)
     python_version: Optional[str] = Field(None)
     pip_dependencies: List[str] = Field(default_factory=list)
     conda_dependencies: List[str] = Field(default_factory=list)
     _env_vars: Dict[str, str] = PrivateAttr(default_factory=dict)
+    model_uris: List[str] = Field(default_factory=list)
 
     def __call__(
         self,
         *args: Any,
         endpoint: Union[UUID, str] = None,
         timeout=None,
         **kwargs: Any,
@@ -364,7 +379,44 @@
     def from_pipeline(cls, pipeline: Pipeline) -> RegisteredPipeline:
         # note: we want every RegisteredPipeline to be re-constructible
         # from mere json, so as a sanity check we use pipeline.json() instead of
         # pipeline.dict() directly
         record = pipeline.json()
         data = json.loads(record)
         return cls(**data)
+
+    def collect_models(self) -> List[RegisteredModel]:
+        """Collect the RegisteredModel objects that are present in the local DB"""
+        from .local_data import get_local_model_by_uri
+
+        models = []
+        for uri in self.model_uris:
+            model = get_local_model_by_uri(uri)
+            if model:
+                models += [model]
+            else:
+                logger.warning(
+                    f"No record in local database for model {uri}. "
+                    "Published garden will not have detailed metadata for that model."
+                )
+        return models
+
+    def expanded_metadata(self) -> Dict[str, Any]:
+        """Helper: build the "complete" metadata dict with nested ``Model`` metadata.
+
+        Notes
+        ------
+        When serializing normally with ``registered_pipeline.{dict(), json()}``, only the
+        uris of the models in the pipeline are included.
+
+        This returns a superset of ``registered_pipeline.dict()``, so that the following holds:
+
+            pipeline == Registered_Pipeline(**pipeline.expanded_metadata()) == Registered_Pipeline(**pipeline.dict())
+
+        Returns
+        -------
+        Dict[str, Any]  ``RegisteredPipeline`` metadata dict augmented with a list of ``RegisteredModel`` metadata
+        """
+
+        data = self.dict()
+        data["models"] = [m.dict() for m in self.collect_models()]
+        return data
```

### Comparing `garden_ai-0.4.0/garden_ai/steps.py` & `garden_ai-0.4.1/garden_ai/steps.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,14 +77,18 @@
         default.
 
 
     authors: List[str]
         The main researchers involved in producing the Step, for citation and discoverability
         purposes.
 
+    model_uris: List[str]
+        A reference to the models used in this step, if any.
+        Model identifiers as stored in MLFlow (not including the 'models:/' prefix).
+
     uuid: UUID
         short for "uuid"
 
     Raises
     ------
     TypeError
         If ``func`` has any arguments without annotations, is missing a return
@@ -120,14 +124,15 @@
     title: Optional[str] = Field(None)
     description: Optional[str] = Field(None)
     input_info: Optional[str] = Field(None)
     output_info: Optional[str] = Field(None)
     conda_dependencies: List[str] = Field(default_factory=list)
     pip_dependencies: List[str] = Field(default_factory=list)
     python_version: Optional[str] = Field(None)
+    model_uris: List[str] = Field(default_factory=list)
 
     def __post_init_post_parse__(self):
         # like __post_init__, but called after pydantic validation
         # copies e.g. __doc__ and __name__ from
         # the underlying callable to this object
         # (also handy for signature/annotations)
         update_wrapper(self, self.func)
@@ -157,14 +162,15 @@
         sig = signature(self.func)
         for param in sig.parameters.values():
             if isinstance(param.default, _Model):
                 model = param.default
                 self.python_version = model.python_version
                 self.conda_dependencies += model.conda_dependencies
                 self.pip_dependencies += model.pip_dependencies
+                self.model_uris += [model.model_full_name]
         return
 
     @validator("func")
     def has_annotations(cls, f: Callable):
         sig = signature(f)
         # check that any positional arguments have annotations
         for p in sig.parameters.values():
```

### Comparing `garden_ai-0.4.0/garden_ai/templates/pipeline` & `garden_ai-0.4.1/garden_ai/templates/pipeline`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 )
 
 REQUIREMENTS_FILE = None  # to specify additional dependencies, replace `None`
                           # with an "/absolute/path/to/requirements.txt"
 
 ################################### PIPELINE ####################################
 
-{{ shortname }}: Pipeline = client.create_pipeline(
+{{ short_name }}: Pipeline = client.create_pipeline(
     title="{{ pipeline.title }}",
     steps=ALL_STEPS,
     requirements_file=REQUIREMENTS_FILE,
     authors={{ pipeline.authors }},
     contributors={{ pipeline.contributors }},
     description="{{ pipeline.description }}",
     version="{{ pipeline.version }}",
```

### Comparing `garden_ai-0.4.0/garden_ai/utils/filesystem.py` & `garden_ai-0.4.1/garden_ai/utils/filesystem.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,10 +33,12 @@
         spec.loader.exec_module(module)
     except Exception as e:
         raise PipelineLoadException("Could not execute the Python code") from e
 
     for obj_name in dir(module):
         obj = getattr(module, obj_name)
         if isinstance(obj, Pipeline):
+            if obj.short_name is None:
+                obj.short_name = obj_name
             return obj
 
     raise PipelineLoadException(f"Could not find pipeline object in {python_file}")
```

### Comparing `garden_ai-0.4.0/garden_ai/utils/misc.py` & `garden_ai-0.4.1/garden_ai/utils/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import base64
 import json
 import logging
 import re
 import sys
+from functools import wraps
 from inspect import Parameter, Signature, signature
 from itertools import zip_longest
-from typing import List, Optional, Tuple, Callable
-from functools import wraps
+from keyword import iskeyword
+from typing import Callable, List, Optional, Tuple
 
 import beartype.door
 import requests
 import yaml
 from packaging.requirements import InvalidRequirement, Requirement
 from typing_extensions import TypeAlias
 
@@ -282,7 +283,38 @@
             import os
 
             for k, v in _env_vars.items():
                 os.environ[k] = v
         return func(*args, **kwargs)
 
     return inner
+
+
+def clean_identifier(name: str) -> str:
+    """Clean the name provided for use as a pipeline's python identifier."""
+    orig = name
+    # Remove invalid characters, replacing with _
+    name = re.sub("[^0-9a-zA-Z_]", "_", name)
+
+    # Remove leading characters until we find a letter
+    name = re.sub("^[^a-zA-Z]+", "", name)
+
+    # Remove doubled/trailing underscores
+    name = re.sub("__+", "_", name).strip("_")
+
+    if not name:
+        # name consisted only of invalid characters
+        raise ValueError(
+            "Invalid short_name. This argument should contain a valid python identifier "
+            "(i.e. something usable as a variable name)."
+        )
+
+    # truncate to sane length, though not strictly necessary
+    name = name[:50]
+
+    if iskeyword(name):
+        name += "_"
+
+    if name != orig:
+        logger.info(f'Generated valid short_name "{name}" from "{orig}".')
+
+    return name.lower()
```

### Comparing `garden_ai-0.4.0/pyproject.toml` & `garden_ai-0.4.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,86 +1,98 @@
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
 [tool.poetry]
 name = "garden-ai"
-version = "0.4.0"
+version = "0.4.1" # placeholder
 description = "Garden: tools to simplify access to scientific AI advances."
-authors = ["Your Name <you@example.com>"]
-license = "Apache-2.0"
+# note to contributors: feel free to add yourselves to this list 🌱
+maintainers = [
+  "Owen Price Skelly",
+  "Will Engler",
+  "Ben Blaiszik",
+  "Ben Galewsky",
+  "Eric Blau",
+  "Steve Barnard"
+]
+authors = [
+  "Garden Team <labs@globus.org>",
+]
+license = "MIT"
 readme = "README.md"
 include = ["templates"]
+homepage = "https://thegardens.ai"
+repository = "https://github.com/Garden-AI/garden"
+documentation = "https://garden-ai.readthedocs.io/en/latest/"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.20.0"
 globus-sdk = "^3.12.0"
 pydantic = "^1.10.2"
-typer = {extras = ["all"], version = "^0.7.0"}
+typer = { extras = ["all"], version = "^0.7.0" }
 beartype = "^0.12.0"
 jinja2 = "^3.1.2"
 mlflow = "2.2.1"
 # numba is an indirect dep of ML Flow.
 # Specifying a recent version of it helps avoid install issues on M1 Macs
 numba = "^0.56"
 boto3 = "^1.26.77"
-dparse = {extras = ["conda"], version = "^0.6.2"}
+dparse = { extras = ["conda"], version = "^0.6.2" }
 pyyaml = "^6.0"
 packaging = "^23.0"
 globus-compute-sdk = "^2.0.0"
 # Be sure to add additional flavors as optional below as support is added and update tool.poetry.extras
-torch = { version = "^2.0.0", optional = true}
+torch = { version = "^2.0.0", optional = true }
 tensorflow = { version = "^2.11.0", optional = true, python = ">=3.8,<3.12" }
 
 [tool.poetry.scripts]
 garden-ai = "garden_ai.app.main:app"
 
 [tool.poetry.group.test]
-optional=true
+optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.0"
 pytest-mock = "^3.10.0"
 pytest-cov = "^4.0.0"
 flake8 = "^5.0.4"
 mypy = "^0.981"
 types-requests = "^2.20.0"
 safety = "^2.3.1"
 types-pyyaml = "^6.0.12.8"
-torch = { version = "^2.0.0"}
+torch = { version = "^2.0.0" }
 tensorflow = { version = "^2.11.0", python = ">=3.8,<3.12" }
-coverage = {extras = ["toml"], version = "^7.2.3"}
-
-
+coverage = { extras = ["toml"], version = "^7.2.3" }
 
 [tool.poetry.group.develop.dependencies]
 sphinx = "4.3.2"
 sphinx-rtd-theme = "^1.0.0"
 pre-commit = "^3.1.1"
 black = "^23.1.0"
 isort = "^5.12.0"
 
+[tool.poetry.extras]
+# Be sure to add additional flavors to below as support is added and in the flavors array
+# Optional dependencies that can be added through `poetry install --extras "torch tensorflow"` etc. or `poetry install --extras "flavors"`
+# `poetry install --all-extras` will install all extras located in tool.poetry.extras
+torch = ["torch"]
+tensorflow = ["tensorflow"]
+flavors = ["tensorflow", "torch"]
+
 [tool.isort]
 profile = "black"
 
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
 [tool.mypy]
 plugins = ["pydantic.mypy"]
 exclude = "/fixtures/"
 
 [tool.pytest.ini_options]
 markers = [
-        "integration: deselect with '-m \"not integration\"' to run unit tests only.",
-        "cli: deselect with '-m \"not cli\"' to disable CLI tests."
+  "integration: deselect with '-m \"not integration\"' to run unit tests only.",
+  "cli: deselect with '-m \"not cli\"' to disable CLI tests."
 ]
 
-[tool.poetry.extras]
-# Be sure to add additional flavors to below as support is added and in the flavors array
-# Optional dependencies that can be added through `poetry install --extras "torch tensorflow"` etc. or `poetry install --extras "flavors"`
-# `poetry install --all-extras` will install all extras located in tool.poetry.extras
-torch = ["torch"]
-tensorflow = ["tensorflow"]
-flavors = ["tensorflow", "torch"]
-
 [tool.coverage.run]
 source = ["garden_ai/"]
 omit = ["garden_ai/templates/pipeline", "tests/"]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `garden_ai-0.4.0/PKG-INFO` & `garden_ai-0.4.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: garden-ai
-Version: 0.4.0
+Version: 0.4.1
 Summary: Garden: tools to simplify access to scientific AI advances.
-License: Apache-2.0
-Author: Your Name
-Author-email: you@example.com
+Home-page: https://thegardens.ai
+License: MIT
+Author: Garden Team
+Author-email: labs@globus.org
+Maintainer: Owen Price Skelly
 Requires-Python: >=3.8,<4.0
-Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: flavors
 Provides-Extra: tensorflow
@@ -26,14 +28,16 @@
 Requires-Dist: packaging (>=23.0,<24.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.20.0,<3.0.0)
 Requires-Dist: tensorflow (>=2.11.0,<3.0.0) ; (python_version >= "3.8" and python_version < "3.12") and (extra == "tensorflow" or extra == "flavors")
 Requires-Dist: torch (>=2.0.0,<3.0.0) ; extra == "torch" or extra == "flavors"
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
+Project-URL: Documentation, https://garden-ai.readthedocs.io/en/latest/
+Project-URL: Repository, https://github.com/Garden-AI/garden
 Description-Content-Type: text/markdown
 
 # Garden
 
 [![NSF-2209892](https://img.shields.io/badge/NSF-2209892-blue)](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2209892&HistoricalAwards=false)
 [![PyPI](https://badge.fury.io/py/garden-ai.svg)](https://badge.fury.io/py/garden-ai)
 [![Tests](https://github.com/Garden-AI/garden/actions/workflows/pypi.yaml/badge.svg)](https://github.com/Garden-AI/garden/actions/workflows/pypi.yaml)
```

