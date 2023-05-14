# Comparing `tmp/sleepyemoji-2.1.tar.gz` & `tmp/sleepyemoji-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleepyemoji-2.1.tar", max compression
+gzip compressed data, was "sleepyemoji-2.2.tar", max compression
```

## Comparing `sleepyemoji-2.1.tar` & `sleepyemoji-2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     2448 2022-12-26 00:23:44.109192 sleepyemoji-2.1/README.md
--rw-r--r--   0        0        0      805 2023-04-13 21:30:19.273627 sleepyemoji-2.1/pyproject.toml
--rwxr-xr-x   0        0        0     4318 2023-04-13 21:29:50.343461 sleepyemoji-2.1/sleepyemoji.py
--rw-r--r--   0        0        0      210 2023-03-13 05:00:42.619222 sleepyemoji-2.1/toolchain/animals.py
--rw-r--r--   0        0        0      339 2023-04-13 21:20:47.281116 sleepyemoji-2.1/toolchain/combos.py
--rw-r--r--   0        0        0     1275 2023-03-13 04:43:30.180373 sleepyemoji-2.1/toolchain/faces.py
--rw-r--r--   0        0        0      812 2022-12-26 00:12:51.472849 sleepyemoji-2.1/toolchain/fetcher.py
--rw-r--r--   0        0        0      694 2023-03-13 04:53:43.875605 sleepyemoji-2.1/toolchain/hands.py
--rw-r--r--   0        0        0     1202 2023-03-13 05:05:03.220006 sleepyemoji-2.1/toolchain/icons.py
--rw-r--r--   0        0        0     1785 2022-12-26 00:12:51.474421 sleepyemoji-2.1/toolchain/option_utils.py
--rw-r--r--   0        0        0      176 2023-03-13 04:58:22.489310 sleepyemoji-2.1/toolchain/people.py
--rw-r--r--   0        0        0     3201 1970-01-01 00:00:00.000000 sleepyemoji-2.1/setup.py
--rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 sleepyemoji-2.1/PKG-INFO
+-rw-r--r--   0        0        0     2448 2022-12-26 00:23:44.109192 sleepyemoji-2.2/README.md
+-rw-r--r--   0        0        0      805 2023-05-14 23:10:33.079558 sleepyemoji-2.2/pyproject.toml
+-rwxr-xr-x   0        0        0     4318 2023-04-13 21:29:50.343461 sleepyemoji-2.2/sleepyemoji.py
+-rw-r--r--   0        0        0      210 2023-03-13 05:00:42.619222 sleepyemoji-2.2/toolchain/animals.py
+-rw-r--r--   0        0        0      339 2023-05-14 23:07:02.349783 sleepyemoji-2.2/toolchain/combos.py
+-rw-r--r--   0        0        0     1275 2023-03-13 04:43:30.180373 sleepyemoji-2.2/toolchain/faces.py
+-rw-r--r--   0        0        0      812 2022-12-26 00:12:51.472849 sleepyemoji-2.2/toolchain/fetcher.py
+-rw-r--r--   0        0        0      694 2023-03-13 04:53:43.875605 sleepyemoji-2.2/toolchain/hands.py
+-rw-r--r--   0        0        0     1202 2023-03-13 05:05:03.220006 sleepyemoji-2.2/toolchain/icons.py
+-rw-r--r--   0        0        0     1785 2022-12-26 00:12:51.474421 sleepyemoji-2.2/toolchain/option_utils.py
+-rw-r--r--   0        0        0      176 2023-03-13 04:58:22.489310 sleepyemoji-2.2/toolchain/people.py
+-rw-r--r--   0        0        0     3201 1970-01-01 00:00:00.000000 sleepyemoji-2.2/setup.py
+-rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 sleepyemoji-2.2/PKG-INFO
```

### Comparing `sleepyemoji-2.1/README.md` & `sleepyemoji-2.2/README.md`

 * *Files identical despite different names*

### Comparing `sleepyemoji-2.1/pyproject.toml` & `sleepyemoji-2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sleepyemoji"
-version = "2.1"
+version = "2.2"
 description = "Print all the emojis that sleepyboy thinks are worthwhile!"
 authors = ["anthonybench <anythonybenchyep@gmail.com>"]
 license = "GNU GPL"
 readme = "README.md"
 keywords = ["emoji", "unicode"]
 repository = "https://github.com/anthonybench/emoji"
 packages = [
```

### Comparing `sleepyemoji-2.1/sleepyemoji.py` & `sleepyemoji-2.2/sleepyemoji.py`

 * *Files identical despite different names*

### Comparing `sleepyemoji-2.1/toolchain/faces.py` & `sleepyemoji-2.2/toolchain/faces.py`

 * *Files identical despite different names*

### Comparing `sleepyemoji-2.1/toolchain/fetcher.py` & `sleepyemoji-2.2/toolchain/fetcher.py`

 * *Files identical despite different names*

### Comparing `sleepyemoji-2.1/toolchain/hands.py` & `sleepyemoji-2.2/toolchain/hands.py`

 * *Files identical despite different names*

### Comparing `sleepyemoji-2.1/toolchain/icons.py` & `sleepyemoji-2.2/toolchain/icons.py`

 * *Files identical despite different names*

### Comparing `sleepyemoji-2.1/toolchain/option_utils.py` & `sleepyemoji-2.2/toolchain/option_utils.py`

 * *Files identical despite different names*

### Comparing `sleepyemoji-2.1/setup.py` & `sleepyemoji-2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
  'faces',
  'fetcher',
  'hands',
  'icons',
  'people']
 setup_kwargs = {
     'name': 'sleepyemoji',
-    'version': '2.1',
+    'version': '2.2',
     'description': 'Print all the emojis that sleepyboy thinks are worthwhile!',
     'long_description': '# **SleepyEmoji**\n*Fetch your favorite emojis fast!*\n\n<br />\n\n## **Welcome to sleepyemoji!**\nThere\'s now a paralyzing volume of unicode characters known as "emojis", which is great for creative expression, but bad for fetching the ~%10 of emojis you ever care to use.\n\nSleepyEmoji has entered the chat!\n\n<br />\n\n### **Table of Contents** 📖\n<hr>\n\n  - **Get Started**\n  - Usage\n  - Technologies\n  - Contribute\n  - Acknowledgements\n  - License/Stats/Author\n\n<br />\n\n## **Get Started 🚀**\n<hr>\n\nTo Install:\n```sh\npip install sleepyemoji\n```\nTo update:\n```sh\npip install sleepyemoji --upgrade\n```\n\nAnd set a personal alias in your shell to run the following script:\n```python\nfrom sleepyemoji import sleepyemoji\nfrom sys import argv, exit\n\nsleepyemoji(argv[1:])\n\nexit(0)\n```\n\nThat\'s it! It will handle command line argument passthrough. \\\nThis document assumes the script alias to be `emoji`.\n\n<br />\n\n## **Usage ⚙**\n<hr>\n\nAfter setting up the tool, run `emoji [-h|--help]` to display this message:\n```txt\nThis tool prints emojis of one or more catgories, each defined in their own file.\nEmojis are given along with their unicode value, discord shorthand, and ios descriptor.\n\nFor the official emoji index:\n  https://unicode.org/emoji/charts/full-emoji-list.html\n\n\nProvide 1 or more options of various emoji categories, or simply request all of them.\n--------------\nAll:\n  ./main.py [-C|--complete]\nCategories:\n  /main.py [*flags]\n    [-A|--animals]\n    [-F|--faces]\n    [-H|--hands]\n    [-I|--icons]\n    [-P|--people]\n    [--combos|--combinations]\nExample:\n  ./main.py -A -H\nInfo:\n  ./main.py [-h|--help]\n--------------\n```\n\n<br />\n\n## **Technologies 🧰**\n<hr>\n\n  - Just vanilla Python3 🙂\n\n<br />\n\n## **Contribute 🤝**\n<hr>\n\nThis tool is kept in **Envi**, where emoji data is added in `emojis/toolchain` in the corresponding folders. This repository is private, thus the user must appreciate my favorite emojis, mwahahaha!\n\nRemember to pull before you push!\n\n<br />\n\n## **Acknowledgements 💙**\n<hr>\n\nThanks to my late cat Merlin, who whispered best practices in my ear while I wrote this.\n\n<br />\n\n## **License, Stats, Author 📜**\n<hr>\n\n<img align="right" alt="example image tag" src="https://i.imgur.com/jtNwEWu.png" width="200" />\n\n<!-- badge cluster -->\n\n![PyPI - License](https://img.shields.io/pypi/l/sleepyemoji?style=plastic)\n\n<!-- / -->\nSee [License](TODO) for the full license text.\n\nThis package was authored by *Isaac Yep*.',
     'author': 'anthonybench',
     'author_email': 'anythonybenchyep@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/anthonybench/emoji',
```

### Comparing `sleepyemoji-2.1/PKG-INFO` & `sleepyemoji-2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepyemoji
-Version: 2.1
+Version: 2.2
 Summary: Print all the emojis that sleepyboy thinks are worthwhile!
 Home-page: https://github.com/anthonybench/emoji
 License: GNU GPL
 Keywords: emoji,unicode
 Author: anthonybench
 Author-email: anythonybenchyep@gmail.com
 Requires-Python: >=3.10,<4.0
```

