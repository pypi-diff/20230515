# Comparing `tmp/acids-msprior-1.0.8.tar.gz` & `tmp/acids-msprior-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acids-msprior-1.0.8.tar", last modified: Mon May 15 19:53:59 2023, max compression
+gzip compressed data, was "acids-msprior-1.0.9.tar", last modified: Mon May 15 20:47:04 2023, max compression
```

## Comparing `acids-msprior-1.0.8.tar` & `acids-msprior-1.0.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:53:59.324900 acids-msprior-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-15 19:50:25.000000 acids-msprior-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-15 19:53:59.324900 acids-msprior-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-15 19:50:25.000000 acids-msprior-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:53:59.320900 acids-msprior-1.0.8/acids_msprior.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-15 19:53:59.000000 acids-msprior-1.0.8/acids_msprior.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-15 19:53:59.000000 acids-msprior-1.0.8/acids_msprior.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 19:53:59.000000 acids-msprior-1.0.8/acids_msprior.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-15 19:53:59.000000 acids-msprior-1.0.8/acids_msprior.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-15 19:53:59.000000 acids-msprior-1.0.8/acids_msprior.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-15 19:53:59.000000 acids-msprior-1.0.8/acids_msprior.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:53:59.320900 acids-msprior-1.0.8/msprior/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-15 19:50:25.000000 acids-msprior-1.0.8/msprior/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19972 2023-05-15 19:50:25.000000 acids-msprior-1.0.8/msprior/attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:53:59.320900 acids-msprior-1.0.8/msprior/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-15 19:50:25.000000 acids-msprior-1.0.8/msprior/configs/decoder_only.gin
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-15 19:50:25.000000 acids-msprior-1.0.8/msprior/configs/encoder_decoder.gin
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-15 19:50:25.000000 acids-msprior-1.0.8/msprior/configs/encoder_decoder_continuous.gin
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-15 19:50:25.000000 acids-msprior-1.0.8/msprior/configs/recurrent.gin
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-15 19:50:25.000000 acids-msprior-1.0.8/msprior/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-15 19:50:25.000000 acids-msprior-1.0.8/msprior/preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-05-15 19:50:25.000000 acids-msprior-1.0.8/msprior/scripted.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-15 19:50:25.000000 acids-msprior-1.0.8/msprior/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-05-15 19:50:25.000000 acids-msprior-1.0.8/msprior/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:53:59.324900 acids-msprior-1.0.8/msprior_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:50:25.000000 acids-msprior-1.0.8/msprior_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-15 19:50:25.000000 acids-msprior-1.0.8/msprior_scripts/compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-15 19:50:25.000000 acids-msprior-1.0.8/msprior_scripts/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-15 19:50:25.000000 acids-msprior-1.0.8/msprior_scripts/main_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-05-15 19:50:25.000000 acids-msprior-1.0.8/msprior_scripts/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-05-15 19:50:25.000000 acids-msprior-1.0.8/msprior_scripts/train.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-15 19:50:25.000000 acids-msprior-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 19:53:59.324900 acids-msprior-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-15 19:50:25.000000 acids-msprior-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:53:59.324900 acids-msprior-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:50:25.000000 acids-msprior-1.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-15 19:50:25.000000 acids-msprior-1.0.8/tests/test_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-05-15 19:50:25.000000 acids-msprior-1.0.8/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-15 19:50:25.000000 acids-msprior-1.0.8/tests/test_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:04.676706 acids-msprior-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-15 20:47:04.676706 acids-msprior-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:04.672706 acids-msprior-1.0.9/acids_msprior.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-15 20:47:04.000000 acids-msprior-1.0.9/acids_msprior.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-15 20:47:04.000000 acids-msprior-1.0.9/acids_msprior.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 20:47:04.000000 acids-msprior-1.0.9/acids_msprior.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-15 20:47:04.000000 acids-msprior-1.0.9/acids_msprior.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-15 20:47:04.000000 acids-msprior-1.0.9/acids_msprior.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-15 20:47:04.000000 acids-msprior-1.0.9/acids_msprior.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:04.672706 acids-msprior-1.0.9/msprior/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/msprior/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19972 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/msprior/attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:04.672706 acids-msprior-1.0.9/msprior/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/msprior/configs/decoder_only.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/msprior/configs/encoder_decoder.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/msprior/configs/encoder_decoder_continuous.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/msprior/configs/recurrent.gin
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/msprior/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/msprior/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/msprior/scripted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/msprior/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/msprior/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:04.676706 acids-msprior-1.0.9/msprior_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/msprior_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/msprior_scripts/compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/msprior_scripts/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/msprior_scripts/main_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/msprior_scripts/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/msprior_scripts/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 20:47:04.676706 acids-msprior-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:04.676706 acids-msprior-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/tests/test_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/tests/test_configs.py
```

### Comparing `acids-msprior-1.0.8/PKG-INFO` & `acids-msprior-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acids-msprior
-Version: 1.0.8
+Version: 1.0.9
 Summary: MSPRIOR: A multiscale prior model for realtime temporal learning
 Author: Antoine CAILLON
 Author-email: caillon@ircam.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: acids-msprior Version: 1.0.8 Summary: MSPRIOR: A
+Metadata-Version: 2.1 Name: acids-msprior Version: 1.0.9 Summary: MSPRIOR: A
 multiscale prior model for realtime temporal learning Author: Antoine CAILLON
 Author-email: caillon@ircam.fr Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
 markdown # MSPrior ### A multi(scale/stream) prior model for realtime temporal
 learning ## Disclaimer This is an experimental project that *will* be subject
 to lots of changes. ## Installation ```bash pip install acids-msprior ``` ##
```

### Comparing `acids-msprior-1.0.8/README.md` & `acids-msprior-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.8/acids_msprior.egg-info/PKG-INFO` & `acids-msprior-1.0.9/acids_msprior.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acids-msprior
-Version: 1.0.8
+Version: 1.0.9
 Summary: MSPRIOR: A multiscale prior model for realtime temporal learning
 Author: Antoine CAILLON
 Author-email: caillon@ircam.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: acids-msprior Version: 1.0.8 Summary: MSPRIOR: A
+Metadata-Version: 2.1 Name: acids-msprior Version: 1.0.9 Summary: MSPRIOR: A
 multiscale prior model for realtime temporal learning Author: Antoine CAILLON
 Author-email: caillon@ircam.fr Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
 markdown # MSPrior ### A multi(scale/stream) prior model for realtime temporal
 learning ## Disclaimer This is an experimental project that *will* be subject
 to lots of changes. ## Installation ```bash pip install acids-msprior ``` ##
```

### Comparing `acids-msprior-1.0.8/acids_msprior.egg-info/SOURCES.txt` & `acids-msprior-1.0.9/acids_msprior.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.8/msprior/attention.py` & `acids-msprior-1.0.9/msprior/attention.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.8/msprior/configs/decoder_only.gin` & `acids-msprior-1.0.9/msprior/configs/decoder_only.gin`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.8/msprior/configs/encoder_decoder.gin` & `acids-msprior-1.0.9/msprior/configs/encoder_decoder.gin`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.8/msprior/configs/encoder_decoder_continuous.gin` & `acids-msprior-1.0.9/msprior/configs/encoder_decoder_continuous.gin`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.8/msprior/dataset.py` & `acids-msprior-1.0.9/msprior/dataset.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.8/msprior/preprocessor.py` & `acids-msprior-1.0.9/msprior/preprocessor.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.8/msprior/scripted.py` & `acids-msprior-1.0.9/msprior/scripted.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.8/msprior/task.py` & `acids-msprior-1.0.9/msprior/task.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.8/msprior/utils.py` & `acids-msprior-1.0.9/msprior/utils.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.8/msprior_scripts/compact.py` & `acids-msprior-1.0.9/msprior_scripts/compact.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.8/msprior_scripts/export.py` & `acids-msprior-1.0.9/msprior_scripts/export.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.8/msprior_scripts/main_cli.py` & `acids-msprior-1.0.9/msprior_scripts/main_cli.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.8/msprior_scripts/preprocess.py` & `acids-msprior-1.0.9/msprior_scripts/preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,17 @@
                     default=None,
                     required=True,
                     help='Output dataset path')
 flags.DEFINE_string('audio',
                     default=None,
                     required=True,
                     help='Path to the audio files')
-flags.DEFINE_integer('num_secs', default=8, help='Audio chunk size in seconds')
+flags.DEFINE_integer('num_secs',
+                     default=16,
+                     help='Audio chunk size in seconds')
 flags.DEFINE_integer('num_tokens', default=1024, help='Rave vocabulary size')
 flags.DEFINE_integer('batch_size',
                      default=64,
                      help='Batch size during processing')
 flags.DEFINE_multi_string('preprocessor',
                           default=[],
                           help='Additional preprocessors to import')
```

### Comparing `acids-msprior-1.0.8/msprior_scripts/train.py` & `acids-msprior-1.0.9/msprior_scripts/train.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,14 +33,17 @@
                     help="use pretrained embeddings from rave.")
 flags.DEFINE_multi_string("override",
                           default=[],
                           help="additional gin bindings.")
 flags.DEFINE_string("ckpt",
                     default=None,
                     help="checkpoint to resume training from.")
+flags.DEFINE_integer("val_every",
+                     default=1000,
+                     help="validate training every n step.")
 
 
 def add_ext(config: str):
     if config[-4:] != ".gin":
         config += ".gin"
     return config
 
@@ -54,24 +57,30 @@
         overrides.append(f"PRETRAINED_RAVE='{FLAGS.pretrained_embedding}'")
 
     gin.parse_config_files_and_bindings(
         configs,
         overrides,
     )
 
-    logging.info("building model")
-    model = Prior()
-
     logging.info("loading dataset")
     dataset = SequenceDataset(db_path=FLAGS.db_path)
     train, val = data.random_split(
         dataset,
         (len(dataset) - FLAGS.val_size, FLAGS.val_size),
         generator=torch.Generator().manual_seed(42),
     )
+
+    logging.info("quantizer number retrieval")
+    with gin.unlock_config():
+        gin.parse_config(
+            f"NUM_QUANTIZERS={train[0]['decoder_inputs'].shape[-1]}")
+
+    logging.info("building model")
+    model = Prior()
+
     train_loader = data.DataLoader(
         train,
         batch_size=FLAGS.batch_size,
         shuffle=True,
         drop_last=True,
         num_workers=FLAGS.workers,
     )
@@ -84,14 +93,21 @@
     )
 
     os.makedirs(os.path.join("runs", FLAGS.name), exist_ok=False)
     with open(os.path.join("runs", FLAGS.name, "config.gin"),
               "w") as config_out:
         config_out.write(gin.config_str())
 
+    val_check = {}
+    if len(train_loader) >= FLAGS.val_every:
+        val_check["val_check_interval"] = FLAGS.val_every
+    else:
+        nepoch = FLAGS.val_every // len(train_loader)
+        val_check["check_val_every_n_epoch"] = nepoch
+
     logging.info("creating trainer")
     trainer = pl.Trainer(
         logger=pl.loggers.TensorBoardLogger('runs', name=FLAGS.name),
         accelerator='gpu',
         devices=[FLAGS.gpu],
         callbacks=[
             callbacks.LearningRateMonitor(logging_interval='step'),
@@ -100,15 +116,15 @@
             callbacks.ModelCheckpoint(filename='last'),
             callbacks.EarlyStopping(
                 "val_cross_entropy",
                 patience=10,
             )
         ],
         log_every_n_steps=10,
-        val_check_interval=1000,
+        **val_check,
     )
 
     torch.backends.cudnn.benchmark = True
     torch.set_float32_matmul_precision('high')
 
     logging.info("launch training")
     trainer.fit(
```

### Comparing `acids-msprior-1.0.8/setup.py` & `acids-msprior-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.8/tests/test_attention.py` & `acids-msprior-1.0.9/tests/test_attention.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.8/tests/test_cache.py` & `acids-msprior-1.0.9/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.8/tests/test_configs.py` & `acids-msprior-1.0.9/tests/test_configs.py`

 * *Files identical despite different names*

