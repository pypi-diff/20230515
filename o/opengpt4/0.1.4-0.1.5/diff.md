# Comparing `tmp/opengpt4-0.1.4.tar.gz` & `tmp/opengpt4-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opengpt4-0.1.4.tar", max compression
+gzip compressed data, was "opengpt4-0.1.5.tar", max compression
```

## Comparing `opengpt4-0.1.4.tar` & `opengpt4-0.1.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    35149 2023-05-14 23:05:32.670989 opengpt4-0.1.4/LICENSE
--rw-r--r--   0        0        0     4740 2023-05-14 23:05:32.670989 opengpt4-0.1.4/README.md
--rw-r--r--   0        0        0      270 2023-05-14 23:05:32.670989 opengpt4-0.1.4/libraries/colorama/__init__.py
--rw-r--r--   0        0        0     2522 2023-05-14 23:05:32.670989 opengpt4-0.1.4/libraries/colorama/ansi.py
--rw-r--r--   0        0        0    11128 2023-05-14 23:05:32.670989 opengpt4-0.1.4/libraries/colorama/ansitowin32.py
--rw-r--r--   0        0        0     3325 2023-05-14 23:05:32.670989 opengpt4-0.1.4/libraries/colorama/initialise.py
--rw-r--r--   0        0        0     6181 2023-05-14 23:05:32.670989 opengpt4-0.1.4/libraries/colorama/win32.py
--rw-r--r--   0        0        0     7168 2023-05-14 23:05:32.670989 opengpt4-0.1.4/libraries/colorama/winterm.py
--rw-r--r--   0        0        0     1691 2023-05-14 23:05:32.670989 opengpt4-0.1.4/libraries/tempmail.py
--rw-r--r--   0        0        0     1097 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/README.md
--rw-r--r--   0        0        0     3355 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/__init__.py
--rw-r--r--   0        0        0      206 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/config.yml
--rw-r--r--   0        0        0      866 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/chatbase/DOC.md
--rw-r--r--   0        0        0      489 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/chatbase/README.md
--rw-r--r--   0        0        0     5320 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/chatbase/model.py
--rw-r--r--   0        0        0      649 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/chatgptproxy/DOC.md
--rw-r--r--   0        0        0      525 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/chatgptproxy/README.md
--rw-r--r--   0        0        0     2406 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/chatgptproxy/model.py
--rw-r--r--   0        0        0      624 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/chatllama/DOC.md
--rw-r--r--   0        0        0      459 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/chatllama/README.md
--rw-r--r--   0        0        0     1150 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/chatllama/model.py
--rw-r--r--   0        0        0     6698 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/forefront/DOC.md
--rw-r--r--   0        0        0     6460 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/forefront/README.md
--rw-r--r--   0        0        0     3788 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/forefront/attributes/conversation.py
--rw-r--r--   0        0        0     7505 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/forefront/model.py
--rw-r--r--   0        0        0     5818 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/forefront/tools/system/email_creation.py
--rw-r--r--   0        0        0      657 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/forefront/tools/system/signature.py
--rw-r--r--   0        0        0      446 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/forefront/tools/typing/response.py
--rw-r--r--   0        0        0      842 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/italygpt/DOC.md
--rw-r--r--   0        0        0      321 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/italygpt/README.md
--rw-r--r--   0        0        0     1495 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/italygpt/model.py
--rw-r--r--   0        0        0     1208 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/usesless/DOC.md
--rw-r--r--   0        0        0      769 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/usesless/README.md
--rw-r--r--   0        0        0     1577 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/usesless/model.py
--rw-r--r--   0        0        0      418 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/usesless/tools/typing/response.py
--rw-r--r--   0        0        0     4110 2023-05-14 23:05:32.674989 opengpt4-0.1.4/opengpt/models/image/hotpot/model.py
--rw-r--r--   0        0        0     3012 2023-05-14 23:05:32.674989 opengpt4-0.1.4/opengpt/models/image/hotpot/styles.yml
--rw-r--r--   0        0        0      232 2023-05-14 23:05:32.674989 opengpt4-0.1.4/opengpt/models/image/hotpot/tools/system/id.py
--rw-r--r--   0        0        0      147 2023-05-14 23:05:32.674989 opengpt4-0.1.4/opengpt/models/image/hotpot/tools/typing/response.py
--rw-r--r--   0        0        0      414 2023-05-14 23:05:32.674989 opengpt4-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     5459 1970-01-01 00:00:00.000000 opengpt4-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-14 23:20:28.677988 opengpt4-0.1.5/LICENSE
+-rw-r--r--   0        0        0     4740 2023-05-14 23:20:28.677988 opengpt4-0.1.5/README.md
+-rw-r--r--   0        0        0      270 2023-05-14 23:20:28.677988 opengpt4-0.1.5/libraries/colorama/__init__.py
+-rw-r--r--   0        0        0     2522 2023-05-14 23:20:28.677988 opengpt4-0.1.5/libraries/colorama/ansi.py
+-rw-r--r--   0        0        0    11128 2023-05-14 23:20:28.677988 opengpt4-0.1.5/libraries/colorama/ansitowin32.py
+-rw-r--r--   0        0        0     3325 2023-05-14 23:20:28.677988 opengpt4-0.1.5/libraries/colorama/initialise.py
+-rw-r--r--   0        0        0     6181 2023-05-14 23:20:28.677988 opengpt4-0.1.5/libraries/colorama/win32.py
+-rw-r--r--   0        0        0     7168 2023-05-14 23:20:28.677988 opengpt4-0.1.5/libraries/colorama/winterm.py
+-rw-r--r--   0        0        0     1691 2023-05-14 23:20:28.677988 opengpt4-0.1.5/libraries/tempmail.py
+-rw-r--r--   0        0        0     1097 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/README.md
+-rw-r--r--   0        0        0     3405 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/__init__.py
+-rw-r--r--   0        0        0      206 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/config.yml
+-rw-r--r--   0        0        0      866 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/models/completion/chatbase/DOC.md
+-rw-r--r--   0        0        0      489 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/models/completion/chatbase/README.md
+-rw-r--r--   0        0        0     5320 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/models/completion/chatbase/model.py
+-rw-r--r--   0        0        0      649 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/models/completion/chatgptproxy/DOC.md
+-rw-r--r--   0        0        0      525 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/models/completion/chatgptproxy/README.md
+-rw-r--r--   0        0        0     2406 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/models/completion/chatgptproxy/model.py
+-rw-r--r--   0        0        0      624 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/models/completion/chatllama/DOC.md
+-rw-r--r--   0        0        0      459 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/models/completion/chatllama/README.md
+-rw-r--r--   0        0        0     1150 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/models/completion/chatllama/model.py
+-rw-r--r--   0        0        0     6698 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/models/completion/forefront/DOC.md
+-rw-r--r--   0        0        0     6460 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/models/completion/forefront/README.md
+-rw-r--r--   0        0        0     3788 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/models/completion/forefront/attributes/conversation.py
+-rw-r--r--   0        0        0     7505 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/models/completion/forefront/model.py
+-rw-r--r--   0        0        0     5818 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/models/completion/forefront/tools/system/email_creation.py
+-rw-r--r--   0        0        0      657 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/models/completion/forefront/tools/system/signature.py
+-rw-r--r--   0        0        0      446 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/models/completion/forefront/tools/typing/response.py
+-rw-r--r--   0        0        0      842 2023-05-14 23:20:28.677988 opengpt4-0.1.5/opengpt/models/completion/italygpt/DOC.md
+-rw-r--r--   0        0        0      321 2023-05-14 23:20:28.681988 opengpt4-0.1.5/opengpt/models/completion/italygpt/README.md
+-rw-r--r--   0        0        0     1495 2023-05-14 23:20:28.681988 opengpt4-0.1.5/opengpt/models/completion/italygpt/model.py
+-rw-r--r--   0        0        0     1208 2023-05-14 23:20:28.681988 opengpt4-0.1.5/opengpt/models/completion/usesless/DOC.md
+-rw-r--r--   0        0        0      769 2023-05-14 23:20:28.681988 opengpt4-0.1.5/opengpt/models/completion/usesless/README.md
+-rw-r--r--   0        0        0     1577 2023-05-14 23:20:28.681988 opengpt4-0.1.5/opengpt/models/completion/usesless/model.py
+-rw-r--r--   0        0        0      418 2023-05-14 23:20:28.681988 opengpt4-0.1.5/opengpt/models/completion/usesless/tools/typing/response.py
+-rw-r--r--   0        0        0     4140 2023-05-14 23:20:28.681988 opengpt4-0.1.5/opengpt/models/image/hotpot/model.py
+-rw-r--r--   0        0        0     3012 2023-05-14 23:20:28.681988 opengpt4-0.1.5/opengpt/models/image/hotpot/styles.yml
+-rw-r--r--   0        0        0      232 2023-05-14 23:20:28.681988 opengpt4-0.1.5/opengpt/models/image/hotpot/tools/system/id.py
+-rw-r--r--   0        0        0      147 2023-05-14 23:20:28.681988 opengpt4-0.1.5/opengpt/models/image/hotpot/tools/typing/response.py
+-rw-r--r--   0        0        0      414 2023-05-14 23:20:28.681988 opengpt4-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5459 1970-01-01 00:00:00.000000 opengpt4-0.1.5/PKG-INFO
```

### Comparing `opengpt4-0.1.4/LICENSE` & `opengpt4-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.4/README.md` & `opengpt4-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.4/libraries/colorama/ansi.py` & `opengpt4-0.1.5/libraries/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.4/libraries/colorama/ansitowin32.py` & `opengpt4-0.1.5/libraries/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.4/libraries/colorama/initialise.py` & `opengpt4-0.1.5/libraries/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.4/libraries/colorama/win32.py` & `opengpt4-0.1.5/libraries/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.4/libraries/colorama/winterm.py` & `opengpt4-0.1.5/libraries/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.4/libraries/tempmail.py` & `opengpt4-0.1.5/libraries/tempmail.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.4/opengpt/README.md` & `opengpt4-0.1.5/opengpt/README.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.4/opengpt/__init__.py` & `opengpt4-0.1.5/opengpt/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Optional, Union, Dict, List, Text
 from libraries.colorama import init, Fore, Style
 import importlib
 import yaml
 import sys
 import inspect
+import os
 
 init()
 
 class OpenGPTError(Exception):
 	@staticmethod
 	def Print(context: Text, warn: Optional[bool] = False) -> None:
 		if warn:
@@ -16,14 +17,15 @@
 			print(Fore.RED + "Error: " + context + Style.RESET_ALL)
 			sys.exit(1)
 
 class OpenGPT:
 	@classmethod
 	def __init__(self: type, provider: Text, type: Optional[Text] = "completion", options: Optional[Union[Dict[Text, Text], None]] = None) -> None:
 		self.__LoadModels()
+		self.__DIR: Text = os.getcwd()
 		self.__TYPE: Text = type
 		self.__OPTIONS: Union[Dict[Text, Text], None] = options
 		self.__PROVIDER: Text = provider
 
 		self.__Verifications()
 		self.__MODULE: module = importlib.import_module(f"opengpt.models.{self.__TYPE}.{self.__PROVIDER}.model")
 		self.__MODEL_CLASS: type = getattr(self.__MODULE, "Model")
@@ -51,15 +53,15 @@
 
 			self.__model = self.__MODEL_CLASS(**self.__OPTIONS)
 		else:
 			self.__model = self.__MODEL_CLASS()
 
 	@classmethod
 	def __LoadModels(self: type) -> None:
-		self.__DATA: Dict[Text, Text] = yaml.safe_load(open("opengpt/config.yml").read())
+		self.__DATA: Dict[Text, Text] = yaml.safe_load(open(self.__DIR + "/config.yml").read())
 
 	@classmethod
 	def __Verifications(self: type) -> None:
 		exists: bool = False
 
 		if self.__TYPE not in self.__DATA["models"]:
 			OpenGPTError.Print(f"The type \"{self.__TYPE}\" not be founded. Try: {', '.join(self.__DATA['models'])}")
@@ -92,8 +94,8 @@
 	@classmethod
 	def __getattr__(self: type, name: Text) -> None:
 		if hasattr(self.__model, name):
 			attr: type = getattr(self.__model, name)
 			if callable(attr):
 				return lambda *args, **kwargs: attr(*args, **kwargs)
 			return attr
-		raise AttributeError(f"\"OpenGPT\" object has no attribute \"{name}\"")
+		raise AttributeError(f"\"OpenGPT\" object has no attribute \"{name}\"")
```

### Comparing `opengpt4-0.1.4/opengpt/models/completion/chatbase/DOC.md` & `opengpt4-0.1.5/opengpt/models/completion/chatbase/DOC.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.4/opengpt/models/completion/chatbase/model.py` & `opengpt4-0.1.5/opengpt/models/completion/chatbase/model.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.4/opengpt/models/completion/chatgptproxy/DOC.md` & `opengpt4-0.1.5/opengpt/models/completion/chatgptproxy/DOC.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.4/opengpt/models/completion/chatgptproxy/README.md` & `opengpt4-0.1.5/opengpt/models/completion/chatgptproxy/README.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.4/opengpt/models/completion/chatgptproxy/model.py` & `opengpt4-0.1.5/opengpt/models/completion/chatgptproxy/model.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.4/opengpt/models/completion/chatllama/DOC.md` & `opengpt4-0.1.5/opengpt/models/completion/chatllama/DOC.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.4/opengpt/models/completion/chatllama/model.py` & `opengpt4-0.1.5/opengpt/models/completion/chatllama/model.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.4/opengpt/models/completion/forefront/DOC.md` & `opengpt4-0.1.5/opengpt/models/completion/forefront/DOC.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.4/opengpt/models/completion/forefront/README.md` & `opengpt4-0.1.5/opengpt/models/completion/forefront/README.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.4/opengpt/models/completion/forefront/attributes/conversation.py` & `opengpt4-0.1.5/opengpt/models/completion/forefront/attributes/conversation.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.4/opengpt/models/completion/forefront/model.py` & `opengpt4-0.1.5/opengpt/models/completion/forefront/model.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.4/opengpt/models/completion/forefront/tools/system/email_creation.py` & `opengpt4-0.1.5/opengpt/models/completion/forefront/tools/system/email_creation.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.4/opengpt/models/completion/forefront/tools/system/signature.py` & `opengpt4-0.1.5/opengpt/models/completion/forefront/tools/system/signature.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.4/opengpt/models/completion/italygpt/DOC.md` & `opengpt4-0.1.5/opengpt/models/completion/italygpt/DOC.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.4/opengpt/models/completion/italygpt/model.py` & `opengpt4-0.1.5/opengpt/models/completion/italygpt/model.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.4/opengpt/models/completion/usesless/DOC.md` & `opengpt4-0.1.5/opengpt/models/completion/usesless/DOC.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.4/opengpt/models/completion/usesless/README.md` & `opengpt4-0.1.5/opengpt/models/completion/usesless/README.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.4/opengpt/models/completion/usesless/model.py` & `opengpt4-0.1.5/opengpt/models/completion/usesless/model.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.4/opengpt/models/image/hotpot/model.py` & `opengpt4-0.1.5/opengpt/models/image/hotpot/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from .tools.system.id import UniqueID
 from .tools.typing.response import ModelResponse
 from libraries.colorama import init, Fore, Style
 import yaml
 import requests
 import fake_useragent
 import logging
+import os
 
 init()
 
 class OpenGPTError(Exception):
 	@staticmethod
 	def Print(context: Text, warn: Optional[bool] = False) -> None:
 		if warn:
@@ -19,14 +20,15 @@
 			sys.exit(1)
 
 class Model:
 	@classmethod
 	def __init__(self: type, style: Optional[Text] = "Hotpot Art 9") -> None:
 		self._SETUP_LOGGER()
 		self.__LoadStyles()
+		self.__DIR: Text = os.getcwd()
 		self.__session: requests.Session = requests.Session()
 		self.__UNIQUE_ID: str = UniqueID(16)
 		self.STYLE: Text = style
 		self.__STYLE_ID = self.__GetStyleID(self.STYLE)
 		self.__HEADERS: Dict[str, str] = {
 			"Accept": "*/*",
 			"Accept-Language": "pt-BR,pt;q=0.9,en-US;q=0.8,en;q=0.7",
@@ -67,15 +69,15 @@
 	@classmethod
 	def UpdateStyle(self: type, style: Text) -> None:
 		self.STYLE = style
 		self.__STYLE_ID = self.__GetStyleID(self.STYLE)
 
 	@classmethod
 	def __LoadStyles(self: type) -> None:
-		self.__DATA: Dict[Text, Text] = yaml.safe_load(open("opengpt/models/image/hotpot/styles.yml").read())
+		self.__DATA: Dict[Text, Text] = yaml.safe_load(open(self.__DIR + "/styles.yml").read())
 
 	@classmethod
 	def __Fields(self: type, *args: Tuple[int, str], **kwargs: Dict[str, Any]) -> Text:
 		return kwargs
 
 	@classmethod
 	def __AddField(self: type, field: Text, value: Any, end: Optional[bool] = False) -> Text:
@@ -107,8 +109,8 @@
 		url: Text = self.__session.post("https://api.hotpot.ai/art-premium-test1", headers=self.__HEADERS, data=__FORM_DATA).content
 		return ModelResponse(**{
 			"id": __DATA["requestId"],
 			"url": url.decode().replace("\"", ""),
 			"style": self.STYLE,
 			"width": __DATA["width"],
 			"height": __DATA["height"]
-		})
+		})
```

### Comparing `opengpt4-0.1.4/opengpt/models/image/hotpot/styles.yml` & `opengpt4-0.1.5/opengpt/models/image/hotpot/styles.yml`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.4/PKG-INFO` & `opengpt4-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengpt4
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 License: GPL-3.0
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

