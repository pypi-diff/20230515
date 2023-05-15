# Comparing `tmp/embedbase-1.1.5.tar.gz` & `tmp/embedbase-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedbase-1.1.5.tar", max compression
+gzip compressed data, was "embedbase-1.1.6.tar", max compression
```

## Comparing `embedbase-1.1.5.tar` & `embedbase-1.1.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1069 2023-05-14 08:01:24.202878 embedbase-1.1.5/LICENSE
--rw-r--r--   0        0        0     4905 2023-05-14 08:01:24.202878 embedbase-1.1.5/README.md
--rw-r--r--   0        0        0      121 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/__init__.py
--rw-r--r--   0        0        0     1646 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/__main__.py
--rw-r--r--   0        0        0      976 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/api.py
--rw-r--r--   0        0        0    16416 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/app.py
--rw-r--r--   0        0        0       88 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/database/__init__.py
--rw-r--r--   0        0        0     3505 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/database/base.py
--rw-r--r--   0        0        0     5939 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/database/memory_db.py
--rw-r--r--   0        0        0     9702 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/database/postgres_db.py
--rw-r--r--   0        0        0     6620 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/database/supabase_db.py
--rw-r--r--   0        0        0       77 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/embedding/__init__.py
--rw-r--r--   0        0        0      858 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/embedding/base.py
--rw-r--r--   0        0        0     1237 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/embedding/cohere.py
--rw-r--r--   0        0        0     2059 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/embedding/openai.py
--rw-r--r--   0        0        0     1551 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/firebase_auth.py
--rw-r--r--   0        0        0      690 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/logging_utils.py
--rw-r--r--   0        0        0      802 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/models.py
--rw-r--r--   0        0        0     1285 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/settings.py
--rw-r--r--   0        0        0     3208 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/strings.py
--rw-r--r--   0        0        0      301 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/supabase_auth.py
--rw-r--r--   0        0        0     3867 2023-05-14 08:01:24.266878 embedbase-1.1.5/embedbase/utils.py
--rw-r--r--   0        0        0     3669 2023-05-14 08:01:24.270878 embedbase-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     6343 1970-01-01 00:00:00.000000 embedbase-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-15 09:33:25.482964 embedbase-1.1.6/LICENSE
+-rw-r--r--   0        0        0     4905 2023-05-15 09:33:25.482964 embedbase-1.1.6/README.md
+-rw-r--r--   0        0        0      121 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/__init__.py
+-rw-r--r--   0        0        0     1716 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/__main__.py
+-rw-r--r--   0        0        0      976 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/api.py
+-rw-r--r--   0        0        0    16416 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/app.py
+-rw-r--r--   0        0        0       88 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/database/__init__.py
+-rw-r--r--   0        0        0     3505 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/database/base.py
+-rw-r--r--   0        0        0     5939 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/database/memory_db.py
+-rw-r--r--   0        0        0     9901 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/database/postgres_db.py
+-rw-r--r--   0        0        0     6827 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/database/supabase_db.py
+-rw-r--r--   0        0        0       77 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/embedding/__init__.py
+-rw-r--r--   0        0        0      858 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/embedding/base.py
+-rw-r--r--   0        0        0     1237 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/embedding/cohere.py
+-rw-r--r--   0        0        0     2059 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/embedding/openai.py
+-rw-r--r--   0        0        0     1551 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/firebase_auth.py
+-rw-r--r--   0        0        0      690 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/logging_utils.py
+-rw-r--r--   0        0        0      802 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/models.py
+-rw-r--r--   0        0        0     1285 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/settings.py
+-rw-r--r--   0        0        0     3208 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/strings.py
+-rw-r--r--   0        0        0      301 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/supabase_auth.py
+-rw-r--r--   0        0        0     3867 2023-05-15 09:33:25.554965 embedbase-1.1.6/embedbase/utils.py
+-rw-r--r--   0        0        0     3669 2023-05-15 09:33:25.558965 embedbase-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0     6343 1970-01-01 00:00:00.000000 embedbase-1.1.6/PKG-INFO
```

### Comparing `embedbase-1.1.5/LICENSE` & `embedbase-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.5/README.md` & `embedbase-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.5/embedbase/__main__.py` & `embedbase-1.1.6/embedbase/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+A simple example to try a local and privacy-first embedbase.
+"""
+
 from typing import List, Union
 import uvicorn
 from embedbase import get_app
 from embedbase.database.memory_db import MemoryDatabase
 from embedbase.embedding.base import Embedder
 from sentence_transformers import SentenceTransformer
```

### Comparing `embedbase-1.1.5/embedbase/api.py` & `embedbase-1.1.6/embedbase/api.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.5/embedbase/app.py` & `embedbase-1.1.6/embedbase/app.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.5/embedbase/database/base.py` & `embedbase-1.1.6/embedbase/database/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.5/embedbase/database/memory_db.py` & `embedbase-1.1.6/embedbase/database/memory_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.5/embedbase/database/postgres_db.py` & `embedbase-1.1.6/embedbase/database/postgres_db.py`

 * *Files 5% similar despite different names*

```diff
@@ -196,14 +196,16 @@
                 row.data if store_data else None,
                 row.embedding,
                 row.hash,
                 dataset_id,
                 user_id,
                 json.dumps(row.metadata),
             ]
+            # {'code': '22P05', 'details': '\\u0000 cannot be converted to text.', 'hint': None, 'message': 'unsupported Unicode escape sequence'}
+            row.data = row.data.replace("\x00", "")
             return data
 
         values = [tuple(_d(row)) for _, row in df.iterrows()]
         num_columns = len(values[0])
         placeholders = ", ".join(
             ["(" + ", ".join(["%s"] * num_columns) + ")"] * len(values)
         )
```

### Comparing `embedbase-1.1.5/embedbase/database/supabase_db.py` & `embedbase-1.1.6/embedbase/database/supabase_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,16 @@
                     "id": row.id,
                     "embedding": row.embedding,
                     "hash": row.hash,
                     "dataset_id": dataset_id,
                     "user_id": user_id,
                     "metadata": row.metadata,
                 }
+                # {'code': '22P05', 'details': '\\u0000 cannot be converted to text.', 'hint': None, 'message': 'unsupported Unicode escape sequence'}
+                row.data = row.data.replace("\x00", "")
                 if store_data:
                     data["data"] = row.data
                 return data
 
             (
                 self.supabase.table("documents")
                 .upsert([_d(row) for _, row in batch_df.iterrows()])
```

### Comparing `embedbase-1.1.5/embedbase/embedding/base.py` & `embedbase-1.1.6/embedbase/embedding/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.5/embedbase/embedding/cohere.py` & `embedbase-1.1.6/embedbase/embedding/cohere.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.5/embedbase/embedding/openai.py` & `embedbase-1.1.6/embedbase/embedding/openai.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.5/embedbase/firebase_auth.py` & `embedbase-1.1.6/embedbase/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.5/embedbase/logging_utils.py` & `embedbase-1.1.6/embedbase/logging_utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.5/embedbase/models.py` & `embedbase-1.1.6/embedbase/models.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.5/embedbase/settings.py` & `embedbase-1.1.6/embedbase/settings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.5/embedbase/strings.py` & `embedbase-1.1.6/embedbase/strings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.5/embedbase/utils.py` & `embedbase-1.1.6/embedbase/utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.5/pyproject.toml` & `embedbase-1.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "embedbase"
-version = "1.1.5"
+version = "1.1.6"
 description = "API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings."
 readme = "README.md"
 authors = ["Different AI <louis@embedbase.xyz>"]
 license = "MIT"
 repository = "https://github.com/different-ai/embedbase"
 homepage = "https://github.com/different-ai/embedbase"
 keywords = ["embeddings", "machine learning", "artificial intelligence"]
```

### Comparing `embedbase-1.1.5/PKG-INFO` & `embedbase-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedbase
-Version: 1.1.5
+Version: 1.1.6
 Summary: API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings.
 Home-page: https://github.com/different-ai/embedbase
 License: MIT
 Keywords: embeddings,machine learning,artificial intelligence
 Author: Different AI
 Author-email: louis@embedbase.xyz
 Requires-Python: >=3.8,<4.0
```

