# Comparing `tmp/paper-qa-1.4.0.tar.gz` & `tmp/paper-qa-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-qa-1.4.0.tar", last modified: Wed May  3 07:10:33 2023, max compression
+gzip compressed data, was "paper-qa-1.4.1.tar", last modified: Mon May 15 19:58:52 2023, max compression
```

## Comparing `paper-qa-1.4.0.tar` & `paper-qa-1.4.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:10:33.769626 paper-qa-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-03 07:09:45.000000 paper-qa-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-05-03 07:10:33.769626 paper-qa-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11423 2023-05-03 07:09:45.000000 paper-qa-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:10:33.765626 paper-qa-1.4.0/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-05-03 07:10:33.000000 paper-qa-1.4.0/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-03 07:10:33.000000 paper-qa-1.4.0/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 07:10:33.000000 paper-qa-1.4.0/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-03 07:10:33.000000 paper-qa-1.4.0/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 07:10:33.000000 paper-qa-1.4.0/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:10:33.769626 paper-qa-1.4.0/paperqa/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-03 07:09:45.000000 paper-qa-1.4.0/paperqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-05-03 07:09:45.000000 paper-qa-1.4.0/paperqa/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:10:33.769626 paper-qa-1.4.0/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-03 07:09:45.000000 paper-qa-1.4.0/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-05-03 07:09:45.000000 paper-qa-1.4.0/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (123)    18130 2023-05-03 07:09:45.000000 paper-qa-1.4.0/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-03 07:09:45.000000 paper-qa-1.4.0/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-05-03 07:09:45.000000 paper-qa-1.4.0/paperqa/qaprompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-05-03 07:09:45.000000 paper-qa-1.4.0/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-03 07:09:45.000000 paper-qa-1.4.0/paperqa/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-03 07:09:45.000000 paper-qa-1.4.0/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-03 07:09:45.000000 paper-qa-1.4.0/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 07:10:33.769626 paper-qa-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-03 07:09:45.000000 paper-qa-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:10:33.769626 paper-qa-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-05-03 07:09:45.000000 paper-qa-1.4.0/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:58:52.414824 paper-qa-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-15 19:58:09.000000 paper-qa-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-05-15 19:58:52.414824 paper-qa-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12150 2023-05-15 19:58:09.000000 paper-qa-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:58:52.410824 paper-qa-1.4.1/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-05-15 19:58:52.000000 paper-qa-1.4.1/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-15 19:58:52.000000 paper-qa-1.4.1/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 19:58:52.000000 paper-qa-1.4.1/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-15 19:58:52.000000 paper-qa-1.4.1/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 19:58:52.000000 paper-qa-1.4.1/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:58:52.414824 paper-qa-1.4.1/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-15 19:58:09.000000 paper-qa-1.4.1/paperqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-05-15 19:58:09.000000 paper-qa-1.4.1/paperqa/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:58:52.414824 paper-qa-1.4.1/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-15 19:58:09.000000 paper-qa-1.4.1/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-05-15 19:58:09.000000 paper-qa-1.4.1/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17678 2023-05-15 19:58:09.000000 paper-qa-1.4.1/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-15 19:58:09.000000 paper-qa-1.4.1/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-05-15 19:58:09.000000 paper-qa-1.4.1/paperqa/qaprompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-05-15 19:58:09.000000 paper-qa-1.4.1/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-15 19:58:09.000000 paper-qa-1.4.1/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-15 19:58:09.000000 paper-qa-1.4.1/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 19:58:09.000000 paper-qa-1.4.1/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 19:58:52.414824 paper-qa-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-15 19:58:09.000000 paper-qa-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:58:52.414824 paper-qa-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10194 2023-05-15 19:58:09.000000 paper-qa-1.4.1/tests/test_paperqa.py
```

### Comparing `paper-qa-1.4.0/LICENSE` & `paper-qa-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-qa-1.4.0/PKG-INFO` & `paper-qa-1.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,12 @@
-Metadata-Version: 2.1
-Name: paper-qa
-Version: 1.4.0
-Summary: LLM Chain for answering questions from docs 
-Home-page: https://github.com/whitead/paper-qa
-Author: Andrew White
-Author-email: white.d.andrew@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Paper QA
 
 [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/whitead/paper-qa)
 [![tests](https://github.com/whitead/paper-qa/actions/workflows/tests.yml/badge.svg)](https://github.com/whitead/paper-qa)
 [![PyPI version](https://badge.fury.io/py/paper-qa.svg)](https://badge.fury.io/py/paper-qa)
-[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
 
 This is a minimal package for doing question and answering from
 PDFs or text files (which can be raw HTML). It strives to give very good answers, with no hallucinations, by grounding responses with in-text citations. It uses [OpenAI Embeddings](https://platform.openai.com/docs/guides/embeddings) with a vector DB called [FAISS](https://github.com/facebookresearch/faiss) to embed and search documents. [langchain](https://github.com/hwchase17/langchain) helps
 generate answers.
 
 It uses the process shown below:
 
@@ -90,19 +75,43 @@
 docs = Docs(llm='gpt-3.5-turbo')
 ```
 #### Locally Hosted
 
 You can also use any other models (or embeddings) available in [langchain](https://github.com/hwchase17/langchain). Here's an example of using `llama.cpp` to have locally hosted paper-qa:
 
 ```py
-from langchain.embeddings import LlamaCppEmbeddings
+from paperqa import Docs
 from langchain.llms import LlamaCpp
-llm = LlamaCpp(model_path="./ggml-model-q4_0.bin")
-embeddings = LlamaCppEmbeddings(model_path="/path/to/model/ggml-model-q4_0.bin")
+from langchain import PromptTemplate, LLMChain
+from langchain.callbacks.manager import CallbackManager
+from langchain.callbacks.streaming_stdout import StreamingStdOutCallbackHandler
+from langchain.embeddings import LlamaCppEmbeddings
+
+# Callbacks support token-wise streaming
+callback_manager = CallbackManager([StreamingStdOutCallbackHandler()])
+# Verbose is required to pass to the callback manager
+
+# Make sure the model path is correct for your system!
+llm = LlamaCpp(
+    model_path="./ggml-model-q4_0.bin", callback_manager=callback_manager
+)
+embeddings = LlamaCppEmbeddings(model_path="./ggml-model-q4_0.bin")
+
 docs = Docs(llm=llm, embeddings=embeddings)
+
+keyword_search = 'bispecific antibody manufacture'
+papers = paperscraper.search_papers(keyword_search, limit=2)
+for path,data in papers.items():
+    try:
+        docs.add(path,chunk_chars=500)
+    except ValueError as e:
+        print('Could not read', path, e)
+
+answer = docs.query("What manufacturing challenges are unique to bispecific antibodies?")
+print(answer)
 ```
 
 ### Adjusting number of sources
 
 You can adjust the numbers of sources (passages of text) to reduce token usage or add more context. `k` refers to the top k most relevant and diverse (may from different sources) passages. Each passage is sent to the LLM to summarize, or determine if it is irrelevant. After this step, a limit of `max_sources` is applied so that the final answer can fit into the LLM context window. Thus, `k` > `max_sources`  and `max_sources` is the number of sources used in the final answer.
 
 ```python
```

### Comparing `paper-qa-1.4.0/README.md` & `paper-qa-1.4.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,26 @@
+Metadata-Version: 2.1
+Name: paper-qa
+Version: 1.4.1
+Summary: LLM Chain for answering questions from docs 
+Home-page: https://github.com/whitead/paper-qa
+Author: Andrew White
+Author-email: white.d.andrew@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Paper QA
 
 [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/whitead/paper-qa)
 [![tests](https://github.com/whitead/paper-qa/actions/workflows/tests.yml/badge.svg)](https://github.com/whitead/paper-qa)
 [![PyPI version](https://badge.fury.io/py/paper-qa.svg)](https://badge.fury.io/py/paper-qa)
-[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
 
 This is a minimal package for doing question and answering from
 PDFs or text files (which can be raw HTML). It strives to give very good answers, with no hallucinations, by grounding responses with in-text citations. It uses [OpenAI Embeddings](https://platform.openai.com/docs/guides/embeddings) with a vector DB called [FAISS](https://github.com/facebookresearch/faiss) to embed and search documents. [langchain](https://github.com/hwchase17/langchain) helps
 generate answers.
 
 It uses the process shown below:
 
@@ -76,19 +89,43 @@
 docs = Docs(llm='gpt-3.5-turbo')
 ```
 #### Locally Hosted
 
 You can also use any other models (or embeddings) available in [langchain](https://github.com/hwchase17/langchain). Here's an example of using `llama.cpp` to have locally hosted paper-qa:
 
 ```py
-from langchain.embeddings import LlamaCppEmbeddings
+from paperqa import Docs
 from langchain.llms import LlamaCpp
-llm = LlamaCpp(model_path="./ggml-model-q4_0.bin")
-embeddings = LlamaCppEmbeddings(model_path="/path/to/model/ggml-model-q4_0.bin")
+from langchain import PromptTemplate, LLMChain
+from langchain.callbacks.manager import CallbackManager
+from langchain.callbacks.streaming_stdout import StreamingStdOutCallbackHandler
+from langchain.embeddings import LlamaCppEmbeddings
+
+# Callbacks support token-wise streaming
+callback_manager = CallbackManager([StreamingStdOutCallbackHandler()])
+# Verbose is required to pass to the callback manager
+
+# Make sure the model path is correct for your system!
+llm = LlamaCpp(
+    model_path="./ggml-model-q4_0.bin", callback_manager=callback_manager
+)
+embeddings = LlamaCppEmbeddings(model_path="./ggml-model-q4_0.bin")
+
 docs = Docs(llm=llm, embeddings=embeddings)
+
+keyword_search = 'bispecific antibody manufacture'
+papers = paperscraper.search_papers(keyword_search, limit=2)
+for path,data in papers.items():
+    try:
+        docs.add(path,chunk_chars=500)
+    except ValueError as e:
+        print('Could not read', path, e)
+
+answer = docs.query("What manufacturing challenges are unique to bispecific antibodies?")
+print(answer)
 ```
 
 ### Adjusting number of sources
 
 You can adjust the numbers of sources (passages of text) to reduce token usage or add more context. `k` refers to the top k most relevant and diverse (may from different sources) passages. Each passage is sent to the LLM to summarize, or determine if it is irrelevant. After this step, a limit of `max_sources` is applied so that the final answer can fit into the LLM context window. Thus, `k` > `max_sources`  and `max_sources` is the number of sources used in the final answer.
 
 ```python
@@ -253,8 +290,8 @@
 # load
 with open("my_docs.pkl", "rb") as f:
     docs = pickle.load(f)
 ```
 
 ### Callbacks
 
-TODO
+TODO
```

### Comparing `paper-qa-1.4.0/paper_qa.egg-info/PKG-INFO` & `paper-qa-1.4.1/paper_qa.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 1.4.0
+Version: 1.4.1
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,15 +13,14 @@
 License-File: LICENSE
 
 # Paper QA
 
 [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/whitead/paper-qa)
 [![tests](https://github.com/whitead/paper-qa/actions/workflows/tests.yml/badge.svg)](https://github.com/whitead/paper-qa)
 [![PyPI version](https://badge.fury.io/py/paper-qa.svg)](https://badge.fury.io/py/paper-qa)
-[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
 
 This is a minimal package for doing question and answering from
 PDFs or text files (which can be raw HTML). It strives to give very good answers, with no hallucinations, by grounding responses with in-text citations. It uses [OpenAI Embeddings](https://platform.openai.com/docs/guides/embeddings) with a vector DB called [FAISS](https://github.com/facebookresearch/faiss) to embed and search documents. [langchain](https://github.com/hwchase17/langchain) helps
 generate answers.
 
 It uses the process shown below:
 
@@ -90,19 +89,43 @@
 docs = Docs(llm='gpt-3.5-turbo')
 ```
 #### Locally Hosted
 
 You can also use any other models (or embeddings) available in [langchain](https://github.com/hwchase17/langchain). Here's an example of using `llama.cpp` to have locally hosted paper-qa:
 
 ```py
-from langchain.embeddings import LlamaCppEmbeddings
+from paperqa import Docs
 from langchain.llms import LlamaCpp
-llm = LlamaCpp(model_path="./ggml-model-q4_0.bin")
-embeddings = LlamaCppEmbeddings(model_path="/path/to/model/ggml-model-q4_0.bin")
+from langchain import PromptTemplate, LLMChain
+from langchain.callbacks.manager import CallbackManager
+from langchain.callbacks.streaming_stdout import StreamingStdOutCallbackHandler
+from langchain.embeddings import LlamaCppEmbeddings
+
+# Callbacks support token-wise streaming
+callback_manager = CallbackManager([StreamingStdOutCallbackHandler()])
+# Verbose is required to pass to the callback manager
+
+# Make sure the model path is correct for your system!
+llm = LlamaCpp(
+    model_path="./ggml-model-q4_0.bin", callback_manager=callback_manager
+)
+embeddings = LlamaCppEmbeddings(model_path="./ggml-model-q4_0.bin")
+
 docs = Docs(llm=llm, embeddings=embeddings)
+
+keyword_search = 'bispecific antibody manufacture'
+papers = paperscraper.search_papers(keyword_search, limit=2)
+for path,data in papers.items():
+    try:
+        docs.add(path,chunk_chars=500)
+    except ValueError as e:
+        print('Could not read', path, e)
+
+answer = docs.query("What manufacturing challenges are unique to bispecific antibodies?")
+print(answer)
 ```
 
 ### Adjusting number of sources
 
 You can adjust the numbers of sources (passages of text) to reduce token usage or add more context. `k` refers to the top k most relevant and diverse (may from different sources) passages. Each passage is sent to the LLM to summarize, or determine if it is irrelevant. After this step, a limit of `max_sources` is applied so that the final answer can fit into the LLM context window. Thus, `k` > `max_sources`  and `max_sources` is the number of sources used in the final answer.
 
 ```python
```

### Comparing `paper-qa-1.4.0/paperqa/agent.py` & `paper-qa-1.4.1/paperqa/agent.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,171 +1,171 @@
-from langchain.agents import AgentType, initialize_agent
-from langchain.chains import LLMChain
-from langchain.chat_models import ChatOpenAI
-from langchain.tools import BaseTool
-from rmrkl import ChatZeroShotAgent, RetryAgentExecutor
-
-from .docs import Answer, Docs
-from .qaprompts import make_chain, select_paper_prompt
-
-
-def status(answer: Answer, docs: Docs):
-    return f" Status: Current Papers: {len(docs.doc_previews())} Current Evidence: {len(answer.contexts)} Current Cost: ${answer.cost:.2f}"
-
-
-class PaperSelection(BaseTool):
-    name = "Select Papers"
-    description = "Select from current papers. Provide instructions as a string to use for choosing papers."
-    docs: Docs = None
-    answer: Answer = None
-    chain: LLMChain = None
-
-    def __init__(self, docs, answer):
-        # call the parent class constructor
-        super(PaperSelection, self).__init__()
-
-        self.docs = docs
-        self.answer = answer
-        self.chain = make_chain(select_paper_prompt, self.docs.summary_llm)
-
-    def _run(self, query: str) -> str:
-        result = self.docs.doc_match(query)
-        if result is None or result.strip().startswith("None"):
-            return "No relevant papers found."
-        return result + status(self.answer, self.docs)
-
-    async def _arun(self, query: str) -> str:
-        """Use the tool asynchronously."""
-        raise NotImplementedError()
-
-
-class ReadPapers(BaseTool):
-    name = "Gather Evidence"
-    description = (
-        "Give a specific question to a researcher that will return evidence for it. "
-        "Optionally, you may specify papers using their key provided by the Select Papers tool. "
-        "Use the format: $QUESTION or use format $QUESTION|$KEY1,$KEY2,..."
-    )
-    docs: Docs = None
-    answer: Answer = None
-
-    def __init__(self, docs, answer):
-        # call the parent class constructor
-        super(ReadPapers, self).__init__()
-
-        self.docs = docs
-        self.answer = answer
-
-    def _run(self, query: str) -> str:
-        if "|" in query:
-            question, keys = query.split("|")
-            keys = [k.strip() for k in keys.split(",")]
-        else:
-            question = query
-            keys = None
-        # swap out the question
-        old = self.answer.question
-        self.answer.question = question
-        # generator, so run it
-        l0 = len(self.answer.contexts)
-        self.docs.get_evidence(self.answer, key_filter=keys)
-        l1 = len(self.answer.contexts)
-        self.answer.question = old
-        return f"Added {l1 - l0} pieces of evidence." + status(self.answer, self.docs)
-
-    async def _arun(self, query: str) -> str:
-        """Use the tool asynchronously."""
-        raise NotImplementedError()
-
-
-class AnswerTool(BaseTool):
-    name = "Propose Answer"
-    description = "Ask a researcher to propose an answer using evidence from papers. The input is the question to be answered."
-    docs: Docs = None
-    answer: Answer = None
-
-    def __init__(self, docs, answer):
-        # call the parent class constructor
-        super(AnswerTool, self).__init__()
-
-        self.docs = docs
-        self.answer = answer
-
-    def _run(self, query: str) -> str:
-        self.answer = self.docs.query(query, answer=self.answer)
-        if "cannot answer" in self.answer.answer:
-            self.answer = Answer(self.answer.question)
-            return (
-                "Failed to answer question. Deleting evidence. Consider rephrasing question or evidence statement."
-                + status(self.answer, self.docs)
-            )
-        return self.answer.answer + status(self.answer, self.docs)
-
-    def _arun(self, query: str) -> str:
-        """Use the tool asynchronously."""
-        raise NotImplementedError()
-
-
-class Search(BaseTool):
-    name = "Paper Search"
-    description = (
-        "Search for papers to add to cur. Input should be a string of keywords."
-    )
-    docs: Docs = None
-    answer: Answer = None
-
-    def __init__(self, docs, answer):
-        # call the parent class constructor
-        super(Search, self).__init__()
-
-        self.docs = docs
-        self.answer = answer
-
-    def _run(self, query: str) -> str:
-        try:
-            import paperscraper
-        except ImportError:
-            raise ImportError(
-                "Please install paperscraper (github.com/blackadad/paper-scraper) to use agent"
-            )
-
-        papers = paperscraper.search_papers(
-            query, limit=20, verbose=False, pdir=self.docs.index_path
-        )
-        for path, data in papers.items():
-            try:
-                self.docs.add(path, citation=data["citation"])
-            except:
-                pass
-        return status(self.answer, self.docs)
-
-    def _arun(self, query: str) -> str:
-        """Use the tool asynchronously."""
-        raise NotImplementedError()
-
-
-def make_tools(docs, answer):
-    tools = []
-
-    tools.append(Search(docs, answer))
-    tools.append(PaperSelection(docs, answer))
-    tools.append(ReadPapers(docs, answer))
-    tools.append(AnswerTool(docs, answer))
-    return tools
-
-
-def run_agent(docs, question, llm=None):
-    if llm is None:
-        llm = ChatOpenAI(temperature=0.0, model="gpt-4")
-    answer = Answer(question)
-    tools = make_tools(docs, answer)
-    mrkl = RetryAgentExecutor.from_agent_and_tools(
-        tools=tools,
-        agent=ChatZeroShotAgent.from_llm_and_tools(llm, tools),
-        verbose=True,
-    )
-    mrkl.run(
-        f"Answer question: {question}. Search for papers, gather evidence, and answer. If you do not have enough evidence, you can search for more papers (preferred) or gather more evidence. You may rephrase or breaking-up the question in those steps. "
-        "Once you have five pieces of evidence, or you have tried for a while, call the Propose Answer tool. "
-    )
-
-    return answer
+from langchain.agents import AgentType, initialize_agent
+from langchain.chains import LLMChain
+from langchain.chat_models import ChatOpenAI
+from langchain.tools import BaseTool
+from rmrkl import ChatZeroShotAgent, RetryAgentExecutor
+
+from .docs import Answer, Docs
+from .qaprompts import make_chain, select_paper_prompt
+
+
+def status(answer: Answer, docs: Docs):
+    return f" Status: Current Papers: {len(docs.doc_previews())} Current Evidence: {len(answer.contexts)} Current Cost: ${answer.cost:.2f}"
+
+
+class PaperSelection(BaseTool):
+    name = "Select Papers"
+    description = "Select from current papers. Provide instructions as a string to use for choosing papers."
+    docs: Docs = None
+    answer: Answer = None
+    chain: LLMChain = None
+
+    def __init__(self, docs, answer):
+        # call the parent class constructor
+        super(PaperSelection, self).__init__()
+
+        self.docs = docs
+        self.answer = answer
+        self.chain = make_chain(select_paper_prompt, self.docs.summary_llm)
+
+    def _run(self, query: str) -> str:
+        result = self.docs.doc_match(query)
+        if result is None or result.strip().startswith("None"):
+            return "No relevant papers found."
+        return result + status(self.answer, self.docs)
+
+    async def _arun(self, query: str) -> str:
+        """Use the tool asynchronously."""
+        raise NotImplementedError()
+
+
+class ReadPapers(BaseTool):
+    name = "Gather Evidence"
+    description = (
+        "Give a specific question to a researcher that will return evidence for it. "
+        "Optionally, you may specify papers using their key provided by the Select Papers tool. "
+        "Use the format: $QUESTION or use format $QUESTION|$KEY1,$KEY2,..."
+    )
+    docs: Docs = None
+    answer: Answer = None
+
+    def __init__(self, docs, answer):
+        # call the parent class constructor
+        super(ReadPapers, self).__init__()
+
+        self.docs = docs
+        self.answer = answer
+
+    def _run(self, query: str) -> str:
+        if "|" in query:
+            question, keys = query.split("|")
+            keys = [k.strip() for k in keys.split(",")]
+        else:
+            question = query
+            keys = None
+        # swap out the question
+        old = self.answer.question
+        self.answer.question = question
+        # generator, so run it
+        l0 = len(self.answer.contexts)
+        self.docs.get_evidence(self.answer, key_filter=keys)
+        l1 = len(self.answer.contexts)
+        self.answer.question = old
+        return f"Added {l1 - l0} pieces of evidence." + status(self.answer, self.docs)
+
+    async def _arun(self, query: str) -> str:
+        """Use the tool asynchronously."""
+        raise NotImplementedError()
+
+
+class AnswerTool(BaseTool):
+    name = "Propose Answer"
+    description = "Ask a researcher to propose an answer using evidence from papers. The input is the question to be answered."
+    docs: Docs = None
+    answer: Answer = None
+
+    def __init__(self, docs, answer):
+        # call the parent class constructor
+        super(AnswerTool, self).__init__()
+
+        self.docs = docs
+        self.answer = answer
+
+    def _run(self, query: str) -> str:
+        self.answer = self.docs.query(query, answer=self.answer)
+        if "cannot answer" in self.answer.answer:
+            self.answer = Answer(self.answer.question)
+            return (
+                "Failed to answer question. Deleting evidence. Consider rephrasing question or evidence statement."
+                + status(self.answer, self.docs)
+            )
+        return self.answer.answer + status(self.answer, self.docs)
+
+    def _arun(self, query: str) -> str:
+        """Use the tool asynchronously."""
+        raise NotImplementedError()
+
+
+class Search(BaseTool):
+    name = "Paper Search"
+    description = (
+        "Search for papers to add to cur. Input should be a string of keywords."
+    )
+    docs: Docs = None
+    answer: Answer = None
+
+    def __init__(self, docs, answer):
+        # call the parent class constructor
+        super(Search, self).__init__()
+
+        self.docs = docs
+        self.answer = answer
+
+    def _run(self, query: str) -> str:
+        try:
+            import paperscraper
+        except ImportError:
+            raise ImportError(
+                "Please install paperscraper (github.com/blackadad/paper-scraper) to use agent"
+            )
+
+        papers = paperscraper.search_papers(
+            query, limit=20, verbose=False, pdir=self.docs.index_path
+        )
+        for path, data in papers.items():
+            try:
+                self.docs.add(path, citation=data["citation"])
+            except:
+                pass
+        return status(self.answer, self.docs)
+
+    def _arun(self, query: str) -> str:
+        """Use the tool asynchronously."""
+        raise NotImplementedError()
+
+
+def make_tools(docs, answer):
+    tools = []
+
+    tools.append(Search(docs, answer))
+    tools.append(PaperSelection(docs, answer))
+    tools.append(ReadPapers(docs, answer))
+    tools.append(AnswerTool(docs, answer))
+    return tools
+
+
+def run_agent(docs, question, llm=None):
+    if llm is None:
+        llm = ChatOpenAI(temperature=0.0, model_name="gpt-4")
+    answer = Answer(question)
+    tools = make_tools(docs, answer)
+    mrkl = RetryAgentExecutor.from_agent_and_tools(
+        tools=tools,
+        agent=ChatZeroShotAgent.from_llm_and_tools(llm, tools),
+        verbose=True,
+    )
+    mrkl.run(
+        f"Answer question: {question}. Search for papers, gather evidence, and answer. If you do not have enough evidence, you can search for more papers (preferred) or gather more evidence. You may rephrase or breaking-up the question in those steps. "
+        "Once you have five pieces of evidence, or you have tried for a while, call the Propose Answer tool. "
+    )
+
+    return answer
```

### Comparing `paper-qa-1.4.0/paperqa/contrib/zotero.py` & `paper-qa-1.4.1/paperqa/contrib/zotero.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.4.0/paperqa/docs.py` & `paper-qa-1.4.1/paperqa/docs.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,462 +1,462 @@
-import asyncio
-import os
-import re
-import sys
-from datetime import datetime
-from functools import reduce
-from pathlib import Path
-from typing import Callable, List, Optional, Tuple, Union
-
-import langchain
-from langchain.cache import SQLiteCache
-from langchain.callbacks import OpenAICallbackHandler, get_openai_callback
-from langchain.callbacks.base import AsyncCallbackHandler
-from langchain.callbacks.manager import AsyncCallbackManager
-from langchain.chat_models import ChatOpenAI
-from langchain.docstore.document import Document
-from langchain.embeddings.base import Embeddings
-from langchain.embeddings.openai import OpenAIEmbeddings
-from langchain.llms.base import LLM
-from langchain.vectorstores import FAISS
-
-from .paths import CACHE_PATH
-from .qaprompts import (citation_prompt, make_chain, qa_prompt, search_prompt,
-                        select_paper_prompt, summary_prompt)
-from .readers import read_doc
-from .types import Answer, Context
-from .utils import maybe_is_text, md5sum
-
-os.makedirs(os.path.dirname(CACHE_PATH), exist_ok=True)
-langchain.llm_cache = SQLiteCache(CACHE_PATH)
-
-
-class Docs:
-    """A collection of documents to be used for answering questions."""
-
-    def __init__(
-        self,
-        chunk_size_limit: int = 3000,
-        llm: Optional[Union[LLM, str]] = None,
-        summary_llm: Optional[Union[LLM, str]] = None,
-        name: str = "default",
-        index_path: Optional[Path] = None,
-        embeddings: Optional[Embeddings] = None,
-    ) -> None:
-        """Initialize the collection of documents.
-
-        Args:
-            chunk_size_limit: The maximum number of characters to use for a single chunk of text.
-            llm: The language model to use for answering questions. Default - OpenAI chat-gpt-turbo
-            summary_llm: The language model to use for summarizing documents. If None, llm is used.
-            name: The name of the collection.
-            index_path: The path to the index file IF pickled. If None, defaults to using name in $HOME/.paperqa/name
-            embeddings: The embeddings to use for indexing documents. Default - OpenAI embeddings
-        """
-        self.docs = dict()
-        self.chunk_size_limit = chunk_size_limit
-        self.keys = set()
-        self._faiss_index = None
-        self._doc_index = None
-        self.update_llm(llm, summary_llm)
-        if index_path is None:
-            index_path = Path.home() / ".paperqa" / name
-        self.index_path = index_path
-        self.name = name
-        if embeddings is None:
-            embeddings = OpenAIEmbeddings()
-        self.embeddings = embeddings
-
-    def update_llm(
-        self,
-        llm: Optional[Union[LLM, str]] = None,
-        summary_llm: Optional[Union[LLM, str]] = None,
-    ) -> None:
-        """Update the LLM for answering questions."""
-        if llm is None:
-            llm = "gpt-3.5-turbo"
-        if type(llm) is str:
-            llm = ChatOpenAI(temperature=0.1, model=llm)
-        if type(summary_llm) is str:
-            summary_llm = ChatOpenAI(temperature=0.1, model=summary_llm)
-        self.llm = llm
-        if summary_llm is None:
-            summary_llm = llm
-        self.summary_llm = summary_llm
-
-    def add(
-        self,
-        path: str,
-        citation: Optional[str] = None,
-        key: Optional[str] = None,
-        disable_check: bool = False,
-        chunk_chars: Optional[int] = 3000,
-    ) -> None:
-        """Add a document to the collection."""
-
-        # first check to see if we already have this document
-        # this way we don't make api call to create citation on file we already have
-        md5 = md5sum(path)
-        if path in self.docs:
-            raise ValueError(f"Document {path} already in collection.")
-
-        if citation is None:
-            cite_chain = make_chain(prompt=citation_prompt, llm=self.summary_llm)
-            # peak first chunk
-            texts, _ = read_doc(path, "", "", chunk_chars=chunk_chars)
-            if len(texts) == 0:
-                raise ValueError(f"Could not read document {path}. Is it empty?")
-            citation = cite_chain.run(texts[0])
-            if len(citation) < 3 or "Unknown" in citation or "insufficient" in citation:
-                citation = f"Unknown, {os.path.basename(path)}, {datetime.now().year}"
-
-        if key is None:
-            # get first name and year from citation
-            try:
-                author = re.search(r"([A-Z][a-z]+)", citation).group(1)
-            except AttributeError:
-                # panicking - no word??
-                raise ValueError(
-                    f"Could not parse key from citation {citation}. Consider just passing key explicitly - e.g. docs.py (path, citation, key='mykey')"
-                )
-            try:
-                year = re.search(r"(\d{4})", citation).group(1)
-            except AttributeError:
-                year = ""
-            key = f"{author}{year}"
-        suffix = ""
-        while key + suffix in self.keys:
-            # move suffix to next letter
-            if suffix == "":
-                suffix = "a"
-            else:
-                suffix = chr(ord(suffix) + 1)
-        key += suffix
-
-        texts, metadata = read_doc(path, citation, key, chunk_chars=chunk_chars)
-        # loose check to see if document was loaded
-        #
-        if len("".join(texts)) < 10 or (
-            not disable_check and not maybe_is_text("".join(texts))
-        ):
-            raise ValueError(
-                f"This does not look like a text document: {path}. Path disable_check to ignore this error."
-            )
-        if self._faiss_index is not None:
-            self._faiss_index.add_texts(texts, metadatas=metadata)
-        if self._doc_index is not None:
-            self._doc_index.add_texts([citation], metadatas=[{"key": key}])
-        self.docs[path] = dict(texts=texts, metadata=metadata, key=key, md5=md5)
-        self.keys.add(key)
-
-    def clear(self) -> None:
-        """Clear the collection of documents."""
-        self.docs = dict()
-        self.keys = set()
-        self._faiss_index = None
-        self._doc_index = None
-        # delete index file
-        pkl = self.index_path / "index.pkl"
-        if pkl.exists():
-            pkl.unlink()
-        fs = self.index_path / "index.faiss"
-        if fs.exists():
-            fs.unlink()
-
-    def doc_previews(self) -> List[Tuple[int, str, str]]:
-        """Return a list of tuples of (key, citation) for each document."""
-        return [
-            (
-                len(doc["texts"]),
-                doc["metadata"][0]["dockey"],
-                doc["metadata"][0]["citation"],
-            )
-            for doc in self.docs.values()
-        ]
-
-    def doc_match(self, query: str, k: int = 25) -> List[str]:
-        """Return a list of documents that match the query."""
-        if len(self.docs) == 0:
-            return ""
-        if self._doc_index is None:
-            texts = [doc["metadata"][0]["citation"] for doc in self.docs.values()]
-            metadatas = [
-                {"key": doc["metadata"][0]["dockey"]} for doc in self.docs.values()
-            ]
-            self._doc_index = FAISS.from_texts(
-                texts, metadatas=metadatas, embedding=self.embeddings
-            )
-        docs = self._doc_index.max_marginal_relevance_search(query, k=k)
-        chain = make_chain(select_paper_prompt, self.summary_llm)
-        papers = [f"{d.metadata['key']}: {d.page_content}" for d in docs]
-        result = chain.run(instructions=query, papers="\n".join(papers))
-        return result
-
-    # to pickle, we have to save the index as a file
-
-    def __getstate__(self):
-        if self._faiss_index is None and len(self.docs) > 0:
-            self._build_faiss_index()
-        state = self.__dict__.copy()
-        if self._faiss_index is not None:
-            state["_faiss_index"].save_local(self.index_path)
-        del state["_faiss_index"]
-        del state["_doc_index"]
-        return state
-
-    def __setstate__(self, state):
-        self.__dict__.update(state)
-        try:
-            self._faiss_index = FAISS.load_local(self.index_path, self.embeddings)
-        except:
-            # they use some special exception type, but I don't want to import it
-            self._faiss_index = None
-        if not hasattr(self, "_doc_index"):
-            self._doc_index = None
-        self.update_llm(None, None)
-
-    def _build_faiss_index(self):
-        if self._faiss_index is None:
-            texts = reduce(
-                lambda x, y: x + y, [doc["texts"] for doc in self.docs.values()], []
-            )
-            metadatas = reduce(
-                lambda x, y: x + y, [doc["metadata"] for doc in self.docs.values()], []
-            )
-            self._faiss_index = FAISS.from_texts(
-                texts, self.embeddings, metadatas=metadatas
-            )
-
-    def get_evidence(
-        self,
-        answer: Answer,
-        k: int = 3,
-        max_sources: int = 5,
-        marginal_relevance: bool = True,
-        key_filter: Optional[List[str]] = None,
-        get_callbacks: Callable[[str], AsyncCallbackHandler] = lambda x: [],
-    ) -> Answer:
-        # special case for jupyter notebooks
-        if "get_ipython" in globals() or "google.colab" in sys.modules:
-            import nest_asyncio
-
-            nest_asyncio.apply()
-        try:
-            loop = asyncio.get_event_loop()
-        except RuntimeError:
-            loop = asyncio.new_event_loop()
-            asyncio.set_event_loop(loop)
-        return loop.run_until_complete(
-            self.aget_evidence(
-                answer,
-                k=k,
-                max_sources=max_sources,
-                marginal_relevance=marginal_relevance,
-                key_filter=key_filter,
-                get_callbacks=get_callbacks,
-            )
-        )
-
-    async def aget_evidence(
-        self,
-        answer: Answer,
-        k: int = 3,
-        max_sources: int = 5,
-        marginal_relevance: bool = True,
-        key_filter: Optional[List[str]] = None,
-        get_callbacks: Callable[[str], AsyncCallbackHandler] = lambda x: [],
-    ) -> Answer:
-        if len(self.docs) == 0:
-            return answer
-        if self._faiss_index is None:
-            self._build_faiss_index()
-        _k = k
-        if key_filter is not None:
-            _k = k * 10  # heuristic
-        # want to work through indices but less k
-        if marginal_relevance:
-            docs = self._faiss_index.max_marginal_relevance_search(
-                answer.question, k=_k, fetch_k=5 * _k
-            )
-        else:
-            docs = self._faiss_index.similarity_search(
-                answer.question, k=_k, fetch_k=5 * _k
-            )
-
-        async def process(doc):
-            if key_filter is not None and doc.metadata["dockey"] not in key_filter:
-                return None, None
-            # check if it is already in answer (possible in agent setting)
-            if doc.metadata["key"] in [c.key for c in answer.contexts]:
-                return None, None
-            callbacks = [OpenAICallbackHandler()] + get_callbacks(
-                "evidence:" + doc.metadata["key"]
-            )
-            summary_chain = make_chain(summary_prompt, self.summary_llm)
-            c = Context(
-                key=doc.metadata["key"],
-                citation=doc.metadata["citation"],
-                context=await summary_chain.arun(
-                    question=answer.question,
-                    context_str=doc.page_content,
-                    citation=doc.metadata["citation"],
-                    callbacks=callbacks,
-                ),
-                text=doc.page_content,
-            )
-            if "Not applicable" not in c.context:
-                return c, cb
-            return None, None
-
-        with get_openai_callback() as cb:
-            results = await asyncio.gather(*[process(doc) for doc in docs])
-        # filter out failures
-        results = [r for r in results if r[0] is not None]
-        answer.tokens += sum([cb.total_tokens for _, cb in results])
-        answer.cost += sum([cb.total_cost for _, cb in results])
-        contexts = [c for c, _ in results if c is not None]
-        if len(contexts) == 0:
-            return answer
-        contexts = sorted(contexts, key=lambda x: len(x.context), reverse=True)
-        contexts = contexts[:max_sources]
-        # add to answer (if not already there)
-        keys = [c.key for c in answer.contexts]
-        for c in contexts:
-            if c.key not in keys:
-                answer.contexts.append(c)
-
-        context_str = "\n\n".join(
-            [
-                f"{c.key}: {c.context}"
-                for c in answer.contexts
-                if "Not applicable" not in c.context
-            ]
-        )
-        valid_keys = [
-            c.key for c in answer.contexts if "Not applicable" not in c.context
-        ]
-        if len(valid_keys) > 0:
-            context_str += "\n\nValid keys: " + ", ".join(valid_keys)
-        answer.context = context_str
-        return answer
-
-    def generate_search_query(self, query: str) -> List[str]:
-        """Generate a list of search strings that can be used to find
-        relevant papers.
-
-        Args:
-            query (str): The query to generate search strings for.
-        """
-
-        search_chain = make_chain(prompt=search_prompt, llm=self.summary_llm)
-        search_query = search_chain.run(question=query)
-        queries = [s for s in search_query.split("\n") if len(s) > 3]
-        # remove 2., 3. from queries
-        queries = [re.sub(r"^\d+\.\s*", "", q) for q in queries]
-        return queries
-
-    def query(
-        self,
-        query: str,
-        k: int = 10,
-        max_sources: int = 5,
-        length_prompt: str = "about 100 words",
-        marginal_relevance: bool = True,
-        answer: Optional[Answer] = None,
-        key_filter: Optional[bool] = None,
-        get_callbacks: Callable[[str], AsyncCallbackHandler] = lambda x: [],
-    ) -> Answer:
-        # special case for jupyter notebooks
-        if "get_ipython" in globals() or "google.colab" in sys.modules:
-            import nest_asyncio
-
-            nest_asyncio.apply()
-        try:
-            loop = asyncio.get_event_loop()
-        except RuntimeError:
-            loop = asyncio.new_event_loop()
-            asyncio.set_event_loop(loop)
-        return loop.run_until_complete(
-            self.aquery(
-                query,
-                k=k,
-                max_sources=max_sources,
-                length_prompt=length_prompt,
-                marginal_relevance=marginal_relevance,
-                answer=answer,
-                key_filter=key_filter,
-                get_callbacks=get_callbacks,
-            )
-        )
-
-    async def aquery(
-        self,
-        query: str,
-        k: int = 10,
-        max_sources: int = 5,
-        length_prompt: str = "about 100 words",
-        marginal_relevance: bool = True,
-        answer: Optional[Answer] = None,
-        key_filter: Optional[bool] = None,
-        get_callbacks: Callable[[str], AsyncCallbackHandler] = lambda x: [],
-    ) -> Answer:
-        if k < max_sources:
-            raise ValueError("k should be greater than max_sources")
-        if answer is None:
-            answer = Answer(query)
-        if len(answer.contexts) == 0:
-            if key_filter or (key_filter is None and len(self.docs) > 5):
-                with get_openai_callback() as cb:
-                    keys = self.doc_match(answer.question)
-                answer.tokens += cb.total_tokens
-                answer.cost += cb.total_cost
-            answer = await self.aget_evidence(
-                answer,
-                k=k,
-                max_sources=max_sources,
-                marginal_relevance=marginal_relevance,
-                key_filter=keys if key_filter else None,
-                get_callbacks=get_callbacks,
-            )
-        context_str, contexts = answer.context, answer.contexts
-        bib = dict()
-        passages = dict()
-        if len(context_str) < 10:
-            answer_text = (
-                "I cannot answer this question due to insufficient information."
-            )
-        else:
-            cb = OpenAICallbackHandler()
-            callbacks = [OpenAICallbackHandler()] + get_callbacks("answer")
-            qa_chain = make_chain(qa_prompt, self.llm)
-            answer_text = await qa_chain.arun(
-                question=query,
-                context_str=context_str,
-                length=length_prompt,
-                callbacks=callbacks,
-            )
-            answer.tokens += cb.total_tokens
-            answer.cost += cb.total_cost
-        # it still happens lol
-        if "(Foo2012)" in answer_text:
-            answer_text = answer_text.replace("(Foo2012)", "")
-        for c in contexts:
-            key = c.key
-            text = c.context
-            citation = c.citation
-            # do check for whole key (so we don't catch Callahan2019a with Callahan2019)
-            skey = key.split(" ")[0]
-            if skey + " " in answer_text or skey + ")" or skey + "," in answer_text:
-                bib[skey] = citation
-                passages[key] = text
-        bib_str = "\n\n".join(
-            [f"{i+1}. ({k}): {c}" for i, (k, c) in enumerate(bib.items())]
-        )
-        formatted_answer = f"Question: {query}\n\n{answer_text}\n"
-        if len(bib) > 0:
-            formatted_answer += f"\nReferences\n\n{bib_str}\n"
-        formatted_answer += f"\nTokens Used: {answer.tokens} Cost: ${answer.cost:.2f}"
-        answer.answer = answer_text
-        answer.formatted_answer = formatted_answer
-        answer.references = bib_str
-        answer.passages = passages
-        return answer
+import asyncio
+import os
+import re
+import sys
+from datetime import datetime
+from functools import reduce
+from pathlib import Path
+from typing import Callable, List, Optional, Tuple, Union
+
+import langchain
+from langchain.cache import SQLiteCache
+from langchain.callbacks import OpenAICallbackHandler, get_openai_callback
+from langchain.callbacks.base import AsyncCallbackHandler
+from langchain.callbacks.manager import AsyncCallbackManager
+from langchain.chat_models import ChatOpenAI
+from langchain.docstore.document import Document
+from langchain.embeddings.base import Embeddings
+from langchain.embeddings.openai import OpenAIEmbeddings
+from langchain.llms.base import LLM
+from langchain.vectorstores import FAISS
+
+from .paths import CACHE_PATH
+from .qaprompts import (citation_prompt, make_chain, qa_prompt, search_prompt,
+                        select_paper_prompt, summary_prompt)
+from .readers import read_doc
+from .types import Answer, Context
+from .utils import maybe_is_text, md5sum
+
+os.makedirs(os.path.dirname(CACHE_PATH), exist_ok=True)
+langchain.llm_cache = SQLiteCache(CACHE_PATH)
+
+
+class Docs:
+    """A collection of documents to be used for answering questions."""
+
+    def __init__(
+        self,
+        chunk_size_limit: int = 3000,
+        llm: Optional[Union[LLM, str]] = None,
+        summary_llm: Optional[Union[LLM, str]] = None,
+        name: str = "default",
+        index_path: Optional[Path] = None,
+        embeddings: Optional[Embeddings] = None,
+    ) -> None:
+        """Initialize the collection of documents.
+
+        Args:
+            chunk_size_limit: The maximum number of characters to use for a single chunk of text.
+            llm: The language model to use for answering questions. Default - OpenAI chat-gpt-turbo
+            summary_llm: The language model to use for summarizing documents. If None, llm is used.
+            name: The name of the collection.
+            index_path: The path to the index file IF pickled. If None, defaults to using name in $HOME/.paperqa/name
+            embeddings: The embeddings to use for indexing documents. Default - OpenAI embeddings
+        """
+        self.docs = dict()
+        self.chunk_size_limit = chunk_size_limit
+        self.keys = set()
+        self._faiss_index = None
+        self._doc_index = None
+        self.update_llm(llm, summary_llm)
+        if index_path is None:
+            index_path = Path.home() / ".paperqa" / name
+        self.index_path = index_path
+        self.name = name
+        if embeddings is None:
+            embeddings = OpenAIEmbeddings()
+        self.embeddings = embeddings
+
+    def update_llm(
+        self,
+        llm: Optional[Union[LLM, str]] = None,
+        summary_llm: Optional[Union[LLM, str]] = None,
+    ) -> None:
+        """Update the LLM for answering questions."""
+        if llm is None:
+            llm = "gpt-3.5-turbo"
+        if type(llm) is str:
+            llm = ChatOpenAI(temperature=0.1, model_name=llm)
+        if type(summary_llm) is str:
+            summary_llm = ChatOpenAI(temperature=0.1, model_name=summary_llm)
+        self.llm = llm
+        if summary_llm is None:
+            summary_llm = llm
+        self.summary_llm = summary_llm
+
+    def add(
+        self,
+        path: str,
+        citation: Optional[str] = None,
+        key: Optional[str] = None,
+        disable_check: bool = False,
+        chunk_chars: Optional[int] = 3000,
+    ) -> None:
+        """Add a document to the collection."""
+
+        # first check to see if we already have this document
+        # this way we don't make api call to create citation on file we already have
+        md5 = md5sum(path)
+        if path in self.docs:
+            raise ValueError(f"Document {path} already in collection.")
+
+        if citation is None:
+            cite_chain = make_chain(prompt=citation_prompt, llm=self.summary_llm)
+            # peak first chunk
+            texts, _ = read_doc(path, "", "", chunk_chars=chunk_chars)
+            if len(texts) == 0:
+                raise ValueError(f"Could not read document {path}. Is it empty?")
+            citation = cite_chain.run(texts[0])
+            if len(citation) < 3 or "Unknown" in citation or "insufficient" in citation:
+                citation = f"Unknown, {os.path.basename(path)}, {datetime.now().year}"
+
+        if key is None:
+            # get first name and year from citation
+            try:
+                author = re.search(r"([A-Z][a-z]+)", citation).group(1)
+            except AttributeError:
+                # panicking - no word??
+                raise ValueError(
+                    f"Could not parse key from citation {citation}. Consider just passing key explicitly - e.g. docs.py (path, citation, key='mykey')"
+                )
+            try:
+                year = re.search(r"(\d{4})", citation).group(1)
+            except AttributeError:
+                year = ""
+            key = f"{author}{year}"
+        suffix = ""
+        while key + suffix in self.keys:
+            # move suffix to next letter
+            if suffix == "":
+                suffix = "a"
+            else:
+                suffix = chr(ord(suffix) + 1)
+        key += suffix
+
+        texts, metadata = read_doc(path, citation, key, chunk_chars=chunk_chars)
+        # loose check to see if document was loaded
+        #
+        if len("".join(texts)) < 10 or (
+            not disable_check and not maybe_is_text("".join(texts))
+        ):
+            raise ValueError(
+                f"This does not look like a text document: {path}. Path disable_check to ignore this error."
+            )
+        if self._faiss_index is not None:
+            self._faiss_index.add_texts(texts, metadatas=metadata)
+        if self._doc_index is not None:
+            self._doc_index.add_texts([citation], metadatas=[{"key": key}])
+        self.docs[path] = dict(texts=texts, metadata=metadata, key=key, md5=md5)
+        self.keys.add(key)
+
+    def clear(self) -> None:
+        """Clear the collection of documents."""
+        self.docs = dict()
+        self.keys = set()
+        self._faiss_index = None
+        self._doc_index = None
+        # delete index file
+        pkl = self.index_path / "index.pkl"
+        if pkl.exists():
+            pkl.unlink()
+        fs = self.index_path / "index.faiss"
+        if fs.exists():
+            fs.unlink()
+
+    def doc_previews(self) -> List[Tuple[int, str, str]]:
+        """Return a list of tuples of (key, citation) for each document."""
+        return [
+            (
+                len(doc["texts"]),
+                doc["metadata"][0]["dockey"],
+                doc["metadata"][0]["citation"],
+            )
+            for doc in self.docs.values()
+        ]
+
+    def doc_match(self, query: str, k: int = 25) -> List[str]:
+        """Return a list of documents that match the query."""
+        if len(self.docs) == 0:
+            return ""
+        if self._doc_index is None:
+            texts = [doc["metadata"][0]["citation"] for doc in self.docs.values()]
+            metadatas = [
+                {"key": doc["metadata"][0]["dockey"]} for doc in self.docs.values()
+            ]
+            self._doc_index = FAISS.from_texts(
+                texts, metadatas=metadatas, embedding=self.embeddings
+            )
+        docs = self._doc_index.max_marginal_relevance_search(query, k=k)
+        chain = make_chain(select_paper_prompt, self.summary_llm)
+        papers = [f"{d.metadata['key']}: {d.page_content}" for d in docs]
+        result = chain.run(instructions=query, papers="\n".join(papers))
+        return result
+
+    # to pickle, we have to save the index as a file
+
+    def __getstate__(self):
+        if self._faiss_index is None and len(self.docs) > 0:
+            self._build_faiss_index()
+        state = self.__dict__.copy()
+        if self._faiss_index is not None:
+            state["_faiss_index"].save_local(self.index_path)
+        del state["_faiss_index"]
+        del state["_doc_index"]
+        return state
+
+    def __setstate__(self, state):
+        self.__dict__.update(state)
+        try:
+            self._faiss_index = FAISS.load_local(self.index_path, self.embeddings)
+        except:
+            # they use some special exception type, but I don't want to import it
+            self._faiss_index = None
+        if not hasattr(self, "_doc_index"):
+            self._doc_index = None
+        self.update_llm(None, None)
+
+    def _build_faiss_index(self):
+        if self._faiss_index is None:
+            texts = reduce(
+                lambda x, y: x + y, [doc["texts"] for doc in self.docs.values()], []
+            )
+            metadatas = reduce(
+                lambda x, y: x + y, [doc["metadata"] for doc in self.docs.values()], []
+            )
+            self._faiss_index = FAISS.from_texts(
+                texts, self.embeddings, metadatas=metadatas
+            )
+
+    def get_evidence(
+        self,
+        answer: Answer,
+        k: int = 3,
+        max_sources: int = 5,
+        marginal_relevance: bool = True,
+        key_filter: Optional[List[str]] = None,
+        get_callbacks: Callable[[str], AsyncCallbackHandler] = lambda x: [],
+    ) -> Answer:
+        # special case for jupyter notebooks
+        if "get_ipython" in globals() or "google.colab" in sys.modules:
+            import nest_asyncio
+
+            nest_asyncio.apply()
+        try:
+            loop = asyncio.get_event_loop()
+        except RuntimeError:
+            loop = asyncio.new_event_loop()
+            asyncio.set_event_loop(loop)
+        return loop.run_until_complete(
+            self.aget_evidence(
+                answer,
+                k=k,
+                max_sources=max_sources,
+                marginal_relevance=marginal_relevance,
+                key_filter=key_filter,
+                get_callbacks=get_callbacks,
+            )
+        )
+
+    async def aget_evidence(
+        self,
+        answer: Answer,
+        k: int = 3,
+        max_sources: int = 5,
+        marginal_relevance: bool = True,
+        key_filter: Optional[List[str]] = None,
+        get_callbacks: Callable[[str], AsyncCallbackHandler] = lambda x: [],
+    ) -> Answer:
+        if len(self.docs) == 0:
+            return answer
+        if self._faiss_index is None:
+            self._build_faiss_index()
+        _k = k
+        if key_filter is not None:
+            _k = k * 10  # heuristic
+        # want to work through indices but less k
+        if marginal_relevance:
+            docs = self._faiss_index.max_marginal_relevance_search(
+                answer.question, k=_k, fetch_k=5 * _k
+            )
+        else:
+            docs = self._faiss_index.similarity_search(
+                answer.question, k=_k, fetch_k=5 * _k
+            )
+
+        async def process(doc):
+            if key_filter is not None and doc.metadata["dockey"] not in key_filter:
+                return None, None
+            # check if it is already in answer (possible in agent setting)
+            if doc.metadata["key"] in [c.key for c in answer.contexts]:
+                return None, None
+            callbacks = [OpenAICallbackHandler()] + get_callbacks(
+                "evidence:" + doc.metadata["key"]
+            )
+            summary_chain = make_chain(summary_prompt, self.summary_llm)
+            c = Context(
+                key=doc.metadata["key"],
+                citation=doc.metadata["citation"],
+                context=await summary_chain.arun(
+                    question=answer.question,
+                    context_str=doc.page_content,
+                    citation=doc.metadata["citation"],
+                    callbacks=callbacks,
+                ),
+                text=doc.page_content,
+            )
+            if "Not applicable" not in c.context:
+                return c, cb
+            return None, None
+
+        with get_openai_callback() as cb:
+            results = await asyncio.gather(*[process(doc) for doc in docs])
+        # filter out failures
+        results = [r for r in results if r[0] is not None]
+        answer.tokens += sum([cb.total_tokens for _, cb in results])
+        answer.cost += sum([cb.total_cost for _, cb in results])
+        contexts = [c for c, _ in results if c is not None]
+        if len(contexts) == 0:
+            return answer
+        contexts = sorted(contexts, key=lambda x: len(x.context), reverse=True)
+        contexts = contexts[:max_sources]
+        # add to answer (if not already there)
+        keys = [c.key for c in answer.contexts]
+        for c in contexts:
+            if c.key not in keys:
+                answer.contexts.append(c)
+
+        context_str = "\n\n".join(
+            [
+                f"{c.key}: {c.context}"
+                for c in answer.contexts
+                if "Not applicable" not in c.context
+            ]
+        )
+        valid_keys = [
+            c.key for c in answer.contexts if "Not applicable" not in c.context
+        ]
+        if len(valid_keys) > 0:
+            context_str += "\n\nValid keys: " + ", ".join(valid_keys)
+        answer.context = context_str
+        return answer
+
+    def generate_search_query(self, query: str) -> List[str]:
+        """Generate a list of search strings that can be used to find
+        relevant papers.
+
+        Args:
+            query (str): The query to generate search strings for.
+        """
+
+        search_chain = make_chain(prompt=search_prompt, llm=self.summary_llm)
+        search_query = search_chain.run(question=query)
+        queries = [s for s in search_query.split("\n") if len(s) > 3]
+        # remove 2., 3. from queries
+        queries = [re.sub(r"^\d+\.\s*", "", q) for q in queries]
+        return queries
+
+    def query(
+        self,
+        query: str,
+        k: int = 10,
+        max_sources: int = 5,
+        length_prompt: str = "about 100 words",
+        marginal_relevance: bool = True,
+        answer: Optional[Answer] = None,
+        key_filter: Optional[bool] = None,
+        get_callbacks: Callable[[str], AsyncCallbackHandler] = lambda x: [],
+    ) -> Answer:
+        # special case for jupyter notebooks
+        if "get_ipython" in globals() or "google.colab" in sys.modules:
+            import nest_asyncio
+
+            nest_asyncio.apply()
+        try:
+            loop = asyncio.get_event_loop()
+        except RuntimeError:
+            loop = asyncio.new_event_loop()
+            asyncio.set_event_loop(loop)
+        return loop.run_until_complete(
+            self.aquery(
+                query,
+                k=k,
+                max_sources=max_sources,
+                length_prompt=length_prompt,
+                marginal_relevance=marginal_relevance,
+                answer=answer,
+                key_filter=key_filter,
+                get_callbacks=get_callbacks,
+            )
+        )
+
+    async def aquery(
+        self,
+        query: str,
+        k: int = 10,
+        max_sources: int = 5,
+        length_prompt: str = "about 100 words",
+        marginal_relevance: bool = True,
+        answer: Optional[Answer] = None,
+        key_filter: Optional[bool] = None,
+        get_callbacks: Callable[[str], AsyncCallbackHandler] = lambda x: [],
+    ) -> Answer:
+        if k < max_sources:
+            raise ValueError("k should be greater than max_sources")
+        if answer is None:
+            answer = Answer(query)
+        if len(answer.contexts) == 0:
+            if key_filter or (key_filter is None and len(self.docs) > 5):
+                with get_openai_callback() as cb:
+                    keys = self.doc_match(answer.question)
+                answer.tokens += cb.total_tokens
+                answer.cost += cb.total_cost
+            answer = await self.aget_evidence(
+                answer,
+                k=k,
+                max_sources=max_sources,
+                marginal_relevance=marginal_relevance,
+                key_filter=keys if key_filter else None,
+                get_callbacks=get_callbacks,
+            )
+        context_str, contexts = answer.context, answer.contexts
+        bib = dict()
+        passages = dict()
+        if len(context_str) < 10:
+            answer_text = (
+                "I cannot answer this question due to insufficient information."
+            )
+        else:
+            cb = OpenAICallbackHandler()
+            callbacks = [OpenAICallbackHandler()] + get_callbacks("answer")
+            qa_chain = make_chain(qa_prompt, self.llm)
+            answer_text = await qa_chain.arun(
+                question=query,
+                context_str=context_str,
+                length=length_prompt,
+                callbacks=callbacks,
+            )
+            answer.tokens += cb.total_tokens
+            answer.cost += cb.total_cost
+        # it still happens lol
+        if "(Foo2012)" in answer_text:
+            answer_text = answer_text.replace("(Foo2012)", "")
+        for c in contexts:
+            key = c.key
+            text = c.context
+            citation = c.citation
+            # do check for whole key (so we don't catch Callahan2019a with Callahan2019)
+            skey = key.split(" ")[0]
+            if skey + " " in answer_text or skey + ")" or skey + "," in answer_text:
+                bib[skey] = citation
+                passages[key] = text
+        bib_str = "\n\n".join(
+            [f"{i+1}. ({k}): {c}" for i, (k, c) in enumerate(bib.items())]
+        )
+        formatted_answer = f"Question: {query}\n\n{answer_text}\n"
+        if len(bib) > 0:
+            formatted_answer += f"\nReferences\n\n{bib_str}\n"
+        formatted_answer += f"\nTokens Used: {answer.tokens} Cost: ${answer.cost:.2f}"
+        answer.answer = answer_text
+        answer.formatted_answer = formatted_answer
+        answer.references = bib_str
+        answer.passages = passages
+        return answer
```

### Comparing `paper-qa-1.4.0/paperqa/readers.py` & `paper-qa-1.4.1/paperqa/readers.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,225 +1,225 @@
-import json
-import logging
-import os
-from hashlib import md5
-from pathlib import Path
-
-from html2text import html2text
-from langchain.cache import SQLiteCache
-from langchain.schema import Generation
-from langchain.text_splitter import TokenTextSplitter
-
-from .paths import OCR_CACHE_PATH
-from .version import __version__
-
-OCR_CACHE = None
-
-
-def _get_ocr_cache() -> SQLiteCache:
-    """Used to lazily create the cache directory and cache object."""
-    global OCR_CACHE
-    if OCR_CACHE is None:
-        os.makedirs(os.path.dirname(OCR_CACHE_PATH), exist_ok=True)
-        OCR_CACHE = SQLiteCache(OCR_CACHE_PATH)
-    return OCR_CACHE
-
-
-TextSplitter = TokenTextSplitter
-
-
-def parse_pdf(path, citation, key, chunk_chars=2000, overlap=50):
-    import pypdf
-
-    pdfFileObj = open(path, "rb")
-    pdfReader = pypdf.PdfReader(pdfFileObj)
-    splits = []
-    split = ""
-    pages = []
-    metadatas = []
-    for i, page in enumerate(pdfReader.pages):
-        split += page.extract_text()
-        pages.append(str(i + 1))
-        # split could be so long it needs to be split
-        # into multiple chunks. Or it could be so short
-        # that it needs to be combined with the next chunk.
-        while len(split) > chunk_chars:
-            splits.append(split[:chunk_chars])
-            # pretty formatting of pages (e.g. 1-3, 4, 5-7)
-            pg = "-".join([pages[0], pages[-1]])
-            metadatas.append(
-                dict(
-                    citation=citation,
-                    dockey=key,
-                    key=f"{key} pages {pg}",
-                )
-            )
-            split = split[chunk_chars - overlap :]
-            pages = [str(i + 1)]
-    if len(split) > overlap:
-        splits.append(split[:chunk_chars])
-        pg = "-".join([pages[0], pages[-1]])
-        metadatas.append(
-            dict(
-                citation=citation,
-                dockey=key,
-                key=f"{key} pages {pg}",
-            )
-        )
-    pdfFileObj.close()
-    return splits, metadatas
-
-
-def parse_txt(path, citation, key, chunk_chars=2000, overlap=50, html=False):
-    try:
-        with open(path) as f:
-            doc = f.read()
-    except UnicodeDecodeError:
-        with open(path, encoding="utf-8", errors="ignore") as f:
-            doc = f.read()
-    if html:
-        doc = html2text(doc)
-    # yo, no idea why but the texts are not split correctly
-    text_splitter = TextSplitter(chunk_size=chunk_chars, chunk_overlap=overlap)
-    texts = text_splitter.split_text(doc)
-    return texts, [dict(citation=citation, dockey=key, key=key)] * len(texts)
-
-
-def parse_code_txt(path, citation, key, chunk_chars=2000, overlap=50):
-    """Parse a document into chunks, based on line numbers (for code)."""
-
-    splits = []
-    split = ""
-    metadatas = []
-    last_line = 0
-
-    with open(path) as f:
-        for i, line in enumerate(f):
-            split += line
-            if len(split) > chunk_chars:
-                splits.append(split[:chunk_chars])
-                metadatas.append(
-                    dict(
-                        citation=citation,
-                        dockey=key,
-                        key=f"{key} lines {last_line}-{i}",
-                    )
-                )
-                split = split[chunk_chars - overlap :]
-                last_line = i
-    if len(split) > overlap:
-        splits.append(split[:chunk_chars])
-        metadatas.append(
-            dict(
-                citation=citation,
-                dockey=key,
-                key=f"{key} lines {last_line}-{i}",
-            )
-        )
-    return splits, metadatas
-
-
-def _serialize_s(obj):
-    """Convert a json-like object to a string"""
-    # We sort the keys to ensure
-    # that the same object always gets serialized to the same string.
-    return json.dumps(obj, sort_keys=True, ensure_ascii=False)
-
-
-def _deserialize_s(obj):
-    """The inverse of _serialize_s"""
-    return json.loads(obj)
-
-
-def _serialize(obj):
-    # llmchain wants a list of "Generation" objects, so we simply
-    # stick this regular text into it.
-    return [Generation(text=_serialize_s(obj))]
-
-
-def _deserialize(obj):
-    # (The inverse of _serialize)
-    try:
-        return _deserialize_s(obj[0].text)
-    except json.JSONDecodeError:
-        return None
-
-
-def _filehash(path):
-    """Fast hash of a file - about 1ms per MB."""
-    bufsize = 65536
-    h = md5()
-    with open(path, "rb") as f:
-        while True:
-            data = f.read(bufsize)
-            if not data:
-                break
-            h.update(data)
-    return h.hexdigest()
-
-
-def read_doc(path, citation, key, chunk_chars=3000, overlap=100, disable_check=False):
-    logger = logging.getLogger(__name__)
-    logger.debug(f"Creating cache key for {path}")
-    cache_key = _serialize_s(
-        dict(
-            hash=str(_filehash(path)),
-            citation=citation,
-            key=key,
-            chunk_chars=chunk_chars,
-            overlap=overlap,
-            disable_check=disable_check,
-            version=__version__,
-        )
-    )
-    logger.debug(f"Looking up cache key for {path}")
-    cache_lookup = _get_ocr_cache().lookup(prompt=cache_key, llm_string="")
-
-    out = None
-    successful_lookup = False
-    cache_exists = cache_lookup is not None
-    if cache_exists:
-        logger.debug(f"Found cache key for {path}")
-        out = _deserialize(cache_lookup)
-
-    successful_lookup = out is not None
-    if successful_lookup:
-        logger.debug(f"Succesfully loaded cache key for {path}")
-    elif cache_exists:
-        logger.debug(f"Failed to decode existing cache for {path}")
-
-    if out is None:
-        logger.debug(f"Did not load cache, so parsing {path}")
-
-        # The actual call:
-        out = _read_doc(
-            path=path,
-            citation=citation,
-            key=key,
-            chunk_chars=chunk_chars,
-            overlap=overlap,
-            disable_check=disable_check,
-        )
-
-        logger.debug(f"Done parsing document {path}")
-    if not successful_lookup:
-        logger.debug(f"Updating cache for {path}")
-        _get_ocr_cache().update(
-            prompt=cache_key,
-            llm_string="",
-            return_val=_serialize(out),
-        )
-    return out
-
-
-def _read_doc(path, citation, key, chunk_chars=3000, overlap=100, disable_check=False):
-    """Parse a document into chunks."""
-    if isinstance(path, Path):
-        path = str(path)
-    if path.endswith(".pdf"):
-        return parse_pdf(path, citation, key, chunk_chars, overlap)
-    elif path.endswith(".txt"):
-        return parse_txt(path, citation, key, chunk_chars, overlap)
-    elif path.endswith(".html"):
-        return parse_txt(path, citation, key, chunk_chars, overlap, html=True)
-    else:
-        return parse_code_txt(path, citation, key, chunk_chars, overlap)
+import json
+import logging
+import os
+from hashlib import md5
+from pathlib import Path
+
+from html2text import html2text
+from langchain.cache import SQLiteCache
+from langchain.schema import Generation
+from langchain.text_splitter import TokenTextSplitter
+
+from .paths import OCR_CACHE_PATH
+from .version import __version__
+
+OCR_CACHE = None
+
+
+def _get_ocr_cache() -> SQLiteCache:
+    """Used to lazily create the cache directory and cache object."""
+    global OCR_CACHE
+    if OCR_CACHE is None:
+        os.makedirs(os.path.dirname(OCR_CACHE_PATH), exist_ok=True)
+        OCR_CACHE = SQLiteCache(OCR_CACHE_PATH)
+    return OCR_CACHE
+
+
+TextSplitter = TokenTextSplitter
+
+
+def parse_pdf(path, citation, key, chunk_chars=2000, overlap=50):
+    import pypdf
+
+    pdfFileObj = open(path, "rb")
+    pdfReader = pypdf.PdfReader(pdfFileObj)
+    splits = []
+    split = ""
+    pages = []
+    metadatas = []
+    for i, page in enumerate(pdfReader.pages):
+        split += page.extract_text()
+        pages.append(str(i + 1))
+        # split could be so long it needs to be split
+        # into multiple chunks. Or it could be so short
+        # that it needs to be combined with the next chunk.
+        while len(split) > chunk_chars:
+            splits.append(split[:chunk_chars])
+            # pretty formatting of pages (e.g. 1-3, 4, 5-7)
+            pg = "-".join([pages[0], pages[-1]])
+            metadatas.append(
+                dict(
+                    citation=citation,
+                    dockey=key,
+                    key=f"{key} pages {pg}",
+                )
+            )
+            split = split[chunk_chars - overlap :]
+            pages = [str(i + 1)]
+    if len(split) > overlap:
+        splits.append(split[:chunk_chars])
+        pg = "-".join([pages[0], pages[-1]])
+        metadatas.append(
+            dict(
+                citation=citation,
+                dockey=key,
+                key=f"{key} pages {pg}",
+            )
+        )
+    pdfFileObj.close()
+    return splits, metadatas
+
+
+def parse_txt(path, citation, key, chunk_chars=2000, overlap=50, html=False):
+    try:
+        with open(path) as f:
+            doc = f.read()
+    except UnicodeDecodeError:
+        with open(path, encoding="utf-8", errors="ignore") as f:
+            doc = f.read()
+    if html:
+        doc = html2text(doc)
+    # yo, no idea why but the texts are not split correctly
+    text_splitter = TextSplitter(chunk_size=chunk_chars, chunk_overlap=overlap)
+    texts = text_splitter.split_text(doc)
+    return texts, [dict(citation=citation, dockey=key, key=key)] * len(texts)
+
+
+def parse_code_txt(path, citation, key, chunk_chars=2000, overlap=50):
+    """Parse a document into chunks, based on line numbers (for code)."""
+
+    splits = []
+    split = ""
+    metadatas = []
+    last_line = 0
+
+    with open(path) as f:
+        for i, line in enumerate(f):
+            split += line
+            if len(split) > chunk_chars:
+                splits.append(split[:chunk_chars])
+                metadatas.append(
+                    dict(
+                        citation=citation,
+                        dockey=key,
+                        key=f"{key} lines {last_line}-{i}",
+                    )
+                )
+                split = split[chunk_chars - overlap :]
+                last_line = i
+    if len(split) > overlap:
+        splits.append(split[:chunk_chars])
+        metadatas.append(
+            dict(
+                citation=citation,
+                dockey=key,
+                key=f"{key} lines {last_line}-{i}",
+            )
+        )
+    return splits, metadatas
+
+
+def _serialize_s(obj):
+    """Convert a json-like object to a string"""
+    # We sort the keys to ensure
+    # that the same object always gets serialized to the same string.
+    return json.dumps(obj, sort_keys=True, ensure_ascii=False)
+
+
+def _deserialize_s(obj):
+    """The inverse of _serialize_s"""
+    return json.loads(obj)
+
+
+def _serialize(obj):
+    # llmchain wants a list of "Generation" objects, so we simply
+    # stick this regular text into it.
+    return [Generation(text=_serialize_s(obj))]
+
+
+def _deserialize(obj):
+    # (The inverse of _serialize)
+    try:
+        return _deserialize_s(obj[0].text)
+    except json.JSONDecodeError:
+        return None
+
+
+def _filehash(path):
+    """Fast hash of a file - about 1ms per MB."""
+    bufsize = 65536
+    h = md5()
+    with open(path, "rb") as f:
+        while True:
+            data = f.read(bufsize)
+            if not data:
+                break
+            h.update(data)
+    return h.hexdigest()
+
+
+def read_doc(path, citation, key, chunk_chars=3000, overlap=100, disable_check=False):
+    logger = logging.getLogger(__name__)
+    logger.debug(f"Creating cache key for {path}")
+    cache_key = _serialize_s(
+        dict(
+            hash=str(_filehash(path)),
+            citation=citation,
+            key=key,
+            chunk_chars=chunk_chars,
+            overlap=overlap,
+            disable_check=disable_check,
+            version=__version__,
+        )
+    )
+    logger.debug(f"Looking up cache key for {path}")
+    cache_lookup = _get_ocr_cache().lookup(prompt=cache_key, llm_string="")
+
+    out = None
+    successful_lookup = False
+    cache_exists = cache_lookup is not None
+    if cache_exists:
+        logger.debug(f"Found cache key for {path}")
+        out = _deserialize(cache_lookup)
+
+    successful_lookup = out is not None
+    if successful_lookup:
+        logger.debug(f"Succesfully loaded cache key for {path}")
+    elif cache_exists:
+        logger.debug(f"Failed to decode existing cache for {path}")
+
+    if out is None:
+        logger.debug(f"Did not load cache, so parsing {path}")
+
+        # The actual call:
+        out = _read_doc(
+            path=path,
+            citation=citation,
+            key=key,
+            chunk_chars=chunk_chars,
+            overlap=overlap,
+            disable_check=disable_check,
+        )
+
+        logger.debug(f"Done parsing document {path}")
+    if not successful_lookup:
+        logger.debug(f"Updating cache for {path}")
+        _get_ocr_cache().update(
+            prompt=cache_key,
+            llm_string="",
+            return_val=_serialize(out),
+        )
+    return out
+
+
+def _read_doc(path, citation, key, chunk_chars=3000, overlap=100, disable_check=False):
+    """Parse a document into chunks."""
+    if isinstance(path, Path):
+        path = str(path)
+    if path.endswith(".pdf"):
+        return parse_pdf(path, citation, key, chunk_chars, overlap)
+    elif path.endswith(".txt"):
+        return parse_txt(path, citation, key, chunk_chars, overlap)
+    elif path.endswith(".html"):
+        return parse_txt(path, citation, key, chunk_chars, overlap, html=True)
+    else:
+        return parse_code_txt(path, citation, key, chunk_chars, overlap)
```

### Comparing `paper-qa-1.4.0/paperqa/types.py` & `paper-qa-1.4.1/paperqa/types.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.4.0/paperqa/utils.py` & `paper-qa-1.4.1/paperqa/utils.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-import math
-import string
-
-import pypdf
-
-from .types import StrPath
-
-
-def maybe_is_text(s, thresh=2.5):
-    if len(s) == 0:
-        return False
-    # Calculate the entropy of the string
-    entropy = 0
-    for c in string.printable:
-        p = s.count(c) / len(s)
-        if p > 0:
-            entropy += -p * math.log2(p)
-
-    # Check if the entropy is within a reasonable range for text
-    if entropy > thresh:
-        return True
-    return False
-
-
-def maybe_is_code(s):
-    if len(s) == 0:
-        return False
-    # Check if the string contains a lot of non-ascii characters
-    if len([c for c in s if ord(c) > 128]) / len(s) > 0.1:
-        return True
-    return False
-
-
-def strings_similarity(s1, s2):
-    if len(s1) == 0 or len(s2) == 0:
-        return 0
-    # break the strings into words
-    s1 = set(s1.split())
-    s2 = set(s2.split())
-    # return the similarity ratio
-    return len(s1.intersection(s2)) / len(s1.union(s2))
-
-
-def maybe_is_truncated(s):
-    punct = [".", "!", "?", '"']
-    if s[-1] in punct:
-        return False
-    return True
-
-
-def maybe_is_html(s):
-    if len(s) == 0:
-        return False
-    # check for html tags
-    if "<body" in s or "<html" in s or "<div" in s:
-        return True
-
-
-def count_pdf_pages(file_path: StrPath) -> int:
-    with open(file_path, "rb") as pdf_file:
-        pdf_reader = pypdf.PdfReader(pdf_file)
-        num_pages = len(pdf_reader.pages)
-    return num_pages
-
-
-def md5sum(file_path: StrPath) -> str:
-    import hashlib
-
-    with open(file_path, "rb") as f:
-        return hashlib.md5(f.read()).hexdigest()
+import math
+import string
+
+import pypdf
+
+from .types import StrPath
+
+
+def maybe_is_text(s, thresh=2.5):
+    if len(s) == 0:
+        return False
+    # Calculate the entropy of the string
+    entropy = 0
+    for c in string.printable:
+        p = s.count(c) / len(s)
+        if p > 0:
+            entropy += -p * math.log2(p)
+
+    # Check if the entropy is within a reasonable range for text
+    if entropy > thresh:
+        return True
+    return False
+
+
+def maybe_is_code(s):
+    if len(s) == 0:
+        return False
+    # Check if the string contains a lot of non-ascii characters
+    if len([c for c in s if ord(c) > 128]) / len(s) > 0.1:
+        return True
+    return False
+
+
+def strings_similarity(s1, s2):
+    if len(s1) == 0 or len(s2) == 0:
+        return 0
+    # break the strings into words
+    s1 = set(s1.split())
+    s2 = set(s2.split())
+    # return the similarity ratio
+    return len(s1.intersection(s2)) / len(s1.union(s2))
+
+
+def maybe_is_truncated(s):
+    punct = [".", "!", "?", '"']
+    if s[-1] in punct:
+        return False
+    return True
+
+
+def maybe_is_html(s):
+    if len(s) == 0:
+        return False
+    # check for html tags
+    if "<body" in s or "<html" in s or "<div" in s:
+        return True
+
+
+def count_pdf_pages(file_path: StrPath) -> int:
+    with open(file_path, "rb") as pdf_file:
+        pdf_reader = pypdf.PdfReader(pdf_file)
+        num_pages = len(pdf_reader.pages)
+    return num_pages
+
+
+def md5sum(file_path: StrPath) -> str:
+    import hashlib
+
+    with open(file_path, "rb") as f:
+        return hashlib.md5(f.read()).hexdigest()
```

### Comparing `paper-qa-1.4.0/setup.py` & `paper-qa-1.4.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from setuptools import setup
-
-exec(open("paperqa/version.py").read())
-
-with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
-
-setup(
-    name="paper-qa",
-    version=__version__,
-    description="LLM Chain for answering questions from docs ",
-    author="Andrew White",
-    author_email="white.d.andrew@gmail.com",
-    url="https://github.com/whitead/paper-qa",
-    license="MIT",
-    packages=["paperqa", "paperqa.contrib"],
-    install_requires=[
-        "pypdf",
-        "langchain>=0.0.157",
-        "openai>=0.27.0",
-        "faiss-cpu",
-        "PyCryptodome",
-        "html2text",
-        "tiktoken",
-        "rmrkl>=0.0.2",
-    ],
-    test_suite="tests",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-)
-1
+from setuptools import setup
+
+exec(open("paperqa/version.py").read())
+
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
+setup(
+    name="paper-qa",
+    version=__version__,
+    description="LLM Chain for answering questions from docs ",
+    author="Andrew White",
+    author_email="white.d.andrew@gmail.com",
+    url="https://github.com/whitead/paper-qa",
+    license="MIT",
+    packages=["paperqa", "paperqa.contrib"],
+    install_requires=[
+        "pypdf",
+        "langchain>=0.0.170",
+        "openai>=0.27.0",
+        "faiss-cpu",
+        "PyCryptodome",
+        "html2text",
+        "tiktoken",
+        "rmrkl>=0.0.2",
+    ],
+    test_suite="tests",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+)
+1
```

### Comparing `paper-qa-1.4.0/tests/test_paperqa.py` & `paper-qa-1.4.1/tests/test_paperqa.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,286 +1,286 @@
-import os
-import pickle
-from unittest import IsolatedAsyncioTestCase
-
-import requests
-from langchain.llms import OpenAI
-from langchain.llms.fake import FakeListLLM
-
-import paperqa
-from paperqa.utils import strings_similarity
-
-
-def test_maybe_is_text():
-    assert paperqa.maybe_is_text(
-        "This is a test. The sample conc. was 1.0 mM (at 245 ^F)"
-    )
-    assert not paperqa.maybe_is_text("\\C0\\C0\\B1\x00")
-    # get front page of wikipedia
-    r = requests.get("https://en.wikipedia.org/wiki/National_Flag_of_Canada_Day")
-    assert paperqa.maybe_is_text(r.text)
-
-    # now force it to contain lots of weird encoding
-    bad_text = r.text.encode("latin1", "ignore").decode("utf-16", "ignore")
-    assert not paperqa.maybe_is_text(bad_text)
-
-
-def test_docs():
-    doc_path = "example.txt"
-    with open(doc_path, "w", encoding="utf-8") as f:
-        # get front page of wikipedia
-        r = requests.get("https://en.wikipedia.org/wiki/National_Flag_of_Canada_Day")
-        f.write(r.text)
-    llm = OpenAI(temperature=0.1, model_name="text-ada-001")
-    docs = paperqa.Docs(llm=llm)
-    docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
-    assert docs.docs[doc_path]["key"] == "Wiki2023"
-    os.remove(doc_path)
-
-
-def test_evidence():
-    doc_path = "example.txt"
-    with open(doc_path, "w", encoding="utf-8") as f:
-        # get wiki page about politician
-        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
-        f.write(r.text)
-    docs = paperqa.Docs()
-    docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
-    evidence = docs.get_evidence(
-        paperqa.Answer("For which state was he a governor"), k=1, max_sources=1
-    )
-    print(evidence.contexts[0].context, evidence.context)
-    assert "Missouri" in evidence.context
-    os.remove(doc_path)
-
-
-def test_query():
-    doc_path = "example.txt"
-    with open(doc_path, "w", encoding="utf-8") as f:
-        # get wiki page about politician
-        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
-        f.write(r.text)
-    docs = paperqa.Docs()
-    docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
-    docs.query("What is Frederick Bates's greatest accomplishment?")
-    os.remove(doc_path)
-
-
-class Test(IsolatedAsyncioTestCase):
-    async def test_aquery(self):
-        doc_path = "example.txt"
-        with open(doc_path, "w", encoding="utf-8") as f:
-            # get wiki page about politician
-            r = requests.get(
-                "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)"
-            )
-            f.write(r.text)
-        docs = paperqa.Docs()
-        docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
-        await docs.aquery("What is Frederick Bates's greatest accomplishment?")
-        os.remove(doc_path)
-
-
-def test_doc_match():
-    doc_path = "example.txt"
-    with open(doc_path, "w", encoding="utf-8") as f:
-        # get wiki page about politician
-        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
-        f.write(r.text)
-    docs = paperqa.Docs()
-    docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
-    docs.doc_match("What is Frederick Bates's greatest accomplishment?")
-    os.remove(doc_path)
-
-
-def test_docs_pickle():
-    doc_path = "example.txt"
-    with open(doc_path, "w", encoding="utf-8") as f:
-        # get front page of wikipedia
-        r = requests.get("https://en.wikipedia.org/wiki/National_Flag_of_Canada_Day")
-        f.write(r.text)
-    llm = OpenAI(temperature=0.0, model_name="text-babbage-001")
-    docs = paperqa.Docs(llm=llm)
-    docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now", chunk_chars=1000)
-    docs_pickle = pickle.dumps(docs)
-    docs2 = pickle.loads(docs_pickle)
-    docs2.update_llm(llm)
-    assert len(docs.docs) == len(docs2.docs)
-    assert (
-        strings_similarity(
-            docs.get_evidence(
-                paperqa.Answer("What date is flag day in Canada?"),
-                k=3,
-                max_sources=1,
-            ).context,
-            docs2.get_evidence(
-                paperqa.Answer("What date is flag day in Canada?"),
-                k=3,
-                max_sources=1,
-            ).context,
-        )
-        > 0.75
-    )
-    os.remove(doc_path)
-
-
-def test_bad_context():
-    doc_path = "example.html"
-    with open(doc_path, "w", encoding="utf-8") as f:
-        # get wiki page about politician
-        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
-        f.write(r.text)
-    docs = paperqa.Docs()
-    docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
-    answer = docs.query(
-        "What year was Barack Obama born?",
-        length_prompt="about 20 words",
-    )
-    assert "cannot answer" in answer.answer
-    os.remove(doc_path)
-
-
-def test_repeat_keys():
-    doc_path = "example.txt"
-    with open(doc_path, "w", encoding="utf-8") as f:
-        # get wiki page about politician
-        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
-        f.write(r.text)
-    docs = paperqa.Docs(llm=OpenAI(temperature=0.0, model_name="text-ada-001"))
-    docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
-    try:
-        docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
-    except ValueError:
-        pass
-    assert len(docs.docs) == 1
-
-    # now with different paths
-    doc_path2 = "example2.txt"
-    with open(doc_path2, "w", encoding="utf-8") as f:
-        # get wiki page about politician
-        f.write(r.text)
-    docs.add(doc_path2, "WikiMedia Foundation, 2023, Accessed now")
-    assert len(docs.docs) == 2
-
-    # check keys
-    assert docs.docs[doc_path]["key"] == "Wiki2023"
-    assert docs.docs[doc_path2]["key"] == "Wiki2023a"
-
-    os.remove(doc_path)
-    os.remove(doc_path2)
-
-
-def test_pdf_reader():
-    tests_dir = os.path.dirname(os.path.abspath(__file__))
-    doc_path = os.path.join(tests_dir, "paper.pdf")
-    docs = paperqa.Docs(llm=OpenAI(temperature=0.0, model_name="text-curie-001"))
-    docs.add(doc_path, "Wellawatte et al, XAI Review, 2023")
-    answer = docs.query("Are counterfactuals actionable?")
-    assert "yes" in answer.answer or "Yes" in answer.answer
-
-
-def test_prompt_length():
-    doc_path = "example.txt"
-    with open(doc_path, "w", encoding="utf-8") as f:
-        # get wiki page about politician
-        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
-        f.write(r.text)
-    docs = paperqa.Docs()
-    docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
-    docs.query("What is the name of the politician?", length_prompt="25 words")
-
-
-def test_doc_preview():
-    doc_path = "example.txt"
-    with open(doc_path, "w", encoding="utf-8") as f:
-        # get wiki page about politician
-        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
-        f.write(r.text)
-    docs = paperqa.Docs(llm=OpenAI(temperature=0.0, model_name="text-ada-001"))
-    docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
-    assert len(docs.doc_previews()) == 1
-
-
-def test_code():
-    # load this script
-    doc_path = os.path.abspath(__file__)
-    docs = paperqa.Docs(llm=OpenAI(temperature=0.0, model_name="text-ada-001"))
-    docs.add(doc_path, "test_paperqa.py", key="test", disable_check=True)
-    assert len(docs.docs) == 1
-    docs.query("What function tests the preview?")
-
-
-def test_citation():
-    doc_path = "example.txt"
-    with open(doc_path, "w", encoding="utf-8") as f:
-        # get wiki page about politician
-        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
-        f.write(r.text)
-    docs = paperqa.Docs()
-    docs.add(doc_path)
-    assert (
-        list(docs.docs.values())[0]["metadata"][0]["key"] == "Wikipedia2023"
-        or list(docs.docs.values())[0]["metadata"][0]["key"] == "Frederick2023"
-    )
-
-
-def test_dockey_filter():
-    """Test that we can filter evidence with dockeys"""
-    doc_path = "example2.txt"
-    with open(doc_path, "w", encoding="utf-8") as f:
-        # get wiki page about politician
-        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
-        f.write(r.text)
-    docs = paperqa.Docs()
-    docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
-    # add with new dockey
-    docs.add("example.txt", "WikiMedia Foundation, 2023, Accessed now", key="test")
-    answer = paperqa.Answer("What country is Bates from?")
-    docs.get_evidence(answer, key_filter=["test"])
-
-
-def test_query_filter():
-    """Test that we can filter evidence with in query"""
-    doc_path = "example2.txt"
-    with open(doc_path, "w", encoding="utf-8") as f:
-        # get wiki page about politician
-        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
-        f.write(r.text)
-    docs = paperqa.Docs()
-    docs.add(
-        doc_path,
-        "Information about Fredrick Bates, WikiMedia Foundation, 2023, Accessed now",
-    )
-    # add with new dockey
-    docs.add("example.txt", "WikiMedia Foundation, 2023, Accessed now", key="test")
-    answer = docs.query("What country is Bates from?", key_filter=True)
-    # the filter shouldn't trigger, so just checking that it doesn't crash
-
-
-def test_nonopenai_model():
-    responses = ["This is a test", "This is another test"] * 50
-    model = FakeListLLM(responses=responses)
-    doc_path = "example.txt"
-    with open(doc_path, "w", encoding="utf-8") as f:
-        # get wiki page about politician
-        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
-        f.write(r.text)
-    docs = paperqa.Docs(llm=model)
-    docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
-    answer = docs.query("What country is Bates from?")
-
-
-def test_agent():
-    docs = paperqa.Docs()
-    answer = paperqa.run_agent(docs, "What compounds target AKT1")
-    print(answer)
-
-
-def test_zotera():
-    from paperqa.contrib import ZoteroDB
-
-    docs = paperqa.Docs()
-    try:
-        zotero = ZoteroDB(library_type="user")  # "group" if group library
-    except ValueError:
-        # close enough
-        return
+import os
+import pickle
+from unittest import IsolatedAsyncioTestCase
+
+import requests
+from langchain.llms import OpenAI
+from langchain.llms.fake import FakeListLLM
+
+import paperqa
+from paperqa.utils import strings_similarity
+
+
+def test_maybe_is_text():
+    assert paperqa.maybe_is_text(
+        "This is a test. The sample conc. was 1.0 mM (at 245 ^F)"
+    )
+    assert not paperqa.maybe_is_text("\\C0\\C0\\B1\x00")
+    # get front page of wikipedia
+    r = requests.get("https://en.wikipedia.org/wiki/National_Flag_of_Canada_Day")
+    assert paperqa.maybe_is_text(r.text)
+
+    # now force it to contain lots of weird encoding
+    bad_text = r.text.encode("latin1", "ignore").decode("utf-16", "ignore")
+    assert not paperqa.maybe_is_text(bad_text)
+
+
+def test_docs():
+    doc_path = "example.txt"
+    with open(doc_path, "w", encoding="utf-8") as f:
+        # get front page of wikipedia
+        r = requests.get("https://en.wikipedia.org/wiki/National_Flag_of_Canada_Day")
+        f.write(r.text)
+    llm = OpenAI(temperature=0.1, model_name="text-ada-001")
+    docs = paperqa.Docs(llm=llm)
+    docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
+    assert docs.docs[doc_path]["key"] == "Wiki2023"
+    os.remove(doc_path)
+
+
+def test_evidence():
+    doc_path = "example.txt"
+    with open(doc_path, "w", encoding="utf-8") as f:
+        # get wiki page about politician
+        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        f.write(r.text)
+    docs = paperqa.Docs()
+    docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
+    evidence = docs.get_evidence(
+        paperqa.Answer("For which state was he a governor"), k=1, max_sources=1
+    )
+    print(evidence.contexts[0].context, evidence.context)
+    assert "Missouri" in evidence.context
+    os.remove(doc_path)
+
+
+def test_query():
+    doc_path = "example.txt"
+    with open(doc_path, "w", encoding="utf-8") as f:
+        # get wiki page about politician
+        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        f.write(r.text)
+    docs = paperqa.Docs()
+    docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
+    docs.query("What is Frederick Bates's greatest accomplishment?")
+    os.remove(doc_path)
+
+
+class Test(IsolatedAsyncioTestCase):
+    async def test_aquery(self):
+        doc_path = "example.txt"
+        with open(doc_path, "w", encoding="utf-8") as f:
+            # get wiki page about politician
+            r = requests.get(
+                "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)"
+            )
+            f.write(r.text)
+        docs = paperqa.Docs()
+        docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
+        await docs.aquery("What is Frederick Bates's greatest accomplishment?")
+        os.remove(doc_path)
+
+
+def test_doc_match():
+    doc_path = "example.txt"
+    with open(doc_path, "w", encoding="utf-8") as f:
+        # get wiki page about politician
+        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        f.write(r.text)
+    docs = paperqa.Docs()
+    docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
+    docs.doc_match("What is Frederick Bates's greatest accomplishment?")
+    os.remove(doc_path)
+
+
+def test_docs_pickle():
+    doc_path = "example.txt"
+    with open(doc_path, "w", encoding="utf-8") as f:
+        # get front page of wikipedia
+        r = requests.get("https://en.wikipedia.org/wiki/National_Flag_of_Canada_Day")
+        f.write(r.text)
+    llm = OpenAI(temperature=0.0, model_name="text-babbage-001")
+    docs = paperqa.Docs(llm=llm)
+    docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now", chunk_chars=1000)
+    docs_pickle = pickle.dumps(docs)
+    docs2 = pickle.loads(docs_pickle)
+    docs2.update_llm(llm)
+    assert len(docs.docs) == len(docs2.docs)
+    assert (
+        strings_similarity(
+            docs.get_evidence(
+                paperqa.Answer("What date is flag day in Canada?"),
+                k=3,
+                max_sources=1,
+            ).context,
+            docs2.get_evidence(
+                paperqa.Answer("What date is flag day in Canada?"),
+                k=3,
+                max_sources=1,
+            ).context,
+        )
+        > 0.75
+    )
+    os.remove(doc_path)
+
+
+def test_bad_context():
+    doc_path = "example.html"
+    with open(doc_path, "w", encoding="utf-8") as f:
+        # get wiki page about politician
+        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        f.write(r.text)
+    docs = paperqa.Docs()
+    docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
+    answer = docs.query(
+        "What year was Barack Obama born?",
+        length_prompt="about 20 words",
+    )
+    assert "cannot answer" in answer.answer
+    os.remove(doc_path)
+
+
+def test_repeat_keys():
+    doc_path = "example.txt"
+    with open(doc_path, "w", encoding="utf-8") as f:
+        # get wiki page about politician
+        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        f.write(r.text)
+    docs = paperqa.Docs(llm=OpenAI(temperature=0.0, model_name="text-ada-001"))
+    docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
+    try:
+        docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
+    except ValueError:
+        pass
+    assert len(docs.docs) == 1
+
+    # now with different paths
+    doc_path2 = "example2.txt"
+    with open(doc_path2, "w", encoding="utf-8") as f:
+        # get wiki page about politician
+        f.write(r.text)
+    docs.add(doc_path2, "WikiMedia Foundation, 2023, Accessed now")
+    assert len(docs.docs) == 2
+
+    # check keys
+    assert docs.docs[doc_path]["key"] == "Wiki2023"
+    assert docs.docs[doc_path2]["key"] == "Wiki2023a"
+
+    os.remove(doc_path)
+    os.remove(doc_path2)
+
+
+def test_pdf_reader():
+    tests_dir = os.path.dirname(os.path.abspath(__file__))
+    doc_path = os.path.join(tests_dir, "paper.pdf")
+    docs = paperqa.Docs(llm=OpenAI(temperature=0.0, model_name="text-curie-001"))
+    docs.add(doc_path, "Wellawatte et al, XAI Review, 2023")
+    answer = docs.query("Are counterfactuals actionable?")
+    assert "yes" in answer.answer or "Yes" in answer.answer
+
+
+def test_prompt_length():
+    doc_path = "example.txt"
+    with open(doc_path, "w", encoding="utf-8") as f:
+        # get wiki page about politician
+        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        f.write(r.text)
+    docs = paperqa.Docs()
+    docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
+    docs.query("What is the name of the politician?", length_prompt="25 words")
+
+
+def test_doc_preview():
+    doc_path = "example.txt"
+    with open(doc_path, "w", encoding="utf-8") as f:
+        # get wiki page about politician
+        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        f.write(r.text)
+    docs = paperqa.Docs(llm=OpenAI(temperature=0.0, model_name="text-ada-001"))
+    docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
+    assert len(docs.doc_previews()) == 1
+
+
+def test_code():
+    # load this script
+    doc_path = os.path.abspath(__file__)
+    docs = paperqa.Docs(llm=OpenAI(temperature=0.0, model_name="text-ada-001"))
+    docs.add(doc_path, "test_paperqa.py", key="test", disable_check=True)
+    assert len(docs.docs) == 1
+    docs.query("What function tests the preview?")
+
+
+def test_citation():
+    doc_path = "example.txt"
+    with open(doc_path, "w", encoding="utf-8") as f:
+        # get wiki page about politician
+        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        f.write(r.text)
+    docs = paperqa.Docs()
+    docs.add(doc_path)
+    assert (
+        list(docs.docs.values())[0]["metadata"][0]["key"] == "Wikipedia2023"
+        or list(docs.docs.values())[0]["metadata"][0]["key"] == "Frederick2023"
+    )
+
+
+def test_dockey_filter():
+    """Test that we can filter evidence with dockeys"""
+    doc_path = "example2.txt"
+    with open(doc_path, "w", encoding="utf-8") as f:
+        # get wiki page about politician
+        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        f.write(r.text)
+    docs = paperqa.Docs()
+    docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
+    # add with new dockey
+    docs.add("example.txt", "WikiMedia Foundation, 2023, Accessed now", key="test")
+    answer = paperqa.Answer("What country is Bates from?")
+    docs.get_evidence(answer, key_filter=["test"])
+
+
+def test_query_filter():
+    """Test that we can filter evidence with in query"""
+    doc_path = "example2.txt"
+    with open(doc_path, "w", encoding="utf-8") as f:
+        # get wiki page about politician
+        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        f.write(r.text)
+    docs = paperqa.Docs()
+    docs.add(
+        doc_path,
+        "Information about Fredrick Bates, WikiMedia Foundation, 2023, Accessed now",
+    )
+    # add with new dockey
+    docs.add("example.txt", "WikiMedia Foundation, 2023, Accessed now", key="test")
+    answer = docs.query("What country is Bates from?", key_filter=True)
+    # the filter shouldn't trigger, so just checking that it doesn't crash
+
+
+def test_nonopenai_model():
+    responses = ["This is a test", "This is another test"] * 50
+    model = FakeListLLM(responses=responses)
+    doc_path = "example.txt"
+    with open(doc_path, "w", encoding="utf-8") as f:
+        # get wiki page about politician
+        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        f.write(r.text)
+    docs = paperqa.Docs(llm=model)
+    docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
+    answer = docs.query("What country is Bates from?")
+
+
+def test_agent():
+    docs = paperqa.Docs()
+    answer = paperqa.run_agent(docs, "What compounds target AKT1")
+    print(answer)
+
+
+def test_zotera():
+    from paperqa.contrib import ZoteroDB
+
+    docs = paperqa.Docs()
+    try:
+        zotero = ZoteroDB(library_type="user")  # "group" if group library
+    except ValueError:
+        # close enough
+        return
```

