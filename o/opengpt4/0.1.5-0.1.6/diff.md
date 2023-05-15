# Comparing `tmp/opengpt4-0.1.5.tar.gz` & `tmp/opengpt4-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opengpt4-0.1.5.tar", max compression
+gzip compressed data, was "opengpt4-0.1.6.tar", max compression
```

## Comparing `opengpt4-0.1.5.tar` & `opengpt4-0.1.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    35149 2023-05-14 23:20:28.677988 opengpt4-0.1.5/LICENSE
--rw-r--r--   0        0        0     4740 2023-05-14 23:20:28.677988 opengpt4-0.1.5/README.md
--rw-r--r--   0        0        0      270 2023-05-14 23:20:28.677988 opengpt4-0.1.5/libraries/colorama/__init__.py
--rw-r--r--   0        0        0     2522 2023-05-14 23:20:28.677988 opengpt4-0.1.5/libraries/colorama/ansi.py
--rw-r--r--   0        0        0    11128 2023-05-14 23:20:28.677988 opengpt4-0.1.5/libraries/colorama/ansitowin32.py
--rw-r--r--   0        0        0     3325 2023-05-14 23:20:28.677988 opengpt4-0.1.5/libraries/colorama/initialise.py
--rw-r--r--   0        0        0     6181 2023-05-14 23:20:28.677988 opengpt4-0.1.5/libraries/colorama/win32.py
--rw-r--r--   0        0        0     7168 2023-05-14 23:20:28.677988 opengpt4-0.1.5/libraries/colorama/winterm.py
--rw-r--r--   0        0        0     1691 2023-05-14 23:20:28.677988 opengpt4-0.1.5/libraries/tempmail.py
--rw-r--r--   0        0        0     1097 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/README.md
--rw-r--r--   0        0        0     3405 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/__init__.py
--rw-r--r--   0        0        0      206 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/config.yml
--rw-r--r--   0        0        0      866 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/models/completion/chatbase/DOC.md
--rw-r--r--   0        0        0      489 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/models/completion/chatbase/README.md
--rw-r--r--   0        0        0     5320 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/models/completion/chatbase/model.py
--rw-r--r--   0        0        0      649 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/models/completion/chatgptproxy/DOC.md
--rw-r--r--   0        0        0      525 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/models/completion/chatgptproxy/README.md
--rw-r--r--   0        0        0     2406 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/models/completion/chatgptproxy/model.py
--rw-r--r--   0        0        0      624 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/models/completion/chatllama/DOC.md
--rw-r--r--   0        0        0      459 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/models/completion/chatllama/README.md
--rw-r--r--   0        0        0     1150 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/models/completion/chatllama/model.py
--rw-r--r--   0        0        0     6698 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/models/completion/forefront/DOC.md
--rw-r--r--   0        0        0     6460 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/models/completion/forefront/README.md
--rw-r--r--   0        0        0     3788 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/models/completion/forefront/attributes/conversation.py
--rw-r--r--   0        0        0     7505 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/models/completion/forefront/model.py
--rw-r--r--   0        0        0     5818 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/models/completion/forefront/tools/system/email_creation.py
--rw-r--r--   0        0        0      657 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/models/completion/forefront/tools/system/signature.py
--rw-r--r--   0        0        0      446 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/models/completion/forefront/tools/typing/response.py
--rw-r--r--   0        0        0      842 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/models/completion/italygpt/DOC.md
--rw-r--r--   0        0        0      321 2023-05-14 23:20:28.681988 opengpt4-0.1.5/opengpt/models/completion/italygpt/README.md
--rw-r--r--   0        0        0     1495 2023-05-14 23:20:28.681988 opengpt4-0.1.5/opengpt/models/completion/italygpt/model.py
--rw-r--r--   0        0        0     1208 2023-05-14 23:20:28.681988 opengpt4-0.1.5/opengpt/models/completion/usesless/DOC.md
--rw-r--r--   0        0        0      769 2023-05-14 23:20:28.681988 opengpt4-0.1.5/opengpt/models/completion/usesless/README.md
--rw-r--r--   0        0        0     1577 2023-05-14 23:20:28.681988 opengpt4-0.1.5/opengpt/models/completion/usesless/model.py
--rw-r--r--   0        0        0      418 2023-05-14 23:20:28.681988 opengpt4-0.1.5/opengpt/models/completion/usesless/tools/typing/response.py
--rw-r--r--   0        0        0     4140 2023-05-14 23:20:28.681988 opengpt4-0.1.5/opengpt/models/image/hotpot/model.py
--rw-r--r--   0        0        0     3012 2023-05-14 23:20:28.681988 opengpt4-0.1.5/opengpt/models/image/hotpot/styles.yml
--rw-r--r--   0        0        0      232 2023-05-14 23:20:28.681988 opengpt4-0.1.5/opengpt/models/image/hotpot/tools/system/id.py
--rw-r--r--   0        0        0      147 2023-05-14 23:20:28.681988 opengpt4-0.1.5/opengpt/models/image/hotpot/tools/typing/response.py
--rw-r--r--   0        0        0      414 2023-05-14 23:20:28.681988 opengpt4-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     5459 1970-01-01 00:00:00.000000 opengpt4-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-14 23:27:03.736924 opengpt4-0.1.6/LICENSE
+-rw-r--r--   0        0        0     4740 2023-05-14 23:27:03.740924 opengpt4-0.1.6/README.md
+-rw-r--r--   0        0        0      270 2023-05-14 23:27:03.740924 opengpt4-0.1.6/libraries/colorama/__init__.py
+-rw-r--r--   0        0        0     2522 2023-05-14 23:27:03.740924 opengpt4-0.1.6/libraries/colorama/ansi.py
+-rw-r--r--   0        0        0    11128 2023-05-14 23:27:03.740924 opengpt4-0.1.6/libraries/colorama/ansitowin32.py
+-rw-r--r--   0        0        0     3325 2023-05-14 23:27:03.740924 opengpt4-0.1.6/libraries/colorama/initialise.py
+-rw-r--r--   0        0        0     6181 2023-05-14 23:27:03.740924 opengpt4-0.1.6/libraries/colorama/win32.py
+-rw-r--r--   0        0        0     7168 2023-05-14 23:27:03.740924 opengpt4-0.1.6/libraries/colorama/winterm.py
+-rw-r--r--   0        0        0     1691 2023-05-14 23:27:03.740924 opengpt4-0.1.6/libraries/tempmail.py
+-rw-r--r--   0        0        0     1097 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/README.md
+-rw-r--r--   0        0        0     3408 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/__init__.py
+-rw-r--r--   0        0        0      206 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/config.yml
+-rw-r--r--   0        0        0      866 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/chatbase/DOC.md
+-rw-r--r--   0        0        0      489 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/chatbase/README.md
+-rw-r--r--   0        0        0     5320 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/chatbase/model.py
+-rw-r--r--   0        0        0      649 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/chatgptproxy/DOC.md
+-rw-r--r--   0        0        0      525 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/chatgptproxy/README.md
+-rw-r--r--   0        0        0     2406 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/chatgptproxy/model.py
+-rw-r--r--   0        0        0      624 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/chatllama/DOC.md
+-rw-r--r--   0        0        0      459 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/chatllama/README.md
+-rw-r--r--   0        0        0     1150 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/chatllama/model.py
+-rw-r--r--   0        0        0     6698 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/forefront/DOC.md
+-rw-r--r--   0        0        0     6460 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/forefront/README.md
+-rw-r--r--   0        0        0     3788 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/forefront/attributes/conversation.py
+-rw-r--r--   0        0        0     7505 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/forefront/model.py
+-rw-r--r--   0        0        0     5818 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/forefront/tools/system/email_creation.py
+-rw-r--r--   0        0        0      657 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/forefront/tools/system/signature.py
+-rw-r--r--   0        0        0      446 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/forefront/tools/typing/response.py
+-rw-r--r--   0        0        0      842 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/italygpt/DOC.md
+-rw-r--r--   0        0        0      321 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/italygpt/README.md
+-rw-r--r--   0        0        0     1495 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/italygpt/model.py
+-rw-r--r--   0        0        0     1208 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/usesless/DOC.md
+-rw-r--r--   0        0        0      769 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/usesless/README.md
+-rw-r--r--   0        0        0     1577 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/usesless/model.py
+-rw-r--r--   0        0        0      418 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/usesless/tools/typing/response.py
+-rw-r--r--   0        0        0     4140 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/image/hotpot/model.py
+-rw-r--r--   0        0        0     3012 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/image/hotpot/styles.yml
+-rw-r--r--   0        0        0      232 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/image/hotpot/tools/system/id.py
+-rw-r--r--   0        0        0      147 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/image/hotpot/tools/typing/response.py
+-rw-r--r--   0        0        0      414 2023-05-14 23:27:03.740924 opengpt4-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     5459 1970-01-01 00:00:00.000000 opengpt4-0.1.6/PKG-INFO
```

### Comparing `opengpt4-0.1.5/LICENSE` & `opengpt4-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.5/README.md` & `opengpt4-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.5/libraries/colorama/ansi.py` & `opengpt4-0.1.6/libraries/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.5/libraries/colorama/ansitowin32.py` & `opengpt4-0.1.6/libraries/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.5/libraries/colorama/initialise.py` & `opengpt4-0.1.6/libraries/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.5/libraries/colorama/win32.py` & `opengpt4-0.1.6/libraries/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.5/libraries/colorama/winterm.py` & `opengpt4-0.1.6/libraries/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.5/libraries/tempmail.py` & `opengpt4-0.1.6/libraries/tempmail.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.5/opengpt/README.md` & `opengpt4-0.1.6/opengpt/README.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.5/opengpt/__init__.py` & `opengpt4-0.1.6/opengpt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,17 @@
 		else:
 			print(Fore.RED + "Error: " + context + Style.RESET_ALL)
 			sys.exit(1)
 
 class OpenGPT:
 	@classmethod
 	def __init__(self: type, provider: Text, type: Optional[Text] = "completion", options: Optional[Union[Dict[Text, Text], None]] = None) -> None:
+	
+		self.__DIR: Text = os.getcwd()	
 		self.__LoadModels()
-		self.__DIR: Text = os.getcwd()
 		self.__TYPE: Text = type
 		self.__OPTIONS: Union[Dict[Text, Text], None] = options
 		self.__PROVIDER: Text = provider
 
 		self.__Verifications()
 		self.__MODULE: module = importlib.import_module(f"opengpt.models.{self.__TYPE}.{self.__PROVIDER}.model")
 		self.__MODEL_CLASS: type = getattr(self.__MODULE, "Model")
```

### Comparing `opengpt4-0.1.5/opengpt/models/completion/chatbase/DOC.md` & `opengpt4-0.1.6/opengpt/models/completion/chatbase/DOC.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.5/opengpt/models/completion/chatbase/model.py` & `opengpt4-0.1.6/opengpt/models/completion/chatbase/model.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.5/opengpt/models/completion/chatgptproxy/DOC.md` & `opengpt4-0.1.6/opengpt/models/completion/chatgptproxy/DOC.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.5/opengpt/models/completion/chatgptproxy/README.md` & `opengpt4-0.1.6/opengpt/models/completion/chatgptproxy/README.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.5/opengpt/models/completion/chatgptproxy/model.py` & `opengpt4-0.1.6/opengpt/models/completion/chatgptproxy/model.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.5/opengpt/models/completion/chatllama/DOC.md` & `opengpt4-0.1.6/opengpt/models/completion/chatllama/DOC.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.5/opengpt/models/completion/chatllama/model.py` & `opengpt4-0.1.6/opengpt/models/completion/chatllama/model.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.5/opengpt/models/completion/forefront/DOC.md` & `opengpt4-0.1.6/opengpt/models/completion/forefront/DOC.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.5/opengpt/models/completion/forefront/README.md` & `opengpt4-0.1.6/opengpt/models/completion/forefront/README.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.5/opengpt/models/completion/forefront/attributes/conversation.py` & `opengpt4-0.1.6/opengpt/models/completion/forefront/attributes/conversation.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.5/opengpt/models/completion/forefront/model.py` & `opengpt4-0.1.6/opengpt/models/completion/forefront/model.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.5/opengpt/models/completion/forefront/tools/system/email_creation.py` & `opengpt4-0.1.6/opengpt/models/completion/forefront/tools/system/email_creation.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.5/opengpt/models/completion/forefront/tools/system/signature.py` & `opengpt4-0.1.6/opengpt/models/completion/forefront/tools/system/signature.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.5/opengpt/models/completion/italygpt/DOC.md` & `opengpt4-0.1.6/opengpt/models/completion/italygpt/DOC.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.5/opengpt/models/completion/italygpt/model.py` & `opengpt4-0.1.6/opengpt/models/completion/italygpt/model.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.5/opengpt/models/completion/usesless/DOC.md` & `opengpt4-0.1.6/opengpt/models/completion/usesless/DOC.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.5/opengpt/models/completion/usesless/README.md` & `opengpt4-0.1.6/opengpt/models/completion/usesless/README.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.5/opengpt/models/completion/usesless/model.py` & `opengpt4-0.1.6/opengpt/models/completion/usesless/model.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.5/opengpt/models/image/hotpot/model.py` & `opengpt4-0.1.6/opengpt/models/image/hotpot/model.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.5/opengpt/models/image/hotpot/styles.yml` & `opengpt4-0.1.6/opengpt/models/image/hotpot/styles.yml`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.5/PKG-INFO` & `opengpt4-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengpt4
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 License: GPL-3.0
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

