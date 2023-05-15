# Comparing `tmp/text_mods-1.30.tar.gz` & `tmp/text_mods-1.40.tar.gz`

## Comparing `text_mods-1.30.tar` & `text_mods-1.40.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 text_mods-1.30/src/Example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 text_mods-1.30/src/__init__.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 text_mods-1.30/src/setup.py
--rw-r--r--   0        0        0     4842 2020-02-02 00:00:00.000000 text_mods-1.30/src/text_mods.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 text_mods-1.30/src/dist/text_mods-1.30-py3-none-any.whl
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 text_mods-1.30/src/dist/text_mods-1.30.tar.gz
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 text_mods-1.30/src/text_mods.egg-info/PKG-INFO
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 text_mods-1.30/src/text_mods.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 text_mods-1.30/src/text_mods.egg-info/dependency_links.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 text_mods-1.30/src/text_mods.egg-info/top_level.txt
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 text_mods-1.30/text_mods.egg-info/PKG-INFO
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 text_mods-1.30/text_mods.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 text_mods-1.30/text_mods.egg-info/dependency_links.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 text_mods-1.30/text_mods.egg-info/top_level.txt
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 text_mods-1.30/LICENSE.txt
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 text_mods-1.30/README.md
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 text_mods-1.30/pyproject.toml
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 text_mods-1.30/PKG-INFO
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 text_mods-1.40/src/Example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 text_mods-1.40/src/__init__.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 text_mods-1.40/src/setup.py
+-rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 text_mods-1.40/src/text_mods.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 text_mods-1.40/src/dist/text_mods-1.30-py3-none-any.whl
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 text_mods-1.40/src/dist/text_mods-1.30.tar.gz
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 text_mods-1.40/src/text_mods.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 text_mods-1.40/src/text_mods.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 text_mods-1.40/src/text_mods.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 text_mods-1.40/src/text_mods.egg-info/top_level.txt
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 text_mods-1.40/text_mods.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 text_mods-1.40/text_mods.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 text_mods-1.40/text_mods.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 text_mods-1.40/text_mods.egg-info/top_level.txt
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 text_mods-1.40/LICENSE.txt
+-rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 text_mods-1.40/README.md
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 text_mods-1.40/pyproject.toml
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 text_mods-1.40/PKG-INFO
```

### Comparing `text_mods-1.30/src/text_mods.py` & `text_mods-1.40/src/text_mods.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,50 +1,42 @@
 import re
 import string
+from typing import List
 import nltk
-from nltk.corpus import wordnet
 from nltk.corpus import stopwords
-from nltk.stem import PorterStemmer, WordNetLemmatizer
-from nltk import ne_chunk, pos_tag
 from nltk.tokenize import word_tokenize
+from collections import Counter
+import random
+from nltk.corpus import wordnet
+from transformers import pipeline
+from nltk.stem import PorterStemmer, WordNetLemmatizer
+from nltk import pos_tag, ne_chunk, word_tokenize
 from nltk.tree import Tree
 from googletrans import Translator
-from gensim.summarization.summarizer import summarize
 from functools import lru_cache
-from typing import List
-from collections import Counter
-import random
-import spacy
 
 stemmer = PorterStemmer()
 lemmatizer = WordNetLemmatizer()
-nlp = spacy.load('en_core_web_sm')
 
 def get_synonyms(word: str, method: str) -> List[str]:
     """Get a list of synonyms for a given word."""
-    synonyms: List[str] = []
+    synonyms = set()
     if method == "synonyms":
         for syn in wordnet.synsets(word):
-            for lemma in syn.lemmas():
-                if lemma.name() not in synonyms and lemma.name() != word:
-                    synonyms.append(lemma.name())
+            synonyms.update(lemma.name() for lemma in syn.lemmas() if lemma.name() != word)
     elif method == "stemming":
         base_word = stemmer.stem(word)
         for syn in wordnet.synsets(base_word):
-            for lemma in syn.lemmas():
-                if lemma.name() not in synonyms and lemma.name() != base_word:
-                    synonyms.append(lemma.name())
+            synonyms.update(lemma.name() for lemma in syn.lemmas() if lemma.name() != base_word)
     elif method == "lemmatization":
-        pos = nltk.pos_tag([word])[0][1][0].lower()
+        pos = pos_tag([word])[0][1][0].lower()
         base_word = lemmatizer.lemmatize(word, pos=pos)
         for syn in wordnet.synsets(base_word):
-            for lemma in syn.lemmas():
-                if lemma.name() not in synonyms and lemma.name() != base_word:
-                    synonyms.append(lemma.name())
-    return synonyms
+            synonyms.update(lemma.name() for lemma in syn.lemmas() if lemma.name() != base_word)
+    return list(synonyms)
 
 def remove_html_tags(text: str) -> str:
     """Remove HTML tags from a given text string."""
     html_pattern = re.compile('<.*?>')
     return re.sub(html_pattern, '', text)
 
 def remove_punctuation(text: str) -> str:
@@ -74,15 +66,17 @@
     stop_words = set(stopwords.words('english'))
     tokens = nltk.word_tokenize(text)
     filtered_text = [token for token in tokens if token.lower() not in stop_words]
     return ' '.join(filtered_text)
 
 def summarize_text(text: str) -> str:
     """Summarize a given text string."""
-    return summarize(text)
+    summarizer = pipeline("summarization")
+    summary = summarizer(text, max_length=100, min_length=30, do_sample=False)
+    return summary[0]['summary']
 
 def extract_entities(text: str) -> List[str]:
     """Extract named entities from a given text string."""
     chunks = ne_chunk(pos_tag(word_tokenize(text)))
     entities = []
     for chunk in chunks:
         if isinstance(chunk, Tree) and chunk.label() in ['PERSON', 'ORGANIZATION', 'GPE']:
```

### Comparing `text_mods-1.30/src/dist/text_mods-1.30-py3-none-any.whl` & `text_mods-1.40/src/dist/text_mods-1.30-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `text_mods-1.30/src/dist/text_mods-1.30.tar.gz` & `text_mods-1.40/src/dist/text_mods-1.30.tar.gz`

 * *Files identical despite different names*

### Comparing `text_mods-1.30/LICENSE.txt` & `text_mods-1.40/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `text_mods-1.30/README.md` & `text_mods-1.40/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 # Text Formatting Toolkit
 
 text_mods is a Python module for formatting text strings in various ways. It includes functions for removing HTML tags and punctuation, replacing words with synonyms, applying different formatting styles such as bold, italic and colored text. In addition it performs natural language processing tasks such as entity recognition, word frequency counting and text summarization.
 
-## Requirements+
+## Requirements
+
+Make sure you have the following requirements installed before running the code:
 
 * Python 3.6 or higher
-* NLTK library
-* WordNet database
+* NLTK library: Install NLTK using 'pip install nltk'
+* NLTK WordNet database
 * gensim library
 * googletrans library
 * spacy library
 * en_core_web_sm package for Spacy
 
 ## Installation
 
 * Install Python 3.6 or higher from the official website: [Here] (<https://www.python.org/downloads/>)
 * Install the NLTK library by running ```pip install nltk``` in your terminal or command prompt.
 * Download the WordNet database by running the following commands in a Python interpreter:
-arduino
 
 ``` Python
 import nltk
 nltk.download('wordnet')
 ```
 
-* Install the gensim, googletrans, and spacy libraries by running
-
-```pip install gensim googletrans spacy```
+* Install gensim using ```pip install gensim```
+* Install googletrans using ```pip install googletrans```
+* Install spacy using ```pip install spacy```
+* Download the en_core_web_sm package for Spacy by running ```python -m spacy download en_core_web_sm```
+* Install the gensim, googletrans, and spacy libraries by running ```pip install gensim googletrans spacy```
 
 * Download the en_core_web_sm package for Spacy by running ```python -m spacy download en_core_web_sm```
 * Download or clone the code from the Github repository: [Github] (<https://github.com/Ilija-nik1/text_mods>)
 
 ### Clone
 
 Clone the repository using git
```

### Comparing `text_mods-1.30/PKG-INFO` & `text_mods-1.40/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 Metadata-Version: 2.1
 Name: text_mods
-Version: 1.30
+Version: 1.40
 Summary: This code defines a collection of functions for formatting and modifying text
 Project-URL: Homepage, https://github.com/Ilija-nik1/text_mods
 Author: I_N-01
 License-File: LICENSE.txt
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Text Formatting Toolkit
 
 text_mods is a Python module for formatting text strings in various ways. It includes functions for removing HTML tags and punctuation, replacing words with synonyms, applying different formatting styles such as bold, italic and colored text. In addition it performs natural language processing tasks such as entity recognition, word frequency counting and text summarization.
 
-## Requirements+
+## Requirements
+
+Make sure you have the following requirements installed before running the code:
 
 * Python 3.6 or higher
-* NLTK library
-* WordNet database
+* NLTK library: Install NLTK using 'pip install nltk'
+* NLTK WordNet database
 * gensim library
 * googletrans library
 * spacy library
 * en_core_web_sm package for Spacy
 
 ## Installation
 
 * Install Python 3.6 or higher from the official website: [Here] (<https://www.python.org/downloads/>)
 * Install the NLTK library by running ```pip install nltk``` in your terminal or command prompt.
 * Download the WordNet database by running the following commands in a Python interpreter:
-arduino
 
 ``` Python
 import nltk
 nltk.download('wordnet')
 ```
 
-* Install the gensim, googletrans, and spacy libraries by running
-
-```pip install gensim googletrans spacy```
+* Install gensim using ```pip install gensim```
+* Install googletrans using ```pip install googletrans```
+* Install spacy using ```pip install spacy```
+* Download the en_core_web_sm package for Spacy by running ```python -m spacy download en_core_web_sm```
+* Install the gensim, googletrans, and spacy libraries by running ```pip install gensim googletrans spacy```
 
 * Download the en_core_web_sm package for Spacy by running ```python -m spacy download en_core_web_sm```
 * Download or clone the code from the Github repository: [Github] (<https://github.com/Ilija-nik1/text_mods>)
 
 ### Clone
 
 Clone the repository using git
```

