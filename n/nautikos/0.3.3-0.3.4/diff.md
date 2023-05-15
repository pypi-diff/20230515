# Comparing `tmp/nautikos-0.3.3.tar.gz` & `tmp/nautikos-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautikos-0.3.3.tar", max compression
+gzip compressed data, was "nautikos-0.3.4.tar", max compression
```

## Comparing `nautikos-0.3.3.tar` & `nautikos-0.3.4.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0        0 2023-03-21 07:42:17.427920 nautikos-0.3.3/nautikos/__init__.py
--rw-r--r--   0        0        0     1333 2023-04-11 15:12:06.664571 nautikos-0.3.3/nautikos/cli.py
--rw-r--r--   0        0        0     4171 2023-04-11 15:12:06.789634 nautikos-0.3.3/nautikos/manifests.py
--rw-r--r--   0        0        0     3214 2023-04-11 14:40:08.893216 nautikos-0.3.3/nautikos/nautikos.py
--rw-r--r--   0        0        0       80 2023-03-24 10:25:48.952431 nautikos-0.3.3/nautikos/yaml.py
--rw-r--r--   0        0        0     1292 2023-04-11 15:27:42.622480 nautikos-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     3758 2023-04-11 15:26:39.822743 nautikos-0.3.3/README.md
--rw-r--r--   0        0        0     4591 1970-01-01 00:00:00.000000 nautikos-0.3.3/setup.py
--rw-r--r--   0        0        0     4510 1970-01-01 00:00:00.000000 nautikos-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     3780 2023-05-15 12:51:22.973609 nautikos-0.3.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-15 12:51:22.973609 nautikos-0.3.4/nautikos/__init__.py
+-rw-r--r--   0        0        0     1282 2023-05-15 12:51:22.973609 nautikos-0.3.4/nautikos/cli.py
+-rw-r--r--   0        0        0     4081 2023-05-15 12:51:22.973609 nautikos-0.3.4/nautikos/manifests.py
+-rw-r--r--   0        0        0     3115 2023-05-15 12:51:22.973609 nautikos-0.3.4/nautikos/nautikos.py
+-rw-r--r--   0        0        0       76 2023-05-15 12:51:22.973609 nautikos-0.3.4/nautikos/yaml.py
+-rw-r--r--   0        0        0     1259 2023-05-15 12:51:22.973609 nautikos-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     4680 1970-01-01 00:00:00.000000 nautikos-0.3.4/PKG-INFO
```

### Comparing `nautikos-0.3.3/nautikos/cli.py` & `nautikos-0.3.4/nautikos/cli.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-import sys
-
-import typer
-
-from .nautikos import Nautikos
-
-app = typer.Typer()
-
-nautikos = Nautikos()
-
-
-@app.command()
-def main(
-    repository: str,
-    tag: str,
-    env: str = typer.Option(None),
-    labels: str = typer.Option(None),
-    config: str = typer.Option("nautikos.yaml"),
-    dry_run: bool = typer.Option(False, "--dry-run"),
-):
-    s = f"Updating '{repository}' to '{tag}'"
-    if env:
-        s += f" in '{env}'"
-    else:
-        s += " in all environments"
-    if labels:
-        s += f" with labels '{labels}'"
-    print(s)
-
-    nautikos.set_dry_run(dry_run)
-    nautikos.load_config(config)
-    nautikos.update_manifests(
-        repository, tag, environment=env, labels=labels.split(",") if labels else None
-    )
-
-    # Print modified files
-    count_updated_img = 0
-    for mod in nautikos.modifications:
-        print(mod)
-        if mod.updated:
-            count_updated_img += 1
-
-    # Determine output
-    if len(nautikos.modifications) == 0:
-        exit_msg = "ERROR - Didn't find any images to modify"
-        exit_code = 1
-    else:
-        exit_msg = f"Updated {count_updated_img} out of {len(nautikos.modifications)} discovered occurances of '{repository}' to '{tag}'"  # noqa: E501
-        exit_code = 0
-    print(exit_msg)
-    sys.exit(exit_code)
+import sys
+
+import typer
+
+from .nautikos import Nautikos
+
+app = typer.Typer()
+
+nautikos = Nautikos()
+
+
+@app.command()
+def main(
+    repository: str,
+    tag: str,
+    env: str = typer.Option(None),
+    labels: str = typer.Option(None),
+    config: str = typer.Option("nautikos.yaml"),
+    dry_run: bool = typer.Option(False, "--dry-run"),
+):
+    s = f"Updating '{repository}' to '{tag}'"
+    if env:
+        s += f" in '{env}'"
+    else:
+        s += " in all environments"
+    if labels:
+        s += f" with labels '{labels}'"
+    print(s)
+
+    nautikos.set_dry_run(dry_run)
+    nautikos.load_config(config)
+    nautikos.update_manifests(
+        repository, tag, environment=env, labels=labels.split(",") if labels else None
+    )
+
+    # Print modified files
+    count_updated_img = 0
+    for mod in nautikos.modifications:
+        print(mod)
+        if mod.updated:
+            count_updated_img += 1
+
+    # Determine output
+    if len(nautikos.modifications) == 0:
+        exit_msg = "ERROR - Didn't find any images to modify"
+        exit_code = 1
+    else:
+        exit_msg = f"Updated {count_updated_img} out of {len(nautikos.modifications)} discovered occurances of '{repository}' to '{tag}'"  # noqa: E501
+        exit_code = 0
+    print(exit_msg)
+    sys.exit(exit_code)
```

### Comparing `nautikos-0.3.3/nautikos/nautikos.py` & `nautikos-0.3.4/nautikos/nautikos.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-from __future__ import annotations
-
-import pathlib
-from typing import TypedDict
-
-from .manifests import Modification, get_manifest
-from .yaml import yaml
-
-
-class ManifestConfig(TypedDict):
-    path: str
-    type: str
-    labels: list[str]
-    repositories: list[str]
-
-
-class EnvironmentConfig(TypedDict):
-    name: str
-    manifests: list[ManifestConfig]
-
-
-class ConfigData(TypedDict):
-    environments: list[EnvironmentConfig]
-
-
-class Nautikos:
-    def __init__(self) -> None:
-        self._workdir: pathlib.Path = pathlib.Path(".")
-        self._dry_run: bool = False
-        self._environments: list[EnvironmentConfig] = []
-        self._modifications: list[Modification] = []
-
-    @property
-    def modifications(self) -> list[Modification]:
-        return self._modifications
-
-    def set_dry_run(self, dry_run: bool) -> None:
-        self._dry_run = dry_run
-
-    def load_config(self, path: str) -> None:
-        self._workdir = pathlib.Path(path).parent
-        with open(path, "r") as f:
-            config_data: ConfigData = yaml.load(f)
-        self._environments = config_data["environments"]
-
-    def update_manifests(
-        self,
-        repository: str,
-        new_tag: str,
-        environment: str | None = None,
-        labels: list[str] | None = None,
-    ) -> None:
-        """Updates image tags of given repository to new tag
-
-        If environment is passed, only environments with matching name are modified;
-        otherwise all environments are modified.
-
-        If label is passed, only manifests with matching label are modified; otherwise
-        all manifests in selected environments are modified.
-        """
-        # Get all relevant environments
-        environments = self._get_environments(environment)
-
-        # Get all relevant manifests
-        manifests: list[ManifestConfig] = []
-        for env in environments:
-            manifests += self._get_manifests(env, labels)
-
-        # Modify manifests
-        for manifest_config in manifests:
-            manifest = get_manifest(
-                manifest_config["path"],
-                manifest_config["type"],
-                workdir=self._workdir,
-            )
-            manifest.load()
-            manifest.modify(repository, new_tag)
-            if len(manifest.modifications) > 0:
-                if not self._dry_run:
-                    manifest.write()
-            self._modifications += manifest.modifications
-
-    def _get_environments(self, environment: str | None) -> list[EnvironmentConfig]:
-        envs: list[EnvironmentConfig] = []
-        for env in self._environments:
-            if not environment or env["name"] == environment:
-                envs.append(env)
-        return envs
-
-    def _get_manifests(
-        self, env: EnvironmentConfig, labels: list[str] | None = None
-    ) -> list[ManifestConfig]:
-        manifests: list[ManifestConfig] = []
-        for manifest in env["manifests"]:
-            if not labels or (
-                "labels" in manifest and set(labels).issubset(set(manifest["labels"]))
-            ):
-                manifests.append(manifest)
-        return manifests
+from __future__ import annotations
+
+import pathlib
+from typing import TypedDict
+
+from .manifests import Modification, get_manifest
+from .yaml import yaml
+
+
+class ManifestConfig(TypedDict):
+    path: str
+    type: str
+    labels: list[str]
+    repositories: list[str]
+
+
+class EnvironmentConfig(TypedDict):
+    name: str
+    manifests: list[ManifestConfig]
+
+
+class ConfigData(TypedDict):
+    environments: list[EnvironmentConfig]
+
+
+class Nautikos:
+    def __init__(self) -> None:
+        self._workdir: pathlib.Path = pathlib.Path(".")
+        self._dry_run: bool = False
+        self._environments: list[EnvironmentConfig] = []
+        self._modifications: list[Modification] = []
+
+    @property
+    def modifications(self) -> list[Modification]:
+        return self._modifications
+
+    def set_dry_run(self, dry_run: bool) -> None:
+        self._dry_run = dry_run
+
+    def load_config(self, path: str) -> None:
+        self._workdir = pathlib.Path(path).parent
+        with open(path, "r") as f:
+            config_data: ConfigData = yaml.load(f)
+        self._environments = config_data["environments"]
+
+    def update_manifests(
+        self,
+        repository: str,
+        new_tag: str,
+        environment: str | None = None,
+        labels: list[str] | None = None,
+    ) -> None:
+        """Updates image tags of given repository to new tag
+
+        If environment is passed, only environments with matching name are modified;
+        otherwise all environments are modified.
+
+        If label is passed, only manifests with matching label are modified; otherwise
+        all manifests in selected environments are modified.
+        """
+        # Get all relevant environments
+        environments = self._get_environments(environment)
+
+        # Get all relevant manifests
+        manifests: list[ManifestConfig] = []
+        for env in environments:
+            manifests += self._get_manifests(env, labels)
+
+        # Modify manifests
+        for manifest_config in manifests:
+            manifest = get_manifest(
+                manifest_config["path"],
+                manifest_config["type"],
+                workdir=self._workdir,
+            )
+            manifest.load()
+            manifest.modify(repository, new_tag)
+            if len(manifest.modifications) > 0:
+                if not self._dry_run:
+                    manifest.write()
+            self._modifications += manifest.modifications
+
+    def _get_environments(self, environment: str | None) -> list[EnvironmentConfig]:
+        envs: list[EnvironmentConfig] = []
+        for env in self._environments:
+            if not environment or env["name"] == environment:
+                envs.append(env)
+        return envs
+
+    def _get_manifests(
+        self, env: EnvironmentConfig, labels: list[str] | None = None
+    ) -> list[ManifestConfig]:
+        manifests: list[ManifestConfig] = []
+        for manifest in env["manifests"]:
+            if not labels or (
+                "labels" in manifest and set(labels).issubset(set(manifest["labels"]))
+            ):
+                manifests.append(manifest)
+        return manifests
```

### Comparing `nautikos-0.3.3/README.md` & `nautikos-0.3.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,99 +1,101 @@
-# Nautikos 
-
-*A lightweight CI/CD tool for updating image tags in Kubernetes manifests.* 
-
-[![PyPI version](https://badge.fury.io/py/nautikos.svg)](https://badge.fury.io/py/nautikos)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Python versions](https://img.shields.io/pypi/pyversions/nautikos)]()
-
-## Rationale
-
-A GitOps CI/CD process often uses a deployment or ops repo containing Kubernetes manifests for multiple services and environments. Tools like *Argo-CD* or *Flux* then track these repo's, and apply any changes to the cluster. When a new image of an application is created, you want the corresponding tags to be updated in the manifests housed in the deployment repo. Doing this manually is error prone. Having to write logic in every repo or pipeline to perform this is tedious. 
-
-This is where Nautikos comes in. 
-
-## Installation 
-
-```bash
-pip install nautikos
-```
-
-## Basic usage 
-
-Nautikos is configured through a YAML-file (`./nautikos.yaml`), that specifies where the manifests for the different images and environments can be found: 
-
-```yaml
-environments: 
-- name: prod 
-  manifests: 
-  - path: prod/app1/deployment.yaml  # Path relative to configuration file
-    type: kubernetes  # Type can be 'kubernetes' or 'kustomize'
-    labels:  # Optional specification of labels for more granular control
-    - app1
-    - refs/heads/main
-  - path: prod/app2/kustomize.yaml
-    type: kustomize
-- name: dev
-  manifests: 
-  - path: dev/app1/deployment.yaml
-    type: kubernetes
-    labels: 
-    - app1
-    - refs/heads/dev
-  - path: dev/app3/feature-A/deployment.yaml
-    type: kubernetes
-    labels: 
-    - app1
-    - refs/heads/feature-A
-```
-
-Next, you can run Nautikos to update the image tags of specific images in different environments.
-
-```bash
-nautikos my-repo 1.2.3  # Updates all occurences of `my-repo` to `1.2.3` in all manifests
-nautikos --env prod my-repo 2.3.4  # Updates all occurences of `my-repo` to `2.3.4` in `prod/app1/deployment.yaml` and `prod/app2/deployment`
-nautikos --env dev --labels app1 my-repo 4.5.6  # Updates all occurences of `my-repo` to `4.5.6` in `dev/app1/deployment.yaml`
-nautikos --labels 'app1,refs/heads/main' my-repo 5.6.7  # Updates all occurences of `my-repo` to `5.6.7` in `prod/app1/deployment.yaml`
-```
-
-## Supported tools
-
-The tool works with standard **Kubernetes** manifests and **Kustomize** - **Helm** might be added later. Each have their own format for defining image tags. 
-
-```yaml
-# Kubernetes manifests
-spec:
-  template:
-    spec:
-      containers:
-      - image: some-repository:tag
-
-# Kustomize
-images: 
-- name: some-repository
-  newTag: tag 
-```
-
-## Advanced usage
-
-Nautikos takes several options: 
-
-* `--dry-run`: prints the modified files to stdout, but doesn't edit in place 
-* `--config config-file.yaml`: path to config YAML, default is `./nautikos.yaml`
-
-## Alternatives 
-
-There are basically three alternatives to do the same thing: 
-
-* **Update manifests manually** - of course this works, but this is not really proper CD
-* **Write your own bash scripts in a pipeline using a tool like `sed` or `yq`** - This works, but having to write this logic for every project is tedious. 
-* **Use a tool like [Argo-CD Image updater](https://argocd-image-updater.readthedocs.io/en/stable/)** - very nice, but a bit heavy-weight, not very actively developed, and doesn't seem to support Azure Container Registry. 
-
-## Notes 
-
-Multiple YAML docs in one file is not yet supported. 
-
-## Dependencies 
-
-* **`typer`** - for creating a CLI 
-* **`ruamel.yaml`** - for handling YAML files while maintaining ordering and comments
+# Nautikos 
+
+*A lightweight CI/CD tool for updating image tags in Kubernetes manifests.* 
+
+[![PyPI version](https://badge.fury.io/py/nautikos.svg)](https://badge.fury.io/py/nautikos)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Python versions](https://img.shields.io/pypi/pyversions/nautikos)]()
+![example branch parameter](https://github.com/janheindejong/nautikos/actions/workflows/test.yml/badge.svg?branch=main)
+
+
+## Rationale
+
+A GitOps CI/CD process often uses a deployment or ops repo containing Kubernetes manifests for multiple services and environments. Tools like *Argo-CD* or *Flux* then track these repo's, and apply any changes to the cluster. When a new image of an application is created, you want the corresponding tags to be updated in the manifests housed in the deployment repo. Doing this manually is error prone. Having to write logic in every repo or pipeline to perform this is tedious. 
+
+This is where Nautikos comes in. 
+
+## Installation 
+
+```bash
+pip install nautikos
+```
+
+## Basic usage 
+
+Nautikos is configured through a YAML-file (`./nautikos.yaml`), that specifies where the manifests for the different images and environments can be found: 
+
+```yaml
+environments: 
+- name: prod 
+  manifests: 
+  - path: prod/app1/deployment.yaml  # Path relative to configuration file
+    type: kubernetes  # Type can be 'kubernetes' or 'kustomize'
+    labels:  # Optional specification of labels for more granular control
+    - app1
+    - refs/heads/main
+  - path: prod/app2/kustomize.yaml
+    type: kustomize
+- name: dev
+  manifests: 
+  - path: dev/app1/deployment.yaml
+    type: kubernetes
+    labels: 
+    - app1
+    - refs/heads/dev
+  - path: dev/app3/feature-A/deployment.yaml
+    type: kubernetes
+    labels: 
+    - app1
+    - refs/heads/feature-A
+```
+
+Next, you can run Nautikos to update the image tags of specific images in different environments.
+
+```bash
+nautikos my-repo 1.2.3  # Updates all occurences of `my-repo` to `1.2.3` in all manifests
+nautikos --env prod my-repo 2.3.4  # Updates all occurences of `my-repo` to `2.3.4` in `prod/app1/deployment.yaml` and `prod/app2/deployment`
+nautikos --env dev --labels app1 my-repo 4.5.6  # Updates all occurences of `my-repo` to `4.5.6` in `dev/app1/deployment.yaml`
+nautikos --labels 'app1,refs/heads/main' my-repo 5.6.7  # Updates all occurences of `my-repo` to `5.6.7` in `prod/app1/deployment.yaml`
+```
+
+## Supported tools
+
+The tool works with standard **Kubernetes** manifests and **Kustomize** - **Helm** might be added later. Each have their own format for defining image tags. 
+
+```yaml
+# Kubernetes manifests
+spec:
+  template:
+    spec:
+      containers:
+      - image: some-repository:tag
+
+# Kustomize
+images: 
+- name: some-repository
+  newTag: tag 
+```
+
+## Advanced usage
+
+Nautikos takes several options: 
+
+* `--dry-run`: prints the modified files to stdout, but doesn't edit in place 
+* `--config config-file.yaml`: path to config YAML, default is `./nautikos.yaml`
+
+## Alternatives 
+
+There are basically three alternatives to do the same thing: 
+
+* **Update manifests manually** - of course this works, but this is not really proper CD
+* **Write your own bash scripts in a pipeline using a tool like `sed` or `yq`** - This works, but having to write this logic for every project is tedious. 
+* **Use a tool like [Argo-CD Image updater](https://argocd-image-updater.readthedocs.io/en/stable/)** - very nice, but a bit heavy-weight, not very actively developed, and doesn't seem to support Azure Container Registry. 
+
+## Notes 
+
+Multiple YAML docs in one file is not yet supported. 
+
+## Dependencies 
+
+* **`typer`** - for creating a CLI 
+* **`ruamel.yaml`** - for handling YAML files while maintaining ordering and comments
```

### Comparing `nautikos-0.3.3/setup.py` & `nautikos-0.3.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,125 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nautikos
+Version: 0.3.4
+Summary: A CD tool for updating image tags in Kubernetes manifests
+Home-page: https://www.github.com/janheindejong/nautikos
+License: MIT
+Keywords: Kubernetes,DevOps,CI/CD,Kustomize,GitOps
+Author: Jan Hein de Jong
+Author-email: janhein.dejong@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Build Tools
+Requires-Dist: ruamel-yaml (>=0.17.21,<0.18.0)
+Requires-Dist: typer (>=0.7.0,<0.8.0)
+Description-Content-Type: text/markdown
+
+# Nautikos 
+
+*A lightweight CI/CD tool for updating image tags in Kubernetes manifests.* 
+
+[![PyPI version](https://badge.fury.io/py/nautikos.svg)](https://badge.fury.io/py/nautikos)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Python versions](https://img.shields.io/pypi/pyversions/nautikos)]()
+![example branch parameter](https://github.com/janheindejong/nautikos/actions/workflows/test.yml/badge.svg?branch=main)
+
+
+## Rationale
+
+A GitOps CI/CD process often uses a deployment or ops repo containing Kubernetes manifests for multiple services and environments. Tools like *Argo-CD* or *Flux* then track these repo's, and apply any changes to the cluster. When a new image of an application is created, you want the corresponding tags to be updated in the manifests housed in the deployment repo. Doing this manually is error prone. Having to write logic in every repo or pipeline to perform this is tedious. 
+
+This is where Nautikos comes in. 
+
+## Installation 
+
+```bash
+pip install nautikos
+```
+
+## Basic usage 
+
+Nautikos is configured through a YAML-file (`./nautikos.yaml`), that specifies where the manifests for the different images and environments can be found: 
+
+```yaml
+environments: 
+- name: prod 
+  manifests: 
+  - path: prod/app1/deployment.yaml  # Path relative to configuration file
+    type: kubernetes  # Type can be 'kubernetes' or 'kustomize'
+    labels:  # Optional specification of labels for more granular control
+    - app1
+    - refs/heads/main
+  - path: prod/app2/kustomize.yaml
+    type: kustomize
+- name: dev
+  manifests: 
+  - path: dev/app1/deployment.yaml
+    type: kubernetes
+    labels: 
+    - app1
+    - refs/heads/dev
+  - path: dev/app3/feature-A/deployment.yaml
+    type: kubernetes
+    labels: 
+    - app1
+    - refs/heads/feature-A
+```
+
+Next, you can run Nautikos to update the image tags of specific images in different environments.
+
+```bash
+nautikos my-repo 1.2.3  # Updates all occurences of `my-repo` to `1.2.3` in all manifests
+nautikos --env prod my-repo 2.3.4  # Updates all occurences of `my-repo` to `2.3.4` in `prod/app1/deployment.yaml` and `prod/app2/deployment`
+nautikos --env dev --labels app1 my-repo 4.5.6  # Updates all occurences of `my-repo` to `4.5.6` in `dev/app1/deployment.yaml`
+nautikos --labels 'app1,refs/heads/main' my-repo 5.6.7  # Updates all occurences of `my-repo` to `5.6.7` in `prod/app1/deployment.yaml`
+```
+
+## Supported tools
+
+The tool works with standard **Kubernetes** manifests and **Kustomize** - **Helm** might be added later. Each have their own format for defining image tags. 
+
+```yaml
+# Kubernetes manifests
+spec:
+  template:
+    spec:
+      containers:
+      - image: some-repository:tag
+
+# Kustomize
+images: 
+- name: some-repository
+  newTag: tag 
+```
+
+## Advanced usage
+
+Nautikos takes several options: 
+
+* `--dry-run`: prints the modified files to stdout, but doesn't edit in place 
+* `--config config-file.yaml`: path to config YAML, default is `./nautikos.yaml`
+
+## Alternatives 
+
+There are basically three alternatives to do the same thing: 
+
+* **Update manifests manually** - of course this works, but this is not really proper CD
+* **Write your own bash scripts in a pipeline using a tool like `sed` or `yq`** - This works, but having to write this logic for every project is tedious. 
+* **Use a tool like [Argo-CD Image updater](https://argocd-image-updater.readthedocs.io/en/stable/)** - very nice, but a bit heavy-weight, not very actively developed, and doesn't seem to support Azure Container Registry. 
 
-packages = \
-['nautikos']
+## Notes 
 
-package_data = \
-{'': ['*']}
+Multiple YAML docs in one file is not yet supported. 
 
-install_requires = \
-['ruamel-yaml>=0.17.21,<0.18.0', 'typer>=0.7.0,<0.8.0']
-
-entry_points = \
-{'console_scripts': ['nautikos = nautikos.cli:app']}
-
-setup_kwargs = {
-    'name': 'nautikos',
-    'version': '0.3.3',
-    'description': 'A CD tool for updating image tags in Kubernetes manifests',
-    'long_description': "# Nautikos \n\n*A lightweight CI/CD tool for updating image tags in Kubernetes manifests.* \n\n[![PyPI version](https://badge.fury.io/py/nautikos.svg)](https://badge.fury.io/py/nautikos)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Python versions](https://img.shields.io/pypi/pyversions/nautikos)]()\n\n## Rationale\n\nA GitOps CI/CD process often uses a deployment or ops repo containing Kubernetes manifests for multiple services and environments. Tools like *Argo-CD* or *Flux* then track these repo's, and apply any changes to the cluster. When a new image of an application is created, you want the corresponding tags to be updated in the manifests housed in the deployment repo. Doing this manually is error prone. Having to write logic in every repo or pipeline to perform this is tedious. \n\nThis is where Nautikos comes in. \n\n## Installation \n\n```bash\npip install nautikos\n```\n\n## Basic usage \n\nNautikos is configured through a YAML-file (`./nautikos.yaml`), that specifies where the manifests for the different images and environments can be found: \n\n```yaml\nenvironments: \n- name: prod \n  manifests: \n  - path: prod/app1/deployment.yaml  # Path relative to configuration file\n    type: kubernetes  # Type can be 'kubernetes' or 'kustomize'\n    labels:  # Optional specification of labels for more granular control\n    - app1\n    - refs/heads/main\n  - path: prod/app2/kustomize.yaml\n    type: kustomize\n- name: dev\n  manifests: \n  - path: dev/app1/deployment.yaml\n    type: kubernetes\n    labels: \n    - app1\n    - refs/heads/dev\n  - path: dev/app3/feature-A/deployment.yaml\n    type: kubernetes\n    labels: \n    - app1\n    - refs/heads/feature-A\n```\n\nNext, you can run Nautikos to update the image tags of specific images in different environments.\n\n```bash\nnautikos my-repo 1.2.3  # Updates all occurences of `my-repo` to `1.2.3` in all manifests\nnautikos --env prod my-repo 2.3.4  # Updates all occurences of `my-repo` to `2.3.4` in `prod/app1/deployment.yaml` and `prod/app2/deployment`\nnautikos --env dev --labels app1 my-repo 4.5.6  # Updates all occurences of `my-repo` to `4.5.6` in `dev/app1/deployment.yaml`\nnautikos --labels 'app1,refs/heads/main' my-repo 5.6.7  # Updates all occurences of `my-repo` to `5.6.7` in `prod/app1/deployment.yaml`\n```\n\n## Supported tools\n\nThe tool works with standard **Kubernetes** manifests and **Kustomize** - **Helm** might be added later. Each have their own format for defining image tags. \n\n```yaml\n# Kubernetes manifests\nspec:\n  template:\n    spec:\n      containers:\n      - image: some-repository:tag\n\n# Kustomize\nimages: \n- name: some-repository\n  newTag: tag \n```\n\n## Advanced usage\n\nNautikos takes several options: \n\n* `--dry-run`: prints the modified files to stdout, but doesn't edit in place \n* `--config config-file.yaml`: path to config YAML, default is `./nautikos.yaml`\n\n## Alternatives \n\nThere are basically three alternatives to do the same thing: \n\n* **Update manifests manually** - of course this works, but this is not really proper CD\n* **Write your own bash scripts in a pipeline using a tool like `sed` or `yq`** - This works, but having to write this logic for every project is tedious. \n* **Use a tool like [Argo-CD Image updater](https://argocd-image-updater.readthedocs.io/en/stable/)** - very nice, but a bit heavy-weight, not very actively developed, and doesn't seem to support Azure Container Registry. \n\n## Notes \n\nMultiple YAML docs in one file is not yet supported. \n\n## Dependencies \n\n* **`typer`** - for creating a CLI \n* **`ruamel.yaml`** - for handling YAML files while maintaining ordering and comments\n",
-    'author': 'Jan Hein de Jong',
-    'author_email': 'janhein.dejong@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://www.github.com/janheindejong/nautikos',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
-}
+## Dependencies 
 
+* **`typer`** - for creating a CLI 
+* **`ruamel.yaml`** - for handling YAML files while maintaining ordering and comments
 
-setup(**setup_kwargs)
```

