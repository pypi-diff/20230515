# Comparing `tmp/pytket-offline-display-0.0.4.tar.gz` & `tmp/pytket-offline-display-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytket-offline-display-0.0.4.tar", last modified: Wed Mar 22 15:23:20 2023, max compression
+gzip compressed data, was "pytket-offline-display-0.0.5.tar", last modified: Mon May 15 15:03:26 2023, max compression
```

## Comparing `pytket-offline-display-0.0.4.tar` & `pytket-offline-display-0.0.5.tar`

### file list

```diff
@@ -1,46 +1,28 @@
-drwxr-xr-x   0 tiffany.duneau   (501) staff       (20)        0 2023-03-22 15:23:20.497600 pytket-offline-display-0.0.4/
--rw-r--r--   0 tiffany.duneau   (501) staff       (20)       40 2023-02-28 17:56:06.000000 pytket-offline-display-0.0.4/MANIFEST.in
--rw-r--r--   0 tiffany.duneau   (501) staff       (20)     1068 2023-03-22 15:23:20.497461 pytket-offline-display-0.0.4/PKG-INFO
--rw-r--r--   0 tiffany.duneau   (501) staff       (20)   125878 2023-03-22 14:41:06.000000 pytket-offline-display-0.0.4/package-lock.json
--rw-r--r--   0 tiffany.duneau   (501) staff       (20)      749 2023-03-22 14:41:06.000000 pytket-offline-display-0.0.4/package.json
--rw-r--r--   0 tiffany.duneau   (501) staff       (20)      126 2022-10-17 09:47:00.000000 pytket-offline-display-0.0.4/pyproject.toml
-drwxr-xr-x   0 tiffany.duneau   (501) staff       (20)        0 2023-03-22 15:23:20.488109 pytket-offline-display-0.0.4/pytket/
-drwxr-xr-x   0 tiffany.duneau   (501) staff       (20)        0 2023-03-22 15:23:20.488155 pytket-offline-display-0.0.4/pytket/extensions/
-drwxr-xr-x   0 tiffany.duneau   (501) staff       (20)        0 2023-03-22 15:23:20.490292 pytket-offline-display-0.0.4/pytket/extensions/offline_display/
--rw-r--r--   0 tiffany.duneau   (501) staff       (20)     1653 2023-03-14 13:25:36.000000 pytket-offline-display-0.0.4/pytket/extensions/offline_display/__init__.py
-drwxr-xr-x   0 tiffany.duneau   (501) staff       (20)        0 2023-03-22 15:23:20.490519 pytket-offline-display-0.0.4/pytket/extensions/offline_display/__pycache__/
--rw-r--r--   0 tiffany.duneau   (501) staff       (20)      887 2023-02-28 14:01:12.000000 pytket-offline-display-0.0.4/pytket/extensions/offline_display/__pycache__/__init__.cpython-310.pyc
-drwxr-xr-x   0 tiffany.duneau   (501) staff       (20)        0 2023-03-22 15:23:20.492290 pytket-offline-display-0.0.4/pytket/extensions/offline_display/dist/
--rw-r--r--   0 tiffany.duneau   (501) staff       (20)   650183 2023-03-13 18:21:27.000000 pytket-offline-display-0.0.4/pytket/extensions/offline_display/dist/main.js
--rw-r--r--   0 tiffany.duneau   (501) staff       (20)      398 2023-03-08 19:09:01.000000 pytket-offline-display-0.0.4/pytket/extensions/offline_display/dist/main.js.LICENSE.txt
-drwxr-xr-x   0 tiffany.duneau   (501) staff       (20)        0 2023-03-22 15:23:20.492533 pytket-offline-display-0.0.4/pytket/extensions/offline_display/js/
--rw-r--r--   0 tiffany.duneau   (501) staff       (20)      620 2023-03-14 12:58:11.000000 pytket-offline-display-0.0.4/pytket/extensions/offline_display/js/index.js
-drwxr-xr-x   0 tiffany.duneau   (501) staff       (20)        0 2023-03-22 15:23:20.492781 pytket-offline-display-0.0.4/pytket/extensions/offline_display/static/
--rw-r--r--   0 tiffany.duneau   (501) staff       (20)       37 2023-01-31 18:41:41.000000 pytket-offline-display-0.0.4/pytket/extensions/offline_display/static/head_imports.html
-drwxr-xr-x   0 tiffany.duneau   (501) staff       (20)        0 2023-03-22 15:23:20.493852 pytket-offline-display-0.0.4/pytket_offline_display.egg-info/
--rw-r--r--   0 tiffany.duneau   (501) staff       (20)     1068 2023-03-22 15:23:20.000000 pytket-offline-display-0.0.4/pytket_offline_display.egg-info/PKG-INFO
--rw-r--r--   0 tiffany.duneau   (501) staff       (20)     1010 2023-03-22 15:23:20.000000 pytket-offline-display-0.0.4/pytket_offline_display.egg-info/SOURCES.txt
--rw-r--r--   0 tiffany.duneau   (501) staff       (20)        1 2023-03-22 15:23:20.000000 pytket-offline-display-0.0.4/pytket_offline_display.egg-info/dependency_links.txt
--rw-r--r--   0 tiffany.duneau   (501) staff       (20)        1 2023-02-28 17:00:55.000000 pytket-offline-display-0.0.4/pytket_offline_display.egg-info/not-zip-safe
--rw-r--r--   0 tiffany.duneau   (501) staff       (20)       26 2023-03-22 15:23:20.000000 pytket-offline-display-0.0.4/pytket_offline_display.egg-info/requires.txt
--rw-r--r--   0 tiffany.duneau   (501) staff       (20)       41 2023-03-22 15:23:20.000000 pytket-offline-display-0.0.4/pytket_offline_display.egg-info/top_level.txt
--rw-r--r--   0 tiffany.duneau   (501) staff       (20)      550 2023-03-22 14:37:47.000000 pytket-offline-display-0.0.4/readme.md
--rw-r--r--   0 tiffany.duneau   (501) staff       (20)       38 2023-03-22 15:23:20.497634 pytket-offline-display-0.0.4/setup.cfg
--rwxr-xr-x   0 tiffany.duneau   (501) staff       (20)     2139 2023-03-22 14:41:06.000000 pytket-offline-display-0.0.4/setup.py
-drwxr-xr-x   0 tiffany.duneau   (501) staff       (20)        0 2023-03-22 15:23:20.488551 pytket-offline-display-0.0.4/venv/
-drwxr-xr-x   0 tiffany.duneau   (501) staff       (20)        0 2023-03-22 15:23:20.497263 pytket-offline-display-0.0.4/venv/bin/
--rw-r--r--   0 tiffany.duneau   (501) staff       (20)     1200 2023-01-30 16:58:43.000000 pytket-offline-display-0.0.4/venv/bin/activate_this.py
--rwxr-xr-x   0 tiffany.duneau   (501) staff       (20)   152047 2023-02-28 14:08:14.000000 pytket-offline-display-0.0.4/venv/bin/bottle.py
--rwxr-xr-x   0 tiffany.duneau   (501) staff       (20)      650 2023-02-28 13:22:53.000000 pytket-offline-display-0.0.4/venv/bin/rst2html.py
--rwxr-xr-x   0 tiffany.duneau   (501) staff       (20)      772 2023-02-28 13:22:53.000000 pytket-offline-display-0.0.4/venv/bin/rst2html4.py
--rwxr-xr-x   0 tiffany.duneau   (501) staff       (20)     1117 2023-02-28 13:22:53.000000 pytket-offline-display-0.0.4/venv/bin/rst2html5.py
--rwxr-xr-x   0 tiffany.duneau   (501) staff       (20)      849 2023-02-28 13:22:53.000000 pytket-offline-display-0.0.4/venv/bin/rst2latex.py
--rwxr-xr-x   0 tiffany.duneau   (501) staff       (20)      672 2023-02-28 13:22:53.000000 pytket-offline-display-0.0.4/venv/bin/rst2man.py
--rwxr-xr-x   0 tiffany.duneau   (501) staff       (20)      838 2023-02-28 13:22:53.000000 pytket-offline-display-0.0.4/venv/bin/rst2odt.py
--rwxr-xr-x   0 tiffany.duneau   (501) staff       (20)     1776 2023-02-28 13:22:53.000000 pytket-offline-display-0.0.4/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 tiffany.duneau   (501) staff       (20)      657 2023-02-28 13:22:53.000000 pytket-offline-display-0.0.4/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 tiffany.duneau   (501) staff       (20)      693 2023-02-28 13:22:53.000000 pytket-offline-display-0.0.4/venv/bin/rst2s5.py
--rwxr-xr-x   0 tiffany.duneau   (501) staff       (20)      929 2023-02-28 13:22:53.000000 pytket-offline-display-0.0.4/venv/bin/rst2xetex.py
--rwxr-xr-x   0 tiffany.duneau   (501) staff       (20)      658 2023-02-28 13:22:53.000000 pytket-offline-display-0.0.4/venv/bin/rst2xml.py
--rwxr-xr-x   0 tiffany.duneau   (501) staff       (20)      726 2023-02-28 13:22:53.000000 pytket-offline-display-0.0.4/venv/bin/rstpep2html.py
--rw-r--r--   0 tiffany.duneau   (501) staff       (20)      367 2023-02-28 17:16:01.000000 pytket-offline-display-0.0.4/webpack.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:03:26.726779 pytket-offline-display-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:03:26.726779 pytket-offline-display-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:03:26.726779 pytket-offline-display-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-15 15:03:04.000000 pytket-offline-display-0.0.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-15 15:03:04.000000 pytket-offline-display-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-15 15:03:26.726779 pytket-offline-display-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)   125878 2023-05-15 15:03:04.000000 pytket-offline-display-0.0.5/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 15:03:04.000000 pytket-offline-display-0.0.5/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-15 15:03:04.000000 pytket-offline-display-0.0.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:03:26.726779 pytket-offline-display-0.0.5/pytket/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:03:26.726779 pytket-offline-display-0.0.5/pytket/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:03:26.726779 pytket-offline-display-0.0.5/pytket/extensions/offline_display/
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-15 15:03:04.000000 pytket-offline-display-0.0.5/pytket/extensions/offline_display/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:03:26.726779 pytket-offline-display-0.0.5/pytket/extensions/offline_display/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-15 15:03:04.000000 pytket-offline-display-0.0.5/pytket/extensions/offline_display/js/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:03:26.726779 pytket-offline-display-0.0.5/pytket/extensions/offline_display/static/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-15 15:03:04.000000 pytket-offline-display-0.0.5/pytket/extensions/offline_display/static/head_imports.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:03:26.726779 pytket-offline-display-0.0.5/pytket_offline_display.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-15 15:03:26.000000 pytket-offline-display-0.0.5/pytket_offline_display.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-15 15:03:26.000000 pytket-offline-display-0.0.5/pytket_offline_display.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 15:03:26.000000 pytket-offline-display-0.0.5/pytket_offline_display.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 15:03:26.000000 pytket-offline-display-0.0.5/pytket_offline_display.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-15 15:03:26.000000 pytket-offline-display-0.0.5/pytket_offline_display.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 15:03:26.000000 pytket-offline-display-0.0.5/pytket_offline_display.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-15 15:03:04.000000 pytket-offline-display-0.0.5/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 15:03:26.726779 pytket-offline-display-0.0.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2140 2023-05-15 15:03:04.000000 pytket-offline-display-0.0.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-15 15:03:04.000000 pytket-offline-display-0.0.5/webpack.config.js
```

### Comparing `pytket-offline-display-0.0.4/PKG-INFO` & `pytket-offline-display-0.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytket-offline-display
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python module for displaying pytket circuits when offline.
 Author: TKET development team
 Author-email: tket-support@cambridgequantum.com
 License: Apache 2
 Project-URL: Documentation, https://cqcl.github.io/tket/pytket/api/index.html
 Project-URL: Source, https://github.com/CQCL/pytket-offline-renderer
 Project-URL: Tracker, https://github.com/CQCL/pytket-offline-renderer/issues
@@ -29,7 +29,19 @@
 circ = Circuit(2,2)
 circ.H(0)
 circ.CX(0,1)
 circ.measure_all()
 
 render_circuit_jupyter(circ)
 ```
+
+If you want to control the default options, you can instead load a configurable instance.
+(Note that this requires pytket >= 1.15)
+```python
+from pytket.extensions.offline_display import get_circuit_renderer
+
+circuit_renderer = get_circuit_renderer()
+circuit_renderer.set_display_options(zx_style=False)  # set the default options.
+circuit_renderer.dark_mode = True  # You can also set them directly.
+
+circuit_renderer.render_circuit_jupyter(circ)
+```
```

### Comparing `pytket-offline-display-0.0.4/package-lock.json` & `pytket-offline-display-0.0.5/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'version'": "'0.0.5'"}*

```diff
@@ -3127,9 +3127,9 @@
             "dev": true,
             "integrity": "sha512-JcKqAHLPxcdb9KM49dufGXn2x3ssnfjbcaQdLlfZsL9rH9wgDQjUtDxbo8NE0F6SFvydeu1VhZe7hZuHsB2/pw==",
             "resolved": "https://registry.npmjs.org/wildcard/-/wildcard-2.0.0.tgz",
             "version": "2.0.0"
         }
     },
     "requires": true,
-    "version": "0.0.4"
+    "version": "0.0.5"
 }
```

### Comparing `pytket-offline-display-0.0.4/package.json` & `pytket-offline-display-0.0.5/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.0.5'"}*

```diff
@@ -23,9 +23,9 @@
         "type": "git",
         "url": "git+https://github.com/CQCL/tket.git"
     },
     "scripts": {
         "build": "webpack",
         "test": "echo \"Error: no test specified\" && exit 1"
     },
-    "version": "0.0.4"
+    "version": "0.0.5"
 }
```

### Comparing `pytket-offline-display-0.0.4/pytket/extensions/offline_display/__init__.py` & `pytket-offline-display-0.0.5/pytket/extensions/offline_display/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -41,13 +41,18 @@
     ])
 })
 
 env = Environment(
     loader=loader, extensions=[IncludeRawExtension]
 )
 
-# Expose the rendering methods with the local jinja env.
-circuit_renderer = CircuitRenderer(env)
 
-render_circuit_as_html = circuit_renderer.render_circuit_as_html
-render_circuit_jupyter = circuit_renderer.render_circuit_jupyter
-view_browser = circuit_renderer.view_browser
+def get_circuit_renderer():
+    """Get a configurable instance of the circuit renderer."""
+    return CircuitRenderer(env)
+
+
+# Expose the rendering methods with the local jinja env.
+_default_circuit_renderer = get_circuit_renderer()
+render_circuit_as_html = _default_circuit_renderer.render_circuit_as_html
+render_circuit_jupyter = _default_circuit_renderer.render_circuit_jupyter
+view_browser = _default_circuit_renderer.view_browser
```

### Comparing `pytket-offline-display-0.0.4/pytket/extensions/offline_display/js/index.js` & `pytket-offline-display-0.0.5/pytket/extensions/offline_display/js/index.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -8,17 +8,22 @@
 // Create the root Vue component
 function displayCircuit() {
     const app = createApp({
         delimiters: ['[[#', '#]]'],
         components: {
             CircuitDisplayContainer
         },
+        data() {
+            return {
+                initRenderOptions: displayOptions, // inserted by jinja in parent
+            }
+        }
     })
     app.config.unwrapInjectedRef = true
-    app.mount('#circuit-display-vue-container-' + circuitRendererUid)
+    app.mount('#circuit-display-vue-container-' + circuitRendererUid) // inserted by jinja
     return app
 }
 
 if (typeof window.pytketCircuitDisplays === "undefined") {
     window.pytketCircuitDisplays = {};
 }
 window.pytketCircuitDisplays[circuitRendererUid] = displayCircuit()
```

### Comparing `pytket-offline-display-0.0.4/pytket_offline_display.egg-info/PKG-INFO` & `pytket-offline-display-0.0.5/pytket_offline_display.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytket-offline-display
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python module for displaying pytket circuits when offline.
 Author: TKET development team
 Author-email: tket-support@cambridgequantum.com
 License: Apache 2
 Project-URL: Documentation, https://cqcl.github.io/tket/pytket/api/index.html
 Project-URL: Source, https://github.com/CQCL/pytket-offline-renderer
 Project-URL: Tracker, https://github.com/CQCL/pytket-offline-renderer/issues
@@ -29,7 +29,19 @@
 circ = Circuit(2,2)
 circ.H(0)
 circ.CX(0,1)
 circ.measure_all()
 
 render_circuit_jupyter(circ)
 ```
+
+If you want to control the default options, you can instead load a configurable instance.
+(Note that this requires pytket >= 1.15)
+```python
+from pytket.extensions.offline_display import get_circuit_renderer
+
+circuit_renderer = get_circuit_renderer()
+circuit_renderer.set_display_options(zx_style=False)  # set the default options.
+circuit_renderer.dark_mode = True  # You can also set them directly.
+
+circuit_renderer.render_circuit_jupyter(circ)
+```
```

### Comparing `pytket-offline-display-0.0.4/setup.py` & `pytket-offline-display-0.0.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,28 +36,28 @@
 
 
 setup(
     name="pytket-offline-display",
     author="TKET development team",
     author_email="tket-support@cambridgequantum.com",
     python_requires=">=3.9",
-    version="0.0.4",
+    version="0.0.5",
     project_urls={
         "Documentation": "https://cqcl.github.io/tket/pytket/api/index.html",
         "Source": "https://github.com/CQCL/pytket-offline-renderer",
         "Tracker": "https://github.com/CQCL/pytket-offline-renderer/issues",
     },
     description="Python module for displaying pytket circuits when offline.",
     long_description=open("readme.md", "r").read(),
     long_description_content_type="text/markdown",
     license="Apache 2",
     packages=setuptools.find_namespace_packages(),
     install_requires=[
         "jinja2 ~= 3.0",
-        "pytket > 1.11.1",
+        "pytket >= 1.15.0",
     ],
     cmdclass={
         "build_py": NPMBuild,
     },
     include_package_data=True,
     zip_safe=False,
 )
```

