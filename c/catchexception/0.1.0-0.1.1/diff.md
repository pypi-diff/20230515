# Comparing `tmp/catchexception-0.1.0.tar.gz` & `tmp/catchexception-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catchexception-0.1.0.tar", last modified: Thu Apr 13 16:39:34 2023, max compression
+gzip compressed data, was "catchexception-0.1.1.tar", last modified: Mon May 15 19:12:35 2023, max compression
```

## Comparing `catchexception-0.1.0.tar` & `catchexception-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 16:39:34.484684 catchexception-0.1.0/
-drwxrwxrwx   0        0        0        0 2023-04-13 16:39:34.463533 catchexception-0.1.0/CatchException/
--rw-rw-rw-   0        0        0      269 2023-04-13 16:38:46.000000 catchexception-0.1.0/CatchException/__init__.py
--rw-rw-rw-   0        0        0     1489 2023-04-13 16:11:17.000000 catchexception-0.1.0/CatchException/__main__.py
--rw-rw-rw-   0        0        0     4350 2023-04-13 16:29:59.000000 catchexception-0.1.0/CatchException/mail_sender.py
--rw-rw-rw-   0        0        0     1104 2023-04-13 16:38:16.000000 catchexception-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     3419 2023-04-13 16:39:34.483451 catchexception-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2256 2023-04-13 16:29:28.000000 catchexception-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 16:39:34.481108 catchexception-0.1.0/catchexception.egg-info/
--rw-rw-rw-   0        0        0     3419 2023-04-13 16:39:34.000000 catchexception-0.1.0/catchexception.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-04-13 16:39:34.000000 catchexception-0.1.0/catchexception.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 16:39:34.000000 catchexception-0.1.0/catchexception.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-04-13 16:39:34.000000 catchexception-0.1.0/catchexception.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-04-13 16:39:34.000000 catchexception-0.1.0/catchexception.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 16:39:34.485695 catchexception-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1981 2023-04-13 16:38:05.000000 catchexception-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 19:12:35.081545 catchexception-0.1.1/
+drwxrwxrwx   0        0        0        0 2023-05-15 19:12:34.907545 catchexception-0.1.1/ExceptNotifier/
+-rw-rw-rw-   0        0        0     4854 2023-05-15 18:54:24.000000 catchexception-0.1.1/ExceptNotifier/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 19:12:34.951228 catchexception-0.1.1/ExceptNotifier/base/
+-rw-rw-rw-   0        0        0     1387 2023-05-15 18:54:13.000000 catchexception-0.1.1/ExceptNotifier/base/__init__.py
+-rw-rw-rw-   0        0        0      541 2023-04-24 14:22:47.000000 catchexception-0.1.1/ExceptNotifier/base/beep_sender.py
+-rw-rw-rw-   0        0        0      790 2023-05-15 15:03:47.000000 catchexception-0.1.1/ExceptNotifier/base/chime_sender.py
+-rw-rw-rw-   0        0        0      523 2023-05-15 15:03:52.000000 catchexception-0.1.1/ExceptNotifier/base/desktop_sender.py
+-rw-rw-rw-   0        0        0     1009 2023-05-15 15:03:55.000000 catchexception-0.1.1/ExceptNotifier/base/discord_sender.py
+-rw-rw-rw-   0        0        0     1321 2023-04-23 07:06:25.000000 catchexception-0.1.1/ExceptNotifier/base/kakao_sender.py
+-rw-rw-rw-   0        0        0      868 2023-04-19 22:26:00.000000 catchexception-0.1.1/ExceptNotifier/base/line_sender.py
+-rw-rw-rw-   0        0        0     1863 2023-05-15 15:07:58.000000 catchexception-0.1.1/ExceptNotifier/base/mail_sender.py
+-rw-rw-rw-   0        0        0      686 2023-04-20 06:03:59.000000 catchexception-0.1.1/ExceptNotifier/base/slack_sender.py
+-rw-rw-rw-   0        0        0     1411 2023-04-23 07:06:40.000000 catchexception-0.1.1/ExceptNotifier/base/sms_sender.py
+-rw-rw-rw-   0        0        0      637 2023-04-23 15:01:26.000000 catchexception-0.1.1/ExceptNotifier/base/teams_sender.py
+-rw-rw-rw-   0        0        0      928 2023-05-15 15:08:12.000000 catchexception-0.1.1/ExceptNotifier/base/telegram_sender.py
+-rw-rw-rw-   0        0        0      580 2023-04-24 11:00:14.000000 catchexception-0.1.1/ExceptNotifier/base/wechat_sender.py
+-rw-rw-rw-   0        0        0     1454 2023-04-24 11:00:21.000000 catchexception-0.1.1/ExceptNotifier/base/whatsapp_sender.py
+drwxrwxrwx   0        0        0        0 2023-05-15 19:12:34.988906 catchexception-0.1.1/ExceptNotifier/ipycore/
+-rw-rw-rw-   0        0        0     1473 2023-05-12 21:30:21.000000 catchexception-0.1.1/ExceptNotifier/ipycore/__init__.py
+-rw-rw-rw-   0        0        0      710 2023-04-24 11:11:18.000000 catchexception-0.1.1/ExceptNotifier/ipycore/beep_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2582 2023-05-15 18:54:23.000000 catchexception-0.1.1/ExceptNotifier/ipycore/chime_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2951 2023-05-15 18:54:23.000000 catchexception-0.1.1/ExceptNotifier/ipycore/desktop_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2594 2023-05-15 18:54:22.000000 catchexception-0.1.1/ExceptNotifier/ipycore/discord_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2574 2023-05-15 18:54:22.000000 catchexception-0.1.1/ExceptNotifier/ipycore/kakao_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2588 2023-05-15 18:54:21.000000 catchexception-0.1.1/ExceptNotifier/ipycore/line_notifier_ipython.py
+-rw-rw-rw-   0        0        0     3981 2023-05-15 19:08:48.000000 catchexception-0.1.1/ExceptNotifier/ipycore/mail_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2581 2023-05-15 18:54:20.000000 catchexception-0.1.1/ExceptNotifier/ipycore/slack_notifier_ipython.py
+-rw-rw-rw-   0        0        0     3053 2023-05-15 18:54:19.000000 catchexception-0.1.1/ExceptNotifier/ipycore/sms_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2585 2023-05-15 18:54:20.000000 catchexception-0.1.1/ExceptNotifier/ipycore/teams_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2587 2023-05-15 18:54:19.000000 catchexception-0.1.1/ExceptNotifier/ipycore/telegram_notifier_ipython.py
+-rw-rw-rw-   0        0        0     2595 2023-05-15 18:54:17.000000 catchexception-0.1.1/ExceptNotifier/ipycore/wechat_notifier_ipython.py
+drwxrwxrwx   0        0        0        0 2023-05-15 19:12:35.024325 catchexception-0.1.1/ExceptNotifier/pycore/
+-rw-rw-rw-   0        0        0     2010 2023-05-15 15:02:54.000000 catchexception-0.1.1/ExceptNotifier/pycore/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 19:12:35.031851 catchexception-0.1.1/ExceptNotifier/pycore/base_handler/
+-rw-rw-rw-   0        0        0        0 2023-05-15 15:53:22.000000 catchexception-0.1.1/ExceptNotifier/pycore/base_handler/__init__.py
+-rw-rw-rw-   0        0        0     1040 2023-05-15 17:50:04.000000 catchexception-0.1.1/ExceptNotifier/pycore/base_handler/base_send_handler.py
+-rw-rw-rw-   0        0        0     1043 2023-05-15 18:02:03.000000 catchexception-0.1.1/ExceptNotifier/pycore/base_handler/base_success_handler.py
+-rw-rw-rw-   0        0        0     2229 2023-05-15 15:02:50.000000 catchexception-0.1.1/ExceptNotifier/pycore/beep_notifier.py
+-rw-rw-rw-   0        0        0     7674 2023-05-15 18:54:17.000000 catchexception-0.1.1/ExceptNotifier/pycore/chime_notifier.py
+-rw-rw-rw-   0        0        0     7251 2023-05-15 18:54:16.000000 catchexception-0.1.1/ExceptNotifier/pycore/desktop_notifier.py
+-rw-rw-rw-   0        0        0     8019 2023-05-15 15:51:05.000000 catchexception-0.1.1/ExceptNotifier/pycore/discord_notifier.py
+-rw-rw-rw-   0        0        0     8054 2023-05-15 18:54:16.000000 catchexception-0.1.1/ExceptNotifier/pycore/kakao_notifier.py
+-rw-rw-rw-   0        0        0     7626 2023-05-15 18:54:15.000000 catchexception-0.1.1/ExceptNotifier/pycore/line_notifier.py
+-rw-rw-rw-   0        0        0    10271 2023-05-15 18:54:14.000000 catchexception-0.1.1/ExceptNotifier/pycore/mail_notifier.py
+-rw-rw-rw-   0        0        0     7580 2023-05-15 18:54:14.000000 catchexception-0.1.1/ExceptNotifier/pycore/slack_notifier.py
+-rw-rw-rw-   0        0        0     7746 2023-05-15 18:54:25.000000 catchexception-0.1.1/ExceptNotifier/pycore/sms_notifier.py
+-rw-rw-rw-   0        0        0     7562 2023-05-15 18:54:14.000000 catchexception-0.1.1/ExceptNotifier/pycore/teams_notifier.py
+drwxrwxrwx   0        0        0        0 2023-05-15 19:12:35.043400 catchexception-0.1.1/ExceptNotifier/pycore/telegram/
+-rw-rw-rw-   0        0        0        0 2023-05-15 15:54:38.000000 catchexception-0.1.1/ExceptNotifier/pycore/telegram/__init__.py
+-rw-rw-rw-   0        0        0     5062 2023-05-15 19:12:08.000000 catchexception-0.1.1/ExceptNotifier/pycore/telegram/except_handler.py
+-rw-rw-rw-   0        0        0      434 2023-05-15 17:53:19.000000 catchexception-0.1.1/ExceptNotifier/pycore/telegram/send_handler.py
+-rw-rw-rw-   0        0        0      478 2023-05-15 18:02:32.000000 catchexception-0.1.1/ExceptNotifier/pycore/telegram/success_handler.py
+-rw-rw-rw-   0        0        0     7789 2023-05-15 18:54:13.000000 catchexception-0.1.1/ExceptNotifier/pycore/telegram_notifier.py
+-rw-rw-rw-   0        0        0     7613 2023-05-15 15:33:15.000000 catchexception-0.1.1/ExceptNotifier/pycore/wechat_notifier.py
+drwxrwxrwx   0        0        0        0 2023-05-15 19:12:35.051240 catchexception-0.1.1/ExceptNotifier/utils/
+-rw-rw-rw-   0        0        0      266 2023-05-12 21:30:27.000000 catchexception-0.1.1/ExceptNotifier/utils/__init__.py
+-rw-rw-rw-   0        0        0     1403 2023-04-19 19:04:19.000000 catchexception-0.1.1/ExceptNotifier/utils/kakao_token.py
+-rw-rw-rw-   0        0        0        0 2023-05-15 19:10:43.000000 catchexception-0.1.1/ExceptNotifier/utils/trace_stacker.py
+-rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 catchexception-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1755 2023-05-15 19:12:35.080547 catchexception-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      707 2023-05-15 18:39:52.000000 catchexception-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 19:12:35.077067 catchexception-0.1.1/catchexception.egg-info/
+-rw-rw-rw-   0        0        0     1755 2023-05-15 19:12:34.000000 catchexception-0.1.1/catchexception.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2390 2023-05-15 19:12:34.000000 catchexception-0.1.1/catchexception.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 19:12:34.000000 catchexception-0.1.1/catchexception.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-15 19:12:34.000000 catchexception-0.1.1/catchexception.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       60 2023-05-15 19:12:34.000000 catchexception-0.1.1/catchexception.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-15 19:12:34.000000 catchexception-0.1.1/catchexception.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 19:12:35.081545 catchexception-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     2040 2023-05-15 19:11:57.000000 catchexception-0.1.1/setup.py
```

### Comparing `catchexception-0.1.0/LICENSE` & `catchexception-0.1.1/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2019 Victor SANH and Hugging Face
+Copyright (c) 2023 MinWoo Park
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `catchexception-0.1.0/setup.py` & `catchexception-0.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,54 +1,60 @@
 import re
 
 from setuptools import find_packages
 from setuptools import setup
 
 
 def get_version():
-    filename = "CatchException/__init__.py"
+    filename = "ExceptNotifier/__init__.py"
     with open(filename) as f:
         match = re.search(r"""^__version__ = ['"]([^'"]*)['"]""", f.read(), re.M)
     if not match:
         raise RuntimeError("{} doesn't contain __version__".format(filename))
     version = match.groups()[0]
     return version
 
 
 def get_long_description():
-    with open("README.md") as f:
+    with open("README.md", encoding="UTF-8") as f:
         long_description = f.read()
         return long_description
 
 
 version = get_version()
 
 
 setup(
     name="catchexception",
-    version="0.1.0",
-    author="parkminwoo",
+    version="0.1.1",
+    author="daniel park",
     author_email="parkminwoo1991@gmail.com",
-    description="With Python's try-except statement, experience a significantly more flexible way to receive notifications.",
+    description="With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
-    url="https://github.com/dsdanielpark/CatchException",
+    url="https://github.com/dsdanielpark/ExceptNotifier",
     packages=find_packages(exclude=[]),
     python_requires=">=3.6",
-    install_requires=[],
+    install_requires=[
+        "twilio",
+        "plyer",
+        "openai",
+        "discord",
+        "sphinx-rtd-theme",
+        "Sphinx",
+        "bardapi",
+    ],
     keywords="Exception, Python, Python Exception Alarm, Error notifications, Customizable notifications, Traceback management, Single line alarm",
     classifiers=[
-        "Development Status :: 2 - Pre-Alpha",
+        "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "Natural Language :: English",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: Implementation :: CPython",
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.6',
-        'Topic :: Scientific/Engineering :: Artificial Intelligence',
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3.6",
+        "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
-    entry_points={"console_scripts": ["CatchException=CatchException.cli:main"]},
-)
+    entry_points={"console_scripts": ["ExceptNotifier=ExceptNotifier.cli:main"]},
+)
```

