# Comparing `tmp/coveo-functools-2.0.8a1.tar.gz` & `tmp/coveo-functools-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coveo-functools-2.0.8a1.tar", max compression
+gzip compressed data, was "coveo-functools-2.0.9.tar", max compression
```

## Comparing `coveo-functools-2.0.8a1.tar` & `coveo-functools-2.0.9.tar`

### file list

```diff
@@ -1,13 +1,18 @@
--rw-r--r--   0        0        0    14146 2021-09-01 12:05:48.640449 coveo-functools-2.0.8a1/README.md
--rw-r--r--   0        0        0        0 2021-09-01 12:05:48.640449 coveo-functools-2.0.8a1/coveo_functools/__init__.py
--rw-r--r--   0        0        0     1111 2021-09-01 12:05:48.640449 coveo-functools-2.0.8a1/coveo_functools/annotations.py
--rw-r--r--   0        0        0     5082 2021-09-01 12:05:48.640449 coveo-functools-2.0.8a1/coveo_functools/casing.py
--rw-r--r--   0        0        0     2187 2021-09-01 12:05:48.640449 coveo-functools-2.0.8a1/coveo_functools/dispatch.py
--rw-r--r--   0        0        0      359 2021-09-01 12:05:48.640449 coveo-functools-2.0.8a1/coveo_functools/exceptions.py
--rw-r--r--   0        0        0      528 2021-09-01 12:05:48.640449 coveo-functools-2.0.8a1/coveo_functools/finalizer.py
--rw-r--r--   0        0        0    12276 2021-09-01 12:05:48.640449 coveo-functools-2.0.8a1/coveo_functools/flex.py
--rw-r--r--   0        0        0        0 2021-09-01 12:05:48.640449 coveo-functools-2.0.8a1/coveo_functools/py.typed
--rw-r--r--   0        0        0     9228 2021-09-01 12:05:48.640449 coveo-functools-2.0.8a1/coveo_functools/wait.py
--rw-r--r--   0        0        0      830 2021-09-01 12:06:21.672245 coveo-functools-2.0.8a1/pyproject.toml
--rw-r--r--   0        0        0    14867 2021-09-01 12:06:22.476472 coveo-functools-2.0.8a1/setup.py
--rw-r--r--   0        0        0    14343 2021-09-01 12:06:22.477792 coveo-functools-2.0.8a1/PKG-INFO
+-rw-r--r--   0        0        0    17041 2021-09-07 10:42:21.479799 coveo-functools-2.0.9/README.md
+-rw-r--r--   0        0        0        0 2021-09-07 10:42:21.479799 coveo-functools-2.0.9/coveo_functools/__init__.py
+-rw-r--r--   0        0        0     1272 2021-09-07 10:42:21.479799 coveo-functools-2.0.9/coveo_functools/annotations.py
+-rw-r--r--   0        0        0     5082 2021-09-07 10:42:21.479799 coveo-functools-2.0.9/coveo_functools/casing.py
+-rw-r--r--   0        0        0     2187 2021-09-07 10:42:21.479799 coveo-functools-2.0.9/coveo_functools/dispatch.py
+-rw-r--r--   0        0        0      359 2021-09-07 10:42:21.479799 coveo-functools-2.0.9/coveo_functools/exceptions.py
+-rw-r--r--   0        0        0      528 2021-09-07 10:42:21.479799 coveo-functools-2.0.9/coveo_functools/finalizer.py
+-rw-r--r--   0        0        0      261 2021-09-07 10:42:21.479799 coveo-functools-2.0.9/coveo_functools/flex/__init__.py
+-rw-r--r--   0        0        0     3155 2021-09-07 10:42:21.479799 coveo-functools-2.0.9/coveo_functools/flex/decorator.py
+-rw-r--r--   0        0        0     9642 2021-09-07 10:42:21.479799 coveo-functools-2.0.9/coveo_functools/flex/deserializer.py
+-rw-r--r--   0        0        0        0 2021-09-07 10:42:21.479799 coveo-functools-2.0.9/coveo_functools/flex/serializer.py
+-rw-r--r--   0        0        0      843 2021-09-07 10:42:21.479799 coveo-functools-2.0.9/coveo_functools/flex/subclass_adapter.py
+-rw-r--r--   0        0        0      283 2021-09-07 10:42:21.479799 coveo-functools-2.0.9/coveo_functools/flex/types.py
+-rw-r--r--   0        0        0        0 2021-09-07 10:42:21.479799 coveo-functools-2.0.9/coveo_functools/py.typed
+-rw-r--r--   0        0        0     9228 2021-09-07 10:42:21.479799 coveo-functools-2.0.9/coveo_functools/wait.py
+-rw-r--r--   0        0        0      828 2021-09-07 10:42:51.967845 coveo-functools-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0    17792 2021-09-07 10:42:52.804363 coveo-functools-2.0.9/setup.py
+-rw-r--r--   0        0        0    17159 2021-09-07 10:42:52.805587 coveo-functools-2.0.9/PKG-INFO
```

### Comparing `coveo-functools-2.0.8a1/README.md` & `coveo-functools-2.0.9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -84,37 +84,114 @@
 This is because `json.load()` already returns these values in the proper type. This may change in the future.
 
 
 ### Supported objects and annotations
 
 Flex can be used with:
 - Classes and dataclasses
+- Abstract classes *(new in 2.0.9)* (requires adapter; explained below)
 - Enums *(new in 2.0.6)* 
 - Functions
 - Methods
 - `Union[str, bool, int, float, list, dict, None]`  (or any combination of these basic **json-compatible types**)
 - These typing constructs, where `T` is your custom class:
   - `List[T]`
   - `Dict[str, T]`
   - `Union[T, List[T]]`  (for APIs that may return a thing-or-list-of-things)
   - `Optional[T]`
 
 
 ### Limitations
 
 - Variable positional args (such as `def fn(*args): ...`) are left untouched.
-- Basic json-compatible types are left untouched. This is determined by the annotation, not the actual value.
+- Basic json-compatible types will be left untouched. This is determined by the annotation, not the actual value.
 - If `None` is given as a value to deserialize into anything, `None` is given back. Absolutely no validation occurs in this case.
-
-- You can only `Union` basic json-compatible types, or `List[T], T`
+- An Abstract class requires a subclass adapter that returns the non-abstract class to use.
 - No support for additional `typing` and `collections` objects other than the ones mentioned in this documentation.
+- You can only `Union` basic json-compatible types, or `List[T], T`.
+
 
 These are subject to change.
 
 
+### Subclass adapters
+
+To use Abstract classes as annotations, you need to register subclass adapters.
+
+The adapter is a `Callable[[Any], TypeHint]` that you provide. 
+It will be called with the payload value as `Any`, so you can inspect the content.
+It must return a `TypeHint` that tells flex which class to use.
+
+With subclass adapters, you can selectively decide the implementation class based on the payload to deserialize.
+While this is necessary when annotating structures with Abstract classes, 
+it can be used for any other class as well.
+
+For this to work, you must register the annotated class with a callback:
+
+```python
+from coveo_functools.flex.subclass_adapter import register_subclass_adapter
+
+class Abstract:
+  @abstractmethod
+  def api(self) -> None:
+    ...
+
+  
+class ThisImplementation(Abstract):
+  def api(self) -> None:
+    ...
+  
+  
+class OtherImplementation(Abstract):
+  def api(self) -> None:
+    ...
+  
+  
+def adapter(payload: Any) -> Type:
+  assert isinstance(payload, dict)  # actual type depends on payload
+  return ThisImplementation if 'this' in payload else OtherImplementation
+  
+  
+register_subclass_adapter(Abstract, adapter)
+```
+
+Thanks to the adapter, this is now possible:
+
+```python
+assert isinstance(deserialize({'this': {}}, hint=Abstract), ThisImplementation)
+assert isinstance(deserialize({}, hint=Abstract), OtherImplementation)
+
+
+@dataclass
+class Payload:
+    owner: Abstract
+    
+
+instance = deserialize({"owner": {"this": {}}}, hint=Payload)
+assert isinstance(instance, ThisImplementation)
+```
+
+The intended use of subclass adapters is to support Abstract classes as annotations.
+
+Any other use will generally:
+  1. Mess up your type annotation game because types are altered dynamically at runtime.
+  1. Make your code more obscure and more likely to investigate the dark arts.
+  1. Break your IDE's autocompletion features.
+  1. Linters which rely on static analysis will not be as powerful as they could be.
+
+
+That being said, it's a powerful and potentially game-breaking feature 
+that can be used to bend the framework if you accept bearing the consequences:
+  - There are no validations (to allow duck typing and stuff)
+  - This means you don't *have* to return an actual subclass; just something that can handle that payload
+  - You can register a callback for `Any` (or anything else really)
+  - You're not limited to return custom classes: you can return things like `Dict[str, int]` or `List[Implementation]` and the flex machinery will handle it just as if it was statically annotated that way.
+  - The payload `value` received by the adapter is not a copy, modifications will be honored.
+
+
 ### About Enums
 
 Enums will resolve by value or name, in this order:
 
 1. By exact value (str/int/etc)
 1. By exact name (str)
 1. By flexed value (str)
```

### Comparing `coveo-functools-2.0.8a1/coveo_functools/casing.py` & `coveo-functools-2.0.9/coveo_functools/casing.py`

 * *Files identical despite different names*

### Comparing `coveo-functools-2.0.8a1/coveo_functools/dispatch.py` & `coveo-functools-2.0.9/coveo_functools/dispatch.py`

 * *Files identical despite different names*

### Comparing `coveo-functools-2.0.8a1/coveo_functools/finalizer.py` & `coveo-functools-2.0.9/coveo_functools/finalizer.py`

 * *Files identical despite different names*

### Comparing `coveo-functools-2.0.8a1/coveo_functools/wait.py` & `coveo-functools-2.0.9/coveo_functools/wait.py`

 * *Files identical despite different names*

### Comparing `coveo-functools-2.0.8a1/pyproject.toml` & `coveo-functools-2.0.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "coveo-functools"
-version = "2.0.8a1"
+version = "2.0.9"
 description = "Generic function tooling helpers"
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/coveooss/coveo-python-oss/tree/main/coveo-functools"
 authors = ["Jonathan Piché <tools@coveo.com>"]
 
 [tool.poetry.dependencies]
```

### Comparing `coveo-functools-2.0.8a1/setup.py` & `coveo-functools-2.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['coveo_functools']
+['coveo_functools', 'coveo_functools.flex']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['inflection', 'typing_extensions']
 
 setup_kwargs = {
     'name': 'coveo-functools',
-    'version': '2.0.8a1',
+    'version': '2.0.9',
     'description': 'Generic function tooling helpers',
-    'long_description': '# `coveo-functools`\n\nIntrospection, finalizers, delegates, dispatchers, waiters...\nThese utilities aim at increasing productivity.\n\n\n# `annotations`\n\nIntrospect classes and callables at runtime.\n\nCan convert string annotations into their actual type reference.\n\n\n# `flex`\n## Overview\nFlex works with annotations to adjust and convert input data to match your target structure.\n\nIt was originally done as a mean to fit `CamelCase` payloads from external APIs into `snake_case` classes.\n\nTake for example this payload that we\'d like to fit into a pep8 context:\n\n```json\n[\n    {"Name": "John", "SocialNumber": 123},\n    {"Name": "Jean", "SocialNumber": 123}\n]\n```\n\nExplicit usage example:\n\n```python\nfrom coveo_functools import flex\n\n@dataclass\nclass Person:\n    name: str\n    social_number: Optional[int] = None\n\n# the deserializer is used directly to receive a list of Person instances\nresponse = flex.deserialize(json.load(), hint=List[Person])\n```\n\nAutomatic usage example:\n\n```python\nfrom coveo_functools.flex import flex\n\n@flex\n@dataclass\nclass SomeObject:\n    """ I am decorated with @flex, so you can always give me some trouble. """\n    name: str\n\nresponse = [SomeObject(**data) for data in json.load()]\n```\n\nWhen remapping keys, Flex will ignore:\n- Casing\n- Underscores\n- Hyphens\n- Dots\n- Spaces\n\nFor instance, it will happily accept `{"__NaM e._": "John"}` as valid input for the `Person` class.\n\nIt can also create instances of custom classes:\n\n```python\n@dataclass\nclass Address:\n  street: str\n\n@dataclass\nclass Person:\n    name: str\n    address: List[Address]\n    social_number: Optional[int] = None\n```\n\nYou could then feed it a payload like `{"name": "Lucy", address: [{"street": ...}, {...}]}`. \nFlex will create an instance of `Person`, that has a list of 2 Address instances.\n\nNote: The basic types `str, bool, int, float, dict, list, None` **are ignored** (no conversion occurs).\nThis is because `json.load()` already returns these values in the proper type. This may change in the future.\n\n\n### Supported objects and annotations\n\nFlex can be used with:\n- Classes and dataclasses\n- Enums *(new in 2.0.6)* \n- Functions\n- Methods\n- `Union[str, bool, int, float, list, dict, None]`  (or any combination of these basic **json-compatible types**)\n- These typing constructs, where `T` is your custom class:\n  - `List[T]`\n  - `Dict[str, T]`\n  - `Union[T, List[T]]`  (for APIs that may return a thing-or-list-of-things)\n  - `Optional[T]`\n\n\n### Limitations\n\n- Variable positional args (such as `def fn(*args): ...`) are left untouched.\n- Basic json-compatible types are left untouched. This is determined by the annotation, not the actual value.\n- If `None` is given as a value to deserialize into anything, `None` is given back. Absolutely no validation occurs in this case.\n\n- You can only `Union` basic json-compatible types, or `List[T], T`\n- No support for additional `typing` and `collections` objects other than the ones mentioned in this documentation.\n\nThese are subject to change.\n\n\n### About Enums\n\nEnums will resolve by value or name, in this order:\n\n1. By exact value (str/int/etc)\n1. By exact name (str)\n1. By flexed value (str)\n1. By flexed name (str)\n\n\n## `flex.deserialize`\n\nThis is where the magic happens, and is the recommended usage whenever it meets your use case. \n\nTL;DR: Given that `payload` is a dict,`flex.deserialize(payload, hint=Job)` will convert `payload` into an instance of `Job`.\n\nHere\'s an example puzzle! An uncanny API returns a messy "transaction" JSON:\n\n```json\n{\n    "Sold_To": {"Name": "Jon"},\n    "Items": [\n        {"sku": 123, "price": 19.99},\n        {"sku": 234, "price": 13.99},\n        {"sku": 0, "price": 0.50, "NOTE": "Forgot the reusable bag at home!!"}\n    ],\n    "Rebates": {\n        "airmiles": {"Flat": 10.0},\n        "coupon": [{"Flat": 0.79}, {"Flat":  1.50}],\n        "senior": {"Percentage": 2.5}\n    },\n    "Id": "GgfhAs89876yh.z"\n}\n```\n\nWouldn\'t it be convenient if you could create simple classes/dataclasses around them without any boilerplate?\n\nYou can solve it with flex. In one line, too!\n\nStart by designing a hierarchy of classes with annotations that closely follow the API reference.\n\nRemember, casing and underscore are ignored in flex, so you could use pep8 if you want:\n\n```python\n# models.py\n\nfrom dataclasses import dataclass\nfrom typing import List, Dict, Union, Optional\n\n\nclass SkuItem:\n    def __init__(self, sku: int, price: float) -> None:\n        self.sku = sku\n        self.price = price\n\n\n@dataclass\nclass Rebate:\n    percentage: Optional[float] = None\n    flat: Optional[float] = None\n\n\n@dataclass\nclass Customer:\n    name: str\n\n\n@dataclass\nclass Transaction:\n    sold_to: Customer\n    items: List[SkuItem]\n    rebates: Dict[str, Union[Rebate, List[Rebate]]]\n```\n\nDid you notice any flex-related boilerplate in the snippet above? No? Good! :)\n\nHere\'s how you can use the flex deserializer to bend the furious API response into your perfect python classes:\n\n```python\npayload = {\n    "Sold_To": {"Name": "Jon"},\n    "Items": [\n        {"sku": 123, "price": 19.99},\n        {"sku": 234, "price": 13.99},\n        {"sku": 0, "price": 0.50, "NOTE": "Forgot the reusable bag at home!!"}\n    ],\n    "Rebates": {\n        "airmiles": {"Flat": 10.0},\n        "coupon": [{"Flat": 0.79}, {"Flat":  1.50}],\n        "senior": {"Percentage": 2.5}\n    },\n    "Id": "GgfhAs89876yh.z"\n}\n\ntransaction = flex.deserialize(payload, hint=Transaction)\nall_transactions = flex.deserialize([payload, payload], hint=List[Transaction])\n```\n\nInteresting details:\n- Well, the casing worked! :shrug:\n- `Id` and `NOTE` were dropped because they were excluded from the `Transaction` model. Time saver; some APIs return _tons_ of data.\n- The rebates actually kept the keys, and created `Rebate` instances as the values.\n- The value type of the `rebates` dict is either a single `Rebate` instance or a list of them. See the "thing or list of things" section below for considerations.\n- In the `all_transactions` variable, `List[Annotation]` was used directly as the hint. Nifty!\n\n\n## `@flex` and `flex(obj)`\n\nThere is a decorator version of `deserialize`.\n\n`from coveo_functools.flex import flex`\n\nIt returns a function, method or class wrapped in `flex.deserialize` magic.\nWhen called, the wrapper will automatically adjust the call arguments to match the wrapped object, call the wrapped object with them, and return the response.\n\n`flex` can be used:\n- as a decorator over classes, methods and functions\n- inline to call a function or to create flexible factories\n\nWhen used inline, you can adjust a payload for any callable:\n\n```python\nfrom some_3rd_party import calculate_price\n\nprice = flex(calculate_price)(**payload)\n```\n\nYou can also generate "flexible" factories, for instance to be used as a delegate:\n\n```python\nfrom some_3rd_party import ThisClass\n\nfactory: Callable[..., T] = flex(ThisClass)\ninstance1 = factory(**payload1)\ninstance2 = factory(**payload2)\n```\n\n\nWhen used as a decorator, all invocations are automatically handled for all callers:\n\n```python\n@flex\ndef calculate_price(sold_to: Customer, items: Union[SkuItems, List[SkuItems]]) -> float:\n    ...\n\n# breaks static analysis; wrong argument shown for demonstration purposes\nprice = calculate_price(SoldTo=dict(Name="Marie"), items={"sku": 123, "price": 19.99})\n```\n\nYou could adjust the `Transaction` from earlier class like this:\n\n```python\n@flex\n@dataclass\nclass Transaction:\n    sold_to: Customer\n    items: List[SkuItem]\n    rebates: Dict[str, Union[Rebate, List[Rebate]]]\n```\n\nSo that you can drop the explicit calls to `flex.deserialize` and use them directly:\n\n```python\none_transaction = Transaction(**payload)\nlist_transactions = [Transaction(**t) for t in [payload, payload]]\n```\n\n\n### `flex` or `deserialize`?\n\nFavor `flex.deserialize` over the decorator pattern:\n- This will make the usages explicit rather than implicit.\n- The additional wrappers created by the decorator may affect performance in the presence of huge structures.\n- You can `flex.deserialize([], hint=List[T])` and get a list, but you cannot `flex(List[T])` directly (both methods demonstrated below)\n\nGenerally, it leads to a better design because you end up wiring the `flex.deserialize` call next to the `json.load()` call in a generic manner, and that\'s 100% of the `flex` code you\'ll ever need:\n\n\n```python\nclass ApiWrapper:\n    def get_transaction(self, id: int) -> Transaction:\n        return self._do_request("GET", f"api/transactions/{id}", hint=Transaction)\n\n    def get_all_transactions(self) -> List[Transaction]:\n        return self._do_request("GET", "api/transactions", hint=List[Transaction])\n  \n    def _do_request(self, method: str, url: str, hint: T) -> T:\n        response = self._session.request(method=method, url=url)\n        return flex.deserialize(response.json, hint=hint)\n```\n\nBecause explicit is better than implicit, the above design is generally easier to understand than the one below, where `Transaction` is assumed to be decorated with `@flex`:\n\n```python\nclass ApiWrapper:\n    def get_transaction(self, id: int) -> Transaction:\n        return Transaction(**self._do_request("GET", f"api/transactions/{id}"))\n\n    def get_all_transactions(self) -> List[Transaction]:\n        return [Transaction(**data) for data in self._do_request("GET", "api/transactions")]\n  \n    def _do_request(self, method: str, url: str) -> Any:\n        response = self._session.request(method=method, url=url)\n        return response.json\n```\n\n\n## Consideration for mypy\n\nThere is one annotation case worth mentioning. \nConsider this code:\n\n```python\nclass Inner:\n    ...\n\n@flex\ndef fn(inner: Inner) -> ...:\n    ...\n\n_ = fn(**{\'inner\': {...}})\n```\n\nIn this case, mypy will infer that you\'re doing `**Dict[str, Dict]`\nand complain that Dict is not compatible with Inner.\n\nTo solve this without an ignore statement, \nexplicitly annotate/cast your payloads with Any:\n\n```python\npayload: Dict[str, Any] = {"inner": {}}\n_ = fn(**payload)\n```\n\n# `unflex`\n\nUnflex is one of the utilities used by `flex.deserializer`.\n\nIt is responsible for adjusting the keyword arguments of a dictionary, so that they match the argument names of a target function.\n\n\nIt does not perform any conversion; all it does is matching keys.\nExtra keys are dropped by default:\n\n```python\nfrom coveo_functools.flex import unflex\n\ndef fn(arg1: str, arg2: str) -> None:\n    ...\n\nassert unflex(fn, {"ARG1": ..., "ArG_2": ..., "extra": ...}) == {"arg1": ..., "arg2": ...}\n```\n\nNote: To target classes, you need to `unflex(cls.__init__, ...)`\n\n\n## `@flexcase`\n\n`flexcase` is the decorator version of `unflex`:\n\n\n```python\nfrom coveo_functools.flex import flexcase\n\n@flexcase\ndef fn(arg1: str, arg2: str) -> str:\n    return f"{arg1} {arg2}"\n\n\nassert fn(ARG1="hello", _arg2="world", extra=...) == "hello world"\n```\n\n\n# `dispatch`\n\nAn enhanced version of [functools.singledispatch](https://docs.python.org/3.8/library/functools.html#functools.singledispatch):\n\n\n- Adds support for `Type[]` annotations (singledispatch only works on instances)\n- You are no longer limited to the first argument of the method\n- You can target an argument by its name too, regardless of its position\n\n\n## `finalizer`\n\nA classic and simple try/finally context manager that launches a delegate once a block of code has completed.\n\nA common trick is to "cook" the finalizer arguments through a mutable type such as a list or dict:\n\n```python\nfrom typing import List\nfrom coveo_functools.finalizer import finalizer\n\ndef clean_up(container_names: List[str]) -> None:\n    for _ in container_names:\n        ...\n    \ndef test_spawning_containers() -> None:\n    containers: List[str] = []\n    with finalizer(clean_up, containers):\n        containers.append(\'some-container-1\')\n        containers.append(\'some-container-2\')\n        containers.append(\'some-container-3\')\n```\n\n\n## `wait.until()`\n\nWaits for a condition to happen. Can be configured with exceptions to ignore.\n\n```python\nfrom coveo_functools import wait\nimport requests\n\ndef _ready() -> bool:\n    return requests.get(\'/ping\').status_code == 200\n\nwait.until(_ready, timeout_s=30, retry_ms=100, handle_exceptions=ConnectionError,\n           failure_message="The service failed to respond in time.")\n```\n\n## `wait.Backoff`\n\nA customizable class to assist in the creation of backoff retry strategies.\n\n- Customizable growth factor\n- Jitter\n- Backoff progress % (want to fire some preliminary alarms at 50% backoff maybe?)\n- Supports infinite backoff\n- Can be configured to raise after too many attempts\n- Can be configured to raise after a set amount of time\n\ne.g.: Worker loop failure management by catching RetriesExhausted\n\n```python\nfrom coveo_functools.wait import Backoff\n\nbackoff = Backoff()\nwhile my_loop:\n    try:\n        do_stuff()\n    except Exception as exception:\n        try:\n            quit_flag.wait(next(backoff))\n        except backoff.RetriesExhausted:\n            raise exception\n```\n\ne.g.: Worker loop failure management without the nested try/catch:\n\n```python\nfrom coveo_functools.wait import Backoff\n\nbackoff = Backoff()\nwhile my_loop:\n    try:\n        do_stuff()\n    except Exception as exception:\n        wait_time = next(backoff, None)\n        if wait_time is None:\n            raise exception\n        quit_flag.wait(wait_time)\n```\n\ne.g.: You can generate the wait times without creating a Backoff instance, too:\n\n```python\nimport time\nfrom coveo_functools.wait import Backoff\n\nwait_times = list(Backoff.generate_backoff_stages(first_wait, growth, max_backoff))\nfor sleep_time in wait_times:\n    try:\n        do_stuff()\n        break\n    except:\n        time.sleep(sleep_time)\nelse:\n    raise ImSickOfTrying()\n```\n',
+    'long_description': '# `coveo-functools`\n\nIntrospection, finalizers, delegates, dispatchers, waiters...\nThese utilities aim at increasing productivity.\n\n\n# `annotations`\n\nIntrospect classes and callables at runtime.\n\nCan convert string annotations into their actual type reference.\n\n\n# `flex`\n## Overview\nFlex works with annotations to adjust and convert input data to match your target structure.\n\nIt was originally done as a mean to fit `CamelCase` payloads from external APIs into `snake_case` classes.\n\nTake for example this payload that we\'d like to fit into a pep8 context:\n\n```json\n[\n    {"Name": "John", "SocialNumber": 123},\n    {"Name": "Jean", "SocialNumber": 123}\n]\n```\n\nExplicit usage example:\n\n```python\nfrom coveo_functools import flex\n\n@dataclass\nclass Person:\n    name: str\n    social_number: Optional[int] = None\n\n# the deserializer is used directly to receive a list of Person instances\nresponse = flex.deserialize(json.load(), hint=List[Person])\n```\n\nAutomatic usage example:\n\n```python\nfrom coveo_functools.flex import flex\n\n@flex\n@dataclass\nclass SomeObject:\n    """ I am decorated with @flex, so you can always give me some trouble. """\n    name: str\n\nresponse = [SomeObject(**data) for data in json.load()]\n```\n\nWhen remapping keys, Flex will ignore:\n- Casing\n- Underscores\n- Hyphens\n- Dots\n- Spaces\n\nFor instance, it will happily accept `{"__NaM e._": "John"}` as valid input for the `Person` class.\n\nIt can also create instances of custom classes:\n\n```python\n@dataclass\nclass Address:\n  street: str\n\n@dataclass\nclass Person:\n    name: str\n    address: List[Address]\n    social_number: Optional[int] = None\n```\n\nYou could then feed it a payload like `{"name": "Lucy", address: [{"street": ...}, {...}]}`. \nFlex will create an instance of `Person`, that has a list of 2 Address instances.\n\nNote: The basic types `str, bool, int, float, dict, list, None` **are ignored** (no conversion occurs).\nThis is because `json.load()` already returns these values in the proper type. This may change in the future.\n\n\n### Supported objects and annotations\n\nFlex can be used with:\n- Classes and dataclasses\n- Abstract classes *(new in 2.0.9)* (requires adapter; explained below)\n- Enums *(new in 2.0.6)* \n- Functions\n- Methods\n- `Union[str, bool, int, float, list, dict, None]`  (or any combination of these basic **json-compatible types**)\n- These typing constructs, where `T` is your custom class:\n  - `List[T]`\n  - `Dict[str, T]`\n  - `Union[T, List[T]]`  (for APIs that may return a thing-or-list-of-things)\n  - `Optional[T]`\n\n\n### Limitations\n\n- Variable positional args (such as `def fn(*args): ...`) are left untouched.\n- Basic json-compatible types will be left untouched. This is determined by the annotation, not the actual value.\n- If `None` is given as a value to deserialize into anything, `None` is given back. Absolutely no validation occurs in this case.\n- An Abstract class requires a subclass adapter that returns the non-abstract class to use.\n- No support for additional `typing` and `collections` objects other than the ones mentioned in this documentation.\n- You can only `Union` basic json-compatible types, or `List[T], T`.\n\n\nThese are subject to change.\n\n\n### Subclass adapters\n\nTo use Abstract classes as annotations, you need to register subclass adapters.\n\nThe adapter is a `Callable[[Any], TypeHint]` that you provide. \nIt will be called with the payload value as `Any`, so you can inspect the content.\nIt must return a `TypeHint` that tells flex which class to use.\n\nWith subclass adapters, you can selectively decide the implementation class based on the payload to deserialize.\nWhile this is necessary when annotating structures with Abstract classes, \nit can be used for any other class as well.\n\nFor this to work, you must register the annotated class with a callback:\n\n```python\nfrom coveo_functools.flex.subclass_adapter import register_subclass_adapter\n\nclass Abstract:\n  @abstractmethod\n  def api(self) -> None:\n    ...\n\n  \nclass ThisImplementation(Abstract):\n  def api(self) -> None:\n    ...\n  \n  \nclass OtherImplementation(Abstract):\n  def api(self) -> None:\n    ...\n  \n  \ndef adapter(payload: Any) -> Type:\n  assert isinstance(payload, dict)  # actual type depends on payload\n  return ThisImplementation if \'this\' in payload else OtherImplementation\n  \n  \nregister_subclass_adapter(Abstract, adapter)\n```\n\nThanks to the adapter, this is now possible:\n\n```python\nassert isinstance(deserialize({\'this\': {}}, hint=Abstract), ThisImplementation)\nassert isinstance(deserialize({}, hint=Abstract), OtherImplementation)\n\n\n@dataclass\nclass Payload:\n    owner: Abstract\n    \n\ninstance = deserialize({"owner": {"this": {}}}, hint=Payload)\nassert isinstance(instance, ThisImplementation)\n```\n\nThe intended use of subclass adapters is to support Abstract classes as annotations.\n\nAny other use will generally:\n  1. Mess up your type annotation game because types are altered dynamically at runtime.\n  1. Make your code more obscure and more likely to investigate the dark arts.\n  1. Break your IDE\'s autocompletion features.\n  1. Linters which rely on static analysis will not be as powerful as they could be.\n\n\nThat being said, it\'s a powerful and potentially game-breaking feature \nthat can be used to bend the framework if you accept bearing the consequences:\n  - There are no validations (to allow duck typing and stuff)\n  - This means you don\'t *have* to return an actual subclass; just something that can handle that payload\n  - You can register a callback for `Any` (or anything else really)\n  - You\'re not limited to return custom classes: you can return things like `Dict[str, int]` or `List[Implementation]` and the flex machinery will handle it just as if it was statically annotated that way.\n  - The payload `value` received by the adapter is not a copy, modifications will be honored.\n\n\n### About Enums\n\nEnums will resolve by value or name, in this order:\n\n1. By exact value (str/int/etc)\n1. By exact name (str)\n1. By flexed value (str)\n1. By flexed name (str)\n\n\n## `flex.deserialize`\n\nThis is where the magic happens, and is the recommended usage whenever it meets your use case. \n\nTL;DR: Given that `payload` is a dict,`flex.deserialize(payload, hint=Job)` will convert `payload` into an instance of `Job`.\n\nHere\'s an example puzzle! An uncanny API returns a messy "transaction" JSON:\n\n```json\n{\n    "Sold_To": {"Name": "Jon"},\n    "Items": [\n        {"sku": 123, "price": 19.99},\n        {"sku": 234, "price": 13.99},\n        {"sku": 0, "price": 0.50, "NOTE": "Forgot the reusable bag at home!!"}\n    ],\n    "Rebates": {\n        "airmiles": {"Flat": 10.0},\n        "coupon": [{"Flat": 0.79}, {"Flat":  1.50}],\n        "senior": {"Percentage": 2.5}\n    },\n    "Id": "GgfhAs89876yh.z"\n}\n```\n\nWouldn\'t it be convenient if you could create simple classes/dataclasses around them without any boilerplate?\n\nYou can solve it with flex. In one line, too!\n\nStart by designing a hierarchy of classes with annotations that closely follow the API reference.\n\nRemember, casing and underscore are ignored in flex, so you could use pep8 if you want:\n\n```python\n# models.py\n\nfrom dataclasses import dataclass\nfrom typing import List, Dict, Union, Optional\n\n\nclass SkuItem:\n    def __init__(self, sku: int, price: float) -> None:\n        self.sku = sku\n        self.price = price\n\n\n@dataclass\nclass Rebate:\n    percentage: Optional[float] = None\n    flat: Optional[float] = None\n\n\n@dataclass\nclass Customer:\n    name: str\n\n\n@dataclass\nclass Transaction:\n    sold_to: Customer\n    items: List[SkuItem]\n    rebates: Dict[str, Union[Rebate, List[Rebate]]]\n```\n\nDid you notice any flex-related boilerplate in the snippet above? No? Good! :)\n\nHere\'s how you can use the flex deserializer to bend the furious API response into your perfect python classes:\n\n```python\npayload = {\n    "Sold_To": {"Name": "Jon"},\n    "Items": [\n        {"sku": 123, "price": 19.99},\n        {"sku": 234, "price": 13.99},\n        {"sku": 0, "price": 0.50, "NOTE": "Forgot the reusable bag at home!!"}\n    ],\n    "Rebates": {\n        "airmiles": {"Flat": 10.0},\n        "coupon": [{"Flat": 0.79}, {"Flat":  1.50}],\n        "senior": {"Percentage": 2.5}\n    },\n    "Id": "GgfhAs89876yh.z"\n}\n\ntransaction = flex.deserialize(payload, hint=Transaction)\nall_transactions = flex.deserialize([payload, payload], hint=List[Transaction])\n```\n\nInteresting details:\n- Well, the casing worked! :shrug:\n- `Id` and `NOTE` were dropped because they were excluded from the `Transaction` model. Time saver; some APIs return _tons_ of data.\n- The rebates actually kept the keys, and created `Rebate` instances as the values.\n- The value type of the `rebates` dict is either a single `Rebate` instance or a list of them. See the "thing or list of things" section below for considerations.\n- In the `all_transactions` variable, `List[Annotation]` was used directly as the hint. Nifty!\n\n\n## `@flex` and `flex(obj)`\n\nThere is a decorator version of `deserialize`.\n\n`from coveo_functools.flex import flex`\n\nIt returns a function, method or class wrapped in `flex.deserialize` magic.\nWhen called, the wrapper will automatically adjust the call arguments to match the wrapped object, call the wrapped object with them, and return the response.\n\n`flex` can be used:\n- as a decorator over classes, methods and functions\n- inline to call a function or to create flexible factories\n\nWhen used inline, you can adjust a payload for any callable:\n\n```python\nfrom some_3rd_party import calculate_price\n\nprice = flex(calculate_price)(**payload)\n```\n\nYou can also generate "flexible" factories, for instance to be used as a delegate:\n\n```python\nfrom some_3rd_party import ThisClass\n\nfactory: Callable[..., T] = flex(ThisClass)\ninstance1 = factory(**payload1)\ninstance2 = factory(**payload2)\n```\n\n\nWhen used as a decorator, all invocations are automatically handled for all callers:\n\n```python\n@flex\ndef calculate_price(sold_to: Customer, items: Union[SkuItems, List[SkuItems]]) -> float:\n    ...\n\n# breaks static analysis; wrong argument shown for demonstration purposes\nprice = calculate_price(SoldTo=dict(Name="Marie"), items={"sku": 123, "price": 19.99})\n```\n\nYou could adjust the `Transaction` from earlier class like this:\n\n```python\n@flex\n@dataclass\nclass Transaction:\n    sold_to: Customer\n    items: List[SkuItem]\n    rebates: Dict[str, Union[Rebate, List[Rebate]]]\n```\n\nSo that you can drop the explicit calls to `flex.deserialize` and use them directly:\n\n```python\none_transaction = Transaction(**payload)\nlist_transactions = [Transaction(**t) for t in [payload, payload]]\n```\n\n\n### `flex` or `deserialize`?\n\nFavor `flex.deserialize` over the decorator pattern:\n- This will make the usages explicit rather than implicit.\n- The additional wrappers created by the decorator may affect performance in the presence of huge structures.\n- You can `flex.deserialize([], hint=List[T])` and get a list, but you cannot `flex(List[T])` directly (both methods demonstrated below)\n\nGenerally, it leads to a better design because you end up wiring the `flex.deserialize` call next to the `json.load()` call in a generic manner, and that\'s 100% of the `flex` code you\'ll ever need:\n\n\n```python\nclass ApiWrapper:\n    def get_transaction(self, id: int) -> Transaction:\n        return self._do_request("GET", f"api/transactions/{id}", hint=Transaction)\n\n    def get_all_transactions(self) -> List[Transaction]:\n        return self._do_request("GET", "api/transactions", hint=List[Transaction])\n  \n    def _do_request(self, method: str, url: str, hint: T) -> T:\n        response = self._session.request(method=method, url=url)\n        return flex.deserialize(response.json, hint=hint)\n```\n\nBecause explicit is better than implicit, the above design is generally easier to understand than the one below, where `Transaction` is assumed to be decorated with `@flex`:\n\n```python\nclass ApiWrapper:\n    def get_transaction(self, id: int) -> Transaction:\n        return Transaction(**self._do_request("GET", f"api/transactions/{id}"))\n\n    def get_all_transactions(self) -> List[Transaction]:\n        return [Transaction(**data) for data in self._do_request("GET", "api/transactions")]\n  \n    def _do_request(self, method: str, url: str) -> Any:\n        response = self._session.request(method=method, url=url)\n        return response.json\n```\n\n\n## Consideration for mypy\n\nThere is one annotation case worth mentioning. \nConsider this code:\n\n```python\nclass Inner:\n    ...\n\n@flex\ndef fn(inner: Inner) -> ...:\n    ...\n\n_ = fn(**{\'inner\': {...}})\n```\n\nIn this case, mypy will infer that you\'re doing `**Dict[str, Dict]`\nand complain that Dict is not compatible with Inner.\n\nTo solve this without an ignore statement, \nexplicitly annotate/cast your payloads with Any:\n\n```python\npayload: Dict[str, Any] = {"inner": {}}\n_ = fn(**payload)\n```\n\n# `unflex`\n\nUnflex is one of the utilities used by `flex.deserializer`.\n\nIt is responsible for adjusting the keyword arguments of a dictionary, so that they match the argument names of a target function.\n\n\nIt does not perform any conversion; all it does is matching keys.\nExtra keys are dropped by default:\n\n```python\nfrom coveo_functools.flex import unflex\n\ndef fn(arg1: str, arg2: str) -> None:\n    ...\n\nassert unflex(fn, {"ARG1": ..., "ArG_2": ..., "extra": ...}) == {"arg1": ..., "arg2": ...}\n```\n\nNote: To target classes, you need to `unflex(cls.__init__, ...)`\n\n\n## `@flexcase`\n\n`flexcase` is the decorator version of `unflex`:\n\n\n```python\nfrom coveo_functools.flex import flexcase\n\n@flexcase\ndef fn(arg1: str, arg2: str) -> str:\n    return f"{arg1} {arg2}"\n\n\nassert fn(ARG1="hello", _arg2="world", extra=...) == "hello world"\n```\n\n\n# `dispatch`\n\nAn enhanced version of [functools.singledispatch](https://docs.python.org/3.8/library/functools.html#functools.singledispatch):\n\n\n- Adds support for `Type[]` annotations (singledispatch only works on instances)\n- You are no longer limited to the first argument of the method\n- You can target an argument by its name too, regardless of its position\n\n\n## `finalizer`\n\nA classic and simple try/finally context manager that launches a delegate once a block of code has completed.\n\nA common trick is to "cook" the finalizer arguments through a mutable type such as a list or dict:\n\n```python\nfrom typing import List\nfrom coveo_functools.finalizer import finalizer\n\ndef clean_up(container_names: List[str]) -> None:\n    for _ in container_names:\n        ...\n    \ndef test_spawning_containers() -> None:\n    containers: List[str] = []\n    with finalizer(clean_up, containers):\n        containers.append(\'some-container-1\')\n        containers.append(\'some-container-2\')\n        containers.append(\'some-container-3\')\n```\n\n\n## `wait.until()`\n\nWaits for a condition to happen. Can be configured with exceptions to ignore.\n\n```python\nfrom coveo_functools import wait\nimport requests\n\ndef _ready() -> bool:\n    return requests.get(\'/ping\').status_code == 200\n\nwait.until(_ready, timeout_s=30, retry_ms=100, handle_exceptions=ConnectionError,\n           failure_message="The service failed to respond in time.")\n```\n\n## `wait.Backoff`\n\nA customizable class to assist in the creation of backoff retry strategies.\n\n- Customizable growth factor\n- Jitter\n- Backoff progress % (want to fire some preliminary alarms at 50% backoff maybe?)\n- Supports infinite backoff\n- Can be configured to raise after too many attempts\n- Can be configured to raise after a set amount of time\n\ne.g.: Worker loop failure management by catching RetriesExhausted\n\n```python\nfrom coveo_functools.wait import Backoff\n\nbackoff = Backoff()\nwhile my_loop:\n    try:\n        do_stuff()\n    except Exception as exception:\n        try:\n            quit_flag.wait(next(backoff))\n        except backoff.RetriesExhausted:\n            raise exception\n```\n\ne.g.: Worker loop failure management without the nested try/catch:\n\n```python\nfrom coveo_functools.wait import Backoff\n\nbackoff = Backoff()\nwhile my_loop:\n    try:\n        do_stuff()\n    except Exception as exception:\n        wait_time = next(backoff, None)\n        if wait_time is None:\n            raise exception\n        quit_flag.wait(wait_time)\n```\n\ne.g.: You can generate the wait times without creating a Backoff instance, too:\n\n```python\nimport time\nfrom coveo_functools.wait import Backoff\n\nwait_times = list(Backoff.generate_backoff_stages(first_wait, growth, max_backoff))\nfor sleep_time in wait_times:\n    try:\n        do_stuff()\n        break\n    except:\n        time.sleep(sleep_time)\nelse:\n    raise ImSickOfTrying()\n```\n',
     'author': 'Jonathan Piché',
     'author_email': 'tools@coveo.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/coveooss/coveo-python-oss/tree/main/coveo-functools',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `coveo-functools-2.0.8a1/PKG-INFO` & `coveo-functools-2.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coveo-functools
-Version: 2.0.8a1
+Version: 2.0.9
 Summary: Generic function tooling helpers
 Home-page: https://github.com/coveooss/coveo-python-oss/tree/main/coveo-functools
 License: Apache-2.0
 Author: Jonathan Piché
 Author-email: tools@coveo.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: Apache Software License
@@ -102,37 +102,114 @@
 This is because `json.load()` already returns these values in the proper type. This may change in the future.
 
 
 ### Supported objects and annotations
 
 Flex can be used with:
 - Classes and dataclasses
+- Abstract classes *(new in 2.0.9)* (requires adapter; explained below)
 - Enums *(new in 2.0.6)* 
 - Functions
 - Methods
 - `Union[str, bool, int, float, list, dict, None]`  (or any combination of these basic **json-compatible types**)
 - These typing constructs, where `T` is your custom class:
   - `List[T]`
   - `Dict[str, T]`
   - `Union[T, List[T]]`  (for APIs that may return a thing-or-list-of-things)
   - `Optional[T]`
 
 
 ### Limitations
 
 - Variable positional args (such as `def fn(*args): ...`) are left untouched.
-- Basic json-compatible types are left untouched. This is determined by the annotation, not the actual value.
+- Basic json-compatible types will be left untouched. This is determined by the annotation, not the actual value.
 - If `None` is given as a value to deserialize into anything, `None` is given back. Absolutely no validation occurs in this case.
-
-- You can only `Union` basic json-compatible types, or `List[T], T`
+- An Abstract class requires a subclass adapter that returns the non-abstract class to use.
 - No support for additional `typing` and `collections` objects other than the ones mentioned in this documentation.
+- You can only `Union` basic json-compatible types, or `List[T], T`.
+
 
 These are subject to change.
 
 
+### Subclass adapters
+
+To use Abstract classes as annotations, you need to register subclass adapters.
+
+The adapter is a `Callable[[Any], TypeHint]` that you provide. 
+It will be called with the payload value as `Any`, so you can inspect the content.
+It must return a `TypeHint` that tells flex which class to use.
+
+With subclass adapters, you can selectively decide the implementation class based on the payload to deserialize.
+While this is necessary when annotating structures with Abstract classes, 
+it can be used for any other class as well.
+
+For this to work, you must register the annotated class with a callback:
+
+```python
+from coveo_functools.flex.subclass_adapter import register_subclass_adapter
+
+class Abstract:
+  @abstractmethod
+  def api(self) -> None:
+    ...
+
+  
+class ThisImplementation(Abstract):
+  def api(self) -> None:
+    ...
+  
+  
+class OtherImplementation(Abstract):
+  def api(self) -> None:
+    ...
+  
+  
+def adapter(payload: Any) -> Type:
+  assert isinstance(payload, dict)  # actual type depends on payload
+  return ThisImplementation if 'this' in payload else OtherImplementation
+  
+  
+register_subclass_adapter(Abstract, adapter)
+```
+
+Thanks to the adapter, this is now possible:
+
+```python
+assert isinstance(deserialize({'this': {}}, hint=Abstract), ThisImplementation)
+assert isinstance(deserialize({}, hint=Abstract), OtherImplementation)
+
+
+@dataclass
+class Payload:
+    owner: Abstract
+    
+
+instance = deserialize({"owner": {"this": {}}}, hint=Payload)
+assert isinstance(instance, ThisImplementation)
+```
+
+The intended use of subclass adapters is to support Abstract classes as annotations.
+
+Any other use will generally:
+  1. Mess up your type annotation game because types are altered dynamically at runtime.
+  1. Make your code more obscure and more likely to investigate the dark arts.
+  1. Break your IDE's autocompletion features.
+  1. Linters which rely on static analysis will not be as powerful as they could be.
+
+
+That being said, it's a powerful and potentially game-breaking feature 
+that can be used to bend the framework if you accept bearing the consequences:
+  - There are no validations (to allow duck typing and stuff)
+  - This means you don't *have* to return an actual subclass; just something that can handle that payload
+  - You can register a callback for `Any` (or anything else really)
+  - You're not limited to return custom classes: you can return things like `Dict[str, int]` or `List[Implementation]` and the flex machinery will handle it just as if it was statically annotated that way.
+  - The payload `value` received by the adapter is not a copy, modifications will be honored.
+
+
 ### About Enums
 
 Enums will resolve by value or name, in this order:
 
 1. By exact value (str/int/etc)
 1. By exact name (str)
 1. By flexed value (str)
```

