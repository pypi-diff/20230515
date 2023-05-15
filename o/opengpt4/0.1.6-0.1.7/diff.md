# Comparing `tmp/opengpt4-0.1.6.tar.gz` & `tmp/opengpt4-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opengpt4-0.1.6.tar", max compression
+gzip compressed data, was "opengpt4-0.1.7.tar", max compression
```

## Comparing `opengpt4-0.1.6.tar` & `opengpt4-0.1.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    35149 2023-05-14 23:27:03.736924 opengpt4-0.1.6/LICENSE
--rw-r--r--   0        0        0     4740 2023-05-14 23:27:03.740924 opengpt4-0.1.6/README.md
--rw-r--r--   0        0        0      270 2023-05-14 23:27:03.740924 opengpt4-0.1.6/libraries/colorama/__init__.py
--rw-r--r--   0        0        0     2522 2023-05-14 23:27:03.740924 opengpt4-0.1.6/libraries/colorama/ansi.py
--rw-r--r--   0        0        0    11128 2023-05-14 23:27:03.740924 opengpt4-0.1.6/libraries/colorama/ansitowin32.py
--rw-r--r--   0        0        0     3325 2023-05-14 23:27:03.740924 opengpt4-0.1.6/libraries/colorama/initialise.py
--rw-r--r--   0        0        0     6181 2023-05-14 23:27:03.740924 opengpt4-0.1.6/libraries/colorama/win32.py
--rw-r--r--   0        0        0     7168 2023-05-14 23:27:03.740924 opengpt4-0.1.6/libraries/colorama/winterm.py
--rw-r--r--   0        0        0     1691 2023-05-14 23:27:03.740924 opengpt4-0.1.6/libraries/tempmail.py
--rw-r--r--   0        0        0     1097 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/README.md
--rw-r--r--   0        0        0     3408 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/__init__.py
--rw-r--r--   0        0        0      206 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/config.yml
--rw-r--r--   0        0        0      866 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/chatbase/DOC.md
--rw-r--r--   0        0        0      489 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/chatbase/README.md
--rw-r--r--   0        0        0     5320 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/chatbase/model.py
--rw-r--r--   0        0        0      649 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/chatgptproxy/DOC.md
--rw-r--r--   0        0        0      525 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/chatgptproxy/README.md
--rw-r--r--   0        0        0     2406 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/chatgptproxy/model.py
--rw-r--r--   0        0        0      624 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/chatllama/DOC.md
--rw-r--r--   0        0        0      459 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/chatllama/README.md
--rw-r--r--   0        0        0     1150 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/chatllama/model.py
--rw-r--r--   0        0        0     6698 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/forefront/DOC.md
--rw-r--r--   0        0        0     6460 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/forefront/README.md
--rw-r--r--   0        0        0     3788 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/forefront/attributes/conversation.py
--rw-r--r--   0        0        0     7505 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/forefront/model.py
--rw-r--r--   0        0        0     5818 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/forefront/tools/system/email_creation.py
--rw-r--r--   0        0        0      657 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/forefront/tools/system/signature.py
--rw-r--r--   0        0        0      446 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/forefront/tools/typing/response.py
--rw-r--r--   0        0        0      842 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/italygpt/DOC.md
--rw-r--r--   0        0        0      321 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/italygpt/README.md
--rw-r--r--   0        0        0     1495 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/italygpt/model.py
--rw-r--r--   0        0        0     1208 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/usesless/DOC.md
--rw-r--r--   0        0        0      769 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/usesless/README.md
--rw-r--r--   0        0        0     1577 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/usesless/model.py
--rw-r--r--   0        0        0      418 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/completion/usesless/tools/typing/response.py
--rw-r--r--   0        0        0     4140 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/image/hotpot/model.py
--rw-r--r--   0        0        0     3012 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/image/hotpot/styles.yml
--rw-r--r--   0        0        0      232 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/image/hotpot/tools/system/id.py
--rw-r--r--   0        0        0      147 2023-05-14 23:27:03.740924 opengpt4-0.1.6/opengpt/models/image/hotpot/tools/typing/response.py
--rw-r--r--   0        0        0      414 2023-05-14 23:27:03.740924 opengpt4-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     5459 1970-01-01 00:00:00.000000 opengpt4-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-15 16:33:50.837635 opengpt4-0.1.7/LICENSE
+-rw-r--r--   0        0        0     4892 2023-05-15 16:33:50.837635 opengpt4-0.1.7/README.md
+-rw-r--r--   0        0        0     1097 2023-05-15 16:33:50.837635 opengpt4-0.1.7/opengpt/README.md
+-rw-r--r--   0        0        0     3440 2023-05-15 16:33:50.837635 opengpt4-0.1.7/opengpt/__init__.py
+-rw-r--r--   0        0        0      206 2023-05-15 16:33:50.837635 opengpt4-0.1.7/opengpt/config.yml
+-rw-r--r--   0        0        0      270 2023-05-15 16:33:50.837635 opengpt4-0.1.7/opengpt/libraries/colorama/__init__.py
+-rw-r--r--   0        0        0     2522 2023-05-15 16:33:50.837635 opengpt4-0.1.7/opengpt/libraries/colorama/ansi.py
+-rw-r--r--   0        0        0    11128 2023-05-15 16:33:50.837635 opengpt4-0.1.7/opengpt/libraries/colorama/ansitowin32.py
+-rw-r--r--   0        0        0     3325 2023-05-15 16:33:50.837635 opengpt4-0.1.7/opengpt/libraries/colorama/initialise.py
+-rw-r--r--   0        0        0     6181 2023-05-15 16:33:50.837635 opengpt4-0.1.7/opengpt/libraries/colorama/win32.py
+-rw-r--r--   0        0        0     7168 2023-05-15 16:33:50.837635 opengpt4-0.1.7/opengpt/libraries/colorama/winterm.py
+-rw-r--r--   0        0        0     1691 2023-05-15 16:33:50.837635 opengpt4-0.1.7/opengpt/libraries/tempmail.py
+-rw-r--r--   0        0        0      866 2023-05-15 16:33:50.837635 opengpt4-0.1.7/opengpt/models/completion/chatbase/DOC.md
+-rw-r--r--   0        0        0      489 2023-05-15 16:33:50.837635 opengpt4-0.1.7/opengpt/models/completion/chatbase/README.md
+-rw-r--r--   0        0        0     5320 2023-05-15 16:33:50.837635 opengpt4-0.1.7/opengpt/models/completion/chatbase/model.py
+-rw-r--r--   0        0        0      649 2023-05-15 16:33:50.837635 opengpt4-0.1.7/opengpt/models/completion/chatgptproxy/DOC.md
+-rw-r--r--   0        0        0      525 2023-05-15 16:33:50.837635 opengpt4-0.1.7/opengpt/models/completion/chatgptproxy/README.md
+-rw-r--r--   0        0        0     2406 2023-05-15 16:33:50.837635 opengpt4-0.1.7/opengpt/models/completion/chatgptproxy/model.py
+-rw-r--r--   0        0        0      624 2023-05-15 16:33:50.837635 opengpt4-0.1.7/opengpt/models/completion/chatllama/DOC.md
+-rw-r--r--   0        0        0      459 2023-05-15 16:33:50.837635 opengpt4-0.1.7/opengpt/models/completion/chatllama/README.md
+-rw-r--r--   0        0        0     1150 2023-05-15 16:33:50.837635 opengpt4-0.1.7/opengpt/models/completion/chatllama/model.py
+-rw-r--r--   0        0        0     6698 2023-05-15 16:33:50.837635 opengpt4-0.1.7/opengpt/models/completion/forefront/DOC.md
+-rw-r--r--   0        0        0     6460 2023-05-15 16:33:50.837635 opengpt4-0.1.7/opengpt/models/completion/forefront/README.md
+-rw-r--r--   0        0        0     3788 2023-05-15 16:33:50.837635 opengpt4-0.1.7/opengpt/models/completion/forefront/attributes/conversation.py
+-rw-r--r--   0        0        0     7505 2023-05-15 16:33:50.837635 opengpt4-0.1.7/opengpt/models/completion/forefront/model.py
+-rw-r--r--   0        0        0     5818 2023-05-15 16:33:50.837635 opengpt4-0.1.7/opengpt/models/completion/forefront/tools/system/email_creation.py
+-rw-r--r--   0        0        0      657 2023-05-15 16:33:50.837635 opengpt4-0.1.7/opengpt/models/completion/forefront/tools/system/signature.py
+-rw-r--r--   0        0        0      446 2023-05-15 16:33:50.837635 opengpt4-0.1.7/opengpt/models/completion/forefront/tools/typing/response.py
+-rw-r--r--   0        0        0      842 2023-05-15 16:33:50.837635 opengpt4-0.1.7/opengpt/models/completion/italygpt/DOC.md
+-rw-r--r--   0        0        0      321 2023-05-15 16:33:50.837635 opengpt4-0.1.7/opengpt/models/completion/italygpt/README.md
+-rw-r--r--   0        0        0     1495 2023-05-15 16:33:50.837635 opengpt4-0.1.7/opengpt/models/completion/italygpt/model.py
+-rw-r--r--   0        0        0     1208 2023-05-15 16:33:50.837635 opengpt4-0.1.7/opengpt/models/completion/usesless/DOC.md
+-rw-r--r--   0        0        0      769 2023-05-15 16:33:50.837635 opengpt4-0.1.7/opengpt/models/completion/usesless/README.md
+-rw-r--r--   0        0        0     1577 2023-05-15 16:33:50.837635 opengpt4-0.1.7/opengpt/models/completion/usesless/model.py
+-rw-r--r--   0        0        0      418 2023-05-15 16:33:50.837635 opengpt4-0.1.7/opengpt/models/completion/usesless/tools/typing/response.py
+-rw-r--r--   0        0        0     4180 2023-05-15 16:33:50.837635 opengpt4-0.1.7/opengpt/models/image/hotpot/model.py
+-rw-r--r--   0        0        0     3012 2023-05-15 16:33:50.837635 opengpt4-0.1.7/opengpt/models/image/hotpot/styles.yml
+-rw-r--r--   0        0        0      232 2023-05-15 16:33:50.841635 opengpt4-0.1.7/opengpt/models/image/hotpot/tools/system/id.py
+-rw-r--r--   0        0        0      147 2023-05-15 16:33:50.841635 opengpt4-0.1.7/opengpt/models/image/hotpot/tools/typing/response.py
+-rw-r--r--   0        0        0      388 2023-05-15 16:33:50.841635 opengpt4-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     5611 1970-01-01 00:00:00.000000 opengpt4-0.1.7/PKG-INFO
```

### Comparing `opengpt4-0.1.6/LICENSE` & `opengpt4-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.6/README.md` & `opengpt4-0.1.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -79,16 +79,17 @@
 ```
 
 #### Package
 
 You can install this project as module using pip command.
 
 ```shell
-pip install opengpt4
+pip install opengpt4==0.1.1
 ```
+> It's recommend to use 0.1.1 version for now, the latest version is with bugs. If you want to use the latest version just download source code.
 
 After install, for use it's simple, you can work with something model like this:
 
 ```py
 from opengpt.forefront.model import Model
 
 # .....
```

### Comparing `opengpt4-0.1.6/libraries/colorama/ansi.py` & `opengpt4-0.1.7/opengpt/libraries/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.6/libraries/colorama/ansitowin32.py` & `opengpt4-0.1.7/opengpt/libraries/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.6/libraries/colorama/initialise.py` & `opengpt4-0.1.7/opengpt/libraries/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.6/libraries/colorama/win32.py` & `opengpt4-0.1.7/opengpt/libraries/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.6/libraries/colorama/winterm.py` & `opengpt4-0.1.7/opengpt/libraries/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.6/libraries/tempmail.py` & `opengpt4-0.1.7/opengpt/libraries/tempmail.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.6/opengpt/README.md` & `opengpt4-0.1.7/opengpt/README.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.6/opengpt/__init__.py` & `opengpt4-0.1.7/opengpt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Optional, Union, Dict, List, Text
-from libraries.colorama import init, Fore, Style
+from .libraries.colorama import init, Fore, Style
 import importlib
 import yaml
 import sys
 import inspect
 import os
 
 init()
@@ -16,25 +16,22 @@
 		else:
 			print(Fore.RED + "Error: " + context + Style.RESET_ALL)
 			sys.exit(1)
 
 class OpenGPT:
 	@classmethod
 	def __init__(self: type, provider: Text, type: Optional[Text] = "completion", options: Optional[Union[Dict[Text, Text], None]] = None) -> None:
-	
-		self.__DIR: Text = os.getcwd()	
+		self.__DIR: Text = os.path.dirname(os.path.abspath(__file__))
 		self.__LoadModels()
 		self.__TYPE: Text = type
 		self.__OPTIONS: Union[Dict[Text, Text], None] = options
 		self.__PROVIDER: Text = provider
-
 		self.__Verifications()
 		self.__MODULE: module = importlib.import_module(f"opengpt.models.{self.__TYPE}.{self.__PROVIDER}.model")
 		self.__MODEL_CLASS: type = getattr(self.__MODULE, "Model")
-
 		self.__model: type = None
 		self.__InitializeModelClass()
 
 	@classmethod
 	def __InitializeModelClass(self: type) -> None:
 		if not self.__OPTIONS is None:
 			args: List[Text] = inspect.signature(self.__MODEL_CLASS.__init__)
@@ -54,15 +51,15 @@
 
 			self.__model = self.__MODEL_CLASS(**self.__OPTIONS)
 		else:
 			self.__model = self.__MODEL_CLASS()
 
 	@classmethod
 	def __LoadModels(self: type) -> None:
-		self.__DATA: Dict[Text, Text] = yaml.safe_load(open(self.__DIR + "/config.yml").read())
+		self.__DATA: Dict[Text, Text] = yaml.safe_load(open(self.__DIR + "/config.yml", "r").read())
 
 	@classmethod
 	def __Verifications(self: type) -> None:
 		exists: bool = False
 
 		if self.__TYPE not in self.__DATA["models"]:
 			OpenGPTError.Print(f"The type \"{self.__TYPE}\" not be founded. Try: {', '.join(self.__DATA['models'])}")
```

### Comparing `opengpt4-0.1.6/opengpt/models/completion/chatbase/DOC.md` & `opengpt4-0.1.7/opengpt/models/completion/chatbase/DOC.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.6/opengpt/models/completion/chatbase/model.py` & `opengpt4-0.1.7/opengpt/models/completion/chatbase/model.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.6/opengpt/models/completion/chatgptproxy/DOC.md` & `opengpt4-0.1.7/opengpt/models/completion/chatgptproxy/DOC.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.6/opengpt/models/completion/chatgptproxy/README.md` & `opengpt4-0.1.7/opengpt/models/completion/chatgptproxy/README.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.6/opengpt/models/completion/chatgptproxy/model.py` & `opengpt4-0.1.7/opengpt/models/completion/chatgptproxy/model.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.6/opengpt/models/completion/chatllama/DOC.md` & `opengpt4-0.1.7/opengpt/models/completion/chatllama/DOC.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.6/opengpt/models/completion/chatllama/model.py` & `opengpt4-0.1.7/opengpt/models/completion/chatllama/model.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.6/opengpt/models/completion/forefront/DOC.md` & `opengpt4-0.1.7/opengpt/models/completion/forefront/DOC.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.6/opengpt/models/completion/forefront/README.md` & `opengpt4-0.1.7/opengpt/models/completion/forefront/README.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.6/opengpt/models/completion/forefront/attributes/conversation.py` & `opengpt4-0.1.7/opengpt/models/completion/forefront/attributes/conversation.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.6/opengpt/models/completion/forefront/model.py` & `opengpt4-0.1.7/opengpt/models/completion/forefront/model.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.6/opengpt/models/completion/forefront/tools/system/email_creation.py` & `opengpt4-0.1.7/opengpt/models/completion/forefront/tools/system/email_creation.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.6/opengpt/models/completion/forefront/tools/system/signature.py` & `opengpt4-0.1.7/opengpt/models/completion/forefront/tools/system/signature.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.6/opengpt/models/completion/italygpt/DOC.md` & `opengpt4-0.1.7/opengpt/models/completion/italygpt/DOC.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.6/opengpt/models/completion/italygpt/model.py` & `opengpt4-0.1.7/opengpt/models/completion/italygpt/model.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.6/opengpt/models/completion/usesless/DOC.md` & `opengpt4-0.1.7/opengpt/models/completion/usesless/DOC.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.6/opengpt/models/completion/usesless/README.md` & `opengpt4-0.1.7/opengpt/models/completion/usesless/README.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.6/opengpt/models/completion/usesless/model.py` & `opengpt4-0.1.7/opengpt/models/completion/usesless/model.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.6/opengpt/models/image/hotpot/model.py` & `opengpt4-0.1.7/opengpt/models/image/hotpot/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, Text, Optional, Generator, Any, Tuple
 from .tools.system.id import UniqueID
 from .tools.typing.response import ModelResponse
-from libraries.colorama import init, Fore, Style
+from ....libraries.colorama import init, Fore, Style
 import yaml
 import requests
 import fake_useragent
 import logging
 import os
 
 init()
@@ -19,16 +19,16 @@
 			print(Fore.RED + "Error: " + context + Style.RESET_ALL)
 			sys.exit(1)
 
 class Model:
 	@classmethod
 	def __init__(self: type, style: Optional[Text] = "Hotpot Art 9") -> None:
 		self._SETUP_LOGGER()
+		self.__DIR: Text = os.path.dirname(os.path.abspath(__file__))
 		self.__LoadStyles()
-		self.__DIR: Text = os.getcwd()
 		self.__session: requests.Session = requests.Session()
 		self.__UNIQUE_ID: str = UniqueID(16)
 		self.STYLE: Text = style
 		self.__STYLE_ID = self.__GetStyleID(self.STYLE)
 		self.__HEADERS: Dict[str, str] = {
 			"Accept": "*/*",
 			"Accept-Language": "pt-BR,pt;q=0.9,en-US;q=0.8,en;q=0.7",
@@ -69,15 +69,15 @@
 	@classmethod
 	def UpdateStyle(self: type, style: Text) -> None:
 		self.STYLE = style
 		self.__STYLE_ID = self.__GetStyleID(self.STYLE)
 
 	@classmethod
 	def __LoadStyles(self: type) -> None:
-		self.__DATA: Dict[Text, Text] = yaml.safe_load(open(self.__DIR + "/styles.yml").read())
+		self.__DATA: Dict[Text, Text] = yaml.safe_load(open(self.__DIR + "/styles.yml", "r").read())
 
 	@classmethod
 	def __Fields(self: type, *args: Tuple[int, str], **kwargs: Dict[str, Any]) -> Text:
 		return kwargs
 
 	@classmethod
 	def __AddField(self: type, field: Text, value: Any, end: Optional[bool] = False) -> Text:
```

### Comparing `opengpt4-0.1.6/opengpt/models/image/hotpot/styles.yml` & `opengpt4-0.1.7/opengpt/models/image/hotpot/styles.yml`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.6/PKG-INFO` & `opengpt4-0.1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengpt4
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 License: GPL-3.0
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -99,16 +99,17 @@
 ```
 
 #### Package
 
 You can install this project as module using pip command.
 
 ```shell
-pip install opengpt4
+pip install opengpt4==0.1.1
 ```
+> It's recommend to use 0.1.1 version for now, the latest version is with bugs. If you want to use the latest version just download source code.
 
 After install, for use it's simple, you can work with something model like this:
 
 ```py
 from opengpt.forefront.model import Model
 
 # .....
```

