# Comparing `tmp/pydantic_view-0.2.0.tar.gz` & `tmp/pydantic_view-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_view-0.2.0.tar", max compression
+gzip compressed data, was "pydantic_view-0.2.1.tar", max compression
```

## Comparing `pydantic_view-0.2.0.tar` & `pydantic_view-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2023-04-22 16:35:00.000000 pydantic_view-0.2.0/LICENSE
--rw-r--r--   0        0        0     5704 2023-04-29 10:58:09.000000 pydantic_view-0.2.0/README.md
--rw-r--r--   0        0        0      163 2023-04-29 10:56:18.000000 pydantic_view-0.2.0/pydantic_view/__init__.py
--rw-r--r--   0        0        0     6473 2023-05-01 11:00:27.000000 pydantic_view-0.2.0/pydantic_view/pydantic_view.py
--rw-r--r--   0        0        0      876 2023-05-01 14:19:36.000000 pydantic_view-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6638 1970-01-01 00:00:00.000000 pydantic_view-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-22 16:35:00.000000 pydantic_view-0.2.1/LICENSE
+-rw-r--r--   0        0        0     5704 2023-05-07 10:28:55.000000 pydantic_view-0.2.1/README.md
+-rw-r--r--   0        0        0      183 2023-05-10 12:31:33.000000 pydantic_view-0.2.1/pydantic_view/__init__.py
+-rw-r--r--   0        0        0     8356 2023-05-15 11:56:56.000000 pydantic_view-0.2.1/pydantic_view/pydantic_view.py
+-rw-r--r--   0        0        0      876 2023-05-15 11:59:13.000000 pydantic_view-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6638 1970-01-01 00:00:00.000000 pydantic_view-0.2.1/PKG-INFO
```

### Comparing `pydantic_view-0.2.0/LICENSE` & `pydantic_view-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_view-0.2.0/README.md` & `pydantic_view-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 ```python
 In [1]: from uuid import UUID, uuid4
    ...: 
    ...: from pydantic import BaseModel, Field
    ...: from pydantic_view import view
    ...: 
    ...: 
-   ...: @view("Create", exclude=["id"])
+   ...: @view("Create", exclude={"id"})
    ...: @view("Update")
-   ...: @view("Patch", optional=["username", "password", "address"])
-   ...: @view("Out", exclude=["password"])
+   ...: @view("Patch", optional={"username", "password", "address"})
+   ...: @view("Out", exclude={"password"})
    ...: class User(BaseModel):
    ...:     id: int
    ...:     username: str
    ...:     password: str
    ...:     address: str
    ...: 
 
@@ -50,44 +50,44 @@
 from fastapi import FastAPI
 from fastapi.testclient import TestClient
 from pydantic import BaseModel, Field
 
 from pydantic_view import view, view_validator
 
 
-@view("Out", exclude=["secret"])
-@view("Create", exclude=["id"], config={"extra": "forbid"})
-@view("Update", exclude=["id"])
+@view("Out", exclude={"secret"})
+@view("Create", exclude={"id"}, config={"extra": "forbid"})
+@view("Update", exclude={"id"})
 @view("UpdateMany")
-@view("Patch", exclude=["id"], optional=["name", "secret"])
-@view("PatchMany", optional=["name", "secret"])
+@view("Patch", exclude={"id"}, optional={"name", "secret"})
+@view("PatchMany", optional={"name", "secret"})
 class Group(BaseModel):
     id: int
     name: str
     secret: str = None
 
     @view_validator(["Create", "Update", "UpdateMany", "Patch", "PatchMany"], "name", allow_reuse=True)
     def validate_name(cls, v):
         if v == "admin":
             raise ValueError("Invalid name")
         return v
 
 
-@view("Out", exclude=["password"], recursive=True)
+@view("Out", exclude={"password"}, recursive=True)
 @view(
     "Create",
-    exclude=["id"],
+    exclude={"id"},
     fields={"groups": Field(default_factory=lambda: [Group(id=0, name="default")])},
     config={"extra": "forbid"},
     recursive=True,
 )
-@view("Update", exclude=["id"], recursive=True)
+@view("Update", exclude={"id"}, recursive=True)
 @view("UpdateMany", recursive=True)
-@view("Patch", exclude=["id"], optional=["username", "password", "groups"], recursive=True)
-@view("PatchMany", optional=["username", "password", "groups"], recursive=True)
+@view("Patch", exclude={"id"}, optional={"username", "password", "groups"}, recursive=True)
+@view("PatchMany", optional={"username", "password", "groups"}, recursive=True)
 class User(BaseModel):
     id: int
     username: str
     password: str
     groups: List[Group]
```

### Comparing `pydantic_view-0.2.0/pydantic_view/pydantic_view.py` & `pydantic_view-0.2.1/pydantic_view/pydantic_view.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,77 +6,98 @@
 
 class CustomDict(dict):
     pass
 
 
 def view(
     name: str,
+    base: List[str] = None,
     include: Set[str] = None,
     exclude: Set[str] = None,
     optional: Set[str] = None,
     optional_not_none: Set[str] = None,
     fields: Dict[str, Union[Type, FieldInfo, Tuple[Type, FieldInfo]]] = None,
     recursive: bool = None,
     extra: Extra = None,
     config=None,
 ):
-    if not include:
+    if include is None:
         include = set()
-    if not exclude:
+    if exclude is None:
         exclude = set()
-    if not optional:
+    if optional is None:
         optional = set()
-    if not optional_not_none:
+    if optional_not_none is None:
         optional_not_none = set()
-    if not fields:
+    if fields is None:
         fields = {}
     if recursive is None:
-        recursive = None
+        recursive = True
     if config is None:
         config = {}
 
+    view_kwds = dict(
+        name=name,
+        base=base,
+        include=include,
+        exclude=exclude,
+        optional=optional,
+        optional_not_none=optional_not_none,
+        fields=fields,
+        recursive=recursive,
+        extra=extra,
+        config=config,
+    )
+
     def wrapper(
         cls,
         name=name,
-        include=set(include),
-        exclude=set(exclude),
-        optional=set(optional),
-        optional_not_none=set(optional_not_none),
+        include=include,
+        exclude=exclude,
+        optional=optional,
+        optional_not_none=optional_not_none,
         fields=fields,
         recursive=recursive,
         config=config,
     ):
+        __base__ = cls
+        for view in base or []:
+            if hasattr(cls, view):
+                __base__ = getattr(cls, view)
+                break
+
         if include and exclude:
             raise ValueError("include and exclude cannot be used together")
 
-        include = include or set(cls.__fields__.keys())
+        include = include or set(__base__.__fields__.keys())
 
         __fields__ = {}
 
         if (optional & optional_not_none) | (optional & set(fields.keys())) | (optional_not_none & set(fields.keys())):
             raise Exception("Field should only present in the one of optional, optional_not_none or fields")
 
         for field_name in optional | optional_not_none:
-            if (field := cls.__fields__.get(field_name)) is None:
+            if (field := __base__.__fields__.get(field_name)) is None:
                 raise Exception(f"Model has not field '{field_name}'")
             __fields__[field_name] = (Optional[field.outer_type_], field.field_info)
 
         for field_name, value in fields.items():
-            if (field := cls.__fields__.get(field_name)) is None:
+            if (field := __base__.__fields__.get(field_name)) is None:
                 raise Exception(f"Model has not field '{field_name}'")
             if isinstance(value, (tuple, list)):
                 __fields__[field_name] = value
             elif isinstance(value, FieldInfo):
                 __fields__[field_name] = (field.type_, value)
             else:
                 __fields__[field_name] = (value, field.field_info)
 
         __validators__ = {}
 
-        for attr_name, attr in cls.__dict__.items():
+        for attr_name in dir(cls):
+            attr = getattr(cls, attr_name)
             if getattr(attr, "_is_view_validator", None) and name in attr._view_validator_view_names:
                 __validators__[attr_name] = validator(
                     *attr._view_validator_args,
                     **attr._view_validator_kwds,
                 )(attr)
             elif getattr(attr, "_is_view_root_validator", None) and name in attr._view_root_validator_view_names:
                 __validators__[attr_name] = root_validator(
@@ -89,48 +110,77 @@
         __cls_kwargs__ = {}
         if extra:
             __cls_kwargs__["extra"] = extra
 
         view_cls = create_model(
             view_cls_name,
             __module__=cls.__module__,
-            __base__=(cls,),
+            __base__=(__base__,),
             __validators__=__validators__,
             __cls_kwargs__=__cls_kwargs__,
             **__fields__,
         )
 
+        class ViewRootClsDesc:
+            def __get__(self, obj, owner=None):
+                return cls
+
+        class ViewNameClsDesc:
+            def __get__(self, obj, owner=None):
+                return name
+
+        setattr(view_cls, "__view_name__", ViewNameClsDesc())
+        setattr(view_cls, "__view_root_cls__", ViewRootClsDesc())
+
         if config:
-            config_cls = type("Config", (cls.Config,), config)
+            config_cls = type("Config", (__base__.Config,), config)
             view_cls = type(view_cls_name, (view_cls,), {"Config": config_cls})
 
         view_cls.__fields__ = {k: v for k, v in view_cls.__fields__.items() if k in include and k not in exclude}
 
+        for field_name in optional | optional_not_none:
+            if field := view_cls.__fields__.get(field_name):
+                field.required = False
+
         for field_name in optional_not_none:
             if field := view_cls.__fields__.get(field_name):
                 field.allow_none = False
 
         if recursive is True:
 
             def update_type(tp):
                 if isinstance(tp, _GenericAlias):
                     tp.__args__ = tuple(update_type(arg) for arg in tp.__args__)
-                elif isinstance(tp, type) and issubclass(tp, BaseModel) and hasattr(tp, name):
-                    tp = getattr(tp, name)
+                elif isinstance(tp, type) and issubclass(tp, BaseModel):
+                    for _name in (name, *tp.__bases__):
+                        if hasattr(tp, name):
+                            tp = getattr(tp, name)
+                            break
                 return tp
 
-            for k, v in view_cls.__fields__.items():
-                if v.sub_fields:
-                    for sub_field in v.sub_fields:
-                        sub_field.type_ = update_type(sub_field.type_)
-                        # sub_field.outer_type_ = update_type(sub_field.outer_type_)
-                        sub_field.prepare()
-                v.type_ = update_type(v.type_)
-                # v.outer_type_ = update_type(v.outer_type_)
-                v.prepare()
+            def update_field_type(field):
+                if field.sub_fields:
+                    for sub_field in field.sub_fields:
+                        update_field_type(sub_field)
+                else:
+                    field.type_ = update_type(field.type_)
+                    field.prepare()
+                if (
+                    isinstance(field.default_factory, type)
+                    and issubclass(field.default_factory, BaseModel)
+                    and hasattr(field.default_factory, name)
+                ):
+                    field.default_factory = getattr(field.default_factory, name)
+
+            for field in view_cls.__fields__.values():
+                update_field_type(field)
+
+        for field_name in optional_not_none:
+            if field := view_cls.__fields__.get(field_name):
+                field.allow_none = False
 
         class ViewDesc:
             def __get__(self, obj, owner=None):
                 if obj:
                     if not hasattr(obj.__dict__, f"_{view_cls_name}"):
 
                         def __init__(self):
@@ -153,24 +203,29 @@
 
                     return getattr(obj.__dict__, f"_{view_cls_name}")
 
                 return view_cls
 
         setattr(cls, name, ViewDesc())
 
+        if "__pydantic_view_kwds__" not in cls.__dict__:
+            setattr(cls, "__pydantic_view_kwds__", {})
+
+        cls.__pydantic_view_kwds__[name] = view_kwds
+
         return cls
 
     return wrapper
 
 
-def view_validator(view_names: List[str], *validator_args, **validator_kwds):
+def view_validator(view_names: List[str], field_name: str, *validator_args, **validator_kwds):
     def wrapper(fn):
         fn._is_view_validator = True
         fn._view_validator_view_names = view_names
-        fn._view_validator_args = validator_args
+        fn._view_validator_args = (field_name,) + validator_args
         fn._view_validator_kwds = validator_kwds
         return fn
 
     return wrapper
 
 
 def view_root_validator(view_names: List[str], *validator_args, **validator_kwds):
@@ -178,7 +233,13 @@
         fn._is_view_root_validator = True
         fn._view_root_validator_view_names = view_names
         fn._view_root_validator_args = validator_args
         fn._view_root_validator_kwds = validator_kwds
         return fn
 
     return wrapper
+
+
+def reapply_base_views(cls):
+    for view_kwds in getattr(cls, "__pydantic_view_kwds__", {}).values():
+        view(**view_kwds)(cls)
+    return cls
```

### Comparing `pydantic_view-0.2.0/pyproject.toml` & `pydantic_view-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-view"
-version = "0.2.0"
+version = "0.2.1"
 description = "View decorator to create the child pydantic models from the root model."
 authors = ["Roman Koshel <roma.koshel@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["pydantic", "model", "view", "utils"]
 packages = [{include = "pydantic_view"}]
 classifiers = [
```

### Comparing `pydantic_view-0.2.0/PKG-INFO` & `pydantic_view-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-view
-Version: 0.2.0
+Version: 0.2.1
 Summary: View decorator to create the child pydantic models from the root model.
 License: MIT
 Keywords: pydantic,model,view,utils
 Author: Roman Koshel
 Author-email: roma.koshel@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -36,18 +36,18 @@
 ```python
 In [1]: from uuid import UUID, uuid4
    ...: 
    ...: from pydantic import BaseModel, Field
    ...: from pydantic_view import view
    ...: 
    ...: 
-   ...: @view("Create", exclude=["id"])
+   ...: @view("Create", exclude={"id"})
    ...: @view("Update")
-   ...: @view("Patch", optional=["username", "password", "address"])
-   ...: @view("Out", exclude=["password"])
+   ...: @view("Patch", optional={"username", "password", "address"})
+   ...: @view("Out", exclude={"password"})
    ...: class User(BaseModel):
    ...:     id: int
    ...:     username: str
    ...:     password: str
    ...:     address: str
    ...: 
 
@@ -74,44 +74,44 @@
 from fastapi import FastAPI
 from fastapi.testclient import TestClient
 from pydantic import BaseModel, Field
 
 from pydantic_view import view, view_validator
 
 
-@view("Out", exclude=["secret"])
-@view("Create", exclude=["id"], config={"extra": "forbid"})
-@view("Update", exclude=["id"])
+@view("Out", exclude={"secret"})
+@view("Create", exclude={"id"}, config={"extra": "forbid"})
+@view("Update", exclude={"id"})
 @view("UpdateMany")
-@view("Patch", exclude=["id"], optional=["name", "secret"])
-@view("PatchMany", optional=["name", "secret"])
+@view("Patch", exclude={"id"}, optional={"name", "secret"})
+@view("PatchMany", optional={"name", "secret"})
 class Group(BaseModel):
     id: int
     name: str
     secret: str = None
 
     @view_validator(["Create", "Update", "UpdateMany", "Patch", "PatchMany"], "name", allow_reuse=True)
     def validate_name(cls, v):
         if v == "admin":
             raise ValueError("Invalid name")
         return v
 
 
-@view("Out", exclude=["password"], recursive=True)
+@view("Out", exclude={"password"}, recursive=True)
 @view(
     "Create",
-    exclude=["id"],
+    exclude={"id"},
     fields={"groups": Field(default_factory=lambda: [Group(id=0, name="default")])},
     config={"extra": "forbid"},
     recursive=True,
 )
-@view("Update", exclude=["id"], recursive=True)
+@view("Update", exclude={"id"}, recursive=True)
 @view("UpdateMany", recursive=True)
-@view("Patch", exclude=["id"], optional=["username", "password", "groups"], recursive=True)
-@view("PatchMany", optional=["username", "password", "groups"], recursive=True)
+@view("Patch", exclude={"id"}, optional={"username", "password", "groups"}, recursive=True)
+@view("PatchMany", optional={"username", "password", "groups"}, recursive=True)
 class User(BaseModel):
     id: int
     username: str
     password: str
     groups: List[Group]
```

