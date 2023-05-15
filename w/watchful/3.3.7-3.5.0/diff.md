# Comparing `tmp/watchful-3.3.7.tar.gz` & `tmp/watchful-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "watchful-3.5.0.tar", last modified: Thu Apr  6 12:17:55 2023, max compression
```

## Comparing `watchful-3.3.7.tar` & `watchful-3.5.0.tar`

### file list

```diff
@@ -1,11 +1,31 @@
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 watchful-3.3.7/src/watchful/__about__.py
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 watchful-3.3.7/src/watchful/__init__.py
--rw-r--r--   0        0        0    39457 2020-02-02 00:00:00.000000 watchful-3.3.7/src/watchful/attributes.py
--rw-r--r--   0        0        0    49486 2020-02-02 00:00:00.000000 watchful-3.3.7/src/watchful/client.py
--rw-r--r--   0        0        0    15852 2020-02-02 00:00:00.000000 watchful-3.3.7/src/watchful/enrich.py
--rw-r--r--   0        0        0     6666 2020-02-02 00:00:00.000000 watchful-3.3.7/src/watchful/enricher.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 watchful-3.3.7/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 watchful-3.3.7/LICENSE
--rw-r--r--   0        0        0     5754 2020-02-02 00:00:00.000000 watchful-3.3.7/README.md
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 watchful-3.3.7/pyproject.toml
--rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 watchful-3.3.7/PKG-INFO
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-06 12:17:55.945730 watchful-3.5.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1075 2023-04-06 12:14:03.000000 watchful-3.5.0/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      261 2023-04-06 12:14:03.000000 watchful-3.5.0/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2650 2023-04-06 12:17:55.945730 watchful-3.5.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6405 2023-04-06 12:14:03.000000 watchful-3.5.0/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2064 2023-04-06 12:14:03.000000 watchful-3.5.0/README_PYPI.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1554 2023-04-06 12:14:03.000000 watchful-3.5.0/README_PY_ENV.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-06 12:17:55.945730 watchful-3.5.0/examples/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   325333 2023-04-06 12:14:03.000000 watchful-3.5.0/examples/api_intro.ipynb
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1900 2023-04-06 12:14:03.000000 watchful-3.5.0/examples/requirements_api_intro.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      998 2023-04-06 12:14:03.000000 watchful-3.5.0/pylama.ini
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      375 2023-04-06 12:14:03.000000 watchful-3.5.0/pyproject.toml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      983 2023-04-06 12:17:55.949730 watchful-3.5.0/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-06 12:17:55.941730 watchful-3.5.0/src/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-06 12:17:55.945730 watchful-3.5.0/src/watchful/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        5 2023-04-06 12:14:03.000000 watchful-3.5.0/src/watchful/VERSION
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      575 2023-04-06 12:14:03.000000 watchful-3.5.0/src/watchful/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    39332 2023-04-06 12:14:03.000000 watchful-3.5.0/src/watchful/attributes.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    48367 2023-04-06 12:14:03.000000 watchful-3.5.0/src/watchful/client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15767 2023-04-06 12:14:03.000000 watchful-3.5.0/src/watchful/enrich.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6356 2023-04-06 12:14:03.000000 watchful-3.5.0/src/watchful/enricher.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-06 12:17:55.945730 watchful-3.5.0/src/watchful.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2650 2023-04-06 12:17:55.000000 watchful-3.5.0/src/watchful.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      587 2023-04-06 12:17:55.000000 watchful-3.5.0/src/watchful.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-06 12:17:55.000000 watchful-3.5.0/src/watchful.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       93 2023-04-06 12:17:55.000000 watchful-3.5.0/src/watchful.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2023-04-06 12:17:55.000000 watchful-3.5.0/src/watchful.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-06 12:17:55.945730 watchful-3.5.0/tests/
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      388 2023-04-06 12:14:03.000000 watchful-3.5.0/tests/test_0000_import_sdk.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2691 2023-04-06 12:14:03.000000 watchful-3.5.0/tests/test_0001_sdk_version_and_default_conn.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      772 2023-04-06 12:14:03.000000 watchful-3.5.0/tests/test_0002_encoding.py
```

### Comparing `watchful-3.3.7/src/watchful/attributes.py` & `watchful-3.5.0/src/watchful/attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """
 This script provides the functions required for data enrichment.
 """
-# mypy: ignore-errors
+################################################################################
+
 
 import csv
 import io
 import json
+import numbers
 import os
 import pprint
 import re
 from heapq import merge
 from multiprocessing import Pool
 from typing import Callable, Dict, List, Optional, Tuple
 import psutil
@@ -78,29 +80,38 @@
 
     assert multiproc_chunksize >= 1
     if IS_MULTIPROC:
         global MULTIPROC_CHUNKSIZE
         MULTIPROC_CHUNKSIZE = multiproc_chunksize
 
 
-# XXX: rockstar (1 May 2023) - This is not base64 encoding, so I'm not
-# sure why it's being named that. It might _look_ like base64 encoding
-# on the output, but it isn't. As it's not actually a standard format,
-# we now have to have parsers/generators in both rust and python. This
-# is not ideal.
+def print_multiproc_params() -> None:
+    """
+    This function prints the multiprocessing flag and the multiprocessing chunk
+    size for the data enrichment. This is still in internal alpha mode and is
+    not expected to be used by user.
+    """
+
+    print(
+        f"multiprocessing: {IS_MULTIPROC}, "
+        f"multiprocessing chunksize: {MULTIPROC_CHUNKSIZE}"
+    )
+
+
 def base64(num: int) -> str:
     """
     This function takes in an integer value and returns its encoded string
     value.
 
     :param num: The integer value.
     :type num: int
     :return: The encoded string value.
     :rtype: str
     """
+
     if num == 0:
         return NUMERALS[0]
 
     ret = ""
     while num > 0:
         ret += NUMERALS[num % BASE]
         num = num // BASE
@@ -257,25 +268,22 @@
             # Gather and create new mappings at the same time. Duh :)
             for attr, vals in attr_vals.items():
                 if attr not in attrs:
                     attrs[attr] = len(attrs) + 1
                     values[attr] = {}
                     new_attrs.append(attr)
                 for val in vals:
-                    if isinstance(val, (int, float, bool)):
+                    if isinstance(val, numbers.Number):
                         val = str(val)
-                    elif val is None:
-                        pass
-                    elif val == "" or not isinstance(val, str):
-                        raise ValueError(
-                            "Attribute value needs to be either a non-empty "
-                            f"string, int, float, bool or None; got {val} "
-                            "instead."
+                    elif val and not isinstance(val, str):
+                        raise Exception(
+                            "Attribute value must be a string, "
+                            "None or a number. Was: " + val
                         )
-                    if val and val not in values[attr]:
+                    if val and not val in values[attr]:
                         values[attr][val] = len(values[attr]) + 1
                         if attr not in new_values:
                             new_values[attr] = []
                         new_values[attr].append(val)
 
             # Create the vector for the current cell.
             span_val = []
@@ -285,20 +293,15 @@
                 assert len(span) == len(
                     vals
                 ), "Must be the same amount of spans as attribute values."
                 # Not base64 the attributes to save space since there aren't
                 # that many of them.
                 span_val.append(attrs[attr])
                 span_val.append(
-                    base64str(
-                        [
-                            0 if val is None else values[attr][str(val)]
-                            for val in vals
-                        ]
-                    )
+                    base64str([values[attr][val] if val else 0 for val in vals])
                 )
 
             cell.append(base64str(contig_spans(span)))
             cell.append(span_val)
 
         # Output the lines (attributes, values and the cell value itself).
         if new_attrs:
@@ -354,15 +357,15 @@
         subjectivity,
         _,
     ) in doc._.blob.sentiment_assessments.assessments:
         for word in words:
             regex = re.compile(f"\\b{re.escape(word)}\\b")
             for m in regex.finditer(doc.text):
                 span = m.span()
-                if span not in assessments:
+                if not span in assessments:
                     assessments[span] = (1, [polarity], [subjectivity])
                 else:
                     (c, ps, ss) = assessments.get(span)
                     ps.append(polarity)
                     ss.append(subjectivity)
                     assessments[span] = (c + 1, ps, ss)
     assess_spans = []
@@ -467,15 +470,15 @@
     :type nlp: Callable
     :return: The enriched cell.
     :rtype: enricher.EnrichedCell
     """
 
     # Adding spacytextblob, cannot do it in load_spacy because of
     # our multiprocessing code. Adding a pipe to SpaCy is idempotent.
-    from spacytextblob.spacytextblob import (  # noqa: F401
+    from spacytextblob.spacytextblob import (  # pylint: disable=unused-import
         SpacyTextBlob,
     )
 
     if not nlp.has_pipe("spacytextblob"):
         nlp.add_pipe("spacytextblob")
     return spacy_atterize_(nlp(cell))
 
@@ -1165,13 +1168,13 @@
     summary = client._assert_success(summary)
     dataset_id = client.get_dataset_id(summary)
     datasets_dir = client.get_datasets_dir(summary, is_local)
 
     if in_file != "":
         # Check that ``in_file`` exists.
         if not os.path.isfile(in_file):
-            raise FileNotFoundError(f"File {in_file} does not exist.")
+            raise Exception(f"File {in_file} does not exist.")
         dataset_filepath = in_file
     else:
         dataset_filepath = client.get_dataset_filepath(summary, is_local)
 
     return dataset_id, datasets_dir, dataset_filepath
```

### Comparing `watchful-3.3.7/src/watchful/client.py` & `watchful-3.5.0/src/watchful/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,28 @@
 """
 This script provides the functions required for interacting directly with
 Watchful client application.
 """
+################################################################################
+
 
 import base64
 import csv
 import io
 import json
 import os
 import socket
 import subprocess
 import sys
 import time
 import urllib
-from typing import (
-    Any,
-    Callable,
-    Dict,
-    Generator,
-    List,
-    Literal,
-    Optional,
-    Union,
-    Mapping,
-)
+from typing import Callable, Dict, Generator, List, Literal, Optional, Union
 from uuid import uuid4
-
-import chardet
 import requests
 
-from watchful.__about__ import __version__
-
 
 THIS_DIR_PATH = os.path.dirname(os.path.abspath(__file__))
 SCHEME: Literal["http", "https"] = "http"
 HOST: str = "localhost"
 PORT: Optional[str] = "9002"
 API_TIMEOUT_SEC: int = 600
 
@@ -43,15 +31,15 @@
     """
     This function explicitly refreshes the imported ``watchful`` package.
     """
 
     del sys.modules["watchful"]
     import watchful
 
-    print(f"watchful version: {watchful.__about__.__version__}")
+    print(f"watchful version: {watchful.__version__}")
 
 
 def _get_conn_url() -> str:
     """
     This function creates the HTTP connection url from the global ``SCHEME``,
     ``HOST`` and ``PORT``.
 
@@ -84,25 +72,18 @@
         sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         sock.settimeout(timeout_sec)
         res = sock.connect_ex((HOST, port))
         if res == 0:
             return None
         time.sleep(0.001)
 
-    raise TimeoutError("Timed out waiting for Watchful to start")
+    raise Exception("Timed out waiting for Watchful to start")
 
 
-def spawn_cmd(
-    cmd: str,
-    env: Union[
-        Mapping[bytes, Union[str, bytes, os.PathLike[str], os.PathLike[bytes]]],
-        Mapping[str, Union[str, bytes, os.PathLike[str], os.PathLike[bytes]]],
-        None,
-    ] = None,
-) -> int:
+def spawn_cmd(cmd: str, env: str = None) -> int:
     """
     This function spawns a command and returns the PID of the spawned process.
 
     :param cmd: The command.
     :type cmd: str
     :param env: The environment, defaults to None.
     :type env: str, optional
@@ -148,22 +129,22 @@
         if pred(summary):
             return summary
         if prev_summary == summary:
             end = time.time_ns() + (unchanged_timeout * 1_000_000_000)
         prev_summary = summary
         time.sleep(0.03)  # 30ms sleep for ~30 requests per second
 
-    raise requests.exceptions.Timeout(
+    raise Exception(
         "Timed out awaiting summary. Summary went stale for "
         + str(unchanged_timeout)
         + " seconds"
     )
 
 
-def _assert_success(summary: Dict) -> Dict:
+def _assert_success(summary: Dict) -> Optional[Dict]:
     """
     This function raises an exception if summary contains "error_msg", otherwise
     it returns the summary.
 
     :param summary: The dictionary of the HTTP response from a connection
         request.
     :type summary: Dict
@@ -171,15 +152,15 @@
     :rtype: Dict, optional
     """
 
     if "error_msg" in summary and summary["error_msg"]:
         verb_str = ""
         if "error_verb" in summary and summary["error_verb"]:
             verb_str = f' ({summary["error_verb"]})'
-        raise ValueError(f'Summary error{verb_str}: {summary["error_msg"]}')
+        raise Exception(f'Summary error{verb_str}: {summary["error_msg"]}')
 
     return summary
 
 
 # as used by register_summary_string_hook
 API_SUMMARY_HOOK_CALLBACK = None
 
@@ -199,15 +180,15 @@
     """
     global API_SUMMARY_HOOK_CALLBACK
     API_SUMMARY_HOOK_CALLBACK = function
 
 
 def _read_response(
     response: requests.models.Response, response_is_summary: bool = False
-) -> Dict:
+) -> Optional[Dict]:
     """
     This function raises an exception if ``response.status_code`` is not 200,
     otherwise it returns ``ret``.
 
     If ``response_is_summary`` then we will also run the
     ``API_SUMMARY_HOOK_CALLBACK`` (any hook that was provided), so this is only
     appropriate for endpoints that return a summary, that is, the /api endpoint
@@ -238,64 +219,54 @@
     if "error_msg" in ret and ret["error_msg"]:
         print(f'{ret["error_verb"]}: {ret["error_msg"]}')
 
     return ret
 
 
 def request(
-    method: str = "GET",
-    path: str = "/",
-    headers: Optional[Dict[str, str]] = None,
-    data: Optional[Union[str, bytes, io.TextIOWrapper]] = None,
-    timeout: Optional[int] = None,
-    stream: Optional[bool] = False,
+    method: str = "GET", path: str = "/", **kwargs: Dict
 ) -> requests.models.Response:
     """
     This is a wrapper function for API calls; made up of the API method, path
     and optional keyword arguments.
 
     :param method: The API method string in uppercase.
     :type method: str
     :param path: The path string after the hostname and port.
     :type path: str
     :param kwargs: Optional parameters to include in the API call.
     :type kwargs: Dict
     :return: The HTTP response from the connection request.
     :rtype: requests.models.Response
     """
-    default_headers = {"x-watchful-sdk": __version__}
 
-    if headers is None:
-        headers = {}
+    methods = ["GET", "POST", "PUT"]
+    assert (
+        method in methods
+    ), f"{method} is not one of the currently implemented methods: {methods}!"
+
+    default_headers = {}
+    version_filepath = os.path.join(THIS_DIR_PATH, "VERSION")
+    with open(version_filepath, encoding="utf-8") as f:
+        version = f.readline()
+        default_headers.update({"x-watchful-sdk": version})
+
+    headers = kwargs.get("headers", {})
     if headers == {}:
         headers.update(default_headers)
+        kwargs["headers"] = headers
     else:
         headers.update(default_headers)
 
-    path = f"{_get_conn_url()}{path}"
-
-    if method == "GET":
-        return requests.get(
-            path, headers=headers, data=data, timeout=timeout, stream=stream
-        )
-    elif method == "POST":
-        return requests.post(
-            path, headers=headers, data=data, timeout=timeout, stream=stream
-        )
-    elif method == "PUT":
-        return requests.put(
-            path, headers=headers, data=data, timeout=timeout, stream=stream
-        )
-    else:
-        raise ValueError(
-            f"{method} is not one of the currently implemented methods: GET, POST, PUT!"
-        )
+    return getattr(requests, method.lower())(
+        f"{_get_conn_url()}{path}", **kwargs
+    )
 
 
-def api(verb: str, **kwargs: Any) -> Dict:
+def api(verb: str, **kwargs: Dict) -> Optional[Dict]:
     """
     This is a convenience function for API calls; made up of a verb and optional
     keyword arguments.
 
     :param verb: The verb for the API.
     :type verb: str
     :param kwargs: Optional parameters to support the API for ``verb``.
@@ -306,31 +277,30 @@
 
     action = kwargs  # already a dictionary
     action["verb"] = verb
 
     return api_send_action(action)
 
 
-def api_send_action(action: Dict[str, str]) -> Dict:
+def api_send_action(action: Dict) -> Optional[Dict]:
     """
     This is a convenience function for API calls with an action.
 
     :param action: The ``verb`` for the API with optional parameters.
     :type action: Dict
     :return: The dictionary of the HTTP response from the connection request.
     :rtype: Dict, optional
     """
 
-    response = request(
-        "POST",
-        "/api",
-        headers={"Content-type": "application/json"},
-        data=json.dumps(action),
-        timeout=API_TIMEOUT_SEC,
-    )
+    fields = {
+        "data": json.dumps(action),
+        "headers": {"Content-Type": "application/json"},
+        "timeout": API_TIMEOUT_SEC,
+    }
+    response = request("POST", "/api", **fields)
 
     return _read_response(response, response_is_summary=True)
 
 
 def ephemeral(port: str = "9002") -> None:
     """
     This function starts the backend using the specified ``port`` for an
@@ -345,17 +315,15 @@
         f">watchful_ephemeral_output.txt 2>&1"
     )
     await_port_opening(int(port))
     external(port=port)
 
 
 def external(
-    host: str = "localhost",
-    port: str = "9001",
-    scheme: Literal["http", "https"] = "http",
+    host: str = "localhost", port: str = "9001", scheme: str = "http"
 ) -> None:
     """
     This function changes the global ``HOST``, ``PORT`` and ``SCHEME`` values.
 
     :param host: The host, defaults to "localhost".
     :type host: str, optional
     :param port: The port, defaults to "9001".
@@ -371,15 +339,15 @@
 
     global SCHEME, HOST, PORT
     SCHEME = scheme
     HOST = host
     PORT = port
 
 
-def list_projects() -> List[Dict[str, Union[str, bool]]]:
+def list_projects() -> Dict:
     """
     This function lists the available projects.
 
     :return: The dictionary of the HTTP response from the connection request.
     :rtype: Dict
     """
 
@@ -409,15 +377,15 @@
 
     ret = response.content.decode("utf-8")
     await_plabels()
 
     return ret
 
 
-def create_project(title_: Optional[str] = None) -> Union[str, Dict]:
+def create_project(title_: Optional[str] = None) -> Union[str, Optional[Dict]]:
     """
     This function creates a new project. Additionally, if title is supplied, a
     title is given to the newly created project.
 
     :param title: The title for the project.
     :type title: str, optional
     :return: If a title is supplied and ``open_project("new")`` is successful,
@@ -430,15 +398,15 @@
     ret = open_project("new")
 
     if title_ is not None and ret == '"OK"\n':
         return title(title_)
     return ret
 
 
-def title(title_: str) -> Dict:
+def title(title_: str) -> Optional[Dict]:
     """
     This function gives a title to a newly created project.
 
     :param title_: The title for the project.
     :type title_: str
     :return: The dictionary of the HTTP response from the connection request.
     :rtype: Dict, optional
@@ -459,15 +427,15 @@
     :return: The project id.
     :rtype: str
     """
 
     if "project_id" in summary:
         return summary["project_id"]
 
-    raise WatchfulAppInstanceError("No project is currently active.")
+    raise Exception("No project is currently active.")
 
 
 def get_dataset_id(summary: Dict) -> str:
     """
     This function gets the active dataset id from ``summary``. For correctness,
     we use the ``summary`` that has been success asserted via
     ``_assert_success``.
@@ -479,19 +447,19 @@
     :rtype: str
     """
 
     if "datasets" in summary:
         # ``dataset_ids`` should either be empty or contain one dataset id.
         dataset_ids = summary["datasets"]
         if len(dataset_ids) == 0:
-            raise WatchfulAppInstanceError("No dataset is currently opened.")
+            raise Exception("No dataset is currently opened.")
         dataset_id = dataset_ids[0]
         return dataset_id
 
-    raise WatchfulAppInstanceError("`datasets` is currently not available.")
+    raise Exception("`datasets` is currently not available.")
 
 
 def get_watchful_home(summary: Dict, is_local: bool = True) -> str:
     """
     This function gets Watchful home from ``summary``. For correctness, we use
     the summary that has been success asserted via ``_assert_success``. If
     Watchful home is not available and the Watchful application is local, we
@@ -510,17 +478,15 @@
     if "watchful_home" in summary:
         return summary["watchful_home"]
     if is_local:
         user_home = os.path.expanduser("~")
         watchful_home = os.path.join(user_home, "watchful")
         return watchful_home
 
-    raise WatchfulAppInstanceError(
-        "`watchful_home` is currently not available."
-    )
+    raise Exception("`watchful_home` is currently not available.")
 
 
 def get_datasets_dir(summary: Dict, is_local: bool = True) -> str:
     """
     This function infers the datasets directory from ``summary``. For
     correctness, we use the summary that has been success asserted via
     ``_assert_success``.
@@ -562,22 +528,22 @@
 
     datasets_dir = get_datasets_dir(summary, is_local)
     dataset_id = get_dataset_id(summary)
     dataset_ref_path = os.path.join(datasets_dir, "refs", dataset_id)
 
     # Check that ``dataset_ref_path`` exists.
     if not os.path.isfile(dataset_ref_path):
-        raise FileNotFoundError(f"File {dataset_ref_path} does not exist.")
+        raise Exception(f"File {dataset_ref_path} does not exist.")
     with open(dataset_ref_path, encoding="utf-8") as f:
         dataset_ref = f.readline()
     dataset_filepath = os.path.join(datasets_dir, "raw", dataset_ref)
 
     # Check that ``dataset_filepath`` exists.
     if not os.path.isfile(dataset_filepath):
-        raise FileNotFoundError(f"File {dataset_filepath} does not exist.")
+        raise Exception(f"File {dataset_filepath} does not exist.")
 
     return dataset_filepath
 
 
 # def poll():
 #     pass
 
@@ -768,16 +734,14 @@
     :return: The fields.
     :rtype: Generator[List[str], None, None]
     """
 
     page = 0
     while True:
         summary = query(q, page)
-        if summary is None:
-            break
         for fields in [cand["fields"] for cand in summary["candidates"]]:
             yield fields
         page += 1
         if summary["query_end"] or max_pages and page == max_pages:
             break
 
 
@@ -803,15 +767,15 @@
     :return: The dictionary of the HTTP response from the connection request.
     :rtype: Dict, optional
     """
 
     return await_summary(lambda s: s["status"] == "current")
 
 
-def hinter_async(class__: str, query_: str, weight: int) -> Dict:
+def hinter_async(class__: str, query_: str, weight: int) -> Optional[Dict]:
     """
     This function creates a hinter. As it is asynchronous, the immediate HTTP
     response is likely not updated yet.
 
     :param class__: The class for the hinter.
     :type class__: str
     :param query_: The query for the hinter.
@@ -865,15 +829,15 @@
     :return: The dictionary of the HTTP response from the connection request.
     :rtype: Dict, optional
     """
 
     return api("delete", class_name=class__)
 
 
-def get() -> Dict:
+def get() -> Optional[Dict]:
     """
     This function gets the current status of the Watchful application,
     containing information such as your currently active project, dataset
     examples (candidates) and classes, hinters created, hand labels and label
     distribution, confidences and error rate, recall and precision and many
     more.
 
@@ -910,15 +874,15 @@
 
     return await_plabels()
 
 
 def upload_attributes(
     dataset_id: str,
     attributes_filepath: str,
-) -> Dict:
+) -> Optional[Dict]:
     """
     This function uploads the attributes for the ``dataset_id`` to the remote
     Watchful application, where the Watchful application then saves it to a
     filepath according to its stable application logic.
 
     :param dataset_id: The dataset id.
     :type dataset_id: str
@@ -943,15 +907,15 @@
 
     return _assert_success(_read_response(response))
 
 
 def load_attributes(
     dataset_id: str,
     attributes_filename: str,
-) -> Dict:
+) -> Optional[Dict]:
     """
     This function is used in the case of Watchful application being on the same
     machine as the data enrichment.
 
     :param dataset_id: The dataset id.
     :type dataset_id: str
     :param attributes_filename: The attributes filename.
@@ -959,15 +923,15 @@
     :return: The dictionary of the HTTP response from the connection request.
     :rtype: Dict, optional
     """
 
     return api("attributes", id=dataset_id, file=attributes_filename)
 
 
-def _dump(offset: int) -> Dict:
+def _dump(offset: int) -> Optional[Dict]:
     """
     This function returns a chunk of candidates in "hint API order".
 
     :param offset: The offset chunk.
     :type offset: int
     :return: The dictionary of the HTTP response from the connection request.
     :rtype: Dict, optional
@@ -1025,15 +989,15 @@
     :type values: List[bool]
     :return: The dictionary of the HTTP response from the connection request.
     :rtype: Dict, optional
 
     TODO: Come up with a better streaming Python API here.
     """
 
-    values = list(map(lambda x: x, values))
+    values = list(map(lambda x: x and 1 or 0, values))
 
     return _assert_success(api("hint", name=name, offset=offset, values=values))
 
 
 def apply_hints(name: str) -> Optional[Dict]:
     """
     This function applies the hints for an external hinter.
@@ -1102,45 +1066,43 @@
     assert (
         200 == response.status_code
     ), f"Request could have failed with status {response.status_code}."
 
     return response
 
 
-def export_dataset_to_path(
-    out_file: str, fields: Optional[List[str]] = None
-) -> None:
+def export_dataset_to_path(out_file: str, fields: List[str] = None) -> None:
     """
     This function exports the original dataset via a buffered stream to the
     specified output file path. It takes ``fields`` as an optional argument for
     the header (column names), for the case where the callee expects to use
     specific columns; otherwise it uses the column names returned by the
     Watchful application. An exception is raised when the dataset's column names
     do not match the user's expected column names.
 
     :param out_file: The file path to export the original dataset to.
     :type out_file: str
     :param fields: The list of column names to use for the dataset export.
     :type fields: List, optional
     """
 
-    if fields is None:
+    if not fields:
         fields = get()["field_names"]
     n_cols = len(fields)
 
     with open(out_file, "w", encoding="utf-8") as f:
         writer = csv.writer(f)
         stream = export_stream().raw
         stream.auto_close = False
         reader = csv.reader(
             io.TextIOWrapper(stream, encoding="utf-8", newline="")
         )
         header = next(reader)
         if header[:n_cols] != fields:
-            raise ValueError(
+            raise Exception(
                 f"Dataset's column names {header} did not match the expected "
                 f"column names {fields}."
             )
         writer.writerow(fields)
         for row in reader:
             writer.writerow(row[:n_cols])
 
@@ -1201,19 +1163,18 @@
         200 == response.status_code
     ), f"Request could have failed with status {response.status_code}."
 
     return response
 
 
 def is_utf8(
-    csv_bytes: Optional[bytes] = None,
-    filepath: Optional[
-        Union[int, Union[str, bytes, os.PathLike[str], os.PathLike[bytes]]]
-    ] = None,
+    csv_bytes: bytes = None,
+    filepath: str = None,
     threshold: float = 0.5,
+    is_fast: bool = True,
 ) -> bool:
     """
     This function attempts to detect if the encoding of the given bytes or the
     content of the given filepath is utf-8. It returns `True` if the detected
     encoding is utf-8 and has a confidence of the given threshold or more,
     otherwise `False`. This function may need some tweaking for a very large
     dataset, but should work with the ``is_fast`` argument set to `True` by
@@ -1224,57 +1185,63 @@
     :param filepath: The path of the csv dataset file.
     :type filepath: str
     :param threshold: The minimum confidence required to accept the detected
         encoding.
     :type threshold: float, optional
     :param is_fast: Whether to use fast encoding detection with a lower
         accuracy, or not.
+    :type is_fast: bool, optional
     :return: `True` if the detected encoding is utf-8 and has a confidence of
         the given threshold or more, otherwise `False`.
     :rtype: bool
     """
-    if csv_bytes is not None and filepath is not None:
-        raise ValueError(
+    if csv_bytes is None and filepath is None:
+        raise Exception(
+            "Both filepath and csv_bytes are not specified. "
+            "One of them needs to be specified."
+        )
+    if csv_bytes and filepath:
+        raise Exception(
             "Both filepath and csv_bytes are specified. "
             "Only one of them needs to be specified."
         )
 
-    if csv_bytes is not None:
+    if is_fast:
+        import cchardet as chardet
+    else:
+        import chardet
+
+    if csv_bytes:
         res = chardet.detect(csv_bytes)
-    elif filepath is not None:
+    else:
         if os.path.isfile(filepath):
             with open(filepath, "rb") as f:
                 res = chardet.detect(f.read())
         else:
-            raise FileNotFoundError(
-                f"There is no file at the given file path {filepath!r}!"
+            raise Exception(
+                f"There is no file at the given file path {filepath}!"
             )
-    else:
-        raise ValueError(
-            "Both filepath and csv_bytes are not specified. "
-            "One of them needs to be specified."
-        )
 
     # Because cChardet likes to be specific with encoding,
     # ASCII will be specified if the valid UTF-8 characters
     # fit within that subset.
     valid_encodings = ["utf-8", "ascii"]
-    if res["encoding"] is not None:
-        enc = res["encoding"].lower()
-        return enc in valid_encodings and res["confidence"] >= threshold
-    raise ValueError("chardet charset detection did not return an encoding.")
+    enc = res["encoding"].lower()
+    if enc in valid_encodings and res["confidence"] >= threshold:
+        return True
+    return False
 
 
 def create_dataset(
     csv_bytes: bytes,
     columns: List[str],
     filename: str = "none",
     has_header: bool = True,
     threshold_detect: float = 0.5,
-    is_fast_detect: bool = True,  # pylint: disable=W0613
+    is_fast_detect: bool = True,
     force_load: bool = True,
 ) -> str:
     """
     This function loads the specified columns of a csv dataset and returns the
     dataset id if its encoding is detected to be utf-8 or if dataset loading is
     forced.
 
@@ -1286,29 +1253,32 @@
     :type filename: str, optional
     :param has_header: The boolean indicating if the csv dataset has a header,
         defaults to True.
     :type has_header: bool, optional
     :param threshold_detect: The minimum confidence required to accept the
         detected encoding.
     :type threshold_detect: float, optional
-    :param is_fast_detect: No longer used, but remains for API compatibility
+    :param is_fast_detect: Whether to use fast encoding detection with a lower
+        accuracy, or not.
     :type is_fast_detect: bool, optional
     :param force_load: The boolean indicating if the csv dataset will be loaded
         even when its encoding is detected to be non-utf-8, defaults to True.
         This is useful in rare cases where the csv dataset is detected to be
         non-utf-8 encoded and the user is sure about the csv dataset being utf-8
         encoded.
     :type force_load: bool, optional
     :return: The dataset id.
     :rtype: str
 
     TODO: Add error handling.
     """
 
-    is_csv_bytes_utf8 = is_utf8(csv_bytes, None, threshold_detect)
+    is_csv_bytes_utf8 = is_utf8(
+        csv_bytes, None, threshold_detect, is_fast_detect
+    )
 
     if is_csv_bytes_utf8 or force_load:
         id_ = str(uuid4())
         response = request(
             "POST",
             f"/api/_stream/{id_}/0/true",
             data=csv_bytes,
@@ -1327,15 +1297,15 @@
         )
         dataset_id = _read_response(response)["id"]
 
         api("dataset_add", id=dataset_id, columns=columns)
 
         return dataset_id
 
-    raise Warning(
+    raise Exception(
         "Dataset is not loaded as the encoding of the csv dataset is not "
         "detected to be utf-8 and dataset loading is not forced."
     )
 
 
 def label_single(row: List[str]) -> List[str]:
     """
@@ -1435,14 +1405,33 @@
         headers={"Content-Type": "text/plain"},
         timeout=API_TIMEOUT_SEC,
     )
 
     return _read_response(response)
 
 
+def print_candidates(summary: Optional[Dict] = None) -> None:
+    """
+    This function retrieves and prints the column names and all the candidates.
+
+    :param summary: The dictionary of the HTTP response from a connection
+        request, defaults to None.
+    :type summary: Dict, optional
+    """
+
+    if summary is None:
+        summary = get()
+    print(
+        "\n".join(
+            [",".join(summary["field_names"])]
+            + list(map(lambda c: ",".join(c["fields"]), summary["candidates"]))
+        )
+    )
+
+
 def candidate_dicts(summary: Optional[Dict] = None) -> List[Dict[str, str]]:
     """
     This function retrieves and returns all the candidates, together with the
     column names for all values.
 
     :param summary: The dictionary of the HTTP response from a connection
         request, defaults to None.
@@ -1450,25 +1439,17 @@
     :return: The list of all the candidates, each as a dictionary of named
         values.
     :rtype: List[Dict[str, str]]
     """
 
     if summary is None:
         summary = get()
-
-    def combine(c: Any):
-        if summary is None:
-            # This should never happen, but is here to convince mypy
-            # that it should never happen.
-            raise ValueError("Error reading the summary")
-        return dict(zip(summary["field_names"], c["fields"]))
-
     return list(
         map(
-            combine,
+            lambda c: dict(zip(summary["field_names"], c["fields"])),
             summary["candidates"],
         )
     )
 
 
 def exit_backend() -> None:
     """
@@ -1484,15 +1465,15 @@
     except requests.exceptions.ConnectionError:
         pass
 
 
 ## Hub API
 
 
-def hub_api(verb: str, token: str) -> Optional[Dict]:
+def hub_api(verb: str, token: str, **kwargs: Dict) -> Optional[Dict]:
     """
     This is a convenience function for collaboration API calls with Watchful;
     made up of a verb, a token and optional keyword arguments.
 
     :param verb: The verb for the hub API.
     :type verb: str
     :param verb: The user's auth token.
@@ -1501,18 +1482,20 @@
     :type kwargs: Dict
     :return: The dictionary of the HTTP response from the connection request.
     :rtype: Dict, optional
     """
 
     headers = {"Content-Type": "application/json"}
     headers.update({"Authorization": "Bearer " + token})
+    action = kwargs  # already a dictionary
+    action["verb"] = verb
     response = request(
         "POST",
         "/remote",
-        data=json.dumps({"verb": verb}),
+        data=json.dumps(action),
         headers=headers,
         timeout=API_TIMEOUT_SEC,
     )
     return _assert_success(_read_response(response))
 
 
 def login(email: str, password: str) -> Optional[Dict]:
@@ -1539,111 +1522,83 @@
         headers=headers,
         timeout=API_TIMEOUT_SEC,
     )
 
     return _assert_success(_read_response(response))
 
 
-def publish(token: str) -> Optional[Dict]:
+def publish(token: Optional[str] = None) -> Optional[Dict]:
     """
     This function performs publish with Watchful hub.
 
     :param token: The user's auth token, defaults to None.
     :type token: str, optional
     :return: The dictionary of the HTTP response from the connection request.
     :rtype: Dict, optional
     """
 
     return hub_api("publish", token)
 
 
-def fetch(token: str) -> Optional[Dict]:
+def fetch(token: Optional[str] = None) -> Optional[Dict]:
     """
     This function performs fetch with Watchful hub.
 
     :param token: The user's auth token, defaults to None.
     :type token: str, optional
     :return: The dictionary of the HTTP response from the connection request.
     :rtype: Dict, optional
     """
 
     return hub_api("fetch", token)
 
 
-def pull(token: str) -> Optional[Dict]:
+def pull(token: Optional[str] = None) -> Optional[Dict]:
     """
     This function performs pull with Watchful hub.
 
     :param token: The user's auth token, defaults to None.
     :type token: str, optional
     :return: The dictionary of the HTTP response from the connection request.
     :rtype: Dict, optional
     """
 
     return hub_api("pull", token)
 
 
-def push(token: str) -> Optional[Dict]:
+def push(token: Optional[str] = None) -> Optional[Dict]:
     """
     This function performs push with Watchful hub.
 
     :param token: The user's auth token, defaults to None.
     :type token: str, optional
     :return: The dictionary of the HTTP response from the connection request.
     :rtype: Dict, optional
     """
 
     return hub_api("push", token)
 
 
-def peek(token: str) -> Optional[Dict]:
+def peek(token: Optional[str] = None) -> Optional[Dict]:
     """
     This function performs peek with Watchful hub.
 
     :param token: The user's auth token, defaults to None.
     :type token: str, optional
     :return: The dictionary of the HTTP response from the connection request.
     :rtype: Dict, optional
     """
 
     return hub_api("peek", token)
 
 
-def whoami(token: str) -> Optional[Dict]:
+def whoami(token: Optional[str] = None) -> Optional[Dict]:
     """
     This function performs whoami with Watchful hub.
 
     :param token: The user's auth token, defaults to None.
     :type token: str, optional
     :return: The dictionary of the HTTP response from the connection request.
     :rtype: Dict, optional
     """
 
     return hub_api("whoami", token)
-
-
-class WatchfulAppInstanceError(Exception):
-    """
-    This class specifies the exception raised for errors relating to the
-    watchful app instance.
-    """
-
-    base_error_message = (
-        "This is a watchful app instance related error and could be resolved "
-        "by for example, creating a project, and/or opening a project, and/or "
-        "and/or adding a dataset to it."
-    )
-
-    def __init__(self, error_message=""):
-        """
-        This function concatenates the base error message with the specific
-        error message.
-
-        :param error_message: The specific error message, defaults to "".
-        :type error_message: str, optional
-        """
-        self.error_message = (
-            " ".join([error_message, self.base_error_message])
-            if error_message
-            else self.base_error_message
-        )
-        super().__init__(self.error_message)
```

### Comparing `watchful-3.3.7/src/watchful/enrich.py` & `watchful-3.5.0/src/watchful/enrich.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 
 import argparse
 import datetime
 import os
 import pathlib
 import shutil
 import sys
-from typing import Optional, List, Type, Sequence
+from typing import List, Type
 from watchful import client, attributes
 from watchful.enricher import Enricher
 
 
 def enrich_dataset(
     custom_enricher_cls: Type[Enricher],
-    args: Optional[List[str]] = None,
+    args: List[str] = None,
 ) -> None:
     """
     This is the function to use for performing custom data enrichment. Custom
     data enrichment variables, functions and mdoels can be defined in
     ``custom_enricher_cls`` and are used to perform the data enrichment.
 
     :param custom_enricher_cls: A custom enricher class that inherited
@@ -37,33 +37,30 @@
         args = []
     attributes.set_multiprocessing(False)
     custom_enricher = custom_enricher_cls()
 
     main(args, custom_enricher)
 
 
-def main(
-    overrides: Optional[Sequence[str]] = None,
-    custom_enricher: Optional[Enricher] = None,
-) -> None:
+def main(args: List[str] = None, custom_enricher: Enricher = None) -> None:
     """
     This is the utility function for performing data enrichment without a custom
     enricher; it is generally not called directly but invoked via the Python
     command line by the user. To perform data enrichment with a custom enricher,
     use :func:`enrich_dataset` instead.
 
     This function contains the logic and pipelining for the data enrichment.
 
     :param args: A list containing optional input arguments as defined in
         the ``parser`` arguments below.
     :type args: List[str]
     """
 
-    if overrides is None:
-        overrides = []
+    if args is None:
+        args = []
 
     parser = argparse.ArgumentParser(
         formatter_class=argparse.ArgumentDefaultsHelpFormatter
     )
 
     # The dataset file; use the dataset currently opened in Watchful if it is
     # not provided. This is not used in remote enrichment as we will retrieve
@@ -146,15 +143,15 @@
     parser.add_argument(
         "--is_local",
         action="store_true",
         help="Optional use of local Watchful local application instead of a \
             hosted application; hosted application if unspecified.",
     )
 
-    args = parser.parse_args(args=overrides)
+    args = parser.parse_args(args=args)
 
     attributes.set_multiprocessing(args.multiprocessing)
 
     client.external(host=args.host, port=args.port)
 
     summary = client.get()
     project_id = client.get_project_id(summary)
```

### Comparing `watchful-3.3.7/src/watchful/enricher.py` & `watchful-3.5.0/src/watchful/enricher.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 custom data enrichment functions and models within :meth:`enrich_fn`. Refer to
 https://github.com/Watchfulio/watchful-py/blob/main/examples/enrichment_intro.ipynb
 for a tutorial on how to implement your custom enricher class.
 """
 ################################################################################
 
 
-from abc import ABCMeta, abstractmethod, abstractproperty
-import typing
+from abc import ABCMeta, abstractmethod
 from typing import (
     Callable,
+    Generic,
     Dict,
     List,
     Literal,
     Optional,
     Tuple,
+    TypeVar,
     Union,
 )
 
 
 EnrichedCell = List[
     Tuple[
         Union[
@@ -30,15 +31,15 @@
         ]
     ]
 ]
 ENRICHMENT_ORDERS: List[str] = ["row", "col"]
 
 
 def set_enrich_fn_order(
-    enrich_fn: Optional[Callable] = None,
+    enrich_fn: Callable = None,
     order: Literal["row", "col"] = "row",
 ) -> Callable:
     """
     This function annotates a data enrichment function with an attribute that
     indicates the order of the data enrichment. Currently, the allowed orders
     are "row" and "col".
 
@@ -78,21 +79,15 @@
         In this method, we create variables that we will store in
         :attr:`self.enrichment_args`. We then later use them in
         :meth:`enrich_fn` to enrich our data row by row or column by column.
         This :meth:`__init__` method needs to be implemented in your enricher
         class.
         """
 
-    @abstractproperty
-    def enrichment_args(self) -> Tuple:
-        # XXX: rockstar (22 Apr 2023) - This Tuple has very
-        # defined requirements, as it will become part of the
-        # (not great) global scope in attributes.py as ENRICHMENT_ARGS.
-        # This will get addressed when attributes gets typed.
-        return (str, "")
+        pass
 
     @abstractmethod
     @set_enrich_fn_order(
         order="row",
     )  # `order` accepts either "row" or "col"; defaults to "row".
     def enrich_fn(
         self,
@@ -125,15 +120,15 @@
             cell, for the entire row or column.
         :rtype: List[EnrichedCell]
         """
 
         pass
 
     @classmethod
-    def is_enricher(cls, possibly_an_enricher: typing.Any) -> bool:
+    def is_enricher(cls, possibly_an_enricher: Generic[TypeVar("T")]) -> bool:
         """
         This is a convenience method used for checking if
         :class:`possibly_an_enricher` is indeed of the :class:`Enricher` class.
 
         :param possibly_an_enricher: A class that is possibly of the
             :class:`Enricher` class.
         :type possibly_an_enricher: Class
@@ -141,15 +136,17 @@
             indeed of the :class:`Enricher` class.
         :rtype: bool
         """
 
         return issubclass(possibly_an_enricher, cls)
 
     @classmethod
-    def is_fully_formed_enricher(cls, possibly_an_enricher: typing.Any) -> bool:
+    def is_fully_formed_enricher(
+        cls, possibly_an_enricher: Generic[TypeVar("T")]
+    ) -> bool:
         """
         This is a convenience method used for checking if
         :class:`possibly_an_enricher` has defined its enrichment order that
         can be one of :attr:`ENRICHMENT_ORDERS`.
 
         :param possibly_an_enricher: A class that is possibly of the
             :class:`Enricher` class.
```

### Comparing `watchful-3.3.7/LICENSE` & `watchful-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `watchful-3.3.7/README.md` & `watchful-3.5.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -7,28 +7,37 @@
 - Watchful API and [notebook](https://github.com/Watchfulio/watchful-py/blob/main/examples/api_intro.ipynb)
 
 - [Data Enrichment](https://github.com/Watchfulio/watchful-py/blob/main/examples/README.md) and [notebook](https://github.com/Watchfulio/watchful-py/blob/main/examples/enrichment_intro.ipynb)
 
 
 ## Steps (Use)
 
+### Create Python Enviroment
+- Refer [here](https://github.com/Watchfulio/watchful-py/blob/main/README_PY_ENV.md) for options.
+
 ### Install Watchful Python SDK from PyPI (Recommended)
 
 If you want to use Python to communicate with the Watchful API, you'll need to install the Watchful Python SDK from PyPI.
 
 - Install your desired release version (they can be found at [PyPI](https://pypi.org/project/watchful/))
 
 ```command
 pip3 install watchful[==your.desired.version]
 ```
 
 ### Basic Usage
 
 Once you have installed the SDK, import it and begin interacting with it.
 
+```python
+import watchful as w
+w.__version__    # This prints the SDK version, for example "2.3.0".
+```
+
+> **Note**:
 > For a more thorough Watchful API introduction, read through our [API Introduction Jupyter Notebook](https://github.com/Watchfulio/watchful-py/blob/main/examples/api_intro.ipynb).
 
 ### Basic Enrichment
 
 The Watchful SDK aims to make enrichment a straight-forward task. The following steps assume a brand new user without any projects.
 
 - Ensure you have the proper Python version and environment setup. Follow the [environment setup guide](https://github.com/Watchfulio/watchful-py/blob/main/README_PY_ENV.md) for more details.
@@ -45,14 +54,31 @@
   - `python3 -m watchful.enrich --host localhost --port 9001`&nbsp;&nbsp;&nbsp;&nbsp;`# Enter your actual host and port.`
 
 > **Note: Enrich via Jupyter Notebook**
 > \- A more comprehensive guide to enrichment is available in the [Enrichment Introduction Jupyter Notebook](https://github.com/Watchfulio/watchful-py/blob/main/examples/enrichment_intro.ipynb).
 
 For more guides and documentation, see the [ReadMe](https://github.com/Watchfulio/watchful-py/blob/main/examples/README.md) in the `examples` directory.
 
+## Steps (Development)
+
+### Create Python Enviroment
+- Refer [here](https://github.com/Watchfulio/watchful-py/blob/main/README_PY_ENV.md) for options.
+
+### Upgrade Tools
+- Upgrade or install `pip`, build and test tools
+```command
+pip3 install pip==22.2.2
+```
+```command
+pip3 install build==0.8.0
+```
+```command
+pip3 install pylint==2.13.9 pylama==8.3.8 black==22.3.0 pytest==7.1.1 nbval==0.9.6
+```
+
 ### Code Practices
 If contributing to this code, you're encouraged to apply the following code practices.
 - Apply linting and formatting
 ```command
 cd to/the/repo_directory/that/being/watchful-py
 ```
 ```command
@@ -61,15 +87,15 @@
 ```command
 black src/watchful/ --config=pyproject.toml --diff
 ```
 
 ### Build & Install Watchful Package Locally
 - Build the package
 ```command
-hatch build
+python3 -m build .
 ```
 - Install the built package (add `--force-reinstall` to guarantee a full (re)installation)
 ```command
 pip3 install dist/watchful-<latest.release.version>-py3-none-any.whl [--force-reinstall]
 ```
 `<latest.release.version>` can be found [here](./src/watchful/VERSION).
 - Show the installed watchful package
```

