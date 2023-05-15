# Comparing `tmp/JsonAndXmlSerializer-0.1.0.tar.gz` & `tmp/JsonAndXmlSerializer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JsonAndXmlSerializer-0.1.0.tar", last modified: Sun May 14 22:03:45 2023, max compression
+gzip compressed data, was "JsonAndXmlSerializer-0.1.1.tar", last modified: Mon May 15 15:04:56 2023, max compression
```

## Comparing `JsonAndXmlSerializer-0.1.0.tar` & `JsonAndXmlSerializer-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-14 22:03:45.520252 JsonAndXmlSerializer-0.1.0/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-14 22:03:45.516252 JsonAndXmlSerializer-0.1.0/JsonAndXmlSerializer.egg-info/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      321 2023-05-14 22:03:45.000000 JsonAndXmlSerializer-0.1.0/JsonAndXmlSerializer.egg-info/PKG-INFO
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      450 2023-05-14 22:03:45.000000 JsonAndXmlSerializer-0.1.0/JsonAndXmlSerializer.egg-info/SOURCES.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-05-14 22:03:45.000000 JsonAndXmlSerializer-0.1.0/JsonAndXmlSerializer.egg-info/dependency_links.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        6 2023-05-14 22:03:45.000000 JsonAndXmlSerializer-0.1.0/JsonAndXmlSerializer.egg-info/requires.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       11 2023-05-14 22:03:45.000000 JsonAndXmlSerializer-0.1.0/JsonAndXmlSerializer.egg-info/top_level.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      321 2023-05-14 22:03:45.520252 JsonAndXmlSerializer-0.1.0/PKG-INFO
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-14 22:03:45.520252 JsonAndXmlSerializer-0.1.0/Serializer/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      603 2023-05-14 16:05:40.000000 JsonAndXmlSerializer-0.1.0/Serializer/__init__.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      361 2023-05-14 10:14:56.000000 JsonAndXmlSerializer-0.1.0/Serializer/base_serializer.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1135 2023-05-13 12:56:57.000000 JsonAndXmlSerializer-0.1.0/Serializer/constants.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)    10104 2023-05-14 16:17:32.000000 JsonAndXmlSerializer-0.1.0/Serializer/dict_serializer.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3997 2023-05-14 16:18:26.000000 JsonAndXmlSerializer-0.1.0/Serializer/json_serializer.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      523 2023-05-14 16:06:03.000000 JsonAndXmlSerializer-0.1.0/Serializer/serializers_factory.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     4112 2023-05-14 16:20:21.000000 JsonAndXmlSerializer-0.1.0/Serializer/xml_serializer.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       38 2023-05-14 22:03:45.520252 JsonAndXmlSerializer-0.1.0/setup.cfg
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      499 2023-05-14 21:32:42.000000 JsonAndXmlSerializer-0.1.0/setup.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-14 22:03:45.520252 JsonAndXmlSerializer-0.1.0/test/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      948 2023-05-14 16:23:30.000000 JsonAndXmlSerializer-0.1.0/test/test_constants.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-15 15:04:56.619408 JsonAndXmlSerializer-0.1.1/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-15 15:04:56.619408 JsonAndXmlSerializer-0.1.1/JsonAndXmlSerializer.egg-info/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      321 2023-05-15 15:04:56.000000 JsonAndXmlSerializer-0.1.1/JsonAndXmlSerializer.egg-info/PKG-INFO
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      450 2023-05-15 15:04:56.000000 JsonAndXmlSerializer-0.1.1/JsonAndXmlSerializer.egg-info/SOURCES.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-05-15 15:04:56.000000 JsonAndXmlSerializer-0.1.1/JsonAndXmlSerializer.egg-info/dependency_links.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        6 2023-05-15 15:04:56.000000 JsonAndXmlSerializer-0.1.1/JsonAndXmlSerializer.egg-info/requires.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       11 2023-05-15 15:04:56.000000 JsonAndXmlSerializer-0.1.1/JsonAndXmlSerializer.egg-info/top_level.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      321 2023-05-15 15:04:56.619408 JsonAndXmlSerializer-0.1.1/PKG-INFO
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-15 15:04:56.619408 JsonAndXmlSerializer-0.1.1/Serializer/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      567 2023-05-15 15:03:43.000000 JsonAndXmlSerializer-0.1.1/Serializer/__init__.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      361 2023-05-14 10:14:56.000000 JsonAndXmlSerializer-0.1.1/Serializer/base_serializer.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1135 2023-05-13 12:56:57.000000 JsonAndXmlSerializer-0.1.1/Serializer/constants.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)    10165 2023-05-15 15:03:43.000000 JsonAndXmlSerializer-0.1.1/Serializer/dict_serializer.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     3946 2023-05-15 15:03:43.000000 JsonAndXmlSerializer-0.1.1/Serializer/json_serializer.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      511 2023-05-15 15:03:43.000000 JsonAndXmlSerializer-0.1.1/Serializer/serializers_factory.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     4094 2023-05-15 15:03:43.000000 JsonAndXmlSerializer-0.1.1/Serializer/xml_serializer.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       38 2023-05-15 15:04:56.619408 JsonAndXmlSerializer-0.1.1/setup.cfg
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      499 2023-05-15 15:04:15.000000 JsonAndXmlSerializer-0.1.1/setup.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-15 15:04:56.619408 JsonAndXmlSerializer-0.1.1/test/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      948 2023-05-14 16:23:30.000000 JsonAndXmlSerializer-0.1.1/test/test_constants.py
```

### Comparing `JsonAndXmlSerializer-0.1.0/Serializer/constants.py` & `JsonAndXmlSerializer-0.1.1/Serializer/constants.py`

 * *Files identical despite different names*

### Comparing `JsonAndXmlSerializer-0.1.0/Serializer/dict_serializer.py` & `JsonAndXmlSerializer-0.1.1/Serializer/dict_serializer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import inspect
 
-from Lab_3.Serializer.constants import nonetype, moduletype, codetype, celltype, functype, bldinfunctype, smethodtype, \
+from Serializer.constants import nonetype, moduletype, codetype, celltype, functype, bldinfunctype, smethodtype, \
     cmethodtype, mapproxytype, wrapdesctype, metdesctype, getsetdesctype, \
     CODE_PROPS, UNIQUE_TYPES
 
 
 class DictSerializer:
     TYPE_KW = "type"
     SOURCE_KW = "source"
@@ -65,82 +65,82 @@
         if type(obj) in (smethodtype, cmethodtype):
             return {cls.TYPE_KW: type(obj).__name__,
                     cls.SOURCE_KW: cls.to_dict(obj.__func__, is_inner_func)}
 
         if inspect.isroutine(obj): # Проверяет, является ли объект функцией или методом.
             source = {}
 
-            # Code cкомпилированный код
+            # Код cкомпилированный код
             source[cls.CODE_KW] = cls.to_dict(obj.__code__)
 
-            # Global vars
+            # Глоб переменные
             gvars = cls.__get_gvars(obj, is_inner_func)
             source[cls.GLOBALS_KW] = cls.to_dict(gvars)
 
-            # Name
+            # Имя
             source[cls.NAME_KW] = cls.to_dict(obj.__name__)
 
-            # Defaults
-            source[cls.DEFAULTS_KW] = cls.to_dict(obj.__defaults__) #кортеж значений по умолчанию аргументов функции
+            # Переменные по умолчанию
+            source[cls.DEFAULTS_KW] = cls.to_dict(obj.__defaults__) # кортеж значений по умолчанию аргументов функции
 
-            #Closure
+            # Замыкания
             source[cls.CLOSURE_KW] = cls.to_dict(obj.__closure__) # кортеж переменных из внешней области видимости, используемые в замыкании
 
             return {cls.TYPE_KW: functype.__name__,
                     cls.SOURCE_KW: source}
 
         elif inspect.isclass(obj):
             source = {}
 
-            # Name
+            # Имя
             source[cls.NAME_KW] = cls.to_dict(obj.__name__)
 
-            # Bases кортеж базовых классов (которых класс наследуется)
+            # Кортеж базовых классов (которых класс наследуется)
             source[cls.BASES_KW] = cls.to_dict(tuple(b for b in obj.__bases__ if b != object))
 
-            # Dict
+            # Словарь
             source[cls.DICT_KW] = cls.__get_obj_dict(obj)
 
             return {cls.TYPE_KW: type.__name__,
                     cls.SOURCE_KW: source}
 
         else:
             source = {}
 
-            # Class
+            # Класс
             source[cls.CLASS_KW] = cls.to_dict(obj.__class__)
 
-            # Dict
+            # Словарь
             source[cls.DICT_KW] = cls.__get_obj_dict(obj)
 
             return {cls.TYPE_KW: cls.OBJECT_KW,
                     cls.SOURCE_KW: source}
 
     @classmethod
     def __get_gvars(cls, func, is_inner_func):
         name = func.__name__
         gvars = {}
 
-        for gvar_name in func.__code__.co_name: # func.code.co_names: # кортеж имен всех переменных
-            # Separating the variables that the function needs
+        for gvar_name in func.__code__.co_name: # кортеж имен всех переменных
+            # Разделение переменных которая функция  использует
             if gvar_name in func.__globals__:
-                # Module
+                # Модуль
                 if type(func.__globals__[gvar_name]) is moduletype:
                     gvars[gvar_name] = func.__globals__[gvar_name]
 
-                # Class
+                # Класс
                 elif inspect.isclass(func.__globals__[gvar_name]):
                     # To prevent recursion, the class in which this method is declared is replaced with the
                     # name of the class. In the future, this name will be replaced by the class type
                     c = func.__globals__[gvar_name]  #значение глобальной переменной
                     if is_inner_func and name in c.__dict__ and func == c.__dict__[name].__func__:
                         gvars[gvar_name] = c.__name__
                     else:
                         gvars[gvar_name] = c
-                # Recursion protection
+                # Защита рекурсии
                 elif gvar_name == func.__code__.co_name:
                     gvars[gvar_name] = func.__name__
 
                 else:
                     gvars[gvar_name] = func.__globals__[gvar_name]
 
         return gvars
@@ -175,16 +175,14 @@
         else:
             obj_type = obj[cls.TYPE_KW]
             obj_source = obj[cls.SOURCE_KW]
 
             if obj_type == dict.__name__:
                 return cls.from_dict(obj_source, is_dict=True)
 
-            # Key - type name, value - type itself. Calling by type name returns that type.
-            # This is necessary for the same creation of simple collections.
             cols_dict = {t.__name__: t for t in [set, frozenset, tuple, bytes, bytearray]}
             if obj_type in cols_dict:
                 return cols_dict[obj_type](cls.from_dict(obj_source))
 
             if obj_type == complex.__name__:
                 return obj_source[complex.real.__name__] + \
                     obj_source[complex.imag.__name__] * 1j
@@ -207,15 +205,15 @@
             if obj_type == functype.__name__:
                 code = cls.from_dict(obj_source[cls.CODE_KW])
                 gvars = cls.from_dict(obj_source[cls.GLOBALS_KW])
                 name = cls.from_dict(obj_source[cls.NAME_KW])
                 defaults = cls.from_dict(obj_source[cls.DEFAULTS_KW])
                 closure = cls.from_dict(obj_source[cls.CLOSURE_KW])
 
-                # If there are suitable global variables, they are replaced.
+                # Если есть подходящие глобальные переменные, то они заменяются.
                 for key in gvars:
                     if key in code.co_name and key in globals(): #Возвращает словарь, содержащий глобальные переменные текущей области
                         gvars[key] = globals()[key]
 
                 func = functype(code, gvars, name, defaults, closure)
 
                 # Restoring recursion
@@ -228,15 +226,15 @@
                 name = cls.from_dict(obj_source[cls.NAME_KW])
                 bases = cls.from_dict(obj_source[cls.BASES_KW])
                 dct = obj_source[cls.DICT_KW]
                 dct = {cls.from_dict(item[0]): cls.from_dict(item[1]) for item in dct.items()}
 
                 cl = type(name, bases, dct)
 
-                # Restore a reference to the current class in the nested method __globals__
+                # Восстановить ссылку на текущий класс во вложенном методе __globals__
                 for attr in cl.__dict__.values():
                     if inspect.isroutine(attr):
                         if type(attr) in (smethodtype, classmethod):
                             fglobs = attr.__func__.__globals__
                         else:
                             fglobs = attr.__globals__
```

### Comparing `JsonAndXmlSerializer-0.1.0/Serializer/json_serializer.py` & `JsonAndXmlSerializer-0.1.1/Serializer/json_serializer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 import regex
-from Lab_3.Serializer.base_serializer import BaseSerializer
-from Lab_3.Serializer.dict_serializer import DictSerializer
+from Serializer.base_serializer import BaseSerializer
+from Serializer.dict_serializer import DictSerializer
 
-from Lab_3.Serializer.constants import nonetype
+from Serializer.constants import nonetype
 
 
 class JsonSerializer(BaseSerializer):
 
     INF_LITERAL = str(1E1000)
     NAN_LITERAL = str(1E1000 / 1E1000)
 
@@ -20,15 +20,14 @@
     FLOAT_PATTERN = fr"(?:[+-]?\d+(?:\.\d+)?(?:e[+-]?\d+)?|[+-]?{INF_LITERAL}\b|{NAN_LITERAL}\b)"
     BOOL_PATTERN = fr"({TRUE_LITERAL}|{FALSE_LITERAL})\b"
     STRING_PATTERN = fr"\"(?:(?:\\\")|[^\"])*\""
     NULL_PATTERN = fr"\b{NULL_LITERAL}\b"
 
     ELEMENTARY_TYPES_PATTERN = fr"{FLOAT_PATTERN}|{INT_PATTERN}|{BOOL_PATTERN}|{STRING_PATTERN}|{NULL_PATTERN}"
 
-    # This regex use recursive statements to be able to capture nested lists and objects.
     ARRAY_PATTERN = r"\[(?R)?(?:,(?R))*\]"
     OBJECT_PATTERN = r"\{(?:(?R):(?R))?(?:,(?R):(?R))*\}"
 
     VALUE_PATTERN = fr"\s*({ELEMENTARY_TYPES_PATTERN}|" + \
                     fr"{ARRAY_PATTERN}|{OBJECT_PATTERN})\s*"
 
     def dumps(self, obj) -> str:
@@ -58,15 +57,15 @@
             raise ValueError
 
     def loads(self, string: str):
         obj = self.__loads_to_dict(string)
         return DictSerializer.from_dict(obj)
 
     def __loads_to_dict(self, string: str):
-        string = string.strip() # удаляет начальные и конечные пробелы
+        string = string.strip()
 
         # Int
         match = re.fullmatch(self.INT_PATTERN, string)
         if match:
             return int(match.group(0))
 
         # Float
@@ -98,16 +97,16 @@
             return [self.__loads_to_dict(match[0]) for match in matches]
 
         # Dict
         if string[0] == '{' and string[-1] == '}':
             string = string[1:-1]
             matches = regex.findall(self.VALUE_PATTERN, string)
 
-            # Variable matches will store key-value pairs in one row. Elements with
-            # even indexes are keys, those with odd indexes are values.
+            # Совпадения переменных будут хранить пары ключ-значение в одной строке. Элементы с
+            # четные индексы являются ключами, а нечетные - значениями.
             return {self.__loads_to_dict(matches[i][0]):
                     self.__loads_to_dict(matches[i + 1][0]) for i in range(0, len(matches), 2)}
 
         else:
             raise ValueError
 
     @staticmethod
```

### Comparing `JsonAndXmlSerializer-0.1.0/Serializer/xml_serializer.py` & `JsonAndXmlSerializer-0.1.1/Serializer/xml_serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 
 import regex
-from Lab_3.Serializer.base_serializer import BaseSerializer
-from Lab_3.Serializer.dict_serializer import DictSerializer
+from Serializer.base_serializer import BaseSerializer
+from Serializer.dict_serializer import DictSerializer
 
-from Lab_3.Serializer.constants import nonetype
+from Serializer.constants import nonetype
 
 
 class XmlSerializer(BaseSerializer):
 
     NONE_LITERAL = "null"
 
     KEY_GROUP_NAME = "key"
```

### Comparing `JsonAndXmlSerializer-0.1.0/test/test_constants.py` & `JsonAndXmlSerializer-0.1.1/test/test_constants.py`

 * *Files identical despite different names*

