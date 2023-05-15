# Comparing `tmp/toui-1.2.0a1.tar.gz` & `tmp/toui-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toui-1.2.0a1.tar", last modified: Wed Apr 19 04:22:56 2023, max compression
+gzip compressed data, was "toui-2.0.0.tar", last modified: Mon May 15 12:58:11 2023, max compression
```

## Comparing `toui-1.2.0a1.tar` & `toui-2.0.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 04:22:56.746577 toui-1.2.0a1/
--rw-rw-rw-   0        0        0     1094 2023-03-28 04:20:49.000000 toui-1.2.0a1/LICENSE
--rw-rw-rw-   0        0        0       16 2023-03-28 04:20:49.000000 toui-1.2.0a1/MANIFEST.in
--rw-rw-rw-   0        0        0     3056 2023-04-19 04:22:56.745573 toui-1.2.0a1/PKG-INFO
--rw-rw-rw-   0        0        0     2620 2023-04-13 08:05:30.000000 toui-1.2.0a1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 04:22:56.679569 toui-1.2.0a1/examples/
--rw-rw-rw-   0        0        0        0 2023-03-28 04:20:49.000000 toui-1.2.0a1/examples/__init__.py
--rw-rw-rw-   0        0        0      910 2023-04-13 08:21:09.000000 toui-1.2.0a1/examples/advanced_example_1_toui_blueprint.py
--rw-rw-rw-   0        0        0      556 2023-03-28 04:20:49.000000 toui-1.2.0a1/examples/example_1_simple_website.py
--rw-rw-rw-   0        0        0      535 2023-03-28 04:20:49.000000 toui-1.2.0a1/examples/example_2_simple_desktop_app.py
--rw-rw-rw-   0        0        0      762 2023-03-28 04:20:49.000000 toui-1.2.0a1/examples/example_3_updating_page.py
--rw-rw-rw-   0        0        0      699 2023-03-28 04:20:49.000000 toui-1.2.0a1/examples/example_4_function_with_arg.py
--rw-rw-rw-   0        0        0      995 2023-03-28 04:20:49.000000 toui-1.2.0a1/examples/example_5_user_variables.py
--rw-rw-rw-   0        0        0      162 2023-03-28 04:20:49.000000 toui-1.2.0a1/examples/example_6_quick_website.py
--rw-rw-rw-   0        0        0      166 2023-03-28 04:20:49.000000 toui-1.2.0a1/examples/example_7_quick_desktop_app.py
-drwxrwxrwx   0        0        0        0 2023-04-19 04:22:56.681812 toui-1.2.0a1/images/
--rw-rw-rw-   0        0        0    29049 2023-03-28 04:20:49.000000 toui-1.2.0a1/images/logo.png
--rw-rw-rw-   0        0        0       42 2023-04-19 04:22:56.747575 toui-1.2.0a1/setup.cfg
--rw-rw-rw-   0        0        0     1225 2023-04-13 08:27:05.000000 toui-1.2.0a1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-19 04:22:56.709021 toui-1.2.0a1/toui/
--rw-rw-rw-   0        0        0      216 2023-04-19 04:19:58.000000 toui-1.2.0a1/toui/__init__.py
--rw-rw-rw-   0        0        0      431 2023-04-15 14:31:15.000000 toui-1.2.0a1/toui/_defaults.py
--rw-rw-rw-   0        0        0     1093 2023-04-15 17:56:59.000000 toui-1.2.0a1/toui/_helpers.py
--rw-rw-rw-   0        0        0     9783 2023-04-19 03:21:10.000000 toui-1.2.0a1/toui/_javascript_templates.py
--rw-rw-rw-   0        0        0     7391 2023-04-19 03:38:33.000000 toui-1.2.0a1/toui/_signals.py
--rw-rw-rw-   0        0        0    24975 2023-04-19 04:15:22.000000 toui-1.2.0a1/toui/apps.py
--rw-rw-rw-   0        0        0    20507 2023-04-19 03:34:58.000000 toui-1.2.0a1/toui/elements.py
--rw-rw-rw-   0        0        0      168 2023-03-28 04:20:49.000000 toui-1.2.0a1/toui/exceptions.py
--rw-rw-rw-   0        0        0    15251 2023-04-15 16:14:35.000000 toui-1.2.0a1/toui/pages.py
--rw-rw-rw-   0        0        0     2350 2023-03-28 04:20:49.000000 toui-1.2.0a1/toui/structure.py
-drwxrwxrwx   0        0        0        0 2023-04-19 04:22:56.743572 toui-1.2.0a1/toui.egg-info/
--rw-rw-rw-   0        0        0     3056 2023-04-19 04:22:56.000000 toui-1.2.0a1/toui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      707 2023-04-19 04:22:56.000000 toui-1.2.0a1/toui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 04:22:56.000000 toui-1.2.0a1/toui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      174 2023-04-19 04:22:56.000000 toui-1.2.0a1/toui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-19 04:22:56.000000 toui-1.2.0a1/toui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-15 12:58:11.279434 toui-2.0.0/
+-rw-rw-rw-   0        0        0     1094 2023-05-04 15:56:54.000000 toui-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0       16 2023-05-04 15:56:54.000000 toui-2.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3153 2023-05-15 12:58:11.278433 toui-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2780 2023-05-14 05:09:36.000000 toui-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 12:58:11.208718 toui-2.0.0/examples/
+-rw-rw-rw-   0        0        0        0 2023-05-04 15:56:54.000000 toui-2.0.0/examples/__init__.py
+-rw-rw-rw-   0        0        0      910 2023-05-04 15:56:54.000000 toui-2.0.0/examples/advanced_example_1_toui_blueprint.py
+-rw-rw-rw-   0        0        0      556 2023-05-04 15:56:54.000000 toui-2.0.0/examples/example_1_simple_website.py
+-rw-rw-rw-   0        0        0      535 2023-05-04 15:56:54.000000 toui-2.0.0/examples/example_2_simple_desktop_app.py
+-rw-rw-rw-   0        0        0      762 2023-05-04 15:56:54.000000 toui-2.0.0/examples/example_3_updating_page.py
+-rw-rw-rw-   0        0        0      699 2023-05-04 15:56:54.000000 toui-2.0.0/examples/example_4_function_with_arg.py
+-rw-rw-rw-   0        0        0      995 2023-05-04 15:56:54.000000 toui-2.0.0/examples/example_5_user_variables.py
+-rw-rw-rw-   0        0        0      162 2023-05-04 15:56:54.000000 toui-2.0.0/examples/example_6_quick_website.py
+-rw-rw-rw-   0        0        0      166 2023-05-04 15:56:54.000000 toui-2.0.0/examples/example_7_quick_desktop_app.py
+drwxrwxrwx   0        0        0        0 2023-05-15 12:58:11.214278 toui-2.0.0/images/
+-rw-rw-rw-   0        0        0    29049 2023-05-04 15:56:54.000000 toui-2.0.0/images/logo.png
+-rw-rw-rw-   0        0        0       42 2023-05-15 12:58:11.279434 toui-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1517 2023-05-15 11:45:45.000000 toui-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 12:58:11.266413 toui-2.0.0/toui/
+-rw-rw-rw-   0        0        0      234 2023-05-15 12:48:40.000000 toui-2.0.0/toui/__init__.py
+-rw-rw-rw-   0        0        0      431 2023-05-04 15:56:54.000000 toui-2.0.0/toui/_defaults.py
+-rw-rw-rw-   0        0        0     1272 2023-05-13 12:51:28.000000 toui-2.0.0/toui/_helpers.py
+-rw-rw-rw-   0        0        0     9902 2023-05-14 03:43:28.000000 toui-2.0.0/toui/_javascript_templates.py
+-rw-rw-rw-   0        0        0     6450 2023-05-15 12:26:57.000000 toui-2.0.0/toui/_signals.py
+-rw-rw-rw-   0        0        0    26536 2023-05-15 12:14:16.000000 toui-2.0.0/toui/apps.py
+-rw-rw-rw-   0        0        0    20537 2023-05-13 12:51:22.000000 toui-2.0.0/toui/elements.py
+-rw-rw-rw-   0        0        0      316 2023-05-15 12:37:07.000000 toui-2.0.0/toui/exceptions.py
+-rw-rw-rw-   0        0        0    17082 2023-05-15 12:22:30.000000 toui-2.0.0/toui/pages.py
+-rw-rw-rw-   0        0        0     2350 2023-05-04 15:56:54.000000 toui-2.0.0/toui/structure.py
+drwxrwxrwx   0        0        0        0 2023-05-15 12:58:11.277433 toui-2.0.0/toui.egg-info/
+-rw-rw-rw-   0        0        0     3153 2023-05-15 12:58:11.000000 toui-2.0.0/toui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      707 2023-05-15 12:58:11.000000 toui-2.0.0/toui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 12:58:11.000000 toui-2.0.0/toui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      196 2023-05-15 12:58:11.000000 toui-2.0.0/toui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-15 12:58:11.000000 toui-2.0.0/toui.egg-info/top_level.txt
```

### Comparing `toui-1.2.0a1/LICENSE` & `toui-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `toui-1.2.0a1/PKG-INFO` & `toui-2.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: toui
-Version: 1.2.0a1
-Summary: Creates user interfaces (websites and desktop apps) from HTML easily
-Home-page: UNKNOWN
-Author: Mubarak Almehairbi
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![ToUI Image](images/logo.png)
 
 # Overview
 ToUI is a Python package for creating user interfaces (websites and desktop apps)
 from HTML easily. No JavaScript knowledge is required, but some knowledge of HTML
 is usually required.
 
@@ -26,14 +12,19 @@
 
 # How to install
 Run this command:
 ```shell
 pip install toui
 ```
 
+To install `toui` with less dependencies (but limited functionality), run the following command:
+```shell
+pip install toui --global-option="--small"
+```
+
 # How to create a basic website
 Import the required classes:
 ```python
 from toui import Website, Page
 ```
 Create a `Website` object:
 ```python
@@ -93,10 +84,8 @@
 Then you need to deploy the `flask_app` and not the `app`.
 
 # License and Copyrights
 Copyrights (c) 2023 Mubarak Almehairbi.
 This package is licensed under the MIT license.
 
 # Documentation
-You can find the documentation in this link: [ToUI docs](https://toui.readthedocs.io)
-
-
+You can find the documentation in this link: [ToUI docs](https://toui.readthedocs.io).
```

### Comparing `toui-1.2.0a1/README.md` & `toui-2.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: toui
+Version: 2.0.0
+Summary: Creates user interfaces (websites and desktop apps) from HTML easily
+Author: Mubarak Almehairbi
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![ToUI Image](images/logo.png)
 
 # Overview
 ToUI is a Python package for creating user interfaces (websites and desktop apps)
 from HTML easily. No JavaScript knowledge is required, but some knowledge of HTML
 is usually required.
 
@@ -12,14 +23,19 @@
 
 # How to install
 Run this command:
 ```shell
 pip install toui
 ```
 
+To install `toui` with less dependencies (but limited functionality), run the following command:
+```shell
+pip install toui --global-option="--small"
+```
+
 # How to create a basic website
 Import the required classes:
 ```python
 from toui import Website, Page
 ```
 Create a `Website` object:
 ```python
@@ -79,8 +95,8 @@
 Then you need to deploy the `flask_app` and not the `app`.
 
 # License and Copyrights
 Copyrights (c) 2023 Mubarak Almehairbi.
 This package is licensed under the MIT license.
 
 # Documentation
-You can find the documentation in this link: [ToUI docs](https://toui.readthedocs.io)
+You can find the documentation in this link: [ToUI docs](https://toui.readthedocs.io).
```

### Comparing `toui-1.2.0a1/examples/advanced_example_1_toui_blueprint.py` & `toui-2.0.0/examples/advanced_example_1_toui_blueprint.py`

 * *Files identical despite different names*

### Comparing `toui-1.2.0a1/examples/example_1_simple_website.py` & `toui-2.0.0/examples/example_1_simple_website.py`

 * *Files identical despite different names*

### Comparing `toui-1.2.0a1/examples/example_2_simple_desktop_app.py` & `toui-2.0.0/examples/example_2_simple_desktop_app.py`

 * *Files identical despite different names*

### Comparing `toui-1.2.0a1/examples/example_3_updating_page.py` & `toui-2.0.0/examples/example_3_updating_page.py`

 * *Files identical despite different names*

### Comparing `toui-1.2.0a1/examples/example_4_function_with_arg.py` & `toui-2.0.0/examples/example_4_function_with_arg.py`

 * *Files identical despite different names*

### Comparing `toui-1.2.0a1/examples/example_5_user_variables.py` & `toui-2.0.0/examples/example_5_user_variables.py`

 * *Files identical despite different names*

### Comparing `toui-1.2.0a1/images/logo.png` & `toui-2.0.0/images/logo.png`

 * *Files identical despite different names*

### Comparing `toui-1.2.0a1/setup.py` & `toui-2.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 import setuptools
+import sys
 from toui import __version__
 
 with open("README.md", "r") as file:
     long_description = file.read()
 
+small = False
+if "--small" in sys.argv:
+    small = True
+    sys.argv.remove('--small')  
+
 name = "ToUI"
 version = __version__
 author = "Mubarak Almehairbi"
 description = "Creates user interfaces (websites and desktop apps) from HTML easily"
 package_name = "toui"
 requirements = []
+optional_requirements = ['flask-login', 'flask-sqlalchemy', 'flask-basicauth']
 with open(f"requirements.txt", "rt") as file:
     for pkg in file.read().splitlines():
         pkg_name = pkg.split("==")[0]
+        if pkg_name.lower().replace("_","-") in optional_requirements and small:
+            continue
         pkg_version = pkg.split("==")[1]
         pkg_major_version = pkg_version.split(".")[0]
         req = f"{pkg_name}>={pkg_version},<{int(pkg_major_version)+1}"
         requirements.append(req)
 
 
 setuptools.setup(
```

### Comparing `toui-1.2.0a1/toui/_helpers.py` & `toui-2.0.0/toui/_helpers.py`

 * *Files 24% similar despite different names*

```diff
@@ -41,8 +41,18 @@
         selectors += f"[class=\"{class_name}\"]"
     if name:
         selectors += f"[name=\"{name}\"]"
     if attrs:
         for attr_key, attr_value in attrs.items():
             if attr_value:
                 selectors += f"[{attr_key}=\"{attr_value}\"]"
-    return selectors
+    return selectors
+
+
+def obj_converter(obj):
+    if obj is True:
+        return 'true'
+    if obj is False:
+        return 'false'
+    if obj is None:
+        return 'null'
+    return obj
```

### Comparing `toui-1.2.0a1/toui/_javascript_templates.py` & `toui-2.0.0/toui/_javascript_templates.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,316 +1,324 @@
 """
 JavaScript code that is added to HTML files.
 """
-web_template = f"""
+template = """
 var conn = "wss"
-if (location.protocol == "http:") {{
+if (location.protocol == "http:") {
     conn = "ws"
-}}
+}
 const socket = new WebSocket(conn + '://' + location.host + '/toui-communicate')
-socket.addEventListener('message', ev => {{
+socket.addEventListener('message', ev => {
     _findAndExecute(ev.data)
-  }});
+  });
 const urlPath = location.pathname
-async function _toPy(...arguments) {{
-    var func = arguments.shift()
-    var json = {{type: "page",
-                func:func,
-                args: arguments,
-                url: urlPath}}
-    var properties = _manageProperties()
+const _appType = "{app_type}"
+_touiFiles = {}
+_pywebviewIsLoaded = false
+async function _toPy(...args) {
+    var func = args.shift()
+    if (_appType === "DesktopApp" && _pywebviewIsLoaded == false) {
+        await _waitForPywebview()
+    }
+    var json = {type: "page",
+                func: func,
+                args: args,
+                url: urlPath}
+    _manageProperties()
     json['html'] = _getDoc()
+    json['uid'] = await _getUid()
     var jsonstring = JSON.stringify(json)
-    if (socket.readyState === 0) {{
-        socket.onopen = function() {{
+    if (socket.readyState === 0) {
+        socket.onopen = async function() {
             socket.send(jsonstring);
-        }}
-    }} else {{
+        }
+    } else {
         socket.send(jsonstring)
-    }}
-}}
+    }
+}
 
-function _send(jsonstring) {{
-    socket.send(jsonstring)
-}}
-"""
-    
-    
-desktop_template = f"""
-function _toPy(...arguments) {{
-    var func = arguments.shift()
-    var json = {{type: "page",
-                func: func,
-                args: arguments}}
-    json['properties'] = _manageProperties()
-    json['html'] = _getDoc()
-    var jsonstring = JSON.stringify(json)
-    pywebview.api.communicate(jsonstring)
-}}
+async function _getUid() {
+    try {
+        const uid = await pywebview.api.get_uid()
+        return uid
+    } catch (err) {
+        const uid = null
+        return null
+    }
+}
+
+window.addEventListener('pywebviewready', function () {
+    _pywebviewIsLoaded = true
+})
+
+function _waitForPywebview() {
+  return new Promise(function (resolve, reject) {
+    window.addEventListener('pywebviewready', function () {
+      resolve()
+      _pywebviewIsLoaded = true
+    })
+  })
+}
 
-function _send(jsonstring) {{
-    return jsonstring
-}}
-"""
-
-
-common_template = f"""
-_touiFiles = {{}}
+function _send(jsonstring) {
+    socket.send(jsonstring)
+}
 
-function _getDoc() {{
+function _getDoc() {
     var serializer = new XMLSerializer()
     const doc = serializer.serializeToString(document)
     return doc
-    }}
+    }
 
-function _setDoc(kwargs) {{
+function _setDoc(kwargs) {
     document.open()
     document.write(kwargs['doc'])
     document.close()
-    }}
+    }
     
-async function _manageProperties() {{
-    var properties = {{files: []}}
+async function _manageProperties() {
+    var properties = {files: []}
     var input_elements = document.getElementsByTagName("input")
-    for (var input_element of input_elements) {{
+    for (var input_element of input_elements) {
         input_element.setAttribute("value", input_element.value)
-        if (input_element.checked == true) {{
+        if (input_element.checked == true) {
             input_element.setAttribute("checked", "")
-        }} else {{
+        } else {
             input_element.removeAttribute("checked")
-        }}
-    }}
+        }
+    }
     return properties
-}}
+}
 
-async function _getFiles(kwargs) {{
+async function _getFiles(kwargs) {
     var files = []
     var element = _getElement(kwargs['selector'])
-    if (element.type == "file") {{
-        for (var file of element.files) {{
+    if (element.type == "file") {
+        for (var file of element.files) {
             var selector = _getElementSelector(element)
-            var fileJSON = {{name: file.name,
+            var fileJSON = {name: file.name,
                              size: file.size,
-                             type: file.type,
+                             'file-type': file.type,
                              'last-modified': file.lastModified,
-                             selector: selector}}
-            if (kwargs['with_content'] == true) {{
-                await file.text().then(function (text) {{
+                             selector: selector}
+            if (kwargs['with_content'] == true) {
+                await file.text().then(function (text) {
                     fileJSON['content'] = text
-                }})
-            }}
+                })
+            }
             var keys = Object.keys(_touiFiles)
             var newKey = 0
-            if (keys.length != 0) {{
+            if (keys.length != 0) {
                 var lastKey = keys.sort().reverse()[0]
                 const newKey = parseInt(lastKey) + 1
-            }}
+            }
             _touiFiles[newKey.toString()] = file
             fileJSON['file-id'] = newKey.toString()
             files.push(fileJSON)
-        }}
-    }}
-    var jsonString = JSON.stringify({{data: files, type: "files"}})
+        }
+    }
+    var jsonString = JSON.stringify({data: files, type: "files"})
     var dataSent = _send(jsonString)
     return dataSent
-}}
+}
 
-async function _saveFile(kwargs) {{
+async function _saveFile(kwargs) {
     var fileId = kwargs['file-id']
     var file = _touiFiles[fileId]
     var reader = new FileReader()
-    if (kwargs['binary'] == true) {{
-        reader.onload = function () {{
+    if (kwargs['binary'] == true) {
+        reader.onload = function () {
             const buffer = reader.result
             const content = new Uint8Array(buffer)
             const lengthPerPart = 16000
             const charsLength = content.length
-            for (var i = 0; i < charsLength; i += lengthPerPart) {{
+            for (var i = 0; i < charsLength; i += lengthPerPart) {
                 var smallerContent = [...content.slice(i, i + lengthPerPart)]
-                var jsonString = JSON.stringify({{type: "save files",
+                var jsonString = JSON.stringify({type: "save files",
                                                   data: smallerContent,
-                                                  end: false}})
+                                                  end: false})
                 var dataSent = _send(jsonString)
-            }}
-            var jsonString = JSON.stringify({{type: "save files", data: [],
-                                              end: true}})
+            }
+            var jsonString = JSON.stringify({type: "save files", data: [],
+                                              end: true})
             var dataSent = _send(jsonString)
-        }}
+        }
         reader.readAsArrayBuffer(file)
-    }} else {{
-        reader.onload = function () {{
+    } else {
+        reader.onload = function () {
             const content = reader.result
             const lengthPerPart = 16000
             const charsLength = content.length
-            for (var i = 0; i < charsLength; i += lengthPerPart) {{
+            for (var i = 0; i < charsLength; i += lengthPerPart) {
                 var smallerContent = content.substring(i, i + lengthPerPart)
-                var jsonString = JSON.stringify({{type: "save files",
+                var jsonString = JSON.stringify({type: "save files",
                                                   data: smallerContent,
-                                                  end: false}})
+                                                  end: false})
                 var dataSent = _send(jsonString)
-            }}
-            var jsonString = JSON.stringify({{type: "save files", data: "",
-                                              end: true}})
+            }
+            var jsonString = JSON.stringify({type: "save files", data: "",
+                                              end: true})
             var dataSent = _send(jsonString)
-        }}
+        }
         reader.readAsText(file)
-    }}
-}}
+    }
+}
     
-function _getElement(kwargs) {{
+function _getElement(kwargs) {
     var number = 0
-    if ('number' in kwargs) {{
+    if ('number' in kwargs) {
         var number = parseInt(kwargs['number'])
-    }}
-    if ('parent' in kwargs) {{
+    }
+    if ('parent' in kwargs) {
         const parent = _getElement(kwargs['parent'])
         const element = parent.querySelectorAll(kwargs['selector'])[number]
         return element
-    }} else {{
+    } else {
         const elements = document.querySelectorAll(kwargs['selector'])
         const element = elements[number]
         return element
-    }}
-}}
+    }
+}
 
-var _getElementSelector = function(el) {{
+var _getElementSelector = function(el) {
   if (!(el instanceof Element))
             return;
         var path = [];
-        while (el.nodeType === Node.ELEMENT_NODE) {{
+        while (el.nodeType === Node.ELEMENT_NODE) {
             var selector = el.nodeName.toLowerCase();
-            if (el.id) {{
+            if (el.id) {
                 selector += '#' + el.id;
                 path.unshift(selector);
                 break;
-            }} else {{
+            } else {
                 var sib = el, nth = 1;
-                while (sib = sib.previousElementSibling) {{
+                while (sib = sib.previousElementSibling) {
                     if (sib.nodeName.toLowerCase() == selector)
                        nth++;
-                }}
+                }
                 if (nth != 1)
                     selector += ":nth-of-type("+nth+")";
-            }}
+            }
             path.unshift(selector);
             el = el.parentNode;
-        }}
+        }
         path = path.join(" > ");
         return path;
-     }}
+     }
 
-function _replaceElement(kwargs) {{
+function _replaceElement(kwargs) {
     var old_element = _getElement(kwargs['selector'])
     old_element.outerHTML = kwargs['element']
-    }}
+    }
 
-function _replaceElements(kwargs) {{
+function _replaceElements(kwargs) {
     var elements = document.querySelectorAll(kwargs['selectors'])
     var pyelements = kwargs['elements']
-    for (i = 0; i < elements.length; i++) {{
+    for (i = 0; i < elements.length; i++) {
         elements[i].outerHTML = pyelements[i];
-        }}
-    }}
+        }
+    }
     
-function _setAttr(kwargs) {{
+function _setAttr(kwargs) {
     var element = _getElement(kwargs['selector'])
     element.setAttribute(kwargs['name'], kwargs['value'])
-    if (kwargs['name'] == 'value') {{
+    if (kwargs['name'] == 'value') {
         element.value = kwargs['value']
-    }}
-    if (kwargs['name'] == 'checked') {{
+    }
+    if (kwargs['name'] == 'checked') {
         element.checked = kwargs['value']
-    }}
-}}
+    }
+}
 
-function _delAttr(kwargs) {{
+function _delAttr(kwargs) {
     var element = _getElement(kwargs['selector'])
     element.removeAttribute(kwargs['name'])
-    if (kwargs['name'] == 'checked') {{
+    if (kwargs['name'] == 'checked') {
         element.checked = false
-    }}
-}}
+    }
+}
 
-function _setContent(kwargs) {{
+function _setContent(kwargs) {
     var element = _getElement(kwargs['selector'])
     element.innerHTML = kwargs['content']
-}}
+}
 
-function _addContent(kwargs) {{
+function _addContent(kwargs) {
     var element = _getElement(kwargs['selector'])
     element.insertAdjacentHTML("beforeend" ,kwargs['content'])
-}}
+}
 
-function _addScript(kwargs) {{
+function _addScript(kwargs) {
     const script = kwargs['script']
     var new_element = document.createElement('script')
     new_element.innerHTML = script
     document.body.appendChild(new_element)
-    }}
+    }
     
-function _goTo(kwargs) {{
+function _goTo(kwargs) {
     const url = kwargs['url']
-    location.href = location.origin + url
-}}
+    const newTab = kwargs['new']
+    if (newTab == true) {
+        window.open(location.origin + url)
+    } else {
+        window.open(location.origin + url, "_self")
+    }
+}
 
-function _resizeEmbed(element) {{
+function _resizeEmbed(element) {
     element.height = 0
     element.width = 0
     element.style.height = element.contentWindow.document.body.scrollHeight + 1 + 'px'
     element.style.width = element.contentWindow.document.body.scrollWidth + 1 + 'px'
-}}
+}
 
-function _findAndExecute(jsonString) {{
+function _findAndExecute(jsonString) {
     var instructions = JSON.parse(jsonString)
     var func = instructions['func']
     var kwargs = instructions['kwargs']
-    if (func == "_replaceElement") {{
+    if (func == "_replaceElement") {
         _replaceElement(kwargs)
-    }}
-    if (func == "_replaceElements") {{
+    }
+    if (func == "_replaceElements") {
         _replaceElements(kwargs)
-    }}
-    if (func == "_setAttr") {{
+    }
+    if (func == "_setAttr") {
         _setAttr(kwargs)
-    }}
-    if (func == "_delAttr") {{
+    }
+    if (func == "_delAttr") {
         _delAttr(kwargs)
-    }}
-    if (func == "_setContent") {{
+    }
+    if (func == "_setContent") {
         _setContent(kwargs)
-    }}
-    if (func == "_addContent") {{
+    }
+    if (func == "_addContent") {
         _addContent(kwargs)
-    }}
-    if (func == "_setDoc") {{
+    }
+    if (func == "_setDoc") {
         _setDoc(kwargs)
-    }}
-    if (func == "_addScript") {{
+    }
+    if (func == "_addScript") {
         _addScript(kwargs)
-    }}
-    if (func == "_goTo") {{
+    }
+    if (func == "_goTo") {
         _goTo(kwargs)
-    }}
-    if (func == "_getFiles") {{
+    }
+    if (func == "_getFiles") {
         _getFiles(kwargs)
-    }}
-    if (func == "_saveFile") {{
+    }
+    if (func == "_saveFile") {
         _saveFile(kwargs)
-    }}
-}}"""
+    }
+}"""
 
 def custom_func(name):
     text = f"""
     function {name}(...args) {{
         _toPy('{name}', ...args)
     }}
     """
     return text
 
 
-def get_script(app_type='web'):
-    if app_type == "desktop":
-        template = desktop_template
-    else:
-        template = web_template
-    script = template + common_template
+def get_script(app_type='Website'):
+    script = template.replace('{app_type}', app_type)
     return script
```

### Comparing `toui-1.2.0a1/toui/_signals.py` & `toui-2.0.0/toui/_signals.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,34 +9,33 @@
 
 
 class Signal:
 
     included_private_methods = ["_open_another_page"]
     no_return_functions = []
 
-    def __init__(self, return_type=None):
+    def __init__(self, return_type=None, app_types=['Website', 'DesktopApp']):
         self.ws = None
         self.return_type = return_type
+        self.app_types = app_types
 
     def __call__(decorator, func):
         decorator._func = func
         @wraps(func)
         def new_func(self, *args, **kwargs):
             decorator.object = self
             if self._signal_mode:
                 original_copy = copy(self)
             value = decorator._func(self, *args, **kwargs)
             real_output = value
-            if self._signal_mode:
+            if self._signal_mode and self._app.__class__.__name__ in decorator.app_types:
                 if self.__class__.__name__ == 'Element':
                     decorator.ws = self._parent_page.__dict__.get("_ws")
-                    decorator.evaluate_js = self._parent_page._evaluate_js
                 elif self.__class__.__name__ == "Page":
                     decorator.ws = self.__dict__.get("_ws")
-                    decorator.evaluate_js = self._evaluate_js
                 kwargs = inspect.signature(decorator._func).bind(self, *args, **kwargs)
                 kwargs.apply_defaults()
                 kwargs = kwargs.arguments
                 kwargs['return_value'] = value
                 kwargs['object'] = kwargs['self']
                 kwargs['original_copy'] = original_copy
                 del kwargs['self']
@@ -55,46 +54,31 @@
                 signal = method(**kwargs)
                 if signal:
                     return self._send(signal)
                 else:
                     return
 
     def _send(self, signal):
-        if self.ws:
-            self.ws.send(json.dumps(signal))
-            debug(f"SENT: {signal}")
-            if self.return_type == "js":
-                data_from_js = self.ws.receive()
-                debug(f"DATA RECEIVED")
-                data_validation = self.object._app._validate_data(data_from_js)
-                if not data_validation:
-                    info("Data validation returns `False`. The data will not be used.")
-                    return
-                data_dict = json.loads(data_from_js)
-                debug(f"RECEIVED DATA KEYS: {list(data_dict.keys())}")
-                if data_dict['type'] == "files":
-                    files = []
-                    for file_dict in data_dict['data']:
-                        files.append(File(file_dict, signal, self.object._app, file_dict['file-id'], ws=self.ws))
-                    return files
-                return data_dict['data']
-        else:
-            out = self.evaluate_js(func=signal['func'], kwargs=signal['kwargs'])
-            debug(f"SENT: {signal}")
-            if self.return_type == "js":
-                try:
-                    data_dict = json.loads(out)
-                    debug(f"DATA RECEIVED")
-                    if data_dict['type'] == "files":
-                        files = []
-                        for file_dict in data_dict['data']:
-                            files.append(File(file_dict, signal, self.object._app, file_dict['file-id'], ws=None))
-                        return files
-                except: data_dict = {"data": None}
-                return data_dict['data']
+        self.ws.send(json.dumps(signal))
+        debug(f"SENT: {signal}")
+        if self.return_type == "js":
+            data_from_js = self.ws.receive()
+            debug(f"DATA RECEIVED")
+            data_validation = self.object._app._validate_data(data_from_js)
+            if not data_validation:
+                info("Data validation returns `False`. The data will not be used.")
+                return
+            data_dict = json.loads(data_from_js)
+            debug(f"RECEIVED DATA KEYS: {list(data_dict.keys())}")
+            if data_dict['type'] == "files":
+                files = []
+                for file_dict in data_dict['data']:
+                    files.append(File(file_dict, signal, self.object._app, file_dict['file-id'], ws=self.ws))
+                return files
+            return data_dict['data']
 
 
 class File:
     """
     Contains the information of an uploaded file and can be used to save the file contents.
 
     This object should only be created through `Element.get_files()` method.
@@ -106,14 +90,19 @@
 
     type
         Type of the file.
 
     size
         Size of the file.
 
+    content: str or None
+        Content of the file. If the parameter `with_contents` in the method `Element.get_files` was set as ``True``,
+        you will be able to access the content using this attribute. Otherwise, the value of this attribute will be
+        ``None``.
+
     last_modified
         The last modified date as the number of milliseconds since the Unix epoch (January 1, 1970 at midnight).
 
     is_binary: bool
         Set the value of this attribute to ``True`` only if you want the file content to be converted to bytes
         before saving it.
 
@@ -122,57 +111,47 @@
     Element.get_files()
 
     """
     def __init__(self, file_dict, signal, app, file_id, ws=None):
         self._file_dict = file_dict
         self.name = self._file_dict['name']
         self.size = self._file_dict['size']
-        self.type = self._file_dict['type']
+        self.type = self._file_dict['file-type']
+        self.content = None
+        if "content" in self._file_dict:
+            self.content = self._file_dict['content']
         self.last_modified = self._file_dict['last-modified']
         self._ws = ws
         self._id = file_id
         self._app = app
         self._signal = signal
         self.is_binary = False
 
     def __iter__(self):
         js_func = "_saveFile"
         js_args = []
         js_kwargs = {}
         js_kwargs['file-id'] = self._id
         js_kwargs['binary'] = self.is_binary
         signal = {'func': js_func, 'args': js_args, 'kwargs': js_kwargs}
-        if self._ws:
-            self._ws.send(json.dumps(signal))
-            debug(f"SENT: {signal}")
-            while True:
-                data_from_js = self._ws.receive()
-                data_validation = self._app._validate_data(data_from_js)
-                if not data_validation:
-                    info("Data validation returns `False`. The data will not be used.")
-                    return
-                data_dict = json.loads(data_from_js)
-                data = data_dict['data']
-                if self.is_binary:
-                    data = bytearray(data)
-                yield data
-                if data_dict['end'] == True:
-                    break
-        else:
-            out = self._signal.evaluate_js(func=signal['func'], kwargs=signal['kwargs'])
-            debug(f"SENT: {signal}")
-            while True:
-                data_from_js = out
-                data_dict = json.loads(data_from_js)
-                data = data_dict['data']
-                if self.is_binary:
-                    data = bytearray(data)
-                yield data
-                if data_dict['end'] == True:
-                    break
+        self._ws.send(json.dumps(signal))
+        debug(f"SENT: {signal}")
+        while True:
+            data_from_js = self._ws.receive()
+            data_validation = self._app._validate_data(data_from_js)
+            if not data_validation:
+                info("Data validation returns `False`. The data will not be used.")
+                return
+            data_dict = json.loads(data_from_js)
+            data = data_dict['data']
+            if self.is_binary:
+                data = bytearray(data)
+            yield data
+            if data_dict['end'] == True:
+                break
 
     def __repr__(self):
         return f"<File {self.name}>"
 
     def save(self, stream):
         """
         Saves the contents of the file to a stream.
```

### Comparing `toui-1.2.0a1/toui/apps.py` & `toui-2.0.0/toui/apps.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,178 +1,140 @@
 """
 A module that creates web apps and desktop apps.
 """
 import __main__
-from flask import Flask, session, request
-from flask_sock import Sock
-from flask_login import LoginManager, UserMixin, current_user, login_user, logout_user
-from flask_sqlalchemy import SQLAlchemy
-import webview
+import threading
 import json
 import inspect
 import time
 import os
 from copy import copy
 from abc import ABCMeta, abstractmethod
-from flask_basicauth import BasicAuth
+from collections.abc import MutableMapping
+from functools import wraps
+from typing import Any
+from flask import Flask, session, request, send_file
+from flask_sock import Sock
+from flask_caching import Cache
+import webview
 from toui._helpers import warn, info, debug, error
 from toui.pages import Page
-from toui.exceptions import ToUIWrongPlaceException
+from toui.exceptions import ToUIWrongPlaceException, ToUINotAddedError
 from toui._defaults import validate_ws, validate_data
 
+_imported_optional_reqs = {'flask-login':False,
+                          'flask-sqlalchemy':False,
+                          'flask-basicauth':False}
+
+try:
+    from flask_login import LoginManager, UserMixin, current_user, login_user, logout_user, AnonymousUserMixin
+    _imported_optional_reqs['flask-login'] = True
+except ModuleNotFoundError: pass
+
+try:
+    from flask_sqlalchemy import SQLAlchemy
+    _imported_optional_reqs['flask-sqlalchemy'] = True
+except ModuleNotFoundError: pass
+
+try:
+    from flask_basicauth import BasicAuth
+    _imported_optional_reqs['flask-basicauth'] = True
+except ModuleNotFoundError: pass
+
+
+class _ReqsChecker:
+
+    def __init__(self, reqs) -> None:
+        self.reqs = reqs
+
+    def __call__(self, func) -> Any:
+        @wraps(func)
+        def new_func(*args, **kwargs):
+            for req in self.reqs:
+                if _imported_optional_reqs[req]:
+                    return func(*args, **kwargs)
+                else:
+                    raise ModuleNotFoundError(f"You have not installed the optional package `{req}` yet, to install it run:\n\tpip install {req}")
+        return new_func
+
 
 class _App(metaclass=ABCMeta):
     """The base class for DesktopApp and Website"""
 
-    def _add_function(self, func):
-        name = func.__name__
-        if not callable(func):
-            warn(f"Variable '{name}' is not a function.")
-            return
-        if name.startswith("_"):
-            warn(f"Function '{name}' starts with '_'. It is safer to avoid functions that starts with '_'"
-                 f"because they might overlap with functions used by the package.")
-        if self._func_exists(name):
-            warn(f"Function '{name}' exists.")
-        self._functions[name] = func
-
-    @abstractmethod
-    def add_pages(self): pass
-
-    @abstractmethod
-    def open_new_page(self, url): pass
-
-    @abstractmethod
-    def get_user_page(self): pass
-
-    @abstractmethod
-    def user_vars(self): pass
-
-    @abstractmethod
-    def _communicate(self): pass
-
-    @abstractmethod
-    def run(self): pass
-
-    def _add_functions(self, *functions):
-        for func in functions:
-            self._add_function(func)
-
-    def _get_functions(self):
-        """Gets all added functions in this class. This is a private function."""
-        return self._functions
-
-    def _func_exists(self, func_name: str):
-        """Checks if a function exists. This is a private function."""
-        if func_name in self._get_functions().keys():
-            return True
-        else:
-            return False
-
-    def _call_func(self, func_name, *args, page=None):
-        """Calls a function in this class. Its return value depends on the function called. This is a private function."""
-        functions = self._get_functions()
-        info(f'"{func_name}" called')
-        if page:
-            func = _FuncWithPage(functions[func_name], page)
-            return func(*args)
-        return functions[func_name](*args)
-
-
-class _FuncWithPage:
-    def __init__(self, func, page):
-        self.func = func
-        self.page = page
-    def __call__(self, *args, **kwargs):
-        return self.func(*args, **kwargs)
-
-        
-class Website(_App):
-    """
-    A class that creates a web application from HTML files.
-
-    Attributes
-    ----------
-    flask_app: Flask
-        ToUI creates web applications using `Flask`. You can access the `Flask` object using the attribute `flask_app`.
-
-    forbidden_urls: list
-        These are URLs that ToUI does not allow the user to use because ToUI uses them.
-
-    user_vars: dict
-        A dictionary that stores data unique to each user. The data are stored in a `flask` `session` object.
-
-    pages: list
-        A list of added `Page` objects.
-
-    Examples
-    --------
-
-    Creating a web app:
-
-    >>> from toui import Website
-    >>> app = Website(__name__, secret_key="some key")
-
-    Creating a page and adding it to the app:
-
-    >>> from toui import Page
-    >>> home_page = Page(html_str="<h1>This is the home page</h1>")
-    >>> app.add_pages(home_page)
-
-    Running the app:
-
-    >>> if __name__ == "__main__":
-    ...     app.run(debug=True) # doctest: +SKIP
-
-    See Also
-    --------
-    :py:class:`toui.pages.Page`
-    :py:class:`DesktopApp`
-
-    """
-    
     def __init__(self, name=None, assets_folder=None, secret_key=None):
         """
 
         Parameters
         ----------
         name: str (optional)
             The name of the app.
 
         assets_folder: str (optional)
             The path to the folder that contains the HTML files and other assets.
 
         secret_key: str (optional)
             Sets the `secret_key` attribute for `flask.Flask`
 
+            
+        Attributes
+        ----------
+        flask_app: Flask
+            ToUI creates applications using `Flask`. You can access the `Flask` object using the attribute `flask_app`.
+
+        forbidden_urls: list
+            These are URLs that ToUI does not allow the user to use because ToUI uses them.
+
+        user_vars: dict
+            A dictionary that stores temporary data unique to each user. The data are stored in a `Cache` object from `flask-caching`
+            package.
+
+        pages: list
+            A list of added `Page` objects.
+
+
+        .. admonition:: Behind The Scenes
+            :class: tip
+            
+            ToUI uses `Flask` and its extenstions to create apps. When creating an instance of this class, the following
+            extensions are used:
+
+            - `Sock` class extension from `Flask-Sock` package.
+            - `Cache` class extension from `Flask-Cache` package.
+
+            The following `Flask` configurations are also set:
+
+            - `CACHE_TYPE = "SimpleCache"`
+
         """
         self._functions = {}
         if not name:
             if hasattr(__main__, "__file__"):
                 name = os.path.basename(__main__.__file__).split(".")[0]
             else:
                 name = "app"
         if not assets_folder:
             assets_folder = "/"
         self.flask_app = Flask(name, static_folder=assets_folder, static_url_path="/")
         if secret_key is None:
             warn("No secret key was set. Generating a random secret key for Flask.")
             secret_key = os.urandom(50)
         self.flask_app.secret_key = secret_key
-        self._socket = Sock(self.flask_app)
         self.pages = []
-        self._socket.route("/toui-communicate")(self._communicate)
-
-        self.forbidden_urls = ['/toui-communicate']
+        self._add_communication_method()
+        self._add_user_vars()
+        self.flask_app.route("/toui-download-<path_id>", methods=['POST', 'GET'])(self._download)
+        self.forbidden_urls = ['/toui-communicate', "/toui-download-<path_id>"]
         self._validate_ws = validate_ws
         self._validate_data = validate_data
         self._auth = None
-        self._default_vars = {}
         self._user_cls = None
 
+    @abstractmethod
+    def run(self): pass
+
     def add_pages(self, *pages, do_copy=False, blueprint=None, endpoint=None):
         """
         Adds pages to the app.
 
         Parameters
         ----------
         pages: list(Page)
@@ -192,32 +154,32 @@
             
         """
         for page in pages:
             if page.url in self.forbidden_urls:
                 warn(f"The URL '{page.url}' is not allowed and might cause errors.")
             if do_copy:
                 page = copy(page)
-            page._add_script()
             page._app = self
+            page._add_script()
             self.pages.append(page)
             view_func = page._view_func
             if self._auth:
                 view_func = self._auth.required(view_func)
             if not endpoint:
-                endpoint = str(id(page))
+                endpoint_ = str(id(page))
+            else:
+                endpoint_ = endpoint
             if blueprint:
-                route = blueprint.route(page.url, methods=['GET', 'POST'], endpoint=endpoint)(view_func)
+                route = blueprint.route(page.url, methods=['GET', 'POST'], endpoint=endpoint_)(view_func)
             else:
-                route = self.flask_app.route(page.url, methods=['GET', 'POST'], endpoint=endpoint)(view_func)
-            for func in page._functions.values():
-                self._add_functions(func)
+                route = self.flask_app.route(page.url, methods=['GET', 'POST'], endpoint=endpoint_)(view_func)
 
-    def open_new_page(self, url):
+    def open_new_page(self, url, new=False):
         """
-        Redirects to another URL.
+        Opens another URL.
 
         This function should only be called after the app starts running.
 
         Parameters
         ----------
         url: str
             URL of the new page.
@@ -225,140 +187,120 @@
         Returns
         -------
         None
 
         """
         try:
             session.keys()
-            self.get_user_page()._open_another_page(url)
+            self.get_user_page()._open_another_page(url, new=new)
         except RuntimeError:
-            raise ToUIWrongPlaceException(f"The function `{inspect.currentframe().f_code.co_name}` should only be called after the app runs.")
+            raise ToUIWrongPlaceException(f"The function `open_new_page` should only be called after the app runs.")
 
-    def get_user_page(self):
+    @staticmethod
+    def get_user_page() -> Page:
         """
-        Returns the current `Page`.
+        A static method that returns the current `Page`.
 
         This function should only be called after the app starts running.
 
         Returns
         -------
         pg: Page
 
         """
         try:
-            pg = session['user page']
-            return pg
+            return session['user page']
         except RuntimeError as e:
-            raise ToUIWrongPlaceException(f"The function `{inspect.currentframe().f_code.co_name}` should only be called after the app runs.")
+            raise ToUIWrongPlaceException(f"The function `get_user_page` should only be called after the app runs.")
 
-    def run(self, *args, **kwargs):
-        """
-        Runs the app. It calls the function `flask.Flask.run`. The arguments will be passed to
-        `flask.Flask.run` function.
+    @property
+    def user_vars(self):
+        """Gets user-specific variables."""
+        return self._user_vars
 
+    def download(self, filepath, new=True):
+        """
+        Downloads a file from the server to a client.
+        
         Parameters
         ----------
-        args: Any
+        filepath: str
+            The path to the file (on the server).
 
-        kwargs: Any
+        new: bool, default=True
+            Opens new tab/window when downloading file.
 
         """
-        self.flask_app.run(*args, **kwargs)
-
-    @property
-    def user_vars(self):
-        session_exists = self._session_check()
-        if session_exists:
-            return session['variables']
-        else:
-            return self._default_vars
-
-    def _session_check(self):
-        """This is a private function."""
-        try:
-            session.keys()
-        except RuntimeError as e:
-            return False
-        if not "variables" in session.keys():
-            session['variables'] = self._default_vars
-        if not "user page" in session.keys():
-            session['user page'] = None
-        return True
+        path_id = 0
+        while self._cache.get(f'toui-download-{path_id}'):
+            path_id += 1
+        self._cache.set(f'toui-download-{path_id}', filepath)
+        self.open_new_page(f"/toui-download-{path_id}", new=new)
 
-    def _communicate(self, ws):
-        """This is a private function."""
-        validation = self._validate_ws(ws)
-        if not validation:
-            info("WebSocket validation returns `False`. No data should be sent or received.")
-            return
-        info(f'WebSocket connected: {ws.connected}')
-        while True:
-            data_from_js = ws.receive()
-            data_validation = self._validate_data(data_from_js)
-            if not data_validation:
-                info("Data validation returns `False`. The data will not be used.")
-                continue
-            debug(data_from_js)
-            s = time.time()
-            self._session_check()
-            data_dict = json.loads(data_from_js)
-            func = data_dict['func']
-            args = data_dict['args']
-            url = data_dict['url']
-            new_html = data_dict['html']
-            new_page = Page(url=url)
-            new_page.from_str(new_html)
-            new_page._app = self
-            new_page._signal_mode = True
-            new_page._ws = ws
-            session['user page'] = new_page
-            if self._func_exists(func):
-                self._call_func(func, *args)
-            del session['user page']
-            e = time.time()
-            debug(f"TIME: {e - s}s")
-
-    def create_user_database(self, database_uri):
+    @_ReqsChecker(['flask-sqlalchemy', 'flask-login'])
+    def add_user_database(self, database_uri, other_columns=[], user_cls=None):
         """
-        Connects to a database that has data specific to each user.
+        Creates a simple database that has data specific to each user.
 
-        The database is a table that contains the following columns: `username`, `password`, and `id`.
+        The database is a table that contains the following columns: `username`, `password`, and `id`. To add other columns,
+        add their names in `other_columns` list.
 
         Parameters
         ----------
-        database_uri
+        database_uri: str
+            The URI of the database that you want to connect to.
+
+        other_columns: list
+            The names of table columns other than `username`, `password`, and `id`.
+
+        user_cls: Callable, default=None
+            If this parameter is ``None``, a table called `User` will be created. However, if this parameter was set, the
+            table `User` will not be created and the parameter `user_cls` will be used instead.
 
-        Returns
-        -------
+
+        .. admonition:: Behind The Scenes
+            :class: tip
+            
+            The following flask extensions are used when calling this function:
+
+            - `SQLAlchemy` class extension from `Flask-SQLAlchemy` package.
+            - `LoginManager` class extension from `Flask-Login` package.
+
+            The following `Flask` configurations are also set:
+
+            - `SQLALCHEMY_DATABASE_URI = database_uri`
 
         """
         self.flask_app.config['SQLALCHEMY_DATABASE_URI'] = database_uri
         self._db = SQLAlchemy(self.flask_app)
         self._login_manager = LoginManager(self.flask_app)
         self._load_user = self._login_manager.user_loader(self._load_user)
-        class User(UserMixin, self._db.Model):
-            __tablename__ = "user"
-
-            id = self._db.Column(self._db.Integer, primary_key=True)
-            username = self._db.Column(self._db.String(80), unique=True, nullable=False)
-            password = self._db.Column(self._db.String(300), nullable=False, unique=True)
-
-            def __repr__(self):
-                return f'<User {self.username}>'
+        if not user_cls:
+            class User(UserMixin, self._db.Model):
+                __tablename__ = "user"
+
+                id = self._db.Column(self._db.Integer, primary_key=True)
+                username = self._db.Column(self._db.String, nullable=False, unique=True)
+                password = self._db.Column(self._db.String, nullable=False, unique=False)
+
+                def __repr__(self):
+                    return f'<User {self.username}>'
+            for col in other_columns:
+                setattr(User, col, self._db.Column(self._db.String))
+        else:
+            User = user_cls
         self._user_cls = User
         with self.flask_app.app_context():
             self._db.create_all()
 
-    def _load_user(self, user_id):
-        return self._user_cls.get(int(user_id))
-
     # Website-specific methods
-    def get_request(self):
+    @staticmethod
+    def get_request():
         """
-        Gets data sent from client using HTTP request.
+        A static method that gets data sent from client using HTTP request.
 
         This method returns the `request` object of `Flask`. The `request` object has some useful attributes such as
         `request.files` which retrieves uploaded files.
 
         Examples
         --------
         To use this method, first create the app and a page:
@@ -395,58 +337,139 @@
             https://flask.palletsprojects.com/en/2.2.x/api/#flask.request
 
         Page.on_url_request
 
         """
         return request
 
-    def signup_user(self, username, password):
-        if self._user_cls is None:
-            raise Exception("You have not created the user database yet.")
+    @_ReqsChecker(['flask-sqlalchemy', 'flask-login'])
+    def signup_user(self, username, password, **other_info):
+        """
+        Creates a new user in the database.
+        
+        Parameters
+        ----------
+        username: str
+
+        password: str
+
+        other_info
+            Other information required for signing up.
+
+        Returns
+        -------
+        bool
+            ``True`` if the user is created, and ``False`` if it is not created.
+
+        """
+        self._confirm_user_database_created()
         if self.username_exists(username):
-            return
-        new_user = self._user_cls(username=username, password=password)
+            return False
+        new_user = self._user_cls(username=username, password=password, **other_info)
         self._db.session.add(new_user)
         self._db.session.commit()
-        login_user(new_user)
+        if self.username_exists(username):
+            return True
+        else:
+            return False
 
-    def signin_user(self, username, password):
-        if self._user_cls is None:
-            raise Exception("You have not created the user database yet.")
-        user = self._user_cls.query.filter_by(username=username, password=password).first()
+    @_ReqsChecker(['flask-sqlalchemy', 'flask-login'])
+    def signin_user(self, username, password, **other_info):
+        """
+        Loads the data of a user from database.
+
+        Parameters
+        ----------
+        username: str
+
+        password: str
+
+        other_info
+            Other information required for signing in.
+
+        Returns
+        -------
+        bool
+            ``True`` if the user is signed in, and ``False`` if it is not signed in.
+
+        """
+        self._confirm_user_database_created()
+        user = self._user_cls.query.filter_by(username=username, password=password, **other_info).first()
         if user:
             login_user(user)
+            return True
+        else:
+            return False
 
-    def signout_user(self):
+    @staticmethod
+    @_ReqsChecker(['flask-login'])
+    def signout_user():
+        """
+        A static method that signs out the current user.
+        """
         logout_user()
 
+    @_ReqsChecker(['flask-sqlalchemy'])
     def username_exists(self, username):
-        if self._user_cls is None:
-            raise Exception("You have not created the user database yet.")
+        """
+        Checks if the username is exists in the database.
+        
+        Parameters
+        ----------
+        username: str
+        
+        Returns
+        -------
+        bool
+            ``True`` if the username exists, otherwise ``False``.
+            """
+        self._confirm_user_database_created()
         if self._user_cls.query.filter_by(username=username).first():
-            info("User exists")
+            info(f"User {username} exists")
             return True
         else:
             return False
 
-    def get_current_user(self):
-        return current_user
+    @staticmethod
+    @_ReqsChecker(['flask-login'])
+    def get_current_user():
+        """
+        A static method that returns the current user.
+        """
+        if isinstance(current_user, AnonymousUserMixin):
+            return None
+        else:
+            return current_user
 
-    def set_restriction(self, username, password):
+    @_ReqsChecker(['flask-basicauth'])
+    def add_restriction(self, username, password):
         """
         Makes the app private.
 
         Adds a username and password to the app.
 
         Parameters
         ----------
         username: str
 
         password: str
 
+
+        .. admonition:: Behind The Scenes
+            :class: tip
+            
+            When calling this method, the following `Flask` extension is used:
+
+            - `BasicAuth` class extension from `Flask-BasicAuth` package.
+
+            The following `Flask` configurations are also set:
+
+            - `BASIC_AUTH_USERNAME = username`
+            - `BASIC_AUTH_PASSWORD = password`
+
         """
         self._auth = BasicAuth(self.flask_app)
         self.flask_app.config['BASIC_AUTH_USERNAME'] = username
         self.flask_app.config['BASIC_AUTH_PASSWORD'] = password
 
     def set_ws_validation(self, func):
         """
@@ -478,47 +501,27 @@
         Validate data received from JavaScript before using it.
 
         ToUI receives data from JavaScript in the form of a JSON object. To validate this data
         before allowing ToUI to use it, input a function that checks the data. This function
         should have one argument `data` and should either return ``True`` or ``False``.
         If the function returns ``False``, the data will not be used by ToUI.
 
-        Currently, there are two types of JSON objects that ToUI receives.
-        One of the JSON objects contains the following keys:
-
-        {type: 'page',
-         func: ...,
-         args: ...,
-         url: ...,
-         html: ...}
-
-        `type` is the type of JSON object, and it always has the value 'page' when JavaScript sends the HTML document
-        as data. `func` contains the name of the Python function that should be called, `args` are the
-        arguments of this function, `url` is the URL of the HTML page that sent the data, 'html'
-        is the HTML document itself as a string.
-
-        Another type of JSON object is a JSON that contains uploaded files:
-
-        {type: 'files',
-         files: ...}
-
-        You can get the uploaded files using the method `Element.get_files()`.
-
-        However, note that the structures of the JSON objects might change in future versions of
-        ToUI.
+        You can check the structures of the data received from JavaScript in
+        https://toui.readthedocs.io/en/latest/how_it_works.html#instructions-sent-and-received.
+        Note that the structures of the JSON objects might change in future versions of ToUI.
 
         Parameters
         ----------
         func: Callable
             A function that validates data received from JavaScript. It should have one argument
             `data` and should either return ``True`` or ``False``.
 
         See Also
         --------
-        Website.set_ws_validation
+        set_ws_validation
 
         """
         self._validate_data = func
 
     def register_toui_blueprint(self, blueprint, **options):
         """
         Registers a `ToUIBlueprint` object. It is similar to `Flask.register_blueprint`.
@@ -535,191 +538,226 @@
         toui.structure.ToUIBlueprint
         flask.Blueprint
 
         """
         self.add_pages(*blueprint.pages, blueprint=blueprint)
         self.flask_app.register_blueprint(blueprint=blueprint, **options)
 
+    def _add_communication_method(self):
+        self._socket = Sock(self.flask_app)
+        self._socket.route("/toui-communicate")(self._communicate)
 
-class _DesktopAppApi:
+    def _add_user_vars(self):
+        self.flask_app.config["CACHE_TYPE"] = "SimpleCache"
+        self._cache = Cache(self.flask_app)
+        self._user_vars = _UserVars(self._cache)
 
-    def __init__(self, app):
-        self.app = app
+    def _session_check(self):
+        """This is a private function."""
+        try:
+            session.keys()
+        except RuntimeError as e:
+            return False
+        if not "user page" in session.keys():
+            session['user page'] = None
+        return True
+    
+    def _download(self, path_id):
+        debug(f"PATH: {path_id}")
+        file_to_download = self._cache.get(f'toui-download-{path_id}')
+        debug(f"File to download: {file_to_download}")
+        if file_to_download:
+            return send_file(file_to_download, as_attachment=True)
 
-    def communicate(self, data_from_js):
-        self.app._communicate(data_from_js, self.window)
+    def _communicate(self, ws):
+        """This is a private function."""
+        validation = self._validate_ws(ws)
+        if not validation:
+            info("WebSocket validation returns `False`. No data should be sent or received.")
+            return
+        info(f'WebSocket connected: {ws.connected}')
+        while True:
+            data_from_js = ws.receive()
+            data_validation = self._validate_data(data_from_js)
+            if not data_validation:
+                info("Data validation returns `False`. The data will not be used.")
+                continue
+            s = time.time()
+            self._session_check()
+            data_dict = json.loads(data_from_js)
+            func = data_dict['func']
+            args = data_dict['args']
+            url = data_dict['url']
+            new_html = data_dict['html']
+            new_page = Page(url=url)
+            new_page.from_str(new_html)
+            new_page._app = self
+            new_page._signal_mode = True
+            new_page._ws = ws
+            new_page._inherit_functions()
+            if "uid" in data_dict:
+                new_page._uid = data_dict['uid']
+            session['user page'] = new_page
+            if new_page._func_exists(func):
+                new_page._call_func(func, *args)
+            del session['user page']
+            e = time.time()
+            debug(f"TIME: {e - s}s")
 
+    def _confirm_user_database_created(self):
+        if self._user_cls is None:
+            raise ToUINotAddedError("You have not created the user database yet. To create it, call the method: `add_user_database`.")
 
-class DesktopApp(_App):
-    """
-    A class that creates a desktop application from HTML files.
+    def _load_user(self, user_id):
+        return self._user_cls.get(int(user_id))
 
-    Attributes
-    ----------
-    name: str
-        The name of the app
 
-    pages: list
-        A list of added `Page` objects.
+class _FuncWithPage:
+    """Currently this class is unused, but it might be used later."""
+    def __init__(self, func, page):
+        self.func = func
+        self.page = page
+    def __call__(self, *args, **kwargs):
+        return self.func(*args, **kwargs)
+
+
+class _UserVars(MutableMapping):
+    """User-specific variables"""
+
+    def __init__(self, cache) -> None:
+        self._cache = cache
+        self._cache.set('toui-vars', {})
 
-    user_vars: dict
-        A normal dictionary. It was created only to make the API for the `Website` class and
-        `DesktopApp` class similar.
+    def __getitem__(self, key):
+        return self._cache.get('toui-vars')[key]
+    
+    def __setitem__(self, key, value):
+        toui_vars = self._cache.get('toui-vars')
+        toui_vars[key] = value
+        self._cache.set('toui-vars', toui_vars)
+
+    def __delitem__(self, key: Any) -> None:
+        toui_vars = self._cache.get('toui-vars')
+        del toui_vars[key]
+        self._cache.set('toui-vars', toui_vars)
+
+    def __iter__(self):
+        for key in self._cache.get('toui-vars'):
+            yield key
+
+    def __len__(self) -> int:
+        return len(self._cache.get('toui-vars'))
+    
+    def __getattr__(self, name: str) -> Any:
+        return getattr(self._cache.get('toui-vars'), name)
+    
+    def __repr__(self) -> str:
+        return repr(self._cache.get('toui-vars'))
+    
+
+class Website(_App):
+    """
+    A class that creates a web application from HTML files.
 
     Examples
     --------
 
-    Creating a desktop app:
+    Creating a web app:
 
-    >>> from toui import DesktopApp
-    >>> app = DesktopApp("MyApp")
+    >>> from toui import Website
+    >>> app = Website(__name__, secret_key="some key")
 
     Creating a page and adding it to the app:
 
     >>> from toui import Page
     >>> home_page = Page(html_str="<h1>This is the home page</h1>")
     >>> app.add_pages(home_page)
 
     Running the app:
 
     >>> if __name__ == "__main__":
-    ...     app.run() # doctest: +SKIP
+    ...     app.run(debug=True) # doctest: +SKIP
 
     See Also
     --------
     :py:class:`toui.pages.Page`
-    :py:class:`Website`
+    :py:class:`DesktopApp`
 
     """
-    def __init__(self, name="App", assets_folder=None):
+
+    @wraps(Flask.run)
+    def run(self, *args, **kwargs):
         """
+        Runs the app. It calls the function `flask.Flask.run`. The arguments will be passed to
+        `flask.Flask.run` function.
 
         Parameters
         ----------
-        name: str
-            The name of the app.
+        args: Any
 
-        """
-        self.name = name
-        self.pages = []
-        if not assets_folder:
-            assets_folder = "."
-        self._assets_folder = assets_folder
-        self._variables = {}
-        self._functions = {}
-        self._is_running = False
+        kwargs: Any
 
-    def add_pages(self, *pages, do_copy=False):
         """
-        Adds pages to the app.
-
-        Parameters
-        ----------
-        pages: list(Page)
-            List of `Page` objects.
+        self.flask_app.run(*args, **kwargs)
 
-        do_copy: bool, default = False
-            If ``True``, the `Page` will be copied before adding to the app.
 
-        """
-        for page in pages:
-            if do_copy:
-                page = copy(page)
-            page._add_script("desktop")
-            page._app = self
-            self.pages.append(page)
-            for func in page._functions.values():
-                self._add_functions(func)
+class DesktopApp(_App):
+    """
+    A class that creates a desktop application from HTML files.
 
-    def open_new_page(self, url):
-        """
-        Opens a new window that has the specified URL.
 
-        This function should only be called after the app starts running.
+    Examples
+    --------
 
-        Parameters
-        ----------
-        url: str
-            URL of the new page.
+    Creating a desktop app:
 
-        Returns
-        -------
-        None
+    >>> from toui import DesktopApp
+    >>> app = DesktopApp("MyApp")
 
-        """
-        for p in self.pages:
-            if p.url == url:
-                api = _DesktopAppApi(self)
-                p._create_window(name=self.name, api=api, assets_folder=self._assets_folder)
+    Creating a page and adding it to the app:
 
-    def get_user_page(self):
-        """
-        Returns the current `Page`.
+    >>> from toui import Page
+    >>> home_page = Page(html_str="<h1>This is the home page</h1>")
+    >>> app.add_pages(home_page)
 
-        This function should only be called after the app starts running.
+    Running the app:
 
-        Returns
-        -------
-        pg: Page
+    >>> if __name__ == "__main__":
+    ...     app.run() # doctest: +SKIP
 
-        """
-        if not self._is_running:
-            raise ToUIWrongPlaceException(f"The function `get_user_page` should only be called after the app runs.")
-        func_frame = inspect.currentframe()
-        func_type = type(None)
-        while func_type is not _FuncWithPage:
-            func_frame = func_frame.f_back
-            if "self" in func_frame.f_locals:
-                func_type = func_frame.f_locals['self'].__class__
-            if func_frame is None:
-                raise Exception("Could not find page. Perhaps `get_user_page` was not called within a function"
-                                "called by HTML event?")
-        page = func_frame.f_locals['self'].page
-        return page
+    See Also
+    --------
+    :py:class:`toui.pages.Page`
+    :py:class:`Website`
 
-    @property
-    def user_vars(self):
-        return self._variables
+    """
+    def _run_server(self):
+        self.flask_app.run(port=self._port, use_reloader=False)
 
+    @wraps(webview.start)
     def run(self, *args, **kwargs):
         """
         Runs the app. It calls the function `webview.start`. The arguments will be passed to
         `webview.start` function.
 
         Parameters
         ----------
         args: Any
 
         kwargs: Any
 
         """
         if len(self.pages) == 0:
-            raise Exception("You need to have at least one `Page` added before running the app.")
-        api = _DesktopAppApi(self)
-        func = self.pages[0]._create_first_window(name=self.name, api=api, assets_folder=self._assets_folder)
-        self._is_running = True
-        webview.start(func)
-
-    def _communicate(self, data_from_js, window):
-        debug("communicating")
-        s = time.time()
-        data_dict = json.loads(data_from_js)
-        debug(data_dict)
-        func = data_dict['func']
-        args = data_dict['args']
-        new_html = data_dict['html']
-        new_page = Page()
-        new_page.from_str(new_html)
-        new_page._app = self
-        new_page._signal_mode = True
-        new_page.window = window
-        if self._func_exists(func):
-            self._call_func(func, *args, page=new_page)
-        e = time.time()
-        debug(f"TIME: {e - s}s")
+            raise Exception("Cannot run the app because no pages were added.")
+        self._port = webview.http._get_random_port()
+        t = threading.Thread(target=self._run_server)
+        t.daemon = True
+        t.start()
+        self.pages[0]._create_window()
+        webview.start(*args, **kwargs)
 
 
 def quick_website(name="App", html_file=None, html_str=None, url="/", assets_folder=None, secret_key=None):
     """
     Creates a web app and adds a single `Page` to it.
 
     Parameters
@@ -750,15 +788,15 @@
     """
     app = Website(name=name, assets_folder=assets_folder, secret_key=secret_key)
     page = Page(url=url, html_file=html_file, html_str=html_str)
     app.add_pages(page)
     return app
 
 
-def quick_desktop_app(name="App", html_file=None, html_str=None, url="/", assets_folder=None):
+def quick_desktop_app(name="App", html_file=None, html_str=None, url="/", assets_folder=None, secret_key=None):
     """
     Creates a desktop app and adds a single `Page` to it.
 
     Parameters
     ----------
     name: str (optional)
         The name of the app.
@@ -777,16 +815,17 @@
         you can ignore this parameter.
 
     Returns
     -------
     DesktopApp
 
     """
-    app = DesktopApp(name=name, assets_folder=assets_folder)
+    app = DesktopApp(name=name, assets_folder=assets_folder, secret_key=secret_key)
     page = Page(url=url, html_file=html_file, html_str=html_str)
     app.add_pages(page)
     return app
 
+
 if __name__ == "__main__":
     import doctest
     results = doctest.testmod()
     print(results)
```

### Comparing `toui-1.2.0a1/toui/elements.py` & `toui-2.0.0/toui/elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 A module that creates HTML elements.
 """
 from bs4 import BeautifulSoup
 from bs4.element import Tag
 from copy import copy
 import tinycss
 from toui._signals import Signal
-from toui._helpers import warn, debug, selector_to_str
+from toui._helpers import warn, debug, selector_to_str, obj_converter
 
 
 class _ElementSignal(Signal):
     """
     Creates signals that will be sent to JavaScript.
 
     These signals are related the methods of the `Element` object.
@@ -631,15 +631,15 @@
 
         >>> #<class 'int'>
 
         """
         if quotes:
             args = ",".join([f'"{arg}"' for arg in func_args])
         else:
-            args = ",".join([f'{arg}' for arg in func_args])
+            args = ",".join([f'{obj_converter(arg)}' for arg in func_args])
         if callable(func_or_name):
             name = func_or_name.__name__
             if self._parent_page:
                 self._parent_page.add_function(func_or_name)
             else:
                 self._functions[func_or_name.__name__] = func_or_name
         else:
```

### Comparing `toui-1.2.0a1/toui/pages.py` & `toui-2.0.0/toui/pages.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 A module that creates web pages or windows.
 """
 import os
 import time
 from bs4 import BeautifulSoup
 import webview
 import json
+from flask import session
 from toui.elements import Element
 from toui._javascript_templates import custom_func, get_script
 from copy import copy
-from toui._helpers import warn, info, debug, selector_to_str
+from toui._helpers import warn, info, debug, selector_to_str, obj_converter
 from toui._signals import Signal
 from toui._defaults import view_func
 
 
 class _PageSignal(Signal):
     """
     Creates signals that will be sent to JavaScript.
@@ -47,30 +48,34 @@
         js_kwargs = {"script": value}
         return {'func': js_func, 'args': js_args, 'kwargs': js_kwargs}
 
     @staticmethod
     def _open_another_page(**kwargs):
         js_func = "_goTo"
         js_args = []
-        js_kwargs = {"url": kwargs['url']}
+        js_kwargs = {"url": kwargs['url'], "new": kwargs['new']}
         return {'func': js_func, 'args': js_args, 'kwargs': js_kwargs}
 
 
 class Page:
     """
     Creates an HTML page that can be used as a window or as a webpage.
 
     Attributes
     ----------
     url: str
         The URL of the page.
 
-    window: pywebview.Window, default = None
-        A `pywebview.Window` object. It is automatically created when adding the `Page` to
-        `DesktopApp` and running the app.
+    title: str
+        In desktop app, this attribute will be the title of the window.
+
+    window_defaults: dict
+        In desktop apps, this dictionary sets the default parameters of the window. To set a certain default parameter for
+        a window before creating it, include it in this dictionary. The parameters that can be set are the keyword arguments
+        of the class [`webview.create_window()`](https://pywebview.flowrl.com/guide/api.html) in pywebview package.
 
     Examples
     --------
 
     Importing the class:
 
     >>> from toui import Page
@@ -99,27 +104,30 @@
 
     See Also
     --------
     `pywebview api`: https://pywebview.flowrl.com/guide/api.html
 
     """
 
-    def __init__(self, html_file=None, html_str=None, url=None):
+    def __init__(self, html_file=None, html_str=None, url=None, title=None):
         """
         Parameters
         ----------
         html_file: str
             The path to the HTML file.
 
         html_str: str
             A string containing HTML code.
 
         url: str, optional
             If the page was used as a webpage, this will be the URL of the page.
 
+        title: str
+            In desktop app, this parameter will be the title of the window.
+
         """
         if html_file:
             self._html_file = html_file
             with open(html_file, "rt") as file:
                 original_html = file.read()
             if url is None:
                 url = "/" + os.path.basename(html_file)
@@ -133,34 +141,35 @@
         if self._html.find("html") is None:
             self._html = BeautifulSoup(f"<html>{original_html}</html>", features="html.parser")
         if url is None:
             url = "/"
         self.url = url
 
         # Other attributes
-        self.window = None
+        self.title = title
+        self.window_defaults = {}
 
         # Other internal attributes
         self._app = None
         self._signal_mode = False
         self._signals = []
         self._functions = {}
         self._basic_view_func = lambda: view_func(self)
         self._view_func = self._basic_view_func
+        self._uid = None
 
     def __str__(self):
         return self.to_str()
 
     def __repr__(self):
         return self.to_str()
 
     def __copy__(self):
         new_pg = Page(html_file=self._html_file, url=self.url)
         new_pg.from_bs4_soup(self.to_bs4_soup())
-        new_pg.window = copy(self.window)
         new_pg._signal_mode = self._signal_mode
         new_pg._app = self._app
         return new_pg
     
     @_PageSignal()
     def from_str(self, html_str):
         """
@@ -326,15 +335,15 @@
             element._signal_mode = self._signal_mode
             element._selector = {"selector": selector_to_str(tag_name=tag_name, class_name=class_name,
                                                              name=name, attrs=attrs),
                                  "number": tag_num}
             elements_list.append(element)
         return elements_list
 
-    def get_html_element(self):
+    def get_html_element(self) -> Element:
         """
         Gets the first ``<html>`` element.
 
         Returns
         -------
         Element
 
@@ -342,15 +351,15 @@
             If the ``<html>`` element was not found.
 
         """
         elements = self.get_elements("html")
         if len(elements) > 0:
             return elements[0]
 
-    def get_body_element(self):
+    def get_body_element(self) -> Element:
         """
         Gets the first ``<body>`` element.
 
         Returns
         -------
         Element
 
@@ -395,119 +404,138 @@
             Function to be added to the page.
 
         Returns
         -------
         None
 
         """
-        if self._app:
-            self._app._add_function(func)
+        name = func.__name__
+        if not callable(func):
+            warn(f"Variable '{name}' is not a function.")
+            return
+        if name.startswith("_"):
+            warn(f"Function '{name}' starts with '_'. It is safer to avoid functions that starts with '_'"
+                 f"because they might overlap with functions used by the package.")
+        if self._func_exists(name):
+            warn(f"Function '{name}' exists.")
         old_functions = copy(self._functions)
-        self._functions[func.__name__] = func
+        self._functions[name] = func
         if func.__name__ in old_functions:
             return ""
         script_element = Element("script")
         script_element.set_content(custom_func(func.__name__))
         self.get_elements(tag_name="html")[0].add_content(script_element)
         return func.__name__
 
     def on_url_request(self, func, display_return_value=False):
         """
         Sets a function that will be called when the user types the URL in a browser or when a request is sent to the
-        URL. You can view it as the `view_func` in Flask.
+        URL. You can view it as the `view_func` in Flask. It might have limited functionality compared to calling Python
+        functions from HTML, but it is the best for retrieving data from HTTP requests.
 
         Parameters
         ----------
         func: Callable
             The function that will be called when a request is sent to the URL.
 
         display_return_value: bool, default=False
             If ``True``, the browser will display the return value of the function when the URL is loaded. If ``False``,
             the return value will be ignored.
 
         """
         def new_func():
             original_return = self._basic_view_func()
+            session['user page'] = copy(self)
             new_return = func()
             if display_return_value:
                 return new_return
             else:
-                return original_return
+                pg = session['user page']
+                del session['user page']
+                return pg.to_str()
         self._view_func = new_func
 
-    def _add_script(self, template_type="web"):
+    def get_window(self):
+        for window in webview.windows:
+            if window.uid == self._uid:
+                return window
+
+    def _add_script(self):
         script_tag = Element("script")
-        script_content = get_script(template_type)
+        script_content = get_script(self._app.__class__.__name__)
         script_tag.set_content(script_content)
         self.get_elements(tag_name="html")[0].add_content(script_tag)
 
-    def _create_window(self, name, api, assets_folder):
-        with _TempHTML(directory=assets_folder, html=self.to_str(),
-                       win_kwargs={"title": name, "js_api": api}) as temp_html:
-            self.window = temp_html.win
-            time.sleep(1)
-        api.window = self.window
-        return self.window
-
-    def _create_first_window(self, name, api, assets_folder):
-        self.window = webview.create_window(title=name, js_api=api)
-        def func():
-            with _TempHTML(directory=assets_folder, html=self.to_str(),
-                           win=self.window) as temp_html:
-                time.sleep(1)
-        api.window = self.window
-        return func
+    def _create_window(self):
+        title = self.title
+        url = f"http://localhost:{self._app._port}"+self.url
+        window_defaults = self.window_defaults.copy()
+        for key, value in window_defaults.items():
+            if key == "title":
+                title = value
+                del window_defaults['title']
+            if key == "url":
+                warn(f"The window will load the URL '{value}' instead of '{self.url}' because it was set in `default_windows`.")
+                url = value
+                del window_defaults['url']
+        window = webview.create_window(title=title, url=url, **window_defaults)
+        self._uid = window.uid
+        debug(f"UID of window: {self._uid}")
+        def get_uid():
+            return self._uid
+        window.expose(get_uid)
+        return window
 
     def _evaluate_js(self, func, kwargs):
+        """This function is currently unused."""
         data_from_js = ""
         def wait_then_get_result(result):
             nonlocal data_from_js
             data_from_js = result
         codejs = f"""
         var kwargs = JSON.parse(\'{json.dumps(kwargs)}\')
         {func}(kwargs)
         """
         debug("EVALUATE: " + codejs)
         self.window.evaluate_js(codejs, callback=wait_then_get_result)
         return data_from_js
 
-    @_PageSignal()
-    def _open_another_page(self, url):
-        return
-
-
-class _TempHTML:
-
-    def __init__(self, directory, win=None, html="", win_args=(), win_kwargs=None):
-        self.directory = directory
-        self.win = win
-        self.html = html
-        self.win_args = win_args
-        if win_kwargs is None:
-            win_kwargs = {}
-        self.win_kwargs = win_kwargs
-
-    def __enter__(self):
-        i = ""
-        name = f"~toui{i}.html"
-        while os.path.exists(f"{self.directory}/{name}"):
-            if i == "":
-                i = 1
+    @_PageSignal(app_types=['Website'])
+    def _open_another_page(self, url, new):
+        if self._app.__class__.__name__ == "DesktopApp":
+            if new:
+                pg = Page(url=url)
+                pg._app = self._app
+                return pg._create_window()
             else:
-                i += 1
-            name = f"~toui{i}.html"
-        self.file = f"{self.directory}/{name}"
-        file = open(self.file, "w")
-        if self.win:
-            self.win.load_url(self.file)
+                full_url = f"http://localhost:{self._app._port}" + url
+                window = self.get_window()
+                window.load_url(full_url)
+                return window
+            
+    def _inherit_functions(self):
+        for page in self._app.pages:
+            if page.url == self.url:
+                self._functions.update(page._functions)
+                return
+            
+    def _get_functions(self):
+        """Gets all added functions in this class. This is a private function."""
+        return self._functions
+
+    def _func_exists(self, func_name: str):
+        """Checks if a function exists. This is a private function."""
+        if func_name in self._get_functions().keys():
+            return True
         else:
-            self.win = webview.create_window(*self.win_args, **self.win_kwargs, url=self.file)
-        file.write(self.html)
-        return self
+            return False
 
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        os.remove(self.file)
+    def _call_func(self, func_name, *args, page=None):
+        """Calls a function in this class. Its return value depends on the function called. This is a private function."""
+        functions = self._get_functions()
+        info(f'"{func_name}" called')
+        return functions[func_name](*args)
 
 
 if __name__ == "__main__":
     import doctest
     doctest.testmod()
```

### Comparing `toui-1.2.0a1/toui/structure.py` & `toui-2.0.0/toui/structure.py`

 * *Files identical despite different names*

### Comparing `toui-1.2.0a1/toui.egg-info/PKG-INFO` & `toui-2.0.0/toui.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 Metadata-Version: 2.1
 Name: toui
-Version: 1.2.0a1
+Version: 2.0.0
 Summary: Creates user interfaces (websites and desktop apps) from HTML easily
-Home-page: UNKNOWN
 Author: Mubarak Almehairbi
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![ToUI Image](images/logo.png)
@@ -26,14 +23,19 @@
 
 # How to install
 Run this command:
 ```shell
 pip install toui
 ```
 
+To install `toui` with less dependencies (but limited functionality), run the following command:
+```shell
+pip install toui --global-option="--small"
+```
+
 # How to create a basic website
 Import the required classes:
 ```python
 from toui import Website, Page
 ```
 Create a `Website` object:
 ```python
@@ -93,10 +95,8 @@
 Then you need to deploy the `flask_app` and not the `app`.
 
 # License and Copyrights
 Copyrights (c) 2023 Mubarak Almehairbi.
 This package is licensed under the MIT license.
 
 # Documentation
-You can find the documentation in this link: [ToUI docs](https://toui.readthedocs.io)
-
-
+You can find the documentation in this link: [ToUI docs](https://toui.readthedocs.io).
```

### Comparing `toui-1.2.0a1/toui.egg-info/SOURCES.txt` & `toui-2.0.0/toui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

