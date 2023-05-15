# Comparing `tmp/slack-primitive-cli-0.2.0.tar.gz` & `tmp/slack_primitive_cli-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slack-primitive-cli-0.2.0.tar", max compression
+gzip compressed data, was "slack_primitive_cli-0.2.1.tar", max compression
```

## Comparing `slack-primitive-cli-0.2.0.tar` & `slack_primitive_cli-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1067 2021-02-11 16:36:30.868073 slack-primitive-cli-0.2.0/LICENSE
--rw-r--r--   0        0        0     6159 2021-11-22 13:36:15.964459 slack-primitive-cli-0.2.0/README.md
--rw-r--r--   0        0        0     1425 2021-11-22 13:36:15.964459 slack-primitive-cli-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       64 2021-02-11 16:36:30.868073 slack-primitive-cli-0.2.0/slack_primitive_cli/__init__.py
--rw-r--r--   0        0        0      356 2021-02-11 16:36:30.868073 slack-primitive-cli-0.2.0/slack_primitive_cli/__main__.py
--rw-r--r--   0        0        0       22 2021-11-22 13:35:42.860459 slack-primitive-cli-0.2.0/slack_primitive_cli/__version__.py
--rw-r--r--   0        0        0        0 2021-02-11 16:36:30.868073 slack-primitive-cli-0.2.0/slack_primitive_cli/command/__init__.py
--rw-r--r--   0        0        0     4259 2021-11-22 13:36:15.964459 slack-primitive-cli-0.2.0/slack_primitive_cli/command/chat.py
--rw-r--r--   0        0        0     2393 2021-11-22 13:36:15.964459 slack-primitive-cli-0.2.0/slack_primitive_cli/command/files.py
--rw-r--r--   0        0        0        0 2021-02-11 17:06:34.792448 slack-primitive-cli-0.2.0/slack_primitive_cli/common/__init__.py
--rw-r--r--   0        0        0     1247 2021-11-22 13:36:15.964459 slack-primitive-cli-0.2.0/slack_primitive_cli/common/utils.py
--rw-r--r--   0        0        0     7248 2021-11-22 13:36:45.956953 slack-primitive-cli-0.2.0/setup.py
--rw-r--r--   0        0        0     7296 2021-11-22 13:36:45.957376 slack-primitive-cli-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-15 07:50:24.563694 slack_primitive_cli-0.2.1/LICENSE
+-rw-r--r--   0        0        0     6159 2023-05-15 07:50:24.563694 slack_primitive_cli-0.2.1/README.md
+-rw-r--r--   0        0        0     1145 2023-05-15 07:50:47.443778 slack_primitive_cli-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       64 2023-05-15 07:50:24.563694 slack_primitive_cli-0.2.1/slack_primitive_cli/__init__.py
+-rw-r--r--   0        0        0      414 2023-05-15 07:50:24.563694 slack_primitive_cli-0.2.1/slack_primitive_cli/__main__.py
+-rw-r--r--   0        0        0      131 2023-05-15 07:50:47.443778 slack_primitive_cli-0.2.1/slack_primitive_cli/__version__.py
+-rw-r--r--   0        0        0        0 2023-05-15 07:50:24.563694 slack_primitive_cli-0.2.1/slack_primitive_cli/command/__init__.py
+-rw-r--r--   0        0        0     4259 2023-05-15 07:50:24.563694 slack_primitive_cli-0.2.1/slack_primitive_cli/command/chat.py
+-rw-r--r--   0        0        0     2393 2023-05-15 07:50:24.563694 slack_primitive_cli-0.2.1/slack_primitive_cli/command/files.py
+-rw-r--r--   0        0        0        0 2023-05-15 07:50:24.563694 slack_primitive_cli-0.2.1/slack_primitive_cli/common/__init__.py
+-rw-r--r--   0        0        0     1247 2023-05-15 07:50:24.563694 slack_primitive_cli-0.2.1/slack_primitive_cli/common/utils.py
+-rw-r--r--   0        0        0     7152 1970-01-01 00:00:00.000000 slack_primitive_cli-0.2.1/PKG-INFO
```

### Comparing `slack-primitive-cli-0.2.0/LICENSE` & `slack_primitive_cli-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `slack-primitive-cli-0.2.0/README.md` & `slack_primitive_cli-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `slack-primitive-cli-0.2.0/pyproject.toml` & `slack_primitive_cli-0.2.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,49 @@
 [tool.poetry]
 name = "slack-primitive-cli"
-version = "0.2.0"
+version = "0.2.1"  # `poetry-dynamic-versioning`を使ってGitHubのバージョンタグを取得している。変更不要
 description = "Primitive Slack CLI"
 authors = ["yuji38kwmt <yuji38kwmt@gmail.com>"]
 maintainers = ["yuji38kwmt <yuji38kwmt@gmail.com>"]
 keywords=["slack", "cli"]
 license="MIT"
 readme="README.md"
 repository="https://github.com/yuji38kwmt/slack-primitive-cli"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
     "Topic :: Utilities",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8.1"
 click = "^8"
 click-option-group = "*"
 backoff = "*"
 slack-sdk = "^3"
 
 
 [tool.poetry.dev-dependencies]
-flake8 = "*"
+flake8 = "^6"
 autoflake = "*"
-isort = "*"
-black = {version = "^21.11b0", allow-prereleases = true}
-mypy = "*"
+isort = "^5"
+black = "^23"
+mypy = "^1"
 
 [tool.poetry.scripts]
 slackcli = "slack_primitive_cli.__main__:cli"
 
 [tool.black]
 line-length = 120
 
 
 [tool.isort]
 line_length = 120
-# blackの設定に合わせる
-# https://black.readthedocs.io/en/stable/the_black_code_style.html#line-length
-multi_line_output=3
-include_trailing_comma=true
-force_grid_wrap=0
-use_parentheses=true
-[build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
 
+[tool.poetry-dynamic-versioning]
+enable = false
+format = "{base}"
+
+[build-system]
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `slack-primitive-cli-0.2.0/slack_primitive_cli/command/chat.py` & `slack_primitive_cli-0.2.1/slack_primitive_cli/command/chat.py`

 * *Files identical despite different names*

### Comparing `slack-primitive-cli-0.2.0/slack_primitive_cli/command/files.py` & `slack_primitive_cli-0.2.1/slack_primitive_cli/command/files.py`

 * *Files identical despite different names*

### Comparing `slack-primitive-cli-0.2.0/slack_primitive_cli/common/utils.py` & `slack_primitive_cli-0.2.1/slack_primitive_cli/common/utils.py`

 * *Files identical despite different names*

### Comparing `slack-primitive-cli-0.2.0/setup.py` & `slack_primitive_cli-0.2.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,191 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: slack-primitive-cli
+Version: 0.2.1
+Summary: Primitive Slack CLI
+Home-page: https://github.com/yuji38kwmt/slack-primitive-cli
+License: MIT
+Keywords: slack,cli
+Author: yuji38kwmt
+Author-email: yuji38kwmt@gmail.com
+Maintainer: yuji38kwmt
+Maintainer-email: yuji38kwmt@gmail.com
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Utilities
+Requires-Dist: backoff
+Requires-Dist: click (>=8,<9)
+Requires-Dist: click-option-group
+Requires-Dist: slack-sdk (>=3,<4)
+Project-URL: Repository, https://github.com/yuji38kwmt/slack-primitive-cli
+Description-Content-Type: text/markdown
 
-packages = \
-['slack_primitive_cli',
- 'slack_primitive_cli.command',
- 'slack_primitive_cli.common']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['backoff', 'click-option-group', 'click>=8,<9', 'slack-sdk>=3,<4']
-
-entry_points = \
-{'console_scripts': ['slackcli = slack_primitive_cli.__main__:cli']}
-
-setup_kwargs = {
-    'name': 'slack-primitive-cli',
-    'version': '0.2.0',
-    'description': 'Primitive Slack CLI',
-    'long_description': '# slack-primitive-cli\n[![Build Status](https://travis-ci.org/yuji38kwmt/slack-primitive-cli.svg?branch=master)](https://travis-ci.org/yuji38kwmt/slack-primitive-cli)\n[![PyPI version](https://badge.fury.io/py/slack-primitive-cli.svg)](https://badge.fury.io/py/slack-primitive-cli)\n[![Python Versions](https://img.shields.io/pypi/pyversions/slack-primitive-cli.svg)](https://pypi.org/project/slack-primitive-cli/)\n\n`slack-primitive-cli` can execute [Slack web api methods](https://api.slack.com/methods) from command line.\nCommand line argument is correspont to web api arguments, so `slack-primitive-cli` is **primitive**.\n\n\n# Requirements\n* Python 3.7+\n\n# Install\n\n```\n$ pip install slack-primitive-cli\n```\n\nhttps://pypi.org/project/slack-primitive-cli/\n\n\n# Usage\n\n## Sending a message\n\n```\n$ slackcli chat.postMessage --token xoxb-XXXXXXX --channel "#random" --text hello\n\n$ export SLACK_API_TOKEN=xoxb-XXXXXXX\n$ slackcli chat.postMessage  --channel "#random" --text hello\n```\n\n\n```\n$ slackcli chat.postMessage --help\n\nUsage: slackcli chat.postMessage [OPTIONS]\n\n  Sends a message to a channel. See\n  https://api.slack.com/methods/chat.postMessage\n\nOptions:\n  --token TEXT               Authentication token. If not specified, refer\n                             `SLACK_API_TOKEN` environment variable.\n                             [required]\n\n  --channel TEXT             Channel, private group, or IM channel to send\n                             message to. Can be an encoded ID, or a name. See\n                             below for more details.  [required]\n\n  --text TEXT                How this field works and whether it is required\n                             depends on other fields you use in your API call.\n                             [required]\n\n  --as_user BOOLEAN          Pass true to post the message as the authed user,\n                             instead of as a bot.\n\n  --attachments TEXT         A JSON-based array of structured attachments,\n                             presented as a URL-encoded string.\n\n  --blocks TEXT              A JSON-based array of structured blocks,\n                             presented as a URL-encoded string.\n\n  --icon_emoji TEXT          Emoji to use as the icon for this message.\n                             Overrides icon_url. Must be used in conjunction\n                             with as_user set to false, otherwise ignored. See\n                             authorship below.\n\n  --icon_url TEXT            URL to an image to use as the icon for this\n                             message. Must be used in conjunction with as_user\n                             set to false, otherwise ignored. See authorship\n                             below.\n\n  --link_names BOOLEAN       Find and link channel names and usernames.\n  --mrkdwn BOOLEAN           Disable Slack markup parsing by setting to false.\n  --parse BOOLEAN            Change how messages are treated.\n  --reply_broadcast BOOLEAN  Used in conjunction with thread_ts and indicates\n                             whether reply should be made visible to everyone\n                             in the channel or conversation.\n\n  --thread_ts TEXT           Provide another message\'s ts value to make this\n                             message a reply. Avoid using a reply\'s ts value;\n                             use its parent instead.\n\n  --unfurl_links BOOLEAN     Pass true to enable unfurling of primarily text-\n                             based content.\n\n  --unfurl_media BOOLEAN     Pass false to disable unfurling of media content.\n  --username TEXT            Set your bot\'s user name. Must be used in\n                             conjunction with as_user set to false, otherwise\n                             ignored.\n\n  --help                     Show this message and exit.\n\n```\n## Uploading files\n\n```\n$ slackcli files.upload --channels "#random" --file foo.txt\n```\n\n```\n$ slackcli files.upload  --help\nUsage: slackcli files.upload [OPTIONS]\n\n  Uploads or creates a file. See https://api.slack.com/methods/files.upload\n\nOptions:\n  --token TEXT                    Authentication token. If not specified,\n                                  refer `SLACK_API_TOKEN` environment\n                                  variable.  [required]\n\n  --channels TEXT                 Comma-separated list of channel names or IDs\n                                  where the file will be shared.  [required]\n\n  File contents: [mutually_exclusive, required]\n    --file TEXT                   File contents via multipart/form-data. If\n                                  omitting this parameter, you must submit\n                                  content.\n\n    --content TEXT                File contents via a POST variable. If\n                                  omitting this parameter, you must provide a\n                                  file.\n\n  --filename TEXT                 Filename of file.\n  --filetype TEXT                 A file type identifier. See also\n                                  https://api.slack.com/types/file#file_types\n                                  .\n\n  --initial_comment TEXT          The message text introducing the file in\n                                  specified channels.\n\n  --thread_ts TEXT                Provide another message\'s ts value to upload\n                                  this file as a reply.\n\n  --title TEXT                    Title of file.\n\n```\n\n# Supported web api methods.\n`slack-primitive-cli` supports a few web api methods.\n\n* [chat.delete](https://api.slack.com/methods/chat.delete)\n* [chat.postMessage](https://api.slack.com/methods/chat.postMessage)\n* [files.delete](https://api.slack.com/methods/files.delete)\n* [files.upload](https://api.slack.com/methods/files.upload)\n\n# Additional\n\n## Shell Completion\n`slack-primitive-cli` depends on [click](https://click.palletsprojects.com/en/7.x/), so `slack-primitive-cli` can provide tab completion.\nBash, Zsh, and Fish are supported\n\nIn order to activate shell completion, you need to execute the following script.\n\n```\n$ eval "$(_SLACKCLI_COMPLETE=source slackcli)"\n```\n\n\nSee [here](https://click.palletsprojects.com/en/7.x/bashcomplete/) for details.\n\n',
-    'author': 'yuji38kwmt',
-    'author_email': 'yuji38kwmt@gmail.com',
-    'maintainer': 'yuji38kwmt',
-    'maintainer_email': 'yuji38kwmt@gmail.com',
-    'url': 'https://github.com/yuji38kwmt/slack-primitive-cli',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+# slack-primitive-cli
+[![Build Status](https://travis-ci.org/yuji38kwmt/slack-primitive-cli.svg?branch=master)](https://travis-ci.org/yuji38kwmt/slack-primitive-cli)
+[![PyPI version](https://badge.fury.io/py/slack-primitive-cli.svg)](https://badge.fury.io/py/slack-primitive-cli)
+[![Python Versions](https://img.shields.io/pypi/pyversions/slack-primitive-cli.svg)](https://pypi.org/project/slack-primitive-cli/)
+
+`slack-primitive-cli` can execute [Slack web api methods](https://api.slack.com/methods) from command line.
+Command line argument is correspont to web api arguments, so `slack-primitive-cli` is **primitive**.
+
+
+# Requirements
+* Python 3.7+
+
+# Install
+
+```
+$ pip install slack-primitive-cli
+```
+
+https://pypi.org/project/slack-primitive-cli/
+
+
+# Usage
+
+## Sending a message
+
+```
+$ slackcli chat.postMessage --token xoxb-XXXXXXX --channel "#random" --text hello
+
+$ export SLACK_API_TOKEN=xoxb-XXXXXXX
+$ slackcli chat.postMessage  --channel "#random" --text hello
+```
+
+
+```
+$ slackcli chat.postMessage --help
+
+Usage: slackcli chat.postMessage [OPTIONS]
+
+  Sends a message to a channel. See
+  https://api.slack.com/methods/chat.postMessage
+
+Options:
+  --token TEXT               Authentication token. If not specified, refer
+                             `SLACK_API_TOKEN` environment variable.
+                             [required]
+
+  --channel TEXT             Channel, private group, or IM channel to send
+                             message to. Can be an encoded ID, or a name. See
+                             below for more details.  [required]
+
+  --text TEXT                How this field works and whether it is required
+                             depends on other fields you use in your API call.
+                             [required]
+
+  --as_user BOOLEAN          Pass true to post the message as the authed user,
+                             instead of as a bot.
+
+  --attachments TEXT         A JSON-based array of structured attachments,
+                             presented as a URL-encoded string.
+
+  --blocks TEXT              A JSON-based array of structured blocks,
+                             presented as a URL-encoded string.
+
+  --icon_emoji TEXT          Emoji to use as the icon for this message.
+                             Overrides icon_url. Must be used in conjunction
+                             with as_user set to false, otherwise ignored. See
+                             authorship below.
+
+  --icon_url TEXT            URL to an image to use as the icon for this
+                             message. Must be used in conjunction with as_user
+                             set to false, otherwise ignored. See authorship
+                             below.
+
+  --link_names BOOLEAN       Find and link channel names and usernames.
+  --mrkdwn BOOLEAN           Disable Slack markup parsing by setting to false.
+  --parse BOOLEAN            Change how messages are treated.
+  --reply_broadcast BOOLEAN  Used in conjunction with thread_ts and indicates
+                             whether reply should be made visible to everyone
+                             in the channel or conversation.
+
+  --thread_ts TEXT           Provide another message's ts value to make this
+                             message a reply. Avoid using a reply's ts value;
+                             use its parent instead.
+
+  --unfurl_links BOOLEAN     Pass true to enable unfurling of primarily text-
+                             based content.
+
+  --unfurl_media BOOLEAN     Pass false to disable unfurling of media content.
+  --username TEXT            Set your bot's user name. Must be used in
+                             conjunction with as_user set to false, otherwise
+                             ignored.
+
+  --help                     Show this message and exit.
+
+```
+## Uploading files
+
+```
+$ slackcli files.upload --channels "#random" --file foo.txt
+```
+
+```
+$ slackcli files.upload  --help
+Usage: slackcli files.upload [OPTIONS]
+
+  Uploads or creates a file. See https://api.slack.com/methods/files.upload
+
+Options:
+  --token TEXT                    Authentication token. If not specified,
+                                  refer `SLACK_API_TOKEN` environment
+                                  variable.  [required]
+
+  --channels TEXT                 Comma-separated list of channel names or IDs
+                                  where the file will be shared.  [required]
+
+  File contents: [mutually_exclusive, required]
+    --file TEXT                   File contents via multipart/form-data. If
+                                  omitting this parameter, you must submit
+                                  content.
+
+    --content TEXT                File contents via a POST variable. If
+                                  omitting this parameter, you must provide a
+                                  file.
+
+  --filename TEXT                 Filename of file.
+  --filetype TEXT                 A file type identifier. See also
+                                  https://api.slack.com/types/file#file_types
+                                  .
+
+  --initial_comment TEXT          The message text introducing the file in
+                                  specified channels.
+
+  --thread_ts TEXT                Provide another message's ts value to upload
+                                  this file as a reply.
+
+  --title TEXT                    Title of file.
+
+```
+
+# Supported web api methods.
+`slack-primitive-cli` supports a few web api methods.
+
+* [chat.delete](https://api.slack.com/methods/chat.delete)
+* [chat.postMessage](https://api.slack.com/methods/chat.postMessage)
+* [files.delete](https://api.slack.com/methods/files.delete)
+* [files.upload](https://api.slack.com/methods/files.upload)
+
+# Additional
+
+## Shell Completion
+`slack-primitive-cli` depends on [click](https://click.palletsprojects.com/en/7.x/), so `slack-primitive-cli` can provide tab completion.
+Bash, Zsh, and Fish are supported
+
+In order to activate shell completion, you need to execute the following script.
+
+```
+$ eval "$(_SLACKCLI_COMPLETE=source slackcli)"
+```
+
+
+See [here](https://click.palletsprojects.com/en/7.x/bashcomplete/) for details.
 
 
-setup(**setup_kwargs)
```

