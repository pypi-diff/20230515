# Comparing `tmp/issue_db_api-0.9.0.tar.gz` & `tmp/issue_db_api-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "issue_db_api-0.9.0.tar", last modified: Mon May 15 11:23:16 2023, max compression
+gzip compressed data, was "issue_db_api-0.9.1.tar", last modified: Mon May 15 11:59:10 2023, max compression
```

## Comparing `issue_db_api-0.9.0.tar` & `issue_db_api-0.9.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-15 11:23:16.982522 issue_db_api-0.9.0/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       82 2023-04-20 09:20:00.000000 issue_db_api-0.9.0/.gitignore
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1069 2023-04-20 08:15:34.000000 issue_db_api-0.9.0/LICENSE
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      103 2023-04-20 08:15:34.000000 issue_db_api-0.9.0/MANIFEST.in
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-15 11:23:16.982522 issue_db_api-0.9.0/PKG-INFO
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      200 2023-04-20 08:15:34.000000 issue_db_api-0.9.0/README.md
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-15 11:23:16.978522 issue_db_api-0.9.0/issue_db_api/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      519 2023-05-15 11:22:45.000000 issue_db_api-0.9.0/issue_db_api/Cargo.toml
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       25 2023-05-04 14:06:56.000000 issue_db_api-0.9.0/issue_db_api/__init__.py
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     9223 2023-05-15 11:22:23.000000 issue_db_api-0.9.0/issue_db_api/issue_api.pyi
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-15 11:23:16.982522 issue_db_api-0.9.0/issue_db_api/src/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    46895 2023-05-15 10:40:01.000000 issue_db_api-0.9.0/issue_db_api/src/api_core.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1049 2023-05-04 13:53:55.000000 issue_db_api-0.9.0/issue_db_api/src/comments.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5322 2023-05-11 12:05:05.000000 issue_db_api-0.9.0/issue_db_api/src/config.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     3788 2023-05-04 13:53:55.000000 issue_db_api-0.9.0/issue_db_api/src/embedding.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     2105 2023-05-12 10:30:49.000000 issue_db_api-0.9.0/issue_db_api/src/errors.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1622 2023-05-15 10:43:58.000000 issue_db_api-0.9.0/issue_db_api/src/files.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     6635 2023-05-11 12:09:47.000000 issue_db_api-0.9.0/issue_db_api/src/issues.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      571 2023-04-20 08:15:34.000000 issue_db_api-0.9.0/issue_db_api/src/labels.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    41681 2023-05-15 11:20:32.000000 issue_db_api-0.9.0/issue_db_api/src/lib.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    10983 2023-05-04 13:53:55.000000 issue_db_api-0.9.0/issue_db_api/src/models.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     3910 2023-05-01 16:59:08.000000 issue_db_api-0.9.0/issue_db_api/src/query.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     7521 2023-05-15 11:20:32.000000 issue_db_api-0.9.0/issue_db_api/src/repository.rs
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-15 11:23:16.982522 issue_db_api-0.9.0/issue_db_api/src/schemas/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5031 2023-04-20 08:15:34.000000 issue_db_api-0.9.0/issue_db_api/src/schemas/raw_issue_response.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       27 2023-04-20 08:15:34.000000 issue_db_api-0.9.0/issue_db_api/src/schemas.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1626 2023-05-04 13:53:55.000000 issue_db_api-0.9.0/issue_db_api/src/tags.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     2583 2023-05-11 11:58:07.000000 issue_db_api-0.9.0/issue_db_api/src/util.rs
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-15 11:23:16.978522 issue_db_api-0.9.0/issue_db_api.egg-info/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-15 11:23:16.000000 issue_db_api-0.9.0/issue_db_api.egg-info/PKG-INFO
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      774 2023-05-15 11:23:16.000000 issue_db_api-0.9.0/issue_db_api.egg-info/SOURCES.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-05-15 11:23:16.000000 issue_db_api-0.9.0/issue_db_api.egg-info/dependency_links.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.9.0/issue_db_api.egg-info/not-zip-safe
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       13 2023-05-15 11:23:16.000000 issue_db_api-0.9.0/issue_db_api.egg-info/top_level.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      529 2023-05-15 11:22:45.000000 issue_db_api-0.9.0/pyproject.toml
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       38 2023-05-15 11:23:16.982522 issue_db_api-0.9.0/setup.cfg
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      253 2023-04-20 08:15:34.000000 issue_db_api-0.9.0/setup.py
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-15 11:59:10.603046 issue_db_api-0.9.1/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       82 2023-04-20 09:20:00.000000 issue_db_api-0.9.1/.gitignore
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1069 2023-04-20 08:15:34.000000 issue_db_api-0.9.1/LICENSE
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      103 2023-04-20 08:15:34.000000 issue_db_api-0.9.1/MANIFEST.in
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-15 11:59:10.603046 issue_db_api-0.9.1/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      200 2023-04-20 08:15:34.000000 issue_db_api-0.9.1/README.md
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-15 11:59:10.599046 issue_db_api-0.9.1/issue_db_api/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      519 2023-05-15 11:58:40.000000 issue_db_api-0.9.1/issue_db_api/Cargo.toml
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       25 2023-05-04 14:06:56.000000 issue_db_api-0.9.1/issue_db_api/__init__.py
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     9223 2023-05-15 11:22:23.000000 issue_db_api-0.9.1/issue_db_api/issue_api.pyi
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-15 11:59:10.603046 issue_db_api-0.9.1/issue_db_api/src/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    46895 2023-05-15 10:40:01.000000 issue_db_api-0.9.1/issue_db_api/src/api_core.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1049 2023-05-04 13:53:55.000000 issue_db_api-0.9.1/issue_db_api/src/comments.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5322 2023-05-11 12:05:05.000000 issue_db_api-0.9.1/issue_db_api/src/config.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3788 2023-05-04 13:53:55.000000 issue_db_api-0.9.1/issue_db_api/src/embedding.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     2105 2023-05-12 10:30:49.000000 issue_db_api-0.9.1/issue_db_api/src/errors.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1622 2023-05-15 10:43:58.000000 issue_db_api-0.9.1/issue_db_api/src/files.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     6635 2023-05-11 12:09:47.000000 issue_db_api-0.9.1/issue_db_api/src/issues.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      571 2023-04-20 08:15:34.000000 issue_db_api-0.9.1/issue_db_api/src/labels.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    41834 2023-05-15 11:58:40.000000 issue_db_api-0.9.1/issue_db_api/src/lib.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    10983 2023-05-04 13:53:55.000000 issue_db_api-0.9.1/issue_db_api/src/models.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3910 2023-05-01 16:59:08.000000 issue_db_api-0.9.1/issue_db_api/src/query.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     7669 2023-05-15 11:58:40.000000 issue_db_api-0.9.1/issue_db_api/src/repository.rs
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-15 11:59:10.603046 issue_db_api-0.9.1/issue_db_api/src/schemas/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5031 2023-04-20 08:15:34.000000 issue_db_api-0.9.1/issue_db_api/src/schemas/raw_issue_response.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       27 2023-04-20 08:15:34.000000 issue_db_api-0.9.1/issue_db_api/src/schemas.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1626 2023-05-04 13:53:55.000000 issue_db_api-0.9.1/issue_db_api/src/tags.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     2583 2023-05-11 11:58:07.000000 issue_db_api-0.9.1/issue_db_api/src/util.rs
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-15 11:59:10.603046 issue_db_api-0.9.1/issue_db_api.egg-info/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-15 11:59:10.000000 issue_db_api-0.9.1/issue_db_api.egg-info/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      774 2023-05-15 11:59:10.000000 issue_db_api-0.9.1/issue_db_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-05-15 11:59:10.000000 issue_db_api-0.9.1/issue_db_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.9.1/issue_db_api.egg-info/not-zip-safe
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       13 2023-05-15 11:59:10.000000 issue_db_api-0.9.1/issue_db_api.egg-info/top_level.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      529 2023-05-15 11:58:40.000000 issue_db_api-0.9.1/pyproject.toml
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       38 2023-05-15 11:59:10.603046 issue_db_api-0.9.1/setup.cfg
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      253 2023-04-20 08:15:34.000000 issue_db_api-0.9.1/setup.py
```

### Comparing `issue_db_api-0.9.0/LICENSE` & `issue_db_api-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.0/PKG-INFO` & `issue_db_api-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issue_db_api
-Version: 0.9.0
+Version: 0.9.1
 Author: Jesse Maarleveld
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `issue_db_api-0.9.0/issue_db_api/Cargo.toml` & `issue_db_api-0.9.1/issue_db_api/Cargo.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "issue-api-client"
-version = "0.9.0"
+version = "0.9.1"
 edition = "2021"
 
 [lib]
 name = "issue_api"
 crate-type = ["cdylib"]
 
 [features]
```

### Comparing `issue_db_api-0.9.0/issue_db_api/issue_api.pyi` & `issue_db_api-0.9.1/issue_db_api/issue_api.pyi`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.0/issue_db_api/src/api_core.rs` & `issue_db_api-0.9.1/issue_db_api/src/api_core.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.0/issue_db_api/src/comments.rs` & `issue_db_api-0.9.1/issue_db_api/src/comments.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.0/issue_db_api/src/config.rs` & `issue_db_api-0.9.1/issue_db_api/src/config.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.0/issue_db_api/src/embedding.rs` & `issue_db_api-0.9.1/issue_db_api/src/embedding.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.0/issue_db_api/src/errors.rs` & `issue_db_api-0.9.1/issue_db_api/src/errors.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.0/issue_db_api/src/files.rs` & `issue_db_api-0.9.1/issue_db_api/src/files.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.0/issue_db_api/src/issues.rs` & `issue_db_api-0.9.1/issue_db_api/src/issues.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.0/issue_db_api/src/labels.rs` & `issue_db_api-0.9.1/issue_db_api/src/labels.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.0/issue_db_api/src/lib.rs` & `issue_db_api-0.9.1/issue_db_api/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -366,14 +366,18 @@
         fn files(&self, category: Option<String>) -> PyResult<Vec<PyFile>> {
             let result = api2py_error(self.repo.files(category))?
                 .into_iter().map(|f| PyFile{inner: f})
                 .collect();
             Ok(result)
         }
 
+        fn get_file_by_id(&self, id: String) -> PyResult<PyFile> {
+            Ok(PyFile{inner: api2py_error(self.repo.get_file_by_id(id))?})
+        }
+
         fn upload_file(&self, path: String, description: String, category: String) -> PyResult<PyFile> {
             Ok(
                 PyFile{inner: api2py_error(self.repo.upload_file(path, description, category))?}
             )
         }
 
         fn delete_file(&self, file: &PyFile) -> PyResult<()> {
```

### Comparing `issue_db_api-0.9.0/issue_db_api/src/models.rs` & `issue_db_api-0.9.1/issue_db_api/src/models.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.0/issue_db_api/src/query.rs` & `issue_db_api-0.9.1/issue_db_api/src/query.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.0/issue_db_api/src/repository.rs` & `issue_db_api-0.9.1/issue_db_api/src/repository.rs`

 * *Files 2% similar despite different names*

```diff
@@ -205,14 +205,18 @@
         let result = self.api
             .get_all_files(category)?
             .into_iter().map(|f| f.into_bound_file(self.api.clone()))
             .collect();
         Ok(result)
     }
 
+    pub fn get_file_by_id(&self, id: String) -> APIResult<File> {
+        self.api.get_file(id).map(|f| f.into_bound_file(self.api.clone()))
+    }
+
     pub fn upload_file(&self, path: String, description: String, category: String) -> APIResult<File> {
         File::upload(self.api.clone(), path, description, category)
     }
 
     pub fn remove_file(&self, file: File) -> APIResult<()> {
         file.delete()
     }
```

### Comparing `issue_db_api-0.9.0/issue_db_api/src/schemas/raw_issue_response.rs` & `issue_db_api-0.9.1/issue_db_api/src/schemas/raw_issue_response.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.0/issue_db_api/src/tags.rs` & `issue_db_api-0.9.1/issue_db_api/src/tags.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.0/issue_db_api/src/util.rs` & `issue_db_api-0.9.1/issue_db_api/src/util.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.0/issue_db_api.egg-info/PKG-INFO` & `issue_db_api-0.9.1/issue_db_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issue-db-api
-Version: 0.9.0
+Version: 0.9.1
 Author: Jesse Maarleveld
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `issue_db_api-0.9.0/issue_db_api.egg-info/SOURCES.txt` & `issue_db_api-0.9.1/issue_db_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.0/pyproject.toml` & `issue_db_api-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools.packages.find]
 where=["."]
 include = ["issue_db_api"]
 
 [project]
 name = "issue_db_api"
-version = "0.9.0"
+version = "0.9.1"
 authors = [
     {name = "Jesse Maarleveld"},
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Rust",
```

