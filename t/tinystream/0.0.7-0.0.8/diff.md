# Comparing `tmp/tinystream-0.0.7.tar.gz` & `tmp/tinystream-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinystream-0.0.7.tar", last modified: Thu May 11 17:27:38 2023, max compression
+gzip compressed data, was "tinystream-0.0.8.tar", last modified: Mon May 15 09:48:22 2023, max compression
```

## Comparing `tinystream-0.0.7.tar` & `tinystream-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-05-11 17:27:38.435296 tinystream-0.0.7/
--rw-r--r--   0 mikereiche   (502) staff       (20)     1068 2022-11-24 09:19:16.000000 tinystream-0.0.7/LICENSE
--rw-r--r--   0 mikereiche   (502) staff       (20)     3795 2023-05-11 17:27:38.435153 tinystream-0.0.7/PKG-INFO
--rw-r--r--   0 mikereiche   (502) staff       (20)     3561 2023-05-11 17:04:01.000000 tinystream-0.0.7/README.md
--rw-r--r--   0 mikereiche   (502) staff       (20)       38 2023-05-11 17:27:38.435340 tinystream-0.0.7/setup.cfg
--rw-r--r--   0 mikereiche   (502) staff       (20)      490 2023-05-11 17:04:39.000000 tinystream-0.0.7/setup.py
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-05-11 17:27:38.434965 tinystream-0.0.7/tinystream.egg-info/
--rw-r--r--   0 mikereiche   (502) staff       (20)     3795 2023-05-11 17:27:38.000000 tinystream-0.0.7/tinystream.egg-info/PKG-INFO
--rw-r--r--   0 mikereiche   (502) staff       (20)      176 2023-05-11 17:27:38.000000 tinystream-0.0.7/tinystream.egg-info/SOURCES.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)        1 2023-05-11 17:27:38.000000 tinystream-0.0.7/tinystream.egg-info/dependency_links.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)       11 2023-05-11 17:27:38.000000 tinystream-0.0.7/tinystream.egg-info/top_level.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)     5863 2023-05-11 17:23:14.000000 tinystream-0.0.7/tinystream.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-05-15 09:48:22.601213 tinystream-0.0.8/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1068 2022-11-24 09:19:16.000000 tinystream-0.0.8/LICENSE
+-rw-r--r--   0 mikereiche   (502) staff       (20)     4063 2023-05-15 09:48:22.601088 tinystream-0.0.8/PKG-INFO
+-rw-r--r--   0 mikereiche   (502) staff       (20)     3829 2023-05-15 09:48:06.000000 tinystream-0.0.8/README.md
+-rw-r--r--   0 mikereiche   (502) staff       (20)       38 2023-05-15 09:48:22.601256 tinystream-0.0.8/setup.cfg
+-rw-r--r--   0 mikereiche   (502) staff       (20)      490 2023-05-15 09:48:16.000000 tinystream-0.0.8/setup.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-05-15 09:48:22.600928 tinystream-0.0.8/tinystream.egg-info/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     4063 2023-05-15 09:48:22.000000 tinystream-0.0.8/tinystream.egg-info/PKG-INFO
+-rw-r--r--   0 mikereiche   (502) staff       (20)      176 2023-05-15 09:48:22.000000 tinystream-0.0.8/tinystream.egg-info/SOURCES.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)        1 2023-05-15 09:48:22.000000 tinystream-0.0.8/tinystream.egg-info/dependency_links.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)       11 2023-05-15 09:48:22.000000 tinystream-0.0.8/tinystream.egg-info/top_level.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)     6605 2023-05-15 09:48:06.000000 tinystream-0.0.8/tinystream.py
```

### Comparing `tinystream-0.0.7/LICENSE` & `tinystream-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tinystream-0.0.7/PKG-INFO` & `tinystream-0.0.8/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinystream
-Version: 0.0.7
+Version: 0.0.8
 Summary: Yet another python streams library
 Home-page: https://github.com/mreiche/python-streams
 Author: Mike Reiche
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Tests Status](https://github.com/mreiche/python-streams/actions/workflows/tests.yml/badge.svg)
@@ -29,35 +29,53 @@
     .sorted(int, reverse=True) \  # sort()
     .reverse() \                  # collect(), count()
     .limit(2) \
     .concat([4]) \
     .sum()                        # reduce(), max(), min()
 ```
 
-## Typehinting
 
-Since Python does not support typed lambdas, this library implements a workaround.
+## Built-in Optional support
 
+Aggregator functions are *optional*:
 ```python
-from tinystream import Stream
+assert Stream.of((1, 2, 3, 4, 5)).sum().is_empty == False
+```
 
-stream = Stream.of(["A", "B", "C"], str)
+Get next value as *optional*:
+```python
+Stream.of((1, 2, 3, 4, 5)).next().is_empty = False
 ```
 
-This is not necessary when typing is used:
+Create custom *optional*:
+```python
+from tinystream import Opt
+
+assert Opt(None).is_empty is True
+```
 
+Map optional:
 ```python
-from tinystream import Stream
-from typing import List
+assert Opt("String").map(len).get() == 6
+```
 
-list: List[str] = ["A", "B", "C"]
-stream = Stream.of(list)
+Get default value:
+```python
+assert Opt(None).get(6) == 6
+assert Opt(None).get(lambda: 6) == 6
 ```
 
-Type hinting the given type:
+Filter value:
+```python
+assert Opt(0).filter(lambda x: x > 0).is_empty is True
+```
+
+## Typehinting
+
+You can typehint datatypes like:
 
 ```python
 from dataclasses import dataclass
 
 @dataclass
 class Node:
     name: str
@@ -67,23 +85,23 @@
 for lambdas:
 
 ```python
 parent = Node(name="B")
 child = Node(name="A", parent=parent)
 
 stream = Stream.of([child])
-assert next(stream.map(lambda x: x.parent, typehint=Node)).name == "B"
+assert stream.map(lambda x: x.parent, typehint=Node).next().get().name == "B"
 ```
 
 This is not necessary when you pass a mapping function:
 ```python
 def map_parent(n: Node):
     return n.parent
 
-assert next(stream.map(map_parent)).name == "B"
+assert stream.map(map_parent).next().get().name == "B"
 ```
 
 ### Typed dictionaries
 
 Dictionaries are streamed as `tuple(key, value)`
 
 ```python
```

### Comparing `tinystream-0.0.7/README.md` & `tinystream-0.0.8/tinystream.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: tinystream
+Version: 0.0.8
+Summary: Yet another python streams library
+Home-page: https://github.com/mreiche/python-streams
+Author: Mike Reiche
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![Tests Status](https://github.com/mreiche/python-streams/actions/workflows/tests.yml/badge.svg)
 [![Code Coverage Status](https://codecov.io/github/mreiche/python-streams/branch/main/graph/badge.svg)](https://app.codecov.io/github/mreiche/python-streams)
 
 # tinystream / python-streams
 
 This is a simple and lightweight Streams API inspired by Java Streams with support for type hinting.
 
@@ -20,35 +29,53 @@
     .sorted(int, reverse=True) \  # sort()
     .reverse() \                  # collect(), count()
     .limit(2) \
     .concat([4]) \
     .sum()                        # reduce(), max(), min()
 ```
 
-## Typehinting
 
-Since Python does not support typed lambdas, this library implements a workaround.
+## Built-in Optional support
 
+Aggregator functions are *optional*:
 ```python
-from tinystream import Stream
+assert Stream.of((1, 2, 3, 4, 5)).sum().is_empty == False
+```
+
+Get next value as *optional*:
+```python
+Stream.of((1, 2, 3, 4, 5)).next().is_empty = False
+```
+
+Create custom *optional*:
+```python
+from tinystream import Opt
 
-stream = Stream.of(["A", "B", "C"], str)
+assert Opt(None).is_empty is True
 ```
 
-This is not necessary when typing is used:
+Map optional:
+```python
+assert Opt("String").map(len).get() == 6
+```
 
+Get default value:
 ```python
-from tinystream import Stream
-from typing import List
+assert Opt(None).get(6) == 6
+assert Opt(None).get(lambda: 6) == 6
+```
 
-list: List[str] = ["A", "B", "C"]
-stream = Stream.of(list)
+Filter value:
+```python
+assert Opt(0).filter(lambda x: x > 0).is_empty is True
 ```
 
-Type hinting the given type:
+## Typehinting
+
+You can typehint datatypes like:
 
 ```python
 from dataclasses import dataclass
 
 @dataclass
 class Node:
     name: str
@@ -58,23 +85,23 @@
 for lambdas:
 
 ```python
 parent = Node(name="B")
 child = Node(name="A", parent=parent)
 
 stream = Stream.of([child])
-assert next(stream.map(lambda x: x.parent, typehint=Node)).name == "B"
+assert stream.map(lambda x: x.parent, typehint=Node).next().get().name == "B"
 ```
 
 This is not necessary when you pass a mapping function:
 ```python
 def map_parent(n: Node):
     return n.parent
 
-assert next(stream.map(map_parent)).name == "B"
+assert stream.map(map_parent).next().get().name == "B"
 ```
 
 ### Typed dictionaries
 
 Dictionaries are streamed as `tuple(key, value)`
 
 ```python
```

### Comparing `tinystream-0.0.7/tinystream.egg-info/PKG-INFO` & `tinystream-0.0.8/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: tinystream
-Version: 0.0.7
-Summary: Yet another python streams library
-Home-page: https://github.com/mreiche/python-streams
-Author: Mike Reiche
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![Tests Status](https://github.com/mreiche/python-streams/actions/workflows/tests.yml/badge.svg)
 [![Code Coverage Status](https://codecov.io/github/mreiche/python-streams/branch/main/graph/badge.svg)](https://app.codecov.io/github/mreiche/python-streams)
 
 # tinystream / python-streams
 
 This is a simple and lightweight Streams API inspired by Java Streams with support for type hinting.
 
@@ -29,35 +20,53 @@
     .sorted(int, reverse=True) \  # sort()
     .reverse() \                  # collect(), count()
     .limit(2) \
     .concat([4]) \
     .sum()                        # reduce(), max(), min()
 ```
 
-## Typehinting
 
-Since Python does not support typed lambdas, this library implements a workaround.
+## Built-in Optional support
 
+Aggregator functions are *optional*:
 ```python
-from tinystream import Stream
+assert Stream.of((1, 2, 3, 4, 5)).sum().is_empty == False
+```
+
+Get next value as *optional*:
+```python
+Stream.of((1, 2, 3, 4, 5)).next().is_empty = False
+```
+
+Create custom *optional*:
+```python
+from tinystream import Opt
 
-stream = Stream.of(["A", "B", "C"], str)
+assert Opt(None).is_empty is True
 ```
 
-This is not necessary when typing is used:
+Map optional:
+```python
+assert Opt("String").map(len).get() == 6
+```
 
+Get default value:
 ```python
-from tinystream import Stream
-from typing import List
+assert Opt(None).get(6) == 6
+assert Opt(None).get(lambda: 6) == 6
+```
 
-list: List[str] = ["A", "B", "C"]
-stream = Stream.of(list)
+Filter value:
+```python
+assert Opt(0).filter(lambda x: x > 0).is_empty is True
 ```
 
-Type hinting the given type:
+## Typehinting
+
+You can typehint datatypes like:
 
 ```python
 from dataclasses import dataclass
 
 @dataclass
 class Node:
     name: str
@@ -67,23 +76,23 @@
 for lambdas:
 
 ```python
 parent = Node(name="B")
 child = Node(name="A", parent=parent)
 
 stream = Stream.of([child])
-assert next(stream.map(lambda x: x.parent, typehint=Node)).name == "B"
+assert stream.map(lambda x: x.parent, typehint=Node).next().get().name == "B"
 ```
 
 This is not necessary when you pass a mapping function:
 ```python
 def map_parent(n: Node):
     return n.parent
 
-assert next(stream.map(map_parent)).name == "B"
+assert stream.map(map_parent).next().get().name == "B"
 ```
 
 ### Typed dictionaries
 
 Dictionaries are streamed as `tuple(key, value)`
 
 ```python
```

### Comparing `tinystream-0.0.7/tinystream.py` & `tinystream-0.0.8/tinystream.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,67 @@
 import functools
 import itertools
 import sys
 import warnings
-from typing import Iterable, TypeVar, Callable, List, Dict, Tuple, Iterator
+from typing import Iterable, TypeVar, Callable, List, Dict, Tuple, Iterator, Generic
 
 T = TypeVar("T")
 R = TypeVar("R")
 K = TypeVar("K")
 
 
+Mapper = Callable[[T], R]
+FlatMapper = Callable[[T], Iterable[R]]
+Consumer = Callable[[T], None]
+Comparator = Callable[[T, T], bool]
+Reducer = Callable[[T, T], R]
+Predicate = Callable[[T], bool]
+
+
+class Opt(Generic[T]):
+    def __init__(self, value: T):
+        self.__val = value
+
+    @property
+    def is_empty(self):
+        return self.__val is None
+
+    def get(self, *args) -> T:
+        if self.__val:
+            return self.__val
+        elif len(args) > 0:
+            if isinstance(args[0], Callable):
+                return args[0]()
+            else:
+                return args[0]
+        else:
+            raise Exception("Cannot get value of empty Opt without default value")
+
+    def if_present(self, consumer: Consumer[T]):
+        if not self.is_empty:
+            consumer(self.get())
+
+    def or_else(self, consumer: Callable):
+        if self.is_empty:
+            return consumer()
+
+    def filter(self, predicate: Predicate[T]):
+        if predicate(self.__val):
+            return self
+        else:
+            return Opt(None)
+
+    def map(self, mapper: Mapper[T, R]):
+        return Opt[R](mapper(self.__val))
+
+
 class Stream:
 
     @staticmethod
-    def of(iterable: Iterable[T], typehint: T = None):
+    def of(iterable: Iterable[T]):
         return IterableStream[T](iterable)
 
     @staticmethod
     def of_dict(source_dict: Dict[K, T]):
         return IterableStream[Tuple[K, T]](source_dict)
 
     @staticmethod
@@ -45,44 +90,35 @@
         else:
             return iterable
 
     def __init__(self, iterable: Iterable[T]):
         self.__iterable = self.__normalize_iterator(iterable)
         self.__collected: List[T] = None
 
-    def map(self, cb: Callable[[T], R], typehint: R = None):
-        return IterableStream[R](map(cb, self.__iterable))
+    def map(self, mapper: Mapper[T, R], typehint: R = None):
+        return IterableStream[R](map(mapper, self.__iterable))
 
     def map_key(self, key: str | int, typehint: R = None) -> "IterableStream[R]":
         def __map_key(x):
             if isinstance(x, (list, dict, tuple)):
                 return x[key]
             else:
                 return getattr(x, key)
 
         return self.filter_key(key).map(__map_key, R)
 
     def map_keys(self, keys: Iterable[str], typehint: R = None) -> "IterableStream[R]":
-        def _map_keys():
-            for val in self.__iterable:
-                for key in keys:
-                    if isinstance(val, (list, dict, tuple)) and key in val:
-                        val = val[key]
-                    elif hasattr(val, key):
-                        val = getattr(val, key)
-                    else:
-                        val = None
-                        break
-                if val:
-                    yield val
+        assert not isinstance(keys, (int, str))
+        inst = self
+        for key in keys:
+            inst = inst.map_key(key)
+        return inst
 
-        return IterableStream[R](_map_keys())
-
-    def filter(self, cb: Callable[[T, T], bool]):
-        return IterableStream[T](filter(cb, self.__iterable))
+    def filter(self, predicate: Predicate[T]):
+        return IterableStream[T](filter(predicate, self.__iterable))
 
     def filter_key(self, key: str | int, invert: bool = False):
         def __filter_key(x):
             if isinstance(x, (list, tuple)):
                 size = len(x)
                 if invert:
                     return key >= size
@@ -97,50 +133,49 @@
                 if invert:
                     return not hasattr(x, key)
                 else:
                     return hasattr(x, key)
 
         return self.filter(__filter_key)
 
-    def flatmap(self, cb: Callable[[T], Iterable[R]] = None, typehint: R = None):
+    def flatmap(self, mapper: FlatMapper[T, R] = None, typehint: R = None):
 
         def __flatmap(f, xs):
             return (y for ys in xs for y in f(ys))
 
         def __flatten(xs):
             return (y for ys in xs for y in ys)
 
-        if cb is not None:
-            return IterableStream[R](__flatmap(cb, self.__iterable))
+        if mapper is not None:
+            return IterableStream[R](__flatmap(mapper, self.__iterable))
         else:
             return IterableStream[R](__flatten(self.__iterable))
 
-    def peek(self, cb: Callable[[T], None]):
+    def peek(self, consumer: Consumer[T]):
         def __peek(x: T):
-            cb(x)
+            consumer(x)
             return x
 
         return IterableStream[T](map(__peek, self.__iterable))
 
-    def sort(self, compare: Callable[[T, T], bool], reverse: bool = False):
+    def sort(self, compare: Comparator[T], reverse: bool = False):
         key = functools.cmp_to_key(compare)
         sort = sorted(self.__iterable, key=key, reverse=reverse)
         return IterableStream[T](sort)
 
     def sorted(self, key, reverse: bool = False):
         sort = sorted(self.__iterable, key=key, reverse=reverse)
         return IterableStream[T](sort)
 
     def each(self) -> Iterable[T]:
         warnings.warn("Use the stream as iterator instead", DeprecationWarning)
         return self.__iterable
 
-    def next(self) -> T | None:
-        warnings.warn("Use next(stream) instead", DeprecationWarning)
-        return self.__next__()
+    def next(self) -> Opt[T]:
+        return Opt(self.__next__())
 
     def collect(self):
         """Collects all items to a list and ends the stream"""
         if not self.__collected:
             self.__collected = list(self.__iterable)
         return self.__collected
 
@@ -153,34 +188,34 @@
         return len(self.collect())
 
     def reverse(self):
         copy = self.collect().copy()
         copy.reverse()
         return IterableStream[T](copy)
 
-    def reduce(self, cb: Callable[[T, T], R]) -> R:
+    def reduce(self, cb: Reducer) -> Opt[R]:
         try:
-            return functools.reduce(cb, self.__iterable)
+            return Opt(functools.reduce(cb, self.__iterable))
         except TypeError:
-            return None
+            return Opt(None)
 
-    def sum(self) -> T:
+    def sum(self) -> Opt[T]:
         """Sums all numbers and ends the stream"""
         return self.reduce(lambda x, y: x + y)
 
-    def max(self) -> T:
+    def max(self) -> Opt[T]:
         return self.reduce(lambda x, y: x if x > y else y)
 
-    def min(self) -> T:
+    def min(self) -> Opt[T]:
         return self.reduce(lambda x, y: x if x < y else y)
 
     def limit(self, limit: int):
         def __limit():
             for i in range(limit):
-                yield self.next()
+                yield self.__next__()
 
         return IterableStream[T](__limit())
 
     def concat(self, *iterables):
         iterators = [self.__iterable]
         for iterator in iterables:
             iterators.append(self.__normalize_iterator(iterator))
```

