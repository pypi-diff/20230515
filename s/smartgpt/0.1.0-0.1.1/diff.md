# Comparing `tmp/smartgpt-0.1.0.tar.gz` & `tmp/smartgpt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartgpt-0.1.0.tar", last modified: Mon May 15 01:07:39 2023, max compression
+gzip compressed data, was "smartgpt-0.1.1.tar", last modified: Mon May 15 03:56:23 2023, max compression
```

## Comparing `smartgpt-0.1.0.tar` & `smartgpt-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-15 01:07:39.926402 smartgpt-0.1.0/
--rw-r--r--   0 evan       (501) staff       (20)     1067 2023-05-11 06:26:43.000000 smartgpt-0.1.0/LICENSE
--rw-r--r--   0 evan       (501) staff       (20)      174 2023-05-15 01:07:39.926639 smartgpt-0.1.0/PKG-INFO
--rw-r--r--   0 evan       (501) staff       (20)     2273 2023-05-14 20:48:56.000000 smartgpt-0.1.0/README.md
-drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-15 01:07:39.916583 smartgpt-0.1.0/bin/
--rwxrwxrwx   0 evan       (501) staff       (20)     1300 2023-05-14 22:16:03.000000 smartgpt-0.1.0/bin/smartgpt
--rw-r--r--   0 evan       (501) staff       (20)       62 2023-05-11 06:10:56.000000 smartgpt-0.1.0/pyproject.toml
--rw-r--r--   0 evan       (501) staff       (20)      103 2023-05-15 01:07:39.927923 smartgpt-0.1.0/setup.cfg
--rw-r--r--   0 evan       (501) staff       (20)      470 2023-05-15 01:07:29.000000 smartgpt-0.1.0/setup.py
-drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-15 01:07:39.921559 smartgpt-0.1.0/smartgpt/
--rw-r--r--   0 evan       (501) staff       (20)      222 2023-05-15 00:44:19.000000 smartgpt-0.1.0/smartgpt/__init__.py
--rw-r--r--   0 evan       (501) staff       (20)    10055 2023-05-15 00:15:08.000000 smartgpt-0.1.0/smartgpt/chat.py
--rw-r--r--   0 evan       (501) staff       (20)     4515 2023-05-15 00:42:32.000000 smartgpt-0.1.0/smartgpt/datatypes.py
--rw-r--r--   0 evan       (501) staff       (20)     1983 2023-05-15 01:06:17.000000 smartgpt-0.1.0/smartgpt/error.py
--rw-r--r--   0 evan       (501) staff       (20)     1146 2023-05-14 22:33:26.000000 smartgpt-0.1.0/smartgpt/logger.py
-drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-15 01:07:39.925851 smartgpt-0.1.0/smartgpt/prompts/
--rw-r--r--   0 evan       (501) staff       (20)      995 2023-05-14 20:45:10.000000 smartgpt-0.1.0/smartgpt/prompts/__init__.py
--rw-r--r--   0 evan       (501) staff       (20)     2125 2023-05-15 01:06:03.000000 smartgpt-0.1.0/smartgpt/repl.py
--rw-r--r--   0 evan       (501) staff       (20)     1379 2023-05-11 06:10:56.000000 smartgpt-0.1.0/smartgpt/strenum.py
--rw-r--r--   0 evan       (501) staff       (20)      808 2023-05-15 00:52:53.000000 smartgpt-0.1.0/smartgpt/user_profile.py
--rw-r--r--   0 evan       (501) staff       (20)       78 2023-05-14 22:46:57.000000 smartgpt-0.1.0/smartgpt/util.py
-drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-15 01:07:39.925213 smartgpt-0.1.0/smartgpt.egg-info/
--rw-r--r--   0 evan       (501) staff       (20)      174 2023-05-15 01:07:39.000000 smartgpt-0.1.0/smartgpt.egg-info/PKG-INFO
--rw-r--r--   0 evan       (501) staff       (20)      459 2023-05-15 01:07:39.000000 smartgpt-0.1.0/smartgpt.egg-info/SOURCES.txt
--rw-r--r--   0 evan       (501) staff       (20)        1 2023-05-15 01:07:39.000000 smartgpt-0.1.0/smartgpt.egg-info/dependency_links.txt
--rw-r--r--   0 evan       (501) staff       (20)        1 2023-05-15 00:27:20.000000 smartgpt-0.1.0/smartgpt.egg-info/not-zip-safe
--rw-r--r--   0 evan       (501) staff       (20)       42 2023-05-15 01:07:39.000000 smartgpt-0.1.0/smartgpt.egg-info/requires.txt
--rw-r--r--   0 evan       (501) staff       (20)        9 2023-05-15 01:07:39.000000 smartgpt-0.1.0/smartgpt.egg-info/top_level.txt
+drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-15 03:56:23.638495 smartgpt-0.1.1/
+-rw-r--r--   0 evan       (501) staff       (20)     1067 2023-05-11 06:26:43.000000 smartgpt-0.1.1/LICENSE
+-rw-r--r--   0 evan       (501) staff       (20)      174 2023-05-15 03:56:23.638737 smartgpt-0.1.1/PKG-INFO
+-rw-r--r--   0 evan       (501) staff       (20)     2273 2023-05-14 20:48:56.000000 smartgpt-0.1.1/README.md
+drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-15 03:56:23.631620 smartgpt-0.1.1/bin/
+-rwxrwxrwx   0 evan       (501) staff       (20)     5058 2023-05-15 03:51:22.000000 smartgpt-0.1.1/bin/smartgpt
+-rw-r--r--   0 evan       (501) staff       (20)       62 2023-05-11 06:10:56.000000 smartgpt-0.1.1/pyproject.toml
+-rw-r--r--   0 evan       (501) staff       (20)      103 2023-05-15 03:56:23.639641 smartgpt-0.1.1/setup.cfg
+-rw-r--r--   0 evan       (501) staff       (20)      470 2023-05-15 03:55:56.000000 smartgpt-0.1.1/setup.py
+drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-15 03:56:23.634983 smartgpt-0.1.1/smartgpt/
+-rw-r--r--   0 evan       (501) staff       (20)      237 2023-05-15 03:44:52.000000 smartgpt-0.1.1/smartgpt/__init__.py
+-rw-r--r--   0 evan       (501) staff       (20)    10063 2023-05-15 03:44:52.000000 smartgpt-0.1.1/smartgpt/chat.py
+-rw-r--r--   0 evan       (501) staff       (20)     5538 2023-05-15 03:50:20.000000 smartgpt-0.1.1/smartgpt/datatypes.py
+-rw-r--r--   0 evan       (501) staff       (20)     1130 2023-05-15 03:44:52.000000 smartgpt-0.1.1/smartgpt/error.py
+-rw-r--r--   0 evan       (501) staff       (20)     1510 2023-05-15 01:46:46.000000 smartgpt-0.1.1/smartgpt/logger.py
+drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-15 03:56:23.638017 smartgpt-0.1.1/smartgpt/prompts/
+-rw-r--r--   0 evan       (501) staff       (20)      995 2023-05-14 20:45:10.000000 smartgpt-0.1.1/smartgpt/prompts/__init__.py
+-rw-r--r--   0 evan       (501) staff       (20)     2113 2023-05-15 03:31:58.000000 smartgpt-0.1.1/smartgpt/repl.py
+-rw-r--r--   0 evan       (501) staff       (20)     1379 2023-05-11 06:10:56.000000 smartgpt-0.1.1/smartgpt/strenum.py
+-rw-r--r--   0 evan       (501) staff       (20)      808 2023-05-15 00:52:53.000000 smartgpt-0.1.1/smartgpt/user_profile.py
+-rw-r--r--   0 evan       (501) staff       (20)      900 2023-05-15 03:44:53.000000 smartgpt-0.1.1/smartgpt/util.py
+drwxr-xr-x   0 evan       (501) staff       (20)        0 2023-05-15 03:56:23.637299 smartgpt-0.1.1/smartgpt.egg-info/
+-rw-r--r--   0 evan       (501) staff       (20)      174 2023-05-15 03:56:23.000000 smartgpt-0.1.1/smartgpt.egg-info/PKG-INFO
+-rw-r--r--   0 evan       (501) staff       (20)      459 2023-05-15 03:56:23.000000 smartgpt-0.1.1/smartgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 evan       (501) staff       (20)        1 2023-05-15 03:56:23.000000 smartgpt-0.1.1/smartgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 evan       (501) staff       (20)        1 2023-05-15 00:27:20.000000 smartgpt-0.1.1/smartgpt.egg-info/not-zip-safe
+-rw-r--r--   0 evan       (501) staff       (20)       42 2023-05-15 03:56:23.000000 smartgpt-0.1.1/smartgpt.egg-info/requires.txt
+-rw-r--r--   0 evan       (501) staff       (20)        9 2023-05-15 03:56:23.000000 smartgpt-0.1.1/smartgpt.egg-info/top_level.txt
```

### Comparing `smartgpt-0.1.0/LICENSE` & `smartgpt-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.0/README.md` & `smartgpt-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.0/smartgpt/chat.py` & `smartgpt-0.1.1/smartgpt/chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     Credentials,
     GPTConfig,
     Message,
     Mode,
     Response,
     Role,
     Settings,
+    Verbosity,
 )
 from smartgpt.logger import default_logger, get_logger
 from smartgpt.repl import repl
 from smartgpt.user_profile import SETTINGS_PATH
 
 
 @attrs.define
@@ -145,21 +146,20 @@
     """
 
     config: GPTConfig
     main: Agent
     researcher: Agent
     resolver: Agent
     generators: List[Agent]
-    debug: bool = False
+    verbosity: Verbosity = Verbosity.SOME
 
     logger: logging.Logger = attrs.field(init=False)
 
     def __attrs_post_init__(self) -> None:
-        self.logger = get_logger()
-        self.logger.setLevel(logging.DEBUG if self.debug else logging.INFO)
+        self.logger = get_logger(verbosity=self.verbosity)
 
     def create_response(self, prompt: str) -> Message:
         """
         Determines the mode of interaction based on the current configuration and
         generates a response from the model accordingly.
 
         In ZERO_SHOT mode, the prompt is sent directly to the main agent, which sends it
@@ -228,15 +228,15 @@
 
             researcher_response = self.researcher.response(researcher_prompt)
             self.logger.debug(f"Researcher response:\n{researcher_response.content}")
 
             self.logger.info("Generating response for resolver...")
 
             resolver_prompt = prompts.you_are_a_resolver(
-                candidates, silence_rationale=not self.debug
+                candidates, silence_rationale=(self.verbosity != Verbosity.ALL)
             )
             self.logger.debug(f"Resolver prompt:\n{resolver_prompt}")
 
             self.resolver.messages = copy.deepcopy(self.researcher.messages)
             response = self.resolver.response(resolver_prompt)
 
             # Add the prompt and response to the main agent
@@ -277,12 +277,12 @@
                 Agent(
                     credentials=settings.credentials,
                     model=settings.model,
                     temp=settings.generator_temps[i],
                 )
                 for i in range(settings.num_agents)
             ],
-            debug=settings.debug,
+            verbosity=settings.verbosity,
         )
 
     def repl(self) -> None:
         repl(self)
```

### Comparing `smartgpt-0.1.0/smartgpt/datatypes.py` & `smartgpt-0.1.1/smartgpt/datatypes.py`

 * *Files 17% similar despite different names*

```diff
@@ -39,17 +39,34 @@
 class Settings:
     generator_temps: List[float]
     researcher_temp: float
     resolver_temp: float
     model: str
     mode: Mode
     credentials: Credentials
-    debug: bool
+    verbosity: Verbosity
     vi_mode: bool
 
+    def __repr__(self):
+        margin = " " * 4
+        lines = [f"\n{margin}Runtime Settings"]
+        middle_prefix = f"{margin}├── "
+        final_prefix = f"{margin}└── "
+
+        attr_names = [attr.name for attr in attrs.fields(Settings)]
+        max_len = max(len(attr_name) for attr_name in attr_names)
+
+        for idx, attr_name in enumerate(attr_names):
+            attr_val = getattr(self, attr_name)
+            spacer = " " * (max_len - len(attr_name))
+            prefix = final_prefix if idx == len(attr_names) - 1 else middle_prefix
+            lines.append(f"{prefix}{attr_name}{spacer} = {attr_val.__str__()}")
+
+        return "\n".join(lines) + "\n"
+
     @property
     def num_agents(self) -> int:
         return len(self.generator_temps)
 
     def save(self, path: Pathish) -> Path:
         path = Path(path)
         with path.open("w") as file:
@@ -73,26 +90,43 @@
         return cls(
             generator_temps=[0.7, 0.7, 0.7],
             researcher_temp=0.5,
             resolver_temp=0.5,
             model="gpt-4",
             mode=Mode.RESOLVER,
             credentials=Credentials.dummy(),
-            debug=False,
+            verbosity=Verbosity.SOME,
             vi_mode=False,
         )
 
 
+class Verbosity(strenum.StrEnum):
+    NONE = strenum.auto()
+    SOME = strenum.auto()
+    ALL = strenum.auto()
+
+
+DUMMY_KEY = "XXXXXX"
+
+
+def _api_key_repr(key: str) -> str:
+    if key == DUMMY_KEY:
+        return key
+
+    assert len(key) > 8
+    return key[:4] + "*" * 4 + key[-4:]
+
+
 @attrs.define
 class Credentials:
-    key: str
+    key: str = attrs.field(repr=_api_key_repr)
 
     @classmethod
     def dummy(cls) -> Credentials:
-        return cls("XXXXXX")
+        return cls(DUMMY_KEY)
 
 
 class Mode(strenum.StrEnum):
     """Enum representing the different modes of interaction."""
 
     ZERO_SHOT = strenum.auto()
     STEP_BY_STEP = strenum.auto()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `smartgpt-0.1.0/smartgpt/prompts/__init__.py` & `smartgpt-0.1.1/smartgpt/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.0/smartgpt/repl.py` & `smartgpt-0.1.1/smartgpt/repl.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     wrap_lines=True,
     vi_mode=Settings.load(SETTINGS_PATH).vi_mode,
 )
 
 
 USER_PREFIX = FormattedText(
     [
-        ("fg:ansigreen", "(To submit: press ESC, then ENTER)\n"),
+        ("", "(To submit: press ESC, then ENTER)\n"),
         ("bold fg:ansigreen", "> "),
     ]
 )
 
 
 class Model(Protocol):
     def create_response(self, prompt: str) -> Message:
```

### Comparing `smartgpt-0.1.0/smartgpt/strenum.py` & `smartgpt-0.1.1/smartgpt/strenum.py`

 * *Files identical despite different names*

### Comparing `smartgpt-0.1.0/smartgpt/user_profile.py` & `smartgpt-0.1.1/smartgpt/user_profile.py`

 * *Files identical despite different names*

