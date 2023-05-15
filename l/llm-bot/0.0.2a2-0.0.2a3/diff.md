# Comparing `tmp/llm_bot-0.0.2a2.tar.gz` & `tmp/llm_bot-0.0.2a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_bot-0.0.2a2.tar", max compression
+gzip compressed data, was "llm_bot-0.0.2a3.tar", max compression
```

## Comparing `llm_bot-0.0.2a2.tar` & `llm_bot-0.0.2a3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35149 2023-04-26 18:09:51.267170 llm_bot-0.0.2a2/LICENSE
--rw-r--r--   0        0        0       61 2023-04-26 18:09:51.267170 llm_bot-0.0.2a2/README.md
--rw-r--r--   0        0        0        0 2023-04-26 18:09:51.267170 llm_bot-0.0.2a2/llm_bot/__init__.py
--rw-r--r--   0        0        0    13612 2023-04-28 17:32:02.416488 llm_bot-0.0.2a2/llm_bot/core.py
--rw-r--r--   0        0        0      942 2023-04-28 17:32:24.904104 llm_bot-0.0.2a2/pyproject.toml
--rw-r--r--   0        0        0      926 1970-01-01 00:00:00.000000 llm_bot-0.0.2a2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-26 18:09:51.267170 llm_bot-0.0.2a3/LICENSE
+-rw-r--r--   0        0        0       61 2023-04-26 18:09:51.267170 llm_bot-0.0.2a3/README.md
+-rw-r--r--   0        0        0        0 2023-04-26 18:09:51.267170 llm_bot-0.0.2a3/llm_bot/__init__.py
+-rw-r--r--   0        0        0    16447 2023-05-04 19:34:38.706275 llm_bot-0.0.2a3/llm_bot/core.py
+-rw-r--r--   0        0        0      942 2023-05-04 19:40:17.928420 llm_bot-0.0.2a3/pyproject.toml
+-rw-r--r--   0        0        0      926 1970-01-01 00:00:00.000000 llm_bot-0.0.2a3/PKG-INFO
```

### Comparing `llm_bot-0.0.2a2/LICENSE` & `llm_bot-0.0.2a3/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_bot-0.0.2a2/llm_bot/core.py` & `llm_bot-0.0.2a3/llm_bot/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,27 +11,30 @@
 from langchain.docstore.document import Document
 from langchain.embeddings import OpenAIEmbeddings
 from langchain.schema import BaseMessage, HumanMessage, SystemMessage
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 from langchain.vectorstores import FAISS
 import requests
 
-INDEX_FILENAME = "index.faiss"
-STORE_FILENAME = "store.pickle"
+CONTEXT_INDEX_FILENAME = "index.faiss"
+CONTEXT_STORE_FILENAME = "store.pickle"
+CHAT_INDEX_FILENAME = "chat_index.faiss"
+CHAT_STORE_FILENAME = "chat_store.pickle"
 
 
 class BaseLLMBot(ABC):
     def __init__(
         self,
         text_chunk_size: int = 1000,
         text_chunk_overlap: int = 250,
         text_separators: List[str] = [" ", ".", ",", ";", ":", "!", "?", "\n"],
         temperature: float = 0,
     ):
         self._store: FAISS = None
+        self._chat_store: FAISS = None
         self._chat = ChatOpenAI(temperature=temperature)
         self._text_chunk_size = text_chunk_size
         self._text_chunk_overlap = text_chunk_overlap
         self._text_separators = text_separators
 
     @abstractmethod
     def train(self, *args, **kwargs) -> None:
@@ -41,50 +44,71 @@
 
     @abstractmethod
     def add_to_index(self, *args, **kwargs) -> None:
         """
         Adds the given data to the index and the vector store.
         """
 
-    def fetch_from_index(self, query: str, n_results: int) -> List[Document]:
+    def fetch_from_index(
+        self, query: str, n_results: int, index: str = "context"
+    ) -> List[Document]:
         """
         Fetches the most relevant documents from the index.
 
         Args:
             query (str): The query to search for.
             n_results (int): The number of results to return.
 
         Returns:
             List[Document]: The most relevant documents.
         """
-        docs: List[Document] = self._store.similarity_search(query, k=n_results)
+        if index == "context":
+            docs: List[Document] = self._store.similarity_search(query, k=n_results)
+        elif index == "chat_history":
+            if self._chat_store is None:
+                raise ValueError("No chat history available.")
+            docs: List[Document] = self._chat_store.similarity_search(
+                query, k=n_results
+            )
+        else:
+            raise ValueError(f"Invalid index '{index}'.")
         return docs
 
     def save(self, path: Union[str, Path]) -> None:
         """
         Saves the index and the vector store to the given path.
 
         Args:
             path (Union[str, Path]): The path to save the index and vector store to.
         """
         # Assert that the path exists
         path = Path(path)
         path.mkdir(parents=True, exist_ok=True)
 
-        # Save the index
-        index_fname = str(path / INDEX_FILENAME)
+        # Save the indexes
+        index_fname = str(path / CONTEXT_INDEX_FILENAME)
         faiss.write_index(self._store.index, index_fname)
+        if self._chat_store is not None:
+            chat_index_fname = str(path / CHAT_INDEX_FILENAME)
+            faiss.write_index(self._chat_store.index, chat_index_fname)
 
-        # Save the vector store
+        # Save the vector stores
         index = self._store.index
         self._store.index = None
-        store_fname = str(path / STORE_FILENAME)
+        store_fname = str(path / CONTEXT_STORE_FILENAME)
         with open(store_fname, "wb") as f:
             pickle.dump(self._store, f)
         self._store.index = index
+        if self._chat_store is not None:
+            index = self._chat_store.index
+            self._chat_store.index = None
+            chat_store_fname = str(path / CHAT_STORE_FILENAME)
+            with open(chat_store_fname, "wb") as f:
+                pickle.dump(self._chat_store, f)
+            self._chat_store.index = index
 
     def download(self, url: str, path: Union[str, Path]) -> None:
         """
         Downloads the model (index + vector store) from a given URL and extracts it to the given
         path.
 
         Args:
@@ -113,16 +137,16 @@
             raise ValueError(f"Unknown compression format for file: {filename}")
 
         # Extract the model
         with tarfile.open(fileobj=response.raw, mode=mode) as tar:
             tar.extractall(path=path)
 
         # Assert that we have the correct files. If we don't, then we need to delete the files
-        index_fname = path / INDEX_FILENAME
-        store_fname = path / STORE_FILENAME
+        index_fname = path / CONTEXT_INDEX_FILENAME
+        store_fname = path / CONTEXT_STORE_FILENAME
         try:
             assert index_fname.exists() and store_fname.exists()
         except AssertionError as exc:
             index_fname.unlink(missing_ok=True)
             store_fname.unlink(missing_ok=True)
             raise AssertionError(
                 f"Either {index_fname} or {store_fname} does not exist."
@@ -136,46 +160,55 @@
             path (Union[str, Path]): The path to load the index and vector store from.
         """
         # Assert that the path exists
         path = Path(path)
         assert path.exists(), f"Path {path} does not exist."
 
         # Assert that both files exist
-        index_fname = path / INDEX_FILENAME
-        store_fname = path / STORE_FILENAME
+        index_fname = path / CONTEXT_INDEX_FILENAME
+        store_fname = path / CONTEXT_STORE_FILENAME
         assert (
             index_fname.exists() and store_fname.exists()
         ), f"Either {index_fname} or {store_fname} does not exist."
 
         # Load the index
         index: IndexFlat = faiss.read_index(str(index_fname))
 
         # Load the vector store
         with open(store_fname, "rb") as f:
             self._store: FAISS = pickle.load(f)
         self._store.index = index
 
+        # Load chat stuff if it exists
+        chat_index_fname = path / CHAT_INDEX_FILENAME
+        chat_store_fname = path / CHAT_STORE_FILENAME
+        if chat_index_fname.exists() and chat_store_fname.exists():
+            chat_index: IndexFlat = faiss.read_index(str(chat_index_fname))
+            with open(chat_store_fname, "rb") as f:
+                self._chat_store: FAISS = pickle.load(f)
+            self._chat_store.index = chat_index
+
     def build_messages(
         self,
         personality_prompt: str,
         user_message: str,
-        chat_history: str = None,
+        use_chat_history: bool = True,
         chat_history_prompt: str = "Aqui está o histórico da conversa até agora:",
+        number_of_chat_history_docs: int = 2,
         use_context: bool = True,
         context_prompt: str = "Aqui estão pedaços de informação que você pode usar:",
         number_of_context_docs: int = 2,
     ) -> Tuple[List[BaseMessage], List[str]]:
         """
         Builds a list of messages to send to the chatbot.
 
         Args:
             personality_prompt (str): The prompt to use for the personality.
             user_message (str): The message from the user.
-            chat_history (str, optional): The chat history. If not provided, the chat history will
-                be empty. Defaults to None.
+            use_chat_history (bool, optional): Whether to use the chat history. Defaults to True.
             chat_history_prompt (str, optional): The prompt to use for the chat history. Defaults
                 to "Aqui está o histórico da conversa até agora:".
             use_context (bool, optional): Whether to search for context documents in the vector
                 store. Defaults to True.
             context_prompt (str, optional): The prompt to use for the context documents. Defaults
                 to "Aqui estão pedaços de informação que você pode usar:".
             number_of_context_docs (int, optional): The number of context documents to use. Defaults
@@ -188,23 +221,43 @@
         # Start list of messages with the personality prompt
         messages: List[BaseMessage] = [SystemMessage(content=personality_prompt)]
 
         # If we are using context, search for context documents and add them to the prompt
         sources: List[str] = []
         if use_context:
             messages.append(SystemMessage(content=context_prompt))
-            docs = self.fetch_from_index(query=user_message, k=number_of_context_docs)
+            docs = self.fetch_from_index(
+                query=user_message, n_results=number_of_context_docs, index="context"
+            )
             sources = list(set([doc.metadata["source"] for doc in docs]))
             for doc in docs:
                 messages.append(SystemMessage(content=f"- {doc.page_content}"))
 
         # If chat history is provided, add messages for it
-        if chat_history:
-            messages.append(SystemMessage(content=chat_history_prompt))
-            messages.append(HumanMessage(content=chat_history))
+        if use_chat_history:
+            if self._chat_store:
+                messages.append(SystemMessage(content=chat_history_prompt))
+                docs = self.fetch_from_index(
+                    query=user_message,
+                    n_results=number_of_chat_history_docs,
+                    index="chat_history",
+                )
+                for doc in docs:
+                    messages.append(SystemMessage(content=f"- {doc.page_content}"))
+                self._chat_store.add_texts(
+                    texts=[f"User: {user_message}"],
+                    metadatas=[{"source": "user"}],
+                )
+            else:
+                embedding = OpenAIEmbeddings()
+                self._chat_store = FAISS.from_texts(
+                    texts=[f"User: {user_message}"],
+                    embedding=embedding,
+                    metadatas=[{"source": "user"}],
+                )
 
         # Add the user message
         messages.append(HumanMessage(content=user_message))
 
         return messages, sources
 
     def chat(self, messages: List[BaseMessage]) -> str:
@@ -213,16 +266,29 @@
 
         Args:
             messages (List[BaseMessage]): The messages to send to the chatbot.
         """
         # Send the messages to the chatbot
         ai_message = self._chat(messages)
 
-        # Return the response
-        return ai_message.content
+        # Get the response, add to index and return
+        response = ai_message.content
+        if self._chat_store:
+            self._chat_store.add_texts(
+                texts=[f"Bot: {response}"],
+                metadatas=[{"source": "bot"}],
+            )
+        else:
+            embedding = OpenAIEmbeddings()
+            self._chat_store = FAISS.from_texts(
+                texts=[f"Bot: {response}"],
+                embedding=embedding,
+                metadatas=[{"source": "bot"}],
+            )
+        return response
 
 
 class HTMLBot(BaseLLMBot):
     def train(self, documents_path: Union[str, Path]) -> None:
         """
         Trains the bot using the given documents.
```

### Comparing `llm_bot-0.0.2a2/pyproject.toml` & `llm_bot-0.0.2a3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llm-bot"
-version = "0.0.2a2"
+version = "0.0.2a3"
 description = "Python library for developing LLM bots"
 authors = ["Gabriel Gazola Milan <gabriel.gazola@poli.ufrj.br>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/prefeitura-rio/chatbot-lab"
 repository = "https://github.com/prefeitura-rio/chatbot-lab"
 keywords = ["python", "chatbot", "bot", "llm"]
```

### Comparing `llm_bot-0.0.2a2/PKG-INFO` & `llm_bot-0.0.2a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-bot
-Version: 0.0.2a2
+Version: 0.0.2a3
 Summary: Python library for developing LLM bots
 Home-page: https://github.com/prefeitura-rio/chatbot-lab
 License: GPL-3.0-only
 Keywords: python,chatbot,bot,llm
 Author: Gabriel Gazola Milan
 Author-email: gabriel.gazola@poli.ufrj.br
 Requires-Python: >=3.10,<4.0
```

