# Comparing `tmp/edwh_sshkey_plugin-0.1.2.tar.gz` & `tmp/edwh_sshkey_plugin-0.1.3.tar.gz`

## Comparing `edwh_sshkey_plugin-0.1.2.tar` & `edwh_sshkey_plugin-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,19 @@
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.2/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.2/config.toml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.2/.idea/.gitignore
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.2/.idea/edwh-sshkey-plugin.iml
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.2/.idea/misc.xml
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.2/.idea/vcs.xml
--rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.2/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.2/src/edwh_sshkey_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.2/src/edwh_sshkey_plugin/__init__.py
--rw-r--r--   0        0        0    14695 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.2/src/edwh_sshkey_plugin/fabfile.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.2/README.md
--rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/CHANGELOG.md
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/.idea/.gitignore
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/.idea/edwh-sshkey-plugin.iml
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/.idea/misc.xml
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/.idea/vcs.xml
+-rw-r--r--   0        0        0     7884 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/.idea/workspace.xml
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/.idea/shelf/Uncommitted_changes_before_Update_at_12-05-2023_17_23__Changes_.xml
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/.idea/shelf/Uncommitted_changes_before_Update_at_12-05-2023_17_23_[Changes]/shelved.patch
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/pynguin-report/statistics.csv
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/src/edwh_sshkey_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/src/edwh_sshkey_plugin/__init__.py
+-rw-r--r--   0        0        0    16473 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/src/edwh_sshkey_plugin/fabfile.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/LICENSE.txt
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/README.md
+-rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3699 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.3/PKG-INFO
```

### Comparing `edwh_sshkey_plugin-0.1.2/CHANGELOG.md` & `edwh_sshkey_plugin-0.1.3/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.1.3 (2023-05-15)
+### Fix
+* Small docs fix ([`6655f04`](https://github.com/educationwarehouse/edwh-sshkey-plugin/commit/6655f045d5a773742de6b37f7df93497d05b3a71))
+* Removal of debug messages ([`4ef8861`](https://github.com/educationwarehouse/edwh-sshkey-plugin/commit/4ef8861d364041f11c3ec5598c40015400f7de24))
+* List shadow, -remote remote because of also being able to run local, show text if running local, showing key_names during listing keys, able to list private keys, bug where keys where the "keys: " was added per generation of an key ([`2c0fabd`](https://github.com/educationwarehouse/edwh-sshkey-plugin/commit/2c0fabdca2bab14ca1e206b08f967130d86ffa2b))
+* Local and remote are now somewhat separated + eod ([`a040491`](https://github.com/educationwarehouse/edwh-sshkey-plugin/commit/a0404917d3f6faad156e6a8b1605ca78babffa2a))
+
 ## v0.1.2 (2023-05-12)
 ### Fix
 * Prevents an error on list of an empty key file. ([`6369365`](https://github.com/educationwarehouse/edwh-sshkey-plugin/commit/6369365def512e55c7cc1eba43940d6bea840fef))
 
 ## v0.1.1 (2023-05-12)
 ### Fix
 * Some small docs changes ([`94445e2`](https://github.com/educationwarehouse/edwh-sshkey-plugin/commit/94445e2968148e18eaddd14506e8eb1c0b7bd6e9))
```

### Comparing `edwh_sshkey_plugin-0.1.2/src/edwh_sshkey_plugin/fabfile.py` & `edwh_sshkey_plugin-0.1.3/src/edwh_sshkey_plugin/fabfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,26 @@
+import fabric.connection
+import invoke
 from fabric import task
 from datetime import datetime
 from yaml.loader import SafeLoader
 import pathlib
 import yaml
 import os
 import subprocess
 import platform
 
 # the path where the yaml file with the keys is stored
 YAML_KEYS_PATH = pathlib.Path("~/.ssh/known_keys.yaml").expanduser()
 
 
+def local_connection(c):
+    return "invoke" in str(type(c))
+
+
 def create_new_yaml_file_if_not_exists():
     """
     Checks if the yaml file exists, if not it will create a new one.
     """
     if not YAML_KEYS_PATH.exists():
         YAML_KEYS_PATH.touch()
 
@@ -23,34 +29,38 @@
     """
     To open the yaml file, this function will be called.
     """
     create_new_yaml_file_if_not_exists()
     return YAML_KEYS_PATH.open("r" if read else "w")
 
 
-def get_keys_from_keyholder() -> dict:
+def get_keys_from_keyholder(gen=False) -> dict:
     """
     This function retrieves keys from a keyholder.
 
     The function first opens a new keyholder and loads its contents as a dictionary using the yaml library.
     If the keyholder is empty, the function prints an error message and exits with code 255.
     Otherwise, it returns a dictionary of keys from the keyholder.
 
     :return: A dictionary of keys from the keyholder.
     """
     # It opens the keyholder and loads its contents as a dictionary using the yaml library.
     key_holder = open_new_keyholder(True)
     key_db: dict = yaml.load(key_holder, Loader=SafeLoader)
     # This checks if the keyholder is empty. If empty -> exit with code 255
     if key_db is None:
+        if gen:
+            return {}
+
         print(
             "functionality for generating local keys automaticly and adding them to the keyholder currently isn't supported"
         )
         print("please run `ew sshkey.generate` to generate a new key")
         exit(255)
+
     # This returns a dictionary of keys from the keyholder.
     return dict(key_db.setdefault("keys"))
 
 
 def get_key_count(keys, command_line_key):
     """
     This function takes in two arguments: a list of keys and a command line key. It returns the number of times the keys appear in the command line key.
@@ -80,15 +90,18 @@
     # If the user enters a key that isn't in the YAML file, it will break out of the loop.
     for command_line_key in command_line_keys:
         if command_line_key not in all_key_information:
             break
 
         all_key_information_remote_items = all_key_information[command_line_key]
 
-        if all(attr in all_key_information_remote_items for attr in ("key", "datetime", "who@hostname", "message")):
+        if all(
+            attr in all_key_information_remote_items
+            for attr in ("key", "datetime", "who@hostname", "message")
+        ):
             # It puts the keys in the authorized_keys file on the remote server.
             # So the public key is now on the remote server.
             # This means that the user can now log in to the remote server using the private key.
             c.run(
                 f'echo "{all_key_information_remote_items["key"]}" >> ~/.ssh/authorized_keys'
             )
             # This is a way to check if the key is already in the authorized_keys file.
@@ -121,15 +134,17 @@
         f'Wrong \033[1m{" ".join(not_in_yaml_keys)}\033[0m key, '
         f"first check if you filled in the right key. Or if it is in the YAML file."
     )
     # Here is the '-' replaced with a space, so it can be used in the generate function.
     # The generate function requires two out of three arguments to be filled in. So that's why the key is split.
     for which_key in not_in_yaml_keys:
         if "-" not in which_key:
-            print(f"\033[1m{which_key}\033[0m isn't a valid host-name please give it up with the format: owner-hostname-goal")
+            print(
+                f"\033[1m{which_key}\033[0m isn't a valid host-name please give it up with the format: owner-hostname-goal"
+            )
             continue
 
         new_key = which_key.replace("-", " ")
 
         # Create the key that isn't in the YAML file.
         if input(f"Do you want to create {which_key}? [Y/n]: ").replace(" ", "") in (
             "y",
@@ -141,46 +156,57 @@
             )
             if not generate_message:
                 print("Please give up a message for the next time!")
                 exit(1)
             key_split = new_key.split()
 
             if len(key_split) > 3:
-                print(f"to many arguments given in the key: {which_key} format needs to be: owner-hostname-goal")
+                print(
+                    f"to many arguments given in the key: {which_key} format needs to be: owner-hostname-goal"
+                )
 
             # This is to create a new key, the split is to make sure that the key is in the right format.
             generate(
                 c,
                 generate_message,
                 owner=key_split[0],
                 hostname=key_split[1],
                 goal=new_key.split()[2] if len(key_split) == 3 else "",
             )
             # eventually it will add the keys that are just created
-            add_to_remote(c, command_line_keys)
+            add(c, command_line_keys)
 
 
 @task(
     help={
         "keys-to-remote": "list of keys you want to add to the remote server",
     },
     iterable=["keys_to_remote"],
 )
-def add_to_remote(c, keys_to_remote: list):
+def add(c, keys_to_remote: list):
     """
     Adds the specified SSH key(s) to the remote machine. You can add multiple keys at once.
 
     The private/public key is located local in the ~/.managed_ssh_keys-{key_name} directory.
     You can see who has the private/public key, by looking at the YAML file.
     There is a key called 'who@hostname', that's the person who created the new ssh key.
 
 
     If there are keys that are not in the YAML file, the user is prompted to create them.
     NOTE: you must provide a message, otherwise the program will terminate.
     """
+    if local_connection(c):
+        if input("are you sure you want to add local keys(Y/n").replace(
+            " ", ""
+        ) not in ["Y", "y", ""]:
+            print("please use `edwh -H ubuntu@user.nl sshkey.add because ")
+            exit(255)
+        else:
+            print("Adding keys to local known_hosts")
+
     # If keys_to_remote is a string, convert it to a list with a single element
     if type(keys_to_remote) == str:
         keys_to_remote = [keys_to_remote]
 
     # check which keys are already in the YAML file
     all_key_information = get_keys_from_keyholder()
 
@@ -195,18 +221,27 @@
 
 @task(
     help={
         "keys_to_remote": "list of keys you want to remove from the server",
     },
     iterable=["keys_to_remote"],
 )
-def delete_remote(c, keys_to_remote):
+def delete(c, keys_to_remote):
     """
     Removes the specified SSH key(s) from the remote machine. You can remove multiple keys at once.
     """
+    if local_connection(c):
+        if input("are you sure you want to add local keys(Y/n").replace(
+            " ", ""
+        ) not in ["Y", "y", ""]:
+            print("please use `edwh -H ubuntu@user.nl sshkey.delete to remove remote keys ")
+            exit(255)
+        else:
+            print("Removing local keys from known_hosts")
+
     # If keys_to_remote is a string, convert it to a list with a single element
     if isinstance(keys_to_remote, str):
         keys_to_remote = [keys_to_remote]
 
     # Get all key information from the keyholder
     all_key_information = get_keys_from_keyholder()
 
@@ -219,41 +254,44 @@
         # Get the SSH key from all_key_information and remove newlines
         ssh_key = all_key_information[command_line_key]["key"].strip()
         # Remove the key from the remote server's authorized_keys file
         c.run(f'grep -v "{ssh_key}" ~/.ssh/authorized_keys > ~/.ssh/keys')
         c.run("mv ~/.ssh/keys ~/.ssh/authorized_keys")
         # Print a success message
         print(f"Success! The {command_line_key} key has been removed.")
+    else:
+        print("please give up keys using edwh.sshkey.delete -k [keys]")
 
 
 @task(
     help={
         "message": "a message to know what the key is used for, REQUIRED",
         "owner": "owner of the server you are generating a key for",
         "hostname": "hostname of the server you are generating the key for",
-        "goal": "What is the goal to use this key for, for example: 'production' or 'testing''",
+        "goal": "What is the goal to use this key for, for example: 'production' or 'testing'",
     }
 )
 def generate(c, message, owner="", hostname="", goal=""):
     """
     This function generates a new SSH key and saves it to a yaml file. (~/.ssh/known_keys.yaml)
 
     You need a message and 2 out of 3 arguments to generate a new key. (owner, hostname, goal) Otherwise it will fail.
 
     The private/public key is located local in the ~/.managed_ssh_keys-{key_name} directory.
     You can see who has the private/public key, by looking at the YAML file.
     There is a key called 'who@hostname', that's the person who created the new ssh key.
     """
-    # Create a new YAML file if it does not already exist
-    create_new_yaml_file_if_not_exists()
+    # Get the yaml keys or create a new YAML file if it does not already exist
+    keys_dict = {"keys": {}}
+    current_keys = get_keys_from_keyholder(gen=True)
 
     # Create a key name by joining the non-empty values of owner, hostname, and goal with a hyphen
     key_name = "-".join(_ for _ in (owner, hostname, goal) if _)
     # If less than two of three from owner, hostname, and goal are provided, print an error message and return
-    if '-' in key_name:
+    if "-" not in key_name:
         print(
             "Please provide at least two of the following arguments: Owner, Hostname, goal"
         )
         return
 
     # If a file with the specified key name already exists, print an error message and return
     if pathlib.Path(f"~/.managed_ssh_keys-{key_name}").expanduser().exists():
@@ -265,68 +303,85 @@
     # The key is saved in ~/.ssh/.managed_ssh_keys-{key_name}
     # The key has no passphrase
     # The key has given a comment with the message
     subprocess.run(
         f'ssh-keygen -t rsa -b 4096 -f ~/.ssh/.managed_ssh_keys-{key_name} -N "" -C "{message}"',
         shell=True,
     )
+    keys_dict["keys"].update(current_keys)
+    keys_dict["keys"][key_name] = {
+        "key": open(
+            pathlib.Path(f"~/.ssh/.managed_ssh_keys-{key_name}.pub").expanduser()
+        ).read(),
+        "datetime": datetime.now().strftime("Datum: %Y-%m-%d Tijdstip: %H:%M:%S"),
+        "who@hostname": f"{os.getlogin()}@{platform.node()}",
+        "message": message,
+    }
 
     # Open the YAML_KEYS_PATH file in append mode
-    with open(YAML_KEYS_PATH, "a") as f:
+    with open(YAML_KEYS_PATH, "w") as f:
         # Dump the key information to the YAML file
         yaml.dump(
-            {
-                "keys": {
-                    key_name: {
-                        "key": open(
-                            pathlib.Path(
-                                f"~/.ssh/.managed_ssh_keys-{key_name}.pub"
-                            ).expanduser()
-                        ).read(),
-                        "datetime": datetime.today().strftime(
-                            "Datum: %Y-%m-%d Tijdstip: %H:%M:%S"
-                        ),
-                        "who@hostname": f"{os.getlogin()}@{platform.node()}",
-                        "message": message,
-                    }
-                }
-            },
+            keys_dict,
             f,
             indent=4,
         )
     # Print a success message
     print(f"Public key saved in ~/.managed_ssh_keys-{key_name}.pub")
     print(f"Private key saved in ~/.managed_ssh_keys-{key_name}")
 
 
-@task()
-def list(c):
+def get_keys(c, private):
+    if not private:
+        return get_keys_from_keyholder()
+
+    key_names = get_keys_from_keyholder()
+    keys = {}
+    for key_name in key_names:
+        # we should only be able to find 1 key
+        private_key_file = pathlib.Path(f"~/.ssh/.managed_ssh_keys-{key_name}").expanduser()
+
+        if private_key_file is None:
+            print(f"[ERROR] private key for {key_name} not found!")
+            print("exiting....")
+            exit(1)
+
+            # reinact yaml file so we don't need to parse this differently
+        keys[key_name] = {"key": private_key_file.read_text()}
+    return keys
+
+
+@task(name="list")
+def list_(c, private=False):
     """
     Lists all the local or local and remote ssh_keys.
     This function lists the authorized keys on a remote machine and compares them with the keys in a local YAML file.
     It separates the keys into three categories: local keys, remote known keys, and unrecognized keys.
     """
     # Load the keys from the YAML file
-    all_key_information = get_keys_from_keyholder()
+    all_key_information = get_keys(c, private)
 
     # Get the list of authorized keys from the remote machine
     if len(c.run("ls ~/.ssh/authorized_keys", warn=True, hide=True).stdout) > 0:
         remote_keys = c.run("cat ~/.ssh/authorized_keys", hide=True).stdout
     else:
         remote_keys = ""
 
     # Iterate through the keys and separate them into two lists
+    key_names = {}
     local_keys = []
     remote_known_keys = []
-    for key_data in all_key_information.values():
+    for key in all_key_information.keys():
+        key_data = all_key_information[key]
         if key_data["key"] in remote_keys:
             remote_known_keys.append(key_data["key"].replace("\n", ""))
         else:
             local_keys.append(key_data["key"])
 
+        key_names[key_data["key"]] = key
     remote_keys = remote_keys.split("\n")
 
     # Check for any unrecognized keys in the authorized_keys file
     if len(c.run("ls ~/.ssh/authorized_keys", warn=True, hide=True).stdout) > 0:
         unrecognized_keys = [
             remote_key
             for remote_key in remote_keys
@@ -344,18 +399,22 @@
             print(f"key {index+1}")
             print(unrecognized_keys[index])
             print()
         print()
 
     # Display the keys in a table
     if local_keys or remote_known_keys:
-        if local_keys:
+        if local_keys and local_connection(c):
             print("\033[1mLocal Keys\033[0m")
             for key in local_keys:
+                print(f"Key {key_names[key]}:")
                 print(f"\033[33m{key}\033[0m")
 
         if remote_known_keys:
             print("\033[1mRemote Keys\033[0m")
             for key in remote_known_keys:
+                print(f"Key {key_names[key]}:")
                 print(f"\033[33m{key}\033[0m")
+        elif not local_connection(c):
+            print("\033[1mNo remote keys have been found!\033[0m")
     else:
         print("No keys found in key_holder.yaml")
```

### Comparing `edwh_sshkey_plugin-0.1.2/tests/__init__.py` & `edwh_sshkey_plugin-0.1.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `edwh_sshkey_plugin-0.1.2/LICENSE.txt` & `edwh_sshkey_plugin-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_sshkey_plugin-0.1.2/README.md` & `edwh_sshkey_plugin-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -26,17 +26,17 @@
 example for ubuntu@user.nl
 ```console
 edwh sshkey.generate --message={message} --owner=ubuntu --hostname=user --doel=nl
 ```
 
 possible arguments for `ew sshkey.generate`:
 - **message**: REQUIRED, message to give with the ssh-keygen
-- **owner**: ubuntu if ubuntu@user.nl
-- **hostname**: user if ubuntu@user.nl
-- **goal**: nl if ubuntu@user.nl
+- **owner**: owner of the server you are generating a key for
+- **hostname**: hostname of the server you are generating the key for
+- **goal**: What is the goal to use this key for, for example: 'production' or 'testing'
 
 #### note:
 you atleast need to give this function 2-3 parameters and a message else it will not work.
 
 ### Adding keys to remote
 example for ubuntu@user.nl
 ```console
```

### Comparing `edwh_sshkey_plugin-0.1.2/pyproject.toml` & `edwh_sshkey_plugin-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_sshkey_plugin-0.1.2/PKG-INFO` & `edwh_sshkey_plugin-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-sshkey-plugin
-Version: 0.1.2
+Version: 0.1.3
 Summary: plugin for adding and removing keys to servers
 Project-URL: Documentation, https://github.com/remcoboerma/edwh_sshkey_plugin#readme
 Project-URL: Issues, https://github.com/remcoboerma/edwh_sshkey_plugin/issues
 Project-URL: Source, https://github.com/remcoboerma/edwh_sshkey_plugin
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Sven Keimpema <sven.k@educationwarehouse.nl>, Romy Schöller <romy.s@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -46,17 +46,17 @@
 example for ubuntu@user.nl
 ```console
 edwh sshkey.generate --message={message} --owner=ubuntu --hostname=user --doel=nl
 ```
 
 possible arguments for `ew sshkey.generate`:
 - **message**: REQUIRED, message to give with the ssh-keygen
-- **owner**: ubuntu if ubuntu@user.nl
-- **hostname**: user if ubuntu@user.nl
-- **goal**: nl if ubuntu@user.nl
+- **owner**: owner of the server you are generating a key for
+- **hostname**: hostname of the server you are generating the key for
+- **goal**: What is the goal to use this key for, for example: 'production' or 'testing'
 
 #### note:
 you atleast need to give this function 2-3 parameters and a message else it will not work.
 
 ### Adding keys to remote
 example for ubuntu@user.nl
 ```console
```

