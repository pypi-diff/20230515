# Comparing `tmp/lnbase_biolab-0.15.0.tar.gz` & `tmp/lnbase_biolab-0.15.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnbase_biolab-0.15.0.tar", last modified: Sat Apr 22 05:27:01 2023, max compression
+gzip compressed data, was "lnbase_biolab-0.15.1.tar", last modified: Mon May 15 09:48:16 2023, max compression
```

## Comparing `lnbase_biolab-0.15.0.tar` & `lnbase_biolab-0.15.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     3181 2023-04-10 14:20:00.286643 lnbase_biolab-0.15.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-03-24 23:23:34.181886 lnbase_biolab-0.15.0/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-03-24 23:23:34.181975 lnbase_biolab-0.15.0/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1395 2023-04-22 04:52:25.248633 lnbase_biolab-0.15.0/.gitignore
--rw-r--r--   0        0        0     1791 2023-03-24 23:23:34.182169 lnbase_biolab-0.15.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-03-24 23:23:34.182289 lnbase_biolab-0.15.0/LICENSE
--rw-r--r--   0        0        0      233 2023-04-22 04:52:25.248802 lnbase_biolab-0.15.0/README.md
--rw-r--r--   0        0        0       55 2023-04-22 04:52:25.248966 lnbase_biolab-0.15.0/docs/api.md
--rw-r--r--   0        0        0    10546 2023-04-22 05:26:41.836240 lnbase_biolab-0.15.0/docs/changelog.md
--rw-r--r--   0        0        0     1148 2023-04-22 04:52:25.249248 lnbase_biolab-0.15.0/docs/guide/base-orms.ipynb
--rw-r--r--   0        0        0       47 2023-03-24 23:23:34.182699 lnbase_biolab-0.15.0/docs/guide/index.md
--rw-r--r--   0        0        0     1114 2023-04-22 04:52:25.249372 lnbase_biolab-0.15.0/docs/index.md
--rw-r--r--   0        0        0      163 2023-04-22 04:52:25.249499 lnbase_biolab-0.15.0/lamin-project.yaml
--rw-r--r--   0        0        0      497 2023-04-22 05:26:33.234096 lnbase_biolab-0.15.0/lnbase_biolab/__init__.py
--rw-r--r--   0        0        0     2031 2023-04-22 04:52:25.249758 lnbase_biolab-0.15.0/lnbase_biolab/_core.py
--rw-r--r--   0        0        0      376 2023-04-22 04:52:25.249825 lnbase_biolab-0.15.0/lnbase_biolab/dev/__init__.py
--rw-r--r--   0        0        0      937 2023-04-22 04:52:25.249906 lnbase_biolab-0.15.0/lnbase_biolab/dev/_id.py
--rw-r--r--   0        0        0     8756 2023-04-22 04:52:25.250017 lnbase_biolab-0.15.0/lnbase_biolab/dev/_sample_submission.py
--rw-r--r--   0        0        0      872 2023-04-22 04:52:25.250094 lnbase_biolab-0.15.0/lnbase_biolab/dev/_versions.py
--rw-r--r--   0        0        0      134 2023-04-22 04:52:25.250164 lnbase_biolab-0.15.0/lnbase_biolab/dev/datasets/__init__.py
--rw-r--r--   0        0        0     2047 2023-04-22 04:52:25.250240 lnbase_biolab-0.15.0/lnbase_biolab/dev/datasets/_core.py
--rw-r--r--   0        0        0      308 2023-04-22 04:52:25.250308 lnbase_biolab-0.15.0/lnbase_biolab/dev/id.py
--rw-r--r--   0        0        0      925 2023-04-22 04:52:25.250645 lnbase_biolab-0.15.0/noxfile.py
--rw-r--r--   0        0        0      935 2023-04-22 04:52:25.250840 lnbase_biolab-0.15.0/pyproject.toml
--rw-r--r--   0        0        0      490 2023-03-24 23:23:34.185127 lnbase_biolab-0.15.0/tests/test_notebooks.py
--rw-r--r--   0        0        0     1124 1970-01-01 00:00:00.000000 lnbase_biolab-0.15.0/PKG-INFO
+-rw-r--r--   0        0        0     3181 2023-04-23 05:14:07.168302 lnbase_biolab-0.15.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-04-23 05:14:07.168467 lnbase_biolab-0.15.1/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-04-23 05:14:07.168559 lnbase_biolab-0.15.1/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1395 2023-04-23 05:14:20.147962 lnbase_biolab-0.15.1/.gitignore
+-rw-r--r--   0        0        0     1791 2023-04-23 05:14:07.168820 lnbase_biolab-0.15.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-04-23 05:14:07.168930 lnbase_biolab-0.15.1/LICENSE
+-rw-r--r--   0        0        0      233 2023-04-23 05:14:20.148391 lnbase_biolab-0.15.1/README.md
+-rw-r--r--   0        0        0       55 2023-04-23 05:14:20.148735 lnbase_biolab-0.15.1/docs/api.md
+-rw-r--r--   0        0        0    10697 2023-05-15 09:47:47.663746 lnbase_biolab-0.15.1/docs/changelog.md
+-rw-r--r--   0        0        0     1148 2023-04-23 05:14:20.149346 lnbase_biolab-0.15.1/docs/guide/base-orms.ipynb
+-rw-r--r--   0        0        0       47 2023-04-23 05:14:07.169864 lnbase_biolab-0.15.1/docs/guide/index.md
+-rw-r--r--   0        0        0     1114 2023-04-23 05:14:20.149678 lnbase_biolab-0.15.1/docs/index.md
+-rw-r--r--   0        0        0      163 2023-04-23 05:14:20.149983 lnbase_biolab-0.15.1/lamin-project.yaml
+-rw-r--r--   0        0        0      533 2023-05-15 09:47:37.807254 lnbase_biolab-0.15.1/lnbase_biolab/__init__.py
+-rw-r--r--   0        0        0     2295 2023-05-15 09:47:09.327669 lnbase_biolab-0.15.1/lnbase_biolab/_core.py
+-rw-r--r--   0        0        0      376 2023-04-23 05:14:20.150771 lnbase_biolab-0.15.1/lnbase_biolab/dev/__init__.py
+-rw-r--r--   0        0        0      937 2023-04-23 05:14:20.150893 lnbase_biolab-0.15.1/lnbase_biolab/dev/_id.py
+-rw-r--r--   0        0        0     8756 2023-04-23 05:14:20.151035 lnbase_biolab-0.15.1/lnbase_biolab/dev/_sample_submission.py
+-rw-r--r--   0        0        0      872 2023-04-23 05:14:20.151117 lnbase_biolab-0.15.1/lnbase_biolab/dev/_versions.py
+-rw-r--r--   0        0        0      134 2023-04-23 05:14:20.151235 lnbase_biolab-0.15.1/lnbase_biolab/dev/datasets/__init__.py
+-rw-r--r--   0        0        0     2047 2023-04-23 05:14:20.151319 lnbase_biolab-0.15.1/lnbase_biolab/dev/datasets/_core.py
+-rw-r--r--   0        0        0      308 2023-04-23 05:14:20.151397 lnbase_biolab-0.15.1/lnbase_biolab/dev/id.py
+-rw-r--r--   0        0        0      925 2023-04-23 05:14:20.151646 lnbase_biolab-0.15.1/noxfile.py
+-rw-r--r--   0        0        0      935 2023-04-23 05:14:20.151899 lnbase_biolab-0.15.1/pyproject.toml
+-rw-r--r--   0        0        0      490 2023-04-23 05:14:07.172497 lnbase_biolab-0.15.1/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1124 1970-01-01 00:00:00.000000 lnbase_biolab-0.15.1/PKG-INFO
```

### Comparing `lnbase_biolab-0.15.0/.github/workflows/build.yml` & `lnbase_biolab-0.15.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lnbase_biolab-0.15.0/.github/workflows/latest-changes.yml` & `lnbase_biolab-0.15.1/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lnbase_biolab-0.15.0/.gitignore` & `lnbase_biolab-0.15.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lnbase_biolab-0.15.0/.pre-commit-config.yaml` & `lnbase_biolab-0.15.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lnbase_biolab-0.15.0/LICENSE` & `lnbase_biolab-0.15.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lnbase_biolab-0.15.0/docs/changelog.md` & `lnbase_biolab-0.15.1/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+✨ Added `TreatmentBase` | [68](https://github.com/laminlabs/lnbase-biolab/pull/68) | [sunnyosun](https://github.com/sunnyosun) | 2023-05-15 | 0.15.1
 🏗️ Turn into base model module `lnschema-wetlab` → `lnbase-biolab` | [67](https://github.com/laminlabs/lnbase-biolab/pull/67) | [falexwolf](https://github.com/falexwolf) | 2023-04-22 | 0.15.0
 🚚 Move Readout to lnschema-bionty | [66](https://github.com/laminlabs/lnbase-biolab/pull/66) | [sunnyosun](https://github.com/sunnyosun) | 2023-03-27 | 0.15rc2
 🚚 Rename `DObject` to `File` | [65](https://github.com/laminlabs/lnbase-biolab/pull/65) | [falexwolf](https://github.com/falexwolf) | 2023-03-24 | 0.15rc1
 ✨ Auto population of readout | [64](https://github.com/laminlabs/lnbase-biolab/pull/64) | [sunnyosun](https://github.com/sunnyosun) | 2023-03-23 | 0.14.0
 🔥 Remove migration files | [63](https://github.com/laminlabs/lnbase-biolab/pull/63) | [sunnyosun](https://github.com/sunnyosun) | 2023-02-15 |
 ⬆️ Upgrade and rename `lndb_setup` to `lndb` (v0.32.0) | [61](https://github.com/laminlabs/lnbase-biolab/pull/61) | [bpenteado](https://github.com/bpenteado) | 2023-02-13 | 0.13.4
 🔥 Move the tests of sample submission to lndb-rest | [60](https://github.com/laminlabs/lnbase-biolab/pull/60) | [sunnyosun](https://github.com/sunnyosun) | 2023-01-17 | 0.13.3
```

### Comparing `lnbase_biolab-0.15.0/docs/guide/base-orms.ipynb` & `lnbase_biolab-0.15.1/docs/guide/base-orms.ipynb`

 * *Files identical despite different names*

### Comparing `lnbase_biolab-0.15.0/docs/index.md` & `lnbase_biolab-0.15.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `lnbase_biolab-0.15.0/lnbase_biolab/_core.py` & `lnbase_biolab-0.15.1/lnbase_biolab/_core.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,7 +55,15 @@
     name: Optional[str] = Field(default=None, index=True)
     batch: Optional[str] = None
     filepath_r1: Optional[str] = None
     filepath_r2: Optional[str] = None
     created_by: str = CreatedBy
     created_at: datetime = CreatedAt
     updated_at: Optional[datetime] = UpdatedAt
+
+
+class TreatmentBase(SQLModel):  # type: ignore
+    """Treatments."""
+
+    id: str = Field(default_factory=idg.treatment, primary_key=True)
+    name: Optional[str] = Field(default=None, index=True)
+    description: Optional[str] = Field(default=None, index=True)
```

### Comparing `lnbase_biolab-0.15.0/lnbase_biolab/dev/_id.py` & `lnbase_biolab-0.15.1/lnbase_biolab/dev/_id.py`

 * *Files identical despite different names*

### Comparing `lnbase_biolab-0.15.0/lnbase_biolab/dev/_sample_submission.py` & `lnbase_biolab-0.15.1/lnbase_biolab/dev/_sample_submission.py`

 * *Files identical despite different names*

### Comparing `lnbase_biolab-0.15.0/lnbase_biolab/dev/_versions.py` & `lnbase_biolab-0.15.1/lnbase_biolab/dev/_versions.py`

 * *Files identical despite different names*

### Comparing `lnbase_biolab-0.15.0/lnbase_biolab/dev/datasets/_core.py` & `lnbase_biolab-0.15.1/lnbase_biolab/dev/datasets/_core.py`

 * *Files identical despite different names*

### Comparing `lnbase_biolab-0.15.0/noxfile.py` & `lnbase_biolab-0.15.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `lnbase_biolab-0.15.0/pyproject.toml` & `lnbase_biolab-0.15.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lnbase_biolab-0.15.0/PKG-INFO` & `lnbase_biolab-0.15.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnbase_biolab
-Version: 0.15.0
+Version: 0.15.1
 Summary: Base classes for a lab schema in biology (`vvhc`).
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

