# Comparing `tmp/iam_ape-1.1.1.tar.gz` & `tmp/iam_ape-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_ape-1.1.1.tar", max compression
+gzip compressed data, was "iam_ape-1.1.2.tar", max compression
```

## Comparing `iam_ape-1.1.1.tar` & `iam_ape-1.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35149 2023-04-27 15:26:26.770889 iam_ape-1.1.1/LICENSE
--rw-r--r--   0        0        0     3031 2023-04-27 15:26:26.771008 iam_ape-1.1.1/README.md
--rw-r--r--   0        0        0        0 2023-04-27 15:26:26.771631 iam_ape-1.1.1/iam_ape/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 15:26:26.771725 iam_ape-1.1.1/iam_ape/aws_iam_actions/__init__.py
--rw-r--r--   0        0        0   260932 2023-05-10 17:36:52.355616 iam_ape-1.1.1/iam_ape/aws_iam_actions/aws_iam_actions.tar.gz
--rw-r--r--   0        0        0     2773 2023-04-27 15:26:26.772225 iam_ape-1.1.1/iam_ape/aws_iam_actions/scrape_iam_actions.py
--rw-r--r--   0        0        0     1748 2023-05-10 17:34:00.350992 iam_ape-1.1.1/iam_ape/consts.py
--rw-r--r--   0        0        0    31885 2023-04-27 15:26:26.772497 iam_ape-1.1.1/iam_ape/evaluator.py
--rw-r--r--   0        0        0    15478 2023-05-10 17:34:00.351179 iam_ape-1.1.1/iam_ape/expand_policy.py
--rw-r--r--   0        0        0     3422 2023-05-10 17:34:00.351308 iam_ape-1.1.1/iam_ape/helper_classes.py
--rw-r--r--   0        0        0     7858 2023-05-10 17:34:00.351446 iam_ape-1.1.1/iam_ape/helper_functions.py
--rw-r--r--   0        0        0     1224 2023-04-27 15:26:26.773011 iam_ape-1.1.1/iam_ape/helper_types.py
--rw-r--r--   0        0        0     9999 2023-05-10 17:34:00.351593 iam_ape-1.1.1/iam_ape/main.py
--rw-r--r--   0        0        0        0 2023-04-27 15:26:26.773181 iam_ape-1.1.1/iam_ape/py.typed
--rw-r--r--   0        0        0     1257 2023-05-10 17:37:12.129154 iam_ape-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     4279 1970-01-01 00:00:00.000000 iam_ape-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-27 15:26:26.770889 iam_ape-1.1.2/LICENSE
+-rw-r--r--   0        0        0     3031 2023-04-27 15:26:26.771008 iam_ape-1.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 15:26:26.771631 iam_ape-1.1.2/iam_ape/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 15:26:26.771725 iam_ape-1.1.2/iam_ape/aws_iam_actions/__init__.py
+-rw-r--r--   0        0        0   261088 2023-05-15 10:16:11.384423 iam_ape-1.1.2/iam_ape/aws_iam_actions/aws_iam_actions.tar.gz
+-rw-r--r--   0        0        0     2854 2023-05-15 10:16:11.386023 iam_ape-1.1.2/iam_ape/aws_iam_actions/scrape_iam_actions.py
+-rw-r--r--   0        0        0     1748 2023-05-10 17:34:00.350992 iam_ape-1.1.2/iam_ape/consts.py
+-rw-r--r--   0        0        0    32182 2023-05-15 10:16:11.386282 iam_ape-1.1.2/iam_ape/evaluator.py
+-rw-r--r--   0        0        0    15833 2023-05-15 10:16:11.386516 iam_ape-1.1.2/iam_ape/expand_policy.py
+-rw-r--r--   0        0        0     3422 2023-05-10 17:34:00.351308 iam_ape-1.1.2/iam_ape/helper_classes.py
+-rw-r--r--   0        0        0     7858 2023-05-10 17:34:00.351446 iam_ape-1.1.2/iam_ape/helper_functions.py
+-rw-r--r--   0        0        0     1224 2023-04-27 15:26:26.773011 iam_ape-1.1.2/iam_ape/helper_types.py
+-rw-r--r--   0        0        0     9999 2023-05-10 17:34:00.351593 iam_ape-1.1.2/iam_ape/main.py
+-rw-r--r--   0        0        0        0 2023-04-27 15:26:26.773181 iam_ape-1.1.2/iam_ape/py.typed
+-rw-r--r--   0        0        0     1257 2023-05-15 10:16:11.387011 iam_ape-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4279 1970-01-01 00:00:00.000000 iam_ape-1.1.2/PKG-INFO
```

### Comparing `iam_ape-1.1.1/LICENSE` & `iam_ape-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_ape-1.1.1/README.md` & `iam_ape-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `iam_ape-1.1.1/iam_ape/aws_iam_actions/scrape_iam_actions.py` & `iam_ape-1.1.2/iam_ape/aws_iam_actions/scrape_iam_actions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import logging
+import os
 import tarfile
 import tempfile
 from collections import defaultdict
 from typing import Any, Dict
 
 import requests
 import tqdm  # type: ignore
@@ -67,19 +68,20 @@
 
         except AttributeError as e:
             logger.error(f"Error occurred while processing {link} - {e}")
             raise e
 
     logger.info("Done!")
 
-    with tempfile.NamedTemporaryFile("w+") as f:
+    tmpf = os.path.join(tempfile.gettempdir(), os.urandom(24).hex())
+    with open(tmpf, "w+") as f:
         json.dump(data, f, indent=2)
         f.flush()
-
         with tarfile.open(actions_json_location, "w:gz") as tar:
             tar.add(f.name, arcname="actions.json")
+    os.remove(tmpf)
 
     return 0
 
 
 if __name__ == "__main__":
     exit(scrape_iam_actions())
```

### Comparing `iam_ape-1.1.1/iam_ape/consts.py` & `iam_ape-1.1.2/iam_ape/consts.py`

 * *Files identical despite different names*

### Comparing `iam_ape-1.1.1/iam_ape/evaluator.py` & `iam_ape-1.1.2/iam_ape/evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import json
 import logging
-import re
 from collections import defaultdict
 from dataclasses import replace
 from fnmatch import fnmatch
-from typing import Any, Dict, List, Optional, Set, Tuple
+from typing import Any, Dict, Iterator, List, Optional, Set, Tuple
 
 from iam_ape.consts import PolicyElement
 from iam_ape.expand_policy import PolicyExpander
 from iam_ape.helper_classes import (
     Action,
     IneffectiveAction,
     PermissionsContainer,
@@ -471,17 +470,18 @@
 
 
 class EffectivePolicyEvaluator:
     def __init__(
         self,
         authorization_details: AuthorizationDetails,
         scp_policies: Optional[List[PolicyWithSource]] = None,
+        policy_expander: Optional[PolicyExpander] = None,
     ) -> None:
         self.auth_details = authorization_details
-        self.policy_expander = PolicyExpander()
+        self.policy_expander = policy_expander or PolicyExpander()
         self.scp_policy = (
             self.policy_expander.expand_policies(scp_policies)
             if scp_policies
             else PermissionsContainer()
         )
 
     def create_json_report(
@@ -635,40 +635,45 @@
                 action_tuple.action
             ]["denied_by"].add(action_tuple.denied_by)
 
         res = json.loads(json.dumps(res, default=serialize_set))
 
         return res
 
-    def get_managed_policies(
-        self, managed_policies: List[Dict[str, str]]
-    ) -> List[PolicyWithSource]:
-        res = []
-        for policy_details in managed_policies:
-            policy_arn = policy_details["PolicyArn"]
-            policy = get_default_policy_for_managed_policy(
-                self.auth_details.Policy.get(policy_arn, {})
-            )
-            res.append(PolicyWithSource(policy=policy, source=policy_arn))
-        return res
-
     def get_direct_policies(
         self, entity_obj: Dict[str, Any], entity_type: EntityType
     ) -> List[PolicyWithSource]:
         inline_policies = [
             PolicyWithSource(
                 "inline policy", normalize_policy(policy["PolicyDocument"])
             )
             for policy in entity_obj.get(f"{entity_type.value}PolicyList", [])
         ]
-        managed_policies = self.get_managed_policies(
-            entity_obj.get("AttachedManagedPolicies", [])
+        managed_policies = list(
+            self.get_managed_policies(entity_obj.get("AttachedManagedPolicies", []))
         )
         return managed_policies + inline_policies
 
+    def get_group_object_by_name(self, group_name: str) -> Optional[Dict[str, Any]]:
+        for group in self.auth_details.Group.values():
+            if group["GroupName"] == group_name:
+                return group
+        logger.warning(f"No such group {group_name}")
+        return None
+
+    def get_managed_policies(
+        self, managed_policies: List[Dict[str, str]]
+    ) -> Iterator[PolicyWithSource]:
+        for policy_details in managed_policies:
+            policy_arn = policy_details["PolicyArn"]
+            policy = get_default_policy_for_managed_policy(
+                self.auth_details.Policy.get(policy_arn, {})
+            )
+            yield PolicyWithSource(policy=policy, source=policy_arn)
+
     def get_permission_boundary(self, entity: Dict[str, Any]) -> PermissionsContainer:
         permissions = PermissionsContainer()
         if pb_arn := entity.get("PermissionsBoundary", {}).get(
             "PermissionsBoundaryArn"
         ):
             policy = PolicyWithSource(
                 source=pb_arn,
@@ -687,19 +692,19 @@
             logger.error(f"Error - couldn't find entity with ARN {arn}")
             raise ValueError(f"couldn't find entity with ARN {arn}")
 
         direct_policies = self.get_direct_policies(entity_obj, entity_type)
         indirect_policies: List[PolicyWithSource] = []
         if entity_type == EntityType.user:
             for group in entity_obj.get("GroupList", []):
-                group_arn = re.sub(":user/.*", f":group/{group}", entity_obj["Arn"])
-                group_obj = self.auth_details.Group[group_arn]
-                indirect_policies.extend(
-                    self.get_direct_policies(group_obj, EntityType.group)
-                )
+                group_obj = self.get_group_object_by_name(group)
+                if group_obj:
+                    indirect_policies.extend(
+                        self.get_direct_policies(group_obj, EntityType.group)
+                    )
 
         direct_permissions = self.policy_expander.expand_policies(
             direct_policies + indirect_policies
         )
         permission_boundary = self.get_permission_boundary(entity_obj)
 
         final_permissions, ineffective_permissions = explicitly_deny(direct_permissions)
```

### Comparing `iam_ape-1.1.1/iam_ape/expand_policy.py` & `iam_ape-1.1.2/iam_ape/expand_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,26 +26,28 @@
     action: str,
     service: str,
     resources: Optional[List[str]],
     not_resources: Optional[List[str]],
     condition: Optional[Dict[str, Any]],
     source: str,
 ) -> None:
-    def relevant_resource(resource: str, service: str) -> bool:
+    def relevant_resource(resource: str, action_service: str) -> bool:
         if resource.lower() in (
             "*",
             "arn:*",
             "arn:aws:*",
-            "arn:aws-gov:*",
-            "arn:aws-china:*",
+            "arn:aws-cn:*",
+            "arn:aws-us-gov:*",
         ):
             return True
         if match := RESOURCE_ARN_RE.match(resource):
-            res_service = match.group("service")
-            return res_service.lower() == service.lower()
+            resource_service = match.group("service").lower()
+            if resource_service == "iam" and action_service == "sts":
+                return True
+            return resource_service == action_service.lower()
         return False
 
     for resource in resources or []:
         if not relevant_resource(resource, service):
             continue
         if condition:
             for key, val in condition.items():
@@ -91,25 +93,30 @@
                     condition=None,
                     source=source,
                 )
             )
 
 
 class PolicyExpander:
-    def __init__(self) -> None:
-        self.all_iam_actions: CaseInsensitiveDict = self._init_iam_actions()
+    def __init__(self, all_iam_actions_file_location: Optional[str] = None) -> None:
+        self.all_iam_actions: CaseInsensitiveDict = self._init_iam_actions(
+            all_iam_actions_file_location
+        )
         self._all_service_wildcards: List[str] = [
             f"{k}:*" for k, v in self.all_iam_actions.items() if len(v) > 0
         ]
 
     @staticmethod
-    def _init_iam_actions() -> CaseInsensitiveDict:
+    def _init_iam_actions(
+        all_iam_actions_file_location: Optional[str] = None,
+    ) -> CaseInsensitiveDict:
         res: CaseInsensitiveDict = CaseInsensitiveDict()
+        file_path = all_iam_actions_file_location or actions_json_location
         try:
-            with tarfile.open(actions_json_location) as f:
+            with tarfile.open(file_path) as f:
                 data = json.load(f.extractfile("actions.json"))  # type: ignore
                 for k, v in data.items():
                     res[k] = CaseInsensitiveDict(v)
         except Exception as e:
             logger.exception(f"Failed to load AWS IAM Actions due to {e}")
         return res
```

### Comparing `iam_ape-1.1.1/iam_ape/helper_classes.py` & `iam_ape-1.1.2/iam_ape/helper_classes.py`

 * *Files identical despite different names*

### Comparing `iam_ape-1.1.1/iam_ape/helper_functions.py` & `iam_ape-1.1.2/iam_ape/helper_functions.py`

 * *Files identical despite different names*

### Comparing `iam_ape-1.1.1/iam_ape/helper_types.py` & `iam_ape-1.1.2/iam_ape/helper_types.py`

 * *Files identical despite different names*

### Comparing `iam_ape-1.1.1/iam_ape/main.py` & `iam_ape-1.1.2/iam_ape/main.py`

 * *Files identical despite different names*

### Comparing `iam_ape-1.1.1/pyproject.toml` & `iam_ape-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-ape"
-version = "1.1.1"
+version = "1.1.2"
 description = "IAM AWS Permissions Evaluator"
 authors = ["Tohar Braun, Orca Security <tohar@orca.security>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/orcasecurity/orca-toolbox/raw/main/iam-ape/"
 repository = "https://github.com/orcasecurity/orca-toolbox/raw/main/iam-ape/"
 keywords = ["aws", "iam"]
```

### Comparing `iam_ape-1.1.1/PKG-INFO` & `iam_ape-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-ape
-Version: 1.1.1
+Version: 1.1.2
 Summary: IAM AWS Permissions Evaluator
 Home-page: https://github.com/orcasecurity/orca-toolbox/raw/main/iam-ape/
 License: GPL-3.0-or-later
 Keywords: aws,iam
 Author: Tohar Braun, Orca Security
 Author-email: tohar@orca.security
 Requires-Python: >=3.8,<4.0
```

