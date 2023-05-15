# Comparing `tmp/lnschema_lamin1-0.16.0.tar.gz` & `tmp/lnschema_lamin1-0.16.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnschema_lamin1-0.16.0.tar", last modified: Mon Apr 24 17:50:09 2023, max compression
+gzip compressed data, was "lnschema_lamin1-0.16.1.tar", last modified: Mon Apr 24 18:22:21 2023, max compression
```

## Comparing `lnschema_lamin1-0.16.0.tar` & `lnschema_lamin1-0.16.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     3577 2023-04-22 05:28:10.791442 lnschema_lamin1-0.16.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-04-22 03:48:17.570277 lnschema_lamin1-0.16.0/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-04-22 03:48:17.570464 lnschema_lamin1-0.16.0/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1416 2023-04-22 03:51:54.773184 lnschema_lamin1-0.16.0/.gitignore
--rw-r--r--   0        0        0     1795 2023-04-24 17:49:33.167540 lnschema_lamin1-0.16.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      145 2023-04-22 05:28:10.791672 lnschema_lamin1-0.16.0/README.md
--rw-r--r--   0        0        0      432 2023-04-24 17:49:45.305188 lnschema_lamin1-0.16.0/docs/changelog.md
--rw-r--r--   0        0        0     5015 2023-04-24 17:39:09.187958 lnschema_lamin1-0.16.0/docs/guide/01-get-started.ipynb
--rw-r--r--   0        0        0     2190 2023-04-24 17:39:09.199540 lnschema_lamin1-0.16.0/docs/guide/02-orms.ipynb
--rw-r--r--   0        0        0     5397 2023-04-24 17:39:09.201311 lnschema_lamin1-0.16.0/docs/guide/10-migrate.ipynb
--rw-r--r--   0        0        0       65 2023-04-22 04:06:04.615921 lnschema_lamin1-0.16.0/docs/guide/index.md
--rw-r--r--   0        0        0      122 2023-04-22 03:48:11.331800 lnschema_lamin1-0.16.0/docs/index.md
--rw-r--r--   0        0        0       63 2023-04-22 03:51:55.148920 lnschema_lamin1-0.16.0/docs/reference.md
--rw-r--r--   0        0        0      163 2023-04-22 04:44:31.557229 lnschema_lamin1-0.16.0/lamin-project.yaml
--rw-r--r--   0        0        0      617 2023-04-24 17:49:37.492197 lnschema_lamin1-0.16.0/lnschema_lamin1/__init__.py
--rw-r--r--   0        0        0     2685 2023-04-24 17:49:33.168641 lnschema_lamin1-0.16.0/lnschema_lamin1/_core.py
--rw-r--r--   0        0        0     1765 2023-04-24 17:49:33.169143 lnschema_lamin1-0.16.0/lnschema_lamin1/_link.py
--rw-r--r--   0        0        0      253 2023-04-22 05:28:10.792283 lnschema_lamin1-0.16.0/lnschema_lamin1/dev/__init__.py
--rw-r--r--   0        0        0      119 2023-04-22 03:48:17.441295 lnschema_lamin1-0.16.0/lnschema_lamin1/dev/_id.py
--rw-r--r--   0        0        0     1145 2023-04-22 03:56:14.122435 lnschema_lamin1-0.16.0/lnschema_lamin1/dev/_versions.py
--rw-r--r--   0        0        0       31 2023-04-22 03:48:17.441214 lnschema_lamin1-0.16.0/lnschema_lamin1/dev/id.py
--rw-r--r--   0        0        0      284 2023-04-24 17:49:33.169327 lnschema_lamin1-0.16.0/lnschema_lamin1/link.py
--rw-r--r--   0        0        0     1063 2023-04-24 17:49:33.169471 lnschema_lamin1-0.16.0/lnschema_lamin1/migrations/versions/2023-04-24-652443621d5a-v0_16_0.py
--rw-r--r--   0        0        0      776 2023-04-24 16:11:06.697345 lnschema_lamin1-0.16.0/noxfile.py
--rw-r--r--   0        0        0      655 2023-04-24 16:22:20.030267 lnschema_lamin1-0.16.0/pyproject.toml
--rw-r--r--   0        0        0      811 2023-04-22 04:38:14.658100 lnschema_lamin1-0.16.0/tests/test_migrations.py
--rw-r--r--   0        0        0      481 2023-04-22 03:48:11.224317 lnschema_lamin1-0.16.0/tests/test_notebooks.py
--rw-r--r--   0        0        0      707 1970-01-01 00:00:00.000000 lnschema_lamin1-0.16.0/PKG-INFO
+-rw-r--r--   0        0        0     3577 2023-04-22 05:28:10.791442 lnschema_lamin1-0.16.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-04-22 03:48:17.570277 lnschema_lamin1-0.16.1/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-04-22 03:48:17.570464 lnschema_lamin1-0.16.1/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1416 2023-04-22 03:51:54.773184 lnschema_lamin1-0.16.1/.gitignore
+-rw-r--r--   0        0        0     1795 2023-04-24 17:49:33.167540 lnschema_lamin1-0.16.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      145 2023-04-22 05:28:10.791672 lnschema_lamin1-0.16.1/README.md
+-rw-r--r--   0        0        0      432 2023-04-24 18:21:54.957433 lnschema_lamin1-0.16.1/docs/changelog.md
+-rw-r--r--   0        0        0     5015 2023-04-24 17:39:09.187958 lnschema_lamin1-0.16.1/docs/guide/01-get-started.ipynb
+-rw-r--r--   0        0        0     2190 2023-04-24 17:39:09.199540 lnschema_lamin1-0.16.1/docs/guide/02-orms.ipynb
+-rw-r--r--   0        0        0     5397 2023-04-24 17:39:09.201311 lnschema_lamin1-0.16.1/docs/guide/10-migrate.ipynb
+-rw-r--r--   0        0        0       65 2023-04-22 04:06:04.615921 lnschema_lamin1-0.16.1/docs/guide/index.md
+-rw-r--r--   0        0        0      122 2023-04-22 03:48:11.331800 lnschema_lamin1-0.16.1/docs/index.md
+-rw-r--r--   0        0        0       63 2023-04-22 03:51:55.148920 lnschema_lamin1-0.16.1/docs/reference.md
+-rw-r--r--   0        0        0      163 2023-04-22 04:44:31.557229 lnschema_lamin1-0.16.1/lamin-project.yaml
+-rw-r--r--   0        0        0      617 2023-04-24 18:21:46.244749 lnschema_lamin1-0.16.1/lnschema_lamin1/__init__.py
+-rw-r--r--   0        0        0     2659 2023-04-24 18:15:37.605909 lnschema_lamin1-0.16.1/lnschema_lamin1/_core.py
+-rw-r--r--   0        0        0     1765 2023-04-24 17:49:33.169143 lnschema_lamin1-0.16.1/lnschema_lamin1/_link.py
+-rw-r--r--   0        0        0      253 2023-04-22 05:28:10.792283 lnschema_lamin1-0.16.1/lnschema_lamin1/dev/__init__.py
+-rw-r--r--   0        0        0      119 2023-04-22 03:48:17.441295 lnschema_lamin1-0.16.1/lnschema_lamin1/dev/_id.py
+-rw-r--r--   0        0        0     1145 2023-04-22 03:56:14.122435 lnschema_lamin1-0.16.1/lnschema_lamin1/dev/_versions.py
+-rw-r--r--   0        0        0       31 2023-04-22 03:48:17.441214 lnschema_lamin1-0.16.1/lnschema_lamin1/dev/id.py
+-rw-r--r--   0        0        0      284 2023-04-24 17:49:33.169327 lnschema_lamin1-0.16.1/lnschema_lamin1/link.py
+-rw-r--r--   0        0        0     1063 2023-04-24 17:49:33.169471 lnschema_lamin1-0.16.1/lnschema_lamin1/migrations/versions/2023-04-24-652443621d5a-v0_16_0.py
+-rw-r--r--   0        0        0      776 2023-04-24 16:11:06.697345 lnschema_lamin1-0.16.1/noxfile.py
+-rw-r--r--   0        0        0      655 2023-04-24 16:22:20.030267 lnschema_lamin1-0.16.1/pyproject.toml
+-rw-r--r--   0        0        0      811 2023-04-22 04:38:14.658100 lnschema_lamin1-0.16.1/tests/test_migrations.py
+-rw-r--r--   0        0        0      481 2023-04-22 03:48:11.224317 lnschema_lamin1-0.16.1/tests/test_notebooks.py
+-rw-r--r--   0        0        0      707 1970-01-01 00:00:00.000000 lnschema_lamin1-0.16.1/PKG-INFO
```

### Comparing `lnschema_lamin1-0.16.0/.github/workflows/build.yml` & `lnschema_lamin1-0.16.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.0/.github/workflows/latest-changes.yml` & `lnschema_lamin1-0.16.1/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.0/.gitignore` & `lnschema_lamin1-0.16.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.0/.pre-commit-config.yaml` & `lnschema_lamin1-0.16.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.0/docs/guide/01-get-started.ipynb` & `lnschema_lamin1-0.16.1/docs/guide/01-get-started.ipynb`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.0/docs/guide/02-orms.ipynb` & `lnschema_lamin1-0.16.1/docs/guide/02-orms.ipynb`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.0/docs/guide/10-migrate.ipynb` & `lnschema_lamin1-0.16.1/docs/guide/10-migrate.ipynb`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.0/lnschema_lamin1/__init__.py` & `lnschema_lamin1-0.16.1/lnschema_lamin1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
    link
 
 """
 
 _schema_id = "tvhn"
 _name = "lamin1"
 _migration = "652443621d5a"
-__version__ = "0.16.0"
+__version__ = "0.16.1"
 
 # prints warning of python versions
 from lamin_logger import py_version_warning
 
 py_version_warning("3.8", "3.10")
```

### Comparing `lnschema_lamin1-0.16.0/lnschema_lamin1/_core.py` & `lnschema_lamin1-0.16.1/lnschema_lamin1/_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     files: File = Relationship(
         back_populates="experiments",
         sa_relationship_kwargs=dict(secondary=FileExperiment.__table__),
     )
 
 
 File.experiments = relationship(Experiment, back_populates="files", secondary=FileExperiment.__table__)
-File.__sqlmodel_relationships__["experiments"] = None
 
 
 class ExperimentType(ExperimentTypeBase, table=True):  # type: ignore
     """Experiment types."""
 
     __tablename__ = f"{prefix}experiment_type"
 
@@ -54,19 +53,20 @@
         back_populates="biosamples",
         sa_relationship_kwargs=dict(secondary=FileBiosample.__table__),
     )
 
 
 File.biosamples = relationship(Biosample, back_populates="files", secondary=FileBiosample.__table__)
 File.cell_types = relationship(CellType, secondary=FileCellType.__table__)
-add_relationship_keys(Biosample)
+add_relationship_keys(File)
 
 
 class Techsample(TechsampleBase, table=True):  # type: ignore
     biosamples: Biosample = Relationship(
         back_populates="techsamples",
         sa_relationship_kwargs=dict(secondary=BiosampleTechsample.__table__),
     )
 
 
 Biosample.techsamples = relationship(Techsample, back_populates="biosamples", secondary=BiosampleTechsample.__table__)
 Biosample.__sqlmodel_relationships__["techsamples"] = None
+add_relationship_keys(Biosample)
```

### Comparing `lnschema_lamin1-0.16.0/lnschema_lamin1/_link.py` & `lnschema_lamin1-0.16.1/lnschema_lamin1/_link.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.0/lnschema_lamin1/dev/_versions.py` & `lnschema_lamin1-0.16.1/lnschema_lamin1/dev/_versions.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.0/lnschema_lamin1/migrations/versions/2023-04-24-652443621d5a-v0_16_0.py` & `lnschema_lamin1-0.16.1/lnschema_lamin1/migrations/versions/2023-04-24-652443621d5a-v0_16_0.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.0/noxfile.py` & `lnschema_lamin1-0.16.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.0/pyproject.toml` & `lnschema_lamin1-0.16.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.0/tests/test_migrations.py` & `lnschema_lamin1-0.16.1/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.0/PKG-INFO` & `lnschema_lamin1-0.16.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnschema_lamin1
-Version: 0.16.0
+Version: 0.16.1
 Summary: Lamin's `lamin1` lab schema (`tvhn`).
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lamindb[bionty,lamin1]
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: nox ; extra == "dev"
 Requires-Dist: pytest>=6.0 ; extra == "test"
```

