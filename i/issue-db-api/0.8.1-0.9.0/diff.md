# Comparing `tmp/issue_db_api-0.8.1.tar.gz` & `tmp/issue_db_api-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "issue_db_api-0.8.1.tar", last modified: Thu May 11 12:12:20 2023, max compression
+gzip compressed data, was "issue_db_api-0.9.0.tar", last modified: Mon May 15 11:23:16 2023, max compression
```

## Comparing `issue_db_api-0.8.1.tar` & `issue_db_api-0.9.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-11 12:12:20.397801 issue_db_api-0.8.1/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       82 2023-04-20 09:20:00.000000 issue_db_api-0.8.1/.gitignore
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1069 2023-04-20 08:15:34.000000 issue_db_api-0.8.1/LICENSE
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      103 2023-04-20 08:15:34.000000 issue_db_api-0.8.1/MANIFEST.in
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-11 12:12:20.397801 issue_db_api-0.8.1/PKG-INFO
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      200 2023-04-20 08:15:34.000000 issue_db_api-0.8.1/README.md
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-11 12:12:20.393800 issue_db_api-0.8.1/issue_db_api/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      519 2023-05-11 12:10:29.000000 issue_db_api-0.8.1/issue_db_api/Cargo.toml
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       25 2023-05-04 14:06:56.000000 issue_db_api-0.8.1/issue_db_api/__init__.py
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     8716 2023-05-11 10:14:20.000000 issue_db_api-0.8.1/issue_db_api/issue_api.pyi
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-11 12:12:20.397801 issue_db_api-0.8.1/issue_db_api/src/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    44902 2023-05-11 10:01:47.000000 issue_db_api-0.8.1/issue_db_api/src/api_core.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1049 2023-05-04 13:53:55.000000 issue_db_api-0.8.1/issue_db_api/src/comments.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5322 2023-05-11 12:05:05.000000 issue_db_api-0.8.1/issue_db_api/src/config.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     3788 2023-05-04 13:53:55.000000 issue_db_api-0.8.1/issue_db_api/src/embedding.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     2105 2023-05-04 13:55:29.000000 issue_db_api-0.8.1/issue_db_api/src/errors.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     6635 2023-05-11 12:09:47.000000 issue_db_api-0.8.1/issue_db_api/src/issues.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      571 2023-04-20 08:15:34.000000 issue_db_api-0.8.1/issue_db_api/src/labels.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    39893 2023-05-11 10:14:19.000000 issue_db_api-0.8.1/issue_db_api/src/lib.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    10983 2023-05-04 13:53:55.000000 issue_db_api-0.8.1/issue_db_api/src/models.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     3910 2023-05-01 16:59:08.000000 issue_db_api-0.8.1/issue_db_api/src/query.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     6964 2023-05-11 10:03:52.000000 issue_db_api-0.8.1/issue_db_api/src/repository.rs
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-11 12:12:20.397801 issue_db_api-0.8.1/issue_db_api/src/schemas/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5031 2023-04-20 08:15:34.000000 issue_db_api-0.8.1/issue_db_api/src/schemas/raw_issue_response.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       27 2023-04-20 08:15:34.000000 issue_db_api-0.8.1/issue_db_api/src/schemas.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1626 2023-05-04 13:53:55.000000 issue_db_api-0.8.1/issue_db_api/src/tags.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     2583 2023-05-11 11:58:07.000000 issue_db_api-0.8.1/issue_db_api/src/util.rs
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-11 12:12:20.397801 issue_db_api-0.8.1/issue_db_api.egg-info/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-11 12:12:20.000000 issue_db_api-0.8.1/issue_db_api.egg-info/PKG-INFO
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      748 2023-05-11 12:12:20.000000 issue_db_api-0.8.1/issue_db_api.egg-info/SOURCES.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-05-11 12:12:20.000000 issue_db_api-0.8.1/issue_db_api.egg-info/dependency_links.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.8.1/issue_db_api.egg-info/not-zip-safe
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       13 2023-05-11 12:12:20.000000 issue_db_api-0.8.1/issue_db_api.egg-info/top_level.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      529 2023-05-11 12:10:29.000000 issue_db_api-0.8.1/pyproject.toml
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       38 2023-05-11 12:12:20.397801 issue_db_api-0.8.1/setup.cfg
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      253 2023-04-20 08:15:34.000000 issue_db_api-0.8.1/setup.py
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-15 11:23:16.982522 issue_db_api-0.9.0/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       82 2023-04-20 09:20:00.000000 issue_db_api-0.9.0/.gitignore
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1069 2023-04-20 08:15:34.000000 issue_db_api-0.9.0/LICENSE
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      103 2023-04-20 08:15:34.000000 issue_db_api-0.9.0/MANIFEST.in
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-15 11:23:16.982522 issue_db_api-0.9.0/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      200 2023-04-20 08:15:34.000000 issue_db_api-0.9.0/README.md
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-15 11:23:16.978522 issue_db_api-0.9.0/issue_db_api/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      519 2023-05-15 11:22:45.000000 issue_db_api-0.9.0/issue_db_api/Cargo.toml
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       25 2023-05-04 14:06:56.000000 issue_db_api-0.9.0/issue_db_api/__init__.py
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     9223 2023-05-15 11:22:23.000000 issue_db_api-0.9.0/issue_db_api/issue_api.pyi
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-15 11:23:16.982522 issue_db_api-0.9.0/issue_db_api/src/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    46895 2023-05-15 10:40:01.000000 issue_db_api-0.9.0/issue_db_api/src/api_core.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1049 2023-05-04 13:53:55.000000 issue_db_api-0.9.0/issue_db_api/src/comments.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5322 2023-05-11 12:05:05.000000 issue_db_api-0.9.0/issue_db_api/src/config.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3788 2023-05-04 13:53:55.000000 issue_db_api-0.9.0/issue_db_api/src/embedding.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     2105 2023-05-12 10:30:49.000000 issue_db_api-0.9.0/issue_db_api/src/errors.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1622 2023-05-15 10:43:58.000000 issue_db_api-0.9.0/issue_db_api/src/files.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     6635 2023-05-11 12:09:47.000000 issue_db_api-0.9.0/issue_db_api/src/issues.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      571 2023-04-20 08:15:34.000000 issue_db_api-0.9.0/issue_db_api/src/labels.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    41681 2023-05-15 11:20:32.000000 issue_db_api-0.9.0/issue_db_api/src/lib.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    10983 2023-05-04 13:53:55.000000 issue_db_api-0.9.0/issue_db_api/src/models.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3910 2023-05-01 16:59:08.000000 issue_db_api-0.9.0/issue_db_api/src/query.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     7521 2023-05-15 11:20:32.000000 issue_db_api-0.9.0/issue_db_api/src/repository.rs
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-15 11:23:16.982522 issue_db_api-0.9.0/issue_db_api/src/schemas/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5031 2023-04-20 08:15:34.000000 issue_db_api-0.9.0/issue_db_api/src/schemas/raw_issue_response.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       27 2023-04-20 08:15:34.000000 issue_db_api-0.9.0/issue_db_api/src/schemas.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1626 2023-05-04 13:53:55.000000 issue_db_api-0.9.0/issue_db_api/src/tags.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     2583 2023-05-11 11:58:07.000000 issue_db_api-0.9.0/issue_db_api/src/util.rs
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-15 11:23:16.978522 issue_db_api-0.9.0/issue_db_api.egg-info/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-15 11:23:16.000000 issue_db_api-0.9.0/issue_db_api.egg-info/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      774 2023-05-15 11:23:16.000000 issue_db_api-0.9.0/issue_db_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-05-15 11:23:16.000000 issue_db_api-0.9.0/issue_db_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.9.0/issue_db_api.egg-info/not-zip-safe
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       13 2023-05-15 11:23:16.000000 issue_db_api-0.9.0/issue_db_api.egg-info/top_level.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      529 2023-05-15 11:22:45.000000 issue_db_api-0.9.0/pyproject.toml
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       38 2023-05-15 11:23:16.982522 issue_db_api-0.9.0/setup.cfg
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      253 2023-04-20 08:15:34.000000 issue_db_api-0.9.0/setup.py
```

### Comparing `issue_db_api-0.8.1/LICENSE` & `issue_db_api-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.8.1/PKG-INFO` & `issue_db_api-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issue_db_api
-Version: 0.8.1
+Version: 0.9.0
 Author: Jesse Maarleveld
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `issue_db_api-0.8.1/issue_db_api/Cargo.toml` & `issue_db_api-0.9.0/issue_db_api/Cargo.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "issue-api-client"
-version = "0.8.1"
+version = "0.9.0"
 edition = "2021"
 
 [lib]
 name = "issue_api"
 crate-type = ["cdylib"]
 
 [features]
```

### Comparing `issue_db_api-0.8.1/issue_db_api/issue_api.pyi` & `issue_db_api-0.9.0/issue_db_api/issue_api.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -83,14 +83,23 @@
 
     def add_model(self, name: str, config: dict[str, typing.Any]) -> Model:
         ...
 
     def delete_model_config(self, model: Model):
         ...
 
+    def files(self, category: str = None) -> list[File]:
+        ...
+
+    def upload_file(self, path: str, description: str, category: str) -> File:
+        ...
+
+    def delete_file(self, file: File):
+        ...
+
 
 class Repo:
     def __repr__(self) -> str:
         ...
 
     @property
     def name(self) -> str:
@@ -493,7 +502,28 @@
     @property
     def description(self) -> str:
         ...
 
     @description.setter
     def description(self, description: str):
         ...
+
+
+class File:
+
+    def __repr__(self) -> str:
+        ...
+
+    def __eq__(self, other) -> bool:
+        ...
+
+    def identifier(self) -> str:
+        ...
+
+    def description(self) -> str:
+        ...
+
+    def category(self) -> str:
+        ...
+
+    def download(self, path: str):
+        ...
```

### Comparing `issue_db_api-0.8.1/issue_db_api/src/api_core.rs` & `issue_db_api-0.9.0/issue_db_api/src/api_core.rs`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 use crate::schemas::raw_issue_response::RawIssueData;
 use crate::query::Query;
 use crate::labels::Label;
 use crate::tags::UnboundTag;
 use crate::util::initialize_lazy_field;
 use crate::errors::APIResult;
 use crate::errors::*;
+use crate::files::UnboundFile;
 use crate::models::{ModelInfo, UnboundModelConfig, UnboundModelVersion, UnboundTestRun};
 
 //////////////////////////////////////////////////////////////////////////////////////////////////
 //////////////////////////////////////////////////////////////////////////////////////////////////
 // Core Structs
 //////////////////////////////////////////////////////////////////////////////////////////////////
 
@@ -1159,8 +1160,61 @@
                                                  performance_id: String,
                                                  description: String) -> APIResult<()> {
         let endpoint = format!("models/{}/performances/{}/description", model_id, performance_id);
         let mut map = Map::new();
         map.insert("description".to_string(), Value::String(description));
         self.call_endpoint_json(endpoint.as_str(), Verb::Put, Value::Object(map))
     }
+
+    /***************************************************************************
+     * Generic File API 
+     */
+    
+    pub(crate) fn get_all_files(&self, category: Option<String>) -> APIResult<Vec<UnboundFile>> {
+        let mut map = Map::new();
+        map.insert(
+            "category".to_string(), 
+            match category {
+                None => Value::Null,
+                Some(c) => Value::String(c)
+        });
+        let response = self.call_endpoint_json::<_, Vec<UnboundFile>>(
+            "files", Verb::Get, Value::Object(map)
+        )?;
+        Ok(response) 
+    }
+    
+    pub(crate) fn upload_file(&self, path: String, description: String, category: String) -> APIResult<String> {
+        #[derive(serde::Deserialize)]
+        struct UploadFileResponse {
+            file_id: String 
+        }
+        let form = multipart::Form::new()
+            .file("file", path)?
+            .text("description", description)
+            .text("category", category);
+        let response = self.call_endpoint_multipart::<UploadFileResponse>(
+            "files", Verb::Post, form
+        )?;
+        Ok(response.file_id)
+    }
+    
+    pub(crate) fn get_file(&self, file_id: String) -> APIResult<UnboundFile> {
+        let endpoint = format!("files/{}", file_id);
+        let response = self.call_endpoint_json::<_, UnboundFile>(
+            endpoint.as_str(), Verb::Get, Value::Object(Map::new())
+        )?;
+        Ok(response)
+    }
+    
+    pub(crate) fn delete_file(&self, file_id: String) -> APIResult<()> {
+        let endpoint = format!("files/{}", file_id);
+        self.call_endpoint_json(endpoint.as_str(), Verb::Delete, Value::Object(Map::new()))
+    }
+    
+    pub(crate) fn download_file(&self, file_id: String, path: String) -> APIResult<()> {
+        let endpoint = format!("files/{file_id}/file");
+        self.call_endpoint_download(
+            endpoint.as_str(), Verb::Get, Value::Object(Map::new()), path
+        )
+    }
 }
```

### Comparing `issue_db_api-0.8.1/issue_db_api/src/comments.rs` & `issue_db_api-0.9.0/issue_db_api/src/comments.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.8.1/issue_db_api/src/config.rs` & `issue_db_api-0.9.0/issue_db_api/src/config.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.8.1/issue_db_api/src/embedding.rs` & `issue_db_api-0.9.0/issue_db_api/src/embedding.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.8.1/issue_db_api/src/errors.rs` & `issue_db_api-0.9.0/issue_db_api/src/errors.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.8.1/issue_db_api/src/issues.rs` & `issue_db_api-0.9.0/issue_db_api/src/issues.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.8.1/issue_db_api/src/labels.rs` & `issue_db_api-0.9.0/issue_db_api/src/labels.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.8.1/issue_db_api/src/lib.rs` & `issue_db_api-0.9.0/issue_db_api/src/lib.rs`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 mod tags;
 mod embedding;
 mod comments;
 mod issues;
 mod config;
 mod errors;
 mod models;
+mod files;
 
 pub use repository::IssueRepository;
 pub use errors::APIResult;
 pub use query::{Query, QueryCMP};
 
 
 #[cfg(feature = "pyo3")]
@@ -33,14 +34,15 @@
     use crate::errors::APIError;
     use crate::issues::Issue;
     use crate::labels::Label;
     use crate::models::{Model, ModelVersion, TestRun};
     use crate::repository::IssueRepo;
     use crate::tags::{Tag, TagType};
     use crate::errors::APIResult;
+    use crate::files::File;
     use super::*;
 
     create_exception!(issue_api, IssueAPIError, PyException);
     create_exception!(issue_api, InvalidCredentialsException, IssueAPIError);
     create_exception!(issue_api, NotAuthorizedException, IssueAPIError);
     create_exception!(issue_api, InvalidTokenException, IssueAPIError);
     create_exception!(issue_api, HTTPException, IssueAPIError);
@@ -356,14 +358,31 @@
             Ok(PyModel{inner: model})
         }
 
         fn delete_model_config(&self, model: &PyModel) -> PyResult<()> {
             api2py_error(self.repo.delete_model_config_by_id(model.inner.identifier()))
 
         }
+
+        fn files(&self, category: Option<String>) -> PyResult<Vec<PyFile>> {
+            let result = api2py_error(self.repo.files(category))?
+                .into_iter().map(|f| PyFile{inner: f})
+                .collect();
+            Ok(result)
+        }
+
+        fn upload_file(&self, path: String, description: String, category: String) -> PyResult<PyFile> {
+            Ok(
+                PyFile{inner: api2py_error(self.repo.upload_file(path, description, category))?}
+            )
+        }
+
+        fn delete_file(&self, file: &PyFile) -> PyResult<()> {
+            api2py_error(self.repo.remove_file(file.inner.clone()))
+        }
     }
 
     #[pyclass(name="IssueRepo")]
     struct PyRepo {
         inner: IssueRepo
     }
 
@@ -1155,14 +1174,53 @@
 
         #[setter]
         pub fn set_description(&mut self, description: String) -> PyResult<()> {
             api2py_error(self.inner.update_description(description))
         }
     }
 
+    #[pyclass(name="File")]
+    #[allow(unused)]
+    struct PyFile {
+        inner: File
+    }
+
+    #[pymethods]
+    impl PyFile {
+        fn __repr__(&self) -> PyResult<String> {
+            let text = format!("<File|id={}>", self.inner.identifier());
+            Ok(text)
+        }
+
+        fn __richcmp__(&self, other: PyRef<PyFile>, op: CompareOp) -> Py<PyAny> {
+            let py = other.py();
+            match op {
+                CompareOp::Eq => (self.inner == other.inner).into_py(py),
+                CompareOp::Ne => (self.inner != other.inner).into_py(py),
+                _ => py.NotImplemented(),
+            }
+        }
+
+        fn identifier(&self) -> PyResult<String> {
+            Ok(self.inner.identifier())
+        }
+
+        fn description(&self) -> PyResult<String> {
+            Ok(self.inner.description())
+        }
+
+        fn category(&self) -> PyResult<String> {
+            Ok(self.inner.category())
+        }
+
+        fn download(&self, path: String) -> PyResult<()> {
+            api2py_error(self.inner.download(path))
+        }
+    }
+
     #[pymodule]
     fn issue_api(py: Python<'_>, m: &PyModule) -> PyResult<()> {
         m.add("IssueAPIError", py.get_type::<IssueAPIError>())?;
         m.add("InvalidCredentialsException", py.get_type::<InvalidCredentialsException>())?;
         m.add("NotAuthorizedException", py.get_type::<NotAuthorizedException>())?;
         m.add("InvalidTokenException", py.get_type::<InvalidTokenException>())?;
         m.add("HTTPException", py.get_type::<HTTPException>())?;
@@ -1174,10 +1232,11 @@
         m.add_class::<PyRepo>()?;
         m.add_class::<PyTag>()?;
         m.add_class::<PyModel>()?;
         m.add_class::<PyVersion>()?;
         m.add_class::<PyPerformance>()?;
         m.add_class::<PyComment>()?;
         m.add_class::<PyEmbedding>()?;
+        m.add_class::<PyFile>()?;
         Ok(())
     }
 }
```

### Comparing `issue_db_api-0.8.1/issue_db_api/src/models.rs` & `issue_db_api-0.9.0/issue_db_api/src/models.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.8.1/issue_db_api/src/query.rs` & `issue_db_api-0.9.0/issue_db_api/src/query.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.8.1/issue_db_api/src/repository.rs` & `issue_db_api-0.9.0/issue_db_api/src/repository.rs`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 use crate::config::{CachingPolicy, IssueLoadingSettings, ConfigHandlingPolicy};
 use crate::embedding::Embedding;
 use crate::issues::Issue;
 use crate::models::Model;
 use crate::query::Query;
 use crate::tags::Tag;
 use crate::errors::APIResult;
+use crate::files::File;
 
 
 #[allow(unused)]
 #[derive(Debug)]
 pub struct IssueRepository {
     label_caching: CachingPolicy,
     config_handling: ConfigHandlingPolicy,
@@ -195,14 +196,30 @@
     pub fn delete_model_config(&self, model: Model) -> APIResult<()> {
         self.api.delete_model_config(model.identifier())
     }
 
     pub(crate) fn delete_model_config_by_id(&self, id: String) -> APIResult<()> {
         self.api.delete_model_config(id)
     }
+
+    pub fn files(&self, category: Option<String>) -> APIResult<Vec<File>> {
+        let result = self.api
+            .get_all_files(category)?
+            .into_iter().map(|f| f.into_bound_file(self.api.clone()))
+            .collect();
+        Ok(result)
+    }
+
+    pub fn upload_file(&self, path: String, description: String, category: String) -> APIResult<File> {
+        File::upload(self.api.clone(), path, description, category)
+    }
+
+    pub fn remove_file(&self, file: File) -> APIResult<()> {
+        file.delete()
+    }
 }
 
 
 pub struct IssueRepo {
     name: String,
     api: Arc<IssueAPI>
 }
```

### Comparing `issue_db_api-0.8.1/issue_db_api/src/schemas/raw_issue_response.rs` & `issue_db_api-0.9.0/issue_db_api/src/schemas/raw_issue_response.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.8.1/issue_db_api/src/tags.rs` & `issue_db_api-0.9.0/issue_db_api/src/tags.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.8.1/issue_db_api/src/util.rs` & `issue_db_api-0.9.0/issue_db_api/src/util.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.8.1/issue_db_api.egg-info/PKG-INFO` & `issue_db_api-0.9.0/issue_db_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issue-db-api
-Version: 0.8.1
+Version: 0.9.0
 Author: Jesse Maarleveld
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `issue_db_api-0.8.1/issue_db_api.egg-info/SOURCES.txt` & `issue_db_api-0.9.0/issue_db_api.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 issue_db_api.egg-info/not-zip-safe
 issue_db_api.egg-info/top_level.txt
 issue_db_api/src/api_core.rs
 issue_db_api/src/comments.rs
 issue_db_api/src/config.rs
 issue_db_api/src/embedding.rs
 issue_db_api/src/errors.rs
+issue_db_api/src/files.rs
 issue_db_api/src/issues.rs
 issue_db_api/src/labels.rs
 issue_db_api/src/lib.rs
 issue_db_api/src/models.rs
 issue_db_api/src/query.rs
 issue_db_api/src/repository.rs
 issue_db_api/src/schemas.rs
```

### Comparing `issue_db_api-0.8.1/pyproject.toml` & `issue_db_api-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools.packages.find]
 where=["."]
 include = ["issue_db_api"]
 
 [project]
 name = "issue_db_api"
-version = "0.8.1"
+version = "0.9.0"
 authors = [
     {name = "Jesse Maarleveld"},
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Rust",
```

