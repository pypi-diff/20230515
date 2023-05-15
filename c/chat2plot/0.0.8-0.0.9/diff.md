# Comparing `tmp/chat2plot-0.0.8.tar.gz` & `tmp/chat2plot-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat2plot-0.0.8.tar", last modified: Sat May 13 17:29:07 2023, max compression
+gzip compressed data, was "chat2plot-0.0.9.tar", last modified: Mon May 15 14:17:59 2023, max compression
```

## Comparing `chat2plot-0.0.8.tar` & `chat2plot-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:29:07.494147 chat2plot-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-13 17:28:55.000000 chat2plot-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-13 17:28:55.000000 chat2plot-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-13 17:29:07.494147 chat2plot-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-13 17:28:55.000000 chat2plot-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:29:07.494147 chat2plot-0.0.8/chat2plot/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-13 17:28:55.000000 chat2plot-0.0.8/chat2plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-05-13 17:28:55.000000 chat2plot-0.0.8/chat2plot/chat2plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-13 17:28:55.000000 chat2plot-0.0.8/chat2plot/dataset_description.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-13 17:28:55.000000 chat2plot-0.0.8/chat2plot/dictionary_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-13 17:28:55.000000 chat2plot-0.0.8/chat2plot/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-05-13 17:28:55.000000 chat2plot-0.0.8/chat2plot/render.py
--rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-05-13 17:28:55.000000 chat2plot-0.0.8/chat2plot/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-13 17:28:55.000000 chat2plot-0.0.8/chat2plot/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-13 17:28:55.000000 chat2plot-0.0.8/chat2plot/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:29:07.494147 chat2plot-0.0.8/chat2plot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-13 17:29:07.000000 chat2plot-0.0.8/chat2plot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-13 17:29:07.000000 chat2plot-0.0.8/chat2plot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 17:29:07.000000 chat2plot-0.0.8/chat2plot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-13 17:29:07.000000 chat2plot-0.0.8/chat2plot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-13 17:29:07.000000 chat2plot-0.0.8/chat2plot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-13 17:28:55.000000 chat2plot-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-13 17:28:55.000000 chat2plot-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-13 17:29:07.494147 chat2plot-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-13 17:28:55.000000 chat2plot-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:29:07.494147 chat2plot-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 17:28:55.000000 chat2plot-0.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-13 17:28:55.000000 chat2plot-0.0.8/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:17:59.095680 chat2plot-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-15 14:17:47.000000 chat2plot-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 14:17:47.000000 chat2plot-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-05-15 14:17:59.095680 chat2plot-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-05-15 14:17:47.000000 chat2plot-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:17:59.095680 chat2plot-0.0.9/chat2plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-15 14:17:47.000000 chat2plot-0.0.9/chat2plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-05-15 14:17:47.000000 chat2plot-0.0.9/chat2plot/chat2plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-15 14:17:47.000000 chat2plot-0.0.9/chat2plot/dataset_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-15 14:17:47.000000 chat2plot-0.0.9/chat2plot/dictionary_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-15 14:17:47.000000 chat2plot-0.0.9/chat2plot/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-05-15 14:17:47.000000 chat2plot-0.0.9/chat2plot/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-05-15 14:17:47.000000 chat2plot-0.0.9/chat2plot/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-15 14:17:47.000000 chat2plot-0.0.9/chat2plot/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 14:17:47.000000 chat2plot-0.0.9/chat2plot/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:17:59.095680 chat2plot-0.0.9/chat2plot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-05-15 14:17:59.000000 chat2plot-0.0.9/chat2plot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-15 14:17:59.000000 chat2plot-0.0.9/chat2plot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 14:17:59.000000 chat2plot-0.0.9/chat2plot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-15 14:17:59.000000 chat2plot-0.0.9/chat2plot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 14:17:59.000000 chat2plot-0.0.9/chat2plot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-15 14:17:47.000000 chat2plot-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-15 14:17:47.000000 chat2plot-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-15 14:17:59.095680 chat2plot-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-15 14:17:47.000000 chat2plot-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:17:59.095680 chat2plot-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 14:17:47.000000 chat2plot-0.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-15 14:17:47.000000 chat2plot-0.0.9/tests/test_schema.py
```

### Comparing `chat2plot-0.0.8/LICENSE` & `chat2plot-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `chat2plot-0.0.8/chat2plot/chat2plot.py` & `chat2plot-0.0.9/chat2plot/chat2plot.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,27 +5,38 @@
 from logging import getLogger
 from typing import Any
 
 import altair as alt
 import commentjson
 import jsonschema
 import pandas as pd
+import pydantic
 from langchain.chat_models import ChatOpenAI
 from langchain.chat_models.base import BaseChatModel
 from langchain.schema import BaseMessage, HumanMessage, SystemMessage
 from plotly.graph_objs import Figure
 
 from chat2plot.dataset_description import description
 from chat2plot.dictionary_helper import delete_null_field
-from chat2plot.prompt import error_correction_prompt, system_prompt
+from chat2plot.prompt import JSON_TAG, error_correction_prompt, system_prompt
 from chat2plot.render import draw_altair, draw_plotly
 from chat2plot.schema import PlotConfig, ResponseType
 
 _logger = getLogger(__name__)
 
+# These errors are caught within the application.
+# Other errors (e.g. openai.error.RateLimitError) are propagated to user code.
+_APPLICATION_ERRORS = (
+    pydantic.ValidationError,
+    jsonschema.ValidationError,
+    ValueError,
+    KeyError,
+    AssertionError,
+)
+
 
 @dataclass(frozen=True)
 class Plot:
     figure: alt.Chart | Figure | None
     config: PlotConfig | dict[str, Any] | None
     response_type: ResponseType
     explanation: str
@@ -103,31 +114,32 @@
     def session(self) -> ChatSession:
         return self._session
 
     def query(self, q: str, config_only: bool = False, show_plot: bool = False) -> Plot:
         raw_response = self._session.query(q)
 
         try:
-            return self._parse_response(raw_response, config_only, show_plot)
-        except Exception as e:
             if self._verbose:
+                _logger.info(f"request: {q}")
                 _logger.info(f"first response: {raw_response}")
+            return self._parse_response(raw_response, config_only, show_plot)
+        except _APPLICATION_ERRORS as e:
+            if self._verbose:
                 _logger.warning(traceback.format_exc())
-
             msg = e.message if isinstance(e, jsonschema.ValidationError) else str(e)
             error_correction = error_correction_prompt().format(
                 error_message=msg,
             )
             corrected_response = self._session.query(error_correction)
             if self._verbose:
                 _logger.info(f"retry response: {corrected_response}")
 
             try:
                 return self._parse_response(corrected_response, config_only, show_plot)
-            except Exception as e:
+            except _APPLICATION_ERRORS as e:
                 if self._verbose:
                     _logger.warning(e)
                     _logger.warning(traceback.format_exc())
                 return Plot(
                     None,
                     None,
                     ResponseType.FAILED_TO_RENDER,
@@ -136,40 +148,35 @@
                 )
 
     def __call__(
         self, q: str, config_only: bool = False, show_plot: bool = False
     ) -> Plot:
         return self.query(q, config_only, show_plot)
 
-    def render(
-        self, df: pd.DataFrame, config: PlotConfig, show_plot: bool = True
-    ) -> Any:
-        return draw_plotly(df, config, show_plot)
-
     def _parse_response(self, content: str, config_only: bool, show_plot: bool) -> Plot:
         explanation, json_data = parse_json(content)
 
         try:
             config = PlotConfig.from_json(json_data)
-        except Exception:
+        except _APPLICATION_ERRORS:
             _logger.warning(traceback.format_exc())
             # To reduce the number of failure cases as much as possible,
             # only check against the json schema when instantiation fails.
             jsonschema.validate(json_data, PlotConfig.schema())
             raise
 
         if self._verbose:
             _logger.info(config)
 
         if config_only:
             return Plot(
                 None, config, ResponseType.SUCCESS, explanation, self._session.history
             )
 
-        figure = self.render(self._df, config, show_plot)
+        figure = draw_plotly(self._df, config, show_plot)
         return Plot(
             figure, config, ResponseType.SUCCESS, explanation, self._session.history
         )
 
 
 class Chat2Vega(Chat2PlotBase):
     def __init__(
@@ -188,30 +195,30 @@
 
         try:
             explanation, config = parse_json(res)
             if "data" in config:
                 del config["data"]
             if self._verbose:
                 _logger.info(config)
-        except Exception:
+        except _APPLICATION_ERRORS:
             _logger.warning(f"failed to parse LLM response: {res}")
             _logger.warning(traceback.format_exc())
             return Plot(None, None, ResponseType.UNKNOWN, res, self._session.history)
 
         if config_only:
             return Plot(
                 None, config, ResponseType.SUCCESS, explanation, self._session.history
             )
 
         try:
             plot = draw_altair(self._df, config, show_plot)
             return Plot(
                 plot, config, ResponseType.SUCCESS, explanation, self._session.history
             )
-        except Exception:
+        except _APPLICATION_ERRORS:
             _logger.warning(traceback.format_exc())
             return Plot(
                 None,
                 config,
                 ResponseType.FAILED_TO_RENDER,
                 explanation,
                 self._session.history,
@@ -225,14 +232,27 @@
 
 def chat2plot(
     df: pd.DataFrame,
     model_type: str = "simple",
     chat: BaseChatModel | None = None,
     verbose: bool = False,
 ) -> Chat2PlotBase:
+    """Create Chat2Plot instance.
+
+    Args:
+        df: Data source for visualization.
+        model_type: Type of json format. "vega" for a vega-lite compliant format, or "simple" or a simpler format.
+        chat: The chat instance for interaction with LLMs.
+              If omitted, `ChatOpenAI(temperature=0, model_name="gpt-3.5-turbo")` will be used.
+        verbose: If `True`, chat2plot will output logs.
+
+    Returns:
+        Chat instance.
+    """
+
     if model_type == "simple":
         return Chat2Plot(df, chat, verbose)
     elif model_type == "vega":
         return Chat2Vega(df, chat, verbose)
     else:
         raise ValueError(
             f"model_type should be one of [default, vega] (given: {model_type})"
@@ -247,17 +267,18 @@
         m = re.search(rf"<{tag}>(.*)<{tag}>", s, re.MULTILINE | re.DOTALL)
         if m:
             return m.group(1)
     return ""
 
 
 def parse_json(content: str) -> tuple[str, dict[str, Any]]:
+    """parse json and split contents by pre-defined tags"""
     json_part = _extract_tag_content(content, "json")  # type: ignore
     if not json_part:
-        raise ValueError("failed to find <json> and </json> tags")
+        raise ValueError(f"failed to find {JSON_TAG[0]} and {JSON_TAG[1]} tags")
 
     explanation_part = _extract_tag_content(content, "explain")
     if not explanation_part:
         explanation_part = _extract_tag_content(content, "explanation")
 
     # LLM rarely generates JSON with comments, so use the commentjson package instead of json
     return explanation_part.strip(), delete_null_field(commentjson.loads(json_part))
```

### Comparing `chat2plot-0.0.8/chat2plot/dictionary_helper.py` & `chat2plot-0.0.9/chat2plot/dictionary_helper.py`

 * *Files identical despite different names*

### Comparing `chat2plot-0.0.8/chat2plot/prompt.py` & `chat2plot-0.0.9/chat2plot/prompt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import json
 from textwrap import dedent
 
 from chat2plot.schema import get_schema_of_chart_config
 
+JSON_TAG = ["<json>", "</json>"]
+EXPLANATION_TAG = ["<explain>", "</explain>"]
+
 
 def system_prompt(model_type: str = "simple") -> str:
     return (
         _task_definition_part(model_type) + "\n" + _data_and_detailed_instruction_part()
     )
 
 
 def error_correction_prompt() -> str:
     return dedent(
         """
         Your response fails with the following error:
         {error_message}
-        
+
         Correct the json and return a new explanation and json that fixes the above mentioned error.
         Do not generate the same json again.
     """
     )
 
 
 def _task_definition_part(model_type: str) -> str:
@@ -39,31 +42,35 @@
             + schema_json.replace("{", "{{").replace("}", "}}")
         )
 
     else:
         return dedent(
             """
             Your task is to generate chart configuration for the given dataset and user question delimited by <>.
-            Responses should be in JSON format compliant with the vega-lite specification, but `data` field must be excluded.
+            Responses should be in JSON format compliant with the vega-lite specification,
+            but `data` field must be excluded.
             """
         )
 
 
 def _data_and_detailed_instruction_part() -> str:
     return dedent(
-        """
-        Note that the user may want to refine the chart by asking a follow-up question to a previous request, or may want to create a new chart in a completely new context.
+        f"""
+        Note that the user may want to refine the chart by asking a follow-up question to a previous request,
+        or may want to create a new chart in a completely new context.
         In the latter case, be careful not to use the context used for the previous chart.
-        
+
         This is the result of `print(df.head())`:
-        
-        {dataset}
-        
+
+        {{dataset}}
+
         You should do the following step by step, and your response should include both 1 and 2:
-        1. Explain whether filters should be applied to the data, which chart_type and columns should be used, and what transformations are necessary to fulfill the user's request.
-           Answers should be in the same language as the user and be understandable to someone who does not know the JSON schema definition.
-           This text should be enclosed with <explain> and </explain> tag.
+        1. Explain whether filters should be applied to the data, which chart_type and columns should be used,
+           and what transformations are necessary to fulfill the user's request.
+           Answers should be in the same language as the user and be understandable to someone who does not know
+           the JSON schema definition.
+           This text should be enclosed with {EXPLANATION_TAG[0]} and {EXPLANATION_TAG[1]} tag.
         2. Generate schema-compliant JSON that represents 1.
-           This text should be enclosed with <json> and </json> tag.
+           This text should be enclosed with {JSON_TAG[0]} and {JSON_TAG[1]} tag.
 
         """
     )
```

### Comparing `chat2plot-0.0.8/chat2plot/render.py` & `chat2plot-0.0.9/chat2plot/render.py`

 * *Files identical despite different names*

### Comparing `chat2plot-0.0.8/chat2plot/schema.py` & `chat2plot-0.0.9/chat2plot/schema.py`

 * *Files identical despite different names*

### Comparing `chat2plot-0.0.8/chat2plot/transform.py` & `chat2plot-0.0.9/chat2plot/transform.py`

 * *Files identical despite different names*

### Comparing `chat2plot-0.0.8/setup.cfg` & `chat2plot-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `chat2plot-0.0.8/setup.py` & `chat2plot-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `chat2plot-0.0.8/tests/test_schema.py` & `chat2plot-0.0.9/tests/test_schema.py`

 * *Files identical despite different names*

