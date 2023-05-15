# Comparing `tmp/desktop-entry-lib-3.0.tar.gz` & `tmp/desktop-entry-lib-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desktop-entry-lib-3.0.tar", last modified: Fri Feb  3 15:44:20 2023, max compression
+gzip compressed data, was "desktop-entry-lib-3.1.tar", last modified: Mon May 15 10:06:53 2023, max compression
```

## Comparing `desktop-entry-lib-3.0.tar` & `desktop-entry-lib-3.1.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 15:44:20.899897 desktop-entry-lib-3.0/
--rw-r--r--   0 root         (0) root         (0)     1318 2023-02-03 15:43:49.000000 desktop-entry-lib-3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       70 2023-02-03 15:43:49.000000 desktop-entry-lib-3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3037 2023-02-03 15:44:20.899897 desktop-entry-lib-3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1729 2023-02-03 15:43:49.000000 desktop-entry-lib-3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 15:44:20.899897 desktop-entry-lib-3.0/desktop_entry_lib/
--rw-r--r--   0 root         (0) root         (0)    27933 2023-02-03 15:43:49.000000 desktop-entry-lib-3.0/desktop_entry_lib/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-03 15:43:49.000000 desktop-entry-lib-3.0/desktop_entry_lib/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 15:44:20.899897 desktop-entry-lib-3.0/desktop_entry_lib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3037 2023-02-03 15:44:20.000000 desktop-entry-lib-3.0/desktop_entry_lib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      265 2023-02-03 15:44:20.000000 desktop-entry-lib-3.0/desktop_entry_lib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-03 15:44:20.000000 desktop-entry-lib-3.0/desktop_entry_lib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-02-03 15:44:20.000000 desktop-entry-lib-3.0/desktop_entry_lib.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1494 2023-02-03 15:43:49.000000 desktop-entry-lib-3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-03 15:44:20.899897 desktop-entry-lib-3.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:06:53.699613 desktop-entry-lib-3.1/
+-rw-r--r--   0 root         (0) root         (0)     1318 2023-05-15 10:06:05.000000 desktop-entry-lib-3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       70 2023-05-15 10:06:05.000000 desktop-entry-lib-3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3037 2023-05-15 10:06:53.699613 desktop-entry-lib-3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-05-15 10:06:05.000000 desktop-entry-lib-3.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:06:53.699613 desktop-entry-lib-3.1/desktop_entry_lib/
+-rw-r--r--   0 root         (0) root         (0)    30767 2023-05-15 10:06:05.000000 desktop-entry-lib-3.1/desktop_entry_lib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 10:06:05.000000 desktop-entry-lib-3.1/desktop_entry_lib/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:06:53.699613 desktop-entry-lib-3.1/desktop_entry_lib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3037 2023-05-15 10:06:53.000000 desktop-entry-lib-3.1/desktop_entry_lib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      353 2023-05-15 10:06:53.000000 desktop-entry-lib-3.1/desktop_entry_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 10:06:53.000000 desktop-entry-lib-3.1/desktop_entry_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-15 10:06:53.000000 desktop-entry-lib-3.1/desktop_entry_lib.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1494 2023-05-15 10:06:05.000000 desktop-entry-lib-3.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 10:06:53.699613 desktop-entry-lib-3.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 10:06:53.699613 desktop-entry-lib-3.1/tests/
+-rw-r--r--   0 root         (0) root         (0)     4189 2023-05-15 10:06:05.000000 desktop-entry-lib-3.1/tests/test_collection.py
+-rw-r--r--   0 root         (0) root         (0)     4922 2023-05-15 10:06:05.000000 desktop-entry-lib-3.1/tests/test_data.py
+-rw-r--r--   0 root         (0) root         (0)     2977 2023-05-15 10:06:05.000000 desktop-entry-lib-3.1/tests/test_entry.py
+-rw-r--r--   0 root         (0) root         (0)     2649 2023-05-15 10:06:05.000000 desktop-entry-lib-3.1/tests/test_functions.py
```

### Comparing `desktop-entry-lib-3.0/LICENSE` & `desktop-entry-lib-3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `desktop-entry-lib-3.0/PKG-INFO` & `desktop-entry-lib-3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: desktop-entry-lib
-Version: 3.0
+Version: 3.1
 Summary: A library for working with .desktop files
 Author-email: JakobDev <jakobdev@gmx.de>
 License: BSD-2-Clause
 Project-URL: Source, https://codeberg.org/JakobDev/desktop-entry-lib
 Project-URL: Issues, https://codeberg.org/JakobDev/desktop-entry-lib/issues
 Project-URL: Documentation, https://desktop-entry-lib.readthedocs.io
 Project-URL: Donation, https://ko-fi.com/jakobdev
```

### Comparing `desktop-entry-lib-3.0/README.md` & `desktop-entry-lib-3.1/README.md`

 * *Files identical despite different names*

### Comparing `desktop-entry-lib-3.0/desktop_entry_lib/__init__.py` & `desktop-entry-lib-3.1/desktop_entry_lib/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,40 +2,53 @@
 import subprocess
 import tempfile
 import locale
 import os
 import re
 
 
-__version__ = "3.0"
+__version__ = "3.1"
 "The version"
 
 
+def _assert_func(expression: bool) -> None:
+    """
+    The assert keyword is not available when running Python in Optimized Mode.
+    This function is a drop-in replacement.
+    See https://docs.python.org/3/using/cmdline.html?highlight=pythonoptimize#cmdoption-O
+    """
+    if not expression:
+        raise AssertionError()
+
+
 def _compare_dict(first_dict: dict, second_dict: dict) -> bool:
+    "Compare 2 dicts"
     if len(first_dict) != len(second_dict):
         return False
 
     for key, value in first_dict.items():
         if key not in second_dict:
             return False
 
         if value != second_dict[key]:
             return False
 
     return True
 
 
 def _strip_list(old_list: list[str]) -> list[str]:
+    "Run .strip() on all Elements of a list"
     new_list = []
     for i in old_list:
         new_list.append(i.strip())
     return new_list
 
 
 def _parse_desktop_sections(content: str) -> dict[str, dict[str, str]]:
+    "Parses a .desktop file"
     sections: dict[str, dict[str, str]] = {}
     current_section = None
     for line in content.splitlines():
         if line.startswith("[") and line.endswith("]"):
             current_section = line[1:-1]
             sections[current_section] = {}
         elif current_section is None:
@@ -58,20 +71,24 @@
     elif string.lower() == "false":
         return False
     else:
         return None
 
 
 def _is_flatpak() -> bool:
-    "Cheks if the lib is running inside a Flatpak"
+    "Checks if the lib is running inside a Flatpak"
     return os.path.isfile("/.flatpak-info")
 
 
 def get_xdg_data_dirs() -> list[str]:
-    "Get all XDG DATA DIRS"
+    """
+    Get all XDG DATA DIRS
+
+    :return: The list of XDG data Dirs
+    """
     try:
         data_dirs = os.getenv("XDG_DATA_DIRS").removesuffix(":").split(":")
     except AttributeError:
         data_dirs = [os.path.expanduser("~/.local/share"), "/usr/share"]
 
     if _is_flatpak():
         return data_dirs + ["/run/host/usr/share"]
@@ -93,15 +110,20 @@
     for size in size_list:
         dir_list.append(f"{size}x{size}")
 
     return dir_list
 
 
 def get_icon_path(icon_name: str) -> Optional[str]:
-    "Get the path of a Icon"
+    """
+    Get the path of a Icon
+
+    :param icon_name: The name of the Icon as found in the desktop entry
+    :return: The full pßath to the Icon. none if the Icon was not found.
+    """
     for data_dir in get_xdg_data_dirs():
         scalable_dir = os.path.join(data_dir, "icons", "hicolor", "scalable")
         if os.path.isdir(scalable_dir):
             for directory in os.listdir(scalable_dir):
                 icon_path = os.path.join(scalable_dir, directory, icon_name + ".svg")
                 if os.path.isfile(icon_path):
                     return icon_path
@@ -116,20 +138,30 @@
             if os.path.isfile(os.path.join(data_dir, "pixmaps", icon_name + ".png")):
                 return os.path.join(data_dir, "pixmaps", icon_name + ".png")
 
     return None
 
 
 def is_action_identifier_valid(identifier: str) -> bool:
-    "Checks if a Action identifier is valid"
+    """
+    Checks if a Action identifier is valid
+
+    :param identifier: The Identifier
+    :return: If the identifier is valid
+    """
     return re.match("^([0-9]|[a-z]|[A-Z]|-)+$", identifier) is not None
 
 
 def is_custom_key_name_valid(name: str) -> bool:
-    "Checks if the given name can be used for a custom key"
+    """
+    Checks if the given name can be used for a custom key
+
+    :param identifier: The name
+    :return: If the name can be used
+    """
     return re.match(r"^X-([0-9]|[a-z]|[A-Z]|-)+(\[([0-9]|[a-z]|[A-Z]|-)+\])?$", name) is not None
 
 
 class ValidationMessageDict(TypedDict):
     "Defines the return type for get_validation_messages()"
     Error: list[str]
     FutureError: list[str]
@@ -149,15 +181,19 @@
         self.default_text: str = ""
         "The untranslated text"
 
         self.translations: dict[str, str] = {}
         "The translations"
 
     def get_translated_text(self) -> str:
-        "Returns the text for the current language"
+        """
+        Returns the text for the current system language
+
+        :return: The text
+        """
         current_lang = locale.getlocale()[0]
         if current_lang is None:
             return self.default_text
         elif current_lang in self.translations:
             return self.translations[current_lang]
         elif current_lang.split("_")[0] in self.translations:
             return self.translations[current_lang.split("_")[0]]
@@ -209,15 +245,18 @@
         return self.default_text == obj.default_text and _compare_dict(self.translations, obj.translations)
 
 
 class TranslatableListKey:
     "Represents a List in a Desktop Entry, that can be translated into different languages"
     def __init__(self) -> None:
         self.default_list: list[str] = []
+        "The unstranslated list"
+
         self.translations: dict[str, list[str]] = {}
+        "The translated lists"
 
     def load_section(self, section: dict[str, str], search_key: str) -> None:
         "Loads a section from a Desktop Entry. Only for internal use."
         self.clear()
 
         for key, value in section.items():
             if not key.startswith(search_key):
@@ -289,15 +328,19 @@
 
         if self.Exec is not None:
             text += f"Exec={self.Exec}"
 
         return text
 
     def get_icon_path(self) -> Optional[str]:
-        "Returns the full path to the Icon"
+        """
+        Returns full Path to the Icon
+
+        :return: The full Path or None, if the Icon can't be found
+        """
         if self.Icon is None:
             return None
         else:
             return get_icon_path(self.Icon)
 
     def __eq__(self, obj: object) -> bool:
         if not isinstance(obj, DesktopAction):
@@ -404,19 +447,27 @@
             os.close(file_handle)
             self.write_file(temp_path)
             return subprocess.run(["desktop-file-validate", temp_path], capture_output=True)
         finally:
             os.remove(temp_path)
 
     def is_valid(self) -> bool:
-        "Returns, if the Desktop Entry is valid. desktop-file-validate needs to be installed."
+        """
+        Returns, if the Desktop Entry is valid. desktop-file-validate needs to be installed.
+
+        :return: If the entry is valid
+        """
         return self._execute_validate_command().returncode == 0
 
     def get_validation_messages(self) -> ValidationMessageDict:
-        "Returns all messages from desktop-file-validate"
+        """
+        Returns all messages from desktop-file-validate
+
+        :return: A dict which contains the validation messages
+        """
         message_dict: ValidationMessageDict = {"Error": [], "FutureError": [], "Warning": [], "Hint": []}
         for i in self._execute_validate_command().stdout.decode("utf-8").splitlines():
             file_name, message_type, message = _strip_list(i.split(":", 2))
             if message_type == "error":
                 if message.startswith("(will be fatal in the future): "):
                     message_dict["FutureError"].append(message.removeprefix("(will be fatal in the future): "))
                 else:
@@ -641,47 +692,51 @@
         return f"<DesktopEntry Name='{self.Name.default_text}'>"
 
     def __eq__(self, obj: object) -> bool:
         if not isinstance(obj, DesktopEntry):
             return False
 
         try:
-            assert self.Type == obj.Type
-            assert self.Version == obj.Version
-            assert self.Name == obj.Name
-            assert self.GenericName == obj.GenericName
-            assert self.NoDisplay == obj.NoDisplay
-            assert self.Comment == obj.Comment
-            assert self.Icon == obj.Icon
-            assert self.Hidden == obj.Hidden
-            assert self.OnlyShowIn == obj.OnlyShowIn
-            assert self.NotShowIn == obj.NotShowIn
-            assert self.DBusActivatable == obj.DBusActivatable
-            assert self.TryExec == obj.TryExec
-            assert self.Exec == obj.Exec
-            assert self.Path == obj.Path
-            assert self.Terminal == obj.Terminal
-            assert self.MimeType == obj.MimeType
-            assert self.Categories == obj.Categories
-            assert self.Implements == obj.Implements
-            assert self.Keywords == obj.Keywords
-            assert self.StartupNotify == obj.StartupNotify
-            assert self.StartupWMClass == obj.StartupWMClass
-            assert self.URL == obj.URL
-            assert self.PrefersNonDefaultGPU == obj.PrefersNonDefaultGPU
-            assert self.SingleMainWindow == obj.SingleMainWindow
-            assert _compare_dict(self.Actions, obj.Actions)
-            assert _compare_dict(self.CustomKeys, obj.CustomKeys)
+            _assert_func(self.Type == obj.Type)
+            _assert_func(self.Version == obj.Version)
+            _assert_func(self.Name == obj.Name)
+            _assert_func(self.GenericName == obj.GenericName)
+            _assert_func(self.NoDisplay == obj.NoDisplay)
+            _assert_func(self.Comment == obj.Comment)
+            _assert_func(self.Icon == obj.Icon)
+            _assert_func(self.Hidden == obj.Hidden)
+            _assert_func(self.OnlyShowIn == obj.OnlyShowIn)
+            _assert_func(self.NotShowIn == obj.NotShowIn)
+            _assert_func(self.DBusActivatable == obj.DBusActivatable)
+            _assert_func(self.TryExec == obj.TryExec)
+            _assert_func(self.Exec == obj.Exec)
+            _assert_func(self.Path == obj.Path)
+            _assert_func(self.Terminal == obj.Terminal)
+            _assert_func(self.MimeType == obj.MimeType)
+            _assert_func(self.Categories == obj.Categories)
+            _assert_func(self.Implements == obj.Implements)
+            _assert_func(self.Keywords == obj.Keywords)
+            _assert_func(self.StartupNotify == obj.StartupNotify)
+            _assert_func(self.StartupWMClass == obj.StartupWMClass)
+            _assert_func(self.URL == obj.URL)
+            _assert_func(self.PrefersNonDefaultGPU == obj.PrefersNonDefaultGPU)
+            _assert_func(self.SingleMainWindow == obj.SingleMainWindow)
+            _assert_func(_compare_dict(self.Actions, obj.Actions))
+            _assert_func(_compare_dict(self.CustomKeys, obj.CustomKeys))
             return True
         except AssertionError:
             return False
 
     @staticmethod
     def get_keywords() -> list[str]:
-        "Returns the list of Keywords of a Desktop Entry"
+        """
+        Returns the list of Keywords of a Desktop Entry
+
+        :return: The list of Keys
+        """
         return [
             "Type",
             "Version",
             "Name",
             "GenericName",
             "NoDisplay",
             "Comment",
@@ -708,70 +763,121 @@
 class DesktopEntryCollection:
     "Represents a Collection of multiple Desktop Entries"
     def __init__(self) -> None:
         self.desktop_entries: dict[str, DesktopEntry] = {}
         "The desktop entries"
 
     def load_file(self, path: Union[str, os.PathLike]) -> None:
-        "Loads the given file"
+        """
+        Lods the given desktop entry file and adds it to the collection
+
+        :param path: The path to the desktop entry
+        """
         entry = DesktopEntry.from_file(path)
         self.desktop_entries[os.path.basename(path).removesuffix(".desktop")] = entry
 
-    def load_directory(self, path: Union[str, os.PathLike]) -> None:
-        "Loads all desktop entries from the given directory"
+    def load_directory(self, path: Union[str, os.PathLike]) -> bool:
+        """
+        Loads all desktop entries from the given directory
+
+        :param path: The directory
+        :return: True if all desktop entries could be loaded, False if some couldn't be loaded
+        """
+        no_error = True
         for i in os.listdir(path):
             if i.endswith(".desktop"):
-                self.load_file(os.path.join(path, i))
-
-    def load_menu(self) -> None:
-        "Loads all desktop entries from the menu"
+                try:
+                    self.load_file(os.path.join(path, i))
+                except Exception:
+                    no_error = False
+        return no_error
+
+    def load_menu(self) -> bool:
+        """
+        Loads all desktop entries from the menu
+
+        :return: True if all desktop entries could be loaded, False if some couldn't be loaded
+        """
+        no_error = True
         for i in get_xdg_data_dirs():
             menu_dir = os.path.join(i, "applications")
             if os.path.isdir(menu_dir):
-                self.load_directory(menu_dir)
+                if not self.load_directory(menu_dir):
+                    no_error = False
+        return no_error
+
+    def load_desktop(self) -> bool:
+        """
+        Loads all desktop entries files from the Desktop
 
-    def load_desktop(self) -> None:
-        "Loads all desktop entries files from the Desktop"
+        :return: True if all desktop etntries could be loaded, False if some couldn't be loaded
+        """
         desktop_path = subprocess.check_output(["xdg-user-dir", "DESKTOP"]).decode("utf-8").strip()
         if os.path.isdir(desktop_path):
-            self.load_directory(desktop_path)
+            return self.load_directory(desktop_path)
+        return False
 
-    def load_autostart(self) -> None:
-        "Loads all autostart entries"
+    def load_autostart(self) -> bool:
+        """
+        Loads all autostart entries
+
+        :return: True if all desktop etntries could be loaded, False if some couldn't be loaded
+        """
+        no_error = True
         for i in ("/run/host/etc/xdg/autostart" if _is_flatpak() else "/etc/xdg/autostart", os.path.expanduser("~/.config/autostart/")):
             if os.path.isdir(i):
-                self.load_directory(i)
+                if not self.load_directory(i):
+                    no_error = False
+        return no_error
 
     def get_entries_by_category(self, category: str) -> list[DesktopEntry]:
-        "Returns a list of all desktop entries that have the given category"
-        entry_list = []
+        """
+        Returns a list of all desktop entries that have the given category
+
+        :param category: The category
+        :return: The list of desktop entries
+        """
+        entry_list: list[DesktopEntry] = []
         for i in self.desktop_entries.values():
             if category in i.Categories:
                 entry_list.append(i)
         return entry_list
 
     def get_entries_by_mime_type(self, mime_type: str) -> list[DesktopEntry]:
-        "Returns a list of all desktop entries that can open the given MimeType"
-        entry_list = []
+        """
+        Returns a list of all desktop entries that can open the given MimeType
+
+        :param mime_type: The MimeType
+        :return: The list of desktop entries
+        """
+        entry_list: list[DesktopEntry] = []
         for i in self.desktop_entries.values():
             if mime_type in i.MimeType:
                 entry_list.append(i)
         return entry_list
 
     def get_visible_entries(self) -> list[DesktopEntry]:
-        "Get a list of all desktop enties that should be shown to the User"
-        entry_list = []
+        """
+        Returns a list of all desktop enties that should be shown to the User
+
+        :return: The list of desktop entries
+        """
+        entry_list: list[DesktopEntry] = []
         for i in self.desktop_entries.values():
             if i.should_show():
                 entry_list.append(i)
         return entry_list
 
     def get_menu_entries(self) -> list[DesktopEntry]:
-        "Get a list of all desktop enties that should be shown in the Menu"
-        entry_list = []
+        """
+        Returns a list of all desktop enties that should be shown in the Menu
+
+        :return: The list of desktop entries
+        """
+        entry_list: list[DesktopEntry] = []
         for i in self.desktop_entries.values():
             if i.should_show_in_menu():
                 entry_list.append(i)
         return entry_list
 
     def __len__(self) -> int:
         return len(self.desktop_entries)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `desktop-entry-lib-3.0/desktop_entry_lib.egg-info/PKG-INFO` & `desktop-entry-lib-3.1/desktop_entry_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: desktop-entry-lib
-Version: 3.0
+Version: 3.1
 Summary: A library for working with .desktop files
 Author-email: JakobDev <jakobdev@gmx.de>
 License: BSD-2-Clause
 Project-URL: Source, https://codeberg.org/JakobDev/desktop-entry-lib
 Project-URL: Issues, https://codeberg.org/JakobDev/desktop-entry-lib/issues
 Project-URL: Documentation, https://desktop-entry-lib.readthedocs.io
 Project-URL: Donation, https://ko-fi.com/jakobdev
```

### Comparing `desktop-entry-lib-3.0/pyproject.toml` & `desktop-entry-lib-3.1/pyproject.toml`

 * *Files identical despite different names*

