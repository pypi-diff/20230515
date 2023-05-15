# Comparing `tmp/edwh_sshkey_plugin-0.1.3.tar.gz` & `tmp/edwh_sshkey_plugin-0.1.4.tar.gz`

## Comparing `edwh_sshkey_plugin-0.1.3.tar` & `edwh_sshkey_plugin-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/CHANGELOG.md
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/.idea/.gitignore
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/.idea/edwh-sshkey-plugin.iml
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/.idea/misc.xml
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/.idea/vcs.xml
--rw-r--r--   0        0        0     7884 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/.idea/workspace.xml
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/.idea/shelf/Uncommitted_changes_before_Update_at_12-05-2023_17_23__Changes_.xml
--rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/.idea/shelf/Uncommitted_changes_before_Update_at_12-05-2023_17_23_[Changes]/shelved.patch
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/pynguin-report/statistics.csv
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/src/edwh_sshkey_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/src/edwh_sshkey_plugin/__init__.py
--rw-r--r--   0        0        0    16473 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/src/edwh_sshkey_plugin/fabfile.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/LICENSE.txt
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/README.md
--rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3699 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.4/CHANGELOG.md
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.4/.idea/.gitignore
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.4/.idea/edwh-sshkey-plugin.iml
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.4/.idea/misc.xml
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.4/.idea/vcs.xml
+-rw-r--r--   0        0        0     9300 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.4/.idea/workspace.xml
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.4/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.4/.idea/shelf/Uncommitted_changes_before_Update_at_12-05-2023_17_23__Changes_.xml
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.4/.idea/shelf/Uncommitted_changes_before_Update_at_12-05-2023_17_23_[Changes]/shelved.patch
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.4/pynguin-report/statistics.csv
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.4/src/edwh_sshkey_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.4/src/edwh_sshkey_plugin/__init__.py
+-rw-r--r--   0        0        0    16622 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.4/src/edwh_sshkey_plugin/fabfile.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.4/LICENSE.txt
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.4/README.md
+-rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.4/PKG-INFO
```

### Comparing `edwh_sshkey_plugin-0.1.3/CHANGELOG.md` & `edwh_sshkey_plugin-0.1.4/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.1.4 (2023-05-15)
+### Fix
+* Error messages improvements and key generation gives more info with the keys ([`e82a53a`](https://github.com/educationwarehouse/edwh-sshkey-plugin/commit/e82a53a565a7cf1416b4794d10dfbf1eabd4288d))
+
 ## v0.1.3 (2023-05-15)
 ### Fix
 * Small docs fix ([`6655f04`](https://github.com/educationwarehouse/edwh-sshkey-plugin/commit/6655f045d5a773742de6b37f7df93497d05b3a71))
 * Removal of debug messages ([`4ef8861`](https://github.com/educationwarehouse/edwh-sshkey-plugin/commit/4ef8861d364041f11c3ec5598c40015400f7de24))
 * List shadow, -remote remote because of also being able to run local, show text if running local, showing key_names during listing keys, able to list private keys, bug where keys where the "keys: " was added per generation of an key ([`2c0fabd`](https://github.com/educationwarehouse/edwh-sshkey-plugin/commit/2c0fabdca2bab14ca1e206b08f967130d86ffa2b))
 * Local and remote are now somewhat separated + eod ([`a040491`](https://github.com/educationwarehouse/edwh-sshkey-plugin/commit/a0404917d3f6faad156e6a8b1605ca78babffa2a))
```

### Comparing `edwh_sshkey_plugin-0.1.3/.idea/workspace.xml` & `edwh_sshkey_plugin-0.1.4/.idea/workspace.xml`

 * *Files 12% similar despite different names*

#### Comparing `edwh_sshkey_plugin-0.1.3/.idea/workspace.xml` & `edwh_sshkey_plugin-0.1.4/.idea/workspace.xml`

```diff
@@ -1,23 +1,40 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="4efbc939-d6a7-49cf-b89a-2d2d13a65de6" name="Changes" comment="fix: small docs fix"/>
-    <list id="43fec3d4-1de5-4a40-814d-47bb24d48abf" name="Changes by romy" comment=""/>
+    <list default="true" id="4efbc939-d6a7-49cf-b89a-2d2d13a65de6" name="Changes" comment="fix: small docs fix">
+      <change beforePath="$PROJECT_DIR$/README.md" beforeDir="false" afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/edwh_sshkey_plugin/fabfile.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/edwh_sshkey_plugin/fabfile.py" afterDir="false"/>
+    </list>
+    <list id="43fec3d4-1de5-4a40-814d-47bb24d48abf" name="Changes by romy" comment="">
+      <change beforePath="$PROJECT_DIR$/src/edwh_sshkey_plugin/fabfile.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/edwh_sshkey_plugin/fabfile.py" afterDir="false"/>
+    </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="Git.Settings">
     <option name="RECENT_GIT_ROOT_PATH" value="$PROJECT_DIR$"/>
   </component>
+  <component name="LineStatusTrackerManager">
+    <file path="$PROJECT_DIR$/src/edwh_sshkey_plugin/fabfile.py">
+      <ranges>
+        <range start1="165" end1="165" start2="165" end2="166" changelist="4efbc939-d6a7-49cf-b89a-2d2d13a65de6"/>
+        <range start1="197" end1="198" start2="198" end2="199" changelist="4efbc939-d6a7-49cf-b89a-2d2d13a65de6"/>
+        <range start1="278" end1="279" start2="279" end2="280" changelist="43fec3d4-1de5-4a40-814d-47bb24d48abf"/>
+        <range start1="305" end1="305" start2="306" end2="309" changelist="4efbc939-d6a7-49cf-b89a-2d2d13a65de6"/>
+        <range start1="306" end1="307" start2="310" end2="312" changelist="4efbc939-d6a7-49cf-b89a-2d2d13a65de6"/>
+        <range start1="314" end1="316" start2="319" end2="321" changelist="43fec3d4-1de5-4a40-814d-47bb24d48abf"/>
+      </ranges>
+    </file>
+  </component>
   <component name="MarkdownSettingsMigration">
     <option name="stateVersion" value="1"/>
   </component>
   <component name="ProjectId" id="2PVDfjpOqXeVwXYp20fetsbIaGQ"/>
   <component name="ProjectLevelVcsManager" settingsEditedManually="true"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
@@ -58,15 +75,16 @@
       <workItem from="1683626467016" duration="2066000"/>
       <workItem from="1683635310950" duration="7083000"/>
       <workItem from="1683642479504" duration="42000"/>
       <workItem from="1683705297886" duration="244000"/>
       <workItem from="1683717762843" duration="1708000"/>
       <workItem from="1683721025404" duration="79000"/>
       <workItem from="1683894489773" duration="2855000"/>
-      <workItem from="1684137116604" duration="8222000"/>
+      <workItem from="1684137116604" duration="8256000"/>
+      <workItem from="1684149684048" duration="1317000"/>
     </task>
     <task id="LOCAL-00001" summary="fix: add_to_remote and delete_remote fixed so they actually add and remove the keys. they did nothing previously due to me not being able to test the functions from home :/">
       <created>1683553464389</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
       <updated>1683553464389</updated>
```

### Comparing `edwh_sshkey_plugin-0.1.3/.idea/inspectionProfiles/Project_Default.xml` & `edwh_sshkey_plugin-0.1.4/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `edwh_sshkey_plugin-0.1.3/.idea/shelf/Uncommitted_changes_before_Update_at_12-05-2023_17_23_[Changes]/shelved.patch` & `edwh_sshkey_plugin-0.1.4/.idea/shelf/Uncommitted_changes_before_Update_at_12-05-2023_17_23_[Changes]/shelved.patch`

 * *Files identical despite different names*

### Comparing `edwh_sshkey_plugin-0.1.3/src/edwh_sshkey_plugin/fabfile.py` & `edwh_sshkey_plugin-0.1.4/src/edwh_sshkey_plugin/fabfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,14 +159,15 @@
                 exit(1)
             key_split = new_key.split()
 
             if len(key_split) > 3:
                 print(
                     f"to many arguments given in the key: {which_key} format needs to be: owner-hostname-goal"
                 )
+                exit(1)
 
             # This is to create a new key, the split is to make sure that the key is in the right format.
             generate(
                 c,
                 generate_message,
                 owner=key_split[0],
                 hostname=key_split[1],
@@ -191,15 +192,15 @@
     There is a key called 'who@hostname', that's the person who created the new ssh key.
 
 
     If there are keys that are not in the YAML file, the user is prompted to create them.
     NOTE: you must provide a message, otherwise the program will terminate.
     """
     if local_connection(c):
-        if input("are you sure you want to add local keys(Y/n").replace(
+        if input("are you sure you want to add local keys(Y/n): ").replace(
             " ", ""
         ) not in ["Y", "y", ""]:
             print("please use `edwh -H ubuntu@user.nl sshkey.add because ")
             exit(255)
         else:
             print("Adding keys to local known_hosts")
 
@@ -272,15 +273,15 @@
 )
 def generate(c, message, owner="", hostname="", goal=""):
     """
     This function generates a new SSH key and saves it to a yaml file. (~/.ssh/known_keys.yaml)
 
     You need a message and 2 out of 3 arguments to generate a new key. (owner, hostname, goal) Otherwise it will fail.
 
-    The private/public key is located local in the ~/.managed_ssh_keys-{key_name} directory.
+    The private and public key is located local in the ~/.managed_ssh_keys-{key_name} directory.
     You can see who has the private/public key, by looking at the YAML file.
     There is a key called 'who@hostname', that's the person who created the new ssh key.
     """
     # Get the yaml keys or create a new YAML file if it does not already exist
     keys_dict = {"keys": {}}
     current_keys = get_keys_from_keyholder(gen=True)
 
@@ -299,25 +300,29 @@
         return
 
     # Run the ssh-keygen command to generate a new SSH key
     # As type of key we use rsa, with a bit size of 4096
     # The key is saved in ~/.ssh/.managed_ssh_keys-{key_name}
     # The key has no passphrase
     # The key has given a comment with the message
+    curr_time = datetime.now().strftime("Datum: %Y-%m-%d Tijdstip: %H:%M:%S")
+    host = f"{os.getlogin()}@{platform.node()}"
+
     subprocess.run(
-        f'ssh-keygen -t rsa -b 4096 -f ~/.ssh/.managed_ssh_keys-{key_name} -N "" -C "{message}"',
+        f'ssh-keygen -t rsa -b 4096 -f ~/.ssh/.managed_ssh_keys-{key_name} -N "" -C "key name: {key_name} '
+        f'message: {message} who@hostname: {host} {curr_time}"',
         shell=True,
     )
     keys_dict["keys"].update(current_keys)
     keys_dict["keys"][key_name] = {
         "key": open(
             pathlib.Path(f"~/.ssh/.managed_ssh_keys-{key_name}.pub").expanduser()
         ).read(),
-        "datetime": datetime.now().strftime("Datum: %Y-%m-%d Tijdstip: %H:%M:%S"),
-        "who@hostname": f"{os.getlogin()}@{platform.node()}",
+        "datetime": curr_time,
+        "who@hostname": host,
         "message": message,
     }
 
     # Open the YAML_KEYS_PATH file in append mode
     with open(YAML_KEYS_PATH, "w") as f:
         # Dump the key information to the YAML file
         yaml.dump(
```

### Comparing `edwh_sshkey_plugin-0.1.3/tests/__init__.py` & `edwh_sshkey_plugin-0.1.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `edwh_sshkey_plugin-0.1.3/LICENSE.txt` & `edwh_sshkey_plugin-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_sshkey_plugin-0.1.3/README.md` & `edwh_sshkey_plugin-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# edwh-demo-plugin
+# edwh-sshkey-plugin
 
 [![PyPI - Version](https://img.shields.io/pypi/v/edwh-demo-plugin.svg)](https://pypi.org/project/edwh-demo-plugin)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/edwh-demo-plugin.svg)](https://pypi.org/project/edwh-demo-plugin)
 
 -----
 
 **Table of Contents**
```

### Comparing `edwh_sshkey_plugin-0.1.3/pyproject.toml` & `edwh_sshkey_plugin-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_sshkey_plugin-0.1.3/PKG-INFO` & `edwh_sshkey_plugin-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-sshkey-plugin
-Version: 0.1.3
+Version: 0.1.4
 Summary: plugin for adding and removing keys to servers
 Project-URL: Documentation, https://github.com/remcoboerma/edwh_sshkey_plugin#readme
 Project-URL: Issues, https://github.com/remcoboerma/edwh_sshkey_plugin/issues
 Project-URL: Source, https://github.com/remcoboerma/edwh_sshkey_plugin
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Sven Keimpema <sven.k@educationwarehouse.nl>, Romy Schöller <romy.s@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: invoke
 Description-Content-Type: text/markdown
 
-# edwh-demo-plugin
+# edwh-sshkey-plugin
 
 [![PyPI - Version](https://img.shields.io/pypi/v/edwh-demo-plugin.svg)](https://pypi.org/project/edwh-demo-plugin)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/edwh-demo-plugin.svg)](https://pypi.org/project/edwh-demo-plugin)
 
 -----
 
 **Table of Contents**
```

