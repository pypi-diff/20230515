# Comparing `tmp/manim_voiceover-0.3.0.tar.gz` & `tmp/manim_voiceover-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manim_voiceover-0.3.0.tar", max compression
+gzip compressed data, was "manim_voiceover-0.3.1.tar", max compression
```

## Comparing `manim_voiceover-0.3.0.tar` & `manim_voiceover-0.3.1.tar`

### file list

```diff
@@ -1,26 +1,23 @@
--rw-r--r--   0        0        0     1088 2023-01-22 10:19:19.964539 manim_voiceover-0.3.0/LICENSE
--rw-r--r--   0        0        0     2604 2023-01-22 10:19:19.964539 manim_voiceover-0.3.0/README.md
--rw-r--r--   0        0        0      203 2023-01-22 10:19:19.968539 manim_voiceover-0.3.0/manim_voiceover/__init__.py
--rw-r--r--   0        0        0     1780 2023-01-22 10:19:19.968539 manim_voiceover-0.3.0/manim_voiceover/defaults.py
--rw-r--r--   0        0        0     8553 2023-01-22 10:19:19.968539 manim_voiceover-0.3.0/manim_voiceover/helper.py
--rw-r--r--   0        0        0      658 2023-01-22 10:19:19.968539 manim_voiceover-0.3.0/manim_voiceover/modify_audio.py
--rw-r--r--   0        0        0      343 2023-01-22 10:19:19.968539 manim_voiceover-0.3.0/manim_voiceover/services/__init__.py
--rw-r--r--   0        0        0     8658 2023-01-22 10:19:19.968539 manim_voiceover-0.3.0/manim_voiceover/services/azure.py
--rw-r--r--   0        0        0     6962 2023-01-22 10:19:19.968539 manim_voiceover-0.3.0/manim_voiceover/services/base.py
--rw-r--r--   0        0        0     1764 2023-01-22 10:19:19.968539 manim_voiceover-0.3.0/manim_voiceover/services/coqui/__init__.py
--rw-r--r--   0        0        0     2663 2023-01-22 10:19:19.968539 manim_voiceover-0.3.0/manim_voiceover/services/coqui/synthesize.py
--rw-r--r--   0        0        0    20497 2023-01-22 10:19:19.968539 manim_voiceover-0.3.0/manim_voiceover/services/coqui/utils_synthesizer.py
--rw-r--r--   0        0        0     2794 2023-01-22 10:19:19.968539 manim_voiceover-0.3.0/manim_voiceover/services/gtts.py
--rw-r--r--   0        0        0     1541 2023-01-22 10:19:19.968539 manim_voiceover-0.3.0/manim_voiceover/services/pyttsx3.py
--rw-r--r--   0        0        0     4022 2023-01-22 10:19:19.968539 manim_voiceover-0.3.0/manim_voiceover/services/recorder/__init__.py
--rw-r--r--   0        0        0     7812 2023-01-22 10:19:19.968539 manim_voiceover-0.3.0/manim_voiceover/services/recorder/utility.py
--rw-r--r--   0        0        0     6047 2023-01-22 10:19:19.968539 manim_voiceover-0.3.0/manim_voiceover/services/stitcher.py
--rw-r--r--   0        0        0     5045 2023-01-22 10:19:19.968539 manim_voiceover-0.3.0/manim_voiceover/tracker.py
--rw-r--r--   0        0        0      583 2023-01-22 10:19:19.968539 manim_voiceover-0.3.0/manim_voiceover/translate/__init__.py
--rw-r--r--   0        0        0     6075 2023-01-22 10:19:19.968539 manim_voiceover-0.3.0/manim_voiceover/translate/gettext_utils.py
--rw-r--r--   0        0        0     3815 2023-01-22 10:19:19.968539 manim_voiceover-0.3.0/manim_voiceover/translate/render.py
--rw-r--r--   0        0        0     2510 2023-01-22 10:19:19.968539 manim_voiceover-0.3.0/manim_voiceover/translate/translate.py
--rw-r--r--   0        0        0     7015 2023-01-22 10:19:19.968539 manim_voiceover-0.3.0/manim_voiceover/voiceover_scene.py
--rw-r--r--   0        0        0     3310 2023-01-22 10:19:19.972539 manim_voiceover-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4544 1970-01-01 00:00:00.000000 manim_voiceover-0.3.0/setup.py
--rw-r--r--   0        0        0     5167 1970-01-01 00:00:00.000000 manim_voiceover-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-05-14 23:08:35.038573 manim_voiceover-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2832 2023-05-14 23:08:35.038573 manim_voiceover-0.3.1/README.md
+-rw-r--r--   0        0        0      203 2023-05-14 23:08:35.042573 manim_voiceover-0.3.1/manim_voiceover/__init__.py
+-rw-r--r--   0        0        0     1779 2023-05-14 23:08:35.042573 manim_voiceover-0.3.1/manim_voiceover/defaults.py
+-rw-r--r--   0        0        0     6032 2023-05-14 23:08:35.042573 manim_voiceover-0.3.1/manim_voiceover/helper.py
+-rw-r--r--   0        0        0      658 2023-05-14 23:08:35.042573 manim_voiceover-0.3.1/manim_voiceover/modify_audio.py
+-rw-r--r--   0        0        0      343 2023-05-14 23:08:35.042573 manim_voiceover-0.3.1/manim_voiceover/services/__init__.py
+-rw-r--r--   0        0        0     8658 2023-05-14 23:08:35.042573 manim_voiceover-0.3.1/manim_voiceover/services/azure.py
+-rw-r--r--   0        0        0     7514 2023-05-14 23:08:35.042573 manim_voiceover-0.3.1/manim_voiceover/services/base.py
+-rw-r--r--   0        0        0     2754 2023-05-14 23:08:35.042573 manim_voiceover-0.3.1/manim_voiceover/services/coqui.py
+-rw-r--r--   0        0        0     2794 2023-05-14 23:08:35.042573 manim_voiceover-0.3.1/manim_voiceover/services/gtts.py
+-rw-r--r--   0        0        0     1541 2023-05-14 23:08:35.042573 manim_voiceover-0.3.1/manim_voiceover/services/pyttsx3.py
+-rw-r--r--   0        0        0     4022 2023-05-14 23:08:35.042573 manim_voiceover-0.3.1/manim_voiceover/services/recorder/__init__.py
+-rw-r--r--   0        0        0     7812 2023-05-14 23:08:35.046573 manim_voiceover-0.3.1/manim_voiceover/services/recorder/utility.py
+-rw-r--r--   0        0        0     6047 2023-05-14 23:08:35.046573 manim_voiceover-0.3.1/manim_voiceover/services/stitcher.py
+-rw-r--r--   0        0        0     5045 2023-05-14 23:08:35.046573 manim_voiceover-0.3.1/manim_voiceover/tracker.py
+-rw-r--r--   0        0        0      584 2023-05-14 23:08:35.046573 manim_voiceover-0.3.1/manim_voiceover/translate/__init__.py
+-rw-r--r--   0        0        0     6395 2023-05-14 23:08:35.046573 manim_voiceover-0.3.1/manim_voiceover/translate/gettext_utils.py
+-rw-r--r--   0        0        0     3815 2023-05-14 23:08:35.046573 manim_voiceover-0.3.1/manim_voiceover/translate/render.py
+-rw-r--r--   0        0        0     2510 2023-05-14 23:08:35.046573 manim_voiceover-0.3.1/manim_voiceover/translate/translate.py
+-rw-r--r--   0        0        0     7089 2023-05-14 23:08:35.046573 manim_voiceover-0.3.1/manim_voiceover/voiceover_scene.py
+-rw-r--r--   0        0        0     3505 2023-05-14 23:08:35.046573 manim_voiceover-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5450 1970-01-01 00:00:00.000000 manim_voiceover-0.3.1/PKG-INFO
```

### Comparing `manim_voiceover-0.3.0/LICENSE` & `manim_voiceover-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.0/README.md` & `manim_voiceover-0.3.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Manim Voiceover
 
 <p>
     <a href="https://github.com/ManimCommunity/manim-voiceover/workflows/Build/badge.svg"><img src="https://github.com/ManimCommunity/manim-voiceover/workflows/Build/badge.svg" alt="Github Actions Status"></a>
     <a href="https://pypi.org/project/manim_voiceover/"><img src="https://img.shields.io/pypi/v/manim_voiceover.svg?style=flat&logo=pypi" alt="PyPI Latest Release"></a>
     <a href="https://pepy.tech/project/manim_voiceover"><img src="https://pepy.tech/badge/manim_voiceover/month?" alt="Downloads"> </a>
-    <a href="https://manim_voiceover.readthedocs.io/en/latest/?badge=latest"><img src="https://readthedocs.org/projects/manim_voiceover/badge/?version=latest" alt="Documentation Status"></a>
+    <a href="https://voiceover.manim.community/en/latest"><img src="https://readthedocs.org/projects/manim_voiceover/badge/?version=latest" alt="Documentation Status"></a>
     <a href="https://github.com/ManimCommunity/manim-voiceover/blob/main/LICENSE"><img src="https://img.shields.io/github/license/ManimCommunity/manim-voiceover.svg?color=blue" alt="License"></a>
     <a href="https://manim.community/discord"><img src="https://dcbadge.vercel.app/api/server/qY23bthHTY?style=flat" alt="Discord"></a>
 </p>
 
 Manim Voiceover is a [Manim](https://manim.community) plugin for all things voiceover:
 
 - Add voiceovers to Manim videos *directly in Python* without having to use a video editor.
@@ -37,8 +37,10 @@
 
 [Check out the docs to get started with Manim Voiceover.](https://voiceover.manim.community/en/latest/quickstart.html)
 
 ## Examples
 
 [Check out the example gallery to get inspired.](https://voiceover.manim.community/en/latest/examples.html)
 
+## Translate
 
+Manim Voiceover can use machine translation services like [DeepL](https://www.deepl.com/) to translate voiceovers into other languages. [Check out the docs for more details.](https://voiceover.manim.community/en/latest/translate.html)
```

#### html2text {}

```diff
@@ -17,8 +17,11 @@
 [gTTS](https://github.com/pndurette/gTTS/) - [pyttsx3](https://github.com/
 nateshmbhat/pyttsx3) [Check out the documentation for more details.](https://
 voiceover.manim.community/) ## Installation [Installation instructions in Manim
 Voiceover docs.](https://voiceover.manim.community/en/latest/installation.html)
 ## Get started [Check out the docs to get started with Manim Voiceover.](https:
 //voiceover.manim.community/en/latest/quickstart.html) ## Examples [Check out
 the example gallery to get inspired.](https://voiceover.manim.community/en/
-latest/examples.html)
+latest/examples.html) ## Translate Manim Voiceover can use machine translation
+services like [DeepL](https://www.deepl.com/) to translate voiceovers into
+other languages. [Check out the docs for more details.](https://
+voiceover.manim.community/en/latest/translate.html)
```

### Comparing `manim_voiceover-0.3.0/manim_voiceover/defaults.py` & `manim_voiceover-0.3.1/manim_voiceover/defaults.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,8 +67,7 @@
     "tr": "Turkish",
     "uk": "Ukrainian",
     "zh": "Chinese (simplified)",
 }
 
 DEEPL_AVAILABLE_SOURCE_LANG = list(DEEPL_SOURCE_LANG.keys())
 DEEPL_AVAILABLE_TARGET_LANG = list(DEEPL_TARGET_LANG.keys())
-
```

### Comparing `manim_voiceover-0.3.0/manim_voiceover/helper.py` & `manim_voiceover-0.3.1/manim_voiceover/helper.py`

 * *Files 24% similar despite different names*

```diff
@@ -115,85 +115,14 @@
 
     json_data.append(data)
     with open(json_file, "w") as f:
         json.dump(json_data, f, indent=2)
     return
 
 
-def get_whisper_model(model_name: str):
-    installed = False
-    while True:
-        try:
-            import whisper
-        except ImportError:
-            logger.info(
-                "OpenAI Whisper is not installed. Shall I install it for you? [Y/n]"
-            )
-            logger.info(
-                "Note: This will install the latest version of Whisper from GitHub."
-            )
-            answer = input()
-            if answer.lower() == "n":
-                raise ImportError(
-                    "Whisper is not installed. Install it by running `pip install git+https://github.com/openai/whisper.git`"
-                )
-            else:
-                logger.info("Installing Whisper...")
-                pip.main(["install", "git+https://github.com/openai/whisper.git"])
-                installed = True
-                continue
-
-        try:
-            import whisper as tmp
-
-            tmp.load_model
-        except AttributeError:
-            logger.info(
-                "The installed whisper package appears to be the wrong one. "
-                "The PyPI package `whisper` is not the one from OpenAI. "
-                "Unfortunately, OpenAI did not publish their package to PyPI "
-                "and it needs to be installed from GitHub. "
-                "Shall I uninstall the wrong `whisper` for you? [Y/n]\n"
-                "Note: Run Manim again after uninstalling the wrong package to install the correct one."
-            )
-            answer = input()
-            if answer.lower() == "n":
-                logger.info("Please uninstall the wrong whisper package manually.")
-                sys.exit(1)
-            else:
-                logger.info("Uninstalling wrong whisper package...")
-                pip.main(["uninstall", "whisper", "-y"])
-                sys.exit(0)
-        try:
-            import stable_whisper as whisper
-        except ImportError:
-            logger.info(
-                "\nThe package stable-ts is not installed (Required for fixing timestamps returned by Whisper)."
-            )
-            logger.info("Shall I install it for you? [Y/n]")
-            answer = input()
-            if answer.lower() == "n":
-                raise ImportError(
-                    "stable-ts is not installed. Install it by running `pip install stable-ts`"
-                )
-            else:
-                logger.info("Installing stable-ts...")
-                pip.main(["install", "manim-voiceover[whisper]"])
-                installed = True
-                continue
-
-        break
-
-    if installed:
-        logger.info("Installed missing packages. Please run Manim again.")
-        sys.exit(0)
-
-    return whisper.load_model(model_name)
-
-
 def prompt_ask_missing_package(target_module: str, package_name: str):
     try:
         importlib.import_module(target_module)
         return
     except ImportError:
         pass
     logger.info(
@@ -214,26 +143,29 @@
 
 def prompt_ask_missing_extras(
     target_module: Union[str, list],
     extras: str,
     dependent_item: str,
 ):
     if isinstance(target_module, str):
-        target_modules = []
+        target_modules = [target_module]
     elif isinstance(target_module, list):
         target_modules = target_module
     else:
         raise TypeError("target_module must be a string or a list of strings")
 
     try:
         for target_module in target_modules:
             importlib.import_module(target_module)
+        # Successfully imported all modules, we can return
         return
-    except ImportError:
+    except (ImportError, ModuleNotFoundError) as e:
         pass
+
+    # If we reach here, it means that at least one of the modules is not installed
     logger.info(
         f"The extra packages required by {dependent_item} are not installed. "
         f"Shall I install them for you? [Y/n]"
     )
     answer = input()
     if answer.lower() == "n":
         raise ImportError(
```

### Comparing `manim_voiceover-0.3.0/manim_voiceover/modify_audio.py` & `manim_voiceover-0.3.1/manim_voiceover/modify_audio.py`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.0/manim_voiceover/services/azure.py` & `manim_voiceover-0.3.1/manim_voiceover/services/azure.py`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.0/manim_voiceover/services/base.py` & `manim_voiceover-0.3.1/manim_voiceover/services/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import humanhash
 from pathlib import Path
 from manim import config, logger
 from manim_voiceover.defaults import (
     DEFAULT_VOICEOVER_CACHE_DIR,
     DEFAULT_VOICEOVER_CACHE_JSON_FILENAME,
 )
-from manim_voiceover.helper import append_to_json_file, get_whisper_model
+from manim_voiceover.helper import append_to_json_file, prompt_ask_missing_extras
 from manim_voiceover.modify_audio import adjust_speed
 from manim_voiceover.tracker import AUDIO_OFFSET_RESOLUTION
 
 
 def timestamps_to_word_boundaries(segments):
     word_boundaries = []
     current_text_offset = 0
@@ -129,15 +129,28 @@
 
         Args:
             model (str, optional): The Whisper model to use for transcription. Defaults to None.
             kwargs (dict, optional): Keyword arguments to pass to the transcribe() function. Defaults to {}.
         """
         if model != self.transcription_model:
             if model is not None:
-                self._whisper_model = get_whisper_model(model)
+                try:
+                    import whisper as __tmp
+                    import stable_whisper as whisper
+                except ImportError:
+                    logger.error(
+                        'Missing packages. Run `pip install "manim-voiceover[transcribe]"` to be able to transcribe voiceovers.'
+                    )
+
+                prompt_ask_missing_extras(
+                    ["whisper", "stable_whisper"],
+                    "transcribe",
+                    "SpeechService.set_transcription()",
+                )
+                self._whisper_model = whisper.load_model(model)
             else:
                 self._whisper_model = None
 
         self.transcription_kwargs = kwargs
 
     def get_data_hash(self, data: dict) -> str:
         dumped_data = json.dumps(data)
```

### Comparing `manim_voiceover-0.3.0/manim_voiceover/services/gtts.py` & `manim_voiceover-0.3.1/manim_voiceover/services/gtts.py`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.0/manim_voiceover/services/pyttsx3.py` & `manim_voiceover-0.3.1/manim_voiceover/services/pyttsx3.py`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.0/manim_voiceover/services/recorder/__init__.py` & `manim_voiceover-0.3.1/manim_voiceover/services/recorder/__init__.py`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.0/manim_voiceover/services/recorder/utility.py` & `manim_voiceover-0.3.1/manim_voiceover/services/recorder/utility.py`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.0/manim_voiceover/services/stitcher.py` & `manim_voiceover-0.3.1/manim_voiceover/services/stitcher.py`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.0/manim_voiceover/tracker.py` & `manim_voiceover-0.3.1/manim_voiceover/tracker.py`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.0/manim_voiceover/translate/__init__.py` & `manim_voiceover-0.3.1/manim_voiceover/translate/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import gettext
 
+
 def get_gettext(locale=None, domain=None):
     ret = gettext.gettext
 
     if locale is None:
         locale = os.getenv("LOCALE")
 
     if domain is None:
```

### Comparing `manim_voiceover-0.3.0/manim_voiceover/translate/gettext_utils.py` & `manim_voiceover-0.3.1/manim_voiceover/translate/gettext_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 import re
-import deepl
 import os
 import typing as t
 
+from manim import logger
+
+from manim_voiceover.helper import prompt_ask_missing_extras
+
+try:
+    import deepl
+except ImportError:
+    logger.error(
+        'Missing packages. Run `pip install "manim-voiceover[translate]"` to be able to translate voiceovers.'
+    )
+
 
 def init_gettext(files, domain, localedir):
     """Initialize gettext for a list of files"""
     # If locale directory does not exist, create it
     if not os.path.exists(localedir):
         os.makedirs(localedir)
 
@@ -129,14 +139,16 @@
             self.entries.append(entry)
 
     def translate(self, target_lang, api_key=None):
         "Translates a .po file using DeepL. Note: This overwrites the .po file."
 
         assert api_key is not None, "Please provide a DeepL API key."
 
+        prompt_ask_missing_extras("deepl", "translate", "POFile")
+
         if target_lang == "en":
             target_lang = "en-US"
         elif target_lang == "pt":
             target_lang = "pt-BR"
 
         translate_idx = []
         for idx, entry in enumerate(self.entries):
```

### Comparing `manim_voiceover-0.3.0/manim_voiceover/translate/render.py` & `manim_voiceover-0.3.1/manim_voiceover/translate/render.py`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.0/manim_voiceover/translate/translate.py` & `manim_voiceover-0.3.1/manim_voiceover/translate/translate.py`

 * *Files identical despite different names*

### Comparing `manim_voiceover-0.3.0/manim_voiceover/voiceover_scene.py` & `manim_voiceover-0.3.1/manim_voiceover/voiceover_scene.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from math import ceil
 from contextlib import contextmanager
 from pathlib import Path
 from typing import Optional, Generator
+import re
 
 from manim import Scene, config
 from manim_voiceover.services.base import SpeechService
 from manim_voiceover.tracker import VoiceoverTracker
 from manim_voiceover.helper import chunks
 
 
@@ -66,15 +67,16 @@
         self.current_tracker = tracker
 
         # if self.create_script:
         #     self.save_to_script_file(text)
 
         if self.create_subcaption:
             if subcaption is None:
-                subcaption = text
+                # Remove placeholders
+                subcaption = re.sub(r"<[^<>]+/>", "", text)
 
             self.add_wrapped_subcaption(
                 subcaption,
                 tracker.duration,
                 subcaption_buff=subcaption_buff,
                 max_subcaption_len=max_subcaption_len,
             )
```

### Comparing `manim_voiceover-0.3.0/pyproject.toml` & `manim_voiceover-0.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "manim-voiceover"
-version = "0.3.0"
+version = "0.3.1"
 description = "Manim plugin for all things voiceover"
 authors = ["The Manim Community Developers <contact@manim.community>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "manim_voiceover" }]
 repository = "https://github.com/ManimCommunity/manim-voiceover"
 homepage = "https://voiceover.manim.community"
@@ -55,33 +55,38 @@
 # TTS = { version = "*", optional = true }
 pynput = { version = "^1.7.6", optional = true }
 playsound = { version = "^1.3.0", optional = true }
 # deep-translator = { version = "^1.9.2", optional = true }
 deepl = { version = "^1.12.0", optional = true }
 humanhash3 = "^0.0.6"
 pip = ">=21.0.1"
+openai-whisper = { version = "^20230117", optional = true }
+stable-ts = { version ="^1.0.3", optional = true }
 
 [tool.poetry.extras]
 azure = ["azure-cognitiveservices-speech"]
 gtts = ["gTTS"]
 pyttsx3 = ["pyttsx3"]
 # coqui = ["torch", "TTS"]
 coqui = [] # Removed TTS as deps for now
 recorder = ["PyAudio", "pynput", "playsound"]
 translate = ["deepl"]
+transcribe = ["openai-whisper", "stable-ts"]
 all = [
     "azure-cognitiveservices-speech",
     "gTTS",
     "pyttsx3",
     "torch",
     "TTS",
     "PyAudio",
     "pynput",
     "playsound",
     "deepl",
+    "openai-whisper",
+    "stable-ts",
 ]
 
 [tool.poetry.group.dev.dependencies]
 Pygments = "^2.13.0"
 pytest-cov = "^3.0.0"
 pytest = "^6.0"
 pylint = "^2.12.2"
```

### Comparing `manim_voiceover-0.3.0/PKG-INFO` & `manim_voiceover-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manim-voiceover
-Version: 0.3.0
+Version: 0.3.1
 Summary: Manim plugin for all things voiceover
 Home-page: https://voiceover.manim.community
 License: MIT
 Keywords: text-to-speech,tts,voiceover,manim,recording,speech synthesis,math animations
 Author: The Manim Community Developers
 Author-email: contact@manim.community
 Requires-Python: >=3.8,<4
@@ -12,58 +12,58 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Multimedia :: Sound/Audio :: Capture/Recording
 Classifier: Topic :: Multimedia :: Sound/Audio :: Sound Synthesis
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Provides-Extra: all
 Provides-Extra: azure
 Provides-Extra: coqui
 Provides-Extra: gtts
 Provides-Extra: pyttsx3
 Provides-Extra: recorder
+Provides-Extra: transcribe
 Provides-Extra: translate
 Requires-Dist: PyAudio (>=0.2.12,<0.3.0) ; extra == "recorder" or extra == "all"
 Requires-Dist: azure-cognitiveservices-speech (>=1.24.0,<2.0.0) ; extra == "azure" or extra == "all"
 Requires-Dist: deepl (>=1.12.0,<2.0.0) ; extra == "translate" or extra == "all"
 Requires-Dist: gTTS (>=2.2.4,<3.0.0) ; extra == "gtts" or extra == "all"
 Requires-Dist: humanhash3 (>=0.0.6,<0.0.7)
 Requires-Dist: manim
 Requires-Dist: mutagen (>=1.46.0,<2.0.0)
+Requires-Dist: openai-whisper (>=20230117,<20230118) ; extra == "transcribe" or extra == "all"
 Requires-Dist: pip (>=21.0.1)
 Requires-Dist: playsound (>=1.3.0,<2.0.0) ; extra == "recorder" or extra == "all"
 Requires-Dist: pydub (>=0.25.1,<0.26.0)
 Requires-Dist: pynput (>=1.7.6,<2.0.0) ; extra == "recorder" or extra == "all"
 Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
 Requires-Dist: pyttsx3 (>=2.90,<3.0) ; extra == "pyttsx3" or extra == "all"
 Requires-Dist: sox (>=1.4.1,<2.0.0)
+Requires-Dist: stable-ts (>=1.0.3,<2.0.0) ; extra == "transcribe" or extra == "all"
 Project-URL: Documentation, https://voiceover.manim.community
 Project-URL: Repository, https://github.com/ManimCommunity/manim-voiceover
 Description-Content-Type: text/markdown
 
 # Manim Voiceover
 
 <p>
     <a href="https://github.com/ManimCommunity/manim-voiceover/workflows/Build/badge.svg"><img src="https://github.com/ManimCommunity/manim-voiceover/workflows/Build/badge.svg" alt="Github Actions Status"></a>
     <a href="https://pypi.org/project/manim_voiceover/"><img src="https://img.shields.io/pypi/v/manim_voiceover.svg?style=flat&logo=pypi" alt="PyPI Latest Release"></a>
     <a href="https://pepy.tech/project/manim_voiceover"><img src="https://pepy.tech/badge/manim_voiceover/month?" alt="Downloads"> </a>
-    <a href="https://manim_voiceover.readthedocs.io/en/latest/?badge=latest"><img src="https://readthedocs.org/projects/manim_voiceover/badge/?version=latest" alt="Documentation Status"></a>
+    <a href="https://voiceover.manim.community/en/latest"><img src="https://readthedocs.org/projects/manim_voiceover/badge/?version=latest" alt="Documentation Status"></a>
     <a href="https://github.com/ManimCommunity/manim-voiceover/blob/main/LICENSE"><img src="https://img.shields.io/github/license/ManimCommunity/manim-voiceover.svg?color=blue" alt="License"></a>
     <a href="https://manim.community/discord"><img src="https://dcbadge.vercel.app/api/server/qY23bthHTY?style=flat" alt="Discord"></a>
 </p>
 
 Manim Voiceover is a [Manim](https://manim.community) plugin for all things voiceover:
 
 - Add voiceovers to Manim videos *directly in Python* without having to use a video editor.
@@ -92,9 +92,10 @@
 
 [Check out the docs to get started with Manim Voiceover.](https://voiceover.manim.community/en/latest/quickstart.html)
 
 ## Examples
 
 [Check out the example gallery to get inspired.](https://voiceover.manim.community/en/latest/examples.html)
 
+## Translate
 
-
+Manim Voiceover can use machine translation services like [DeepL](https://www.deepl.com/) to translate voiceovers into other languages. [Check out the docs for more details.](https://voiceover.manim.community/en/latest/translate.html)
```

#### html2text {}

```diff
@@ -1,39 +1,40 @@
-Metadata-Version: 2.1 Name: manim-voiceover Version: 0.3.0 Summary: Manim
+Metadata-Version: 2.1 Name: manim-voiceover Version: 0.3.1 Summary: Manim
 plugin for all things voiceover Home-page: https://voiceover.manim.community
 License: MIT Keywords: text-to-speech,tts,voiceover,manim,recording,speech
 synthesis,math animations Author: The Manim Community Developers Author-email:
 contact@manim.community Requires-Python: >=3.8,<4 Classifier: Development
 Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Topic :: Multimedia ::
+Programming Language :: Python :: 3.7 Classifier: Topic :: Multimedia ::
 Graphics Classifier: Topic :: Multimedia :: Sound/Audio :: Capture/Recording
 Classifier: Topic :: Multimedia :: Sound/Audio :: Sound Synthesis Classifier:
 Topic :: Multimedia :: Sound/Audio :: Speech Classifier: Topic :: Multimedia ::
 Video Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
 Scientific/Engineering :: Visualization Provides-Extra: all Provides-Extra:
 azure Provides-Extra: coqui Provides-Extra: gtts Provides-Extra: pyttsx3
-Provides-Extra: recorder Provides-Extra: translate Requires-Dist: PyAudio
-(>=0.2.12,<0.3.0) ; extra == "recorder" or extra == "all" Requires-Dist: azure-
-cognitiveservices-speech (>=1.24.0,<2.0.0) ; extra == "azure" or extra == "all"
-Requires-Dist: deepl (>=1.12.0,<2.0.0) ; extra == "translate" or extra == "all"
-Requires-Dist: gTTS (>=2.2.4,<3.0.0) ; extra == "gtts" or extra == "all"
-Requires-Dist: humanhash3 (>=0.0.6,<0.0.7) Requires-Dist: manim Requires-Dist:
-mutagen (>=1.46.0,<2.0.0) Requires-Dist: pip (>=21.0.1) Requires-Dist:
-playsound (>=1.3.0,<2.0.0) ; extra == "recorder" or extra == "all" Requires-
-Dist: pydub (>=0.25.1,<0.26.0) Requires-Dist: pynput (>=1.7.6,<2.0.0) ; extra
-== "recorder" or extra == "all" Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
-Requires-Dist: pyttsx3 (>=2.90,<3.0) ; extra == "pyttsx3" or extra == "all"
-Requires-Dist: sox (>=1.4.1,<2.0.0) Project-URL: Documentation, https://
+Provides-Extra: recorder Provides-Extra: transcribe Provides-Extra: translate
+Requires-Dist: PyAudio (>=0.2.12,<0.3.0) ; extra == "recorder" or extra ==
+"all" Requires-Dist: azure-cognitiveservices-speech (>=1.24.0,<2.0.0) ; extra
+== "azure" or extra == "all" Requires-Dist: deepl (>=1.12.0,<2.0.0) ; extra ==
+"translate" or extra == "all" Requires-Dist: gTTS (>=2.2.4,<3.0.0) ; extra ==
+"gtts" or extra == "all" Requires-Dist: humanhash3 (>=0.0.6,<0.0.7) Requires-
+Dist: manim Requires-Dist: mutagen (>=1.46.0,<2.0.0) Requires-Dist: openai-
+whisper (>=20230117,<20230118) ; extra == "transcribe" or extra == "all"
+Requires-Dist: pip (>=21.0.1) Requires-Dist: playsound (>=1.3.0,<2.0.0) ; extra
+== "recorder" or extra == "all" Requires-Dist: pydub (>=0.25.1,<0.26.0)
+Requires-Dist: pynput (>=1.7.6,<2.0.0) ; extra == "recorder" or extra == "all"
+Requires-Dist: python-dotenv (>=0.21.0,<0.22.0) Requires-Dist: pyttsx3
+(>=2.90,<3.0) ; extra == "pyttsx3" or extra == "all" Requires-Dist: sox
+(>=1.4.1,<2.0.0) Requires-Dist: stable-ts (>=1.0.3,<2.0.0) ; extra ==
+"transcribe" or extra == "all" Project-URL: Documentation, https://
 voiceover.manim.community Project-URL: Repository, https://github.com/
 ManimCommunity/manim-voiceover Description-Content-Type: text/markdown # Manim
 Voiceover
 [Github_Actions_Status] [PyPI_Latest_Release] [Downloads] [Documentation
 Status] [License] [Discord]
 Manim Voiceover is a [Manim](https://manim.community) plugin for all things
 voiceover: - Add voiceovers to Manim videos *directly in Python* without having
@@ -51,8 +52,11 @@
 [gTTS](https://github.com/pndurette/gTTS/) - [pyttsx3](https://github.com/
 nateshmbhat/pyttsx3) [Check out the documentation for more details.](https://
 voiceover.manim.community/) ## Installation [Installation instructions in Manim
 Voiceover docs.](https://voiceover.manim.community/en/latest/installation.html)
 ## Get started [Check out the docs to get started with Manim Voiceover.](https:
 //voiceover.manim.community/en/latest/quickstart.html) ## Examples [Check out
 the example gallery to get inspired.](https://voiceover.manim.community/en/
-latest/examples.html)
+latest/examples.html) ## Translate Manim Voiceover can use machine translation
+services like [DeepL](https://www.deepl.com/) to translate voiceovers into
+other languages. [Check out the docs for more details.](https://
+voiceover.manim.community/en/latest/translate.html)
```

