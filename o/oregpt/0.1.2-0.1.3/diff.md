# Comparing `tmp/oregpt-0.1.2.tar.gz` & `tmp/oregpt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oregpt-0.1.2.tar", max compression
+gzip compressed data, was "oregpt-0.1.3.tar", max compression
```

## Comparing `oregpt-0.1.2.tar` & `oregpt-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,13 @@
--rw-r--r--   0        0        0     1076 2023-05-07 04:09:40.942289 oregpt-0.1.2/LICENSE
--rw-r--r--   0        0        0     2051 2023-05-07 08:54:28.160734 oregpt-0.1.2/README.md
--rw-r--r--   0        0        0     2274 2023-05-07 08:41:56.348454 oregpt-0.1.2/oregpt/chat_bot.py
--rw-r--r--   0        0        0     2136 2023-05-07 08:41:56.348614 oregpt-0.1.2/oregpt/main.py
--rw-r--r--   0        0        0      304 2023-05-07 08:41:56.348724 oregpt-0.1.2/oregpt/resources/config.yml
--rw-r--r--   0        0        0     2188 2023-05-07 08:41:56.348886 oregpt-0.1.2/oregpt/stdinout.py
--rw-r--r--   0        0        0     1907 2023-05-07 08:54:28.160930 oregpt-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-07 04:09:40.943569 oregpt-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0      851 2023-05-07 08:41:56.349839 oregpt-0.1.2/tests/test_chat_bot.py
--rw-r--r--   0        0        0     2913 1970-01-01 00:00:00.000000 oregpt-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-07 04:09:40.942289 oregpt-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2612 2023-05-15 11:00:22.153239 oregpt-0.1.3/README.md
+-rw-r--r--   0        0        0     2116 2023-05-15 00:57:48.021998 oregpt-0.1.3/oregpt/chat_bot.py
+-rw-r--r--   0        0        0     3647 2023-05-15 11:00:22.153431 oregpt-0.1.3/oregpt/command.py
+-rw-r--r--   0        0        0     2077 2023-05-15 11:00:22.153598 oregpt-0.1.3/oregpt/main.py
+-rw-r--r--   0        0        0      304 2023-05-07 08:41:56.348724 oregpt-0.1.3/oregpt/resources/config.yml
+-rw-r--r--   0        0        0     2352 2023-05-15 00:57:48.022534 oregpt-0.1.3/oregpt/stdinout.py
+-rw-r--r--   0        0        0     2117 2023-05-15 11:00:30.334307 oregpt-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-07 04:09:40.943569 oregpt-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     1290 2023-05-15 11:00:22.153925 oregpt-0.1.3/tests/conftest.py
+-rw-r--r--   0        0        0     1765 2023-05-15 11:00:22.154075 oregpt-0.1.3/tests/test_chat_bot.py
+-rw-r--r--   0        0        0     1425 2023-05-15 11:00:22.154223 oregpt-0.1.3/tests/test_command.py
+-rw-r--r--   0        0        0     3474 1970-01-01 00:00:00.000000 oregpt-0.1.3/PKG-INFO
```

### Comparing `oregpt-0.1.2/LICENSE` & `oregpt-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `oregpt-0.1.2/README.md` & `oregpt-0.1.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![release](https://img.shields.io/github/release/shinichi-takayanagi/oregpt.svg)](https://github.com/shinichi-takayanagi/oregpt/releases/latest)
 [![python-version](https://img.shields.io/pypi/pyversions/oregpt.svg)](https://pypi.org/project/oregpt/)
 [![pypi](https://img.shields.io/pypi/v/oregpt?color=%2334D058&label=pypi%20package)](https://pypi.org/project/oregpt)
 
 A tiny GPT CLI tool.
 You can chat with the GPT model developped by OpenAI and save the conversation as json.
 
-![oregpt](https://user-images.githubusercontent.com/24406372/236609166-0f2385b1-fd9e-4810-b80d-c19c44d13411.gif)
+<img src="https://github.com/shinichi-takayanagi/oregpt/assets/24406372/91969861-9f29-4c81-9505-620ef5567a5b" width="800px">
 
 ## Installation
 ### Get your own OpenAI API Key
 Assuming you have an environment variable with key named `OPENAI_API_KEY`.
 If you don't have a OpenAI API key [visit here](https://platform.openai.com/account/api-keys), generate one and add it as an environment variable
 
 ```bash
@@ -29,14 +29,28 @@
 
 ## Usage
 Once you have installed oregpt, you can run it by typing:
 ```bash
 $ oregpt
 ```
 
+## Supported commands on chat
+Commands such as saving and loading conversations are available as the following:
+
+|  Command  |  Description  |
+| ---- | ---- |
+| `/exit`    | Exit from this chat tool |
+| `/quit`    | Exit from this chat tool |
+| `/q`       | Exit from this chat tool |
+| `/clear`   | Clear chat history all |
+| `/history` | Show chat history in json format |
+| `/save`    | Save chat hisotry in json format |
+| `/load`    | Load chat hisotry from a json file |
+| `/help`    | Show all commands which you can use in this chat tool |
+
 ## Configuration
 You can specify the place of conversation `log`,
 [style (color etc)](https://python-prompt-toolkit.readthedocs.io/en/master/pages/advanced_topics/styling.html)
 and
 [the model supported in /v1/chat/completions endpoint provided by OpenAI](https://platform.openai.com/docs/models/overview)
 in `~/.config/oregpt/config.yml`
 ```yaml
```

### Comparing `oregpt-0.1.2/oregpt/main.py` & `oregpt-0.1.3/oregpt/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import shutil
 from typing import Any
 
 import openai
 import yaml
 
 from oregpt.chat_bot import ChatBot
+from oregpt.command import CommandBuilder
 from oregpt.stdinout import StdInOut
 
 
 def load_config() -> dict[str, Any]:
     # TODO: Find more sophisticated way to do this...
     config_file = os.path.join(os.path.expanduser("~"), ".config/oregpt/config.yml")
     if not os.path.exists(config_file):
@@ -32,35 +33,32 @@
 
     raise LookupError("OpenAI's API key was not found in config.yml and environment variables")
 
 
 def main() -> int:
     config = load_config()
     initialize_open_ai_key(config["openai"])
-    std_in_out = StdInOut(config["character"], lambda: "To exit, type q, quit, exit, or Ctrl + C")
+    std_in_out = StdInOut(config["character"], lambda: "To exit, type /q, /quit, /exit, or Ctrl + C")
     bot = ChatBot(config["openai"]["model"], std_in_out)
+    command_builder = CommandBuilder(config, bot)
 
     try:
         while True:
             message = std_in_out.input().lower()
-            match message:
-                case "exit" | "quit" | "q":
-                    break
-                case "clear":
-                    bot.clear()
-                    std_in_out.print_system("Clear all conversation history")
-                case "history":
-                    std_in_out.print_system(str(bot.log))
-                case "save":
-                    file_name = bot.save(config["log"])
-                    std_in_out.print_system(f"Save all conversation history in {file_name}")
-                case _:
+            if command := command_builder.build(message):
+                command.execute()
+            else:
+                if command_builder.looks_like_command(message):
+                    std_in_out.print_system("Invalid command. Valid commands are as the following:")
+                    command_builder.build("/help").execute()  # type: ignore
+                else:
                     bot.respond(message)
     except KeyboardInterrupt:
         return 0
     except Exception as e:
         raise Exception(f"Something happened: {str(e)}") from e
+
     return 0
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `oregpt-0.1.2/oregpt/stdinout.py` & `oregpt-0.1.3/oregpt/stdinout.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,19 @@
 class Character:
     name: str
     style: str
 
 
 class StdInOut:
     def __init__(self, config: dict[str, Any], bottom_toolbar: Optional[AnyFormattedText]):
-        self._characters: dict[str, Character] = {}
+        self._characters: dict[str, Character] = {
+            "user": Character("Me", "#00BEFE"),
+            "assistant": Character("AI", "#87CEEB"),
+            "system": Character("System", "#cc0000"),
+        }
         for key, value in config.items():
             self._characters[key] = Character(**value)
         self._bottom_toolbar = bottom_toolbar
 
     def input(self) -> str:
         text = FormattedText([("class:user", f"<{self._characters['user'].name}> ")])
         return str(prompt(text, style=self._style(), bottom_toolbar=self._bottom_toolbar))
```

### Comparing `oregpt-0.1.2/pyproject.toml` & `oregpt-0.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oregpt"
-version = "0.1.2"
+version = "0.1.3"
 description = "A tiny GPT CLI tool"
 authors = ["Shinichi Takayanagi <shinichi.takayanagi@gmail.com>"]
 homepage = "https://github.com/shinichi-takayanagi/oregpt"
 repository = "https://github.com/shinichi-takayanagi/oregpt"
 license = "MIT"
 readme = "README.md"
 keywords = ["gpt-chatbot", "gpt-cli", "openai-cli"]
@@ -36,14 +36,15 @@
 
 
 [tool.poetry.group.lint.dependencies]
 black = "^23.3.0"
 isort = "^5.12.0"
 mypy = "^1.2.0"
 autoflake = "^2.1.1"
+pre-commit = "^3.3.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 # === Black ===
@@ -58,14 +59,20 @@
   | docs
   | docs_src
   | .venv
   | .mypy_cache
 )/
 '''
 
+# === Autoflake ===
+[tool.autoflake]
+remove-all-unused-imports = true
+remove-duplicate-keys = true
+remove-unused-variables = true
+
 # === Isort ===
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
@@ -79,15 +86,19 @@
 norecursedirs = ["venv", ".venv", ".env"]
 testpaths = [
     "tests",
 ]
 console_output_style = "progress"
 log_cli = true
 
+
+# === Mypy ===
 [tool.mypy]
+strict = true
+scripts_are_modules = true
 check_untyped_defs = true
 disallow_untyped_defs = true
 disallow_any_generics = true
 ignore_missing_imports = true
 no_implicit_optional = true
 no_site_packages = true
 show_error_codes = true
```

### Comparing `oregpt-0.1.2/PKG-INFO` & `oregpt-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oregpt
-Version: 0.1.2
+Version: 0.1.3
 Summary: A tiny GPT CLI tool
 Home-page: https://github.com/shinichi-takayanagi/oregpt
 License: MIT
 Keywords: gpt-chatbot,gpt-cli,openai-cli
 Author: Shinichi Takayanagi
 Author-email: shinichi.takayanagi@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -27,15 +27,15 @@
 [![release](https://img.shields.io/github/release/shinichi-takayanagi/oregpt.svg)](https://github.com/shinichi-takayanagi/oregpt/releases/latest)
 [![python-version](https://img.shields.io/pypi/pyversions/oregpt.svg)](https://pypi.org/project/oregpt/)
 [![pypi](https://img.shields.io/pypi/v/oregpt?color=%2334D058&label=pypi%20package)](https://pypi.org/project/oregpt)
 
 A tiny GPT CLI tool.
 You can chat with the GPT model developped by OpenAI and save the conversation as json.
 
-![oregpt](https://user-images.githubusercontent.com/24406372/236609166-0f2385b1-fd9e-4810-b80d-c19c44d13411.gif)
+<img src="https://github.com/shinichi-takayanagi/oregpt/assets/24406372/91969861-9f29-4c81-9505-620ef5567a5b" width="800px">
 
 ## Installation
 ### Get your own OpenAI API Key
 Assuming you have an environment variable with key named `OPENAI_API_KEY`.
 If you don't have a OpenAI API key [visit here](https://platform.openai.com/account/api-keys), generate one and add it as an environment variable
 
 ```bash
@@ -52,14 +52,28 @@
 
 ## Usage
 Once you have installed oregpt, you can run it by typing:
 ```bash
 $ oregpt
 ```
 
+## Supported commands on chat
+Commands such as saving and loading conversations are available as the following:
+
+|  Command  |  Description  |
+| ---- | ---- |
+| `/exit`    | Exit from this chat tool |
+| `/quit`    | Exit from this chat tool |
+| `/q`       | Exit from this chat tool |
+| `/clear`   | Clear chat history all |
+| `/history` | Show chat history in json format |
+| `/save`    | Save chat hisotry in json format |
+| `/load`    | Load chat hisotry from a json file |
+| `/help`    | Show all commands which you can use in this chat tool |
+
 ## Configuration
 You can specify the place of conversation `log`,
 [style (color etc)](https://python-prompt-toolkit.readthedocs.io/en/master/pages/advanced_topics/styling.html)
 and
 [the model supported in /v1/chat/completions endpoint provided by OpenAI](https://platform.openai.com/docs/models/overview)
 in `~/.config/oregpt/config.yml`
 ```yaml
```

