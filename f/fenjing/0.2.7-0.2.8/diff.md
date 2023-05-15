# Comparing `tmp/fenjing-0.2.7.tar.gz` & `tmp/fenjing-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenjing-0.2.7.tar", last modified: Mon May 15 11:37:02 2023, max compression
+gzip compressed data, was "fenjing-0.2.8.tar", last modified: Mon May 15 11:55:20 2023, max compression
```

## Comparing `fenjing-0.2.7.tar` & `fenjing-0.2.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:37:02.323589 fenjing-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-15 11:36:51.000000 fenjing-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-15 11:36:51.000000 fenjing-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-15 11:37:02.323589 fenjing-0.2.7/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     5621 2023-05-15 11:36:51.000000 fenjing-0.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 11:36:51.000000 fenjing-0.2.7/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:37:02.323589 fenjing-0.2.7/fenjing/
--rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-05-15 11:36:51.000000 fenjing-0.2.7/fenjing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-15 11:36:51.000000 fenjing-0.2.7/fenjing/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-05-15 11:36:51.000000 fenjing-0.2.7/fenjing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-15 11:36:51.000000 fenjing-0.2.7/fenjing/colorize.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-15 11:36:51.000000 fenjing-0.2.7/fenjing/config_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-15 11:36:51.000000 fenjing-0.2.7/fenjing/const.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-05-15 11:36:51.000000 fenjing-0.2.7/fenjing/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-15 11:36:51.000000 fenjing-0.2.7/fenjing/form.py
--rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-05-15 11:36:51.000000 fenjing-0.2.7/fenjing/form_cracker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3474 2023-05-15 11:36:51.000000 fenjing-0.2.7/fenjing/full_payload_gen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2846 2023-05-15 11:36:51.000000 fenjing-0.2.7/fenjing/int_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    28509 2023-05-15 11:36:51.000000 fenjing-0.2.7/fenjing/payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-15 11:36:51.000000 fenjing-0.2.7/fenjing/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-15 11:36:51.000000 fenjing-0.2.7/fenjing/scan_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-15 11:36:51.000000 fenjing-0.2.7/fenjing/shell_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-15 11:36:51.000000 fenjing-0.2.7/fenjing/waf_func_gen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:37:02.323589 fenjing-0.2.7/fenjing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-15 11:37:02.000000 fenjing-0.2.7/fenjing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-15 11:37:02.000000 fenjing-0.2.7/fenjing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 11:37:02.000000 fenjing-0.2.7/fenjing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-15 11:37:02.000000 fenjing-0.2.7/fenjing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 11:37:02.000000 fenjing-0.2.7/fenjing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-15 11:36:51.000000 fenjing-0.2.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 11:37:02.323589 fenjing-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-15 11:36:51.000000 fenjing-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:55:20.383300 fenjing-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-15 11:55:09.000000 fenjing-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-15 11:55:09.000000 fenjing-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-15 11:55:20.379300 fenjing-0.2.8/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5621 2023-05-15 11:55:09.000000 fenjing-0.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 11:55:09.000000 fenjing-0.2.8/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:55:20.379300 fenjing-0.2.8/fenjing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-05-15 11:55:09.000000 fenjing-0.2.8/fenjing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-15 11:55:09.000000 fenjing-0.2.8/fenjing/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-05-15 11:55:09.000000 fenjing-0.2.8/fenjing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-15 11:55:09.000000 fenjing-0.2.8/fenjing/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-15 11:55:09.000000 fenjing-0.2.8/fenjing/config_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-15 11:55:09.000000 fenjing-0.2.8/fenjing/const.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-05-15 11:55:09.000000 fenjing-0.2.8/fenjing/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-15 11:55:09.000000 fenjing-0.2.8/fenjing/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-05-15 11:55:09.000000 fenjing-0.2.8/fenjing/form_cracker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3493 2023-05-15 11:55:09.000000 fenjing-0.2.8/fenjing/full_payload_gen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2846 2023-05-15 11:55:09.000000 fenjing-0.2.8/fenjing/int_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28558 2023-05-15 11:55:09.000000 fenjing-0.2.8/fenjing/payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-15 11:55:09.000000 fenjing-0.2.8/fenjing/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-15 11:55:09.000000 fenjing-0.2.8/fenjing/scan_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-15 11:55:09.000000 fenjing-0.2.8/fenjing/shell_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-15 11:55:09.000000 fenjing-0.2.8/fenjing/waf_func_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:55:20.379300 fenjing-0.2.8/fenjing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-15 11:55:20.000000 fenjing-0.2.8/fenjing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-15 11:55:20.000000 fenjing-0.2.8/fenjing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 11:55:20.000000 fenjing-0.2.8/fenjing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-15 11:55:20.000000 fenjing-0.2.8/fenjing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 11:55:20.000000 fenjing-0.2.8/fenjing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-15 11:55:09.000000 fenjing-0.2.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 11:55:20.383300 fenjing-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-15 11:55:09.000000 fenjing-0.2.8/setup.py
```

### Comparing `fenjing-0.2.7/LICENSE` & `fenjing-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.7/PKG-INFO` & `fenjing-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.2.7
+Version: 0.2.8
 Summary: A Jinja2 SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.2.7/README.md` & `fenjing-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.7/fenjing/cli.py` & `fenjing-0.2.8/fenjing/cli.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.7/fenjing/colorize.py` & `fenjing-0.2.8/fenjing/colorize.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.7/fenjing/config_payload.py` & `fenjing-0.2.8/fenjing/config_payload.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import Callable, Tuple, Dict
+from typing import Callable, Tuple, Dict, Union
 from .const import CONFIG
 from .full_payload_gen import FullPayloadGen
 
 full_payload_store: Dict[int, FullPayloadGen] = {}
 
-def config_payload(waf_func: Callable[[str, ], bool]) -> str | None:
+def config_payload(waf_func: Callable[[str, ], bool]) -> Union[str, None]:
     """根据提供的waf函数生成读取config的payload
 
     Args:
         waf_func (Callable[[str, ], bool]): waf函数，判断提供的payload能否通过waf, 能则返回True
 
     Returns:
         str|None: payload
```

### Comparing `fenjing-0.2.7/fenjing/const.py` & `fenjing-0.2.8/fenjing/const.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.7/fenjing/form.py` & `fenjing-0.2.8/fenjing/form.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from urllib.parse import urlparse, urlunparse
 from typing import Iterable
 import random
 import logging
 import string
-from typing import Dict, Any, List
+from typing import Dict, Any, List, Union
 
 from bs4 import BeautifulSoup
 
 logger = logging.getLogger("utils.form")
 
 
 def Form(*, action: str, inputs: Iterable, method: str = "POST") -> Dict[str, Any]:
@@ -28,20 +28,20 @@
     return {
         "action": action,
         "method": method,
         "inputs": set(inputs)
     }
 
 
-def parse_forms(url, html: str | BeautifulSoup) -> List[dict]:
+def parse_forms(url, html: Union[str, BeautifulSoup]) -> List[dict]:
     """从html中解析出对应的表单
 
     Args:
         url (str): HTML对应的URL
-        html (str | BeautifulSoup): HTML
+        html (Union[str, BeautifulSoup]): HTML
 
     Returns:
         List[dict]: 所有表单
     """
     parsed_url = urlparse(url)
     uri = parsed_url.path
```

### Comparing `fenjing-0.2.7/fenjing/form_cracker.py` & `fenjing-0.2.8/fenjing/form_cracker.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from collections import namedtuple
 import logging
-from typing import List, Dict, Any
+from typing import List, Dict, Any, Union
 
 from .form import random_fill, fill_form
 from .requester import Requester
 from .colorize import colored
 from .const import OS_POPEN_READ
 from .waf_func_gen import WafFuncGen
 from .full_payload_gen import FullPayloadGen
@@ -78,22 +78,22 @@
         all_length = sum(len(v) for v in inputs.values())
         if all_length > 2048 and self.form["method"] == "GET":
             logger.warning(
                 f"inputs are extremely long (len={all_length}) that the request might fail")
         return self.req.request(
             **fill_form(self.url, self.form, inputs))
 
-    def crack_inputs(self, input_field: str) -> Result | None:
+    def crack_inputs(self, input_field: str) -> Union[Result, None]:
         """攻击对应的input
 
         Args:
             input_field (str): 需要攻击的input
 
         Returns:
-            Result | None: 对应的payload生成函数，以及对应的input
+            Union[Result, None]: 对应的payload生成函数，以及对应的input
         """
         logger.info(f"Testing {colored('yellow', input_field)}")
 
         waf_func = self.waf_func_gen.generate(input_field)
         full_payload_gen = FullPayloadGen(waf_func)
         payload, will_echo = full_payload_gen.generate(OS_POPEN_READ, self.test_cmd)
         # payload, will_echo = exec_cmd_payload(waf_func, self.test_cmd)
@@ -119,19 +119,19 @@
                 f"Input {input_field} looks great, but we WON'T SEE the execution result! " +
                 "You can try generating payloads anyway.")
             return Result(
                 full_payload_gen=full_payload_gen,
                 input_field=input_field
             )
 
-    def crack(self) -> Result | None:
+    def crack(self) -> Union[Result, None]:
         """攻击表单
 
         Returns:
-            Result | None: 对应的payload生成函数，以及对应的input
+            Union[Result, None]: 对应的payload生成函数，以及对应的input
         """
         logger.info(f"Start cracking {self.form}")
         vulunables = self.vulunable_inputs()
         logger.info(
             f"These inputs might be vulunable: {colored('yellow', repr(vulunables))}")
 
         for input_field in vulunables:
@@ -155,17 +155,17 @@
 #     test_result = "f3n j1ng"
 
 #     def __init__(
 #             self,
 #             form: Dict[str, Any],
 #             method: str = "POST",
 #             inputs: List[str] | None = None,
-#             url: str | None = None,
-#             action: str | None = None,
-#             requester: Requester | None = None,
+#             url: Union[str, None] = None,
+#             action: Union[str, None] = None,
+#             requester: Union[Requester, None] = None,
 #             request_interval: float = 0.0
 #     ):
 #         """生成用于攻击form的类
 
 #         Args:
 #             form (dict): 解析后的form元素
 #             method (str, optional): form的提交方法. Defaults to "POST".
@@ -247,22 +247,22 @@
 #         # }
 #         hashes = [
 #             hash(r.text) for keyword, r in resps.items()
 #             if r is not None and r.status_code != 500 and keyword not in r.text
 #         ]
 #         return [pair[0] for pair in Counter(hashes).most_common(2)]
 
-#     def crack_inputs(self, input_field: str) -> Result | None:
+#     def crack_inputs(self, input_field: str) -> Union[Result, None]:
 #         """攻击对应的input
 
 #         Args:
 #             input_field (str): 需要攻击的input
 
 #         Returns:
-#             Result | None: 对应的payload生成函数，以及对应的input
+#             Union[Result, None]: 对应的payload生成函数，以及对应的input
 #         """
 #         logger.info(f"Testing {colored('yellow', input_field)}")
 
 #         waf_hashes = self.waf_page_hash(input_field)
 
 #         @lru_cache(1000)
 #         def waf_func(value):
@@ -295,19 +295,19 @@
 #                 "You can try generating payloads anyway.")
 #             return Result(
 #                 payload_generate_func=(
 #                     lambda cmd: exec_cmd_payload(waf_func, cmd)[0]),
 #                 input_field=input_field
 #             )
 
-#     def crack(self) -> Result | None:
+#     def crack(self) -> Union[Result, None]:
 #         """攻击表单
 
 #         Returns:
-#             Result | None: 对应的payload生成函数，以及对应的input
+#             Union[Result, None]: 对应的payload生成函数，以及对应的input
 #         """
 #         logger.info(f"Start cracking {self.form}")
 #         vulunables = self.vulunable_inputs()
 #         logger.info(
 #             f"These inputs might be vulunable: {colored('yellow', repr(vulunables))}")
 
 #         for input_field in vulunables:
```

### Comparing `fenjing-0.2.7/fenjing/full_payload_gen.py` & `fenjing-0.2.8/fenjing/full_payload_gen.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Callable, List, Tuple
+from typing import Callable, List, Tuple, Union
 import logging
 
 from . import payload_gen
 from .int_vars import get_useable_int_vars
 from .colorize import colored
 
 logger = logging.getLogger("shell_payload")
@@ -68,15 +68,15 @@
                 f"use {colored('blue', self.outer_pattern)}, which {colored('red', 'will not print')} your result!")
 
         self.payload_gen = payload_gen.PayloadGenerator(self.waf_func, self.context)
 
         self.prepared = True
         return True
 
-    def generate(self, gen_type, *args) -> Tuple[str | None, bool | None]:
+    def generate(self, gen_type, *args) -> Tuple[Union[str, None], Union[bool, None]]:
 
         if not self.prepared and not self.do_prepare():
             return None, None
 
         # inner_payload = payload_gen.generate(
         #     gen_type,
         #     *args,
```

### Comparing `fenjing-0.2.7/fenjing/int_vars.py` & `fenjing-0.2.8/fenjing/int_vars.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.7/fenjing/payload_gen.py` & `fenjing-0.2.8/fenjing/payload_gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections import defaultdict
-from typing import Callable, DefaultDict, List, Dict
+from typing import Callable, DefaultDict, List, Dict, Union
 import re
 import time
 import logging
 from .colorize import colored
 from .const import *
 
 req_gens: DefaultDict[str, List[Callable]] = defaultdict(list)
@@ -16,15 +16,15 @@
     if not gen_type:
         raise Exception(
             f"Error found when register payload generator {f.__name__}")
     req_gens[gen_type.group(1)].append(f)
 
 
 class PayloadGenerator:
-    def __init__(self, waf_func: Callable, context: Dict | None):
+    def __init__(self, waf_func: Callable, context: Union[Dict, None]):
         self.waf_func = waf_func
         self.context = context
         self.cache = {}
         self.generate_funcs = {
             LITERAL: self.literal_generate,
             UNSATISFIED: self.unsatisfied_generate
         }
@@ -122,19 +122,19 @@
         return None
 
     def generate(self, gen_type, *args):
         generate_func = self.generate_funcs[gen_type] if gen_type in self.generate_funcs else self.default_generate
         return generate_func(gen_type, *args)
 
 
-def generate(gen_type, *args, waf_func: Callable, context: dict | None = None) -> str | None:
+def generate(gen_type, *args, waf_func: Callable, context: Union[dict, None] = None) -> Union[str, None]:
     payload_generator = PayloadGenerator(waf_func, context)
     return payload_generator.generate(gen_type, *args)
 
-# def generate(gen_type, *args, waf_func: Callable | None = None, context: dict | None = None, cache: dict | None = None) -> str | None:
+# def generate(gen_type, *args, waf_func: Union[Callable, None] = None, context: Union[dict, None] = None, cache: Union[dict, None] = None) -> Union[str, None]:
 
 #     if waf_func is None:
 #         raise Exception("waf_func cannot be None")
 #     if context is None:
 #         context = {}
 #     if cache is None:
 #         cache = {}
```

### Comparing `fenjing-0.2.7/fenjing/requester.py` & `fenjing-0.2.8/fenjing/requester.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.7/fenjing/scan_url.py` & `fenjing-0.2.8/fenjing/scan_url.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import logging
-
+from typing import Union
 from .requester import Requester
 from .form import parse_forms
 
 from bs4 import BeautifulSoup
 
 logger = logging.getLogger("scan_url")
 
 
-def parse_urls(html: str | BeautifulSoup) -> list:
+def parse_urls(html: Union[str, BeautifulSoup]) -> list:
     """从html中解析出所有的链接
 
     Args:
         html (str|BeautifulSoup): HTML
 
     Returns:
         List[str]: 所有链接
```

### Comparing `fenjing-0.2.7/fenjing/shell_payload.py` & `fenjing-0.2.8/fenjing/shell_payload.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import Callable, Tuple, Dict
+from typing import Callable, Tuple, Dict, Union
 from .const import OS_POPEN_READ
 from .full_payload_gen import FullPayloadGen
 
 full_payload_store: Dict[int, FullPayloadGen] = {}
 
-def exec_cmd_payload(waf_func: Callable[[str, ], bool], cmd: str) -> Tuple[str | None, bool | None]:
+def exec_cmd_payload(waf_func: Callable[[str, ], bool], cmd: str) -> Tuple[Union[str, None], Union[bool, None]]:
     """根据提供的waf函数为一个shell命令生成对应的payload
 
     Args:
         waf_func (Callable[[str, ], bool]): waf函数，判断提供的payload能否通过waf, 能则返回True
         cmd (str): 需要执行的shell命令
 
     Returns:
```

### Comparing `fenjing-0.2.7/fenjing/waf_func_gen.py` & `fenjing-0.2.8/fenjing/waf_func_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.7/fenjing.egg-info/PKG-INFO` & `fenjing-0.2.8/fenjing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.2.7
+Version: 0.2.8
 Summary: A Jinja2 SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.2.7/fenjing.egg-info/SOURCES.txt` & `fenjing-0.2.8/fenjing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.7/setup.py` & `fenjing-0.2.8/setup.py`

 * *Files identical despite different names*

