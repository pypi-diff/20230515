# Comparing `tmp/gptty-0.2.5.tar.gz` & `tmp/gptty-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptty-0.2.5.tar", last modified: Tue Apr  4 22:03:51 2023, max compression
+gzip compressed data, was "gptty-0.2.6.tar", last modified: Mon May 15 19:14:45 2023, max compression
```

## Comparing `gptty-0.2.5.tar` & `gptty-0.2.6.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-04-04 22:03:51.215911 gptty-0.2.5/
--rw-rw-r--   0 sig       (1000) sig       (1000)     1073 2023-03-19 16:18:57.000000 gptty-0.2.5/LICENSE
--rw-rw-r--   0 sig       (1000) sig       (1000)      102 2023-03-28 21:47:19.000000 gptty-0.2.5/MANIFEST.in
--rw-rw-r--   0 sig       (1000) sig       (1000)    11989 2023-04-04 22:03:51.215911 gptty-0.2.5/PKG-INFO
--rw-rw-r--   0 sig       (1000) sig       (1000)    11566 2023-04-04 22:00:34.000000 gptty-0.2.5/README.md
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-04-04 22:03:51.207911 gptty-0.2.5/assets/
--rw-rw-r--   0 sig       (1000) sig       (1000)    90232 2023-03-20 03:21:49.000000 gptty-0.2.5/assets/context_example.png
--rw-rw-r--   0 sig       (1000) sig       (1000)   170440 2023-03-27 23:01:52.000000 gptty-0.2.5/assets/question_chain_example.png
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-04-04 22:03:51.211911 gptty-0.2.5/gptty/
--rw-rw-r--   0 sig       (1000) sig       (1000)      269 2023-04-04 22:02:02.000000 gptty-0.2.5/gptty/__init__.py
--rw-rw-r--   0 sig       (1000) sig       (1000)     7020 2023-04-04 22:02:02.000000 gptty-0.2.5/gptty/__main__.py
--rw-rw-r--   0 sig       (1000) sig       (1000)     1819 2023-04-04 22:02:02.000000 gptty-0.2.5/gptty/config.py
--rw-rw-r--   0 sig       (1000) sig       (1000)     7531 2023-04-04 22:02:02.000000 gptty-0.2.5/gptty/context.py
--rw-rw-r--   0 sig       (1000) sig       (1000)    14220 2023-04-04 22:02:02.000000 gptty-0.2.5/gptty/gptty.py
--rw-rw-r--   0 sig       (1000) sig       (1000)     3349 2023-04-04 22:02:02.000000 gptty-0.2.5/gptty/tagging.py
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-04-04 22:03:51.215911 gptty-0.2.5/gptty.egg-info/
--rw-rw-r--   0 sig       (1000) sig       (1000)    11989 2023-04-04 22:03:51.000000 gptty-0.2.5/gptty.egg-info/PKG-INFO
--rw-rw-r--   0 sig       (1000) sig       (1000)      458 2023-04-04 22:03:51.000000 gptty-0.2.5/gptty.egg-info/SOURCES.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)        1 2023-04-04 22:03:51.000000 gptty-0.2.5/gptty.egg-info/dependency_links.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)       46 2023-04-04 22:03:51.000000 gptty-0.2.5/gptty.egg-info/entry_points.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)      119 2023-04-04 22:03:51.000000 gptty-0.2.5/gptty.egg-info/requires.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)        6 2023-04-04 22:03:51.000000 gptty-0.2.5/gptty.egg-info/top_level.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)      118 2023-04-02 01:10:59.000000 gptty-0.2.5/requirements.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)       38 2023-04-04 22:03:51.215911 gptty-0.2.5/setup.cfg
--rw-rw-r--   0 sig       (1000) sig       (1000)      835 2023-04-04 22:02:02.000000 gptty-0.2.5/setup.py
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-04-04 22:03:51.215911 gptty-0.2.5/tests/
--rw-rw-r--   0 sig       (1000) sig       (1000)     1900 2023-03-29 19:30:28.000000 gptty-0.2.5/tests/test_config.py
--rw-rw-r--   0 sig       (1000) sig       (1000)     5149 2023-04-04 21:44:31.000000 gptty-0.2.5/tests/test_context.py
--rw-rw-r--   0 sig       (1000) sig       (1000)     1036 2023-03-29 19:43:35.000000 gptty-0.2.5/tests/test_tagging.py
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-05-15 19:14:45.792317 gptty-0.2.6/
+-rw-rw-r--   0 sig       (1000) sig       (1000)     1073 2023-03-19 16:18:57.000000 gptty-0.2.6/LICENSE
+-rw-rw-r--   0 sig       (1000) sig       (1000)       46 2023-04-05 23:32:19.000000 gptty-0.2.6/MANIFEST.in
+-rw-rw-r--   0 sig       (1000) sig       (1000)    12097 2023-05-15 19:14:45.792317 gptty-0.2.6/PKG-INFO
+-rw-rw-r--   0 sig       (1000) sig       (1000)    11674 2023-05-14 21:20:17.000000 gptty-0.2.6/README.md
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-05-15 19:14:45.788317 gptty-0.2.6/assets/
+-rw-rw-r--   0 sig       (1000) sig       (1000)    90232 2023-03-20 03:21:49.000000 gptty-0.2.6/assets/context_example.png
+-rw-rw-r--   0 sig       (1000) sig       (1000)   125593 2023-03-29 18:54:23.000000 gptty-0.2.6/assets/error_troubleshooting_example.png
+-rw-rw-r--   0 sig       (1000) sig       (1000)    83079 2023-03-31 16:52:10.000000 gptty-0.2.6/assets/json_example.png
+-rw-rw-r--   0 sig       (1000) sig       (1000)   170440 2023-03-27 23:01:52.000000 gptty-0.2.6/assets/question_chain_example.png
+-rw-rw-r--   0 sig       (1000) sig       (1000)    53244 2023-03-30 21:07:16.000000 gptty-0.2.6/assets/verbosity_example.png
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-05-15 19:14:45.788317 gptty-0.2.6/gptty/
+-rw-rw-r--   0 sig       (1000) sig       (1000)      269 2023-05-15 19:14:04.000000 gptty-0.2.6/gptty/__init__.py
+-rw-rw-r--   0 sig       (1000) sig       (1000)     8533 2023-05-15 19:14:04.000000 gptty-0.2.6/gptty/__main__.py
+-rw-rw-r--   0 sig       (1000) sig       (1000)     3415 2023-05-15 19:14:04.000000 gptty-0.2.6/gptty/config.py
+-rw-rw-r--   0 sig       (1000) sig       (1000)     9363 2023-05-15 19:14:04.000000 gptty-0.2.6/gptty/context.py
+-rw-rw-r--   0 sig       (1000) sig       (1000)    18316 2023-05-15 19:14:04.000000 gptty-0.2.6/gptty/gptty.py
+-rw-rw-r--   0 sig       (1000) sig       (1000)     4154 2023-05-15 19:14:04.000000 gptty-0.2.6/gptty/tagging.py
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-05-15 19:14:45.788317 gptty-0.2.6/gptty.egg-info/
+-rw-rw-r--   0 sig       (1000) sig       (1000)    12097 2023-05-15 19:14:45.000000 gptty-0.2.6/gptty.egg-info/PKG-INFO
+-rw-rw-r--   0 sig       (1000) sig       (1000)      552 2023-05-15 19:14:45.000000 gptty-0.2.6/gptty.egg-info/SOURCES.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)        1 2023-05-15 19:14:45.000000 gptty-0.2.6/gptty.egg-info/dependency_links.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)       46 2023-05-15 19:14:45.000000 gptty-0.2.6/gptty.egg-info/entry_points.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)      119 2023-05-15 19:14:45.000000 gptty-0.2.6/gptty.egg-info/requires.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)        6 2023-05-15 19:14:45.000000 gptty-0.2.6/gptty.egg-info/top_level.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)      118 2023-04-02 01:10:59.000000 gptty-0.2.6/requirements.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)       38 2023-05-15 19:14:45.792317 gptty-0.2.6/setup.cfg
+-rw-rw-r--   0 sig       (1000) sig       (1000)      835 2023-05-15 19:14:04.000000 gptty-0.2.6/setup.py
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-05-15 19:14:45.788317 gptty-0.2.6/tests/
+-rw-rw-r--   0 sig       (1000) sig       (1000)     2047 2023-05-14 21:23:21.000000 gptty-0.2.6/tests/test_config.py
+-rw-rw-r--   0 sig       (1000) sig       (1000)     5149 2023-04-04 21:44:31.000000 gptty-0.2.6/tests/test_context.py
+-rw-rw-r--   0 sig       (1000) sig       (1000)     1036 2023-03-29 19:43:35.000000 gptty-0.2.6/tests/test_tagging.py
```

### Comparing `gptty-0.2.5/LICENSE` & `gptty-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gptty-0.2.5/PKG-INFO` & `gptty-0.2.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,13 @@
-Metadata-Version: 2.1
-Name: gptty
-Version: 0.2.5
-Summary: Chat GPT wrapper in your TTY 
-Home-page: https://github.com/signebedi/gptty
-Author: Sig Janoska-Bedi
-Author-email: signe@atreeus.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # gptty
 
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/signebedi/gptty/blob/master/LICENSE) 
+[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/signebedi/gptty/blob/master/LICENSE) 
 [![PyPI version](https://badge.fury.io/py/gptty.svg)](https://pypi.python.org/pypi/gptty)
 [![Downloads](https://static.pepy.tech/badge/gptty)](https://pepy.tech/project/gptty)
-[![gptty tests](https://github.com/signebedi/gptty/workflows/Tests/badge.svg)](https://github.com/signebedi/gptty/actions)
+[![gptty tests](https://github.com/signebedi/gptty/workflows/tests/badge.svg)](https://github.com/signebedi/gptty/actions)
 
 ChatGPT wrapper in your TTY
 
 ## About
 
 gptty is a ChatGPT shell interface that allows you to (1) interact with ChatGPT in a manner similar to the web application, but without needing to rely on the web application's stability; (2) preserve context across chat sessions and structure your conversations however you want; (3) save local copies of your conversations for easy reference.
 
@@ -65,15 +51,16 @@
 
 ## Configuration
 
 `gptty` reads configuration settings from a file named `gptty.ini`, which the app expects to be located in the same directory that you are running `gptty` from unless you pass a custom `config_file`. The file uses the INI file format, which consists of sections, each with its own key-value pairs.
 
 | Key    | Type | Default Value    | Description |
 | -------- | ------- | -------- | ------- |
-| api_key  | String    | ""  |   The API key for OpenAI's GPT service  |
+| api_key  | String    | ""  |   Your API key for OpenAI's GPT service  |
+| org_id  | String    | ""  |   Your organization ID for OpenAI's GPT service  |
 | your_name    | String    | "question"    |   The name of the input prompt  |
 | gpt_name  | String    | "response"  |   The name of the generated response  |
 | output_file | String     | "output.txt" |    The name of the file where the output will be saved  |
 | model    | String    | "text-davinci-003"    |   The name of the GPT model to use  |
 | temperature  | Float    | 0.0  |   The temperature to use for sampling  |
 | max_tokens | Integer     | 250 |    The maximum number of tokens to generate for the response  |
 | max_context_length    | Integer    | 150    |   The maximum length of the input context  |
@@ -114,14 +101,15 @@
 
 To use a command, simply type it into the command prompt and press Enter. For example, use the following command to display the current configuration settings in the terminal:
 
 ```
 > :configs
 
 api_key: SOME_CONFIG_HERE
+org_id: org-SOME_CHARS_HERE
 your_name: question
 gpt_name: response
 output_file: output.txt
 model: text-davinci-003
 temperature: 0.0
 max_tokens: 250
 max_context_length: 5000
```

### Comparing `gptty-0.2.5/README.md` & `gptty-0.2.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,27 @@
+Metadata-Version: 2.1
+Name: gptty
+Version: 0.2.6
+Summary: Chat GPT wrapper in your TTY 
+Home-page: https://github.com/signebedi/gptty
+Author: Sig Janoska-Bedi
+Author-email: signe@atreeus.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # gptty
 
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/signebedi/gptty/blob/master/LICENSE) 
+[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/signebedi/gptty/blob/master/LICENSE) 
 [![PyPI version](https://badge.fury.io/py/gptty.svg)](https://pypi.python.org/pypi/gptty)
 [![Downloads](https://static.pepy.tech/badge/gptty)](https://pepy.tech/project/gptty)
-[![gptty tests](https://github.com/signebedi/gptty/workflows/Tests/badge.svg)](https://github.com/signebedi/gptty/actions)
+[![gptty tests](https://github.com/signebedi/gptty/workflows/tests/badge.svg)](https://github.com/signebedi/gptty/actions)
 
 ChatGPT wrapper in your TTY
 
 ## About
 
 gptty is a ChatGPT shell interface that allows you to (1) interact with ChatGPT in a manner similar to the web application, but without needing to rely on the web application's stability; (2) preserve context across chat sessions and structure your conversations however you want; (3) save local copies of your conversations for easy reference.
 
@@ -51,15 +65,16 @@
 
 ## Configuration
 
 `gptty` reads configuration settings from a file named `gptty.ini`, which the app expects to be located in the same directory that you are running `gptty` from unless you pass a custom `config_file`. The file uses the INI file format, which consists of sections, each with its own key-value pairs.
 
 | Key    | Type | Default Value    | Description |
 | -------- | ------- | -------- | ------- |
-| api_key  | String    | ""  |   The API key for OpenAI's GPT service  |
+| api_key  | String    | ""  |   Your API key for OpenAI's GPT service  |
+| org_id  | String    | ""  |   Your organization ID for OpenAI's GPT service  |
 | your_name    | String    | "question"    |   The name of the input prompt  |
 | gpt_name  | String    | "response"  |   The name of the generated response  |
 | output_file | String     | "output.txt" |    The name of the file where the output will be saved  |
 | model    | String    | "text-davinci-003"    |   The name of the GPT model to use  |
 | temperature  | Float    | 0.0  |   The temperature to use for sampling  |
 | max_tokens | Integer     | 250 |    The maximum number of tokens to generate for the response  |
 | max_context_length    | Integer    | 150    |   The maximum length of the input context  |
@@ -100,14 +115,15 @@
 
 To use a command, simply type it into the command prompt and press Enter. For example, use the following command to display the current configuration settings in the terminal:
 
 ```
 > :configs
 
 api_key: SOME_CONFIG_HERE
+org_id: org-SOME_CHARS_HERE
 your_name: question
 gpt_name: response
 output_file: output.txt
 model: text-davinci-003
 temperature: 0.0
 max_tokens: 250
 max_context_length: 5000
```

### Comparing `gptty-0.2.5/assets/context_example.png` & `gptty-0.2.6/assets/context_example.png`

 * *Files identical despite different names*

### Comparing `gptty-0.2.5/assets/question_chain_example.png` & `gptty-0.2.6/assets/question_chain_example.png`

 * *Files identical despite different names*

### Comparing `gptty-0.2.5/gptty/__main__.py` & `gptty-0.2.6/gptty/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 gptty: context-preserving chatGPT CLI wrapper
 
 """
 
 __name__ = "gptty"
 __author__ = "Sig Janoska-Bedi"
 __credits__ = ["Sig Janoska-Bedi"]
-__version__ = "0.2.5"
+__version__ = "0.2.6"
 __license__ = "MIT"
 __maintainer__ = "Sig Janoska-Bedi"
 __email__ = "signe@atreeus.com"
 
 # general packages
 import click
 import os
@@ -106,15 +106,15 @@
    \__, / .___/ | |_| |_| |_| |
   /____/_/       \__|\__|\__, |
                           __/ |
                          |___/ 
   """
 
   # Print the text in cyan
-  click.echo(f"{CYAN}{title}\nWelcome to gptty (v.{__version__}), a ChatGPT wrapper in your TTY.\nType :help in the chat interface if you need help getting started.{' Verbose / Debug mode is on.' if verbose else ''}{RESET}\n")
+  click.echo(f"{CYAN}{title}\nWelcome to gptty (v.{__version__}), a ChatGPT wrapper in your TTY. Type :help in the chat interface if you need help getting started.{' Verbose / Debug mode is on. Query prompts will be preceded by your daily API usage in the format (query count, query tokens, response tokens).' if verbose else ''}{RESET}\n")
   
   if not os.path.exists(config_path):
       click.echo(f"{RED}FAILED to access app config file at {config_path}. Are you sure this is a valid config file? Run `gptty chat --help` for more information. You can get a sample config at <https://github.com/signebedi/gptty/blob/master/assets/gptty.ini.example>.")
       return
 
   # load the app configs
   configs = get_config_data(config_file=config_path)
@@ -123,14 +123,20 @@
   if not has_internet_connection(configs['verify_internet_endpoint']):
     click.echo(f"{RED}FAILED to verify connection at {configs['verify_internet_endpoint']}. Are you sure you are connected to the internet?")
     return
 
   # create the output file if it doesn't exist
   with open (configs['output_file'], 'a'): pass
   
+  # Authenticate with OpenAI using your API key
+  # click.echo (configs['api_key'])
+  if configs['api_key'].rstrip('\n') == "":
+      click.echo(f"{RED}FAILED to initialize connection to OpenAI. Have you added an API token? See gptty docs <https://github.com/signebedi/gptty#configuration> or <https://platform.openai.com/account/api-keys> for more information.")
+      return
+
   # Run the main function
   # create_chat_room(configs=configs, config_path=config_path)
   # asyncio.run(create_chat_room(configs=configs, config_path=config_path))
   await create_chat_room(configs=configs, config_path=config_path, verbose=verbose)
 
 
 @click.command()
@@ -148,24 +154,40 @@
   Submit a gptty query
   """
 
   asyncio.run(query_async_wrapper(config_path, question, tag, additional_context, verbose, json, quiet))
 
 
 async def query_async_wrapper(config_path:str, question:str, tag:str, additional_context:str, verbose:bool, json:bool, quiet:bool):
+
+  if not os.path.exists(config_path):
+      click.echo(f"{RED}FAILED to access app config file at {config_path}. Are you sure this is a valid config file? Run `gptty chat --help` for more information.")
+      return
+
   # load the app configs
   configs = get_config_data(config_file=config_path)
 
   # Here, we verify that we have a wifi connection and if not, exit
   if not has_internet_connection(configs['verify_internet_endpoint']):
     click.echo(f"{RED}FAILED to verify connection at {configs['verify_internet_endpoint']}. Are you sure you are connected to the internet?")
     return
+
   # create the output file if it doesn't exist
   with open (configs['output_file'], 'a'): pass
 
+  # Authenticate with OpenAI using your API key
+  # click.echo (configs['api_key'])
+  if configs['api_key'].rstrip('\n') == "":
+      click.echo(f"{RED}FAILED to initialize connection to OpenAI. Have you added an API token? See gptty docs <https://github.com/signebedi/gptty#configuration> or <https://platform.openai.com/account/api-keys> for more information.")
+      return
+
+  if len(questions) < 1 or not isinstance(questions, tuple):
+      click.echo(f"{RED}FAILED to query ChatGPT. Did you forget to ask a question? Run `gptty chat --help` for more information.")
+      return
+
   await run_query(questions=question, tag=tag, configs=configs, additional_context=additional_context, config_path=config_path, verbose=verbose, return_json=json, quiet=quiet)
 
 
 @click.command()
 @click.option('--config_path', '-c', default=os.path.join(os.getcwd(),'gptty.ini'), help="Path to config file.")
 def log(config_path):
   """
@@ -173,14 +195,19 @@
   """
   # load the app configs
   configs = get_config_data(config_file=config_path)
   
   # create the output file if it doesn't exist
   with open (configs['output_file'], 'a'): pass
 
+  if not os.path.exists(config_path):
+      click.echo(f"{RED}FAILED to access app config file at {config_path}. Are you sure this is a valid config file? Run `gptty chat --help` for more information.")
+      return
+
+
   df = return_log_as_df(configs)
 
   click.echo(df)
 
 
 
 main.add_command(chat)
```

### Comparing `gptty-0.2.5/gptty/context.py` & `gptty-0.2.6/gptty/context.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __name__ = "gptty.context"
 __author__ = "Sig Janoska-Bedi"
 __credits__ = ["Sig Janoska-Bedi"]
-__version__ = "0.2.5"
+__version__ = "0.2.6"
 __license__ = "MIT"
 __maintainer__ = "Sig Janoska-Bedi"
 __email__ = "signe@atreeus.com"
 
 
 import click
 import tiktoken
@@ -13,29 +13,46 @@
 from collections import Counter, defaultdict
 from nltk.corpus import stopwords
 
 
 YELLOW = "\033[1;33m"
 RESET = "\033[0m"
 
-def verify_added_phrase(phrase:str,context:str, max_len:int) -> bool:
+def get_token_count(s, model_name):
 
-    if len(context) + len(phrase) <= max_len:
-        return True
+    """
+    Returns the number of tokens in a text string encoded using a specified model.
 
-    return False
+    Args:
+
+        s (str): The input text string.
+        model_name (str): The name of the model used for encoding.
+
+    Returns:
+
+        num_tokens (int): The number of tokens in the encoded text string.
+    """
 
-def get_token_count(s, model_name):
-    """Returns the number of tokens in a text string."""
     encoding = tiktoken.encoding_for_model(model_name)
     num_tokens = len(encoding.encode(s))
     return num_tokens
 
 def return_most_common_phrases(text:str, weight_recent=True) -> list:
 
+    """
+    Returns a list of the most common noun phrases in the input text, with an option to weight more recent phrases more heavily.
+
+    Args:
+    - text (str): The input text.
+    - weight_recent (bool): If True, more recent phrases are weighted more heavily.
+
+    Returns:
+    - list: A list of the most common noun phrases in the input text. Each item in the list is a string representing a noun phrase.
+    """
+
     # Extract noun phrases using TextBlob
     blob = TextBlob(text)
     noun_phrases = blob.noun_phrases
 
     # Remove stopwords from noun phrases
     stop_words = set(stopwords.words('english'))
     filtered_noun_phrases = []
@@ -70,15 +87,49 @@
                 model_name:str, 
                 context_keywords_only: bool = True, 
                 additional_context: str = "",
                 model_type: str = None, 
                 question: str = None, 
                 debug: bool = False):
 
-    # additional_context = additional_context.replace("\n",'')
+
+    """
+    Returns a full query context for a given tag, question and additional context.
+    
+    Parameters:
+        tag: str
+            Tag to identify a conversation with a specific topic
+        max_context_length: int
+            Maximum length of the context to return.
+        output_file: str
+            Path to the file to read the context from.
+        model_name: str
+            Name of the language model to use
+        context_keywords_only: bool, optional
+            If True, use only the most common phrases and words from the context and additional context.
+            Default is True.
+        additional_context: str, optional
+            Additional context to add to the context.
+            Default is an empty string.
+        model_type: str, optional
+            Type of the language model. If 'v1/chat/completions', return a list of dicts with 'role' and 'content' keys
+            If not, return a string.
+            Default is None.
+        question: str, optional
+            Question to add to the context. If None, return only the context.
+            Default is None.
+        debug: bool, optional
+            If True, print debug information.
+            Default is False.
+    
+    Returns:
+        If `model_type` is 'v1/chat/completions', returns a list of dicts with 'role' and 'content' keys
+        If not, returns a string.
+    """
+
 
     if len(tag) < 1:
         if model_type == 'v1/chat/completions':
 
             context = [{"role": "user", "content": question}]
 
             if len(additional_context) > 0:
```

### Comparing `gptty-0.2.5/gptty/gptty.py` & `gptty-0.2.6/gptty/gptty.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __name__ = "gptty.gptty"
 __author__ = "Sig Janoska-Bedi"
 __credits__ = ["Sig Janoska-Bedi"]
-__version__ = "0.2.5"
+__version__ = "0.2.6"
 __license__ = "MIT"
 __maintainer__ = "Sig Janoska-Bedi"
 __email__ = "signe@atreeus.com"
 
 import click
 import openai
 import pandas as pd
@@ -42,34 +42,101 @@
 
                         [Questions]
 `why is the sky blue`                       -   send a question to ChatGPT
 `[shakespeare] who is william shakespeare`  -   share context across conversations
 `[a:b] what is the meaning of life`         -   pass context positionally
 """
 
+
+def usage_stats_today():
+
+    try:
+        r = openai.api_requestor.APIRequestor()
+        resp = r.request("GET", f'/usage?date={datetime.now().strftime("%Y-%m-%d")}')
+        resp_object = resp[0].data
+    except:
+        return None
+    # requests_today = resp_object['data'][0]['n_requests'] # num requests
+    # query_tokens_today = resp_object['data'][0]['n_context_tokens_total'] # query tokens
+    # response_tokens_today = resp_object['data'][0]['n_generated_tokens_total'] # response tokens
+
+    requests_today = sum(item["n_requests"] for item in resp_object['data'])
+    query_tokens_today = sum(item["n_context_tokens_total"] for item in resp_object['data'])
+    response_tokens_today = sum(item["n_generated_tokens_total"] for item in resp_object['data'])
+
+    return requests_today, query_tokens_today, response_tokens_today
+
 ## VALIDATE MODELS - these functions are use to validate the model passed by the user and raises an exception if 
 ## the model does not exist.
 def get_available_models():
+
+    """    
+    Returns:
+        - List: list of available OpenAI model IDs.
+
+    """
+
     response = openai.Model.list()
     return [model.id for model in response['data']]
 
 def is_valid_model(model_name):
+    """
+    Validates whether a given model name is available in the OpenAI platform.
+
+    Parameters:
+    - model_name (str): The name of the model to validate.
+
+    Returns:
+    - bool: True if the model name is available, False otherwise.
+    """
+
     available_models = get_available_models()
     return model_name in available_models
 
 def validate_model_type(model_name):
+
+    """
+    Validates whether a given model name is a supported model type for OpenAI API completion requests.
+
+    Parameters:
+    - model_name (str): The name of the model to validate.
+
+    Returns:
+    - str: The API endpoint to use for completion requests if the model name is valid and supported.
+
+    Raises:
+    - Exception: If the model name is not valid or not supported.
+    """
+
     if ('davinci' in model_name or 'curie' in model_name) and is_valid_model(model_name):
         return 'v1/completions'
     elif 'gpt' in model_name and is_valid_model(model_name):
         return 'v1/chat/completions'
     raise Exception()
 
 # here we define the async call to the openai API that is used when running queries
 async def fetch_response(prompt, model_engine, max_tokens, temperature, model_type):
 
+    """
+    This module provides a function to fetch a response from the OpenAI API based on the given prompt and model specifications.
+
+    Parameters:
+    - prompt (str): The prompt to use for the API request.
+    - model_engine (str): The engine ID to use for the API request.
+    - max_tokens (int): The maximum number of tokens to generate in the response.
+    - temperature (float): The temperature to use for the API request.
+    - model_type (str): The API endpoint to use for the API request.
+
+    Returns:
+    - OpenAICompletion: The completion response object from the OpenAI API.
+
+    Raises:
+    - Exception: If the model type is not recognized or supported.
+    """
+
     if model_type == 'v1/completions':
 
         return await openai.Completion.acreate(
             engine=model_engine,
             prompt=prompt,
             max_tokens=max_tokens,
             temperature=temperature,
@@ -94,45 +161,66 @@
 
     click.echo(f"\n{RED}FAILED to validate the model type '{model_type}'. Are you sure this is a valid OpenAI model endpoint? Check the available model endpoints at <https://platform.openai.com/docs/models/model-endpoint-compatibility>. If you believe this is a bug, submit a bug request at <https://github.com/signebedi/gptty/issues>.{RESET}\n")
     return None
 
 
 # here we design the wait graphic that is called while awaiting responses
 async def wait_graphic():
+
+    """
+    This module provides a function to display a wait graphic while awaiting responses.
+
+    Returns:
+    - None
+    """
+
     while True:
         # for i in range(1, 11):
         #     print("." * i + " " * (9 - i), end="", flush=True)
         #     await asyncio.sleep(0.1)
         #     print("\b" * 10, end="", flush=True)
 
         # Show the waiting graphic
         for i in range(10):
             print("." * i + " " * (9 - i), end="", flush=True)
             await asyncio.sleep(0.1)
             print("\b" * 10, end="", flush=True)
 
+
+
 # this is used when we run the `chat` command
 async def create_chat_room(configs=get_config_data(), log_responses:bool=True, config_path=None, verbose:bool=False):
 
-    # Authenticate with OpenAI using your API key
-    # click.echo (configs['api_key'])
-    if configs['api_key'].rstrip('\n') == "":
-        click.echo(f"{RED}FAILED to initialize connection to OpenAI. Have you added an API token? See gptty docs <https://github.com/signebedi/gptty#configuration> or <https://platform.openai.com/account/api-keys> for more information.")
-        return
+    """
+    This function creates a chat room using the OpenAI API to generate responses to user inputs. 
+    The user input is prompted and the response is displayed on the console. 
+    The chat session is continuously open until the user enters ':quit' or ':q' to terminate the session. 
+    The session log is stored in a csv file. 
+    
+    Parameters:
+    - configs: A dictionary containing OpenAI API key, model name, temperature, max_tokens, max_context_length, context_keywords_only, preserve_new_lines, gpt_name and your_name.
+    - log_responses: A boolean indicating whether or not to log the responses in a csv file. Default is True.
+    - config_path: The path to the configuration file.
+    - verbose: A boolean indicating whether or not to print debugging information. Default is False.
+
+    Returns:
+    - None
+    """
+
 
     # here we add a pandas df reference object, see 
     # https://github.com/signebedi/gptty/issues/15
     try:
         df = pd.read_csv(configs['output_file'], header=None,sep='|').fillna('')
         df.columns = ['timestamp','tag','question','response']
     except:
         df = pd.DataFrame(columns=['timestamp','tag','question','response'])
 
     try:
-
+        openai.organization = configs['org_id'].rstrip('\n')
         openai.api_key = configs['api_key'].rstrip('\n')
     except:
         click.echo(f"{RED}FAILED to initialize connection to OpenAI. Have you added an API token? See gptty docs <https://github.com/signebedi/gptty#configuration> or <https://platform.openai.com/account/api-keys> for more information.")
         return
 
     # Set the parameters for the OpenAI completion API
     model_engine = configs['model'].rstrip('\n')
@@ -150,17 +238,18 @@
 
     # Continuously send and receive messages
     while True:
 
         # Get user input
         try:
 
+
             with patch_stdout():
-                i = await session.prompt_async(ANSI(f"{CYAN}> "), style=Style.from_dict({'': 'ansicyan'}))
-            print(f"{ERASE_LINE}{MOVE_CURSOR_UP}{GREY}> {i}\n", end="")
+                i = await session.prompt_async(ANSI(f"{CYAN}{usage_stats_today() if verbose else ''}> "), style=Style.from_dict({'': 'ansicyan'}))
+            print(f"{ERASE_LINE}{MOVE_CURSOR_UP}{GREY}{usage_stats_today() if verbose else ''}> {i}\n", end="")
 
             # i = await ainput(f"{CYAN}> ")
             tag,question = get_tag_from_text(i)
             prompt_length = len(question)
 
         # handle keyboard interrupt
         except KeyboardInterrupt:
@@ -226,27 +315,40 @@
 
 
 
 
 # this is used when we run the `query` command
 async def run_query(questions:list, tag:str, configs=get_config_data(), additional_context:str="", log_responses:bool=True, config_path=None, verbose:bool=False, return_json:bool=False, quiet:bool=False):
 
-    if not os.path.exists(config_path):
-        click.echo(f"{RED}FAILED to access app config file at {config_path}. Are you sure this is a valid config file? Run `gptty chat --help` for more information.")
-        return
-
-    # Authenticate with OpenAI using your API key
-    # click.echo (configs['api_key'])
-    if configs['api_key'].rstrip('\n') == "":
-        click.echo(f"{RED}FAILED to initialize connection to OpenAI. Have you added an API token? See gptty docs <https://github.com/signebedi/gptty#configuration> or <https://platform.openai.com/account/api-keys> for more information.")
-        return
+    """
+    This function is used to run a query command using OpenAI. 
+    It takes in a list of questions, a tag, additional context, and various configuration options. 
+    It authenticates with OpenAI using the API key specified in the configuration file, and then continuously sends and receives messages until all the questions 
+    have been answered. The responses are either printed to the console in color or returned in a JSON format, depending on the options specified. Additionally, 
+    the function logs the questions and responses in a pandas dataframe if specified in the configuration file.
+
+    Parameters:
+        questions (list): a list of questions to ask the GPT-3 model
+        tag (str): a tag to associate with the questions and responses
+        configs (dict): a dictionary containing configuration options (default: get_config_data())
+        additional_context (str): additional context to provide to the GPT-3 model (default: "")
+        log_responses (bool): whether to log the questions and responses in a pandas dataframe (default: True)
+        config_path (str): the path to the configuration file (default: None)
+        verbose (bool): whether to enable debug mode (default: False)
+        return_json (bool): whether to return the responses in a JSON format (default: False)
+        quiet (bool): whether to suppress console output (default: False)
+
+    Returns:
+        None if the function fails to authenticate with OpenAI or if there are no questions to ask
+        if return_json is True and quiet is False, prints a JSON representation of the question/response data to the console and returns None
+        if return_json is True and quiet is True, returns a JSON representation of the question/response data
+        if return_json is False and quiet is False, prints the responses to the console in color and returns None
+        if return_json is False and quiet is True, returns None
+    """
 
-    if len(questions) < 1 or not isinstance(questions, tuple):
-        click.echo(f"{RED}FAILED to query ChatGPT. Did you forget to ask a question? Run `gptty chat --help` for more information.")
-        return
 
     # here we add a pandas df reference object, see 
     # https://github.com/signebedi/gptty/issues/15
     try:
         df = pd.read_csv(configs['output_file'], header=None,sep='|').fillna('')
         df.columns = ['timestamp','tag','question','response']
     except:
```

### Comparing `gptty-0.2.5/gptty/tagging.py` & `gptty-0.2.6/gptty/tagging.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,70 +1,83 @@
 
 __name__ = "gptty.tagging"
 __author__ = "Sig Janoska-Bedi"
 __credits__ = ["Sig Janoska-Bedi"]
-__version__ = "0.2.5"
+__version__ = "0.2.6"
 __license__ = "MIT"
 __maintainer__ = "Sig Janoska-Bedi"
 __email__ = "signe@atreeus.com"
 
-def old_get_tag_from_text(user_input, replacement_string='-'):
+# def old_get_tag_from_text(user_input, replacement_string='-'):
 
-    # Initialize the tag and remaining text variables
-    tag = None
-    remaining_text = user_input.strip()
+#     # Initialize the tag and remaining text variables
+#     tag = None
+#     remaining_text = user_input.strip()
+
+#     # Loop until we find a tag or run out of text
+#     while tag is None and remaining_text != "":
+#         # Remove leading whitespace and get the first word
+#         first_word = remaining_text.lstrip().split()[0]
+
+#         # Check if the first word starts with '['
+#         if first_word.startswith('['):
+#             # Check if the first word ends with ']'
+#             if first_word.endswith(']'):
+#                 # Get the tag by removing the '[' and ']' characters
+#                 tag = first_word[1:-1].replace(" ", replacement_string)
+
+#                 # Strip the tag from the remaining text and remove any extra whitespace
+#                 remaining_text = remaining_text[len(first_word):].strip()
+#             else:
+#                 # The first word doesn't end with ']', so keep appending words to the tag until we find one that does
+#                 tag = first_word[1:].replace(" ", replacement_string)
+#                 remaining_text = remaining_text[len(first_word):].lstrip()
+
+#                 while "]" not in tag and remaining_text != "":
+#                     # Append the next word to the tag
+#                     next_word = remaining_text.lstrip().split()[0]
+#                     tag += replacement_string+next_word.replace(" ", replacement_string)
+#                     remaining_text = remaining_text[len(next_word):].lstrip()
+
+#                 # If we found the end of the tag, remove it from the remaining text
+#                 if "]" in tag:
+#                     # Remove the ']' character from the tag and strip any extra whitespace
+#                     tag = tag[:-1].strip()
+
+#                     # Remove the tag from the remaining text and remove any extra whitespace
+#                     remaining_text = remaining_text[len(tag) + 2:].strip()
+#                 else:
+#                     # We ran out of text before finding the end of the tag
+#                     tag = None
+#         else:
+#             # The text doesn't start with a tag
+#             tag = None
+#             break
+
+#     # Output the tag and remaining text, if we found a tag, as a tuple
+#     if tag is not None:
+#         return tag,remaining_text
+#     else:
+#         return '',remaining_text
 
-    # Loop until we find a tag or run out of text
-    while tag is None and remaining_text != "":
-        # Remove leading whitespace and get the first word
-        first_word = remaining_text.lstrip().split()[0]
 
-        # Check if the first word starts with '['
-        if first_word.startswith('['):
-            # Check if the first word ends with ']'
-            if first_word.endswith(']'):
-                # Get the tag by removing the '[' and ']' characters
-                tag = first_word[1:-1].replace(" ", replacement_string)
-
-                # Strip the tag from the remaining text and remove any extra whitespace
-                remaining_text = remaining_text[len(first_word):].strip()
-            else:
-                # The first word doesn't end with ']', so keep appending words to the tag until we find one that does
-                tag = first_word[1:].replace(" ", replacement_string)
-                remaining_text = remaining_text[len(first_word):].lstrip()
-
-                while "]" not in tag and remaining_text != "":
-                    # Append the next word to the tag
-                    next_word = remaining_text.lstrip().split()[0]
-                    tag += replacement_string+next_word.replace(" ", replacement_string)
-                    remaining_text = remaining_text[len(next_word):].lstrip()
-
-                # If we found the end of the tag, remove it from the remaining text
-                if "]" in tag:
-                    # Remove the ']' character from the tag and strip any extra whitespace
-                    tag = tag[:-1].strip()
-
-                    # Remove the tag from the remaining text and remove any extra whitespace
-                    remaining_text = remaining_text[len(tag) + 2:].strip()
-                else:
-                    # We ran out of text before finding the end of the tag
-                    tag = None
-        else:
-            # The text doesn't start with a tag
-            tag = None
-            break
-
-    # Output the tag and remaining text, if we found a tag, as a tuple
-    if tag is not None:
-        return tag,remaining_text
-    else:
-        return '',remaining_text
+def get_tag_from_text(user_input, replacement_string='-'):
 
+    """
+    This function takes a user input and returns the first tag found within square brackets along with the remaining text after the tag. The square brackets are removed from the tag and any spaces within the tag are replaced with the provided replacement string. If no tag is found, an empty string is returned as the tag.
 
-def get_tag_from_text(user_input, replacement_string='-'):
+    Parameters:
+
+        user_input (str): The input string to search for a tag.
+        replacement_string (str): The string to replace any spaces within the tag. Defaults to '-' if no replacement string is provided.
+
+    Returns:
+
+        Tuple: A tuple containing the tag (str) and the remaining text after the tag (str). If no tag is found, the tag will be an empty string.
+    """
 
     tag = None
     remaining_text = user_input.strip()
 
     while tag is None and remaining_text != "":
         first_word = remaining_text.lstrip().split()[0]
```

### Comparing `gptty-0.2.5/gptty.egg-info/PKG-INFO` & `gptty-0.2.6/gptty.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: gptty
-Version: 0.2.5
+Version: 0.2.6
 Summary: Chat GPT wrapper in your TTY 
 Home-page: https://github.com/signebedi/gptty
 Author: Sig Janoska-Bedi
 Author-email: signe@atreeus.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gptty
 
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/signebedi/gptty/blob/master/LICENSE) 
+[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/signebedi/gptty/blob/master/LICENSE) 
 [![PyPI version](https://badge.fury.io/py/gptty.svg)](https://pypi.python.org/pypi/gptty)
 [![Downloads](https://static.pepy.tech/badge/gptty)](https://pepy.tech/project/gptty)
-[![gptty tests](https://github.com/signebedi/gptty/workflows/Tests/badge.svg)](https://github.com/signebedi/gptty/actions)
+[![gptty tests](https://github.com/signebedi/gptty/workflows/tests/badge.svg)](https://github.com/signebedi/gptty/actions)
 
 ChatGPT wrapper in your TTY
 
 ## About
 
 gptty is a ChatGPT shell interface that allows you to (1) interact with ChatGPT in a manner similar to the web application, but without needing to rely on the web application's stability; (2) preserve context across chat sessions and structure your conversations however you want; (3) save local copies of your conversations for easy reference.
 
@@ -65,15 +65,16 @@
 
 ## Configuration
 
 `gptty` reads configuration settings from a file named `gptty.ini`, which the app expects to be located in the same directory that you are running `gptty` from unless you pass a custom `config_file`. The file uses the INI file format, which consists of sections, each with its own key-value pairs.
 
 | Key    | Type | Default Value    | Description |
 | -------- | ------- | -------- | ------- |
-| api_key  | String    | ""  |   The API key for OpenAI's GPT service  |
+| api_key  | String    | ""  |   Your API key for OpenAI's GPT service  |
+| org_id  | String    | ""  |   Your organization ID for OpenAI's GPT service  |
 | your_name    | String    | "question"    |   The name of the input prompt  |
 | gpt_name  | String    | "response"  |   The name of the generated response  |
 | output_file | String     | "output.txt" |    The name of the file where the output will be saved  |
 | model    | String    | "text-davinci-003"    |   The name of the GPT model to use  |
 | temperature  | Float    | 0.0  |   The temperature to use for sampling  |
 | max_tokens | Integer     | 250 |    The maximum number of tokens to generate for the response  |
 | max_context_length    | Integer    | 150    |   The maximum length of the input context  |
@@ -114,14 +115,15 @@
 
 To use a command, simply type it into the command prompt and press Enter. For example, use the following command to display the current configuration settings in the terminal:
 
 ```
 > :configs
 
 api_key: SOME_CONFIG_HERE
+org_id: org-SOME_CHARS_HERE
 your_name: question
 gpt_name: response
 output_file: output.txt
 model: text-davinci-003
 temperature: 0.0
 max_tokens: 250
 max_context_length: 5000
```

### Comparing `gptty-0.2.5/setup.py` & `gptty-0.2.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     DESCRIPTION = f.read()
 
 with open('requirements.txt') as f:
     REQUIRED = f.read().splitlines()
 
 setup(
     name='gptty',
-    version="0.2.5",
+    version="0.2.6",
     description='Chat GPT wrapper in your TTY ',
     author='Sig Janoska-Bedi',
     author_email='signe@atreeus.com',
     long_description=DESCRIPTION, 
     long_description_content_type='text/markdown',
     url="https://github.com/signebedi/gptty",
     packages=['gptty'],
```

### Comparing `gptty-0.2.5/tests/test_config.py` & `gptty-0.2.6/tests/test_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 class TestConfig(unittest.TestCase):
 
     # Test the default configuration values
     def test_default_config(self):
         default_config_data = get_config_data('test/test_default_gptty.ini')
         self.assertEqual(default_config_data['api_key'], "")
+        self.assertEqual(default_config_data['org_id'], "")
         self.assertEqual(default_config_data['your_name'], 'question')
         self.assertEqual(default_config_data['gpt_name'], 'response')
         self.assertEqual(default_config_data['output_file'], 'output.txt')
         self.assertEqual(default_config_data['model'], 'text-davinci-003')
         self.assertEqual(default_config_data['temperature'], 0.0)
         self.assertEqual(default_config_data['max_tokens'], 25)
         self.assertEqual(default_config_data['max_context_length'], 150)
         self.assertEqual(default_config_data['context_keywords_only'], True)
         self.assertEqual(default_config_data['preserve_new_lines'], False)
 
     # Test with a custom configuration file
     def test_custom_config(self):
         custom_config_data = get_config_data(config_file='tests/test_gptty.ini')
         self.assertEqual(custom_config_data['api_key'], "ANOTHER_KEY_HERE")
+        self.assertEqual(custom_config_data['org_id'], "org-536JCU1SlmsQZB0i734dCsGC")
         self.assertEqual(custom_config_data['your_name'], 'custom_question')
         self.assertEqual(custom_config_data['gpt_name'], 'custom_response')
         self.assertEqual(custom_config_data['output_file'], 'custom_output.txt')
         self.assertEqual(custom_config_data['model'], 'text-curie-003')
         self.assertEqual(custom_config_data['temperature'], 0.5)
         self.assertEqual(custom_config_data['max_tokens'], 300)
         self.assertEqual(custom_config_data['max_context_length'], 200)
```

### Comparing `gptty-0.2.5/tests/test_context.py` & `gptty-0.2.6/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `gptty-0.2.5/tests/test_tagging.py` & `gptty-0.2.6/tests/test_tagging.py`

 * *Files identical despite different names*

