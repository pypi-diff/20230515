# Comparing `tmp/languagemodels-0.0.3.tar.gz` & `tmp/languagemodels-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "languagemodels-0.0.3.tar", last modified: Fri May 12 16:19:36 2023, max compression
+gzip compressed data, was "languagemodels-0.0.4.tar", last modified: Mon May 15 18:09:36 2023, max compression
```

## Comparing `languagemodels-0.0.3.tar` & `languagemodels-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-05-12 16:19:36.207180 languagemodels-0.0.3/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     3537 2023-05-12 16:19:36.207180 languagemodels-0.0.3/PKG-INFO
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-05-12 16:19:36.203180 languagemodels-0.0.3/languagemodels/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     6099 2023-05-12 14:02:41.000000 languagemodels-0.0.3/languagemodels/__init__.py
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     2265 2023-05-09 19:09:44.000000 languagemodels-0.0.3/languagemodels/embeddings.py
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     1910 2023-05-12 13:21:50.000000 languagemodels-0.0.3/languagemodels/inference.py
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-05-12 16:19:36.207180 languagemodels-0.0.3/languagemodels.egg-info/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     3537 2023-05-12 16:19:35.000000 languagemodels-0.0.3/languagemodels.egg-info/PKG-INFO
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      281 2023-05-12 16:19:35.000000 languagemodels-0.0.3/languagemodels.egg-info/SOURCES.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)        1 2023-05-12 16:19:35.000000 languagemodels-0.0.3/languagemodels.egg-info/dependency_links.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       52 2023-05-12 16:19:35.000000 languagemodels-0.0.3/languagemodels.egg-info/requires.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       15 2023-05-12 16:19:35.000000 languagemodels-0.0.3/languagemodels.egg-info/top_level.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       38 2023-05-12 16:19:36.207180 languagemodels-0.0.3/setup.cfg
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      788 2023-05-12 16:19:16.000000 languagemodels-0.0.3/setup.py
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-05-15 18:09:36.367425 languagemodels-0.0.4/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     3925 2023-05-15 18:09:36.367425 languagemodels-0.0.4/PKG-INFO
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-05-15 18:09:36.367425 languagemodels-0.0.4/languagemodels/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     7513 2023-05-15 17:19:44.000000 languagemodels-0.0.4/languagemodels/__init__.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     2265 2023-05-09 19:09:44.000000 languagemodels-0.0.4/languagemodels/embeddings.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     3639 2023-05-15 17:19:44.000000 languagemodels-0.0.4/languagemodels/inference.py
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-05-15 18:09:36.367425 languagemodels-0.0.4/languagemodels.egg-info/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     3925 2023-05-15 18:09:36.000000 languagemodels-0.0.4/languagemodels.egg-info/PKG-INFO
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      281 2023-05-15 18:09:36.000000 languagemodels-0.0.4/languagemodels.egg-info/SOURCES.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)        1 2023-05-15 18:09:36.000000 languagemodels-0.0.4/languagemodels.egg-info/dependency_links.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       52 2023-05-15 18:09:36.000000 languagemodels-0.0.4/languagemodels.egg-info/requires.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       15 2023-05-15 18:09:36.000000 languagemodels-0.0.4/languagemodels.egg-info/top_level.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       38 2023-05-15 18:09:36.367425 languagemodels-0.0.4/setup.cfg
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      788 2023-05-15 18:09:27.000000 languagemodels-0.0.4/setup.py
```

### Comparing `languagemodels-0.0.3/PKG-INFO` & `languagemodels-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: languagemodels
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple inference for large language models
 Home-page: https://github.com/jncraton/languagemodels
 Author: Jon Craton
 Author-email: jon@joncraton.com
 License: UNKNOWN
 Description: Language Models
         ===============
         
         [![PyPI version](https://badge.fury.io/py/languagemodels.svg)](https://badge.fury.io/py/languagemodels)
         [![docs](https://img.shields.io/badge/docs-online-brightgreen)](https://languagemodels.netlify.app/)
         [![Build](https://github.com/jncraton/languagemodels/actions/workflows/build.yml/badge.svg)](https://github.com/jncraton/languagemodels/actions/workflows/build.yml)
         [![Netlify Status](https://api.netlify.com/api/v1/badges/722e625a-c6bc-4373-bd88-c017adc58c00/deploy-status)](https://app.netlify.com/sites/languagemodels/deploys)
         
-        `languagemodels` is a Python package providing simple building blocks for exploring natural language processing.
+        A Python package providing simple building blocks for exploring natural language processing.
         
         ![Translation hello world example](media/hello.gif)
         
         Installation
         ------------
         
         This package can be installed using the following command:
@@ -65,15 +65,15 @@
         ### Semantic Search
         
         ```python
         >>> import languagemodels as lm
         
         >>> lm.store_doc("Mars is a planet")
         >>> lm.store_doc("The sun is hot")
-        >>> lm.search_docs("What is Mars?")
+        >>> lm.load_doc("What is Mars?")
         'Mars is a planet'
         ```
         
         ### Extractive Question Answering
         
         ```python
         >>> import languagemodels as lm
@@ -101,13 +101,26 @@
         
         >>> get_date()
         'Friday, May 12, 2023 at 09:27AM'
         ```
         
         [Full documentation](https://languagemodels.netlify.app/)
         
+        Projects
+        --------
+        
+        This package can be used to do the heavy lifting for a number of learning projects:
+        
+        - Basic chatbot
+        - Chatbot with information retrieval
+        - Chatbot with access to real-time information
+        - Text classification
+        - Extractive question answering
+        - Semantic search
+        - Document question answering
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `languagemodels-0.0.3/languagemodels/__init__.py` & `languagemodels-0.0.4/languagemodels/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 import datetime
 import json
 
-from languagemodels.inference import generate_instruct, get_pipeline
+from languagemodels.inference import generate_instruct, get_pipeline, convert_chat
 from languagemodels.embeddings import RetrievalContext
 
 docs = RetrievalContext()
 
 
 def complete(prompt: str) -> str:
     """Provide one completion for a given open-ended prompt
@@ -47,14 +47,54 @@
 
     >>> do("Does this make sense: The course is jumping well.")
     'no'
     """
     return generate_instruct(prompt, max_tokens=200)
 
 
+def chat(prompt: str) -> str:
+    """Get new message from chat-optimized language model
+
+    The `prompt` for this model is provided as a series of messages as a single
+    plain-text string. Several special tokens are used to delineate chat
+    messages.
+
+    - `<|system|>` - Indicates the start of a system message providing
+    instructions about how the assistant should behave.
+    - `<|prompter|>` - Indicates the start of a prompter (typically user)
+    message.
+    - `<|assistant|>` - Indicates the start of an assistant message.
+    - `<|endoftext|>` - Used to terminal all message types.
+
+    A complete prompt may look something like this:
+
+    ```
+    <|system|>Assistant is helpful and harmless<|endoftext|>
+    <|prompter|>What is the capital of Germany?<|endoftext|>
+    <|assistant|>The capital of Germany is Berlin.<|endoftext|>
+    <|prompter|>How many people live there?<|endoftext|>
+    <|assistant|>
+    ```
+
+    The completion from the language model is returned.
+
+    :param message: List of message as (role, content) tuples
+    :return: Completion returned from the language model
+
+    >>> chat("<|system|>It is 5:15pm. Assistant is helpful<|endoftext|>" \\
+    ...      "<|prompter|>Do you know what time it is?<|endoftext|>" \\
+    ...      "<|assistant|>")
+    'It is 5:15pm.'
+    """
+
+    prompt = convert_chat(prompt)
+
+    return generate_instruct(prompt, max_tokens=200)
+
+
 def extract_answer(question: str, context: str) -> str:
     """Extract an answer to a `question` from a provided `context`
 
     The returned answer will always be a substring extracted from `context`.
     It may not always be a correct or meaningful answer, but it will never be
     an arbitrary hallucination.
 
@@ -109,25 +149,25 @@
     :param doc: A plain text document to store.
 
     >>> store_doc("The sky is blue.")
     """
     docs.store(doc)
 
 
-def search_docs(query: str) -> str:
-    """Search stored documents
+def load_doc(query: str) -> str:
+    """Load a matching document
 
     A single document that best matches `query` will be returned.
 
-    :param prompt: Query to compare to stored documents
+    :param query: Query to compare to stored documents
     :return: Content of the closest matching document
 
     >>> store_doc("The sky is blue.")
     >>> store_doc("Paris is in France.")
-    >>> search_docs("Where is Paris?")
+    >>> load_doc("Where is Paris?")
     'Paris is in France.'
     """
     return docs.get_match(query)
 
 
 def fetch_wiki(topic: str) -> str:
     """
```

### Comparing `languagemodels-0.0.3/languagemodels/embeddings.py` & `languagemodels-0.0.4/languagemodels/embeddings.py`

 * *Files identical despite different names*

### Comparing `languagemodels-0.0.3/languagemodels.egg-info/PKG-INFO` & `languagemodels-0.0.4/languagemodels.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: languagemodels
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple inference for large language models
 Home-page: https://github.com/jncraton/languagemodels
 Author: Jon Craton
 Author-email: jon@joncraton.com
 License: UNKNOWN
 Description: Language Models
         ===============
         
         [![PyPI version](https://badge.fury.io/py/languagemodels.svg)](https://badge.fury.io/py/languagemodels)
         [![docs](https://img.shields.io/badge/docs-online-brightgreen)](https://languagemodels.netlify.app/)
         [![Build](https://github.com/jncraton/languagemodels/actions/workflows/build.yml/badge.svg)](https://github.com/jncraton/languagemodels/actions/workflows/build.yml)
         [![Netlify Status](https://api.netlify.com/api/v1/badges/722e625a-c6bc-4373-bd88-c017adc58c00/deploy-status)](https://app.netlify.com/sites/languagemodels/deploys)
         
-        `languagemodels` is a Python package providing simple building blocks for exploring natural language processing.
+        A Python package providing simple building blocks for exploring natural language processing.
         
         ![Translation hello world example](media/hello.gif)
         
         Installation
         ------------
         
         This package can be installed using the following command:
@@ -65,15 +65,15 @@
         ### Semantic Search
         
         ```python
         >>> import languagemodels as lm
         
         >>> lm.store_doc("Mars is a planet")
         >>> lm.store_doc("The sun is hot")
-        >>> lm.search_docs("What is Mars?")
+        >>> lm.load_doc("What is Mars?")
         'Mars is a planet'
         ```
         
         ### Extractive Question Answering
         
         ```python
         >>> import languagemodels as lm
@@ -101,13 +101,26 @@
         
         >>> get_date()
         'Friday, May 12, 2023 at 09:27AM'
         ```
         
         [Full documentation](https://languagemodels.netlify.app/)
         
+        Projects
+        --------
+        
+        This package can be used to do the heavy lifting for a number of learning projects:
+        
+        - Basic chatbot
+        - Chatbot with information retrieval
+        - Chatbot with access to real-time information
+        - Text classification
+        - Extractive question answering
+        - Semantic search
+        - Document question answering
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `languagemodels-0.0.3/setup.py` & `languagemodels-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="languagemodels",
-    version="0.0.3",
+    version="0.0.4",
     author="Jon Craton",
     author_email="jon@joncraton.com",
     description="Simple inference for large language models",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jncraton/languagemodels",
     packages=setuptools.find_packages(),
```

