# Comparing `tmp/pyattck_data-2.6.2.tar.gz` & `tmp/pyattck_data-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyattck_data-2.6.2.tar", max compression
+gzip compressed data, was "pyattck_data-2.6.3.tar", max compression
```

## Comparing `pyattck_data-2.6.2.tar` & `pyattck_data-2.6.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1065 2023-02-10 22:42:52.760817 pyattck_data-2.6.2/LICENSE
--rw-r--r--   0        0        0     1080 2023-02-10 22:42:52.760817 pyattck_data-2.6.2/LICENSE.rst
--rw-r--r--   0        0        0    13638 2023-02-10 22:42:52.760817 pyattck_data-2.6.2/README.md
--rw-r--r--   0        0        0     1686 2023-02-10 22:42:52.848817 pyattck_data-2.6.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-10 22:42:52.848817 pyattck_data-2.6.2/src/pyattck_data/__init__.py
--rw-r--r--   0        0        0     3647 2023-02-10 22:42:52.848817 pyattck_data-2.6.2/src/pyattck_data/actor.py
--rw-r--r--   0        0        0     2499 2023-02-10 22:42:52.848817 pyattck_data-2.6.2/src/pyattck_data/attack.py
--rw-r--r--   0        0        0     2256 2023-02-10 22:42:52.848817 pyattck_data-2.6.2/src/pyattck_data/base.py
--rw-r--r--   0        0        0     2310 2023-02-10 22:42:52.848817 pyattck_data-2.6.2/src/pyattck_data/campaign.py
--rw-r--r--   0        0        0     1128 2023-02-10 22:42:52.848817 pyattck_data-2.6.2/src/pyattck_data/control.py
--rw-r--r--   0        0        0     1524 2023-02-10 22:42:52.848817 pyattck_data-2.6.2/src/pyattck_data/datacomponent.py
--rw-r--r--   0        0        0     1857 2023-02-10 22:42:52.848817 pyattck_data-2.6.2/src/pyattck_data/datasource.py
--rw-r--r--   0        0        0     1367 2023-02-10 22:42:52.848817 pyattck_data-2.6.2/src/pyattck_data/definition.py
--rw-r--r--   0        0        0    11522 2023-02-10 22:42:52.848817 pyattck_data-2.6.2/src/pyattck_data/generated.py
--rw-r--r--   0        0        0     1110 2023-02-10 22:42:52.848817 pyattck_data-2.6.2/src/pyattck_data/identity.py
--rw-r--r--   0        0        0     4584 2023-02-10 22:42:52.848817 pyattck_data-2.6.2/src/pyattck_data/malware.py
--rw-r--r--   0        0        0     1409 2023-02-10 22:42:52.848817 pyattck_data-2.6.2/src/pyattck_data/matrix.py
--rw-r--r--   0        0        0     1867 2023-02-10 22:42:52.848817 pyattck_data-2.6.2/src/pyattck_data/mitigation.py
--rw-r--r--   0        0        0     2400 2023-02-10 22:42:52.848817 pyattck_data-2.6.2/src/pyattck_data/nist.py
--rw-r--r--   0        0        0        0 2023-02-10 22:42:52.848817 pyattck_data-2.6.2/src/pyattck_data/py.typed
--rw-r--r--   0        0        0     1216 2023-02-10 22:42:52.848817 pyattck_data-2.6.2/src/pyattck_data/relationship.py
--rw-r--r--   0        0        0     1849 2023-02-10 22:42:52.848817 pyattck_data-2.6.2/src/pyattck_data/tactic.py
--rw-r--r--   0        0        0     6036 2023-02-10 22:42:52.848817 pyattck_data-2.6.2/src/pyattck_data/technique.py
--rw-r--r--   0        0        0     4784 2023-02-10 22:42:52.848817 pyattck_data-2.6.2/src/pyattck_data/tool.py
--rw-r--r--   0        0        0     5361 2023-02-10 22:42:52.848817 pyattck_data-2.6.2/src/pyattck_data/types.py
--rw-r--r--   0        0        0    14973 1970-01-01 00:00:00.000000 pyattck_data-2.6.2/setup.py
--rw-r--r--   0        0        0    14676 1970-01-01 00:00:00.000000 pyattck_data-2.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-15 19:36:20.665864 pyattck_data-2.6.3/LICENSE
+-rw-r--r--   0        0        0     1080 2023-05-15 19:36:20.665864 pyattck_data-2.6.3/LICENSE.rst
+-rw-r--r--   0        0        0    13638 2023-05-15 19:36:20.665864 pyattck_data-2.6.3/README.md
+-rw-r--r--   0        0        0     1686 2023-05-15 19:36:20.749867 pyattck_data-2.6.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-15 19:36:20.749867 pyattck_data-2.6.3/src/pyattck_data/__init__.py
+-rw-r--r--   0        0        0     3647 2023-05-15 19:36:20.749867 pyattck_data-2.6.3/src/pyattck_data/actor.py
+-rw-r--r--   0        0        0     2499 2023-05-15 19:36:20.749867 pyattck_data-2.6.3/src/pyattck_data/attack.py
+-rw-r--r--   0        0        0     2256 2023-05-15 19:36:20.749867 pyattck_data-2.6.3/src/pyattck_data/base.py
+-rw-r--r--   0        0        0     2310 2023-05-15 19:36:20.749867 pyattck_data-2.6.3/src/pyattck_data/campaign.py
+-rw-r--r--   0        0        0     1128 2023-05-15 19:36:20.749867 pyattck_data-2.6.3/src/pyattck_data/control.py
+-rw-r--r--   0        0        0     1524 2023-05-15 19:36:20.749867 pyattck_data-2.6.3/src/pyattck_data/datacomponent.py
+-rw-r--r--   0        0        0     1857 2023-05-15 19:36:20.749867 pyattck_data-2.6.3/src/pyattck_data/datasource.py
+-rw-r--r--   0        0        0     1367 2023-05-15 19:36:20.749867 pyattck_data-2.6.3/src/pyattck_data/definition.py
+-rw-r--r--   0        0        0    11594 2023-05-15 19:36:20.749867 pyattck_data-2.6.3/src/pyattck_data/generated.py
+-rw-r--r--   0        0        0     1110 2023-05-15 19:36:20.749867 pyattck_data-2.6.3/src/pyattck_data/identity.py
+-rw-r--r--   0        0        0     4584 2023-05-15 19:36:20.749867 pyattck_data-2.6.3/src/pyattck_data/malware.py
+-rw-r--r--   0        0        0     1409 2023-05-15 19:36:20.749867 pyattck_data-2.6.3/src/pyattck_data/matrix.py
+-rw-r--r--   0        0        0     1867 2023-05-15 19:36:20.749867 pyattck_data-2.6.3/src/pyattck_data/mitigation.py
+-rw-r--r--   0        0        0     2400 2023-05-15 19:36:20.749867 pyattck_data-2.6.3/src/pyattck_data/nist.py
+-rw-r--r--   0        0        0        0 2023-05-15 19:36:20.749867 pyattck_data-2.6.3/src/pyattck_data/py.typed
+-rw-r--r--   0        0        0     1216 2023-05-15 19:36:20.749867 pyattck_data-2.6.3/src/pyattck_data/relationship.py
+-rw-r--r--   0        0        0     1849 2023-05-15 19:36:20.749867 pyattck_data-2.6.3/src/pyattck_data/tactic.py
+-rw-r--r--   0        0        0     6126 2023-05-15 19:36:20.749867 pyattck_data-2.6.3/src/pyattck_data/technique.py
+-rw-r--r--   0        0        0     4784 2023-05-15 19:36:20.749867 pyattck_data-2.6.3/src/pyattck_data/tool.py
+-rw-r--r--   0        0        0     5361 2023-05-15 19:36:20.749867 pyattck_data-2.6.3/src/pyattck_data/types.py
+-rw-r--r--   0        0        0    14973 1970-01-01 00:00:00.000000 pyattck_data-2.6.3/setup.py
+-rw-r--r--   0        0        0    14676 1970-01-01 00:00:00.000000 pyattck_data-2.6.3/PKG-INFO
```

### Comparing `pyattck_data-2.6.2/LICENSE` & `pyattck_data-2.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyattck_data-2.6.2/LICENSE.rst` & `pyattck_data-2.6.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pyattck_data-2.6.2/README.md` & `pyattck_data-2.6.3/README.md`

 * *Files identical despite different names*

### Comparing `pyattck_data-2.6.2/pyproject.toml` & `pyattck_data-2.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyattck-data"
-version = "2.6.2"
+version = "2.6.3"
 description = "Pyattck Data"
 authors = ["Swimlane <info@swimlane.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/swimlane/pyattck-data"
 repository = "https://github.com/swimlane/pyattck-data"
 classifiers = [
```

### Comparing `pyattck_data-2.6.2/src/pyattck_data/actor.py` & `pyattck_data-2.6.3/src/pyattck_data/actor.py`

 * *Files identical despite different names*

### Comparing `pyattck_data-2.6.2/src/pyattck_data/attack.py` & `pyattck_data-2.6.3/src/pyattck_data/attack.py`

 * *Files identical despite different names*

### Comparing `pyattck_data-2.6.2/src/pyattck_data/base.py` & `pyattck_data-2.6.3/src/pyattck_data/base.py`

 * *Files identical despite different names*

### Comparing `pyattck_data-2.6.2/src/pyattck_data/campaign.py` & `pyattck_data-2.6.3/src/pyattck_data/campaign.py`

 * *Files identical despite different names*

### Comparing `pyattck_data-2.6.2/src/pyattck_data/control.py` & `pyattck_data-2.6.3/src/pyattck_data/control.py`

 * *Files identical despite different names*

### Comparing `pyattck_data-2.6.2/src/pyattck_data/datacomponent.py` & `pyattck_data-2.6.3/src/pyattck_data/datacomponent.py`

 * *Files identical despite different names*

### Comparing `pyattck_data-2.6.2/src/pyattck_data/datasource.py` & `pyattck_data-2.6.3/src/pyattck_data/datasource.py`

 * *Files identical despite different names*

### Comparing `pyattck_data-2.6.2/src/pyattck_data/definition.py` & `pyattck_data-2.6.3/src/pyattck_data/definition.py`

 * *Files identical despite different names*

### Comparing `pyattck_data-2.6.2/src/pyattck_data/generated.py` & `pyattck_data-2.6.3/src/pyattck_data/generated.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,31 +229,32 @@
                     )
                 )
 
     def add_dataset(self, technique_id, content):
         if self.techniques:
             found = False
             for technique in self.techniques:
-                if technique.technique_id == technique_id:
+                if technique.technique_id == technique_id and content:
                     found = True
                     technique.parsed_datasets.append(content)
-            if not found:
+            if not found and content:
                 self.techniques.append(
                     Technique(
                         technique_id=technique_id,
                         parsed_datasets=[content]
                     )
                 )
         else:
-            self.techniques.append(
-                    Technique(
-                        technique_id=technique_id,
-                        parsed_datasets=[content]
+            if content:
+                self.techniques.append(
+                        Technique(
+                            technique_id=technique_id,
+                            parsed_datasets=[content]
+                        )
                     )
-                )
 
     def add_possible_queries(self, technique_id, product, content, name):
         q = Query(
             product=product,
             query=content,
             name=name
         )
```

### Comparing `pyattck_data-2.6.2/src/pyattck_data/identity.py` & `pyattck_data-2.6.3/src/pyattck_data/identity.py`

 * *Files identical despite different names*

### Comparing `pyattck_data-2.6.2/src/pyattck_data/malware.py` & `pyattck_data-2.6.3/src/pyattck_data/malware.py`

 * *Files identical despite different names*

### Comparing `pyattck_data-2.6.2/src/pyattck_data/matrix.py` & `pyattck_data-2.6.3/src/pyattck_data/matrix.py`

 * *Files identical despite different names*

### Comparing `pyattck_data-2.6.2/src/pyattck_data/mitigation.py` & `pyattck_data-2.6.3/src/pyattck_data/mitigation.py`

 * *Files identical despite different names*

### Comparing `pyattck_data-2.6.2/src/pyattck_data/nist.py` & `pyattck_data-2.6.3/src/pyattck_data/nist.py`

 * *Files identical despite different names*

### Comparing `pyattck_data-2.6.2/src/pyattck_data/relationship.py` & `pyattck_data-2.6.3/src/pyattck_data/relationship.py`

 * *Files identical despite different names*

### Comparing `pyattck_data-2.6.2/src/pyattck_data/tactic.py` & `pyattck_data-2.6.3/src/pyattck_data/tactic.py`

 * *Files identical despite different names*

### Comparing `pyattck_data-2.6.2/src/pyattck_data/technique.py` & `pyattck_data-2.6.3/src/pyattck_data/technique.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,17 +71,19 @@
 
     command_list: List = field(factory=list)
     commands: List[Command] = field(factory=list) # need to define this object better
     queries: List = field(factory=list) # need to define this object better
     parsed_datasets: List = field(factory=list) # need to define this object better
     possible_detections: List = field(factory=list) # need to define this object better
     external_reference: List = field(factory=list)
-
     controls: List = field(factory=list)
 
+    # Added in v13 of ATT&CK
+    x_mitre_network_requirements: bool = field(factory=bool)
+
     # additional convenience properties 
     technique_id: AnyStr = field(factory=str)
     stix: Id = field(factory=Id)
 
     @property
     def actors(self):
         return self._get_relationship_objects(
```

### Comparing `pyattck_data-2.6.2/src/pyattck_data/tool.py` & `pyattck_data-2.6.3/src/pyattck_data/tool.py`

 * *Files identical despite different names*

### Comparing `pyattck_data-2.6.2/src/pyattck_data/types.py` & `pyattck_data-2.6.3/src/pyattck_data/types.py`

 * *Files identical despite different names*

### Comparing `pyattck_data-2.6.2/setup.py` & `pyattck_data-2.6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'importlib-metadata<3.4',
  'openpyxl>=3.0.10,<4.0.0',
  'pydantic>=1.9.1,<2.0.0',
  'requests>=2.28.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'pyattck-data',
-    'version': '2.6.2',
+    'version': '2.6.3',
     'description': 'Pyattck Data',
     'long_description': '# pyattck-data\n\n<a href="https://pypi.org/project/pyattck-data-models/"><img src="https://img.shields.io/pypi/v/pyattck-data-models.svg" alt="PyPI" style="float: left; margin-right: 10px;" /></a>\n<a href="https://pypi.org/project/pyattck-data-models/"><img src="https://img.shields.io/pypi/status/pyattck-data-models.svg" alt="Status" style="float: left; margin-right: 10px;" /></a>\n<a href="https://pypi.org/project/pyattck-data-models/"><img src="https://img.shields.io/pypi/pyversions/pyattck-data-models" alt="Python Version" style="float: left; margin-right: 10px;" /></a>\n<a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/pypi/l/pyattck-data-models" alt="License" style="float: left; margin-right: 10px;" /></a>\n<a href="https://github.com/swimlane/pyattck-data-models/actions?workflow=Tests"><img src="https://github.com/swimlane/pyattck-data-models/workflows/Tests/badge.svg" alt="Tests" style="float: left; margin-right: 10px;" /></a>\n<a href="https://codecov.io/gh/swimlane/pyattck-data-models"><img src="https://codecov.io/gh/swimlane/pyattck-data-models/branch/main/graph/badge.svg" alt="Codecov" style="float: left; margin-right: 10px;" /></a>\n<a href="https://github.com/pre-commit/pre-commit"><img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white" alt="pre-commit" style="float: left; margin-right: 10px;" /></a>\n<a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Black" style="float: left; margin-right: 10px;" /></a>\n\n\n## Features\n\nIncludes data models for the following projects:\n\n* [pyattck](https://github.com/swimlane/pyattck/)\n\n\nThis repository contains generated contextual data utilized by pyattck.\n\n## Generated Data Access\n\nGenerated data can be retrieved from the following URLs:\n\n* Enterprise ATT&CK JSON (merged with external data) - [https://swimlane-pyattck.s3.us-west-2.amazonaws.com/merged_enterprise_attck_v1.json](https://swimlane-pyattck.s3.us-west-2.amazonaws.com/merged_enterprise_attck_v1.json)\n* Pre-ATT&CK JSON (merged with external data) - [https://swimlane-pyattck.s3.us-west-2.amazonaws.com/merged_pre_attck_v1.json](https://swimlane-pyattck.s3.us-west-2.amazonaws.com/merged_pre_attck_v1.json)\n* Mobile ATT&CK JSON (merged with external data) - [https://swimlane-pyattck.s3.us-west-2.amazonaws.com/merged_mobile_attck_v1.json](https://swimlane-pyattck.s3.us-west-2.amazonaws.com/merged_mobile_attck_v1.json)\n* ICS ATT&CK JSON (merged with external data) - [https://swimlane-pyattck.s3.us-west-2.amazonaws.com/merged_ics_attck_v1.json](https://swimlane-pyattck.s3.us-west-2.amazonaws.com/merged_ics_attck_v1.json)\n* NIST Controls JSON - [https://swimlane-pyattck.s3.us-west-2.amazonaws.com/merged_nist_controls_v1.json](https://swimlane-pyattck.s3.us-west-2.amazonaws.com/merged_nist_controls_v1.json)\n* Generated NIST JSON - [https://swimlane-pyattck.s3.us-west-2.amazonaws.com/attck_to_nist_controls.json](https://swimlane-pyattck.s3.us-west-2.amazonaws.com/attck_to_nist_controls.json)\n* generated_attck_data.json - [https://swimlane-pyattck.s3.us-west-2.amazonaws.com/generated_attck_data.json](https://swimlane-pyattck.s3.us-west-2.amazonaws.com/generated_attck_data.json)\n* generated_attck_data_v2.json - [https://swimlane-pyattck.s3.us-west-2.amazonaws.com/generated_attck_data_v2.json](https://swimlane-pyattck.s3.us-west-2.amazonaws.com/generated_attck_data_v2.json)\n\n# Generated ATT&CK Datasets\n\nThis page outlines and provides detailed information regarding the data generated and used with the `pyattck` python package.\n\n## Data Categories\n\nAt this time, a shareable JSON file is generated on the `1st` and `15th` of the month and stored in a S3 bucket. This data is used and retrieved by `pyattck`.\n\nThis generated json file has the following main keys:\n\n- timestamp\n- techniques\n    - technique_id\n    - commands\n    - parsed_datasets\n    - command_list\n    - attack_paths\n    - queries\n    - possible_detections\n- actors\n    - israel\n    - iran\n    - middle_east\n    - north_korea\n    - china\n    - unknown\n    - other\n    - nato\n    - russia\n    - Each actor will have the following data structure\n        - actor_names\n        - target\n        - operations\n        - description\n        - tools\n        - links\n        - attck_id\n        - comment\n- tools\n    - names\n    - links\n    - family\n    - comments\n- c2_data\n    - name_of_c2\n        - HTTP\n        - Implementation\n        - Custom Profile\n        - DomainFront\n        - Multi-User\n        - SMB\n        - Kill Date\n        - macOS\n        - GitHub\n        - Key Exchange\n        - Chaining\n        - Price\n        - TCP\n        - Proxy Aware\n        - HTTP3\n        - HTTP2\n        - Date\n        - Evaluator\n        - Working Hours\n        - Slack\n        - FTP\n        - Version Reviewed\n        - Logging\n        - Name\n        - License\n        - Windows\n        - Stego\n        - Notes\n        - Server\n        - Actively Maint.\n        - Dashboard\n        - DNS\n        - Popular Site\n        - ICMP\n        - IMAP\n        - DoH\n        - Jitter\n        - How-To\n        - ATT&CK Mapping\n        - Kali\n        - Twitter\n        - MAPI\n        - Site\n        - Agent\n        - API\n        - UI\n        - Linux\n\n\n## Generated Attck Data Structure\n\nThe [generated_attck_data.json](https://swimlane-pyattck.s3.us-west-2.amazonaws.com/generated_attck_data.json) has the following base structure. This is purely an example and contains modified/fake data.\n\n\n```json\n\n{\n    "last_updated": "2019-12-06T15:21:02.175108", \n    "techniques": [\n        {\n            "technique_id": "T1082", \n            "commands": [\n                {\n                    "source": "https://attack.mitre.org/docs/APT3_Adversary_Emulation_Field_Manual.xlsx", \n                    "command": "whoami /all /fo list", \n                    "name": "Built-in Windows Command"\n                },\n                {\n                    "source": "atomics/T1033/T1033.yaml", \n                    "command": "cmd.exe /C whoami\\nwmic useraccount get /ALL\\nquser /SERVER:\\"computer1\\"\\nquser\\nqwinsta.exe\\" /server:computer1\\nqwinsta.exe\\nfor /F \\"tokens=1,2\\" %i in (\'qwinsta /server:computer1 ^| findstr \\"Active Disc\\"\') do @echo %i | find /v \\"#\\" | find /v \\"console\\" || echo %j > usernames.txt\\n@FOR /F %n in (computers.txt) DO @FOR /F \\"tokens=1,2\\" %i in (\'qwinsta /server:%n ^| findstr \\"Active Disc\\"\') do @echo %i | find /v \\"#\\" | find /v \\"console\\" || echo %j > usernames.txt\\n", \n                    "name": null\n                }\n            ],\n            "command_list": [\n                    "ver", \n                    "shell ver", \n                    "set", \n                    "shell set", \n                    "get_env.rb", \n                    "net config workstation",\n                    "net config server", \n                    "shell net config workstation",\n                    "reg query HKLM\\\\SYSTEM\\\\CurrentControlSet\\\\Services\\\\Disk\\\\Enum"\n            ], \n            "parsed_datasets": [\n                {\n                    "Mitre APT3 Adversary Emulation Field Manual": {"Category": "T1033", "Built-in Windows Command": "whoami /all /fo list", "Cobalt Strike": "shell whoami /all /fo list", "Description": "Get current user information, SID, domain, groups the user belongs to, security privs of the user", "Metasploit": "getuid"}\n                },\n                {\n                    "Atomic Red Team Test - System Owner/User Discovery": {"display_name": "System Owner/User Discovery", "atomic_tests": [{"executor": {"elevation_required": false, "command": "cmd.exe /C whoami\\nwmic useraccount get /ALL\\nquser /SERVER:\\"#{computer_name}\\"\\nquser\\nqwinsta.exe\\" /server:#{computer_name}\\nqwinsta.exe\\nfor /F \\"tokens=1,2\\" %i in (\'qwinsta /server:#{computer_name} ^| findstr \\"Active Disc\\"\') do @echo %i | find /v \\"#\\" | find /v \\"console\\" || echo %j > usernames.txt\\n@FOR /F %n in (computers.txt) DO @FOR /F \\"tokens=1,2\\" %i in (\'qwinsta /server:%n ^| findstr \\"Active Disc\\"\') do @echo %i | find /v \\"#\\" | find /v \\"console\\" || echo %j > usernames.txt\\n", "name": "command_prompt"}, "supported_platforms": ["windows"], "description": "Identify System owner or users on an endpoint\\n", "input_arguments": {"computer_name": {"default": "computer1", "type": "string", "description": "Name of remote computer"}}, "name": "System Owner/User Discovery"}, {"executor": {"elevation_required": false, "command": "users\\nw\\nwho\\n", "name": "sh"}, "supported_platforms": ["linux", "macos"], "description": "Identify System owner or users on an endpoint\\n", "name": "System Owner/User Discovery"}], "attack_technique": "T1033"}\n                }\n            ],\n            "queries": [\n                {\n                    "query": "Sysmon| where EventID == 1 and (process_path contains\\"sysinfo.exe\\"or process_path contains \\"reg.exe\\")and process_commandline contains \\"reg*query HKLM\\\\\\\\SYSTEM\\\\\\\\CurrentControlSet\\\\\\\\Services\\\\\\\\Disk\\\\\\\\Enum\\"", \n                    "product": "Azure Sentinel", \n                    "name": "System Information Discovery"\n                },\n                {\n                    "query": "title: Reconnaissance Activity with Net Command\\nid: 2887e914-ce96-435f-8105-593937e90757\\nstatus: experimental\\ndescription: Detects a set of commands often used in recon stages by different attack groups\\nreferences:\\n    - https://twitter.com/haroonmeer/status/939099379834658817\\n    - https://twitter.com/c_APT_ure/status/939475433711722497\\n    - https://www.fireeye.com/blog/threat-research/2016/05/targeted_attacksaga.html\\nauthor: Florian Roth, Markus Neis\\ndate: 2018/08/22\\nmodified: 2018/12/11\\ntags:\\n    - attack.discovery\\n    - attack.t1087\\n    - attack.t1082\\n    - car.2016-03-001\\nlogsource:\\n    category: process_creation\\n    product: windows\\ndetection:\\n    selection:\\n        CommandLine:\\n            - tasklist\\n            - net time\\n            - systeminfo\\n            - whoami\\n            - nbtstat\\n            - net start\\n            - \'*\\\\net1 start\'\\n            - qprocess\\n            - nslookup\\n            - hostname.exe\\n            - \'*\\\\net1 user /domain\'\\n            - \'*\\\\net1 group /domain\'\\n            - \'*\\\\net1 group \\"domain admins\\" /domain\'\\n            - \'*\\\\net1 group \\"Exchange Trusted Subsystem\\" /domain\'\\n            - \'*\\\\net1 accounts /domain\'\\n            - \'*\\\\net1 user net localgroup administrators\'\\n            - netstat -an\\n    timeframe: 15s\\n    condition: selection | count() by CommandLine > 4\\nfalsepositives:\\n    - False positives depend on scripts and administrative tools used in the monitored environment\\nlevel: medium", "product": "Atomic Threat Coverage", \n                    "name": "Sigma rule"\n                },\n                {\n                    "query": "(CommandLine=\\"tasklist\\" OR CommandLine=\\"net time\\" OR CommandLine=\\"systeminfo\\" OR CommandLine=\\"whoami\\" OR CommandLine=\\"nbtstat\\" OR CommandLine=\\"net start\\" OR CommandLine=\\"*\\\\\\\\\\\\\\\\net1 start\\" OR CommandLine=\\"qprocess\\" OR CommandLine=\\"nslookup\\" OR CommandLine=\\"hostname.exe\\" OR CommandLine=\\"*\\\\\\\\\\\\\\\\net1 user /domain\\" OR CommandLine=\\"*\\\\\\\\\\\\\\\\net1 group /domain\\" OR CommandLine=\\"*\\\\\\\\\\\\\\\\net1 group \\\\\\\\\\"domain admins\\\\\\\\\\" /domain\\" OR CommandLine=\\"*\\\\\\\\\\\\\\\\net1 group \\\\\\\\\\"Exchange Trusted Subsystem\\\\\\\\\\" /domain\\" OR CommandLine=\\"*\\\\\\\\\\\\\\\\net1 accounts /domain\\" OR CommandLine=\\"*\\\\\\\\\\\\\\\\net1 user net localgroup administrators\\" OR CommandLine=\\"netstat -an\\") | eventstats count as val by CommandLine| search val > 4", \n                    "product": "Atomic Threat Coverage", \n                    "name": "splunk"\n                }\n            ],\n}\n```\n\n## Sources\n\n\n> **First of all, I would like to thank everyone who contributes to open-source projects, especially the maintainers and creators of these projects.  Without them, this capability would not be possible.**\n\nThis data set is generated from many different sources. As we continue to add more sources, we will continue to add them here.  Again thank you to all of these projects.  In no particular order, `pyattck` utilizes data from the following projects:\n\n* [Mitre ATT&CK APT3 Adversary Emulation Field Manual](https://attack.mitre.org/docs/APT3_Adversary_Emulation_Field_Manual.xlsx)\n* [Atomic Red Team (by Red Canary)](https://github.com/redcanaryco/atomic-red-team)\n* [Atomic Threat Coverage](https://github.com/atc-project/atomic-threat-coverage)\n* [attck_empire (by dstepanic)](https://github.com/dstepanic/attck_empire)\n* [sentinel-attack (by BlueTeamLabs)](https://github.com/BlueTeamLabs/sentinel-attack)\n* [Litmus_test (by Kirtar22)](https://github.com/Kirtar22/Litmus_Test)\n* [nsm-attack (by oxtf)](https://github.com/0xtf/nsm-attack)\n* [osquery-attck (by teoseller)](https://github.com/teoseller/osquery-attck)\n* [Mitre Stockpile](https://github.com/mitre/stockpile)\n* [SysmonHunter (by baronpan)](https://github.com/baronpan/SysmonHunter)\n* [ThreatHunting-Book (by 12306Bro)](https://github.com/12306Bro/Threathunting-book)\n* [threat_hunting_tables (by dwestgard)](https://github.com/dwestgard/threat_hunting_tables)\n* [APT Groups & Operations](https://docs.google.com/spreadsheets/d/1H9_xaxQHpWaa4O_Son4Gx0YOIzlcBWMsdvePFX68EKU/edit#gid=1864660085)\n* [C2Matrix (by @jorgeorchilles, @brysonbort, @adam_mashinchi)](https://www.thec2matrix.com/)\n* [Elemental](https://github.com/Elemental-attack/Elemental)\n* [MalwareArchaeology - ATTACK](https://github.com/MalwareArchaeology/ATTACK)\n* [Attack-Technique-Dataset](https://github.com/NewBee119/Attack-Technique-Dataset)\n\n',
     'author': 'Swimlane',
     'author_email': 'info@swimlane.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/swimlane/pyattck-data',
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['pyattck_data'] package_data = \ {'': ['*']}
 install_requires = \ ['PyYAML>=6.0,<7.0', 'attrs>=21.4.0,<22.0.0', 'importlib-
 metadata<3.4', 'openpyxl>=3.0.10,<4.0.0', 'pydantic>=1.9.1,<2.0.0',
 'requests>=2.28.0,<3.0.0'] setup_kwargs = { 'name': 'pyattck-data', 'version':
-'2.6.2', 'description': 'Pyattck Data', 'long_description': '# pyattck-data\n\n
+'2.6.3', 'description': 'Pyattck Data', 'long_description': '# pyattck-data\n\n
 [PyPI]\n[Status]\n[Python_Version]\n[License]\n[Tests]\n[Codecov]\n[pre-
 commit]\n[Black]\n\n\n## Features\n\nIncludes data models for the following
 projects:\n\n* [pyattck](https://github.com/swimlane/pyattck/)\n\n\nThis
 repository contains generated contextual data utilized by pyattck.\n\n##
 Generated Data Access\n\nGenerated data can be retrieved from the following
 URLs:\n\n* Enterprise ATT&CK JSON (merged with external data) - [https://
 swimlane-pyattck.s3.us-west-2.amazonaws.com/merged_enterprise_attck_v1.json]
```

### Comparing `pyattck_data-2.6.2/PKG-INFO` & `pyattck_data-2.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyattck-data
-Version: 2.6.2
+Version: 2.6.3
 Summary: Pyattck Data
 Home-page: https://github.com/swimlane/pyattck-data
 License: MIT
 Author: Swimlane
 Author-email: info@swimlane.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyattck-data Version: 2.6.2 Summary: Pyattck Data
+Metadata-Version: 2.1 Name: pyattck-data Version: 2.6.3 Summary: Pyattck Data
 Home-page: https://github.com/swimlane/pyattck-data License: MIT Author:
 Swimlane Author-email: info@swimlane.com Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

