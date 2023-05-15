# Comparing `tmp/hyperparameters-0.2.1.tar.gz` & `tmp/hyperparameters-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperparameters-0.2.1.tar", max compression
+gzip compressed data, was "hyperparameters-0.3.0.tar", max compression
```

## Comparing `hyperparameters-0.2.1.tar` & `hyperparameters-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1081 2023-05-14 10:27:43.299402 hyperparameters-0.2.1/LICENSE
--rw-r--r--   0        0        0     7491 2023-05-14 10:27:43.299402 hyperparameters-0.2.1/README.md
--rw-r--r--   0        0        0      768 2023-05-14 16:10:38.643028 hyperparameters-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       74 2023-05-14 10:27:43.299402 hyperparameters-0.2.1/src/hyperparameters/__init__.py
--rw-r--r--   0        0        0     9436 2023-05-14 12:39:18.806313 hyperparameters-0.2.1/src/hyperparameters/hyperparams.py
--rw-r--r--   0        0        0      849 2023-05-13 17:20:06.420558 hyperparameters-0.2.1/src/hyperparameters/ray_tune_hyperparams.py
--rw-r--r--   0        0        0     8235 1970-01-01 00:00:00.000000 hyperparameters-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-14 10:27:43.299402 hyperparameters-0.3.0/LICENSE
+-rw-r--r--   0        0        0     7498 2023-05-15 12:43:54.565884 hyperparameters-0.3.0/README.md
+-rw-r--r--   0        0        0      768 2023-05-15 16:19:51.657110 hyperparameters-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       74 2023-05-14 10:27:43.299402 hyperparameters-0.3.0/src/hyperparameters/__init__.py
+-rw-r--r--   0        0        0    11539 2023-05-15 16:15:36.529767 hyperparameters-0.3.0/src/hyperparameters/hyperparams.py
+-rw-r--r--   0        0        0     1135 2023-05-15 12:42:47.049637 hyperparameters-0.3.0/src/hyperparameters/ray_tune_hyperparams.py
+-rw-r--r--   0        0        0     8242 1970-01-01 00:00:00.000000 hyperparameters-0.3.0/PKG-INFO
```

### Comparing `hyperparameters-0.2.1/LICENSE` & `hyperparameters-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperparameters-0.2.1/README.md` & `hyperparameters-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 
 1. use the hypertunning library API to describe the search space and provide this object to the `HP(..., search_space=)` parameter;
 2. if you already specify the `HP(..., choices=[])` parameter you can treat the possible choices as a search space by setting the `HP(..., tunable=True)` parameter.
 3. for `bool` fields just set the `HP(..., tunable=True)` parameter, which is equivallent to `HP(..., tunable=True, choices=[False, True])`.
 
 Note that when using the `search_space` parameter, you don't need to use the `tunable` parameter.
 
-Finally, you are ready to use the mixin-specific class methods to extract information about your search spaces. For `ray.tune` these are:
+Finally, you are ready to use the mixin-specific methods to extract information about your search spaces. For `ray.tune` these are:
 
 1. `.ray_tune_param_space()` method that returns a dictionary describing the search space.
 2. `.ray_tune_best_values()` method that returns a dictionary of the best values to start hypertunning from.
 
 Here is a complete example of defining parameters hypertunable with `ray.tune`:
 ```python
 from ray import tune
@@ -148,19 +148,22 @@
     )
     use_dropout: bool = HP(
         "Whether the dropout layers should be activated",
         default=True,
         tunable=True,
     )
 
+
+params = MyHyperparams()
+
 # Search space config that ray.tune understands
-MyHyperparams.ray_tune_param_space()
+params.ray_tune_param_space()
 
 # Best values to start the hypertunning from
-MyHyperparams.ray_tune_best_values()
+params.ray_tune_best_values()
 ```
 
 ### Supporting other hypertunning libraries
 
 In `Hyperparameters`, the logic specific to hypertunning libraries is implemented with mixin classes. This means that you can add many mixins to your parameters and support several hypertunning libraries at once.
 
 The best place to start is to review the implementation of the `RayTuneHyperparamsMixin` class in `hyperparameters/ray_tune_hyperparams.py`.
```

### Comparing `hyperparameters-0.2.1/pyproject.toml` & `hyperparameters-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Hyperparameters"
-version = "0.2.1"
+version = "0.3.0"
 description = "Define your Hyperparameters once and use in argparse, hypertunning libraries, and as strongly-typed attributes in code!"
 authors = ["Oleh Lokshyn <olokshyn@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.urls]
 "Repository" = "https://github.com/olokshyn/Hyperparameters"
```

### Comparing `hyperparameters-0.2.1/src/hyperparameters/hyperparams.py` & `hyperparameters-0.3.0/src/hyperparameters/hyperparams.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import argparse
+import os
 from functools import partial, wraps
-from typing import Any, Iterator, TypeVar, Protocol, _ProtocolMeta
+from typing import Any, Iterator, TypeVar, Protocol, _ProtocolMeta, Optional
 
 from pydantic.fields import Field, Undefined, Validator
 from pydantic.main import BaseModel, ModelField, ModelMetaclass
 
 
 class HyperparamInfo(BaseModel):
     class Config:
@@ -12,14 +13,15 @@
         arbitrary_types_allowed = True
 
     description: str
     default: Any = None
     tunable: bool = False
     search_space: Any = None
     choices: list[Any] | None = None
+    is_path: bool = False
 
     annotation: Any = None
     type_: Any = None
     required: bool = False
 
     def can_be_none(self) -> bool:
         if self.annotation is Any:
@@ -30,25 +32,27 @@
 def HP(
     description: str,
     *,
     default: Any = Undefined,
     tunable: bool | None = None,
     search_space: Any = None,
     choices: list[Any] | None = None,
+    is_path: bool = False,
 ):
     field = Field(
         default=default,
         description=description,
     )
     field.extra["info"] = HyperparamInfo(
         description=description,
         default=default if default is not Undefined else None,
         tunable=tunable if tunable is not None else search_space is not None,
         search_space=search_space,
         choices=choices,
+        is_path=is_path,
     )
     return field
 
 
 def _choices_validator(value: Any, *, field_name: str, choices: list[Any]) -> None:
     if value not in choices:
         raise ValueError(
@@ -61,25 +65,53 @@
     info: HyperparamInfo | None = field.field_info.extra.get("info")
     if info is None:
         raise ValueError(f"Field {field_name} was not defined correctly, use HP().")
     assert isinstance(info, HyperparamInfo)
     return info
 
 
+def _get_config_value(cls: type, name: str, default: Any) -> Any:
+    for curr_cls in cls.__mro__:
+        config = getattr(curr_cls, "Config", None)
+        if config is None:
+            continue
+        if hasattr(config, name):
+            return getattr(config, name)
+    return default
+
+
+def _get_relative_paths_root(cls: type) -> Optional[str]:
+    should_adjust = _get_config_value(cls, "adjust_relative_paths", False)
+    if not should_adjust:
+        return None
+    return _get_config_value(cls, "relative_paths_root", None)
+
+
 class HyperparamsMeta(ModelMetaclass, _ProtocolMeta):
     def __new__(mcs, name, bases, namespace, **kwargs) -> type[BaseModel]:
         cls: type[BaseModel] = super().__new__(mcs, name, bases, namespace, **kwargs)
+        relative_paths_root = _get_relative_paths_root(cls)
         field: ModelField
         for field_name, field in cls.__fields__.items():
             info = _load_info(field_name, field)
 
             info.type_ = field.type_
             info.annotation = field.annotation
             info.required = field.required is True
 
+            if (
+                relative_paths_root
+                and info.is_path
+                and info.default is not None
+                and not os.path.isabs(info.default)
+            ):
+                value = os.path.join(relative_paths_root, info.default)
+                info.default = value
+                field.default = value
+
             if not info.required:
                 if info.default is None and not info.can_be_none():
                     raise ValueError(
                         f"Field {field_name} is of type {info.annotation} but is None by default. Use Optional."
                     )
 
                 if info.default is not None and not isinstance(
@@ -154,17 +186,41 @@
 
 
 SelfHyperparams = TypeVar("SelfHyperparams", bound="Hyperparams")
 
 
 class Hyperparams(BaseModel, HyperparamsProtocol, metaclass=HyperparamsMeta):
     class Config:
+        # BaseModel configs
         validate_assignment = True
         arbitrary_types_allowed = True
 
+        # Hyperparams config
+        adjust_relative_paths: bool = False
+        relative_paths_root: str = os.getcwd()
+
+    def __init__(self, **data: Any) -> None:
+        relative_paths_root = _get_relative_paths_root(self.__class__)
+        if relative_paths_root:
+            for name in data:
+                if name not in self.__fields__:
+                    continue
+                info: HyperparamInfo = _load_info(name, self.__fields__[name])
+                if info.is_path and not os.path.isabs(data[name]):
+                    data[name] = os.path.join(relative_paths_root, data[name])
+        super().__init__(**data)
+
+    def __setattr__(self, name, value) -> None:
+        relative_paths_root = _get_relative_paths_root(self.__class__)
+        if relative_paths_root:
+            info: HyperparamInfo = _load_info(name, self.__fields__[name])
+            if info.is_path and not os.path.isabs(value):
+                value = os.path.join(relative_paths_root, value)
+        return super().__setattr__(name, value)
+
     @classmethod
     def parameters(cls: type[SelfHyperparams]) -> dict[str, HyperparamInfo]:
         return {
             field_name: _load_info(field_name, field)
             for field_name, field in cls.__fields__.items()
         }
```

### Comparing `hyperparameters-0.2.1/PKG-INFO` & `hyperparameters-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperparameters
-Version: 0.2.1
+Version: 0.3.0
 Summary: Define your Hyperparameters once and use in argparse, hypertunning libraries, and as strongly-typed attributes in code!
 License: MIT
 Author: Oleh Lokshyn
 Author-email: olokshyn@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -135,15 +135,15 @@
 
 1. use the hypertunning library API to describe the search space and provide this object to the `HP(..., search_space=)` parameter;
 2. if you already specify the `HP(..., choices=[])` parameter you can treat the possible choices as a search space by setting the `HP(..., tunable=True)` parameter.
 3. for `bool` fields just set the `HP(..., tunable=True)` parameter, which is equivallent to `HP(..., tunable=True, choices=[False, True])`.
 
 Note that when using the `search_space` parameter, you don't need to use the `tunable` parameter.
 
-Finally, you are ready to use the mixin-specific class methods to extract information about your search spaces. For `ray.tune` these are:
+Finally, you are ready to use the mixin-specific methods to extract information about your search spaces. For `ray.tune` these are:
 
 1. `.ray_tune_param_space()` method that returns a dictionary describing the search space.
 2. `.ray_tune_best_values()` method that returns a dictionary of the best values to start hypertunning from.
 
 Here is a complete example of defining parameters hypertunable with `ray.tune`:
 ```python
 from ray import tune
@@ -166,19 +166,22 @@
     )
     use_dropout: bool = HP(
         "Whether the dropout layers should be activated",
         default=True,
         tunable=True,
     )
 
+
+params = MyHyperparams()
+
 # Search space config that ray.tune understands
-MyHyperparams.ray_tune_param_space()
+params.ray_tune_param_space()
 
 # Best values to start the hypertunning from
-MyHyperparams.ray_tune_best_values()
+params.ray_tune_best_values()
 ```
 
 ### Supporting other hypertunning libraries
 
 In `Hyperparameters`, the logic specific to hypertunning libraries is implemented with mixin classes. This means that you can add many mixins to your parameters and support several hypertunning libraries at once.
 
 The best place to start is to review the implementation of the `RayTuneHyperparamsMixin` class in `hyperparameters/ray_tune_hyperparams.py`.
```

