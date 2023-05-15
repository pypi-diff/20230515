# Comparing `tmp/redmage-0.1.1.tar.gz` & `tmp/redmage-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redmage-0.1.1.tar", max compression
+gzip compressed data, was "redmage-0.2.0.tar", max compression
```

## Comparing `redmage-0.1.1.tar` & `redmage-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1060 2023-04-30 18:42:13.320074 redmage-0.1.1/LICENSE
--rw-r--r--   0        0        0    14351 2023-05-12 14:17:31.917169 redmage-0.1.1/README.md
--rw-r--r--   0        0        0      660 2023-05-12 15:01:02.142626 redmage-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      333 2023-05-12 13:48:08.901451 redmage-0.1.1/redmage/__init__.py
--rw-r--r--   0        0        0     6689 2023-05-12 14:38:21.207931 redmage-0.1.1/redmage/components.py
--rw-r--r--   0        0        0      611 2023-04-30 17:51:09.398688 redmage-0.1.1/redmage/convertors.py
--rw-r--r--   0        0        0     7141 2023-05-12 15:00:48.077628 redmage-0.1.1/redmage/core.py
--rw-r--r--   0        0        0     9605 2023-04-30 17:34:15.446362 redmage-0.1.1/redmage/elements.py
--rw-r--r--   0        0        0       40 2023-04-30 16:16:17.636906 redmage-0.1.1/redmage/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-29 15:02:07.108573 redmage-0.1.1/redmage/py.typed
--rw-r--r--   0        0        0     1582 2023-04-29 14:59:56.659250 redmage-0.1.1/redmage/targets.py
--rw-r--r--   0        0        0     2187 2023-04-30 16:49:07.664173 redmage-0.1.1/redmage/triggers.py
--rw-r--r--   0        0        0     1314 2023-05-01 00:53:46.268926 redmage-0.1.1/redmage/types.py
--rw-r--r--   0        0        0      558 2023-04-30 18:18:23.887821 redmage-0.1.1/redmage/utils.py
--rw-r--r--   0        0        0    15052 1970-01-01 00:00:00.000000 redmage-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-04-30 18:42:13.320074 redmage-0.2.0/LICENSE
+-rw-r--r--   0        0        0    14693 2023-05-15 02:00:21.924105 redmage-0.2.0/README.md
+-rw-r--r--   0        0        0      660 2023-05-15 01:59:45.682116 redmage-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      328 2023-05-15 02:04:21.318232 redmage-0.2.0/redmage/__init__.py
+-rw-r--r--   0        0        0     6689 2023-05-12 14:38:21.207931 redmage-0.2.0/redmage/components.py
+-rw-r--r--   0        0        0      611 2023-04-30 17:51:09.398688 redmage-0.2.0/redmage/convertors.py
+-rw-r--r--   0        0        0     7389 2023-05-15 02:27:20.247267 redmage-0.2.0/redmage/core.py
+-rw-r--r--   0        0        0     9605 2023-04-30 17:34:15.446362 redmage-0.2.0/redmage/elements.py
+-rw-r--r--   0        0        0       40 2023-04-30 16:16:17.636906 redmage-0.2.0/redmage/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:02:07.108573 redmage-0.2.0/redmage/py.typed
+-rw-r--r--   0        0        0     1582 2023-04-29 14:59:56.659250 redmage-0.2.0/redmage/targets.py
+-rw-r--r--   0        0        0     2187 2023-04-30 16:49:07.664173 redmage-0.2.0/redmage/triggers.py
+-rw-r--r--   0        0        0     1314 2023-05-01 00:53:46.268926 redmage-0.2.0/redmage/types.py
+-rw-r--r--   0        0        0      558 2023-04-30 18:18:23.887821 redmage-0.2.0/redmage/utils.py
+-rw-r--r--   0        0        0    15394 1970-01-01 00:00:00.000000 redmage-0.2.0/PKG-INFO
```

### Comparing `redmage-0.1.1/LICENSE` & `redmage-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `redmage-0.1.1/README.md` & `redmage-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,28 +13,31 @@
 Consider the example below.
 
 ```
 from redmage import Component, Redmage, Target
 from redmage.elements import Button, Div, H1, Script
 
 
+app = Redmage()
+
+
 class Counter(Component, routes=("/",)):
     count: int
 
     def __init__(self):
         self.count = 0
 
     def render(self):
         return Div(
             H1(f"Clicked {self.count} times."),
             Button(
                 "Add 1",
                 click=self.add_one(),
             ),
-            Script(src="https://unpkg.com/htmx.org@1.8.5"),
+            Script(src="https://unpkg.com/htmx.org@1.9.2"),
         )
 
     @Target.post
     def add_one(self):
         self.count += 1
 ```
 
@@ -47,51 +50,66 @@
 
 Redmage is available on pypi.
 
 ```
 pip install redmage
 ```
 
+## Redmage application
+
+
+The first thing you need to do is create an instance of the Redmage class.
+
+```
+from redmage import Redmage
+
+
+app = Redmage()
+```
+
+At this point our app won't do anything because we haven't registered any routes by sublassing Component. But you can start it up using your favorite ASGI server like uvicorn.
+
+```
+uvicorn <module>:<filename>:app.starlette
+```
+
 
 ## First Component
 
 
 Let's create a Component. In the example we just returned a **div** element. This works but we're going to want to create a proper html page with **html**, **header**, **body** tags etc.
 
 ```
-from redmage import Component, app
+from redmage import Component, Redmage
 from redmage.elements import Body, Doc, H1, Head, Html, Script, Title
 
 
+app = Redmage()
+
+
 class Index(Component, routes=("/",)):
 
     def render(self):
         return Doc(
             Html(
                 Head(
                     Title("Example"),
                 ),
                 Body(
                     H1("Hello Redmage"),
-                    Script(src="https://unpkg.com/htmx.org@1.8.5"),
+                    Script(src="https://unpkg.com/htmx.org@1.9.2"),
                 ),
             )
         )
 ```
 
 This tells our app to register the **Index** component with the route "/". When you navigate to _localhost:8000/_ an instance of **Index** will be created and it's render method will be called to generate the html.
 
 The **Component** class is abstract and has a single abstract base method, **render**, that must be implemented and return and instance of **redmage.elements.Element**.
 
-You can start the application using your favorite ASGI server like uvicorn.
-
-```
-uvicorn <module>:<filename>:app.starlette
-```
-
 
 ## Elements
 
 Redmage internally uses python classes associated with each html tag (**Div**, **Body**, **H1** etc.). They can all be imported from **redmage.elements**. Each of these classes subclasses **redmage.elements.Element**. Pass the elements inner html as positional arguments and add attributes with keyword arguments.
 
 ```
 from redmage.elements import Div
@@ -142,28 +160,32 @@
 
 ## Nesting Components
 
 
 Components can be easily nested by using them just like you would use any other html **Element** object.
 
 ```
+from redmage import Redmage
 from redmage.elements import Body, Doc, H1, Head, Html, Script, Title
 
 
+app = Redmage()
+
+
 class Index(Component, routes=("/",)):
 
     def render(self):
         return Doc(
             Html(
                 Head(
                     Title("Todo App"),
                 ),
                 Body(
                     ChildComponent(),
-                    Script(src="https://unpkg.com/htmx.org@1.8.5"),
+                    Script(src="https://unpkg.com/htmx.org@1.9.2"),
                 ),
             )
         )
 
 
 class ChildComponent(Component):
```

### Comparing `redmage-0.1.1/pyproject.toml` & `redmage-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redmage"
-version = "0.1.1"
+version = "0.2.0"
 description = "A component based library for building htmx powered applications."
 authors = ["Scott Russell <me@scottrussell.net>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `redmage-0.1.1/redmage/components.py` & `redmage-0.2.0/redmage/components.py`

 * *Files identical despite different names*

### Comparing `redmage-0.1.1/redmage/convertors.py` & `redmage-0.2.0/redmage/convertors.py`

 * *Files identical despite different names*

### Comparing `redmage-0.1.1/redmage/core.py` & `redmage-0.2.0/redmage/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,32 +19,38 @@
 logger = logging.getLogger("redmage")
 
 
 ComponentClass = Type[Component]
 
 
 class Redmage:
-    def __init__(self) -> None:
-        self.debug = False
+    def __init__(self, debug: bool = False):
+        self.debug = debug
         self.routes: List[Route] = []
-        # Could cuase problems if multiple apps are created
+        self.components: List[Tuple[ComponentClass, Optional[Tuple[str]]]] = []
+        # Could cause problems if multiple apps are created
         Component.set_app(self)
 
     @property
     def starlette(self) -> Starlette:
         if not hasattr(self, "_starlette"):
+            self.create_routes()
             self._starlette = Starlette(debug=self.debug, routes=self.routes)
         return self._starlette
 
+    def create_routes(self) -> None:
+        for cls, routes in self.components:
+            if routes:
+                self._register_routes(cls, routes)
+            self._register_targets(cls)
+
     def register_component(
         self, cls: ComponentClass, routes: Optional[Tuple[str]] = None
     ) -> None:
-        if routes:
-            self._register_routes(cls, routes)
-        self._register_targets(cls)
+        self.components.append((cls, routes))
 
     def _get_explicit_route_function(self, cls: ComponentClass) -> Callable:
         async def route_function(request: Request) -> HTMLResponse:
             attrs = {**request.path_params, **request.query_params}
             instance = cls(**attrs)
             return HTMLResponse(str(instance))
 
@@ -196,10 +202,7 @@
                 name=method_name,
                 methods=[method_fn.target_method],  # type: ignore
             )
         )
 
         target_method = self._get_target_method(method_name, method_fn)
         setattr(cls, method_name, target_method)
-
-
-app = Redmage()
```

### Comparing `redmage-0.1.1/redmage/elements.py` & `redmage-0.2.0/redmage/elements.py`

 * *Files identical despite different names*

### Comparing `redmage-0.1.1/redmage/targets.py` & `redmage-0.2.0/redmage/targets.py`

 * *Files identical despite different names*

### Comparing `redmage-0.1.1/redmage/triggers.py` & `redmage-0.2.0/redmage/triggers.py`

 * *Files identical despite different names*

### Comparing `redmage-0.1.1/redmage/types.py` & `redmage-0.2.0/redmage/types.py`

 * *Files identical despite different names*

### Comparing `redmage-0.1.1/redmage/utils.py` & `redmage-0.2.0/redmage/utils.py`

 * *Files identical despite different names*

### Comparing `redmage-0.1.1/PKG-INFO` & `redmage-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redmage
-Version: 0.1.1
+Version: 0.2.0
 Summary: A component based library for building htmx powered applications.
 License: MIT
 Author: Scott Russell
 Author-email: me@scottrussell.net
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -32,28 +32,31 @@
 Consider the example below.
 
 ```
 from redmage import Component, Redmage, Target
 from redmage.elements import Button, Div, H1, Script
 
 
+app = Redmage()
+
+
 class Counter(Component, routes=("/",)):
     count: int
 
     def __init__(self):
         self.count = 0
 
     def render(self):
         return Div(
             H1(f"Clicked {self.count} times."),
             Button(
                 "Add 1",
                 click=self.add_one(),
             ),
-            Script(src="https://unpkg.com/htmx.org@1.8.5"),
+            Script(src="https://unpkg.com/htmx.org@1.9.2"),
         )
 
     @Target.post
     def add_one(self):
         self.count += 1
 ```
 
@@ -66,51 +69,66 @@
 
 Redmage is available on pypi.
 
 ```
 pip install redmage
 ```
 
+## Redmage application
+
+
+The first thing you need to do is create an instance of the Redmage class.
+
+```
+from redmage import Redmage
+
+
+app = Redmage()
+```
+
+At this point our app won't do anything because we haven't registered any routes by sublassing Component. But you can start it up using your favorite ASGI server like uvicorn.
+
+```
+uvicorn <module>:<filename>:app.starlette
+```
+
 
 ## First Component
 
 
 Let's create a Component. In the example we just returned a **div** element. This works but we're going to want to create a proper html page with **html**, **header**, **body** tags etc.
 
 ```
-from redmage import Component, app
+from redmage import Component, Redmage
 from redmage.elements import Body, Doc, H1, Head, Html, Script, Title
 
 
+app = Redmage()
+
+
 class Index(Component, routes=("/",)):
 
     def render(self):
         return Doc(
             Html(
                 Head(
                     Title("Example"),
                 ),
                 Body(
                     H1("Hello Redmage"),
-                    Script(src="https://unpkg.com/htmx.org@1.8.5"),
+                    Script(src="https://unpkg.com/htmx.org@1.9.2"),
                 ),
             )
         )
 ```
 
 This tells our app to register the **Index** component with the route "/". When you navigate to _localhost:8000/_ an instance of **Index** will be created and it's render method will be called to generate the html.
 
 The **Component** class is abstract and has a single abstract base method, **render**, that must be implemented and return and instance of **redmage.elements.Element**.
 
-You can start the application using your favorite ASGI server like uvicorn.
-
-```
-uvicorn <module>:<filename>:app.starlette
-```
-
 
 ## Elements
 
 Redmage internally uses python classes associated with each html tag (**Div**, **Body**, **H1** etc.). They can all be imported from **redmage.elements**. Each of these classes subclasses **redmage.elements.Element**. Pass the elements inner html as positional arguments and add attributes with keyword arguments.
 
 ```
 from redmage.elements import Div
@@ -161,28 +179,32 @@
 
 ## Nesting Components
 
 
 Components can be easily nested by using them just like you would use any other html **Element** object.
 
 ```
+from redmage import Redmage
 from redmage.elements import Body, Doc, H1, Head, Html, Script, Title
 
 
+app = Redmage()
+
+
 class Index(Component, routes=("/",)):
 
     def render(self):
         return Doc(
             Html(
                 Head(
                     Title("Todo App"),
                 ),
                 Body(
                     ChildComponent(),
-                    Script(src="https://unpkg.com/htmx.org@1.8.5"),
+                    Script(src="https://unpkg.com/htmx.org@1.9.2"),
                 ),
             )
         )
 
 
 class ChildComponent(Component):
```

