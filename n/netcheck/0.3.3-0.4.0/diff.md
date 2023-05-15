# Comparing `tmp/netcheck-0.3.3.tar.gz` & `tmp/netcheck-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netcheck-0.3.3.tar", max compression
+gzip compressed data, was "netcheck-0.4.0.tar", max compression
```

## Comparing `netcheck-0.3.3.tar` & `netcheck-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-05-04 21:41:09.154313 netcheck-0.3.3/LICENSE
--rw-r--r--   0        0        0     7609 2023-05-04 21:41:09.154313 netcheck-0.3.3/README.md
--rw-r--r--   0        0        0        0 2023-05-04 21:41:09.162313 netcheck-0.3.3/netcheck/__init__.py
--rw-r--r--   0        0        0     5825 2023-05-04 21:41:09.162313 netcheck-0.3.3/netcheck/cli.py
--rw-r--r--   0        0        0     2374 2023-05-04 21:41:09.162313 netcheck-0.3.3/netcheck/dns.py
--rw-r--r--   0        0        0     2150 2023-05-04 21:41:09.162313 netcheck-0.3.3/netcheck/http.py
--rw-r--r--   0        0        0     3438 2023-05-04 21:41:09.162313 netcheck-0.3.3/netcheck/runner.py
--rw-r--r--   0        0        0     1184 2023-05-04 21:41:09.162313 netcheck-0.3.3/netcheck/validation.py
--rw-r--r--   0        0        0      232 2023-05-04 21:41:09.162313 netcheck-0.3.3/netcheck/version.py
--rw-r--r--   0        0        0      850 2023-05-04 21:41:09.170313 netcheck-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     8401 1970-01-01 00:00:00.000000 netcheck-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-15 09:52:07.646954 netcheck-0.4.0/LICENSE
+-rw-r--r--   0        0        0     8655 2023-05-15 09:52:07.646954 netcheck-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-15 09:52:07.658955 netcheck-0.4.0/netcheck/__init__.py
+-rw-r--r--   0        0        0     5829 2023-05-15 09:52:07.658955 netcheck-0.4.0/netcheck/cli.py
+-rw-r--r--   0        0        0     3790 2023-05-15 09:52:07.658955 netcheck-0.4.0/netcheck/context.py
+-rw-r--r--   0        0        0     2374 2023-05-15 09:52:07.658955 netcheck-0.4.0/netcheck/dns.py
+-rw-r--r--   0        0        0     2150 2023-05-15 09:52:07.658955 netcheck-0.4.0/netcheck/http.py
+-rw-r--r--   0        0        0     4907 2023-05-15 09:52:07.658955 netcheck-0.4.0/netcheck/runner.py
+-rw-r--r--   0        0        0     2131 2023-05-15 09:52:07.658955 netcheck-0.4.0/netcheck/validation.py
+-rw-r--r--   0        0        0      214 2023-05-15 09:52:07.658955 netcheck-0.4.0/netcheck/version.py
+-rw-r--r--   0        0        0      850 2023-05-15 09:52:07.670956 netcheck-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     9447 1970-01-01 00:00:00.000000 netcheck-0.4.0/PKG-INFO
```

### Comparing `netcheck-0.3.3/LICENSE` & `netcheck-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netcheck-0.3.3/README.md` & `netcheck-0.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Netchecks
 
 <p align="center">
-  <img alt="Netchecks Logo" src=".github/logo.png" width="150" />
+  <img alt="Netchecks Logo" src="https://raw.githubusercontent.com/hardbyte/netchecks/main/.github/logo.png" width="150" />
 </p>
 
 <div align="center">
 
 [![PyPI](https://img.shields.io/pypi/v/netcheck.svg)](https://pypi.org/project/netcheck/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/netcheck)
 [![ArtifactHub - Netchecks](https://img.shields.io/badge/ArtifactHub-Netchecks-informational)](https://artifacthub.io/packages/helm/netchecks/netchecks)
@@ -14,31 +14,35 @@
 [![PyPI Downloads](https://static.pepy.tech/badge/netcheck)](https://pypi.org/project/netcheck/)
 
 </div>
 
 **Netchecks** is a set of tools for testing network conditions and asserting that they are as expected.
 
 There are two main components:
-- **Netchecks Operator** - Kubernetes Operator that runs network checks and reports results as `PolicyReport` resources. See the [operator README](operator/README.md) for more details and the full documentation can be found at [https://docs.netchecks.io](https://docs.netchecks.io)
+- **Netchecks Operator** - Kubernetes Operator that runs network checks and reports results as `PolicyReport` resources. See the [operator README](https://github.com/hardbyte/netchecks/blob/main/operator/README.md) for more details and the full documentation can be found at [https://docs.netchecks.io](https://docs.netchecks.io)
 - **Netcheck CLI and Python Library** - Command line tool for running network checks and asserting that they are as expected. Keep reading for the quickstart.
 
 
-# Netcheck Command Line Tool Quickstart
+# Netcheck Command Line Tool
 
-`netcheck` is a configurable command line application that can be used to test network conditions are as expected.
+`netcheck` is a configurable command line application for testing network conditions are as expected. It can be used to validate DNS and HTTP connectivity and can be configured to assert that the results are as expected, for example:
+
+```shell
+netcheck http --url=https://github.com/status --validation-rule "data.body.contains('GitHub lives!') && data['status-code'] in [200, 201]"
+```
 
 ## Installation
 
-Install the Python package:
+Install the Python package from PyPi:
 
 ```
 pip install netcheck
 ```
 
-Or run with Docker:
+The cli can also be run via Docker:
 
 ```shell
 docker run -it ghcr.io/hardbyte/netchecks:main
 ```
 
 ### Individual Assertions
 
@@ -83,26 +87,27 @@
 
 ```json
 {
   "spec": {
     "type": "dns",
     "nameserver": "1.1.1.1",
     "host": "hardbyte.nz",
-    "timeout": 30.0
+    "timeout": 30.0,
+    "pattern": "\ndata['response-code'] == 'NOERROR' &&\nsize(data['A']) >= 1 && \n(timestamp(data['endTimestamp']) - timestamp(data['startTimestamp']) < duration('10s'))\n"
   },
   "data": {
     "canonical_name": "hardbyte.nz.",
-    "expiration": 1675827006.4370346,
-    "response": "id 23453\nopcode QUERY\nrcode NOERROR\nflags QR RD RA\nedns 0\npayload 1232\noption EDE 10: for DNSKEY nz., id = 13646\n;QUESTION\nhardbyte.nz. IN A\n;ANSWER\nhardbyte.nz. 985 IN A 209.58.165.79\n;AUTHORITY\n;ADDITIONAL",
+    "expiration": 1683241225.5542665,
+    "response": "id 53196\nopcode QUERY\nrcode NOERROR\nflags QR RD RA\n;QUESTION\nhardbyte.nz. IN A\n;ANSWER\nhardbyte.nz. 3600 IN A 209.58.165.79\n;AUTHORITY\n;ADDITIONAL",
     "A": [
       "209.58.165.79"
     ],
     "response-code": "NOERROR",
-    "startTimestamp": "2023-02-08T03:13:41.402313",
-    "endTimestamp": "2023-02-08T03:13:41.437115"
+    "startTimestamp": "2023-05-04T22:00:24.491750",
+    "endTimestamp": "2023-05-04T22:00:25.554344"
   },
   "status": "pass"
 }
 ```
 
 Netcheck can handle checks that are expected to fail:
 ```shell
@@ -181,63 +186,63 @@
 And the `run` command can be called:
 
 
 ```shell
 $ netcheck run --config tests/testdata/dns-config.json
 ```
 
+The output should be valid JSON containing results for each assertion.
+
+Multiple assertions with multiple rules can be specified in the config file,
+configuration can be provided to each rule such as headers and custom validation:
+
 ```json
 {
-  "type": "netcheck-output",
-  "outputVersion": "dev",
-  "metadata": {
-    "creationTimestamp": "2022-12-27T22:16:43.438696",
-    "version": "0.1.7"
-  },
   "assertions": [
-    {
-      "name": "default-dns",
-      "results": [
-        {
-          "status": "pass",
-          "spec": {
-            "type": "dns",
-            "shouldFail": false,
-            "nameserver": null,
-            "host": "github.com",
-            "timeout": null
-          },
-          "data": {
-            "startTimestamp": "2022-12-27T22:16:43.438704",
-            "A": [
-              "20.248.137.48"
-            ],
-            "endTimestamp": "2022-12-27T22:16:43.455657"
-          }
-        }
-      ]
-    }
+    {"name":  "get-with-header", "rules": [
+      {"type": "http", "url": "https://pie.dev/headers", "headers": {"X-Test-Header":  "value"}},
+      {"type": "http", "url": "https://pie.dev/headers", "headers": {"X-Header": "secret"}, "validation": "parse_json(data.body).headers['X-Header'] == 'secret'" }
+    ]}
   ]
 }
 ```
 
-Multiple assertions with multiple rules can be specified in the config file, configuration can be provided
-to each rule such as headers and custom validation:
+## External Data
+
+Finally, external context can be referenced to inject data. The following example is a valid config file, if a bit contrived:
 
 ```json
 {
   "assertions": [
-    {"name":  "get-with-header", "rules": [
-      {"type": "http", "url": "https://pie.dev/headers", "headers": {"X-Test-Header":  "value"}},
-      {"type": "http", "url": "https://pie.dev/headers", "headers": {"X-Header": "secret"}, "validation": "parse_json(data.body).headers['X-Header'] == 'secret'" }
-    ]}
+    {
+      "name": "example-assertion",
+      "rules": [
+        {
+          "type": "http",
+          "url": "{{customdata.url}}",
+          "headers": {"{{customdata.header}}": "{{ b64decode(token) }}"},
+          "validation": "parse_json(data.body).headers['X-Header'] == 'secret'"
+        }
+      ]
+    }
+  ],
+  "contexts": [
+    {"name": "customdata", "type": "inline", "data": {"url": "https://pie.dev/headers", "header": "X-Header"}},
+    {"name": "token", "type": "inline", "data": "c2VjcmV0=="},
+    {"name": "selfref", "type": "file", "path": "example-config.json"}
   ]
 }
 ```
 
+In the above example the `customdata` and `token` contexts are injected into the rule.
+The `customdata.url` is used as the URL for the request, `customdata.header` is used as the name of the header.
+The `token` is base64 decoded and used as the value of the header.
+The `selfref` context is unused but shows how to load data an external JSON file which is used extensively by the
+Kubernetes operator to inject data.
+
 ## Development
 
 Update version in pyproject.toml, push to `main` and create a release on GitHub. Pypi release will be carried
 out by GitHub actions. 
 
 Install dev dependencies with Poetry:
```

### Comparing `netcheck-0.3.3/netcheck/cli.py` & `netcheck-0.4.0/netcheck/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 from rich import print_json
 from rich.console import Console
 import typer
 from typing import List, Optional
 
 from netcheck.dns import DEFAULT_DNS_VALIDATION_RULE
-from .validation import validate_probe_result
+from .validation import evaluate_cel_with_context
 from .version import NETCHECK_VERSION
 from .http import NetcheckHttpMethod, DEFAULT_HTTP_VALIDATION_RULE
 from .runner import run_from_config, check_individual_assertion
 
 
 app = typer.Typer(no_args_is_help=True)
 logger = logging.getLogger("netcheck")
```

### Comparing `netcheck-0.3.3/netcheck/dns.py` & `netcheck-0.4.0/netcheck/dns.py`

 * *Files identical despite different names*

### Comparing `netcheck-0.3.3/netcheck/http.py` & `netcheck-0.4.0/netcheck/http.py`

 * *Files identical despite different names*

### Comparing `netcheck-0.3.3/netcheck/runner.py` & `netcheck-0.4.0/netcheck/runner.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import datetime
+import json
 import logging
 from typing import Dict
 
-from netcheck.validation import validate_probe_result
+
+from netcheck.validation import evaluate_cel_with_context
 from netcheck.version import OUTPUT_JSON_VERSION
 
 from netcheck.version import NETCHECK_VERSION
 from netcheck.dns import dns_lookup_check, DEFAULT_DNS_VALIDATION_RULE
 from netcheck.http import http_request_check, DEFAULT_HTTP_VALIDATION_RULE
+from netcheck.context import replace_template, LazyFileLoadingDict
 
 logger = logging.getLogger("netcheck.runner")
 
 
 def run_from_config(netchecks_config: Dict, err_console, verbose: bool = False):
     if verbose:
         err_console.print(f"Loaded {len(netchecks_config['assertions'])} assertions")
@@ -20,37 +23,64 @@
         "outputVersion": OUTPUT_JSON_VERSION,
         "metadata": {
             "creationTimestamp": datetime.datetime.utcnow().isoformat(),
             "version": NETCHECK_VERSION,
         },
         "assertions": [],
     }
+
+    # Load optional external contexts from the config
+    context = {}
+    for c in netchecks_config.get("contexts", []):
+        # If type is "directory", load the file at "path", parse it as JSON,
+        # then add it to the context using its "name" as the key
+        if c["type"] == "file":
+            with open(c["path"], "r") as f:
+                context[c["name"]] = json.load(f)
+        elif c["type"] == "inline":
+            context[c["name"]] = c["data"]
+        elif c["type"] == "directory":
+            # Return a Dict like object that lazy loads individual files
+            # from the directory (with caching) and add them to the context
+            context[c["name"]] = LazyFileLoadingDict(c["path"])
+        else:
+            logger.warning(f"Unknown context type '{c['type']}'")
+
+    # Replace any template strings in the config
+    netchecks_config = replace_template(netchecks_config, context)
+
     # Run each test
     for assertion in netchecks_config["assertions"]:
         assertion_results = []
         if verbose:
             err_console.print(f"Running tests for assertion '{assertion['name']}'")
         for rule in assertion["rules"]:
             result = check_individual_assertion(
                 rule["type"],
                 rule,
                 err_console=err_console,
                 validation_rule=rule.get("validation"),
+                validation_context=context,
                 verbose=verbose,
             )
             assertion_results.append(result)
 
         overall_results["assertions"].append(
             {"name": assertion["name"], "results": assertion_results}
         )
     return overall_results
 
 
 def check_individual_assertion(
-    test_type: str, test_config, err_console, validation_rule=None, verbose=False
+    test_type: str,
+    test_config,
+    err_console,
+    validation_rule=None,
+    validation_context=None,
+    verbose=False,
 ):
     match test_type:
         case "dns":
             if verbose:
                 err_console.print(f"DNS check looking up host '{test_config['host']}'")
             test_detail = dns_lookup_check(
                 host=test_config["host"],
@@ -78,15 +108,23 @@
                 validation_rule = DEFAULT_HTTP_VALIDATION_RULE
             case "dns":
                 validation_rule = DEFAULT_DNS_VALIDATION_RULE
     elif verbose:
         err_console.print("Using custom validation rule")
 
     test_detail["spec"]["pattern"] = validation_rule
-    passed = validate_probe_result(test_detail, validation_rule)
+
+    logger.info(f"Validating probe result with rule: {validation_rule}")
+    logger.info(f"Probe result: {test_detail}")
+    if validation_context is not None:
+        if "data" in validation_context or "spec" in validation_context:
+            raise ValueError("validation_context cannot contain a 'data' or 'spec' key")
+        test_detail.update(validation_context)
+
+    passed = evaluate_cel_with_context(test_detail, validation_rule)
 
     # Add the pass/status to the individual result. We also support an "expected": "fail" option
     # which will cause the test to fail if the validation passes.
     if test_config.get("expected") == "fail":
         test_detail["status"] = "fail" if passed else "pass"
     else:
         test_detail["status"] = "pass" if passed else "fail"
```

### Comparing `netcheck-0.3.3/netcheck/validation.py` & `netcheck-0.4.0/netcheck/validation.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,63 @@
+import base64
 import json
 import logging
 from typing import Dict
 
 import celpy
 from celpy import CELParseError, CELEvalError, json_to_cel
 
 logger = logging.getLogger("netcheck.validation")
 
 
-def validate_probe_result(result: Dict, validation_rule: str):
-    logger.info(f"Validating probe result with rule: {validation_rule}")
-    logger.info(f"Probe result: {result}")
+def evaluate_cel_with_context(context: Dict, validation_rule: str):
+    """
+    Evaluates a Common Expression Language (CEL) validation rule with a given context.
+
+    This function compiles the CEL validation rule into an Abstract Syntax Tree (AST),
+    creates a CEL program with additional functions (parse_json), sets up the context, and then
+    evaluates the CEL expression. If the evaluation fails due to a missing key in the
+    context, the function returns False.
+
+    Args:
+        context: A dictionary representing the context in which the validation rule
+            is evaluated. The context should be in a format that can be converted to CEL.
+        validation_rule: A CEL validation rule to be evaluated.
+
+    Returns:
+        Any: The result of the CEL expression evaluation. If the evaluation fails due to a
+            missing key in the context, the function returns False.
+
+    Raises:
+        ValueError: If the CEL expression is invalid.
+    """
 
     env = celpy.Environment()
 
     # Validate the CEL validation rule and compile to ast
     try:
         ast = env.compile(validation_rule)
     except CELParseError as e:
         print("Invalid CEL expression. Treating as error.")
         raise ValueError("Invalid CEL expression")
 
     # create the CEL program
     functions = {
         "parse_json": lambda s: json_to_cel(json.loads(s)),
+        "b64decode": lambda s: base64.b64decode(s).decode("utf-8"),
+        "b64encode": lambda s: base64.b64encode(s.encode()).decode(),
     }
     prgm = env.program(ast, functions=functions)
 
     # Set up the context
-    activation = celpy.json_to_cel(result)
+    activation = celpy.json_to_cel(context)
 
     # Evaluate the CEL expression
     try:
-        result = prgm.evaluate(activation)
+        context = prgm.evaluate(activation)
     except CELEvalError as e:
         # Note this can fail if the context is missing a key e.g. the probe
         # failed to return a value for a key that the validation rule expects
 
         return False
 
-    return result
+    return context
```

### Comparing `netcheck-0.3.3/pyproject.toml` & `netcheck-0.4.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "netcheck"
-version = "0.3.3"
+version = "0.4.0"
 description = "Netchecks is a cloud native tool for specifying and regularly checking assertions about network conditions. Use netchecks to proactively verify whether security controls are working as intended, alerting on misconfiguration."
 authors = ["Brian Thorne <brian@hardbyte.nz>"]
 readme = "README.md"
 packages = [{include = "netcheck"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `netcheck-0.3.3/PKG-INFO` & `netcheck-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netcheck
-Version: 0.3.3
+Version: 0.4.0
 Summary: Netchecks is a cloud native tool for specifying and regularly checking assertions about network conditions. Use netchecks to proactively verify whether security controls are working as intended, alerting on misconfiguration.
 Author: Brian Thorne
 Author-email: brian@hardbyte.nz
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -15,15 +15,15 @@
 Requires-Dist: rich (>=10.11.0,<14.0.0)
 Requires-Dist: typer (>=0.9,<0.10)
 Description-Content-Type: text/markdown
 
 # Netchecks
 
 <p align="center">
-  <img alt="Netchecks Logo" src=".github/logo.png" width="150" />
+  <img alt="Netchecks Logo" src="https://raw.githubusercontent.com/hardbyte/netchecks/main/.github/logo.png" width="150" />
 </p>
 
 <div align="center">
 
 [![PyPI](https://img.shields.io/pypi/v/netcheck.svg)](https://pypi.org/project/netcheck/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/netcheck)
 [![ArtifactHub - Netchecks](https://img.shields.io/badge/ArtifactHub-Netchecks-informational)](https://artifacthub.io/packages/helm/netchecks/netchecks)
@@ -32,31 +32,35 @@
 [![PyPI Downloads](https://static.pepy.tech/badge/netcheck)](https://pypi.org/project/netcheck/)
 
 </div>
 
 **Netchecks** is a set of tools for testing network conditions and asserting that they are as expected.
 
 There are two main components:
-- **Netchecks Operator** - Kubernetes Operator that runs network checks and reports results as `PolicyReport` resources. See the [operator README](operator/README.md) for more details and the full documentation can be found at [https://docs.netchecks.io](https://docs.netchecks.io)
+- **Netchecks Operator** - Kubernetes Operator that runs network checks and reports results as `PolicyReport` resources. See the [operator README](https://github.com/hardbyte/netchecks/blob/main/operator/README.md) for more details and the full documentation can be found at [https://docs.netchecks.io](https://docs.netchecks.io)
 - **Netcheck CLI and Python Library** - Command line tool for running network checks and asserting that they are as expected. Keep reading for the quickstart.
 
 
-# Netcheck Command Line Tool Quickstart
+# Netcheck Command Line Tool
 
-`netcheck` is a configurable command line application that can be used to test network conditions are as expected.
+`netcheck` is a configurable command line application for testing network conditions are as expected. It can be used to validate DNS and HTTP connectivity and can be configured to assert that the results are as expected, for example:
+
+```shell
+netcheck http --url=https://github.com/status --validation-rule "data.body.contains('GitHub lives!') && data['status-code'] in [200, 201]"
+```
 
 ## Installation
 
-Install the Python package:
+Install the Python package from PyPi:
 
 ```
 pip install netcheck
 ```
 
-Or run with Docker:
+The cli can also be run via Docker:
 
 ```shell
 docker run -it ghcr.io/hardbyte/netchecks:main
 ```
 
 ### Individual Assertions
 
@@ -101,26 +105,27 @@
 
 ```json
 {
   "spec": {
     "type": "dns",
     "nameserver": "1.1.1.1",
     "host": "hardbyte.nz",
-    "timeout": 30.0
+    "timeout": 30.0,
+    "pattern": "\ndata['response-code'] == 'NOERROR' &&\nsize(data['A']) >= 1 && \n(timestamp(data['endTimestamp']) - timestamp(data['startTimestamp']) < duration('10s'))\n"
   },
   "data": {
     "canonical_name": "hardbyte.nz.",
-    "expiration": 1675827006.4370346,
-    "response": "id 23453\nopcode QUERY\nrcode NOERROR\nflags QR RD RA\nedns 0\npayload 1232\noption EDE 10: for DNSKEY nz., id = 13646\n;QUESTION\nhardbyte.nz. IN A\n;ANSWER\nhardbyte.nz. 985 IN A 209.58.165.79\n;AUTHORITY\n;ADDITIONAL",
+    "expiration": 1683241225.5542665,
+    "response": "id 53196\nopcode QUERY\nrcode NOERROR\nflags QR RD RA\n;QUESTION\nhardbyte.nz. IN A\n;ANSWER\nhardbyte.nz. 3600 IN A 209.58.165.79\n;AUTHORITY\n;ADDITIONAL",
     "A": [
       "209.58.165.79"
     ],
     "response-code": "NOERROR",
-    "startTimestamp": "2023-02-08T03:13:41.402313",
-    "endTimestamp": "2023-02-08T03:13:41.437115"
+    "startTimestamp": "2023-05-04T22:00:24.491750",
+    "endTimestamp": "2023-05-04T22:00:25.554344"
   },
   "status": "pass"
 }
 ```
 
 Netcheck can handle checks that are expected to fail:
 ```shell
@@ -199,63 +204,63 @@
 And the `run` command can be called:
 
 
 ```shell
 $ netcheck run --config tests/testdata/dns-config.json
 ```
 
+The output should be valid JSON containing results for each assertion.
+
+Multiple assertions with multiple rules can be specified in the config file,
+configuration can be provided to each rule such as headers and custom validation:
+
 ```json
 {
-  "type": "netcheck-output",
-  "outputVersion": "dev",
-  "metadata": {
-    "creationTimestamp": "2022-12-27T22:16:43.438696",
-    "version": "0.1.7"
-  },
   "assertions": [
-    {
-      "name": "default-dns",
-      "results": [
-        {
-          "status": "pass",
-          "spec": {
-            "type": "dns",
-            "shouldFail": false,
-            "nameserver": null,
-            "host": "github.com",
-            "timeout": null
-          },
-          "data": {
-            "startTimestamp": "2022-12-27T22:16:43.438704",
-            "A": [
-              "20.248.137.48"
-            ],
-            "endTimestamp": "2022-12-27T22:16:43.455657"
-          }
-        }
-      ]
-    }
+    {"name":  "get-with-header", "rules": [
+      {"type": "http", "url": "https://pie.dev/headers", "headers": {"X-Test-Header":  "value"}},
+      {"type": "http", "url": "https://pie.dev/headers", "headers": {"X-Header": "secret"}, "validation": "parse_json(data.body).headers['X-Header'] == 'secret'" }
+    ]}
   ]
 }
 ```
 
-Multiple assertions with multiple rules can be specified in the config file, configuration can be provided
-to each rule such as headers and custom validation:
+## External Data
+
+Finally, external context can be referenced to inject data. The following example is a valid config file, if a bit contrived:
 
 ```json
 {
   "assertions": [
-    {"name":  "get-with-header", "rules": [
-      {"type": "http", "url": "https://pie.dev/headers", "headers": {"X-Test-Header":  "value"}},
-      {"type": "http", "url": "https://pie.dev/headers", "headers": {"X-Header": "secret"}, "validation": "parse_json(data.body).headers['X-Header'] == 'secret'" }
-    ]}
+    {
+      "name": "example-assertion",
+      "rules": [
+        {
+          "type": "http",
+          "url": "{{customdata.url}}",
+          "headers": {"{{customdata.header}}": "{{ b64decode(token) }}"},
+          "validation": "parse_json(data.body).headers['X-Header'] == 'secret'"
+        }
+      ]
+    }
+  ],
+  "contexts": [
+    {"name": "customdata", "type": "inline", "data": {"url": "https://pie.dev/headers", "header": "X-Header"}},
+    {"name": "token", "type": "inline", "data": "c2VjcmV0=="},
+    {"name": "selfref", "type": "file", "path": "example-config.json"}
   ]
 }
 ```
 
+In the above example the `customdata` and `token` contexts are injected into the rule.
+The `customdata.url` is used as the URL for the request, `customdata.header` is used as the name of the header.
+The `token` is base64 decoded and used as the value of the header.
+The `selfref` context is unused but shows how to load data an external JSON file which is used extensively by the
+Kubernetes operator to inject data.
+
 ## Development
 
 Update version in pyproject.toml, push to `main` and create a release on GitHub. Pypi release will be carried
 out by GitHub actions. 
 
 Install dev dependencies with Poetry:
```

