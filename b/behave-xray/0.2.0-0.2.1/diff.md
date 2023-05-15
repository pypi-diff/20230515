# Comparing `tmp/behave_xray-0.2.0-py3-none-any.whl.zip` & `tmp/behave_xray-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,16 @@
-Zip file size: 15613 bytes, number of entries: 15
--rw-r--r--  2.0 unx      129 b- defN 23-Apr-25 14:09 behave_xray/__init__.py
--rw-r--r--  2.0 unx     1765 b- defN 23-Apr-04 19:53 behave_xray/authentication.py
+Zip file size: 15359 bytes, number of entries: 14
+-rw-r--r--  2.0 unx      129 b- defN 23-May-14 18:58 behave_xray/__init__.py
+-rw-r--r--  2.0 unx     1765 b- defN 23-May-14 18:58 behave_xray/authentication.py
 -rw-r--r--  2.0 unx     1625 b- defN 23-Apr-25 16:01 behave_xray/evidence.py
 -rw-r--r--  2.0 unx      137 b- defN 22-Oct-09 13:17 behave_xray/exceptions.py
--rw-r--r--  2.0 unx    10199 b- defN 23-Apr-25 14:09 behave_xray/formatter.py
+-rw-r--r--  2.0 unx    10381 b- defN 23-May-15 16:59 behave_xray/formatter.py
 -rw-r--r--  2.0 unx     1866 b- defN 23-Apr-25 14:09 behave_xray/helper.py
--rw-r--r--  2.0 unx      239 b- defN 23-Mar-19 17:44 behave_xray/hookimpl.py
--rw-r--r--  2.0 unx      239 b- defN 23-Apr-25 14:09 behave_xray/hookspecs.py
--rw-r--r--  2.0 unx     4458 b- defN 23-Apr-25 14:09 behave_xray/model.py
--rw-r--r--  2.0 unx     2798 b- defN 23-Apr-25 14:09 behave_xray/xray_publisher.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Apr-25 16:02 behave_xray-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     4698 b- defN 23-Apr-25 16:02 behave_xray-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-25 16:02 behave_xray-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Apr-25 16:02 behave_xray-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1215 b- defN 23-Apr-25 16:02 behave_xray-0.2.0.dist-info/RECORD
-15 files, 40829 bytes uncompressed, 13611 bytes compressed:  66.7%
+-rw-r--r--  2.0 unx      239 b- defN 23-May-14 18:58 behave_xray/hookspecs.py
+-rw-r--r--  2.0 unx     4458 b- defN 23-May-14 18:58 behave_xray/model.py
+-rw-r--r--  2.0 unx     2798 b- defN 23-May-14 18:58 behave_xray/xray_publisher.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-15 17:01 behave_xray-0.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4698 b- defN 23-May-15 17:01 behave_xray-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-15 17:01 behave_xray-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-15 17:01 behave_xray-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1136 b- defN 23-May-15 17:01 behave_xray-0.2.1.dist-info/RECORD
+14 files, 40693 bytes uncompressed, 13479 bytes compressed:  66.9%
```

## zipnote {}

```diff
@@ -12,35 +12,32 @@
 
 Filename: behave_xray/formatter.py
 Comment: 
 
 Filename: behave_xray/helper.py
 Comment: 
 
-Filename: behave_xray/hookimpl.py
-Comment: 
-
 Filename: behave_xray/hookspecs.py
 Comment: 
 
 Filename: behave_xray/model.py
 Comment: 
 
 Filename: behave_xray/xray_publisher.py
 Comment: 
 
-Filename: behave_xray-0.2.0.dist-info/LICENSE
+Filename: behave_xray-0.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: behave_xray-0.2.0.dist-info/METADATA
+Filename: behave_xray-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: behave_xray-0.2.0.dist-info/WHEEL
+Filename: behave_xray-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: behave_xray-0.2.0.dist-info/top_level.txt
+Filename: behave_xray-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: behave_xray-0.2.0.dist-info/RECORD
+Filename: behave_xray-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## behave_xray/formatter.py

```diff
@@ -1,19 +1,20 @@
+import importlib
+import json
+import sys
 from collections import defaultdict
 from dataclasses import dataclass, field
 from enum import Enum, auto
-import importlib
 from os import environ, getenv
 from typing import AnyStr, Dict, List, Optional, Tuple, Union
 
 import pluggy
 from behave.formatter.base import Formatter
 from behave.model import Feature as BehaveFeature
 from behave.model import Scenario as BehaveScenario
-from behave.model import ScenarioOutline as BehaveScenarioOutline
 from behave.model import Status
 
 from behave_xray import hookspecs
 from behave_xray.authentication import AuthBase, BearerAuth, PersonalAccessTokenAuth
 from behave_xray.exceptions import XrayError
 from behave_xray.helper import (
     get_overall_status,
@@ -75,14 +76,15 @@
     name = 'xray'
     description = 'Jira XRAY formatter'
 
     STATUS_MAPS: Dict[str, str] = {}
 
     def __init__(self, stream, config, publisher: XrayPublisher):
         super().__init__(stream, config)
+        self.stream = self.open()
         self.pm = self._get_plugin_manager()
         self._register_user_hook()
         self.xray_publisher = publisher
         self.current_feature: Optional[BehaveFeature] = None
         self.current_scenario: Optional[BehaveScenario] = None
         self.current_test_key: Optional[str] = None
         self.test_execution: TestExecution = TestExecution(
@@ -116,15 +118,15 @@
                 base_url=jira_config.jira_url,
                 client_id=jira_config.client_id,
                 client_secret=jira_config.client_secret
             )
         elif jira_config.auth_method == AuthType.token:
             return PersonalAccessTokenAuth(token=jira_config.token)
         else:  # basic
-            return (jira_config.user_name, jira_config.user_password)
+            return jira_config.user_name, jira_config.user_password
 
     def _get_summary(self) -> str:
         return self.config.userdata.get('xray.summary', '')
 
     def _get_user(self) -> str:
         return self.config.userdata.get('xray.user', '')
 
@@ -152,15 +154,15 @@
             if test_exec_key:
                 self.test_execution.test_execution_key = test_exec_key
             test_plan_key = get_test_plan_key_from_tag(tag)
             if test_plan_key:
                 self.test_execution.test_plan_key = test_plan_key
 
     def is_scenario_outline(self):
-        return isinstance(self.current_scenario, BehaveScenarioOutline)
+        return True if 'Scenario Outline' in self.current_scenario.keyword else False
 
     def scenario(self, scenario):
         self.current_scenario = scenario
         self.current_test_key = None
         if not scenario.tags:
             return
 
@@ -176,22 +178,22 @@
         except KeyError:
             return 'TODO'
 
     def get_verdict(self, step) -> Verdict:
         verdict = Verdict(self.current_scenario.status, '')
         if step.status == Status.failed:
             verdict.message = step.error_message
-        if step.status == Status.untested:
+        elif step.status == Status.untested:
             verdict.message = 'Untested'
-        if step.status == Status.skipped:
+        elif step.status == Status.skipped:
             verdict.message = self.current_scenario.skip_reason
         return verdict
 
     @property
-    def current_test_case(self) -> ScenarioResult:
+    def current_test_case(self) -> Optional[ScenarioResult]:
         try:
             return self.testcases[self.current_test_key]
         except KeyError:
             return None
 
     def result(self, step):
         if self.current_scenario.status == Status.untested:
@@ -217,14 +219,17 @@
         # run when current feature is done
         if self.config.dry_run:
             return
 
         self.collect_tests()
         if self.test_execution.tests:
             self.xray_publisher.publish(self.test_execution.as_dict())
+            if self.stream != sys.stdout:
+                self.stream.write(json.dumps(self.test_execution.as_dict(), indent=4))
+                self.stream.flush()
         self.test_execution.flush()
         self.reset()
 
     def collect_tests(self) -> None:
         """Update test execution with test cases."""
         for tc_id, tc_status in self.testcases.items():
             testcase = self._get_test_case(test_key=tc_id)
```

## Comparing `behave_xray-0.2.0.dist-info/LICENSE` & `behave_xray-0.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `behave_xray-0.2.0.dist-info/METADATA` & `behave_xray-0.2.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: behave-xray
-Version: 0.2.0
+Version: 0.2.1
 Summary: Behave JIRA XRAY results uploader
 Home-page: https://github.com/fundakol/behave-xray
 Author: Lukasz Fundakowski
 Author-email: fundakol@yahoo.com
 Keywords: behave JIRA XRAY
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

## Comparing `behave_xray-0.2.0.dist-info/RECORD` & `behave_xray-0.2.1.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 behave_xray/__init__.py,sha256=fH09Qs25fPbpmzvbit-j6zx0RRgPf7rnaSNCyKpzv08,129
 behave_xray/authentication.py,sha256=gC8YDPe2kgKy7s3IpG6WH_ayKAQHf2uR0AyImIvuF4k,1765
 behave_xray/evidence.py,sha256=leBrNulch6jOo-KC7j2TAhUnM3LIQw-1mTemZIDDVOA,1625
 behave_xray/exceptions.py,sha256=IS-_20kUX3rUTdg_22x5itn2rq-JgpXXO1r5BMq42Xo,137
-behave_xray/formatter.py,sha256=n3o42OivmeMhvwShsoeD6VE3FXNrgIhP4wxCAMgSEhc,10199
+behave_xray/formatter.py,sha256=4dkVn39lyrnyl5bOE1gzqu3PLjU3vqLxRfFc5tb9fQY,10381
 behave_xray/helper.py,sha256=HP5pNQL-Ya444FCctX7AVw4JLrXMHTrHurTw6XsQHOU,1866
-behave_xray/hookimpl.py,sha256=2IkfiSVg6uetFS6YWw8Uia7texma5sIkK0h5nlla_ms,239
 behave_xray/hookspecs.py,sha256=LcznKPkPTvyvb2yG3Bte3nRtXAo_krrAVV36Gr61gL8,239
 behave_xray/model.py,sha256=IXcAhABj-UAdWawrLjkQ5weYG7BrKBfPZkT8TKClHWg,4458
 behave_xray/xray_publisher.py,sha256=0GI1mF5KBlQzxb2FzJd-Pzf3E__PV2t2uLgSRBglqio,2798
-behave_xray-0.2.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-behave_xray-0.2.0.dist-info/METADATA,sha256=FtF6dNgrZD2FDF9fvnbueL4K6KNL23a3x1RrTWEEqX0,4698
-behave_xray-0.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-behave_xray-0.2.0.dist-info/top_level.txt,sha256=OYIfJ2lUkKf_kjicCEoXpvVm3yp17ORgb_M-rPkX5Jg,12
-behave_xray-0.2.0.dist-info/RECORD,,
+behave_xray-0.2.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+behave_xray-0.2.1.dist-info/METADATA,sha256=-B8yXEqYdpO_7VzZoyLsQVTEgMxH_s5lE_7yrYvxqVU,4698
+behave_xray-0.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+behave_xray-0.2.1.dist-info/top_level.txt,sha256=OYIfJ2lUkKf_kjicCEoXpvVm3yp17ORgb_M-rPkX5Jg,12
+behave_xray-0.2.1.dist-info/RECORD,,
```

