# Comparing `tmp/pynterface-0.0.1.tar.gz` & `tmp/pynterface-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynterface-0.0.1.tar", last modified: Sun May 14 18:06:37 2023, max compression
+gzip compressed data, was "pynterface-0.0.2.tar", last modified: Mon May 15 15:01:12 2023, max compression
```

## Comparing `pynterface-0.0.1.tar` & `pynterface-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-14 18:06:37.295855 pynterface-0.0.1/
--rw-r--r--   0 vivaan     (501) staff       (20)     1071 2023-05-04 02:59:32.000000 pynterface-0.0.1/LICENSE
--rw-r--r--   0 vivaan     (501) staff       (20)       33 2023-05-14 03:48:17.000000 pynterface-0.0.1/MANIFEST.in
--rw-r--r--   0 vivaan     (501) staff       (20)     1484 2023-05-14 18:06:37.295554 pynterface-0.0.1/PKG-INFO
--rw-r--r--   0 vivaan     (501) staff       (20)     1156 2023-05-14 04:10:04.000000 pynterface-0.0.1/README.md
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-14 18:06:37.293350 pynterface-0.0.1/pynterface/
--rw-r--r--   0 vivaan     (501) staff       (20)      238 2023-05-14 18:02:44.000000 pynterface-0.0.1/pynterface/__init__.py
--rw-r--r--   0 vivaan     (501) staff       (20)     2840 2023-05-14 01:50:32.000000 pynterface-0.0.1/pynterface/input.py
--rw-r--r--   0 vivaan     (501) staff       (20)     6495 2023-05-09 23:26:51.000000 pynterface-0.0.1/pynterface/loading.py
--rw-r--r--   0 vivaan     (501) staff       (20)     3525 2023-05-14 01:47:16.000000 pynterface-0.0.1/pynterface/menu.py
--rw-r--r--   0 vivaan     (501) staff       (20)     5209 2023-05-14 02:09:21.000000 pynterface-0.0.1/pynterface/printing.py
--rw-r--r--   0 vivaan     (501) staff       (20)     5848 2023-05-14 02:31:12.000000 pynterface-0.0.1/pynterface/style.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-14 18:06:37.295192 pynterface-0.0.1/pynterface.egg-info/
--rw-r--r--   0 vivaan     (501) staff       (20)     1484 2023-05-14 18:06:37.000000 pynterface-0.0.1/pynterface.egg-info/PKG-INFO
--rw-r--r--   0 vivaan     (501) staff       (20)      301 2023-05-14 18:06:37.000000 pynterface-0.0.1/pynterface.egg-info/SOURCES.txt
--rw-r--r--   0 vivaan     (501) staff       (20)        1 2023-05-14 18:06:37.000000 pynterface-0.0.1/pynterface.egg-info/dependency_links.txt
--rw-r--r--   0 vivaan     (501) staff       (20)       11 2023-05-14 18:06:37.000000 pynterface-0.0.1/pynterface.egg-info/top_level.txt
--rw-r--r--   0 vivaan     (501) staff       (20)       38 2023-05-14 18:06:37.295957 pynterface-0.0.1/setup.cfg
--rw-r--r--   0 vivaan     (501) staff       (20)      612 2023-05-14 04:04:56.000000 pynterface-0.0.1/setup.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-15 15:01:12.756802 pynterface-0.0.2/
+-rw-r--r--   0 vivaan     (501) staff       (20)     1071 2023-05-04 02:59:32.000000 pynterface-0.0.2/LICENSE
+-rw-r--r--   0 vivaan     (501) staff       (20)       33 2023-05-14 03:48:17.000000 pynterface-0.0.2/MANIFEST.in
+-rw-r--r--   0 vivaan     (501) staff       (20)     1484 2023-05-15 15:01:12.756540 pynterface-0.0.2/PKG-INFO
+-rw-r--r--   0 vivaan     (501) staff       (20)     1156 2023-05-14 04:10:04.000000 pynterface-0.0.2/README.md
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-15 15:01:12.755107 pynterface-0.0.2/pynterface/
+-rw-r--r--   0 vivaan     (501) staff       (20)      238 2023-05-15 15:00:32.000000 pynterface-0.0.2/pynterface/__init__.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     2840 2023-05-14 01:50:32.000000 pynterface-0.0.2/pynterface/input.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     6495 2023-05-09 23:26:51.000000 pynterface-0.0.2/pynterface/loading.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     3375 2023-05-15 14:59:09.000000 pynterface-0.0.2/pynterface/menu.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     5444 2023-05-14 18:25:39.000000 pynterface-0.0.2/pynterface/printing.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     5848 2023-05-15 14:51:42.000000 pynterface-0.0.2/pynterface/style.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-15 15:01:12.756202 pynterface-0.0.2/pynterface.egg-info/
+-rw-r--r--   0 vivaan     (501) staff       (20)     1484 2023-05-15 15:01:12.000000 pynterface-0.0.2/pynterface.egg-info/PKG-INFO
+-rw-r--r--   0 vivaan     (501) staff       (20)      301 2023-05-15 15:01:12.000000 pynterface-0.0.2/pynterface.egg-info/SOURCES.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)        1 2023-05-15 15:01:12.000000 pynterface-0.0.2/pynterface.egg-info/dependency_links.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)       11 2023-05-15 15:01:12.000000 pynterface-0.0.2/pynterface.egg-info/top_level.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)       38 2023-05-15 15:01:12.756881 pynterface-0.0.2/setup.cfg
+-rw-r--r--   0 vivaan     (501) staff       (20)      612 2023-05-14 04:04:56.000000 pynterface-0.0.2/setup.py
```

### Comparing `pynterface-0.0.1/LICENSE` & `pynterface-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pynterface-0.0.1/PKG-INFO` & `pynterface-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynterface
-Version: 0.0.1
+Version: 0.0.2
 Summary: Terminal-Based Printing Tools!
 Author: Vivaan Singhvi
 Author-email: singhvi.vivaan@gmail.com
 License: MIT
 Project-URL: Documentation, https://pynterface.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pynterface-0.0.1/README.md` & `pynterface-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pynterface-0.0.1/pynterface/input.py` & `pynterface-0.0.2/pynterface/input.py`

 * *Files identical despite different names*

### Comparing `pynterface-0.0.1/pynterface/loading.py` & `pynterface-0.0.2/pynterface/loading.py`

 * *Files identical despite different names*

### Comparing `pynterface-0.0.1/pynterface/menu.py` & `pynterface-0.0.2/pynterface/menu.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,25 +14,14 @@
     if isinstance(opt, (bool, str, float, int, object)):
         return str(opt)
     try:
         return opt.__name__
     except:
         raise AssertionError("Option type unable to be converted to string using __name__.")
 
-def __list_print(prompt: str, spacing: int, str_options: list) -> None:
-    """
-    Prints menu options and beginning prompt.
-    """
-
-    if prompt:
-        print(prompt)
-
-    for index, opt in enumerate(str_options):
-        print(f"{' '*spacing}{index+1}. {opt}")
-
 def numbered_menu(options: Iterable[Any], beginning_prompt: str = None, 
                   selection_prompt: str = None, spacing: int = 4, return_number: bool = False) -> Any:
 
     """
     Creates a numbered menu, in the following format:
     ```
     '''
@@ -52,15 +41,19 @@
 
     assert isinstance(options, Iterable), "Options must be iterable!"
     assert len(options) >= 2, "There should be at least two values to select from!"
     assert isinstance(spacing, int) and spacing >= 0, "Spacing must be a non-negative integer!"
 
     str_options = list(map(__map_to_str, options))
 
-    __list_print(prompt=beginning_prompt, spacing=spacing, str_options=str_options)
+    if beginning_prompt:
+        print(beginning_prompt)
+
+    for index, opt in enumerate(str_options):
+        print(f"{' '*spacing}{index+1}. {opt}")
     
     choice = bounded_int(1, len(str_options), prompt=selection_prompt)
 
     if return_number:
         return choice
     
     return options[choice - 1]
@@ -91,15 +84,19 @@
     assert isinstance(options, Iterable), "Options must be iterable!"
     assert len(options) >= 2, "There should be at least two values to select from!"
     assert isinstance(spacing, int) and spacing >= 0, "Spacing must be a non-negative integer!"
     assert isinstance(selector, str), "List element introducer must be a string!"
 
     str_options = list(map(__map_to_str, options))
 
-    __list_print(prompt=beginning_prompt, spacing=spacing, str_options=str_options)
+    if beginning_prompt:
+        print(beginning_prompt)
+
+    for opt in str_options:
+        print(f"{' '*spacing}{selector} {opt}")
 
     choice = input(selection_prompt)
 
     while choice.strip() not in str_options:
         choice = input(error_prompt)
 
     return options[str_options.index(choice)]
```

### Comparing `pynterface-0.0.1/pynterface/printing.py` & `pynterface-0.0.2/pynterface/printing.py`

 * *Files 5% similar despite different names*

```diff
@@ -136,24 +136,26 @@
     """
 
     assert all([0 <= color <= 255 for color in left_rgb+right_rgb]), "Invalid RGB number entered."
     assert len(left_rgb) == len(right_rgb) == 3, "Tuple with RGB values must have a length of 3." 
     assert isinstance(message, (str, Iterable)), "Message must be a string or a list of strings representing newlines."
     assert mode in ["text", "background"], "Invalid mode."
 
-    def get_value(a, b, i, n): return a + round((b-a)*(i/n))
+    # tune hte rgb value depending on progress in the line: a and b are start and end values, i is the progress, and n is the max count.
+    def get_value(a, b, i, n): return a + round((b-a)*(i/n))  
 
+    # filter mode
     if mode == "text": method = Color
     elif mode == "background": method = Background
     
     # splits depending on the types
     if isinstance(message, str): messages = message.split("\n")
     else: messages = [*message]
 
     messages = [__split_esc_chars(line) for line in messages]
     max_len = max([len(s) for s in messages]) - 1
     rgb_vals = [tuple([get_value(left_rgb[ii], right_rgb[ii], i, max_len) for ii in range(3)]) for i in range(max_len+1)]
-    output = f"{method.RESET_COLOR if method == Color else method.RESET_BACKGROUND}\n".join(
-        ["".join([method.RGB(rgb_vals[i]) + line[i] for i in range(len(line))]) for line in messages]
+    output = f"{method.RESET_COLOR if method == Color else method.RESET_BACKGROUND}\n".join(            # joins the lines by a reset color/background
+        ["".join([method.RGB(rgb_vals[i]) + line[i] for i in range(len(line))]) for line in messages]   # creates the line
     )
 
     return output
```

### Comparing `pynterface-0.0.1/pynterface/style.py` & `pynterface-0.0.2/pynterface/style.py`

 * *Files identical despite different names*

### Comparing `pynterface-0.0.1/pynterface.egg-info/PKG-INFO` & `pynterface-0.0.2/pynterface.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynterface
-Version: 0.0.1
+Version: 0.0.2
 Summary: Terminal-Based Printing Tools!
 Author: Vivaan Singhvi
 Author-email: singhvi.vivaan@gmail.com
 License: MIT
 Project-URL: Documentation, https://pynterface.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pynterface-0.0.1/setup.py` & `pynterface-0.0.2/setup.py`

 * *Files identical despite different names*

