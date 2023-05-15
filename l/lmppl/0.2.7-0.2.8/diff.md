# Comparing `tmp/lmppl-0.2.7.tar.gz` & `tmp/lmppl-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmppl-0.2.7.tar", last modified: Fri May 12 20:53:41 2023, max compression
+gzip compressed data, was "lmppl-0.2.8.tar", last modified: Mon May 15 21:11:12 2023, max compression
```

## Comparing `lmppl-0.2.7.tar` & `lmppl-0.2.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-12 20:53:41.926712 lmppl-0.2.7/
--rw-r--r--   0 asahi      (501) staff       (20)     1064 2023-02-07 11:28:13.000000 lmppl-0.2.7/LICENSE.txt
--rw-r--r--   0 asahi      (501) staff       (20)     5200 2023-05-12 20:53:41.926902 lmppl-0.2.7/PKG-INFO
--rw-r--r--   0 asahi      (501) staff       (20)     4437 2023-02-09 18:23:49.000000 lmppl-0.2.7/README.md
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-12 20:53:41.921659 lmppl-0.2.7/lmppl/
--rw-r--r--   0 asahi      (501) staff       (20)      150 2023-04-05 16:38:19.000000 lmppl-0.2.7/lmppl/__init__.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-12 20:53:41.924384 lmppl-0.2.7/lmppl/lmppl_cl/
--rw-r--r--   0 asahi      (501) staff       (20)        0 2023-02-07 11:25:50.000000 lmppl-0.2.7/lmppl/lmppl_cl/__init__.py
--rw-r--r--   0 asahi      (501) staff       (20)     2688 2023-05-12 20:52:46.000000 lmppl-0.2.7/lmppl/openai_models.py
--rw-r--r--   0 asahi      (501) staff       (20)     8597 2023-04-01 16:15:20.000000 lmppl-0.2.7/lmppl/ppl_encoder_decoder_lm.py
--rw-r--r--   0 asahi      (501) staff       (20)     6883 2023-03-10 20:47:02.000000 lmppl-0.2.7/lmppl/ppl_mlm.py
--rw-r--r--   0 asahi      (501) staff       (20)     5709 2023-05-01 10:56:55.000000 lmppl-0.2.7/lmppl/ppl_recurrent_lm.py
--rw-r--r--   0 asahi      (501) staff       (20)      227 2023-02-07 13:19:37.000000 lmppl-0.2.7/lmppl/util.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-12 20:53:41.923906 lmppl-0.2.7/lmppl.egg-info/
--rw-r--r--   0 asahi      (501) staff       (20)     5200 2023-05-12 20:53:41.000000 lmppl-0.2.7/lmppl.egg-info/PKG-INFO
--rw-r--r--   0 asahi      (501) staff       (20)      399 2023-05-12 20:53:41.000000 lmppl-0.2.7/lmppl.egg-info/SOURCES.txt
--rw-r--r--   0 asahi      (501) staff       (20)        1 2023-05-12 20:53:41.000000 lmppl-0.2.7/lmppl.egg-info/dependency_links.txt
--rw-r--r--   0 asahi      (501) staff       (20)       79 2023-05-12 20:53:41.000000 lmppl-0.2.7/lmppl.egg-info/requires.txt
--rw-r--r--   0 asahi      (501) staff       (20)        6 2023-05-12 20:53:41.000000 lmppl-0.2.7/lmppl.egg-info/top_level.txt
--rw-r--r--   0 asahi      (501) staff       (20)       38 2023-05-12 20:53:41.927391 lmppl-0.2.7/setup.cfg
--rw-r--r--   0 asahi      (501) staff       (20)     1760 2023-05-12 20:53:11.000000 lmppl-0.2.7/setup.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-12 20:53:41.925785 lmppl-0.2.7/test/
--rw-r--r--   0 asahi      (501) staff       (20)     1249 2023-02-09 19:14:51.000000 lmppl-0.2.7/test/test_analogy.py
--rw-r--r--   0 asahi      (501) staff       (20)     2261 2023-02-12 13:50:45.000000 lmppl-0.2.7/test/test_model_with_simple_input.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-15 21:11:12.000130 lmppl-0.2.8/
+-rw-r--r--   0 asahi      (501) staff       (20)     1064 2023-02-07 11:28:13.000000 lmppl-0.2.8/LICENSE.txt
+-rw-r--r--   0 asahi      (501) staff       (20)     5200 2023-05-15 21:11:12.000280 lmppl-0.2.8/PKG-INFO
+-rw-r--r--   0 asahi      (501) staff       (20)     4437 2023-02-09 18:23:49.000000 lmppl-0.2.8/README.md
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-15 21:11:11.995499 lmppl-0.2.8/lmppl/
+-rw-r--r--   0 asahi      (501) staff       (20)      150 2023-04-05 16:38:19.000000 lmppl-0.2.8/lmppl/__init__.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-15 21:11:11.998285 lmppl-0.2.8/lmppl/lmppl_cl/
+-rw-r--r--   0 asahi      (501) staff       (20)        0 2023-02-07 11:25:50.000000 lmppl-0.2.8/lmppl/lmppl_cl/__init__.py
+-rw-r--r--   0 asahi      (501) staff       (20)     2688 2023-05-12 20:52:46.000000 lmppl-0.2.8/lmppl/openai_models.py
+-rw-r--r--   0 asahi      (501) staff       (20)     8597 2023-04-01 16:15:20.000000 lmppl-0.2.8/lmppl/ppl_encoder_decoder_lm.py
+-rw-r--r--   0 asahi      (501) staff       (20)     6883 2023-03-10 20:47:02.000000 lmppl-0.2.8/lmppl/ppl_mlm.py
+-rw-r--r--   0 asahi      (501) staff       (20)     5816 2023-05-15 21:10:27.000000 lmppl-0.2.8/lmppl/ppl_recurrent_lm.py
+-rw-r--r--   0 asahi      (501) staff       (20)      227 2023-02-07 13:19:37.000000 lmppl-0.2.8/lmppl/util.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-15 21:11:11.997822 lmppl-0.2.8/lmppl.egg-info/
+-rw-r--r--   0 asahi      (501) staff       (20)     5200 2023-05-15 21:11:11.000000 lmppl-0.2.8/lmppl.egg-info/PKG-INFO
+-rw-r--r--   0 asahi      (501) staff       (20)      399 2023-05-15 21:11:11.000000 lmppl-0.2.8/lmppl.egg-info/SOURCES.txt
+-rw-r--r--   0 asahi      (501) staff       (20)        1 2023-05-15 21:11:11.000000 lmppl-0.2.8/lmppl.egg-info/dependency_links.txt
+-rw-r--r--   0 asahi      (501) staff       (20)       79 2023-05-15 21:11:11.000000 lmppl-0.2.8/lmppl.egg-info/requires.txt
+-rw-r--r--   0 asahi      (501) staff       (20)        6 2023-05-15 21:11:11.000000 lmppl-0.2.8/lmppl.egg-info/top_level.txt
+-rw-r--r--   0 asahi      (501) staff       (20)       38 2023-05-15 21:11:12.000637 lmppl-0.2.8/setup.cfg
+-rw-r--r--   0 asahi      (501) staff       (20)     1760 2023-05-15 21:10:58.000000 lmppl-0.2.8/setup.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-15 21:11:11.999411 lmppl-0.2.8/test/
+-rw-r--r--   0 asahi      (501) staff       (20)     1249 2023-02-09 19:14:51.000000 lmppl-0.2.8/test/test_analogy.py
+-rw-r--r--   0 asahi      (501) staff       (20)     2261 2023-02-12 13:50:45.000000 lmppl-0.2.8/test/test_model_with_simple_input.py
```

### Comparing `lmppl-0.2.7/LICENSE.txt` & `lmppl-0.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lmppl-0.2.7/PKG-INFO` & `lmppl-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: lmppl
-Version: 0.2.7
+Version: 0.2.8
 Summary: Calculate perplexity on the text with pre-trained language models.
 Home-page: https://github.com/asahi417/lmppl
 Author: Asahi Ushio
 Author-email: asahi1992ushio@gmail.com
 License: MIT License
-Download-URL: https://github.com/asahi417/lmppl/archive/v0.2.7.tar.gz
+Download-URL: https://github.com/asahi417/lmppl/archive/v0.2.8.tar.gz
 Keywords: language model,t5,gpt3,bert,perplexity,nlp
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lmppl-0.2.7/README.md` & `lmppl-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `lmppl-0.2.7/lmppl/openai_models.py` & `lmppl-0.2.8/lmppl/openai_models.py`

 * *Files identical despite different names*

### Comparing `lmppl-0.2.7/lmppl/ppl_encoder_decoder_lm.py` & `lmppl-0.2.8/lmppl/ppl_encoder_decoder_lm.py`

 * *Files identical despite different names*

### Comparing `lmppl-0.2.7/lmppl/ppl_mlm.py` & `lmppl-0.2.8/lmppl/ppl_mlm.py`

 * *Files identical despite different names*

### Comparing `lmppl-0.2.7/lmppl/ppl_recurrent_lm.py` & `lmppl-0.2.8/lmppl/ppl_recurrent_lm.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,26 +34,28 @@
                  model: str = 'gpt2',
                  use_auth_token: bool = False,
                  max_length: int = None,
                  num_gpus: int = None,
                  torch_dtype=None,
                  device_map: str = None,
                  low_cpu_mem_usage: bool = False,
+                 trust_remote_code: bool = True,
                  hf_cache_dir: str = None):
         """ Language Model.
 
         @param model: Model alias or path to local model file.
         @param use_auth_token: Huggingface transformers argument of `use_auth_token`
         @param device: Device name to load the models.
         @param num_gpus: Number of gpus to be used.
         """
         logging.info(f'Loading Model: `{model}`')
 
         # load model
-        params = {"local_files_only": not internet_connection(), "use_auth_token": use_auth_token}
+        params = {"local_files_only": not internet_connection(), "use_auth_token": use_auth_token,
+                  "trust_remote_code": trust_remote_code}
         if hf_cache_dir is not None:
             params["cache_dir"] = hf_cache_dir
         self.tokenizer = transformers.AutoTokenizer.from_pretrained(model, **params)
         self.config = transformers.AutoConfig.from_pretrained(model, **params)
 
         params.update({"config": self.config, "low_cpu_mem_usage": low_cpu_mem_usage})
         if torch_dtype is not None:
```

### Comparing `lmppl-0.2.7/lmppl.egg-info/PKG-INFO` & `lmppl-0.2.8/lmppl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: lmppl
-Version: 0.2.7
+Version: 0.2.8
 Summary: Calculate perplexity on the text with pre-trained language models.
 Home-page: https://github.com/asahi417/lmppl
 Author: Asahi Ushio
 Author-email: asahi1992ushio@gmail.com
 License: MIT License
-Download-URL: https://github.com/asahi417/lmppl/archive/v0.2.7.tar.gz
+Download-URL: https://github.com/asahi417/lmppl/archive/v0.2.8.tar.gz
 Keywords: language model,t5,gpt3,bert,perplexity,nlp
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lmppl-0.2.7/setup.py` & `lmppl-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     readme = f.read()
-VERSION = '0.2.7'
+VERSION = '0.2.8'
 NAME = 'lmppl'
 LICENSE = 'MIT License'
 setup(
     name=NAME,
     packages=find_packages(exclude=['tests', 'misc', 'asset']),
     version=VERSION,
     license=LICENSE,
```

### Comparing `lmppl-0.2.7/test/test_analogy.py` & `lmppl-0.2.8/test/test_analogy.py`

 * *Files identical despite different names*

### Comparing `lmppl-0.2.7/test/test_model_with_simple_input.py` & `lmppl-0.2.8/test/test_model_with_simple_input.py`

 * *Files identical despite different names*

