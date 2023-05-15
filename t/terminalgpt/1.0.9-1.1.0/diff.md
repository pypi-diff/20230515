# Comparing `tmp/terminalgpt-1.0.9.tar.gz` & `tmp/terminalgpt-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminalgpt-1.0.9.tar", max compression
+gzip compressed data, was "terminalgpt-1.1.0.tar", max compression
```

## Comparing `terminalgpt-1.0.9.tar` & `terminalgpt-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1070 2023-03-21 18:01:34.353070 terminalgpt-1.0.9/LICENSE
--rw-r--r--   0        0        0     3395 2023-03-31 14:16:15.983658 terminalgpt-1.0.9/README.md
--rw-r--r--   0        0        0      779 2023-03-31 14:16:15.984032 terminalgpt-1.0.9/pyproject.toml
--rw-r--r--   0        0        0       66 2023-03-11 15:11:43.240080 terminalgpt-1.0.9/terminalgpt/.gitattributes
--rw-r--r--   0        0        0        0 2023-03-11 15:11:43.240200 terminalgpt-1.0.9/terminalgpt/__init__.py
--rw-r--r--   0        0        0     6878 2023-03-31 14:16:15.984259 terminalgpt-1.0.9/terminalgpt/chat_utils.py
--rw-r--r--   0        0        0     2800 2023-03-31 14:16:15.984397 terminalgpt-1.0.9/terminalgpt/config.py
--rw-r--r--   0        0        0     2440 2023-03-31 11:16:37.570616 terminalgpt-1.0.9/terminalgpt/conversations.py
--rw-r--r--   0        0        0     1479 2023-03-21 17:20:53.535542 terminalgpt-1.0.9/terminalgpt/encryption.py
--rw-r--r--   0        0        0     7057 2023-03-31 14:16:15.984537 terminalgpt-1.0.9/terminalgpt/main.py
--rw-r--r--   0        0        0     3134 2023-03-31 11:16:37.571044 terminalgpt-1.0.9/terminalgpt/print_utils.py
--rw-r--r--   0        0        0     4253 1970-01-01 00:00:00.000000 terminalgpt-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-03-21 18:01:34.353070 terminalgpt-1.1.0/LICENSE
+-rw-r--r--   0        0        0     4104 2023-05-15 13:33:16.882545 terminalgpt-1.1.0/README.md
+-rw-r--r--   0        0        0      892 2023-05-15 13:33:34.078516 terminalgpt-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       66 2023-03-11 15:11:43.240080 terminalgpt-1.1.0/terminalgpt/.gitattributes
+-rw-r--r--   0        0        0        0 2023-03-11 15:11:43.240200 terminalgpt-1.1.0/terminalgpt/__init__.py
+-rw-r--r--   0        0        0     7564 2023-05-15 13:32:22.775984 terminalgpt-1.1.0/terminalgpt/chat_utils.py
+-rw-r--r--   0        0        0     2839 2023-05-15 13:32:22.776237 terminalgpt-1.1.0/terminalgpt/config.py
+-rw-r--r--   0        0        0     2617 2023-05-15 13:32:22.776448 terminalgpt-1.1.0/terminalgpt/conversations.py
+-rw-r--r--   0        0        0     1601 2023-04-05 00:33:46.085427 terminalgpt-1.1.0/terminalgpt/encryption.py
+-rw-r--r--   0        0        0     8373 2023-05-15 13:32:22.776677 terminalgpt-1.1.0/terminalgpt/main.py
+-rw-r--r--   0        0        0     4856 2023-05-15 13:32:22.776853 terminalgpt-1.1.0/terminalgpt/print_utils.py
+-rw-r--r--   0        0        0     5119 1970-01-01 00:00:00.000000 terminalgpt-1.1.0/PKG-INFO
```

### Comparing `terminalgpt-1.0.9/LICENSE` & `terminalgpt-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `terminalgpt-1.0.9/README.md` & `terminalgpt-1.1.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # ![TerminalGPT](logo.png)
 
-[![Continuous Integration](https://github.com/adamyodinsky/TerminalGPT/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/adamyodinsky/TerminalGPT/actions/workflows/main.yml) ![PyPI](https://img.shields.io/pypi/v/terminalgpt) ![PyPI - Downloads](https://img.shields.io/pypi/dm/terminalgpt) ![commits-since](https://img.shields.io/github/commits-since/adamyodinsky/TerminalGPT/latest) ![GitHub last commit](https://img.shields.io/github/last-commit/adamyodinsky/terminalgpt)
+[![Continuous Integration](https://github.com/adamyodinsky/TerminalGPT/actions/workflows/MainCI.yml/badge.svg?branch=main)](https://github.com/adamyodinsky/TerminalGPT/actions/workflows/main.yml) ![PyPI](https://img.shields.io/pypi/v/terminalgpt) ![PyPI - Downloads](https://img.shields.io/pypi/dm/terminalgpt) ![commits-since](https://img.shields.io/github/commits-since/adamyodinsky/TerminalGPT/latest) ![GitHub last commit](https://img.shields.io/github/last-commit/adamyodinsky/terminalgpt)
 
 Welcome to terminalGPT, the terminal-based ChatGPT personal assistant app!
-With terminalGPT, you can easily interact with the OpenAI GPT 3.5 language model.
+With terminalGPT, you can easily interact with the OpenAI GPT-3.5 and GPT-4 language models.
 
 Whether you need help with a quick question or want to explore a complex topic, TerminalGPT is here to assist you. Simply enter your query and TerminalGPT will provide you with the best answer possible based on its extensive knowledge base.
 
 ---
 
-![Alt Text](./usage.gif)
+<img width="910" alt="image" src="https://user-images.githubusercontent.com/27074934/229319537-f332923d-f92e-4d91-8d5e-d26d8997341e.png">
 
 ---
 
 ## Why?
 
 Some advantages of using TerminalGPT over the chatGPT browser-based app:
 
@@ -24,25 +24,30 @@
 - TerminalGPT's answers are tailored to your machine's operating system, distribution, and chip-set architecture
 - Doesn't use your conversation data for training the model (unlike the browser-based app).
 - Your conversations are stored locally on your machine, so only you can access them.
 
 ## Pre-requisites
 
 - Python 3.6 or higher
-- An OpenAI Account and API key (It's free for personal use).
+- An OpenAI Account and API key.
    1. Sign up at <https://beta.openai.com/signup> using email or Google/Microsoft account.
    2. Go to <https://beta.openai.com/account/api-keys> or click on "View API keys" in the menu to get your API key.
-   For a more detailed guide on how to create an OpenAI API key, click [here](https://elephas.app/blog/how-to-create-openai-api-keys-cl5c4f21d281431po7k8fgyol0).
+
+**Notes:** OpenAI FREE API trial expired on 01-04-2023. You can still use the API, but you will need to set up a payment method.
+
+- To set up a payment method [click here](https://platform.openai.com/account/billing/payment-methods).
+- To check your usage [click here](https://platform.openai.com/account/usage).
+- To check pricing [click here](https://openai.com/pricing#language-models).
 
 ## Installation
 
 1. Install the latest TerminalGPT with pip install.
 
 ```sh
-pip install terminalgpt -U
+pip install terminalgpt -U --user
 ```
 
 2. Now you have `terminalgpt` command available in your terminal. Run the following install command to configure the app.
 
 ```sh
 terminalgpt install
 ```
@@ -51,35 +56,53 @@
 
 That's it! You're ready to use TerminalGPT!
 
 ---
 
 ## Usage
 
+### TL;DR
+
 ```sh
-Usage: terminalgpt [OPTIONS] COMMAND [ARGS]...
+Usage: main.py [OPTIONS] COMMAND [ARGS]...
+
+  *~ TerminalGPT - Your Personal Terminal Assistant ~*
 
 Options:
-  --help                 Show this message and exit.
+  --version                       Show the version and exit.
+  -m, --model [gpt-3.5-turbo|gpt-4]
+                                  Choose a model to use.  [default:
+                                  gpt-3.5-turbo]
+  -p, --plain                     Plain text output.
+  --help                          Show this message and exit.
 
 Commands:
-  new      Start a new conversation.
-  load     Choose a previous conversation to load.
-  delete   Choose a previous conversation to load.
-  install  Creating a secret api key for the chatbot.
+  delete    Choose a previous conversation to load.
+  install   Creating a secret api key for the chatbot.
+  load      Choose a previous conversation to load.
+  new       Start a new conversation.
+  one-shot  One shot question answer.
 ```
 
 ### New
 
 Start a new conversation:
 
 ```sh
 terminalgpt new
 ```
 
+### One-Shot
+
+One shot question to get a fast answer in the terminal.
+
+```sh
+terminalgpt one-shot "What is the meaning of life?"
+```
+
 ### Load
 
 Load previous conversations:
 
 ```sh
 terminalgpt load
 ```
@@ -92,14 +115,12 @@
 terminalgpt delete
 ```
 
 ---
 
 ## Future Plans
 
-1. Support multiline input.
-2. Support optional vim input mode.
-3. Auto-completion for all commands.
-4. Open source the project.
-5. Add more models (???)
-6. Encrypt the conversation data.
-7. Migrating to [Typer](https://typer.tiangolo.com/)
+1. Support optional Vim input mode.
+2. Auto-completion for all commands.
+3. Support local models
+
+---
```

### Comparing `terminalgpt-1.0.9/terminalgpt/chat_utils.py` & `terminalgpt-1.1.0/terminalgpt/chat_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,27 +7,29 @@
 import openai
 import tiktoken
 from colorama import Back, Fore, Style
 from prompt_toolkit import PromptSession
 from yaspin import yaspin
 from yaspin.spinners import Spinners
 
-from terminalgpt import config, conversations, print_utils
+from terminalgpt import config, conversations, encryption, print_utils
 
 TIKTOKEN_ENCODER = tiktoken.get_encoding(config.ENCODING_MODEL)
 
 
 def chat_loop(
-    conversation_name: str = None,
+    conversation_name: str = "",
     **kwargs,
 ):
     """Main chat loop."""
     token_limit: int = kwargs["token_limit"]
     session: PromptSession = kwargs["session"]
     messages: list = kwargs["messages"]
+    model: str = kwargs["model"]
+    plain: bool = kwargs["plain"]
 
     while True:
         # Get user input
 
         # user_input = click.edit() # can edit at vim
         user_input = session.prompt()
         print()
@@ -42,37 +44,43 @@
                 messages=messages,
                 total_usage=total_usage,
                 token_limit=token_limit,
             )
 
         # Get answer
         try:
-            answer = get_user_answer(messages)
+            answer = get_user_answer(messages, model)
         except KeyboardInterrupt:
             print(Style.BRIGHT + "Assistant:" + Style.RESET_ALL)
             stopped_message = print_utils.choose_random_message()
             print_utils.print_slowly(Fore.YELLOW + stopped_message + Style.RESET_ALL)
             continue
+        except Exception as error:  # pylint: disable=broad-except
+            print(Style.BRIGHT + "Assistant:" + Style.RESET_ALL)
+            print_utils.print_slowly(
+                Back.RED + Style.BRIGHT + str(error) + Style.RESET_ALL
+            )
+            continue
 
         # Parse total_usage and message from answer
         total_usage = answer["usage"]["total_tokens"]
         message = answer["choices"][0]["message"]["content"]
 
         # Append to messages list for next iteration keeping context
         messages.append({"role": "assistant", "content": message})
 
         # Save context wait for some context
         if not conversation_name and total_usage > token_limit / 10:
             conversation_name = conversations.create_conversation_name(messages)
         elif conversation_name:
-            conversations.save_conversation(messages, conversation_name)
+            conversations.save_conversation(messages, f"{conversation_name}-{model}")
 
         # Print answer message
         print(Style.BRIGHT + "Assistant:" + Style.RESET_ALL)
-        print_utils.print_slowly(Fore.YELLOW + message + Style.RESET_ALL)
+        print_utils.print_assistance_message(message, plain)
 
         # Print usage
         if os.environ.get("LOG_LEVEL") == "DEBUG":
             print(
                 Fore.LIGHTBLUE_EX
                 + f"\nAPI Total Usage: {str(total_usage)} tokens"
                 + Style.RESET_ALL
@@ -83,51 +91,46 @@
                 + Style.RESET_ALL
             )
 
         if user_input == "exit":
             sys.exit()
 
 
-def get_user_answer(messages):
+def get_user_answer(messages, model):
     """Returns the answer from OpenAI API."""
 
     while True:
-        with yaspin(
-            Spinners.earth,
-            text=Style.BRIGHT + "Assistant:" + Style.RESET_ALL,
-            color="blue",
-            side="right",
-        ):
-            try:
-                answer = openai.ChatCompletion.create(
-                    model=config.MODEL, messages=messages
-                )
+        try:
+            with yaspin(
+                Spinners.earth,
+                text=Style.BRIGHT + "Assistant:" + Style.RESET_ALL,
+                color="blue",
+                side="right",
+            ):
+                answer = openai.ChatCompletion.create(model=model, messages=messages)
                 return answer
-            except openai.error.RateLimitError as error:
-                print_utils.print_slowly(
-                    Back.RED + Style.BRIGHT + str(error) + Style.RESET_ALL
-                )
-                waiting_before_trying_again()
-            except openai.error.InvalidRequestError as error:
-                if "Please reduce the length of the messages" in str(error):
-                    messages.pop(1)
-                else:
-                    raise error
+        except openai.InvalidRequestError as error:
+            if "Please reduce the length of the messages" in str(error):
+                messages.pop(1)
+                time.sleep(0.5)
+            else:
+                raise error
 
 
 def exceeding_token_limit(total_usage: int, token_limit: int):
     """Returns True if the total_usage is greater than the token limit with some safe buffer."""
 
     return total_usage > token_limit
 
 
 def reduce_tokens(messages: list, token_limit: int, total_usage: int):
     """Reduce tokens in messages context."""
 
     reduce_amount = total_usage - token_limit
+    tokenized_message = []
     while exceeding_token_limit(total_usage, token_limit):
         message = messages.pop(1)
         tokenized_message = TIKTOKEN_ENCODER.encode(message["content"])
 
         while reduce_amount > 0 and len(tokenized_message) > 0:
             total_usage -= 1
             reduce_amount -= 1
@@ -168,36 +171,47 @@
     for message in messages:
         num_tokens += (
             4  # every message follows <im_start>{role/name}\n{content}<im_end>\n
         )
         for key, value in message.items():
             num_tokens += len(encoding.encode(value))
             if key == "name":  # if there's a name, the role is omitted
-                num_tokens += -1  # role is always required and always 1 token
+                num_tokens -= 1  # role is always required and always 1 token
     num_tokens -= 2  # every reply is primed with <im_start>assistant
     return num_tokens
 
 
-def waiting_before_trying_again(wait_time: int = 10):
-    """Waits for a given time before trying again."""
-
-    with yaspin() as spinner:
-        for i in range(wait_time):
-            spinner.text = (
-                Style.BRIGHT + f"Trying again in {wait_time - i}" + Style.RESET_ALL
-            )
-            spinner.color = "red"
-            time.sleep(1)
-
-
 # pylint: disable=W0102, W0621
 def welcome_message(messages: list):
     """Prints the welcome message."""
 
     print()
-    welcome_message = get_user_answer(messages)
-    print(Style.BRIGHT + "\nAssistant:" + Style.RESET_ALL)
-    print_utils.print_slowly(
-        Fore.YELLOW
-        + welcome_message["choices"][0]["message"]["content"]
-        + Style.RESET_ALL
-    )
+    try:
+        welcome_message = get_user_answer(messages, config.DEFAULT_MODEL)
+        print(Style.BRIGHT + "\nAssistant:" + Style.RESET_ALL)
+        print_utils.print_markdown_slowly(
+            welcome_message["choices"][0]["message"]["content"]
+        )
+    except KeyboardInterrupt:
+        print(Style.BRIGHT + "Assistant:" + Style.RESET_ALL)
+        stopped_message = print_utils.choose_random_message(
+            print_utils.STOPPED_MESSAGES
+        )
+        print_utils.print_markdown_slowly(
+            Fore.YELLOW + stopped_message + Style.RESET_ALL
+        )
+        sys.exit(0)
+    except Exception as error:  # pylint: disable=W0718
+        print(Style.BRIGHT + "Assistant:" + Style.RESET_ALL)
+        print_utils.print_slowly(Back.RED + Style.BRIGHT + str(error) + Style.RESET_ALL)
+        sys.exit(1)
+
+
+def set_api_key():
+    """Sets the API key for OpenAI API."""
+
+    if os.environ.get("OPENAI_API_KEY"):
+        openai.api_key = os.environ.get("OPENAI_API_KEY")
+    else:
+        encryption.check_api_key()
+        key = encryption.get_encryption_key(config.KEY_PATH)
+        openai.api_key = encryption.decrypt(config.SECRET_PATH, key)
```

### Comparing `terminalgpt-1.0.9/terminalgpt/config.py` & `terminalgpt-1.1.0/terminalgpt/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,25 +21,26 @@
 def machine_info():
     """Get the current machine info."""
 
     return platform.platform()
 
 
 APP_NAME = "terminalgpt"
-API_TOKEN_LIMIT = 4096
-SAFETY_BUFFER = 1024
+DEFAULT_API_TOKEN_LIMIT = 4096
 
 BASE_PATH = f"~/.{APP_NAME}".replace("~", path.expanduser("~"))
 CONVERSATIONS_PATH = f"{BASE_PATH}/conversations"
 SECRET_PATH = f"{BASE_PATH}/{APP_NAME}.encrypted"
 KEY_PATH = f"{BASE_PATH}/{APP_NAME}.key"
 
-MODEL = "gpt-3.5-turbo-0301"
+DEFAULT_MODEL = "gpt-3.5-turbo"
 ENCODING_MODEL = "cl100k_base"
 
+MODELS = {"gpt-3.5-turbo": 4096, "gpt-4": 8092}
+
 INIT_SYSTEM_MESSAGE = {
     "role": "system",
     "content": f"""
 - Your name is "TerminalGPT".
 - You are a helpful personal assistant for programers.
 - You are running on {machine_info()} machine.
 - Please note that your answers will be displayed on the terminal.
```

### Comparing `terminalgpt-1.0.9/terminalgpt/conversations.py` & `terminalgpt-1.1.0/terminalgpt/conversations.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,35 +25,43 @@
 
 
 def save_conversation(
     messages: list, file_name: str, path: str = config.CONVERSATIONS_PATH
 ):
     """Saves a conversation to a file."""
 
+    if not os.path.exists(path):
+        os.makedirs(path)
+
     with open(file=f"{path}/{file_name}", mode="w", encoding="utf-8") as conv_file:
         json.dump(messages, conv_file)
 
 
 def delete_conversation(conversation, path: str = config.CONVERSATIONS_PATH):
     """Deletes a conversation from a file."""
 
     os.remove(f"{path}/{conversation}")
 
 
 def load_conversation(file_name: str, path=config.CONVERSATIONS_PATH) -> list:
     """Loads a conversation from a file. returns a list of messages."""
 
+    messages = []
+
     try:
         with open(file=f"{path}/{file_name}", mode="r", encoding="utf-8") as conv_file:
             messages = json.load(conv_file)
-    except FileNotFoundError:
-        error_message = f"Failed loading conversation {file_name} from {path}."
+    except FileNotFoundError as error:
+        error_message = (
+            f"Failed loading conversation {file_name} from {path}.\n{str(error)}"
+        )
         print_utils.print_slowly(
             Back.RED + Style.BRIGHT + error_message + Style.RESET_ALL
         )
+        messages = []
 
     return messages
 
 
 def get_conversations(path=config.CONVERSATIONS_PATH):
     """Lists all saved conversations."""
 
@@ -67,17 +75,19 @@
 
 
 def get_system_answer(messages):
     """Returns the answer from OpenAI API."""
 
     while True:
         try:
-            answer = openai.ChatCompletion.create(model=config.MODEL, messages=messages)
+            answer = openai.ChatCompletion.create(
+                model=config.DEFAULT_MODEL, messages=messages
+            )
             return answer
-        except openai.error.RateLimitError:
+        except openai.OpenAIError:
             time.sleep(10)
 
 
 def is_conversations_empty(files: list, message: str):
     """Checks if the conversations directory is empty."""
 
     if files == []:
```

### Comparing `terminalgpt-1.0.9/terminalgpt/encryption.py` & `terminalgpt-1.1.0/terminalgpt/encryption.py`

 * *Files 16% similar despite different names*

```diff
@@ -52,13 +52,14 @@
 
 
 def check_api_key():
     """Checks if the API key is installed."""
 
     message = f"""
 OpenAI API key is missing!
-Please install the chatbot api key first with '{config.APP_NAME} install' command.
-    """
+Please install OpenAI API key first with '{config.APP_NAME} install' command.
+Or you can set the OPENAI_API_KEY environment variable export OPENAI_API_KEY=<your_api_key>
+"""
 
-    if not os.path.exists(config.SECRET_PATH):
+    if not os.path.exists(config.SECRET_PATH) and "OPENAI_API_KEY" not in os.environ:
         print(Style.BRIGHT + Fore.RED + message + Style.RESET_ALL)
         sys.exit(1)
```

### Comparing `terminalgpt-1.0.9/terminalgpt/main.py` & `terminalgpt-1.1.0/terminalgpt/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,58 @@
 """Main module for the terminalgpt package."""
 
 import getpass
 import os
 
 import click
-import openai
 from colorama import Fore, Style
 from prompt_toolkit import PromptSession, prompt
 from prompt_toolkit.completion import WordCompleter
 from prompt_toolkit.styles import Style as PromptStyle
 
-from terminalgpt import chat_utils, config, print_utils
+from terminalgpt import chat_utils, config
 from terminalgpt import conversations as conv
-from terminalgpt import encryption
+from terminalgpt import encryption, print_utils
 
 
 @click.group()
+@click.version_option(prog_name="TerminalGPT", message="%(prog)s %(version)s")
+@click.option(
+    "--model",
+    "-m",
+    type=click.Choice(list(config.MODELS.keys())),
+    default=config.DEFAULT_MODEL,
+    show_default=True,
+    help="Choose a model to use.",
+)
+# option to choose rich text output
+@click.option(
+    "--plain",
+    "-p",
+    is_flag=True,
+    default=False,
+    help="Plain text output.",
+)
 @click.pass_context
-def cli(ctx):
+def cli(ctx, model, plain):
     """*~ TerminalGPT - Your Personal Terminal Assistant ~*"""
 
     ctx.ensure_object(dict)
     ctx.obj["SESSION"] = PromptSession(
         style=PromptStyle.from_dict({"prompt": "bold"}),
         message="\nUser: ",
     )
-    ctx.obj["TOKEN_LIMIT"] = config.API_TOKEN_LIMIT - config.SAFETY_BUFFER
 
-    encryption.check_api_key()
-    key = encryption.get_encryption_key(config.KEY_PATH)
-    openai.api_key = encryption.decrypt(config.SECRET_PATH, key)
+    ctx.obj["MODEL"] = model
+
+    token_limit = config.MODELS[model]
+    safety_buffer = token_limit * 0.25
+
+    ctx.obj["TOKEN_LIMIT"] = token_limit - safety_buffer
+    ctx.obj["PLAIN"] = plain
 
 
 @click.command(
     help="Creating a secret api key for the chatbot."
     + " You will be asked to enter your OpenAI API key."
 )
 def install():
@@ -68,32 +87,68 @@
 
 
 @cli.command(help="Start a new conversation.")
 @click.pass_context
 def new(ctx):
     """Start a new conversation."""
 
+    chat_utils.set_api_key()
+
     messages = [
         config.INIT_SYSTEM_MESSAGE,
     ]
 
     chat_utils.welcome_message(messages + [config.INIT_WELCOME_MESSAGE])
 
     chat_utils.chat_loop(
         token_limit=ctx.obj["TOKEN_LIMIT"],
         session=ctx.obj["SESSION"],
         messages=messages,
+        model=ctx.obj["MODEL"],
+        plain=ctx.obj["PLAIN"],
     )
 
 
+@cli.command(help="One shot question answer.")
+# argument to ask a question
+@click.argument(
+    "question",
+    type=str,
+)
+@click.pass_context
+def one_shot(ctx, question):
+    """One shot question answer."""
+
+    chat_utils.set_api_key()
+
+    messages = [
+        config.INIT_SYSTEM_MESSAGE,
+    ]
+
+    messages.append({"role": "user", "content": question})
+
+    print()
+    answer = chat_utils.get_user_answer(
+        messages=messages,
+        model=ctx.obj["MODEL"],
+    )
+    message = answer["choices"][0]["message"]["content"]
+    print(Style.BRIGHT + "Assistant:" + Style.RESET_ALL, end=" ", flush=True)
+
+    print_utils.print_assistance_message(message, ctx.obj["PLAIN"])
+
+
 @cli.command(help="Choose a previous conversation to load.")
 @click.pass_context
 def load(ctx):
     """Load a previous conversation."""
 
+    messages = []
+    chat_utils.set_api_key()
+
     # get conversations list
     conversations = conv.get_conversations()
 
     msg = (
         Style.BRIGHT
         + Fore.RED
         + "\n** There are no conversations to load! **"
@@ -125,15 +180,17 @@
             + Fore.RED
             + "\n** Conversation not found! **"
             + Style.RESET_ALL
         )
         return
 
     # load conversation
-    messages = conv.load_conversation(conversation)
+    while not messages:
+        messages = conv.load_conversation(conversation)
+
     print_utils.print_slowly(
         Style.BRIGHT
         + Fore.LIGHTBLUE_EX
         + "\n** Conversation "
         + Fore.WHITE
         + conversation
         + Fore.LIGHTBLUE_EX
@@ -151,20 +208,23 @@
         messages, total_usage = chat_utils.reduce_tokens(
             messages=messages,
             total_usage=total_usage,
             token_limit=token_limit,
         )
 
     chat_utils.welcome_message(messages=messages)
+    messages.pop()
 
     chat_utils.chat_loop(
         token_limit=token_limit,
         session=ctx.obj["SESSION"],
         messages=messages,
         conversation_name=conversation,
+        model=ctx.obj["MODEL"],
+        plain=ctx.obj["PLAIN"],
     )
 
 
 @click.command(help="Choose a previous conversation to load.")
 def delete():
     """Delete previous conversations."""
```

### Comparing `terminalgpt-1.0.9/PKG-INFO` & `terminalgpt-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 Metadata-Version: 2.1
 Name: terminalgpt
-Version: 1.0.9
+Version: 1.1.0
 Summary: AI chat asistent in your terminal powered by OpenAI GPT-3.5
 Keywords: ai,chat,terminal,openai,gpt3,chatGPT,assistant,gpt3.5,terminalGPT,gpt-3.5-turbo
 Author: Adam Yodinsky
 Author-email: 27074934+adamyodinsky@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
-Requires-Dist: cryptography (>=39.0.2,<40.0.0)
-Requires-Dist: openai (>=0.27.0,<0.28.0)
+Requires-Dist: cryptography (>=40.0.2,<41.0.0)
+Requires-Dist: isort (>=5.12.0,<6.0.0)
+Requires-Dist: openai (>=0.27.6,<0.28.0)
 Requires-Dist: prompt-toolkit (>=3.0.38,<4.0.0)
+Requires-Dist: pylint (>=2.17.4,<3.0.0)
+Requires-Dist: pytest (>=7.3.1,<8.0.0)
+Requires-Dist: rich (>=13.3.5,<14.0.0)
 Requires-Dist: tiktoken (>=0.2,<0.4)
 Requires-Dist: yaspin (>=2.3.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # ![TerminalGPT](logo.png)
 
-[![Continuous Integration](https://github.com/adamyodinsky/TerminalGPT/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/adamyodinsky/TerminalGPT/actions/workflows/main.yml) ![PyPI](https://img.shields.io/pypi/v/terminalgpt) ![PyPI - Downloads](https://img.shields.io/pypi/dm/terminalgpt) ![commits-since](https://img.shields.io/github/commits-since/adamyodinsky/TerminalGPT/latest) ![GitHub last commit](https://img.shields.io/github/last-commit/adamyodinsky/terminalgpt)
+[![Continuous Integration](https://github.com/adamyodinsky/TerminalGPT/actions/workflows/MainCI.yml/badge.svg?branch=main)](https://github.com/adamyodinsky/TerminalGPT/actions/workflows/main.yml) ![PyPI](https://img.shields.io/pypi/v/terminalgpt) ![PyPI - Downloads](https://img.shields.io/pypi/dm/terminalgpt) ![commits-since](https://img.shields.io/github/commits-since/adamyodinsky/TerminalGPT/latest) ![GitHub last commit](https://img.shields.io/github/last-commit/adamyodinsky/terminalgpt)
 
 Welcome to terminalGPT, the terminal-based ChatGPT personal assistant app!
-With terminalGPT, you can easily interact with the OpenAI GPT 3.5 language model.
+With terminalGPT, you can easily interact with the OpenAI GPT-3.5 and GPT-4 language models.
 
 Whether you need help with a quick question or want to explore a complex topic, TerminalGPT is here to assist you. Simply enter your query and TerminalGPT will provide you with the best answer possible based on its extensive knowledge base.
 
 ---
 
-![Alt Text](./usage.gif)
+<img width="910" alt="image" src="https://user-images.githubusercontent.com/27074934/229319537-f332923d-f92e-4d91-8d5e-d26d8997341e.png">
 
 ---
 
 ## Why?
 
 Some advantages of using TerminalGPT over the chatGPT browser-based app:
 
@@ -45,25 +49,30 @@
 - TerminalGPT's answers are tailored to your machine's operating system, distribution, and chip-set architecture
 - Doesn't use your conversation data for training the model (unlike the browser-based app).
 - Your conversations are stored locally on your machine, so only you can access them.
 
 ## Pre-requisites
 
 - Python 3.6 or higher
-- An OpenAI Account and API key (It's free for personal use).
+- An OpenAI Account and API key.
    1. Sign up at <https://beta.openai.com/signup> using email or Google/Microsoft account.
    2. Go to <https://beta.openai.com/account/api-keys> or click on "View API keys" in the menu to get your API key.
-   For a more detailed guide on how to create an OpenAI API key, click [here](https://elephas.app/blog/how-to-create-openai-api-keys-cl5c4f21d281431po7k8fgyol0).
+
+**Notes:** OpenAI FREE API trial expired on 01-04-2023. You can still use the API, but you will need to set up a payment method.
+
+- To set up a payment method [click here](https://platform.openai.com/account/billing/payment-methods).
+- To check your usage [click here](https://platform.openai.com/account/usage).
+- To check pricing [click here](https://openai.com/pricing#language-models).
 
 ## Installation
 
 1. Install the latest TerminalGPT with pip install.
 
 ```sh
-pip install terminalgpt -U
+pip install terminalgpt -U --user
 ```
 
 2. Now you have `terminalgpt` command available in your terminal. Run the following install command to configure the app.
 
 ```sh
 terminalgpt install
 ```
@@ -72,35 +81,53 @@
 
 That's it! You're ready to use TerminalGPT!
 
 ---
 
 ## Usage
 
+### TL;DR
+
 ```sh
-Usage: terminalgpt [OPTIONS] COMMAND [ARGS]...
+Usage: main.py [OPTIONS] COMMAND [ARGS]...
+
+  *~ TerminalGPT - Your Personal Terminal Assistant ~*
 
 Options:
-  --help                 Show this message and exit.
+  --version                       Show the version and exit.
+  -m, --model [gpt-3.5-turbo|gpt-4]
+                                  Choose a model to use.  [default:
+                                  gpt-3.5-turbo]
+  -p, --plain                     Plain text output.
+  --help                          Show this message and exit.
 
 Commands:
-  new      Start a new conversation.
-  load     Choose a previous conversation to load.
-  delete   Choose a previous conversation to load.
-  install  Creating a secret api key for the chatbot.
+  delete    Choose a previous conversation to load.
+  install   Creating a secret api key for the chatbot.
+  load      Choose a previous conversation to load.
+  new       Start a new conversation.
+  one-shot  One shot question answer.
 ```
 
 ### New
 
 Start a new conversation:
 
 ```sh
 terminalgpt new
 ```
 
+### One-Shot
+
+One shot question to get a fast answer in the terminal.
+
+```sh
+terminalgpt one-shot "What is the meaning of life?"
+```
+
 ### Load
 
 Load previous conversations:
 
 ```sh
 terminalgpt load
 ```
@@ -113,15 +140,13 @@
 terminalgpt delete
 ```
 
 ---
 
 ## Future Plans
 
-1. Support multiline input.
-2. Support optional vim input mode.
-3. Auto-completion for all commands.
-4. Open source the project.
-5. Add more models (???)
-6. Encrypt the conversation data.
-7. Migrating to [Typer](https://typer.tiangolo.com/)
+1. Support optional Vim input mode.
+2. Auto-completion for all commands.
+3. Support local models
+
+---
```

