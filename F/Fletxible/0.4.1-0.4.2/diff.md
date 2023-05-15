# Comparing `tmp/Fletxible-0.4.1.tar.gz` & `tmp/Fletxible-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fletxible-0.4.1.tar", last modified: Sat May 13 13:56:08 2023, max compression
+gzip compressed data, was "Fletxible-0.4.2.tar", last modified: Mon May 15 13:41:39 2023, max compression
```

## Comparing `Fletxible-0.4.1.tar` & `Fletxible-0.4.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-13 13:56:08.551626 Fletxible-0.4.1/
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-13 13:56:08.548640 Fletxible-0.4.1/Fletxible.egg-info/
--rw-r--r--   0 ahmad      (501) staff       (20)      830 2023-05-13 13:56:08.000000 Fletxible-0.4.1/Fletxible.egg-info/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)      326 2023-05-13 13:56:08.000000 Fletxible-0.4.1/Fletxible.egg-info/SOURCES.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-05-13 13:56:08.000000 Fletxible-0.4.1/Fletxible.egg-info/dependency_links.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       50 2023-05-13 13:56:08.000000 Fletxible-0.4.1/Fletxible.egg-info/entry_points.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       37 2023-05-13 13:56:08.000000 Fletxible-0.4.1/Fletxible.egg-info/requires.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        6 2023-05-13 13:56:08.000000 Fletxible-0.4.1/Fletxible.egg-info/top_level.txt
--rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-04-29 15:25:05.000000 Fletxible-0.4.1/LICENSE
--rw-r--r--   0 ahmad      (501) staff       (20)      830 2023-05-13 13:56:08.551396 Fletxible-0.4.1/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)     4106 2023-05-01 16:06:19.000000 Fletxible-0.4.1/README.md
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-13 13:56:08.550493 Fletxible-0.4.1/logic/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-01 13:39:08.000000 Fletxible-0.4.1/logic/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2168 2023-05-13 13:50:26.000000 Fletxible-0.4.1/logic/cli.py
--rw-r--r--   0 ahmad      (501) staff       (20)      164 2023-05-13 13:31:46.000000 Fletxible-0.4.1/logic/main.py
--rw-r--r--   0 ahmad      (501) staff       (20)     6555 2023-05-13 13:45:23.000000 Fletxible-0.4.1/logic/script.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2094 2023-05-13 13:48:57.000000 Fletxible-0.4.1/logic/utilities.py
--rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-05-13 13:56:08.551693 Fletxible-0.4.1/setup.cfg
--rw-r--r--   0 ahmad      (501) staff       (20)     1110 2023-05-13 13:53:17.000000 Fletxible-0.4.1/setup.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-13 13:56:08.550930 Fletxible-0.4.1/tests/
--rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-05-01 14:25:50.000000 Fletxible-0.4.1/tests/test_route.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-15 13:41:39.313826 Fletxible-0.4.2/
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-15 13:41:39.311269 Fletxible-0.4.2/Fletxible.egg-info/
+-rw-r--r--   0 ahmad      (501) staff       (20)      830 2023-05-15 13:41:39.000000 Fletxible-0.4.2/Fletxible.egg-info/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)      326 2023-05-15 13:41:39.000000 Fletxible-0.4.2/Fletxible.egg-info/SOURCES.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-05-15 13:41:39.000000 Fletxible-0.4.2/Fletxible.egg-info/dependency_links.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       50 2023-05-15 13:41:39.000000 Fletxible-0.4.2/Fletxible.egg-info/entry_points.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       37 2023-05-15 13:41:39.000000 Fletxible-0.4.2/Fletxible.egg-info/requires.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        6 2023-05-15 13:41:39.000000 Fletxible-0.4.2/Fletxible.egg-info/top_level.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-04-29 15:25:05.000000 Fletxible-0.4.2/LICENSE
+-rw-r--r--   0 ahmad      (501) staff       (20)      830 2023-05-15 13:41:39.313624 Fletxible-0.4.2/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)     4106 2023-05-01 16:06:19.000000 Fletxible-0.4.2/README.md
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-15 13:41:39.312741 Fletxible-0.4.2/logic/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-01 13:39:08.000000 Fletxible-0.4.2/logic/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2168 2023-05-13 13:50:26.000000 Fletxible-0.4.2/logic/cli.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      312 2023-05-14 11:02:33.000000 Fletxible-0.4.2/logic/main.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     6485 2023-05-13 15:17:29.000000 Fletxible-0.4.2/logic/script.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2304 2023-05-14 20:20:25.000000 Fletxible-0.4.2/logic/utilities.py
+-rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-05-15 13:41:39.313898 Fletxible-0.4.2/setup.cfg
+-rw-r--r--   0 ahmad      (501) staff       (20)     1110 2023-05-15 13:41:13.000000 Fletxible-0.4.2/setup.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-15 13:41:39.313200 Fletxible-0.4.2/tests/
+-rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-05-01 14:25:50.000000 Fletxible-0.4.2/tests/test_route.py
```

### Comparing `Fletxible-0.4.1/Fletxible.egg-info/PKG-INFO` & `Fletxible-0.4.2/Fletxible.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fletxible
-Version: 0.4.1
+Version: 0.4.2
 Summary: Web Boilerplate for Flet Library
 Home-page: https://github.com/LineIndent/fletxible
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 Keywords: python web template,web application,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Fletxible-0.4.1/LICENSE` & `Fletxible-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Fletxible-0.4.1/PKG-INFO` & `Fletxible-0.4.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fletxible
-Version: 0.4.1
+Version: 0.4.2
 Summary: Web Boilerplate for Flet Library
 Home-page: https://github.com/LineIndent/fletxible
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 Keywords: python web template,web application,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Fletxible-0.4.1/README.md` & `Fletxible-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `Fletxible-0.4.1/logic/cli.py` & `Fletxible-0.4.2/logic/cli.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.4.1/logic/script.py` & `Fletxible-0.4.2/logic/script.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,38 +77,35 @@
 
 def set_default_methods_script(docs: dict):
     # Loop over the nav list and create/update files
     # 1. Temp. list to store the filepaths in + the modules dict
     file_list: list = []
     # route_keys: dict = {}
 
-    # 2. Returned default page text
-    # method = set_app_default_pages()
-
-    # 3. Loop through navigation tree and append the file_list with the filepaths
+    # 2. Loop through navigation tree and append the file_list with the filepaths
     for page in docs["nav"]:
         for key in page:
             filename = f"{page[key]}"
             filepath = os.path.join("pages", filename)
             file_list.append(filepath)
 
         filename = os.path.splitext(filename)[0]
 
         route_keys["/" + filename] = importlib.util.spec_from_file_location(
             filename, filepath
         )
 
-    # 4. Loop through the file_list and create the corresponding pages
+    # 3. Loop through the file_list and create the corresponding pages
     for filepath in file_list:
         method = set_app_default_pages()
         if not os.path.exists(filepath):
             with open(filepath, "w") as f:
                 f.write(f"{method}")
 
-    # 5. Update/create the route.pickles file for modules setup
+    # 4. Update/create the route.pickles file for modules setup
     for file in os.listdir("pages"):
         # Set the path of the file to loop over folders and only include files
         path = os.path.join("pages", file)
 
         # If the path is NOT a folder, continue ...
         if not os.path.isdir(path):
             # Get the list of routes from utilitites
@@ -132,19 +129,19 @@
 
             with open(f"./pages/{file}", "w") as f:
                 f.write(modified_string)
 
         else:
             pass
 
-    # the route.pickle file is a binary file!
+    # 5. The route.pickle file is a binary file!
     with open("./logic/route.pickle", "wb") as f:
         pickle.dump(route_keys, f)
 
-    # Finally, return the route_keys so we use itin the route.py logic
+    # 6. Finally, return the route_keys so we use itin the route.py logic
     return route_keys
 
 
 def map_yaml(yaml_file_path, output_file_path):
     # 1. open the flet_config.yml file and safe load the data
     with open(yaml_file_path) as f:
         yaml_data = yaml.safe_load(f)
```

### Comparing `Fletxible-0.4.1/logic/utilities.py` & `Fletxible-0.4.2/logic/utilities.py`

 * *Files 27% similar despite different names*

```diff
@@ -38,38 +38,41 @@
 import flet as ft
 from route import route
 
 # main view
 def pageView():
     return ft.View(
         horizontal_alignment="center",
-        vertical_alignment="center",
+        vertical_alignment="start",
         controls=[
-            ft.Row(
-                alignment="center",
-                controls=
-                    [
-                    # start #
-                    
-                    # end #       
+           ft.Row(
+                alignment="spaceAround",
+                controls=[
+                    ft.Row(
+                        alignment="start",
+                        controls=[ft.Text("fletxible.", size=21, weight="w700")],
+                    ),
+                ft.Row(
+                    alignment="center",
+                    controls=
+                        [
+                        # start #
+                        
+                        # end #       
+                    ],
+                ),
                 ],
             ),
-            ft.Text("Hello World!", size=21)
         ]
     )
 """
 
     return string
 
 
-############################################
-######### Create config file YAML ##########
-############################################
-
-
 def set_up_yaml_file():
     string = """
 site-name: ""
 repo-url: ""
 
 theme:
   - bgcolor: "#2e2f3e"
@@ -81,19 +84,21 @@
   - About: "about.py"
 
 """
     return string
 
 
 def set_up_main_method():
-    string = """import flet as ft
+    string = """# Modules for Flet and Fletxible
+import flet as ft
 from script import script
 
 
 def main(page: ft.Page):
+    # Run main script ... 
     script(page)
     page.update()
 
 
 if __name__ == "__main__":
     ft.flet.app(target=main)  
 """
```

### Comparing `Fletxible-0.4.1/setup.py` & `Fletxible-0.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="Fletxible",
-    version="0.4.1",
+    version="0.4.2",
     author="S. Ahmad P. Hakimi",
     author_email="pourhakimi@pm.me",
     description="Web Boilerplate for Flet Library",
     long_description="Fletxible is a Python web boilerplate project designed to provide a solid foundation for building web applications with Python and Flet. The project comes pre-configured with a range of tools and features to make it easy for developers to get started building their applications, without the need to spend time setting up infrastructure or configuring tools.",
     long_description_content_type="text/markdown",
     url="https://github.com/LineIndent/fletxible",
     packages=["logic"],
```

