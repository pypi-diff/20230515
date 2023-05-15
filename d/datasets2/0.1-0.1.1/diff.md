# Comparing `tmp/datasets2-0.1.tar.gz` & `tmp/datasets2-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasets2-0.1.tar", last modified: Fri Apr 28 02:50:20 2023, max compression
+gzip compressed data, was "datasets2-0.1.1.tar", last modified: Mon May 15 20:57:08 2023, max compression
```

## Comparing `datasets2-0.1.tar` & `datasets2-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:50:20.322569 datasets2-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-28 02:50:20.322569 datasets2-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-28 02:50:09.000000 datasets2-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:50:20.322569 datasets2-0.1/datasets2/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-28 02:50:09.000000 datasets2-0.1/datasets2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-28 02:50:09.000000 datasets2-0.1/datasets2/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-04-28 02:50:09.000000 datasets2-0.1/datasets2/save.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:50:20.322569 datasets2-0.1/datasets2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-28 02:50:20.000000 datasets2-0.1/datasets2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-28 02:50:20.000000 datasets2-0.1/datasets2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 02:50:20.000000 datasets2-0.1/datasets2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 02:50:20.000000 datasets2-0.1/datasets2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 02:50:20.000000 datasets2-0.1/datasets2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 02:50:20.000000 datasets2-0.1/datasets2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 02:50:20.322569 datasets2-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-28 02:50:09.000000 datasets2-0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:50:20.322569 datasets2-0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 02:50:09.000000 datasets2-0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-04-28 02:50:09.000000 datasets2-0.1/tests/test_save_as_parquet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:57:08.938389 datasets2-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-15 20:57:08.938389 datasets2-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-15 20:56:59.000000 datasets2-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:57:08.934389 datasets2-0.1.1/datasets2/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-15 20:56:59.000000 datasets2-0.1.1/datasets2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-15 20:56:59.000000 datasets2-0.1.1/datasets2/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-05-15 20:56:59.000000 datasets2-0.1.1/datasets2/save.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:57:08.938389 datasets2-0.1.1/datasets2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-15 20:57:08.000000 datasets2-0.1.1/datasets2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-15 20:57:08.000000 datasets2-0.1.1/datasets2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 20:57:08.000000 datasets2-0.1.1/datasets2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 20:57:08.000000 datasets2-0.1.1/datasets2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 20:57:08.000000 datasets2-0.1.1/datasets2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 20:57:08.000000 datasets2-0.1.1/datasets2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 20:57:08.938389 datasets2-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-15 20:56:59.000000 datasets2-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:57:08.938389 datasets2-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:56:59.000000 datasets2-0.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-05-15 20:56:59.000000 datasets2-0.1.1/tests/test_save_as_parquet.py
```

### Comparing `datasets2-0.1/PKG-INFO` & `datasets2-0.1.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: datasets2
-Version: 0.1
+Version: 0.1.1
 Summary: Add-ons to the huggingface `datasets`
-Home-page: 
-Author: 
-Author-email: 
+Home-page: https://github.com/zzsi/datasets2
+Author: ZZ Si
+Author-email: zhangzhang.si@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 `datasets2` provides add-ons to the huggingface `datasets`.
 
 Example usage:
```

### Comparing `datasets2-0.1/README.md` & `datasets2-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `datasets2-0.1/datasets2/load.py` & `datasets2-0.1.1/datasets2/load.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,18 @@
         if filename.endswith(".parquet") and filename.startswith(split + "-"):
             yield os.path.join(directory, filename)
 
 
 def load_dataset(path, *args, **kwargs):
     """
     Extends datasets.load_dataset to support loading from parquet files.
+
+    # TODO: it currently downloads the parquet files to the tmp folder.
+    e.g. Downloading and preparing dataset parquet/default to /root/.cache/huggingface/datasets/parquet
+    This is not necessary.
     """
     if there_exist_parquet_files_in_this_directory(path):
         if dataset_info_says_buider_is_parquet(path):
             dataset_info = load_dataset_info(path)
             data_files = {}
             for split in dataset_info.splits:
                 data_files[split] = sorted(
```

### Comparing `datasets2-0.1/datasets2/save.py` & `datasets2-0.1.1/datasets2/save.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,21 +46,25 @@
             num_shards=num_shards,
         )
         infos.append(info)
 
     # Merge the infos.
     merged_info = infos[0]
     dataset_sizes = [i.dataset_size for i in infos]
+    dataset_sizes = [x for x in dataset_sizes if x is not None]
     sizes_in_bytes = [i.size_in_bytes for i in infos]
+    sizes_in_bytes = [x for x in sizes_in_bytes if x is not None]
     split_infos = [i.splits for i in infos]
     data_files = []
     for i in infos:
         data_files.extend(i.data_files)
-    merged_info.dataset_size = sum(dataset_sizes)
-    merged_info.size_in_bytes = sum(sizes_in_bytes)
+    if len(dataset_sizes) > 0:
+        merged_info.dataset_size = sum(dataset_sizes)
+    if len(sizes_in_bytes) > 0:
+        merged_info.size_in_bytes = sum(sizes_in_bytes)
     splits = {}
     for split_info in split_infos:
         for k, v in split_info.items():
             splits[k] = v
     merged_info.splits = splits
     # merged_info.data_files = data_files  # This is not saved anyway.
     merged_info.builder_name = "parquet"
@@ -84,22 +88,27 @@
             for k, v in ds._info.features.items()
             if require_decoding(v, ignore_decode_attribute=True)
         ]
         if embed_external_files
         else []
     )
 
-    dataset_nbytes = ds._estimate_nbytes()
+    if hasattr(ds, "_estimate_nbytes"):
+        dataset_nbytes = ds._estimate_nbytes()
 
-    if num_shards is None:
-        max_shard_size = convert_file_size_to_int(
-            max_shard_size or datasets_config.MAX_SHARD_SIZE
-        )
-        num_shards = int(dataset_nbytes / max_shard_size) + 1
-        num_shards = max(num_shards, 1)
+        if num_shards is None:
+            max_shard_size = convert_file_size_to_int(
+                max_shard_size or datasets_config.MAX_SHARD_SIZE
+            )
+            num_shards = int(dataset_nbytes / max_shard_size) + 1
+            num_shards = max(num_shards, 1)
+    else:
+        dataset_nbytes = None
+        if num_shards is None:
+            num_shards = 1
 
     shards = (
         ds.shard(num_shards=num_shards, index=i, contiguous=True)
         for i in range(num_shards)
     )
 
     if decodable_columns:
@@ -129,17 +138,17 @@
     for index, shard in tqdm.tqdm(
         enumerate(itertools.chain([first_shard], shards_iter)),
         desc="preparing dataset shards",
         total=num_shards,
         # disable=not logging.is_progress_bar_enabled(),
     ):
         shard_path_in_repo = path_in_repo(index, shard)
-        print("")
-        print(shard_path_in_repo)
-        print(type(shard))
+        # print("")
+        # print(shard_path_in_repo)
+        # print(type(shard))
         shard.to_parquet(shard_path_in_repo)
         shards_path_in_repo.append(str(shard_path_in_repo))
 
     # Populate dataset info.
     info_to_dump = ds.info.copy()
     info_to_dump.dataset_size = dataset_nbytes
     info_to_dump.size_in_bytes = dataset_nbytes
```

### Comparing `datasets2-0.1/datasets2.egg-info/PKG-INFO` & `datasets2-0.1.1/datasets2.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: datasets2
-Version: 0.1
+Version: 0.1.1
 Summary: Add-ons to the huggingface `datasets`
-Home-page: 
-Author: 
-Author-email: 
+Home-page: https://github.com/zzsi/datasets2
+Author: ZZ Si
+Author-email: zhangzhang.si@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 `datasets2` provides add-ons to the huggingface `datasets`.
 
 Example usage:
```

### Comparing `datasets2-0.1/setup.py` & `datasets2-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,19 +5,19 @@
     install_requires = f.read().splitlines()
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="datasets2",
-    version="0.1",
+    version="0.1.1",
     description="Add-ons to the huggingface `datasets`",
-    url="",
-    author="",
-    author_email="",
+    url="https://github.com/zzsi/datasets2",
+    author="ZZ Si",
+    author_email="zhangzhang.si@gmail.com",
     license="MIT",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires=">=3.6",
     install_requires=install_requires,
     include_package_data=True,
```

### Comparing `datasets2-0.1/tests/test_save_as_parquet.py` & `datasets2-0.1.1/tests/test_save_as_parquet.py`

 * *Files identical despite different names*

