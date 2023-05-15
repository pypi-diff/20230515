# Comparing `tmp/python-zephyr-0.0.5.tar.gz` & `tmp/python-zephyr-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\python-zephyr-0.0.5.tar", last modified: Tue Aug 30 12:38:40 2022, max compression
+gzip compressed data, was "python-zephyr-0.0.6.tar", last modified: Mon May 15 15:08:49 2023, max compression
```

## Comparing `python-zephyr-0.0.5.tar` & `python-zephyr-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2022-08-30 12:38:40.557875 python-zephyr-0.0.5/
--rw-rw-rw-   0        0        0     1105 2022-08-29 22:31:19.000000 python-zephyr-0.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0     1369 2022-08-30 12:38:40.556923 python-zephyr-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      786 2022-08-29 22:31:19.000000 python-zephyr-0.0.5/README.md
--rw-rw-rw-   0        0        0       86 2022-08-29 22:31:19.000000 python-zephyr-0.0.5/pyproject.toml
-drwxrwxrwx   0        0        0        0 2022-08-30 12:38:40.539797 python-zephyr-0.0.5/python_zephyr.egg-info/
--rw-rw-rw-   0        0        0     1369 2022-08-30 12:38:40.000000 python-zephyr-0.0.5/python_zephyr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2022-08-30 12:38:40.000000 python-zephyr-0.0.5/python_zephyr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-30 12:38:40.000000 python-zephyr-0.0.5/python_zephyr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-08-30 12:38:40.000000 python-zephyr-0.0.5/python_zephyr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-08-30 12:38:40.000000 python-zephyr-0.0.5/python_zephyr.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-08-30 12:38:40.541700 python-zephyr-0.0.5/scripts/
--rw-rw-rw-   0        0        0     1633 2022-08-29 22:31:19.000000 python-zephyr-0.0.5/scripts/tc_report_upload.py
--rw-rw-rw-   0        0        0       42 2022-08-30 12:38:40.558828 python-zephyr-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1111 2022-08-30 11:51:11.000000 python-zephyr-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-30 12:38:40.555020 python-zephyr-0.0.5/zephyr/
--rw-rw-rw-   0        0        0       22 2022-08-29 22:31:19.000000 python-zephyr-0.0.5/zephyr/__init__.py
--rw-rw-rw-   0        0        0      870 2022-08-29 22:31:19.000000 python-zephyr-0.0.5/zephyr/exceptions.py
--rw-rw-rw-   0        0        0    15556 2022-08-30 11:51:11.000000 python-zephyr-0.0.5/zephyr/interface.py
--rw-rw-rw-   0        0        0    22823 2022-08-30 11:51:11.000000 python-zephyr-0.0.5/zephyr/tc_mgmt.py
+drwxrwxrwx   0        0        0        0 2023-05-15 15:08:49.336676 python-zephyr-0.0.6/
+-rw-rw-rw-   0        0        0     1105 2023-05-15 15:00:37.000000 python-zephyr-0.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     1369 2023-05-15 15:08:49.335677 python-zephyr-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      786 2023-05-15 15:00:37.000000 python-zephyr-0.0.6/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-15 15:00:37.000000 python-zephyr-0.0.6/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-15 15:08:49.329675 python-zephyr-0.0.6/python_zephyr.egg-info/
+-rw-rw-rw-   0        0        0     1369 2023-05-15 15:08:49.000000 python-zephyr-0.0.6/python_zephyr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2023-05-15 15:08:49.000000 python-zephyr-0.0.6/python_zephyr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 15:08:49.000000 python-zephyr-0.0.6/python_zephyr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-15 15:08:49.000000 python-zephyr-0.0.6/python_zephyr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-15 15:08:49.000000 python-zephyr-0.0.6/python_zephyr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-15 15:08:49.330677 python-zephyr-0.0.6/scripts/
+-rw-rw-rw-   0        0        0     1570 2023-05-15 15:00:37.000000 python-zephyr-0.0.6/scripts/tc_report_upload.py
+-rw-rw-rw-   0        0        0       42 2023-05-15 15:08:49.336676 python-zephyr-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1111 2023-05-15 15:07:59.000000 python-zephyr-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 15:08:49.334675 python-zephyr-0.0.6/zephyr/
+-rw-rw-rw-   0        0        0       22 2023-05-15 15:00:37.000000 python-zephyr-0.0.6/zephyr/__init__.py
+-rw-rw-rw-   0        0        0      875 2023-05-15 15:00:37.000000 python-zephyr-0.0.6/zephyr/exceptions.py
+-rw-rw-rw-   0        0        0    15600 2023-05-15 15:00:37.000000 python-zephyr-0.0.6/zephyr/interface.py
+-rw-rw-rw-   0        0        0    21826 2023-05-15 15:00:37.000000 python-zephyr-0.0.6/zephyr/tc_mgmt.py
```

### Comparing `python-zephyr-0.0.5/LICENSE.txt` & `python-zephyr-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-zephyr-0.0.5/PKG-INFO` & `python-zephyr-0.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-zephyr
-Version: 0.0.5
+Version: 0.0.6
 Summary: An easy to use Zephyr Scale library for python
 Home-page: https://bitbucket.org/melectrification/python-zephyr/src/master/
 Author: Atabey Onur
 Author-email: a.onur@munichelectrification.com
 Maintainer: Atabey Onur
 Maintainer-email: a.onur@munichelectrification.com
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python-zephyr-0.0.5/README.md` & `python-zephyr-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `python-zephyr-0.0.5/python_zephyr.egg-info/PKG-INFO` & `python-zephyr-0.0.6/python_zephyr.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-zephyr
-Version: 0.0.5
+Version: 0.0.6
 Summary: An easy to use Zephyr Scale library for python
 Home-page: https://bitbucket.org/melectrification/python-zephyr/src/master/
 Author: Atabey Onur
 Author-email: a.onur@munichelectrification.com
 Maintainer: Atabey Onur
 Maintainer-email: a.onur@munichelectrification.com
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python-zephyr-0.0.5/scripts/tc_report_upload.py` & `python-zephyr-0.0.6/scripts/tc_report_upload.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,39 +4,37 @@
 
 def main():
     """
     Main function.
     """
     import argparse
 
-    parser = argparse.ArgumentParser(
-        description='Upload test results to Zephyr Test Database.')
-    parser.add_argument(
-        '--token', help='Zephyr API token file.', required=True)
-    parser.add_argument(
-        '--sw_ver', help='Software version of the DUT. (Format: XXXXXXXX_XXXXXXXX)', required=True)
-    parser.add_argument(
-        '--hw_ver', help='Hardware version of the DUT.', required=True)
-    parser.add_argument(
-        '--test_key', help='key of the test. (e.g. BSBS-T1)', required=True)
-    parser.add_argument(
-        '--test_result', help='Result of the test (PASS, FAIL, NOT EXECUTED).', required=True)
-    parser.add_argument('--execution_time',
-                        help='Execution time of the test.', required=True)
-    parser.add_argument(
-        '--log_path', help='Path to the test log.', required=True)
-    parser.add_argument(
-        '--comments', help='Comments to be added to the test.', required=True)
-    parser.add_argument(
-        '--env_name', help='Name of the test environment.', required=False)
+    parser = argparse.ArgumentParser(description="Upload test results to Zephyr Test Database.")
+    parser.add_argument("--token", help="Zephyr API token file.", required=True)
+    parser.add_argument("--sw_ver", help="Software version of the DUT. (Format: XXXXXXXX_XXXXXXXX)", required=True)
+    parser.add_argument("--hw_ver", help="Hardware version of the DUT.", required=True)
+    parser.add_argument("--test_key", help="key of the test. (e.g. BSBS-T1)", required=True)
+    parser.add_argument("--test_result", help="Result of the test (PASS, FAIL, NOT EXECUTED).", required=True)
+    parser.add_argument("--execution_time", help="Execution time of the test.", required=True)
+    parser.add_argument("--log_path", help="Path to the test log.", required=True)
+    parser.add_argument("--comments", help="Comments to be added to the test.", required=True)
+    parser.add_argument("--env_name", help="Name of the test environment.", required=False)
     args = parser.parse_args()
 
-    with open(args.token, 'r') as token_file:
+    with open(args.token, "r") as token_file:
         token = token_file.read().strip()
 
     tc_mgmt = tc_lib.TestManagement(token)
-    tc_mgmt.upload_results(args.sw_ver, args.hw_ver, args.test_key, tc_lib.TestVerdicts[args.test_result],
-                           int(args.execution_time), args.log_path, args.comments, args.env_name)
+    tc_mgmt.upload_results(
+        args.sw_ver,
+        args.hw_ver,
+        args.test_key,
+        tc_lib.TestVerdicts[args.test_result],
+        int(args.execution_time),
+        args.log_path,
+        args.comments,
+        args.env_name,
+    )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `python-zephyr-0.0.5/setup.py` & `python-zephyr-0.0.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 with open(os.path.join(HERE, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 packages = find_packages(".")
 
 setup(
     name="python-zephyr",
-    version="0.0.5",
+    version="0.0.6",
     description="An easy to use Zephyr Scale library for python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     scripts=list(filter(os.path.isfile, (os.path.join("scripts/", f) for f in os.listdir("scripts/")))),
     author="Atabey Onur",
     author_email="a.onur@munichelectrification.com",
     maintainer="Atabey Onur",
```

### Comparing `python-zephyr-0.0.5/zephyr/exceptions.py` & `python-zephyr-0.0.6/zephyr/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 """
 Exceptions that may be raised by Zephyr interface classes.
 """
 
 
 class FolderNotFoundError(Exception):
-    """ Name doesnt exist """
+    """Name doesn't exist"""
+
     def __init__(self, *args, **kwargs):  # real signature unknown
         pass
 
 
 class ProjectNotFoundError(Exception):
-    """ Project doesnt exist """
+    """Project doesn't exist"""
+
     def __init__(self, *args, **kwargs):  # real signature unknown
         pass
 
 
 class BadResponseError(Exception):
-    """ Response is not valid """
+    """Response is not valid"""
+
     def __init__(self, *args, **kwargs):  # real signature unknown
         pass
 
 
 class TestCaseNotFoundError(Exception):
-    """ Test case doesnt exist """
+    """Test case doesn't exist"""
+
     def __init__(self, *args, **kwargs):  # real signature unknown
         pass
 
 
 class TestCycleNotFoundError(Exception):
-    """ Test case doesnt exist """
+    """Test cycle doesn't exist"""
+
     def __init__(self, *args, **kwargs):  # real signature unknown
         pass
```

### Comparing `python-zephyr-0.0.5/zephyr/interface.py` & `python-zephyr-0.0.6/zephyr/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,17 +188,21 @@
             if matched_dict is not None:
                 return matched_dict["id"]
             else:
                 raise exceptions.FolderNotFoundError(f"Folder {project_key} not found")
         else:
             return None
 
-
     def get_all_folders(
-        self, project_key: str = None, folder_type: Literal["TEST_CASE", "TEST_PLAN", "TEST_CYCLE"] = "TEST_CASE", timeout_s: float = 1.0, *args, **kwargs
+        self,
+        project_key: str = None,
+        folder_type: Literal["TEST_CASE", "TEST_PLAN", "TEST_CYCLE"] = "TEST_CASE",
+        timeout_s: float = 1.0,
+        *args,
+        **kwargs,
     ):
         """
         Gets folders from Zephyr
 
         :param project_key:
             key of the project we want to look at
         :param folder_type:
```

### Comparing `python-zephyr-0.0.5/zephyr/tc_mgmt.py` & `python-zephyr-0.0.6/zephyr/tc_mgmt.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,46 +107,50 @@
         url = self.base_url + "/testcases/{}".format(testcase_key)
 
         try:
             return self.get_request(url)
         except exceptions.BadResponseError:
             raise exceptions.TestCaseNotFoundError(testcase_key)
 
-    def get_test_case_by_name(self, project_key: str, testcase_name: str, folder_path: str, partial_match: bool = False, *args, **kwargs):
+    def get_test_case_by_name(
+        self, project_key: str, testcase_name: str, folder_path: str, partial_match: bool = False, *args, **kwargs
+    ):
         """
         Gets a testcase from Zephyr
 
         :param testcase_name:
             name of the testcase (e.g. Application_test
         :param folder_path:
             folder path (e.g. Gtest/Master/bolognasc
         :param partial_match:
             match type (e.g. set partial_match to True for partially matching testcase name
         :return:
             testcases
         """
-        folder_path = folder_path.split('/')
-        parent_id = self.get_folder_id(project_key=project_key, folder_name=folder_path[0], parent_id=None,
-                           folder_type="TEST_CASE")
+        folder_path = folder_path.split("/")
+        parent_id = self.get_folder_id(
+            project_key=project_key, folder_name=folder_path[0], parent_id=None, folder_type="TEST_CASE"
+        )
         for folder_name in folder_path[1:]:
-            parent_id = self.get_folder_id(project_key=project_key, folder_name=folder_name, parent_id=parent_id, folder_type="TEST_CASE")
+            parent_id = self.get_folder_id(
+                project_key=project_key, folder_name=folder_name, parent_id=parent_id, folder_type="TEST_CASE"
+            )
 
         try:
             testcases = self.get_all_testcases(project_key=project_key, folder_id=parent_id)
             _testcases = []
             for testcase in testcases:
-                if not partial_match and testcase['name'] == testcase_name:
+                if not partial_match and testcase["name"] == testcase_name:
                     _testcases.append(testcase)
-                if partial_match and testcase_name in testcase['name']:
+                if partial_match and testcase_name in testcase["name"]:
                     _testcases.append(testcase)
             return _testcases
         except exceptions.BadResponseError:
             raise exceptions.TestCaseNotFoundError(testcase_name)
 
-
     def get_all_testcases(
         self, project_key: str = None, folder_id: int = None, timeout_s: float = 1.0, *args, **kwargs
     ):
         """
         Gets testcases from Zephyr
 
         :param project_key:
@@ -295,30 +299,28 @@
         :param folder_type:
            folder type : [TEST_CASE, TEST_CYCLE]
         :param parent_folder_path:
             id of the folder to create the test cycle in (optional)
         :return:
             response data from post command
         """
-        folder_path = parent_folder_path.split('/')
-        parent_id = self.get_folder_id(project_key=project_key, folder_name=folder_path[0], parent_id=None,
-                           folder_type="TEST_CASE")
+        folder_path = parent_folder_path.split("/")
+        parent_id = self.get_folder_id(
+            project_key=project_key, folder_name=folder_path[0], parent_id=None, folder_type="TEST_CASE"
+        )
         for folder_name in folder_path[1:]:
-            parent_id = self.get_folder_id(project_key=project_key, folder_name=folder_name, parent_id=parent_id, folder_type="TEST_CASE")
-        payload = {
-            "parentId": parent_id,
-            "name": folder_name,
-            "projectKey": project_key,
-            "folderType": folder_type
-        }
+            parent_id = self.get_folder_id(
+                project_key=project_key, folder_name=folder_name, parent_id=parent_id, folder_type="TEST_CASE"
+            )
+        payload = {"parentId": parent_id, "name": folder_name, "projectKey": project_key, "folderType": folder_type}
         url = self.base_url + "/folders"
         try:
             return self.post_request(url=url, payload=payload)
         except exceptions.BadResponseError:
-            raise exceptions.BadResponseError(f"Folder creation Failed")
+            raise exceptions.BadResponseError(f"Folder creation failed for new folder: {folder_name}.")
 
     def create_testcycle(self, project_key: str, name: str, descr: str = None, folder_id: int = None, *args, **kwargs):
         """
         Creates a new test cycle
 
         :param project_key:
             key of the project (e.g. BSBS)
@@ -607,39 +609,29 @@
             if locals().get(k) is not None:
                 payload[k] = locals().get(k)
             elif kwargs.get(k) is not None:
                 payload[k] = kwargs.get(k)
 
         self.put_request(url, payload)
 
+    def get_sorted_testexecutions_for_cycle(self, project_key: str, testcycle_key: str, *args, **kwargs):
+        """
+        Sorts test executions for a given test cycle by ActualEndDate
+        :param project_key:
+            Key of the zephyr project.
+        :param testcycle_key:
+            Key of the test cycle.
+        :return:
+            Test executions as a sorted data dictionary,
+             in ascending order from oldest to most recent
+        """
+        test_executions = self.get_test_executions(project_key=project_key, testcycle_key=testcycle_key, **kwargs)
+        sorted_executions = sorted(test_executions, key=lambda x: x["actualEndDate"], reverse=False)
+        return sorted_executions
+
 
 if __name__ == "__main__":
     with open("mytoken.txt", "r") as f:
         token = f.read()
 
     testmgmt = TestManagement(token)
-    data = testmgmt.get_test_case_by_name(folder_path="2.6.18_Diagnostics/2.6.18.2_DTCs", project_key='BMC', testcase_name="P", partial_match=True)
-    for tc in data:
-        print(tc['name'], tc['key'])
-    # print(testmgmt.create_testcase("BSBS", "Test", folder_name="SCS"))
-    # print(testmgmt.get_testcase("BSBS-T1"))
-    print(testmgmt.get_testcycle("BSBS-R18"))
-    myFolderId = testmgmt.get_folder_id(project_key="BMC", folder_name="Gtest")
-    myFolderId = testmgmt.get_folder_id(project_key="BMC", folder_name="bolognasc", parent_id=myFolderId)
-    myChildrenIds = testmgmt.get_children_folder_ids(folder_type="TEST_CASE", parent_id=myFolderId)
-    # for folderId in myChildrenIds:
-    #    print(testmgmt.get_all_testcases(project_key="BMC", folder_id=folderId))
-    # print(testmgmt.get_test_executions(project_key="BMC", testcycle_key="BMC-R362"))
-    tc = testmgmt.get_testcasekeys_from_cycle(project_key="BMC", testcycle_key="BMC-R362")
-    print(tc[0])
-    # print(testmgmt.create_testcycle("BSBS", "Test", descr="Test"))
-    # print(testmgmt.get_all_testcycles("BSBS"))
-    # print(testmgmt.get_environments("BSBS"))
-    # print(testmgmt.get_test_executions("BSBS", "BSBS-R3", "BSBS-T25"))
-    # test_exec = testmgmt.get_test_executions("BSBS", "BSBS-R3", "BSBS-T25")[0]
-    # print(testmgmt.get_status_by_id(test_exec["testExecutionStatus"]["id"]))
-    # print(testmgmt.post_test_execution("BSBS", "BSBS-T1", "BSBS-R3", TestVerdicts.PASS, comment="Test",
-    #                                    env_name="HIL_automated"))
-    # print(testmgmt.get_testcase_folder_id("BSBS", "SCS"))
-    # print(testmgmt.upload_results("0000dead_0000beef", "ffff", "BSBS-T1", TestVerdicts.PASS, 42, "logs/log.txt",
-    #                               "Test Passed."))
-
+    # room for some tests here
```

