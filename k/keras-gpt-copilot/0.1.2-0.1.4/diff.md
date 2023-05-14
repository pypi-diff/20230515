# Comparing `tmp/keras-gpt-copilot-0.1.2.tar.gz` & `tmp/keras-gpt-copilot-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras-gpt-copilot-0.1.2.tar", last modified: Sun May 14 22:22:55 2023, max compression
+gzip compressed data, was "keras-gpt-copilot-0.1.4.tar", last modified: Sun May 14 23:00:30 2023, max compression
```

## Comparing `keras-gpt-copilot-0.1.2.tar` & `keras-gpt-copilot-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 22:22:54.998480 keras-gpt-copilot-0.1.2/
-drwxrwxrwx   0        0        0        0 2023-05-14 22:22:54.921000 keras-gpt-copilot-0.1.2/KerasGPTCopilot/
--rw-rw-rw-   0        0        0       38 2023-05-12 17:32:21.000000 keras-gpt-copilot-0.1.2/KerasGPTCopilot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 22:22:54.934517 keras-gpt-copilot-0.1.2/KerasGPTCopilot/core/
--rw-rw-rw-   0        0        0    13226 2023-05-14 19:14:45.000000 keras-gpt-copilot-0.1.2/KerasGPTCopilot/core/ModelAdvisor.py
--rw-rw-rw-   0        0        0       38 2023-05-12 17:32:21.000000 keras-gpt-copilot-0.1.2/KerasGPTCopilot/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 22:22:54.943512 keras-gpt-copilot-0.1.2/KerasGPTCopilot/extras/
--rw-rw-rw-   0        0        0        0 2023-04-20 19:05:36.000000 keras-gpt-copilot-0.1.2/KerasGPTCopilot/extras/__init__.py
--rw-rw-rw-   0        0        0     1441 2023-05-14 19:15:26.000000 keras-gpt-copilot-0.1.2/KerasGPTCopilot/extras/util.py
--rw-rw-rw-   0        0        0     1068 2023-04-26 21:45:39.000000 keras-gpt-copilot-0.1.2/LICENSE
--rw-rw-rw-   0        0        0       74 2023-05-14 22:20:59.000000 keras-gpt-copilot-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1182 2023-05-14 22:22:54.986487 keras-gpt-copilot-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0    16847 2023-05-14 19:59:57.000000 keras-gpt-copilot-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 22:22:54.981490 keras-gpt-copilot-0.1.2/keras_gpt_copilot.egg-info/
--rw-rw-rw-   0        0        0     1182 2023-05-14 22:22:54.000000 keras-gpt-copilot-0.1.2/keras_gpt_copilot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2023-05-14 22:22:54.000000 keras-gpt-copilot-0.1.2/keras_gpt_copilot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 22:22:54.000000 keras-gpt-copilot-0.1.2/keras_gpt_copilot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-05-14 22:22:54.000000 keras-gpt-copilot-0.1.2/keras_gpt_copilot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-14 22:22:54.000000 keras-gpt-copilot-0.1.2/keras_gpt_copilot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 22:22:54.999482 keras-gpt-copilot-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1413 2023-05-14 22:21:54.000000 keras-gpt-copilot-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 23:00:30.668484 keras-gpt-copilot-0.1.4/
+-rw-rw-rw-   0        0        0     1068 2023-04-26 21:45:39.000000 keras-gpt-copilot-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0       74 2023-05-14 22:38:12.000000 keras-gpt-copilot-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1182 2023-05-14 23:00:30.654484 keras-gpt-copilot-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0    16847 2023-05-14 22:39:42.000000 keras-gpt-copilot-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 23:00:30.588019 keras-gpt-copilot-0.1.4/kerasGPTcopilot/
+-rw-rw-rw-   0        0        0        0 2023-05-14 22:30:26.000000 keras-gpt-copilot-0.1.4/kerasGPTcopilot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 23:00:30.601008 keras-gpt-copilot-0.1.4/kerasGPTcopilot/core/
+-rw-rw-rw-   0        0        0    13226 2023-05-14 22:40:51.000000 keras-gpt-copilot-0.1.4/kerasGPTcopilot/core/ModelAdvisor.py
+-rw-rw-rw-   0        0        0       38 2023-05-12 17:32:21.000000 keras-gpt-copilot-0.1.4/kerasGPTcopilot/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 23:00:30.611003 keras-gpt-copilot-0.1.4/kerasGPTcopilot/extras/
+-rw-rw-rw-   0        0        0        0 2023-04-20 19:05:36.000000 keras-gpt-copilot-0.1.4/kerasGPTcopilot/extras/__init__.py
+-rw-rw-rw-   0        0        0     1441 2023-05-14 19:15:26.000000 keras-gpt-copilot-0.1.4/kerasGPTcopilot/extras/util.py
+drwxrwxrwx   0        0        0        0 2023-05-14 23:00:30.648980 keras-gpt-copilot-0.1.4/keras_gpt_copilot.egg-info/
+-rw-rw-rw-   0        0        0     1182 2023-05-14 23:00:30.000000 keras-gpt-copilot-0.1.4/keras_gpt_copilot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2023-05-14 23:00:30.000000 keras-gpt-copilot-0.1.4/keras_gpt_copilot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 23:00:30.000000 keras-gpt-copilot-0.1.4/keras_gpt_copilot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-05-14 23:00:30.000000 keras-gpt-copilot-0.1.4/keras_gpt_copilot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-14 23:00:30.000000 keras-gpt-copilot-0.1.4/keras_gpt_copilot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-14 23:00:30.669489 keras-gpt-copilot-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1413 2023-05-14 22:33:17.000000 keras-gpt-copilot-0.1.4/setup.py
```

### Comparing `keras-gpt-copilot-0.1.2/KerasGPTCopilot/core/ModelAdvisor.py` & `keras-gpt-copilot-0.1.4/kerasGPTcopilot/core/ModelAdvisor.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import sys
 
 import numpy as np
 import openai
 import pyperclip
 from tensorflow.keras.models import Model
 
-from KerasGPTCopilot.extras.util import CustomJSONEncoder
+from kerasGPTcopilot.extras.util import CustomJSONEncoder
 
 
 class ModelAdvisor:
     """
     A class to interact with OpenAI GPT to get suggestions on improving deep learning model performance.
 
     Attributes:
```

### Comparing `keras-gpt-copilot-0.1.2/KerasGPTCopilot/extras/util.py` & `keras-gpt-copilot-0.1.4/kerasGPTcopilot/extras/util.py`

 * *Files identical despite different names*

### Comparing `keras-gpt-copilot-0.1.2/LICENSE` & `keras-gpt-copilot-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `keras-gpt-copilot-0.1.2/PKG-INFO` & `keras-gpt-copilot-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-gpt-copilot
-Version: 0.1.2
+Version: 0.1.4
 Summary: Integrate an LLM copilot within your Keras model development workflow
 Home-page: https://github.com/fabprezja/keras-gpt-copilot
 Author: Fabi Prezja
 Author-email: faprezja@fairn.fi
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `keras-gpt-copilot-0.1.2/README.md` & `keras-gpt-copilot-0.1.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -11,39 +11,39 @@
 - Can be used with non-OpenAI LLMs to generate suggestions
 - Offers options to downsample and/or smoothen validation curves to accommodate large (and/or noisy) results within the copilot prompt
 - Provides flexibility in customizing the copilot prompt, allowing for the addition of extra information.
 - Supports follow-up questions for extended guidance, such as requesting specific code changes based on previous recommendations
 
 ## Installation
 
-To install the KerasGPTCopilot library, run:
+To install the kerasGPTcopilot library, run:
 ```
 pip install keras-gpt-copilot
 ```
 - Note 1: This is an experimental package; I aim to expand capabilities over time.
 - Note 2: GPT4 or similarly capable models tend to perform best.
 
 ## Usage
 ... with Open A.I API
 ```python
 from tensorflow.keras.models import Model
-from KerasGPTCopilot.core import ModelAdvisor
+from kerasGPTcopilot.core import ModelAdvisor
 
 model = Model(...)  # Your Keras model
 history = model.fit(...)  # The Keras History object
 api_key = "your_openai_api_key"
 
 advisor = ModelAdvisor(model, history, api_key)
 suggestion = advisor.get_suggestions(model="gpt-4", print_cp_prompt=True, print_cp_response=True)
 ```
 
 ... with other LLMs (copilot prompt only)
  ```python
 from tensorflow.keras.models import Model
-from KerasGPTCopilot.core import ModelAdvisor
+from kerasGPTcopilot.core import ModelAdvisor
 
 model = Model(...)  # Your Keras model
 history = model.fit(...)  # The Keras History object
 
 advisor = ModelAdvisor(model, history, None)  # No API key
 copilot_prompt = advisor.get_suggestions(cp_prompt_only=True, print_cp_prompt=True)
 ```
@@ -87,15 +87,15 @@
 history = model.fit(X_train, y_train, validation_data=(X_val, y_val),
                     epochs=11, batch_size=128, callbacks=[model_checkpoint])
                     
 ```
 ### Step 2: Keras GPT Copilot
 
  ```python
-from KerasGPTCopilot.core import ModelAdvisor
+from kerasGPTcopilot.core import ModelAdvisor
 advisor = ModelAdvisor(model, history, None, test_loss=test_loss,test_metric=("test_accuracy", test_accuracy))
 suggestion = advisor.get_suggestions(cp_prompt_only=True,print_cp_prompt=True)
 ```
 
 ### Step 2.1: Keras GPT Copilot generated prompt
 
 ```
```

### Comparing `keras-gpt-copilot-0.1.2/keras_gpt_copilot.egg-info/PKG-INFO` & `keras-gpt-copilot-0.1.4/keras_gpt_copilot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-gpt-copilot
-Version: 0.1.2
+Version: 0.1.4
 Summary: Integrate an LLM copilot within your Keras model development workflow
 Home-page: https://github.com/fabprezja/keras-gpt-copilot
 Author: Fabi Prezja
 Author-email: faprezja@fairn.fi
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `keras-gpt-copilot-0.1.2/setup.py` & `keras-gpt-copilot-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="keras-gpt-copilot",
-    version="0.1.2",
+    version="0.1.4",
     description="Integrate an LLM copilot within your Keras model development workflow",
     long_description="Keras GPT Copilot is the first Python package designed to integrate an LLM copilot within the model development workflow, offering iterative feedback options for enhancing the performance of your Keras deep learning models. Utilizing the power of OpenAI's GPT models, Keras GPT Copilot can use any of the compatible models (GPT4 is recommended). However, the prompt-only mode allows for compatibility with other large language models.",
     author="Fabi Prezja",
     author_email="faprezja@fairn.fi",
     url="https://github.com/fabprezja/keras-gpt-copilot",
     packages=find_packages(),
     install_requires=[
```

