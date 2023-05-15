# Comparing `tmp/yyjson-1.0.1.tar.gz` & `tmp/yyjson-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yyjson-1.0.1.tar", last modified: Mon Jun 13 05:18:35 2022, max compression
+gzip compressed data, was "yyjson-2.0.2.tar", last modified: Mon May 15 12:33:11 2023, max compression
```

## Comparing `yyjson-1.0.1.tar` & `yyjson-2.0.2.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 05:18:35.770998 yyjson-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)     2260 2022-06-13 05:18:10.000000 yyjson-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-06-13 05:18:10.000000 yyjson-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3211 2022-06-13 05:18:35.770998 yyjson-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2646 2022-06-13 05:18:10.000000 yyjson-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-06-13 05:18:35.770998 yyjson-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1445 2022-06-13 05:18:10.000000 yyjson-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 05:18:35.770998 yyjson-1.0.1/yyjson/
--rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-06-13 05:18:10.000000 yyjson-1.0.1/yyjson/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      686 2022-06-13 05:18:10.000000 yyjson-1.0.1/yyjson/binding.c
--rw-r--r--   0 runner    (1001) docker     (121)    24464 2022-06-13 05:18:10.000000 yyjson-1.0.1/yyjson/document.c
--rw-r--r--   0 runner    (1001) docker     (121)      521 2022-06-13 05:18:10.000000 yyjson-1.0.1/yyjson/memory.c
--rw-r--r--   0 runner    (1001) docker     (121)   300466 2022-06-13 05:18:10.000000 yyjson-1.0.1/yyjson/yyjson.c
--rw-r--r--   0 runner    (1001) docker     (121)   209548 2022-06-13 05:18:10.000000 yyjson-1.0.1/yyjson/yyjson.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 05:18:35.770998 yyjson-1.0.1/yyjson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3211 2022-06-13 05:18:35.000000 yyjson-1.0.1/yyjson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      328 2022-06-13 05:18:35.000000 yyjson-1.0.1/yyjson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-13 05:18:35.000000 yyjson-1.0.1/yyjson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-13 05:18:20.000000 yyjson-1.0.1/yyjson.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-06-13 05:18:35.000000 yyjson-1.0.1/yyjson.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-06-13 05:18:35.000000 yyjson-1.0.1/yyjson.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:33:11.843392 yyjson-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-15 12:32:43.000000 yyjson-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-15 12:32:43.000000 yyjson-2.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-15 12:33:11.843392 yyjson-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-15 12:32:43.000000 yyjson-2.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-15 12:33:11.843392 yyjson-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-15 12:32:43.000000 yyjson-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:33:11.843392 yyjson-2.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-05-15 12:32:43.000000 yyjson-2.0.2/tests/test_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-15 12:32:43.000000 yyjson-2.0.2/tests/test_merge_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-15 12:32:43.000000 yyjson-2.0.2/tests/test_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:33:11.843392 yyjson-2.0.2/yyjson/
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-15 12:32:43.000000 yyjson-2.0.2/yyjson/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-15 12:32:43.000000 yyjson-2.0.2/yyjson/binding.c
+-rw-r--r--   0 runner    (1001) docker     (123)    26819 2023-05-15 12:32:43.000000 yyjson-2.0.2/yyjson/document.c
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-15 12:32:43.000000 yyjson-2.0.2/yyjson/memory.c
+-rw-r--r--   0 runner    (1001) docker     (123)   338960 2023-05-15 12:32:43.000000 yyjson-2.0.2/yyjson/yyjson.c
+-rw-r--r--   0 runner    (1001) docker     (123)   291337 2023-05-15 12:32:43.000000 yyjson-2.0.2/yyjson/yyjson.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:33:11.843392 yyjson-2.0.2/yyjson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-15 12:33:11.000000 yyjson-2.0.2/yyjson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-15 12:33:11.000000 yyjson-2.0.2/yyjson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:33:11.000000 yyjson-2.0.2/yyjson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:32:52.000000 yyjson-2.0.2/yyjson.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-15 12:33:11.000000 yyjson-2.0.2/yyjson.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-15 12:33:11.000000 yyjson-2.0.2/yyjson.egg-info/top_level.txt
```

### Comparing `yyjson-1.0.1/LICENSE` & `yyjson-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yyjson-1.0.1/yyjson/__init__.py` & `yyjson-2.0.2/yyjson/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class ReaderFlags(enum.IntFlag):
     """
     Flags that can be passed into JSON reading functions to control parsing
     behaviour.
     """
     #: Stop when done instead of issues an error if there's additional content
     #: after a JSON document. This option may be used to parse small pieces of
-    # JSON in larger data, such as NDJSON.
+    #: JSON in larger data, such as NDJSON.
     STOP_WHEN_DONE = 0x02
     #: Allow single trailing comma at the end of an object or array, such as
     #: [1,2,3,] {"a":1,"b":2,}.
     ALLOW_TRAILING_COMMAS = 0x04
     #: Allow C-style single line and multiple line comments.
     ALLOW_COMMENTS = 0x08
     #: Allow inf/nan number and literal, case-insensitive, such as 1e999, NaN,
@@ -34,14 +34,17 @@
 class WriterFlags(enum.IntFlag):
     """
     Flags that can be passed into JSON writing functions to control writing
     behaviour.
     """
     #: Write the JSON with 4-space indents and newlines.
     PRETTY = 0x01
+    #: Write JSON pretty with 2 space indent. This flag will override
+    #: the PRETTY flag.
+    PRETTY_TWO_SPACES = 0x40
     #: Escapes unicode as \uXXXXX so that all output is ASCII.
     ESCAPE_UNICODE = 0x02
     #: Escapes / as \/.
     ESCAPE_SLASHES = 0x04
     #: Writes Infinity and NaN.
     ALLOW_INF_AND_NAN = 0x08
     #: Writes Infinity and NaN as `null` instead of raising an error.
```

### Comparing `yyjson-1.0.1/yyjson/binding.c` & `yyjson-2.0.2/yyjson/binding.c`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 #define PY_SSIZE_T_CLEAN
 #include <Python.h>
-#include "yyjson.h"
-#include "memory.h"
+
 #include "document.h"
+#include "memory.h"
+#include "yyjson.h"
 
 static PyModuleDef yymodule = {
-    PyModuleDef_HEAD_INIT,
-    .m_name = "cyyjson",
-    .m_doc = "Python bindings for the yyjson project.",
-    .m_size = -1
-};
-
-PyMODINIT_FUNC
-PyInit_cyyjson(void)
-{
-    PyObject *m;
-    if (PyType_Ready(&DocumentType) < 0) {
-        return NULL;
-    }
-
-    m = PyModule_Create(&yymodule);
-    if (m == NULL) {
-        return NULL;
-    }
-
-    Py_INCREF(&DocumentType);
-    if (PyModule_AddObject(m, "Document", (PyObject *)&DocumentType) < 0) {
-        Py_DECREF(&DocumentType);
-        Py_DECREF(m);
-        return NULL;
-    }
+    PyModuleDef_HEAD_INIT, .m_name = "cyyjson",
+    .m_doc = "Python bindings for the yyjson project.", .m_size = -1};
+
+PyMODINIT_FUNC PyInit_cyyjson(void) {
+  PyObject* m;
+
+  if (PyType_Ready(&DocumentType) < 0) {
+    return NULL;
+  }
+
+  m = PyModule_Create(&yymodule);
+  if (m == NULL) {
+    return NULL;
+  }
+
+  Py_INCREF(&DocumentType);
+  if (PyModule_AddObject(m, "Document", (PyObject*)&DocumentType) < 0) {
+    Py_DECREF(&DocumentType);
+    Py_DECREF(m);
+    return NULL;
+  }
 
-    return m;
+  return m;
 }
```

### Comparing `yyjson-1.0.1/yyjson/document.c` & `yyjson-2.0.2/yyjson/document.c`

 * *Files 14% similar despite different names*

```diff
@@ -1,459 +1,472 @@
-#include "memory.h"
 #include "document.h"
 
-#define ENSURE_MUTABLE(self) \
-    if (self->i_doc) { \
-        self->m_doc = yyjson_doc_mut_copy(self->i_doc, self->alc); \
-        yyjson_doc_free(self->i_doc); \
-    }
+#include "memory.h"
 
-static inline PyObject * element_to_primitive(yyjson_val *val);
-static inline PyObject * mut_element_to_primitive(yyjson_mut_val *val);
+#define ENSURE_MUTABLE(self)                                   \
+  if (self->i_doc) {                                           \
+    self->m_doc = yyjson_doc_mut_copy(self->i_doc, self->alc); \
+    yyjson_doc_free(self->i_doc);                              \
+    self->i_doc = NULL;                                        \
+  }
+
+static inline PyObject* mut_element_to_primitive(yyjson_mut_val* val);
+static inline PyObject* element_to_primitive(yyjson_val* val);
 
 /**
  * Recursively convert the given value into an equivalent high-level Python
  * object.
  **/
-static inline PyObject *
-mut_element_to_primitive(yyjson_mut_val *val)
-{
-    yyjson_type type = yyjson_mut_get_type(val);
-
-    switch (type) {
-        case YYJSON_TYPE_NULL:
-            Py_RETURN_NONE;
-        case YYJSON_TYPE_BOOL:
-            if (yyjson_mut_get_subtype(val) == YYJSON_SUBTYPE_TRUE) {
-                Py_RETURN_TRUE;
-            } else {
-                Py_RETURN_FALSE;
-            }
-        case YYJSON_TYPE_NUM:
-        {
-            switch (yyjson_mut_get_subtype(val)) {
-                case YYJSON_SUBTYPE_UINT:
-                    return PyLong_FromUnsignedLongLong(yyjson_mut_get_uint(val));
-                case YYJSON_SUBTYPE_SINT:
-                    return PyLong_FromLongLong(yyjson_mut_get_sint(val));
-                case YYJSON_SUBTYPE_REAL:
-                    return PyFloat_FromDouble(yyjson_mut_get_real(val));
-            }
-        }
-        case YYJSON_TYPE_STR:
-        {
-            size_t str_len = yyjson_mut_get_len(val);
-            const char *str = yyjson_mut_get_str(val);
+static inline PyObject* element_to_primitive(yyjson_val* val) {
+  yyjson_type type = yyjson_get_type(val);
 
-            return PyUnicode_FromStringAndSize(str, str_len);
+  switch (type) {
+    case YYJSON_TYPE_NULL:
+      Py_RETURN_NONE;
+    case YYJSON_TYPE_BOOL:
+      if (yyjson_get_subtype(val) == YYJSON_SUBTYPE_TRUE) {
+        Py_RETURN_TRUE;
+      } else {
+        Py_RETURN_FALSE;
+      }
+    case YYJSON_TYPE_NUM: {
+      switch (yyjson_get_subtype(val)) {
+        case YYJSON_SUBTYPE_UINT:
+          return PyLong_FromUnsignedLongLong(yyjson_get_uint(val));
+        case YYJSON_SUBTYPE_SINT:
+          return PyLong_FromLongLong(yyjson_get_sint(val));
+        case YYJSON_SUBTYPE_REAL:
+          return PyFloat_FromDouble(yyjson_get_real(val));
+      }
+    }
+    case YYJSON_TYPE_STR: {
+      size_t str_len = yyjson_get_len(val);
+      const char* str = yyjson_get_str(val);
+
+      return PyUnicode_FromStringAndSize(str, str_len);
+    }
+    case YYJSON_TYPE_ARR: {
+      PyObject* arr = PyList_New(yyjson_arr_size(val));
+      if (!arr) {
+        return NULL;
+      }
+
+      yyjson_val* obj_val;
+      PyObject* py_val;
+
+      yyjson_arr_iter iter = {0};
+      yyjson_arr_iter_init(val, &iter);
+
+      size_t idx = 0;
+      while ((obj_val = yyjson_arr_iter_next(&iter))) {
+        py_val = element_to_primitive(obj_val);
+        if (!py_val) {
+          return NULL;
         }
-        case YYJSON_TYPE_ARR:
-        {
-            PyObject *arr = PyList_New(yyjson_mut_arr_size(val));
-            if (!arr) {
-                return NULL;
-            }
-
-            yyjson_mut_val *obj_val;
-            PyObject *py_val;
-
-            yyjson_mut_arr_iter iter = {0};
-            yyjson_mut_arr_iter_init(val, &iter);
-
-            size_t idx = 0;
-            while ((obj_val = yyjson_mut_arr_iter_next(&iter))) {
-                py_val = mut_element_to_primitive(obj_val);
-                if (!py_val) {
-                    return NULL;
-                }
 
-                PyList_SET_ITEM(arr, idx++, py_val);
-            }
+        PyList_SET_ITEM(arr, idx++, py_val);
+      }
 
-            return arr;
+      return arr;
+    }
+    case YYJSON_TYPE_OBJ: {
+      PyObject* dict = PyDict_New();
+      if (!dict) {
+        return NULL;
+      }
+
+      yyjson_val *obj_key, *obj_val;
+      PyObject *py_key, *py_val;
+
+      yyjson_obj_iter iter = {0};
+      yyjson_obj_iter_init(val, &iter);
+
+      while ((obj_key = yyjson_obj_iter_next(&iter))) {
+        obj_val = yyjson_obj_iter_get_val(obj_key);
+
+        py_key = element_to_primitive(obj_key);
+        py_val = element_to_primitive(obj_val);
+
+        if (!py_key) {
+          return NULL;
         }
-        case YYJSON_TYPE_OBJ:
-        {
-            PyObject *dict = PyDict_New();
-            if (!dict) {
-                return NULL;
-            }
-
-            yyjson_mut_val *obj_key, *obj_val;
-            PyObject *py_key, *py_val;
-
-            yyjson_mut_obj_iter iter = {0};
-            yyjson_mut_obj_iter_init(val, &iter);
-
-            while ((obj_key = yyjson_mut_obj_iter_next(&iter))) {
-                obj_val = yyjson_mut_obj_iter_get_val(obj_key);
-
-                py_key = mut_element_to_primitive(obj_key);
-                py_val = mut_element_to_primitive(obj_val);
-
-                if (!py_key) {
-                    return NULL;
-                }
-
-                if (!py_val) {
-                    Py_DECREF(py_key);
-                    return NULL;
-                }
-
-                if(PyDict_SetItem(dict, py_key, py_val) == -1) {
-                    return NULL;
-                }
-
-                Py_DECREF(py_key);
-                Py_DECREF(py_val);
-            }
-            return dict;
+
+        if (!py_val) {
+          Py_DECREF(py_key);
+          return NULL;
+        }
+
+        if (PyDict_SetItem(dict, py_key, py_val) == -1) {
+          return NULL;
         }
-        case YYJSON_TYPE_RAW:
-            return PyLong_FromString(yyjson_mut_get_raw(val), NULL, 10);
-        case YYJSON_TYPE_NONE:
-        default:
-            PyErr_SetString(PyExc_TypeError, "Unknown tape type encountered.");
-            return NULL;
+
+        Py_DECREF(py_key);
+        Py_DECREF(py_val);
+      }
+      return dict;
     }
+    case YYJSON_TYPE_RAW:
+      return PyLong_FromString(yyjson_get_raw(val), NULL, 10);
+    case YYJSON_TYPE_NONE:
+    default:
+      PyErr_SetString(PyExc_TypeError, "Unknown tape type encountered.");
+      return NULL;
+  }
 }
 
 /**
  * Recursively convert the given value into an equivalent high-level Python
  * object.
  **/
-static inline PyObject *
-element_to_primitive(yyjson_val *val)
-{
-    yyjson_type type = yyjson_get_type(val);
-
-    switch (type) {
-        case YYJSON_TYPE_NULL:
-            Py_RETURN_NONE;
-        case YYJSON_TYPE_BOOL:
-            if (yyjson_get_subtype(val) == YYJSON_SUBTYPE_TRUE) {
-                Py_RETURN_TRUE;
-            } else {
-                Py_RETURN_FALSE;
-            }
-        case YYJSON_TYPE_NUM:
-        {
-            switch (yyjson_get_subtype(val)) {
-                case YYJSON_SUBTYPE_UINT:
-                    return PyLong_FromUnsignedLongLong(yyjson_get_uint(val));
-                case YYJSON_SUBTYPE_SINT:
-                    return PyLong_FromLongLong(yyjson_get_sint(val));
-                case YYJSON_SUBTYPE_REAL:
-                    return PyFloat_FromDouble(yyjson_get_real(val));
-            }
-        }
-        case YYJSON_TYPE_STR:
-        {
-            size_t str_len = yyjson_get_len(val);
-            const char *str = yyjson_get_str(val);
+static inline PyObject* mut_element_to_primitive(yyjson_mut_val* val) {
+  yyjson_type type = yyjson_mut_get_type(val);
 
-            return PyUnicode_FromStringAndSize(str, str_len);
-        }
-        case YYJSON_TYPE_ARR:
-        {
-            PyObject *arr = PyList_New(yyjson_arr_size(val));
-            if (!arr) {
-                return NULL;
-            }
-
-            yyjson_val *obj_val;
-            PyObject *py_val;
-
-            yyjson_arr_iter iter = {0};
-            yyjson_arr_iter_init(val, &iter);
-
-            size_t idx = 0;
-            while ((obj_val = yyjson_arr_iter_next(&iter))) {
-                py_val = element_to_primitive(obj_val);
-                if (!py_val) {
-                    return NULL;
-                }
+  switch (type) {
+    case YYJSON_TYPE_NULL:
+      Py_RETURN_NONE;
+    case YYJSON_TYPE_BOOL:
+      if (yyjson_mut_get_subtype(val) == YYJSON_SUBTYPE_TRUE) {
+        Py_RETURN_TRUE;
+      } else {
+        Py_RETURN_FALSE;
+      }
+    case YYJSON_TYPE_NUM: {
+      switch (yyjson_mut_get_subtype(val)) {
+        case YYJSON_SUBTYPE_UINT:
+          return PyLong_FromUnsignedLongLong(yyjson_mut_get_uint(val));
+        case YYJSON_SUBTYPE_SINT:
+          return PyLong_FromLongLong(yyjson_mut_get_sint(val));
+        case YYJSON_SUBTYPE_REAL:
+          return PyFloat_FromDouble(yyjson_mut_get_real(val));
+      }
+    }
+    case YYJSON_TYPE_STR: {
+      size_t str_len = yyjson_mut_get_len(val);
+      const char* str = yyjson_mut_get_str(val);
+
+      return PyUnicode_FromStringAndSize(str, str_len);
+    }
+    case YYJSON_TYPE_ARR: {
+      PyObject* arr = PyList_New(yyjson_mut_arr_size(val));
+      if (!arr) {
+        return NULL;
+      }
 
-                PyList_SET_ITEM(arr, idx++, py_val);
-            }
+      yyjson_mut_val* obj_val;
+      PyObject* py_val;
 
-            return arr;
-        }
-        case YYJSON_TYPE_OBJ:
-        {
-            PyObject *dict = PyDict_New();
-            if (!dict) {
-                return NULL;
-            }
-
-            yyjson_val *obj_key, *obj_val;
-            PyObject *py_key, *py_val;
-
-            yyjson_obj_iter iter = {0};
-            yyjson_obj_iter_init(val, &iter);
-
-            while ((obj_key = yyjson_obj_iter_next(&iter))) {
-                obj_val = yyjson_obj_iter_get_val(obj_key);
-
-                py_key = element_to_primitive(obj_key);
-                py_val = element_to_primitive(obj_val);
-
-                if (!py_key) {
-                    return NULL;
-                }
-
-                if (!py_val) {
-                    Py_DECREF(py_key);
-                    return NULL;
-                }
-
-                if(PyDict_SetItem(dict, py_key, py_val) == -1) {
-                    return NULL;
-                }
-
-                Py_DECREF(py_key);
-                Py_DECREF(py_val);
-            }
-            return dict;
+      yyjson_mut_arr_iter iter = {0};
+      yyjson_mut_arr_iter_init(val, &iter);
+
+      size_t idx = 0;
+      while ((obj_val = yyjson_mut_arr_iter_next(&iter))) {
+        py_val = mut_element_to_primitive(obj_val);
+        if (!py_val) {
+          return NULL;
         }
-        case YYJSON_TYPE_RAW:
-            return PyLong_FromString(yyjson_get_raw(val), NULL, 10);
-        case YYJSON_TYPE_NONE:
-        default:
-            PyErr_SetString(PyExc_TypeError, "Unknown tape type encountered.");
-            return NULL;
-    }
-}
 
+        PyList_SET_ITEM(arr, idx++, py_val);
+      }
 
-PyTypeObject *type_for_conversion(PyObject *obj) {
-    if (obj->ob_type == &PyUnicode_Type) {
-        return &PyUnicode_Type;
-    } else if (obj->ob_type == &PyLong_Type) {
-        return &PyLong_Type;
-    } else if (obj->ob_type == &PyFloat_Type) {
-        return &PyFloat_Type;
-    } else if (obj->ob_type == &PyDict_Type) {
-        return &PyDict_Type;
-    } else if (obj->ob_type == &PyList_Type) {
-        return &PyList_Type;
-    } else if (obj->ob_type == &PyBool_Type) {
-        return &PyBool_Type;
-    } else if (obj->ob_type == Py_None->ob_type) {
-        return Py_None->ob_type;
+      return arr;
     }
-    return NULL;
-}
+    case YYJSON_TYPE_OBJ: {
+      PyObject* dict = PyDict_New();
+      if (!dict) {
+        return NULL;
+      }
 
+      yyjson_mut_val *obj_key, *obj_val;
+      PyObject *py_key, *py_val;
+
+      yyjson_mut_obj_iter iter = {0};
+      yyjson_mut_obj_iter_init(val, &iter);
+
+      while ((obj_key = yyjson_mut_obj_iter_next(&iter))) {
+        obj_val = yyjson_mut_obj_iter_get_val(obj_key);
+
+        py_key = mut_element_to_primitive(obj_key);
+        py_val = mut_element_to_primitive(obj_val);
+
+        if (!py_key) {
+          return NULL;
+        }
+
+        if (!py_val) {
+          Py_DECREF(py_key);
+          return NULL;
+        }
+
+        if (PyDict_SetItem(dict, py_key, py_val) == -1) {
+          return NULL;
+        }
+
+        Py_DECREF(py_key);
+        Py_DECREF(py_val);
+      }
+      return dict;
+    }
+    case YYJSON_TYPE_RAW:
+      return PyLong_FromString(yyjson_mut_get_raw(val), NULL, 10);
+    case YYJSON_TYPE_NONE:
+    default:
+      PyErr_SetString(PyExc_TypeError, "Unknown tape type encountered.");
+      return NULL;
+  }
+}
+
+PyTypeObject* type_for_conversion(PyObject* obj) {
+  if (obj->ob_type == &PyUnicode_Type) {
+    return &PyUnicode_Type;
+  } else if (obj->ob_type == &PyLong_Type) {
+    return &PyLong_Type;
+  } else if (obj->ob_type == &PyFloat_Type) {
+    return &PyFloat_Type;
+  } else if (obj->ob_type == &PyDict_Type) {
+    return &PyDict_Type;
+  } else if (obj->ob_type == &PyList_Type) {
+    return &PyList_Type;
+  } else if (obj->ob_type == &PyBool_Type) {
+    return &PyBool_Type;
+  } else if (obj->ob_type == Py_None->ob_type) {
+    return Py_None->ob_type;
+  }
+  return NULL;
+}
 
 /**
  * Recursively convert a Python object into yyjson elements.
  */
-static inline yyjson_mut_val *
-mut_primitive_to_element(yyjson_mut_doc *doc, PyObject *obj) {
-    const PyTypeObject *ob_type = type_for_conversion(obj);
-
-    if (ob_type == &PyUnicode_Type) {
-        Py_ssize_t str_len;
-        const char *str = PyUnicode_AsUTF8AndSize(obj, &str_len);
-        return yyjson_mut_strncpy(doc, str, str_len);
-    } else if (ob_type == &PyLong_Type) {
-        // Serialization of integers is a little special, since Python allows
-        // integers of (effectively) any size. While > 53bit is technically
-        // against the spec, at least 64bit is widely supported and the builtin
-        // Python JSON module supports integers of any size.
-        int overflow = 0;
-        const int64_t num = PyLong_AsLongLongAndOverflow(obj, &overflow);
-        if (!overflow) {
-            if (num == -1 && PyErr_Occurred()) return NULL;
-            return yyjson_mut_sint(doc, num);
-        } else {
-            // Number overflowed, try an unsigned long long.
-            const uint64_t unum = PyLong_AsUnsignedLongLong(obj);
-            if (unum == (uint64_t)-1 && PyErr_Occurred()) {
-                // Number might have been too large even for a unit64_t, resort
-                // to a raw type by converting the number to its string
-                // representation.
-                PyErr_Clear(); // Erase the OverflowError
-                PyObject *str_repr = PyObject_Str(obj);
-                Py_ssize_t str_len;
-                const char *str = PyUnicode_AsUTF8AndSize(str_repr, &str_len);
-                return yyjson_mut_rawncpy(doc, str, str_len);
-            } else {
-                return yyjson_mut_uint(doc, unum);
-            }
-        }
-    } else if (ob_type == &PyList_Type) {
-        yyjson_mut_val *val = yyjson_mut_arr(doc);
-        for (Py_ssize_t i = 0; i < PyList_GET_SIZE(obj); i++) {
-            yyjson_mut_arr_append(
-                val,
-                mut_primitive_to_element(doc, PyList_GET_ITEM(obj, i))
-            );
-        }
-        return val;
-    } else if (ob_type == &PyDict_Type) {
-        yyjson_mut_val *val = yyjson_mut_obj(doc);
-        Py_ssize_t i = 0;
-        PyObject *key, *value;
-        while (PyDict_Next(obj, &i, &key, &value)) {
-            yyjson_mut_obj_add(
-                val,
-                // TODO: Keys of valid JSON documents will always be a string,
-                // we should hot-path this.
-                mut_primitive_to_element(doc, key),
-                mut_primitive_to_element(doc, value)
-            );
-        }
-        return val;
-    } else if (ob_type == &PyFloat_Type) {
-        double dnum = PyFloat_AsDouble(obj);
-        if (dnum == -1 && PyErr_Occurred()) return NULL;
-        return yyjson_mut_real(doc, dnum);
-    } else if (obj == Py_True) {
-        return yyjson_mut_true(doc);
-    } else if (obj == Py_False) {
-        return yyjson_mut_false(doc);
-    } else if (obj == Py_None) {
-        return yyjson_mut_null(doc);
+static inline yyjson_mut_val* mut_primitive_to_element(yyjson_mut_doc* doc,
+                                                       PyObject* obj) {
+  const PyTypeObject* ob_type = type_for_conversion(obj);
+
+  if (ob_type == &PyUnicode_Type) {
+    Py_ssize_t str_len;
+    const char* str = PyUnicode_AsUTF8AndSize(obj, &str_len);
+    return yyjson_mut_strncpy(doc, str, str_len);
+  } else if (ob_type == &PyLong_Type) {
+    // Serialization of integers is a little special, since Python allows
+    // integers of (effectively) any size. While > 53bit is technically
+    // against the spec, at least 64bit is widely supported and the builtin
+    // Python JSON module supports integers of any size.
+    int overflow = 0;
+    const int64_t num = PyLong_AsLongLongAndOverflow(obj, &overflow);
+    if (!overflow) {
+      if (num == -1 && PyErr_Occurred()) return NULL;
+      return yyjson_mut_sint(doc, num);
     } else {
-        PyErr_SetString(
-            PyExc_TypeError,
-            // TODO: We can provide a much better error here. Also add support
-            // for a default hook.
-            "Tried to serialize an object we don't know how to handle."
-        );
-        return NULL;
-    }
+      // Number overflowed, try an unsigned long long.
+      const uint64_t unum = PyLong_AsUnsignedLongLong(obj);
+      if (unum == (uint64_t)-1 && PyErr_Occurred()) {
+        // Number might have been too large even for a unit64_t, resort
+        // to a raw type by converting the number to its string
+        // representation.
+        PyErr_Clear();  // Erase the OverflowError
+        PyObject* str_repr = PyObject_Str(obj);
+        Py_ssize_t str_len;
+        const char* str = PyUnicode_AsUTF8AndSize(str_repr, &str_len);
+        return yyjson_mut_rawncpy(doc, str, str_len);
+      } else {
+        return yyjson_mut_uint(doc, unum);
+      }
+    }
+  } else if (ob_type == &PyList_Type) {
+    yyjson_mut_val* val = yyjson_mut_arr(doc);
+    for (Py_ssize_t i = 0; i < PyList_GET_SIZE(obj); i++) {
+      yyjson_mut_arr_append(
+          val, mut_primitive_to_element(doc, PyList_GET_ITEM(obj, i)));
+    }
+    return val;
+  } else if (ob_type == &PyDict_Type) {
+    yyjson_mut_val* val = yyjson_mut_obj(doc);
+    Py_ssize_t i = 0;
+    PyObject *key, *value;
+    while (PyDict_Next(obj, &i, &key, &value)) {
+      Py_ssize_t str_len;
+      const char* str = PyUnicode_AsUTF8AndSize(key, &str_len);
+
+      yyjson_mut_obj_add(val,
+                         yyjson_mut_strncpy(doc, str, str_len),
+                         mut_primitive_to_element(doc, value));
+    }
+    return val;
+  } else if (ob_type == &PyFloat_Type) {
+    double dnum = PyFloat_AsDouble(obj);
+    if (dnum == -1 && PyErr_Occurred()) return NULL;
+    return yyjson_mut_real(doc, dnum);
+  } else if (obj == Py_True) {
+    return yyjson_mut_true(doc);
+  } else if (obj == Py_False) {
+    return yyjson_mut_false(doc);
+  } else if (obj == Py_None) {
+    return yyjson_mut_null(doc);
+  } else {
+    PyErr_SetString(
+        PyExc_TypeError,
+        // TODO: We can provide a much better error here. Also add support
+        // for a default hook.
+        "Tried to serialize an object we don't know how to handle.");
+    return NULL;
+  }
 }
 
-static void
-Document_dealloc(DocumentObject *self)
-{
-    if (self->i_doc != NULL) yyjson_doc_free(self->i_doc);
-    if (self->m_doc != NULL) yyjson_mut_doc_free(self->m_doc);
-    Py_TYPE(self)->tp_free((PyObject *) self);
-}
-
-static PyObject *
-Document_new(PyTypeObject *type, PyObject *args, PyObject *kwds)
-{
-    DocumentObject *self;
-    self = (DocumentObject *) type->tp_alloc(type, 0);
-
-    if (self != NULL) {
-        self->i_doc = NULL;
-        self->m_doc = NULL;
-        self->alc = &PyMem_Allocator;
-    }
+static void Document_dealloc(DocumentObject* self) {
+  if (self->i_doc != NULL) yyjson_doc_free(self->i_doc);
+  if (self->m_doc != NULL) yyjson_mut_doc_free(self->m_doc);
+  Py_TYPE(self)->tp_free((PyObject*)self);
+}
+
+static PyObject* Document_new(PyTypeObject* type, PyObject* args,
+                              PyObject* kwds) {
+  DocumentObject* self;
+  self = (DocumentObject*)type->tp_alloc(type, 0);
+
+  if (self != NULL) {
+    self->m_doc = NULL;
+    self->i_doc = NULL;
+    self->alc = &PyMem_Allocator;
+  }
 
-    return (PyObject *) self;
+  return (PyObject*)self;
 }
 
 PyDoc_STRVAR(
     Document_init_doc,
     "A single JSON document.\n"
     "\n"
     "A `Document` can be built from a JSON-serializable Python object,\n"
-    "a JSON document in a ``str``, or a JSON document encoded to ``bytes``.\n"
+    "a JSON document in a ``str``, a JSON document encoded to ``bytes``,\n"
+    "or a ``Path()`` object to read a file from disk.\n"
     "Ex:\n"
     "\n"
     ".. doctest::\n"
     "\n"
     "   >>> Document({'a': 1, 'b': 2})\n"
     "   >>> Document(b'{\"a\": 1, \"b\": 2}')\n"
     "   >>> Document('{\"a\": 1, \"b\": 2}')\n"
+    "   >>> Document(Path('path/to/file.json'))\n"
     "\n"
     "By default, the parsing is strict and follows the JSON specifications.\n"
     "You can change this behaviour by passing in :class:`ReaderFlags`. Ex:\n"
     "\n"
     ".. doctest::\n"
     "\n"
     "   >>> Document('''{\n"
     "   ...     // Comments in JSON!?!?\n"
     "   ...     \"a\": 1\n"
     "   ... }''', flags=ReaderFlags.ALLOW_COMMENTS)\n"
     "\n"
+    ".. note::\n"
+    "\n"
+    "   yyjson has distinct APIs and data structures for mutable and immutable\n"
+    "   documents. This class is a wrapper around both of them, and will\n"
+    "   automatically convert between them as needed.\n"
+    "\n"
     ":param content: The initial content of the document.\n"
-    ":type content: A JSON ``str`` or ``bytes``, or a Python object that can\n"
-    "               be serialized.\n"
+    ":type content: ``str``, ``bytes``, ``Path``, ``dict``, ``list``\n"
     ":param flags: Flags that modify the document parsing behaviour.\n"
-    ":type flags: :class:`ReaderFlags`, optional"
-);
-static int
-Document_init(DocumentObject *self, PyObject *args, PyObject *kwds)
-{
-    static char *kwlist[] = {"content", "flags", NULL};
-    PyObject *content;
-    yyjson_read_err err;
-    yyjson_read_flag r_flag = 0;
-
-    if(!PyArg_ParseTupleAndKeywords(
-            args,
-            kwds,
-            "O|$I",
-            kwlist,
-            &content,
-            &r_flag
-        )) {
-        return -1;
-    }
-
-    // We were given a string, so just parse it into an immutable document.
-    if (PyUnicode_Check(content) || PyBytes_Check(content)) {
-        Py_ssize_t content_len;
-        const char *content_as_utf8 = NULL;
-
-        if (PyUnicode_Check(content)) {
-            content_as_utf8 = PyUnicode_AsUTF8AndSize(content, &content_len);
-        } else {
-            PyBytes_AsStringAndSize(content, (char **)&content_as_utf8, &content_len);
-        }
+    ":type flags: :class:`ReaderFlags`, optional");
+static int Document_init(DocumentObject* self, PyObject* args, PyObject* kwds) {
+  static char* kwlist[] = {"content", "flags", NULL};
+  PyObject* content;
+  yyjson_read_err err;
+  yyjson_read_flag r_flag = 0;
 
-        self->i_doc = yyjson_read_opts(
-            // As long as we don't expose the insitu reader flag, it's safe to
-            // discard the const here.
-            (char *)content_as_utf8,
-            content_len,
-            r_flag,
-            self->alc,
-            &err
-        );
-
-        if (!self->i_doc) {
-            // TODO: Error conversion! ValueError is not always the right
-            // choice, although JSONDecodeError is a ValueError subclass.
-            PyErr_SetString(PyExc_ValueError, err.msg);
-            return -1;
-        }
+  if (!PyArg_ParseTupleAndKeywords(args, kwds, "O|$I", kwlist, &content,
+                                   &r_flag)) {
+    return -1;
+  }
+
+  PyObject* pathlib = PyImport_ImportModule("pathlib");
+  PyObject* path = PyObject_GetAttrString(pathlib, "Path");
+
+  if (PyObject_IsInstance(content, path)) {
+    // We were given a Path object to a location on disk.
+    PyObject* as_str = PyObject_Str(content);
+    if (!as_str) {
+      return -1;
+    }
+
+    Py_ssize_t str_len;
+    const char* str = PyUnicode_AsUTF8AndSize(as_str, &str_len);
+    if (!str) {
+      Py_XDECREF(as_str);
+      return -1;
+    }
+
+    self->i_doc = yyjson_read_file(str, r_flag, self->alc, &err);
+
+    Py_XDECREF(as_str);
+    Py_XDECREF(str);
+
+    if (!self->i_doc) {
+      PyErr_SetString(PyExc_ValueError, err.msg);
+      return -1;
+    }
+
+    return 0;
+  } else if (PyUnicode_Check(content) || PyBytes_Check(content)) {
+    // We were given a string, so just parse it into a document.
+    Py_ssize_t content_len;
+    const char* content_as_utf8 = NULL;
+
+    if (PyUnicode_Check(content)) {
+      content_as_utf8 = PyUnicode_AsUTF8AndSize(content, &content_len);
     } else {
-        self->m_doc = yyjson_mut_doc_new(self->alc);
-        yyjson_mut_val *val = mut_primitive_to_element(self->m_doc, content);
-        if (val == NULL) {
-            return -1;
-        }
-        yyjson_mut_doc_set_root(self->m_doc, val);
+      PyBytes_AsStringAndSize(content, (char**)&content_as_utf8, &content_len);
+    }
+
+    self->i_doc = yyjson_read_opts(
+        // As long as we don't expose the insitu reader flag, it's safe to
+        // discard the const here.
+        (char*)content_as_utf8, content_len, r_flag, self->alc, &err);
+
+    if (!self->i_doc) {
+      PyErr_SetString(PyExc_ValueError, err.msg);
+      return -1;
     }
 
     return 0;
+  } else {
+    self->m_doc = yyjson_mut_doc_new(self->alc);
+
+    if (!self->m_doc) {
+      PyErr_SetString(PyExc_ValueError,
+                      "Unable to create empty mutable document.");
+      return -1;
+    }
+
+    yyjson_mut_val* val = mut_primitive_to_element(self->m_doc, content);
+    if (val == NULL) {
+      return -1;
+    }
+
+    yyjson_mut_doc_set_root(self->m_doc, val);
+  }
+
+  return 0;
 }
 
 /**
  * Recursively convert the document into Python objects.
  */
-static PyObject *
-Document_as_obj(DocumentObject *self, void* closure)
-{
-    if (self->i_doc != NULL) {
-        yyjson_val *root = yyjson_doc_get_root(self->i_doc);
-        return element_to_primitive(root);
-    } else {
-        yyjson_mut_val *root = yyjson_mut_doc_get_root(self->m_doc);
-        return mut_element_to_primitive(root);
-    }
+static PyObject* Document_as_obj(DocumentObject* self, void* closure) {
+  if (self->i_doc) {
+    return element_to_primitive(yyjson_doc_get_root(self->i_doc));
+  } else {
+    return mut_element_to_primitive(yyjson_mut_doc_get_root(self->m_doc));
+  }
+}
+
+/**
+ * Is the document mutable?
+ */
+static PyObject* Document_is_thawed(DocumentObject* self, void* closure) {
+  return PyBool_FromLong(self->m_doc != NULL);
 }
 
 PyDoc_STRVAR(
     Document_dumps_doc,
     "Dumps the document to a string and returns it.\n"
     "\n"
     "By default, serializes to a minified string and strictly follows the\n"
@@ -484,343 +497,371 @@
     "    >>> print(doc.dumps(at_pointer='/results/rows'))\n"
     "    [55,66,77]\n"
     "\n"
     ":param flags: Flags that control JSON writing behaviour.\n"
     ":type flags: :class:`yyjson.WriterFlags`, optional\n"
     ":param at_pointer: An optional JSON pointer specifying what part of the\n"
     "                   document should be dumped. If not specified, defaults\n"
-    "                   to the entire Document.\n"
+    "                   to the entire ``Document``.\n"
     ":type at_pointer: str, optional\n"
     ":returns: The serialized ``Document``.\n"
-    ":rtype: ``str``"
-);
-static PyObject *
-Document_dumps(DocumentObject *self, PyObject *args, PyObject *kwds)
-{
-    static char *kwlist[] = {
-        "flags",
-        "at_pointer",
-        NULL
-    };
-    yyjson_write_flag w_flag = 0;
-    const char *pointer = NULL;
-    Py_ssize_t pointer_size;
-
-    if(!PyArg_ParseTupleAndKeywords(
-            args,
-            kwds,
-            "|$Is#",
-            kwlist,
-            &w_flag,
-            &pointer,
-            &pointer_size
-        )) {
-        return NULL;
-    }
+    ":rtype: ``str``");
+static PyObject* Document_dumps(DocumentObject* self, PyObject* args,
+                                PyObject* kwds) {
+  static char* kwlist[] = {"flags", "at_pointer", NULL};
+  yyjson_write_flag w_flag = 0;
+  const char* pointer = NULL;
+  Py_ssize_t pointer_size;
 
-    char *result = NULL;
-    size_t w_len;
-    yyjson_write_err w_err;
-    PyObject *obj_result = NULL;
-
-    if (self->i_doc != NULL) {
-        yyjson_val *val_to_serialize = NULL;
-
-        if (pointer) {
-            val_to_serialize = yyjson_doc_get_pointern(
-                self->i_doc,
-                pointer,
-                pointer_size
-            );
-        } else {
-            val_to_serialize = yyjson_doc_get_root(self->i_doc);
-        }
+  if (!PyArg_ParseTupleAndKeywords(args, kwds, "|$Is#", kwlist, &w_flag,
+                                   &pointer, &pointer_size)) {
+    return NULL;
+  }
 
-        result = yyjson_val_write_opts(
-            val_to_serialize,
-            w_flag,
-            self->alc,
-            &w_len,
-            &w_err
-        );
+  char* result = NULL;
+  size_t w_len;
+  yyjson_write_err w_err;
+  PyObject* obj_result = NULL;
+
+  if (self->i_doc) {
+    yyjson_val* val_to_serialize = NULL;
+
+    if (pointer) {
+      val_to_serialize =
+          yyjson_doc_ptr_getn(self->i_doc, pointer, pointer_size);
     } else {
-        yyjson_mut_val *mut_val_to_serialize = NULL;
+      val_to_serialize = yyjson_doc_get_root(self->i_doc);
+    }
 
-        if (pointer) {
-            mut_val_to_serialize = yyjson_mut_doc_get_pointern(
-                self->m_doc,
-                pointer,
-                pointer_size
-            );
-        } else {
-            mut_val_to_serialize = yyjson_mut_doc_get_root(self->m_doc);
-        }
+    result = yyjson_val_write_opts(val_to_serialize, w_flag, self->alc, &w_len,
+                                   &w_err);
+  } else {
+    yyjson_mut_val* mut_val_to_serialize = NULL;
 
-        result = yyjson_mut_val_write_opts(
-            mut_val_to_serialize,
-            w_flag,
-            self->alc,
-            &w_len,
-            &w_err
-        );
+    if (pointer) {
+      mut_val_to_serialize =
+          yyjson_mut_doc_ptr_getn(self->m_doc, pointer, pointer_size);
+    } else {
+      mut_val_to_serialize = yyjson_mut_doc_get_root(self->m_doc);
     }
 
-    if (yyjson_unlikely(!result)) {
-        PyErr_SetString(PyExc_ValueError, w_err.msg);
-        return NULL;
-    }
+    result = yyjson_mut_val_write_opts(mut_val_to_serialize, w_flag, self->alc,
+                                       &w_len, &w_err);
+  }
+
+  if (yyjson_unlikely(!result)) {
+    PyErr_SetString(PyExc_ValueError, w_err.msg);
+    return NULL;
+  }
 
-    obj_result = PyUnicode_FromStringAndSize(result, w_len);
-    self->alc->free(NULL, result);
+  obj_result = PyUnicode_FromStringAndSize(result, w_len);
+  self->alc->free(NULL, result);
 
-    return obj_result;
+  return obj_result;
 }
 
-PyDoc_STRVAR(
-    Document_get_pointer_doc,
-    "Returns the JSON element at the given JSON pointer (RFC 6901).\n"
-    "\n"
-    ":param pointer: JSON Pointer to search for.\n"
-    ":type pointer: str"
-);
-static PyObject *
-Document_get_pointer(DocumentObject *self, PyObject *args)
-{
-    char *pointer = NULL;
-    Py_ssize_t pointer_len;
-
-    if (!PyArg_ParseTuple(
-            args,
-            "s#",
-            &pointer,
-            &pointer_len
-        )) {
-        return NULL;
-    }
+PyDoc_STRVAR(Document_get_pointer_doc,
+             "Returns the JSON element at the given JSON pointer (RFC 6901).\n"
+             "\n"
+             ":param pointer: JSON Pointer to search for.\n"
+             ":type pointer: ``str``");
+static PyObject* Document_get_pointer(DocumentObject* self, PyObject* args) {
+  char* pointer = NULL;
+  Py_ssize_t pointer_len;
 
-    if (self->i_doc) {
-        yyjson_val *result = yyjson_doc_get_pointer(
-            self->i_doc,
-            pointer
-        );
-
-        if (!result) {
-            PyErr_SetString(PyExc_ValueError, "Not a valid JSON Pointer");
-            return NULL;
-        }
+  if (!PyArg_ParseTuple(args, "s#", &pointer, &pointer_len)) {
+    return NULL;
+  }
 
-        return element_to_primitive(result);
-    } else {
-        yyjson_mut_val *result = yyjson_mut_doc_get_pointer(
-            self->m_doc,
-            pointer
-        );
-
-        if (!result) {
-            PyErr_SetString(PyExc_ValueError, "Not a valid JSON Pointer");
-            return NULL;
-        }
+  yyjson_ptr_err err;
+
+  if (self->i_doc) {
+    yyjson_val* result =
+        yyjson_doc_ptr_getx(self->i_doc, pointer, pointer_len, &err);
+
+    if (!result) {
+      PyErr_SetString(PyExc_ValueError,
+                      err.msg ? err.msg : "Not a valid JSON Pointer");
+      return NULL;
+    }
+
+    return element_to_primitive(result);
+  } else {
+    yyjson_mut_val* result =
+        yyjson_mut_doc_ptr_getx(self->m_doc, pointer, pointer_len, NULL, &err);
 
-        return mut_element_to_primitive(result);
+    if (!result) {
+      PyErr_SetString(PyExc_ValueError,
+                      err.msg ? err.msg : "Not a valid JSON Pointer");
+      return NULL;
     }
+
+    return mut_element_to_primitive(result);
+  }
 }
 
 PyDoc_STRVAR(
-    Document_merge_patch_doc,
-    "Performs an RFC 7386 JSON merge-patch and returns the result as a\n"
-    "new Document.\n"
+    Document_freeze_doc,
+    "Freezes the document, copying it into yyjson's read-only internal object.\n"
     "\n"
-    "If you intend to re-use the same patch many times, you should pre-create\n"
-    "a :class:`Document` containing the patch, ex:\n"
+    "This object can be used as a normal ``Document`` object, but uses less\n"
+    "memory after creation, and offers slightly improved performance.\n"
     "\n"
-    ".. doctest::\n"
+    ".. note::\n"
     "\n"
-    "    >>> patch = Document({'planets': {'pluto': False}})\n"
-    "    >>> doc = Document({'planets': {'mars': True, 'pluto': True}})\n"
-    "    >>> new_doc = doc.merge_patch(patch)\n"
-    "    >>> print(new_doc.dumps())\n"
-    "    {\"planets\":{\"mars\":true,\"pluto\":false}}\n"
+    "    If a ``Document`` method that requires mutation is called on a frozen\n"
+    "    ``Document``, such as :func:`patch()`, it will be automatically thawed.\n"
+    "    This is an advanced function and can usually be ignored.\n");
+static PyObject* Document_freeze(DocumentObject* self) {
+  if (self->m_doc) {
+    self->i_doc = yyjson_mut_doc_imut_copy(self->m_doc, self->alc);
+    yyjson_mut_doc_free(self->m_doc);
+    self->m_doc = NULL;
+  }
+
+  Py_RETURN_NONE;
+}
+
+PyDoc_STRVAR(
+    Document_thaw_doc,
+    "Thaws the document, copying it into yyjson's mutable internal object.\n"
     "\n"
-    ":param patch: The JSON patch to apply.\n"
-    ":type patch: Document, dict(), or a string containing a JSON document.\n"
-    ":param at_pointer: An optional JSON pointer specifying what part of the\n"
-    "                   document should be patched. If not specified, defaults\n"
-    "                   to the entire Document.\n"
-    ":type at_pointer: str, optional"
-);
-static PyObject *
-Document_merge_patch(DocumentObject *self, PyObject *args, PyObject *kwds)
-{
-    // Create a new, essentially empty Document which will serve as the
-    // container for the patch result.
-    DocumentObject *obj = (DocumentObject*)PyObject_CallFunction(
-        (PyObject*)&DocumentType,
-        "(O)",
-        Py_None
-    );
-    Py_INCREF(Py_None);
+    "This object can be used as a normal ``Document`` object, but will use\n"
+    "slightly more memory after creation, and offers slightly worse\n"
+    "performance.\n"
+    "\n"
+    ".. note::\n"
+    "\n"
+    "    This is an advanced function and can usually be ignored.\n");
+static PyObject* Document_thaw(DocumentObject* self) {
+  if (self->i_doc) {
+    self->m_doc = yyjson_doc_mut_copy(self->i_doc, self->alc);
+    yyjson_doc_free(self->i_doc);
+    self->i_doc = NULL;
+  }
+
+  Py_RETURN_NONE;
+}
+
+PyDoc_STRVAR(
+    Document_patch_doc,
+    "Patch a ``Document`` with another ``Document``, using either JSON Patch (RFC 6902)\n"
+    "or JSON Merge-Patch (RFC 7386).\n"
+    "\n"
+    "By default, this will apply a JSON Patch. Specify ``use_merge_patch=True`` to\n"
+    "use JSON Merge-Patch instead.\n"
+    "\n"
+    ".. note::\n"
+    "\n"
+    "    This method will automatically thaw a frozen ``Document``.\n"
+    "\n"
+    ":param patch: The ``Document`` to patch with.\n"
+    ":type patch: ``Document``\n"
+    ":param at_pointer: The (optional) JSON Pointer (RFC 6901) to patch at,\n"
+    "                   instead of patching the entire document.\n"
+    ":type at_pointer: ``str``\n"
+    ":param use_merge_patch: Whether to use JSON Merge-Patch (RFC 7386) instead of\n"
+    "    JSON Patch (RFC 6902).\n"
+    "\n");
+static PyObject* Document_patch(DocumentObject* self, PyObject* args,
+                                PyObject* kwds) {
+  // Create a new, essentially empty Document which will serve as the
+  // container for the patch result.
+  DocumentObject* obj = (DocumentObject*)PyObject_CallFunction(
+      (PyObject*)&DocumentType, "(O)", Py_None);
+  Py_INCREF(Py_None);
 
-    if (!obj) {
+  if (!obj) {
+    PyErr_SetString(
+        PyExc_ValueError,
+        "Unable to create container Document for results of merge-patch");
+    return NULL;
+  }
+
+  static char* kwlist[] = {"patch", "at_pointer", "use_merge_patch", NULL};
+
+  const char* pointer = NULL;
+  Py_ssize_t pointer_size;
+  PyObject* patch = NULL;
+  int use_merge_patch = false;
+
+  if (!PyArg_ParseTupleAndKeywords(
+          args, kwds,
+          /* We can switch the "i" for "p" to be explicit with our bool
+           * flag, but only after we drop support for everything < 3.3. */
+          "O|$z#i", kwlist, &patch, &pointer, &pointer_size,
+          &use_merge_patch)) {
+    return NULL;
+  }
+
+  // If a pointer was provided, that's the value we're going to be patching,
+  // otherwise we use the root of the document.
+  if (self->i_doc) {
+    yyjson_val* original = NULL;
+
+    if (pointer != NULL) {
+      yyjson_ptr_err ptr_err;
+
+      original =
+          yyjson_doc_ptr_getx(self->i_doc, pointer, pointer_size, &ptr_err);
+      if (!original) {
+        PyErr_SetString(PyExc_ValueError,
+                        ptr_err.msg ? ptr_err.msg : "Not a valid JSON Pointer");
         return NULL;
+      }
+    } else {
+      original = yyjson_doc_get_root(self->i_doc);
+      if (yyjson_unlikely(!original)) {
+        PyErr_SetString(PyExc_ValueError, "Document has no root.");
+        return NULL;
+      }
     }
 
-    static char *kwlist[] = {
-        "patch",
-        "at_pointer",
-        NULL
-    };
-
-    const char *pointer = NULL;
-    Py_ssize_t pointer_size;
-    yyjson_mut_val *original = NULL;
-    PyObject *patch = NULL;
-
-    if(!PyArg_ParseTupleAndKeywords(
-            args,
-            kwds,
-            "O|$s#",
-            kwlist,
-            &patch,
-            &pointer,
-            &pointer_size
-        )) {
-        return NULL;
+    if (!PyObject_IsInstance(patch, (PyObject*)&DocumentType)) {
+      PyErr_SetString(PyExc_TypeError, "Patch must be a Document.");
+      return NULL;
     }
 
-    ENSURE_MUTABLE(self);
+    DocumentObject* patch_doc = (DocumentObject*)patch;
 
-    // If a pointer was provided, that's the value we're going to be patching,
-    // otherwise we use the root of the document.
-    if (pointer != NULL) {
-        original = yyjson_mut_doc_get_pointern(
-            self->m_doc,
-            pointer,
-            pointer_size
-        );
-        if (!original) {
-            PyErr_SetString(PyExc_ValueError, "Not a valid JSON Pointer");
-            return NULL;
-        }
-    } else {
-        original = yyjson_mut_doc_get_root(self->m_doc);
-        if (yyjson_unlikely(!original)) {
-            PyErr_SetString(PyExc_ValueError, "Document has no root.");
-            return NULL;
-        }
+    // If the patch is a mutable document, we need to freeze it before we can
+    // use it with with the immutable merge_patch API.
+    if (patch_doc->m_doc) {
+      patch_doc->i_doc =
+          yyjson_mut_doc_imut_copy(patch_doc->m_doc, patch_doc->alc);
+      yyjson_mut_doc_free(patch_doc->m_doc);
+      patch_doc->m_doc = NULL;
     }
 
-    yyjson_mut_val *patch_val = NULL;
+    yyjson_val* patch_val = yyjson_doc_get_root(patch_doc->i_doc);
+    if (!patch_val) {
+      PyErr_SetString(PyExc_ValueError, "Patch document has no root value.");
+      return NULL;
+    }
+
+    yyjson_mut_val* patched_val = NULL;
 
-    if (PyObject_IsInstance(patch, (PyObject*)&DocumentType)) {
-        // If we were given an existing document, we'll just take the root
-        // and use it as our patch.
-        patch_val = yyjson_mut_doc_get_root(((DocumentObject*)patch)->m_doc);
+    if (use_merge_patch) {
+      patched_val = yyjson_merge_patch(obj->m_doc, original, patch_val);
     } else {
-        // Otherwise, see if what we were given is a valid JSON document, and
-        // use it if so.
-        DocumentObject *patch_doc = (DocumentObject*)PyObject_CallFunction(
-            (PyObject*)&DocumentType,
-            "(O)",
-            patch
-        );
-        if (!patch_doc) return NULL;
-        ENSURE_MUTABLE(patch_doc);
-        patch_val = yyjson_mut_doc_get_root(patch_doc->m_doc);
-    }
-
-    yyjson_mut_val *merged = yyjson_mut_merge_patch(
-        obj->m_doc,
-        original,
-        patch_val
-    );
+      yyjson_patch_err patch_err;
+
+      patched_val = yyjson_patch(obj->m_doc, original, patch_val, &patch_err);
 
-    yyjson_mut_doc_set_root(obj->m_doc, merged);
+      if (!patched_val) {
+        PyErr_SetString(PyExc_ValueError,
+                        patch_err.msg ? patch_err.msg
+                                      : "Unable to apply patch to document.");
+        return NULL;
+      }
+    }
 
+    if (!patched_val) {
+      PyErr_SetString(PyExc_ValueError, "Unable to apply patch to document.");
+      return NULL;
+    }
+
+    yyjson_mut_doc_set_root(obj->m_doc, patched_val);
     return (PyObject*)obj;
-}
+  } else {
+    yyjson_mut_val* original = NULL;
 
-static Py_ssize_t
-Document_length(DocumentObject *self)
-{
-    if (self->i_doc != NULL) {
-        yyjson_val *root = yyjson_doc_get_root(self->i_doc);
-        if (yyjson_unlikely(!root)) {
-            return 0;
-        }
+    if (pointer != NULL) {
+      yyjson_ptr_err ptr_err;
 
-        yyjson_type type = yyjson_get_type(root);
-        if (type == YYJSON_TYPE_OBJ) {
-            return yyjson_obj_size(root);
-        } else if (type == YYJSON_TYPE_ARR) {
-            return yyjson_arr_size(root);
-        }
+      original = yyjson_mut_doc_ptr_getx(self->m_doc, pointer, pointer_size,
+                                         NULL, &ptr_err);
+      if (!original) {
+        PyErr_SetString(PyExc_ValueError,
+                        ptr_err.msg ? ptr_err.msg : "Not a valid JSON Pointer");
+        return NULL;
+      }
     } else {
-        yyjson_mut_val *root = yyjson_mut_doc_get_root(self->m_doc);
-        if (yyjson_unlikely(!root)) {
-            return 0;
-        }
+      original = yyjson_mut_doc_get_root(self->m_doc);
+      if (yyjson_unlikely(!original)) {
+        PyErr_SetString(PyExc_ValueError, "Document has no root.");
+        return NULL;
+      }
+    }
 
-        yyjson_type type = yyjson_mut_get_type(root);
-        if (type == YYJSON_TYPE_OBJ) {
-            return yyjson_mut_obj_size(root);
-        } else if (type == YYJSON_TYPE_ARR) {
-            return yyjson_mut_arr_size(root);
-        }
+    DocumentObject* patch_doc = (DocumentObject*)patch;
+    ENSURE_MUTABLE(patch_doc);
+
+    yyjson_mut_val* patch_val = yyjson_mut_doc_get_root(patch_doc->m_doc);
+    if (!patch_val) {
+      PyErr_SetString(PyExc_ValueError, "Patch document has no root value.");
+      return NULL;
     }
 
-    PyErr_SetString(
-        PyExc_TypeError,
-        "Can't get the length of element that isn't an object or array."
-    );
-    return -1;
+    yyjson_mut_val* patched_val;
+
+    if (use_merge_patch) {
+      patched_val = yyjson_mut_merge_patch(obj->m_doc, original, patch_val);
+    } else {
+      yyjson_patch_err patch_err;
+
+      patched_val =
+          yyjson_mut_patch(obj->m_doc, original, patch_val, &patch_err);
+
+      if (!patched_val) {
+        PyErr_SetString(PyExc_ValueError,
+                        patch_err.msg ? patch_err.msg
+                                      : "Unable to apply patch to document.");
+        return NULL;
+      }
+    }
+
+    if (!patched_val) {
+      PyErr_SetString(PyExc_ValueError, "Unable to apply patch to document.");
+      return NULL;
+    }
+
+    yyjson_mut_doc_set_root(obj->m_doc, patched_val);
+    return (PyObject*)obj;
+  }
+}
+
+static Py_ssize_t Document_length(DocumentObject* self) {
+  if (self->i_doc) {
+    return yyjson_get_len(yyjson_doc_get_root(self->i_doc));
+  } else {
+    return yyjson_mut_get_len(yyjson_mut_doc_get_root(self->m_doc));
+  }
 }
 
 static PyMethodDef Document_methods[] = {
-    {"dumps",
-        (PyCFunction)(void(*)(void))Document_dumps,
-        METH_VARARGS | METH_KEYWORDS,
-        Document_dumps_doc
-    },
-    {"at_pointer",
-        (PyCFunction)(void(*)(void))Document_get_pointer,
-        METH_VARARGS,
-        Document_get_pointer_doc
-    },
-    {"merge_patch",
-        (PyCFunction)(void(*)(void))Document_merge_patch,
-        METH_VARARGS | METH_KEYWORDS,
-        Document_merge_patch_doc
-    },
+    {"patch", (PyCFunction)(void (*)(void))Document_patch,
+     METH_VARARGS | METH_KEYWORDS, Document_patch_doc},
+    {"dumps", (PyCFunction)(void (*)(void))Document_dumps,
+     METH_VARARGS | METH_KEYWORDS, Document_dumps_doc},
+    {"get_pointer", (PyCFunction)(void (*)(void))Document_get_pointer,
+     METH_VARARGS, Document_get_pointer_doc},
+    {"freeze", (PyCFunction)(void (*)(void))Document_freeze, METH_NOARGS,
+     Document_freeze_doc},
+    {"thaw", (PyCFunction)(void (*)(void))Document_thaw, METH_NOARGS,
+     Document_thaw_doc},
     {NULL} /* Sentinel */
 };
 
 static PyGetSetDef Document_members[] = {
-    {"as_obj",
-        (getter)Document_as_obj,
-        NULL,
-        "Converts the Document to a native Python object.",
-        NULL
-    },
+    {"as_obj", (getter)Document_as_obj, NULL,
+     "Converts the Document to a native Python object, such as a ``dict`` or ``list``.", NULL},
+    {"is_thawed", (getter)Document_is_thawed, NULL,
+     "Returns whether the Document is thawed/mutable.", NULL},
     {NULL} /* Sentinel */
 };
 
-
-static PyMappingMethods Document_mapping_methods = {
-    (lenfunc)Document_length,
-    NULL,
-    NULL
-};
+static PyMappingMethods Document_mapping_methods = {(lenfunc)Document_length,
+                                                    NULL, NULL};
 
 PyTypeObject DocumentType = {
-    PyVarObject_HEAD_INIT(NULL, 0)
-    .tp_name = "cyyjson.Document",
+    PyVarObject_HEAD_INIT(NULL, 0).tp_name = "cyyjson.Document",
     .tp_doc = Document_init_doc,
     .tp_basicsize = sizeof(DocumentObject),
     .tp_itemsize = 0,
     .tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_BASETYPE,
     .tp_new = Document_new,
-    .tp_init = (initproc) Document_init,
-    .tp_dealloc = (destructor) Document_dealloc,
+    .tp_init = (initproc)Document_init,
+    .tp_dealloc = (destructor)Document_dealloc,
     .tp_getset = Document_members,
     .tp_as_mapping = &Document_mapping_methods,
-    .tp_methods = Document_methods
-};
+    .tp_methods = Document_methods};
```

### Comparing `yyjson-1.0.1/yyjson/yyjson.c` & `yyjson-2.0.2/yyjson/yyjson.c`

 * *Files 12% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 
 
 /*==============================================================================
  * Version
  *============================================================================*/
 
-yyjson_api uint32_t yyjson_version(void) {
+uint32_t yyjson_version(void) {
     return YYJSON_VERSION_HEX;
 }
 
 
 
 /*==============================================================================
  * Flags
@@ -187,55 +187,18 @@
     defined(__I86__) || defined(__IA32__) || defined(__THW_INTEL)
 #   if (defined(_MSC_VER) && defined(_M_IX86_FP) && _M_IX86_FP == 2) || \
         (defined(__SSE2_MATH__) && __SSE2_MATH__)
 #       define YYJSON_DOUBLE_MATH_CORRECT 1
 #   else
 #       define YYJSON_DOUBLE_MATH_CORRECT 0
 #   endif
-#elif defined(__x86_64) || defined(__x86_64__) || \
-    defined(__amd64) || defined(__amd64__) || \
-    defined(_M_AMD64) || defined(_M_X64) || \
-    defined(__ia64) || defined(_IA64) || defined(__IA64__) ||  \
-    defined(__ia64__) || defined(_M_IA64) || defined(__itanium__) || \
-    defined(__arm64) || defined(__arm64__) || \
-    defined(__aarch64__) || defined(_M_ARM64) || \
-    defined(__arm) || defined(__arm__) || defined(_ARM_) || \
-    defined(_ARM) || defined(_M_ARM) || defined(__TARGET_ARCH_ARM) || \
-    defined(mips) || defined(__mips) || defined(__mips__) || \
-    defined(MIPS) || defined(_MIPS_) || defined(__MIPS__) || \
-    defined(_ARCH_PPC64) || defined(__PPC64__) || \
-    defined(__ppc64__) || defined(__powerpc64__) || \
-    defined(__powerpc) || defined(__powerpc__) || defined(__POWERPC__) || \
-    defined(__ppc__) || defined(__ppc) || defined(__PPC__) || \
-    defined(__sparcv9) || defined(__sparc_v9__) || \
-    defined(__sparc) || defined(__sparc__) || defined(__sparc64__) || \
-    defined(__alpha) || defined(__alpha__) || defined(_M_ALPHA) || \
-    defined(__or1k__) || defined(__OR1K__) || defined(OR1K) || \
-    defined(__hppa) || defined(__hppa__) || defined(__HPPA__) || \
-    defined(__riscv) || defined(__riscv__) || \
-    defined(__s390__) || defined(__avr32__) || defined(__SH4__) || \
-    defined(__e2k__) || defined(__arc__) || defined(__ARC64__) || \
-    defined(__loongarch__) || defined(__nios2__) || defined(__ghs) || \
-    defined(__microblaze__) || defined(__XTENSA__) || \
-    defined(__EMSCRIPTEN__) || defined(__wasm__)
-#   define YYJSON_DOUBLE_MATH_CORRECT 1
+#elif defined(__mc68000__) || defined(__pnacl__) || defined(__native_client__)
+#   define YYJSON_DOUBLE_MATH_CORRECT 0
 #else
-#   define YYJSON_DOUBLE_MATH_CORRECT 0 /* unknown, disable fast path */
-#endif
-
-/*
- Microsoft Visual C++ 6.0 doesn't support converting number from u64 to f64:
- error C2520: conversion from unsigned __int64 to double not implemented.
- */
-#ifndef YYJSON_U64_TO_F64_NO_IMPL
-#   if (0 < YYJSON_MSC_VER) && (YYJSON_MSC_VER <= 1200)
-#       define YYJSON_U64_TO_F64_NO_IMPL 1
-#   else
-#       define YYJSON_U64_TO_F64_NO_IMPL 0
-#   endif
+#   define YYJSON_DOUBLE_MATH_CORRECT 1
 #endif
 
 /* endian */
 #if yyjson_has_include(<sys/types.h>)
 #    include <sys/types.h>
 #endif
 
@@ -280,15 +243,16 @@
     defined(_M_AMD64) || defined(_M_X64) || \
     defined(__ia64) || defined(_IA64) || defined(__IA64__) ||  \
     defined(__ia64__) || defined(_M_IA64) || defined(__itanium__) || \
     defined(__ARMEL__) || defined(__THUMBEL__) || defined(__AARCH64EL__) || \
     defined(__alpha) || defined(__alpha__) || defined(_M_ALPHA) || \
     defined(__riscv) || defined(__riscv__) || \
     defined(_MIPSEL) || defined(__MIPSEL) || defined(__MIPSEL__) || \
-    defined(__EMSCRIPTEN__) || defined(__wasm__)
+    defined(__EMSCRIPTEN__) || defined(__wasm__) || \
+    defined(__loongarch__)
 #   define YYJSON_ENDIAN YYJSON_LITTLE_ENDIAN
 
 #elif (defined(__BIG_ENDIAN__) && __BIG_ENDIAN__ == 1) || \
     defined(__ARMEB__) || defined(__THUMBEB__) || defined(__AARCH64EB__) || \
     defined(_MIPSEB) || defined(__MIPSEB) || defined(__MIPSEB__) || \
     defined(_ARCH_PPC) || defined(_ARCH_PPC64) || \
     defined(__ppc) || defined(__ppc__) || \
@@ -299,15 +263,15 @@
 #else
 #   define YYJSON_ENDIAN 0 /* unknown endian, detect at run-time */
 #endif
 
 /*
  Unaligned memory access detection.
  
- Some architectures cannot perform unaligned memory accesse, or unaligned memory
+ Some architectures cannot perform unaligned memory access, or unaligned memory
  accesses can have a large performance penalty. Modern compilers can make some
  optimizations for unaligned access. For example: https://godbolt.org/z/Ejo3Pa
  
     typedef struct { char c[2] } vec2;
     void copy_vec2(vec2 *dst, vec2 *src) {
         *dst = *src;
     }
@@ -348,14 +312,17 @@
         defined(__powerpc64__) || defined(_ARCH_PPC64) || \
         defined(__ppc) || defined(__ppc__) || defined(__PPC__) || \
         defined(__powerpc) || defined(__powerpc__) || defined(__POWERPC__) || \
         defined(_ARCH_PPC) || defined(_M_PPC) || \
         defined(__PPCGECKO__) || defined(__PPCBROADWAY__) || defined(_XENON)
 #       define YYJSON_DISABLE_UNALIGNED_MEMORY_ACCESS 0 /* PowerPC */
 
+#   elif defined(__loongarch__)
+#       define YYJSON_DISABLE_UNALIGNED_MEMORY_ACCESS 0 /* loongarch */
+
 #   else
 #       define YYJSON_DISABLE_UNALIGNED_MEMORY_ACCESS 0 /* Unknown */
 #   endif
 
 #endif
 
 /*
@@ -367,29 +334,38 @@
     value_count: 5
     ratio:       6
     
  yyjson uses dynamic memory with a growth factor of 1.5 when reading and writing
  JSON, the ratios below are used to determine the initial memory size.
  
  A too large ratio will waste memory, and a too small ratio will cause multiple
- memory growths and degrade performance. Currently these ratios are generated
+ memory growths and degrade performance. Currently, these ratios are generated
  with some commonly used JSON datasets.
  */
 #define YYJSON_READER_ESTIMATED_PRETTY_RATIO 16
 #define YYJSON_READER_ESTIMATED_MINIFY_RATIO 6
 #define YYJSON_WRITER_ESTIMATED_PRETTY_RATIO 32
 #define YYJSON_WRITER_ESTIMATED_MINIFY_RATIO 18
 
+/* The initial and maximum size of the memory pool's chunk in yyjson_mut_doc. */
+#define YYJSON_MUT_DOC_STR_POOL_INIT_SIZE   0x100
+#define YYJSON_MUT_DOC_STR_POOL_MAX_SIZE    0x10000000
+#define YYJSON_MUT_DOC_VAL_POOL_INIT_SIZE   (0x10 * sizeof(yyjson_mut_val))
+#define YYJSON_MUT_DOC_VAL_POOL_MAX_SIZE    (0x1000000 * sizeof(yyjson_mut_val))
+
 /* Default value for compile-time options. */
 #ifndef YYJSON_DISABLE_READER
 #define YYJSON_DISABLE_READER 0
 #endif
 #ifndef YYJSON_DISABLE_WRITER
 #define YYJSON_DISABLE_WRITER 0
 #endif
+#ifndef YYJSON_DISABLE_UTILS
+#define YYJSON_DISABLE_UTILS 0
+#endif
 #ifndef YYJSON_DISABLE_FAST_FP_CONV
 #define YYJSON_DISABLE_FAST_FP_CONV 0
 #endif
 #ifndef YYJSON_DISABLE_NON_STANDARD
 #define YYJSON_DISABLE_NON_STANDARD 0
 #endif
 
@@ -433,43 +409,54 @@
 #undef  yyjson_max
 #define yyjson_max(x, y) ((x) > (y) ? (x) : (y))
 
 /* Used to write u64 literal for C89 which doesn't support "ULL" suffix. */
 #undef  U64
 #define U64(hi, lo) ((((u64)hi##UL) << 32U) + lo##UL)
 
+/* Used to cast away (remove) const qualifier. */
+#define constcast(type) (type)(void *)(size_t)(const void *)
+
 
 
 /*==============================================================================
  * Integer Constants
  *============================================================================*/
 
 /* U64 constant values */
 #undef  U64_MAX
 #define U64_MAX         U64(0xFFFFFFFF, 0xFFFFFFFF)
 #undef  I64_MAX
 #define I64_MAX         U64(0x7FFFFFFF, 0xFFFFFFFF)
 #undef  USIZE_MAX
 #define USIZE_MAX       ((usize)(~(usize)0))
 
-/* Maximum number of digits for reading u64 safety. */
+/* Maximum number of digits for reading u32/u64/usize safety (not overflow). */
+#undef  U32_SAFE_DIG
+#define U32_SAFE_DIG    9   /* u32 max is 4294967295, 10 digits */
 #undef  U64_SAFE_DIG
-#define U64_SAFE_DIG    19
+#define U64_SAFE_DIG    19  /* u64 max is 18446744073709551615, 20 digits */
+#undef  USIZE_SAFE_DIG
+#define USIZE_SAFE_DIG  (sizeof(usize) == 64 ? U64_SAFE_DIG : U32_SAFE_DIG)
 
 
 
 /*==============================================================================
  * IEEE-754 Double Number Constants
  *============================================================================*/
 
 /* Inf raw value (positive) */
 #define F64_RAW_INF U64(0x7FF00000, 0x00000000)
 
-/* NaN raw value (positive, without payload) */
+/* NaN raw value (quiet NaN, no payload, no sign) */
+#if defined(__hppa__) || (defined(__mips__) && !defined(__mips_nan2008))
+#define F64_RAW_NAN U64(0x7FF7FFFF, 0xFFFFFFFF)
+#else
 #define F64_RAW_NAN U64(0x7FF80000, 0x00000000)
+#endif
 
 /* double number bits */
 #define F64_BITS 64
 
 /* double number exponent part bits */
 #define F64_EXP_BITS 11
 
@@ -547,71 +534,71 @@
  * Load/Store Utils
  *============================================================================*/
 
 #define byte_move_idx(x) ((u8 *)dst)[x] = ((u8 *)src)[x];
 
 static_inline void byte_move_2(void *dst, const void *src) {
 #if YYJSON_DISABLE_UNALIGNED_MEMORY_ACCESS
-    repeat2_incr(byte_move_idx);
+    repeat2_incr(byte_move_idx)
 #else
     memmove(dst, src, 2);
 #endif
 }
 
 static_inline void byte_move_4(void *dst, const void *src) {
 #if YYJSON_DISABLE_UNALIGNED_MEMORY_ACCESS
-    repeat4_incr(byte_move_idx);
+    repeat4_incr(byte_move_idx)
 #else
     memmove(dst, src, 4);
 #endif
 }
 
 static_inline void byte_move_8(void *dst, const void *src) {
 #if YYJSON_DISABLE_UNALIGNED_MEMORY_ACCESS
-    repeat8_incr(byte_move_idx);
+    repeat8_incr(byte_move_idx)
 #else
     memmove(dst, src, 8);
 #endif
 }
 
 static_inline void byte_move_16(void *dst, const void *src) {
 #if YYJSON_DISABLE_UNALIGNED_MEMORY_ACCESS
-    repeat16_incr(byte_move_idx);
+    repeat16_incr(byte_move_idx)
 #else
     memmove(dst, src, 16);
 #endif
 }
 
 static_inline void byte_copy_2(void *dst, const void *src) {
 #if YYJSON_DISABLE_UNALIGNED_MEMORY_ACCESS
-    repeat2_incr(byte_move_idx);
+    repeat2_incr(byte_move_idx)
 #else
     memcpy(dst, src, 2);
 #endif
 }
 
 static_inline void byte_copy_4(void *dst, const void *src) {
 #if YYJSON_DISABLE_UNALIGNED_MEMORY_ACCESS
-    repeat4_incr(byte_move_idx);
+    repeat4_incr(byte_move_idx)
 #else
     memcpy(dst, src, 4);
 #endif
 }
 
 static_inline void byte_copy_8(void *dst, const void *src) {
 #if YYJSON_DISABLE_UNALIGNED_MEMORY_ACCESS
-    repeat8_incr(byte_move_idx);
+    repeat8_incr(byte_move_idx)
 #else
     memcpy(dst, src, 8);
 #endif
 }
 
 static_inline void byte_copy_16(void *dst, const void *src) {
 #if YYJSON_DISABLE_UNALIGNED_MEMORY_ACCESS
-    repeat16_incr(byte_move_idx);
+    repeat16_incr(byte_move_idx)
 #else
     memcpy(dst, src, 16);
 #endif
 }
 
 static_inline bool byte_match_2(void *buf, const char *pat) {
 #if YYJSON_DISABLE_UNALIGNED_MEMORY_ACCESS
@@ -639,29 +626,29 @@
     u2.v = *(const v32 *)buf;
     return u1.u == u2.u;
 #endif
 }
 
 static_inline u16 byte_load_2(const void *src) {
     v16_uni uni;
-    uni.v = *(v16 *)src;
+    uni.v = *(const v16 *)src;
     return uni.u;
 }
 
 static_inline u32 byte_load_3(const void *src) {
     v32_uni uni;
-    ((v16_uni *)&uni)->v = *(v16 *)src;
-    uni.v.c3 = ((char *)src)[2];
+    ((v16_uni *)&uni)->v = *(const v16 *)src;
+    uni.v.c3 = ((const char *)src)[2];
     uni.v.c4 = 0;
     return uni.u;
 }
 
 static_inline u32 byte_load_4(const void *src) {
     v32_uni uni;
-    uni.v = *(v32 *)src;
+    uni.v = *(const v32 *)src;
     return uni.u;
 }
 
 #undef byte_move_expr
 
 
 
@@ -746,16 +733,15 @@
 /*==============================================================================
  * Size Utils
  * These functions are used for memory allocation.
  *============================================================================*/
 
 /** Returns whether the size is overflow after increment. */
 static_inline bool size_add_is_overflow(usize size, usize add) {
-    usize val = size + add;
-    return (val < size) | (val < add);
+    return size > (size + add);
 }
 
 /** Returns whether the size is power of 2 (size should not be 0). */
 static_inline bool size_is_pow2(usize size) {
     return (size & (size - 1)) == 0;
 }
 
@@ -782,23 +768,14 @@
     usize size;
     memcpy(&size, &mem, sizeof(usize));
     size = size_align_up(size, align);
     memcpy(&mem, &size, sizeof(usize));
     return mem;
 }
 
-/** Align address downwards. */
-static_inline void *mem_align_down(void *mem, usize align) {
-    usize size;
-    memcpy(&size, &mem, sizeof(usize));
-    size = size_align_down(size, align);
-    memcpy(&mem, &size, sizeof(usize));
-    return mem;
-}
-
 
 
 /*==============================================================================
  * Bits Utils
  * These functions are used by the floating-point number reader and writer.
  *============================================================================*/
 
@@ -903,15 +880,15 @@
     u128 m = (u128)a * b + c;
     *hi = (u64)(m >> 64);
     *lo = (u64)(m);
 #else
     u64 h, l, t;
     u128_mul(a, b, &h, &l);
     t = l + c;
-    h += ((t < l) | (t < c));
+    h += (u64)(((t < l) | (t < c)));
     *hi = h;
     *lo = t;
 #endif
 }
 
 
 
@@ -961,29 +938,48 @@
  * This is a simple libc memory allocator wrapper.
  *============================================================================*/
 
 static void *default_malloc(void *ctx, usize size) {
     return malloc(size);
 }
 
-static void *default_realloc(void *ctx, void *ptr, usize size) {
+static void *default_realloc(void *ctx, void *ptr, usize old_size, usize size) {
     return realloc(ptr, size);
 }
 
 static void default_free(void *ctx, void *ptr) {
     free(ptr);
 }
 
 static const yyjson_alc YYJSON_DEFAULT_ALC = {
     default_malloc,
     default_realloc,
     default_free,
     NULL
 };
 
+static void *null_malloc(void *ctx, usize size) {
+    return NULL;
+}
+
+static void *null_realloc(void *ctx, void *ptr, usize old_size, usize size) {
+    return NULL;
+}
+
+static void null_free(void *ctx, void *ptr) {
+    return;
+}
+
+static const yyjson_alc YYJSON_NULL_ALC = {
+    null_malloc,
+    null_realloc,
+    null_free,
+    NULL
+};
+
 
 
 /*==============================================================================
  * Pool Memory Allocator
  * This is a simple memory allocator that uses linked list memory chunk.
  * The following code will be executed only when the library user creates
  * this allocator manually.
@@ -1053,15 +1049,16 @@
     if (prev && ((u8 *)prev + prev->size) == (u8 *)cur) {
         /* merge cur to lower chunk */
         prev->size += cur->size;
         prev->next = cur->next;
     }
 }
 
-static void *pool_realloc(void *ctx_ptr, void *ptr, usize size) {
+static void *pool_realloc(void *ctx_ptr, void *ptr,
+                          usize old_size, usize size) {
     pool_ctx *ctx = (pool_ctx *)ctx_ptr;
     pool_chunk *cur = ((pool_chunk *)ptr) - 1, *prev, *next, *tmp;
     usize free_size;
     void *new_ptr;
     
     if (unlikely(size == 0 || size >= ctx->size)) return NULL;
     size = size_align_up(size, sizeof(pool_chunk)) + sizeof(pool_chunk);
@@ -1114,15 +1111,17 @@
     return new_ptr;
 }
 
 bool yyjson_alc_pool_init(yyjson_alc *alc, void *buf, usize size) {
     pool_chunk *chunk;
     pool_ctx *ctx;
     
-    if (unlikely(!alc || size < sizeof(pool_ctx) * 4)) return false;
+    if (unlikely(!alc)) return false;
+    *alc = YYJSON_NULL_ALC;
+    if (size < sizeof(pool_ctx) * 4) return false;
     ctx = (pool_ctx *)mem_align_up(buf, sizeof(pool_ctx));
     if (unlikely(!ctx)) return false;
     size -= (usize)((u8 *)ctx - (u8 *)buf);
     size = size_align_down(size, sizeof(pool_ctx));
     
     chunk = (pool_chunk *)(ctx + 1);
     chunk->size = size - sizeof(pool_ctx);
@@ -1160,53 +1159,81 @@
         next = chunk->next;
         alc->free(alc->ctx, chunk);
         chunk = next;
     }
 }
 
 bool unsafe_yyjson_str_pool_grow(yyjson_str_pool *pool,
-                                 yyjson_alc *alc, usize len) {
+                                 const yyjson_alc *alc, usize len) {
     yyjson_str_chunk *chunk;
-    usize size = len + sizeof(yyjson_str_chunk);
+    usize size, max_len;
+    
+    /* create a new chunk */
+    max_len = USIZE_MAX - sizeof(yyjson_str_chunk);
+    if (unlikely(len > max_len)) return false;
+    size = len + sizeof(yyjson_str_chunk);
     size = yyjson_max(pool->chunk_size, size);
     chunk = (yyjson_str_chunk *)alc->malloc(alc->ctx, size);
-    if (yyjson_unlikely(!chunk)) return false;
+    if (unlikely(!chunk)) return false;
     
+    /* insert the new chunk as the head of the linked list */
     chunk->next = pool->chunks;
+    chunk->chunk_size = size;
     pool->chunks = chunk;
     pool->cur = (char *)chunk + sizeof(yyjson_str_chunk);
     pool->end = (char *)chunk + size;
     
+    /* the next chunk is twice the size of the current one */
     size = yyjson_min(pool->chunk_size * 2, pool->chunk_size_max);
+    if (size < pool->chunk_size) size = pool->chunk_size_max; /* overflow */
     pool->chunk_size = size;
     return true;
 }
 
 bool unsafe_yyjson_val_pool_grow(yyjson_val_pool *pool,
-                                 yyjson_alc *alc, usize count) {
+                                 const yyjson_alc *alc, usize count) {
     yyjson_val_chunk *chunk;
-    usize size;
+    usize size, max_count;
     
-    if (count >= USIZE_MAX / sizeof(yyjson_mut_val) - 16) return false;
+    /* create a new chunk */
+    max_count = USIZE_MAX / sizeof(yyjson_mut_val) - 1;
+    if (unlikely(count > max_count)) return false;
     size = (count + 1) * sizeof(yyjson_mut_val);
     size = yyjson_max(pool->chunk_size, size);
     chunk = (yyjson_val_chunk *)alc->malloc(alc->ctx, size);
-    if (yyjson_unlikely(!chunk)) return false;
+    if (unlikely(!chunk)) return false;
     
+    /* insert the new chunk as the head of the linked list */
     chunk->next = pool->chunks;
+    chunk->chunk_size = size;
     pool->chunks = chunk;
-    pool->cur = (yyjson_mut_val *)(void *)((u8 *)chunk
-                                           + sizeof(yyjson_mut_val));
+    pool->cur = (yyjson_mut_val *)(void *)((u8 *)chunk) + 1;
     pool->end = (yyjson_mut_val *)(void *)((u8 *)chunk + size);
     
+    /* the next chunk is twice the size of the current one */
     size = yyjson_min(pool->chunk_size * 2, pool->chunk_size_max);
+    if (size < pool->chunk_size) size = pool->chunk_size_max; /* overflow */
     pool->chunk_size = size;
     return true;
 }
 
+bool yyjson_mut_doc_set_str_pool_size(yyjson_mut_doc *doc, size_t len) {
+    usize max_size = USIZE_MAX - sizeof(yyjson_str_chunk);
+    if (!doc || !len || len > max_size) return false;
+    doc->str_pool.chunk_size = len + sizeof(yyjson_str_chunk);
+    return true;
+}
+
+bool yyjson_mut_doc_set_val_pool_size(yyjson_mut_doc *doc, size_t count) {
+    usize max_count = USIZE_MAX / sizeof(yyjson_mut_val) - 1;
+    if (!doc || !count || count > max_count) return false;
+    doc->val_pool.chunk_size = (count + 1) * sizeof(yyjson_mut_val);
+    return true;
+}
+
 void yyjson_mut_doc_free(yyjson_mut_doc *doc) {
     if (doc) {
         yyjson_alc alc = doc->alc;
         unsafe_yyjson_str_pool_release(&doc->str_pool, &alc);
         unsafe_yyjson_val_pool_release(&doc->val_pool, &alc);
         alc.free(alc.ctx, doc);
     }
@@ -1216,23 +1243,22 @@
     yyjson_mut_doc *doc;
     if (!alc) alc = &YYJSON_DEFAULT_ALC;
     doc = (yyjson_mut_doc *)alc->malloc(alc->ctx, sizeof(yyjson_mut_doc));
     if (!doc) return NULL;
     memset(doc, 0, sizeof(yyjson_mut_doc));
     
     doc->alc = *alc;
-    doc->str_pool.chunk_size = 0x100;
-    doc->str_pool.chunk_size_max = 0x10000000;
-    doc->val_pool.chunk_size = 0x10 * sizeof(yyjson_mut_val);
-    doc->val_pool.chunk_size_max = 0x1000000 * sizeof(yyjson_mut_val);
+    doc->str_pool.chunk_size = YYJSON_MUT_DOC_STR_POOL_INIT_SIZE;
+    doc->str_pool.chunk_size_max = YYJSON_MUT_DOC_STR_POOL_MAX_SIZE;
+    doc->val_pool.chunk_size = YYJSON_MUT_DOC_VAL_POOL_INIT_SIZE;
+    doc->val_pool.chunk_size_max = YYJSON_MUT_DOC_VAL_POOL_MAX_SIZE;
     return doc;
 }
 
-yyjson_api yyjson_mut_doc *yyjson_doc_mut_copy(yyjson_doc *doc,
-                                               const yyjson_alc *alc) {
+yyjson_mut_doc *yyjson_doc_mut_copy(yyjson_doc *doc, const yyjson_alc *alc) {
     yyjson_mut_doc *m_doc;
     yyjson_mut_val *m_val;
     
     if (!doc || !doc->root) return NULL;
     m_doc = yyjson_mut_doc_new(alc);
     if (!m_doc) return NULL;
     m_val = yyjson_val_mut_copy(m_doc, doc->root);
@@ -1240,33 +1266,35 @@
         yyjson_mut_doc_free(m_doc);
         return NULL;
     }
     yyjson_mut_doc_set_root(m_doc, m_val);
     return m_doc;
 }
 
-yyjson_api yyjson_mut_doc *yyjson_mut_doc_mut_copy(yyjson_mut_doc *doc,
-                                                   const yyjson_alc *alc) {
+yyjson_mut_doc *yyjson_mut_doc_mut_copy(yyjson_mut_doc *doc,
+                                        const yyjson_alc *alc) {
     yyjson_mut_doc *m_doc;
     yyjson_mut_val *m_val;
     
-    if (!doc || !doc->root) return NULL;
+    if (!doc) return NULL;
+    if (!doc->root) return yyjson_mut_doc_new(alc);
+    
     m_doc = yyjson_mut_doc_new(alc);
     if (!m_doc) return NULL;
     m_val = yyjson_mut_val_mut_copy(m_doc, doc->root);
     if (!m_val) {
         yyjson_mut_doc_free(m_doc);
         return NULL;
     }
     yyjson_mut_doc_set_root(m_doc, m_val);
     return m_doc;
 }
 
-yyjson_api yyjson_mut_val *yyjson_val_mut_copy(yyjson_mut_doc *m_doc,
-                                               yyjson_val *i_vals) {
+yyjson_mut_val *yyjson_val_mut_copy(yyjson_mut_doc *m_doc,
+                                    yyjson_val *i_vals) {
     /*
      The immutable object or array stores all sub-values in a contiguous memory,
      We copy them to another contiguous memory as mutable values,
      then reconnect the mutable values with the original relationship.
      */
     
     usize i_vals_len;
@@ -1375,20 +1403,133 @@
             m_val->uni = m_vals->uni;
             break;
     }
     
     return m_val;
 }
 
-yyjson_api yyjson_mut_val *yyjson_mut_val_mut_copy(yyjson_mut_doc *doc,
-                                                   yyjson_mut_val *val) {
+yyjson_mut_val *yyjson_mut_val_mut_copy(yyjson_mut_doc *doc,
+                                        yyjson_mut_val *val) {
     if (doc && val) return unsafe_yyjson_mut_val_mut_copy(doc, val);
     return NULL;
 }
 
+/* Count the number of values and the total length of the strings. */
+static void yyjson_mut_stat(yyjson_mut_val *val,
+                            usize *val_sum, usize *str_sum) {
+    yyjson_type type = unsafe_yyjson_get_type(val);
+    *val_sum += 1;
+    if (type == YYJSON_TYPE_ARR || type == YYJSON_TYPE_OBJ) {
+        yyjson_mut_val *child = (yyjson_mut_val *)val->uni.ptr;
+        usize len = unsafe_yyjson_get_len(val), i;
+        len <<= (u8)(type == YYJSON_TYPE_OBJ);
+        *val_sum += len;
+        for (i = 0; i < len; i++) {
+            yyjson_type stype = unsafe_yyjson_get_type(child);
+            if (stype == YYJSON_TYPE_STR || stype == YYJSON_TYPE_RAW) {
+                *str_sum += unsafe_yyjson_get_len(child) + 1;
+            } else if (stype == YYJSON_TYPE_ARR || stype == YYJSON_TYPE_OBJ) {
+                yyjson_mut_stat(child, val_sum, str_sum);
+                *val_sum -= 1;
+            }
+            child = child->next;
+        }
+    } else if (type == YYJSON_TYPE_STR || type == YYJSON_TYPE_RAW) {
+        *str_sum += unsafe_yyjson_get_len(val) + 1;
+    }
+}
+
+/* Copy mutable values to immutable value pool. */
+static usize yyjson_imut_copy(yyjson_val **val_ptr, char **buf_ptr,
+                              yyjson_mut_val *mval) {
+    yyjson_val *val = *val_ptr;
+    yyjson_type type = unsafe_yyjson_get_type(mval);
+    if (type == YYJSON_TYPE_ARR || type == YYJSON_TYPE_OBJ) {
+        yyjson_mut_val *child = (yyjson_mut_val *)mval->uni.ptr;
+        usize len = unsafe_yyjson_get_len(mval), i;
+        usize val_sum = 1;
+        if (type == YYJSON_TYPE_OBJ) {
+            if (len) child = child->next->next;
+            len <<= 1;
+        } else {
+            if (len) child = child->next;
+        }
+        *val_ptr = val + 1;
+        for (i = 0; i < len; i++) {
+            val_sum += yyjson_imut_copy(val_ptr, buf_ptr, child);
+            child = child->next;
+        }
+        val->tag = mval->tag;
+        val->uni.ofs = val_sum * sizeof(yyjson_val);
+        return val_sum;
+    } else if (type == YYJSON_TYPE_STR || type == YYJSON_TYPE_RAW) {
+        char *buf = *buf_ptr;
+        usize len = unsafe_yyjson_get_len(mval);
+        memcpy((void *)buf, (const void *)mval->uni.str, len);
+        buf[len] = '\0';
+        val->tag = mval->tag;
+        val->uni.str = buf;
+        *val_ptr = val + 1;
+        *buf_ptr = buf + len + 1;
+        return 1;
+    } else {
+        val->tag = mval->tag;
+        val->uni = mval->uni;
+        *val_ptr = val + 1;
+        return 1;
+    }
+}
+
+yyjson_doc *yyjson_mut_doc_imut_copy(yyjson_mut_doc *mdoc,
+                                     const yyjson_alc *alc) {
+    if (!mdoc) return NULL;
+    return yyjson_mut_val_imut_copy(mdoc->root, alc);
+}
+
+yyjson_doc *yyjson_mut_val_imut_copy(yyjson_mut_val *mval,
+                                     const yyjson_alc *alc) {
+    usize val_num = 0, str_sum = 0, hdr_size, buf_size;
+    yyjson_doc *doc = NULL;
+    yyjson_val *val_hdr = NULL;
+    
+    /* This value should be NULL here. Setting a non-null value suppresses
+       warning from the clang analyzer. */
+    char *str_hdr = (char *)(void *)&str_sum;
+    if (!mval) return NULL;
+    if (!alc) alc = &YYJSON_DEFAULT_ALC;
+    
+    /* traverse the input value to get pool size */
+    yyjson_mut_stat(mval, &val_num, &str_sum);
+    
+    /* create doc and val pool */
+    hdr_size = size_align_up(sizeof(yyjson_doc), sizeof(yyjson_val));
+    buf_size = hdr_size + val_num * sizeof(yyjson_val);
+    doc = (yyjson_doc *)alc->malloc(alc->ctx, buf_size);
+    if (!doc) return NULL;
+    memset(doc, 0, sizeof(yyjson_doc));
+    val_hdr = (yyjson_val *)(void *)((char *)(void *)doc + hdr_size);
+    doc->root = val_hdr;
+    doc->alc = *alc;
+    
+    /* create str pool */
+    if (str_sum > 0) {
+        str_hdr = (char *)alc->malloc(alc->ctx, str_sum);
+        doc->str_pool = str_hdr;
+        if (!str_hdr) {
+            alc->free(alc->ctx, (void *)doc);
+            return NULL;
+        }
+    }
+    
+    /* copy vals and strs */
+    doc->val_read = yyjson_imut_copy(&val_hdr, &str_hdr, mval);
+    doc->dat_read = str_sum + 1;
+    return doc;
+}
+
 static_inline bool unsafe_yyjson_num_equals(void *lhs, void *rhs) {
     yyjson_val_uni *luni = &((yyjson_val *)lhs)->uni;
     yyjson_val_uni *runi = &((yyjson_val *)rhs)->uni;
     yyjson_subtype lt = unsafe_yyjson_get_subtype(lhs);
     yyjson_subtype rt = unsafe_yyjson_get_subtype(rhs);
     if (lt == rt)
         return luni->u64 == runi->u64;
@@ -1398,20 +1539,19 @@
         return runi->i64 >= 0 && luni->u64 == runi->u64;
     return false;
 }
 
 static_inline bool unsafe_yyjson_str_equals(void *lhs, void *rhs) {
     usize len = unsafe_yyjson_get_len(lhs);
     if (len != unsafe_yyjson_get_len(rhs)) return false;
-    return 0 == len ||
-           0 == memcmp(unsafe_yyjson_get_str(lhs),
-                       unsafe_yyjson_get_str(rhs), len);
+    return !memcmp(unsafe_yyjson_get_str(lhs),
+                   unsafe_yyjson_get_str(rhs), len);
 }
 
-yyjson_api bool unsafe_yyjson_equals(yyjson_val *lhs, yyjson_val *rhs) {
+bool unsafe_yyjson_equals(yyjson_val *lhs, yyjson_val *rhs) {
     yyjson_type type = unsafe_yyjson_get_type(lhs);
     if (type != unsafe_yyjson_get_type(rhs)) return false;
     
     switch (type) {
         case YYJSON_TYPE_OBJ: {
             usize len = unsafe_yyjson_get_len(lhs);
             if (len != unsafe_yyjson_get_len(rhs)) return false;
@@ -1434,16 +1574,15 @@
         case YYJSON_TYPE_ARR: {
             usize len = unsafe_yyjson_get_len(lhs);
             if (len != unsafe_yyjson_get_len(rhs)) return false;
             if (len > 0) {
                 lhs = unsafe_yyjson_get_first(lhs);
                 rhs = unsafe_yyjson_get_first(rhs);
                 while (len-- > 0) {
-                    if (!unsafe_yyjson_equals(lhs, rhs))
-                        return false;
+                    if (!unsafe_yyjson_equals(lhs, rhs)) return false;
                     lhs = unsafe_yyjson_get_next(lhs);
                     rhs = unsafe_yyjson_get_next(rhs);
                 }
             }
             return true;
         }
         
@@ -1490,16 +1629,15 @@
         case YYJSON_TYPE_ARR: {
             usize len = unsafe_yyjson_get_len(lhs);
             if (len != unsafe_yyjson_get_len(rhs)) return false;
             if (len > 0) {
                 lhs = (yyjson_mut_val *)lhs->uni.ptr;
                 rhs = (yyjson_mut_val *)rhs->uni.ptr;
                 while (len-- > 0) {
-                    if (!unsafe_yyjson_mut_equals(lhs, rhs))
-                        return false;
+                    if (!unsafe_yyjson_mut_equals(lhs, rhs)) return false;
                     lhs = lhs->next;
                     rhs = rhs->next;
                 }
             }
             return true;
         }
         
@@ -1517,195 +1655,844 @@
         default:
             return false;
     }
 }
 
 
 
+#if !YYJSON_DISABLE_UTILS
+
 /*==============================================================================
- * JSON Pointer
+ * JSON Pointer API (RFC 6901)
  *============================================================================*/
 
 /**
- Get value from JSON array with a path segment (array index).
- @param ptr Input the segment after `/`, output the end of segment.
- @param end The end of entire JSON pointer.
- @param arr JSON array (yyjson_val/yyjson_mut_val, based on `mut`).
- @param mut Whether `arr` is mutable.
- @return The matched value, or NULL if not matched.
+ Get a token from JSON pointer string.
+ @param ptr [in,out]
+                in:  string that points to current token prefix `/`
+                out: string that points to next token prefix `/`, or string end
+ @param end [in] end of the entire JSON Pointer string
+ @param len [out] unescaped token length
+ @param esc [out] number of escaped characters in this token
+ @return head of the token, or NULL if syntax error
  */
-static_inline void *pointer_read_arr(const char **ptr,
-                                     const char *end,
-                                     void *arr,
-                                     bool mut) {
-    const char *hdr = *ptr;
+static_inline const char *ptr_next_token(const char **ptr, const char *end,
+                                         usize *len, usize *esc) {
+    const char *hdr = *ptr + 1;
     const char *cur = hdr;
-    yyjson_val *i_arr = (yyjson_val *)arr;
-    yyjson_mut_val *m_arr = (yyjson_mut_val *)arr;
-    u64 idx = 0;
-    u8 add;
-    
-    /* start with 0 */
-    if (cur < end && *cur == '0') {
-        *ptr = cur + 1;
-        return mut
-            ? (void *)yyjson_mut_arr_get_first(m_arr)
-            : (void *)yyjson_arr_get_first(i_arr);
-    }
-    
-    /* read whole number */
-    if (cur + U64_SAFE_DIG < end) end = cur + U64_SAFE_DIG;
-    while (cur < end && (add = (u8)((u8)*cur - (u8)'0')) <= 9) {
-        cur++;
-        idx = idx * 10 + add;
+    /* skip unescaped characters */
+    while (cur < end && *cur != '/' && *cur != '~') cur++;
+    if (likely(cur == end || *cur != '~')) {
+        /* no escaped characters, return */
+        *ptr = cur;
+        *len = (usize)(cur - hdr);
+        *esc = 0;
+        return hdr;
+    } else {
+        /* handle escaped characters */
+        usize esc_num = 0;
+        while (cur < end && *cur != '/') {
+            if (*cur++ == '~') {
+                if (cur == end || (*cur != '0' && *cur != '1')) {
+                    *ptr = cur - 1;
+                    return NULL;
+                }
+                esc_num++;
+            }
+        }
+        *ptr = cur;
+        *len = (usize)(cur - hdr) - esc_num;
+        *esc = esc_num;
+        return hdr;
     }
-    if (cur == hdr) return NULL;
-    *ptr = cur;
-    return mut
-        ? (void *)yyjson_mut_arr_get(m_arr, idx)
-        : (void *)yyjson_arr_get(i_arr, idx);
 }
 
 /**
- Get value from JSON object with a path segment (object key).
- @param ptr Input the segment after `/`, output the end of segment.
- @param end The end of entire JSON pointer.
- @param obj JSON object (yyjson_val/yyjson_mut_val, based on `mut`).
- @param mut `obj` is mutable.
- @return The matched value, or NULL if not matched.
+ Convert token string to index.
+ @param cur [in]  token head
+ @param len [in]  token length
+ @param idx [out] the index number, or USIZE_MAX if token is '-'
+ @return true if token is a valid array index
  */
-static_inline void *pointer_read_obj(const char **ptr,
-                                     const char *end,
-                                     void *obj,
-                                     bool mut) {
-#define BUF_SIZE 512
-#define is_escaped(cur) ((cur) < end && (*(cur) == '0' || *(cur) == '1'))
-#define is_unescaped(cur) ((cur) < end && *(cur) != '/' && *(cur) != '~')
-#define is_completed(cur) ((cur) == end || *(cur) == '/')
+static_inline bool ptr_token_to_idx(const char *cur, usize len, usize *idx) {
+    const char *end = cur + len;
+    usize num = 0, add;
+    if (unlikely(len == 0 || len > USIZE_SAFE_DIG)) return false;
+    if (*cur == '0') {
+        if (unlikely(len > 1)) return false;
+        *idx = 0;
+        return true;
+    }
+    if (*cur == '-') {
+        if (unlikely(len > 1)) return false;
+        *idx = USIZE_MAX;
+        return true;
+    }
+    for (; cur < end && (add = (usize)((u8)*cur - (u8)'0')) <= 9; cur++) {
+        num = num * 10 + add;
+    }
+    if (unlikely(num == 0 || cur < end)) return false;
+    *idx = num;
+    return true;
+}
+
+/**
+ Compare JSON key with token.
+ @param key a string key (yyjson_val or yyjson_mut_val)
+ @param tag the expected string key tag
+ @param token a JSON pointer token
+ @param len unescaped token length
+ @param esc number of escaped characters in this token
+ @return true if `str` is equals to `token`
+ */
+static_inline bool ptr_token_eq(void *key, u64 tag,
+                                const char *token, usize len, usize esc) {
+    yyjson_val *val = (yyjson_val *)key;
+    if (val->tag != tag) return false;
+    if (likely(!esc)) {
+        return memcmp(val->uni.str, token, len) == 0;
+    } else {
+        const char *str = val->uni.str;
+        for (; len-- > 0; token++, str++) {
+            if (*token == '~') {
+                if (*str != (*++token == '0' ? '~' : '/')) return false;
+            } else {
+                if (*str != *token) return false;
+            }
+        }
+        return true;
+    }
+}
+
+/**
+ Get a value from array by token.
+ @param arr   an array, should not be NULL or non-array type
+ @param token a JSON pointer token
+ @param len   unescaped token length
+ @param esc   number of escaped characters in this token
+ @return value at index, or NULL if token is not index or index is out of range
+ */
+static_inline yyjson_val *ptr_arr_get(yyjson_val *arr, const char *token,
+                                      usize len, usize esc) {
+    yyjson_val *val = unsafe_yyjson_get_first(arr);
+    usize num = unsafe_yyjson_get_len(arr), idx;
+    if (unlikely(num == 0)) return NULL;
+    if (unlikely(!ptr_token_to_idx(token, len, &idx))) return NULL;
+    if (unlikely(idx >= num)) return NULL;
+    if (unsafe_yyjson_arr_is_flat(arr)) {
+        return val + idx;
+    } else {
+        while (idx-- > 0) val = unsafe_yyjson_get_next(val);
+        return val;
+    }
+}
+
+/**
+ Get a value from object by token.
+ @param obj   [in] an object, should not be NULL or non-object type
+ @param token [in] a JSON pointer token
+ @param len   [in] unescaped token length
+ @param esc   [in] number of escaped characters in this token
+ @return value associated with the token, or NULL if no value
+ */
+static_inline yyjson_val *ptr_obj_get(yyjson_val *obj, const char *token,
+                                      usize len, usize esc) {
+    u64 tag = (((u64)len) << YYJSON_TAG_BIT) | YYJSON_TYPE_STR;
+    yyjson_val *key = unsafe_yyjson_get_first(obj);
+    usize num = unsafe_yyjson_get_len(obj);
+    if (unlikely(num == 0)) return NULL;
+    for (; num > 0; num--, key = unsafe_yyjson_get_next(key + 1)) {
+        if (ptr_token_eq(key, tag, token, len, esc)) return key + 1;
+    }
+    return NULL;
+}
+
+/**
+ Get a value from array by token.
+ @param arr   [in] an array, should not be NULL or non-array type
+ @param token [in] a JSON pointer token
+ @param len   [in] unescaped token length
+ @param esc   [in] number of escaped characters in this token
+ @param pre   [out] previous (sibling) value of the returned value
+ @param last  [out] whether index is last
+ @return value at index, or NULL if token is not index or index is out of range
+ */
+static_inline yyjson_mut_val *ptr_mut_arr_get(yyjson_mut_val *arr,
+                                              const char *token,
+                                              usize len, usize esc,
+                                              yyjson_mut_val **pre,
+                                              bool *last) {
+    yyjson_mut_val *val = (yyjson_mut_val *)arr->uni.ptr; /* last (tail) */
+    usize num = unsafe_yyjson_get_len(arr), idx;
+    if (last) *last = false;
+    if (pre) *pre = NULL;
+    if (unlikely(num == 0)) {
+        if (last && len == 1 && (*token == '0' || *token == '-')) *last = true;
+        return NULL;
+    }
+    if (unlikely(!ptr_token_to_idx(token, len, &idx))) return NULL;
+    if (last) *last = (idx == num || idx == USIZE_MAX);
+    if (unlikely(idx >= num)) return NULL;
+    while (idx-- > 0) val = val->next;
+    *pre = val;
+    return val->next;
+}
+
+/**
+ Get a value from object by token.
+ @param obj   [in] an object, should not be NULL or non-object type
+ @param token [in] a JSON pointer token
+ @param len   [in] unescaped token length
+ @param esc   [in] number of escaped characters in this token
+ @param pre   [out] previous (sibling) key of the returned value's key
+ @return value associated with the token, or NULL if no value
+ */
+static_inline yyjson_mut_val *ptr_mut_obj_get(yyjson_mut_val *obj,
+                                              const char *token,
+                                              usize len, usize esc,
+                                              yyjson_mut_val **pre) {
+    u64 tag = (((u64)len) << YYJSON_TAG_BIT) | YYJSON_TYPE_STR;
+    yyjson_mut_val *pre_key = (yyjson_mut_val *)obj->uni.ptr, *key;
+    usize num = unsafe_yyjson_get_len(obj);
+    if (pre) *pre = NULL;
+    if (unlikely(num == 0)) return NULL;
+    for (; num > 0; num--, pre_key = key) {
+        key = pre_key->next->next;
+        if (ptr_token_eq(key, tag, token, len, esc)) {
+            *pre = pre_key;
+            return key->next;
+        }
+    }
+    return NULL;
+}
+
+/**
+ Create a string value with JSON pointer token.
+ @param token [in] a JSON pointer token
+ @param len   [in] unescaped token length
+ @param esc   [in] number of escaped characters in this token
+ @param doc   [in] used for memory allocation when creating value
+ @return new string value, or NULL if memory allocation failed
+ */
+static_inline yyjson_mut_val *ptr_new_key(const char *token,
+                                          usize len, usize esc,
+                                          yyjson_mut_doc *doc) {
+    const char *src = token;
+    if (likely(!esc)) {
+        return yyjson_mut_strncpy(doc, src, len);
+    } else {
+        const char *end = src + len + esc;
+        char *dst = unsafe_yyjson_mut_str_alc(doc, len + esc);
+        char *str = dst;
+        if (unlikely(!dst)) return NULL;
+        for (; src < end; src++, dst++) {
+            if (*src != '~') *dst = *src;
+            else *dst = (*++src == '0' ? '~' : '/');
+        }
+        *dst = '\0';
+        return yyjson_mut_strn(doc, str, len);
+    }
+}
+
+/* macros for yyjson_ptr */
+#define return_err(_ret, _code, _pos, _msg) do { \
+    if (err) { \
+        err->code = YYJSON_PTR_ERR_##_code; \
+        err->msg = _msg; \
+        err->pos = (usize)(_pos); \
+    } \
+    return _ret; \
+} while (false)
+
+#define return_err_resolve(_ret, _pos) \
+    return_err(_ret, RESOLVE, _pos, "JSON pointer cannot be resolved")
+#define return_err_syntax(_ret, _pos) \
+    return_err(_ret, SYNTAX, _pos, "invalid escaped character")
+#define return_err_alloc(_ret) \
+    return_err(_ret, MEMORY_ALLOCATION, 0, "failed to create value")
+
+yyjson_val *unsafe_yyjson_ptr_getx(yyjson_val *val,
+                                   const char *ptr, size_t ptr_len,
+                                   yyjson_ptr_err *err) {
+    
+    const char *hdr = ptr, *end = ptr + ptr_len, *token;
+    usize len, esc;
+    yyjson_type type;
     
-    const char *hdr = *ptr;
-    const char *cur = hdr;
-    yyjson_val *i_obj = (yyjson_val *)obj;
-    yyjson_mut_val *m_obj = (yyjson_mut_val *)obj;
-    yyjson_obj_iter i_iter;
-    yyjson_mut_obj_iter m_iter;
-    void *key;
+    while (true) {
+        token = ptr_next_token(&ptr, end, &len, &esc);
+        if (unlikely(!token)) return_err_syntax(NULL, ptr - hdr);
+        type = unsafe_yyjson_get_type(val);
+        if (type == YYJSON_TYPE_OBJ) {
+            val = ptr_obj_get(val, token, len, esc);
+        } else if (type == YYJSON_TYPE_ARR) {
+            val = ptr_arr_get(val, token, len, esc);
+        } else {
+            val = NULL;
+        }
+        if (!val) return_err_resolve(NULL, token - hdr);
+        if (ptr == end) return val;
+    }
+}
+
+yyjson_mut_val *unsafe_yyjson_mut_ptr_getx(yyjson_mut_val *val,
+                                           const char *ptr,
+                                           size_t ptr_len,
+                                           yyjson_ptr_ctx *ctx,
+                                           yyjson_ptr_err *err) {
+    
+    const char *hdr = ptr, *end = ptr + ptr_len, *token;
+    usize len, esc;
+    yyjson_mut_val *ctn, *pre = NULL;
+    yyjson_type type;
+    bool idx_is_last = false;
     
-    /* skip unescaped characters */
-    while (is_unescaped(cur)) cur++;
-    if (likely(is_completed(cur))) {
-        usize len = (usize)(cur - hdr);
-        *ptr = cur;
-        return mut
-            ? (void *)yyjson_mut_obj_getn(m_obj, hdr, len)
-            : (void *)yyjson_obj_getn(i_obj, hdr, len);
+    while (true) {
+        token = ptr_next_token(&ptr, end, &len, &esc);
+        if (unlikely(!token)) return_err_syntax(NULL, ptr - hdr);
+        ctn = val;
+        type = unsafe_yyjson_get_type(val);
+        if (type == YYJSON_TYPE_OBJ) {
+            val = ptr_mut_obj_get(val, token, len, esc, &pre);
+        } else if (type == YYJSON_TYPE_ARR) {
+            val = ptr_mut_arr_get(val, token, len, esc, &pre, &idx_is_last);
+        } else {
+            val = NULL;
+        }
+        if (ctx && (ptr == end)) {
+            if (type == YYJSON_TYPE_OBJ ||
+                (type == YYJSON_TYPE_ARR && (val || idx_is_last))) {
+                ctx->ctn = ctn;
+                ctx->pre = pre;
+            }
+        }
+        if (!val) return_err_resolve(NULL, token - hdr);
+        if (ptr == end) return val;
     }
+}
+
+bool unsafe_yyjson_mut_ptr_putx(yyjson_mut_val *val,
+                                const char *ptr, size_t ptr_len,
+                                yyjson_mut_val *new_val,
+                                yyjson_mut_doc *doc,
+                                bool create_parent, bool insert_new,
+                                yyjson_ptr_ctx *ctx,
+                                yyjson_ptr_err *err) {
+    
+    const char *hdr = ptr, *end = ptr + ptr_len, *token;
+    usize token_len, esc, ctn_len;
+    yyjson_mut_val *ctn, *key, *pre = NULL;
+    yyjson_mut_val *sep_ctn = NULL, *sep_key = NULL, *sep_val = NULL;
+    yyjson_type ctn_type;
+    bool idx_is_last = false;
     
-    /* copy escaped characters to buffer */
-    if (likely(end - hdr <= BUF_SIZE)) {
-        char buf[BUF_SIZE];
-        char *dst = buf + (usize)(cur - hdr);
-        memcpy(buf, hdr, (usize)(cur - hdr));
-        while (true) {
-            if (is_unescaped(cur)) {
-                *dst++ = *cur++;
-            } else if (is_completed(cur)) {
-                usize len = (usize)(dst - buf);
-                *ptr = cur;
-                return mut
-                    ? (void *)yyjson_mut_obj_getn(m_obj, buf, len)
-                    : (void *)yyjson_obj_getn(i_obj, buf, len);
+    /* skip exist parent nodes */
+    while (true) {
+        token = ptr_next_token(&ptr, end, &token_len, &esc);
+        if (unlikely(!token)) return_err_syntax(false, ptr - hdr);
+        ctn = val;
+        ctn_type = unsafe_yyjson_get_type(ctn);
+        if (ctn_type == YYJSON_TYPE_OBJ) {
+            val = ptr_mut_obj_get(ctn, token, token_len, esc, &pre);
+        } else if (ctn_type == YYJSON_TYPE_ARR) {
+            val = ptr_mut_arr_get(ctn, token, token_len, esc, &pre,
+                                  &idx_is_last);
+        } else return_err_resolve(false, token - hdr);
+        if (!val) break;
+        if (ptr == end) break; /* is last token */
+    }
+    
+    /* create parent nodes if not exist */
+    if (unlikely(ptr != end)) { /* not last token */
+        if (!create_parent) return_err_resolve(false, token - hdr);
+        
+        /* add value at last index if container is array */
+        if (ctn_type == YYJSON_TYPE_ARR) {
+            if (!idx_is_last || !insert_new) {
+                return_err_resolve(false, token - hdr);
+            }
+            val = yyjson_mut_obj(doc);
+            if (!val) return_err_alloc(false);
+            
+            /* delay attaching until all operations are completed */
+            sep_ctn = ctn;
+            sep_key = NULL;
+            sep_val = val;
+            
+            /* move to next token */
+            ctn = val;
+            val = NULL;
+            ctn_type = YYJSON_TYPE_OBJ;
+            token = ptr_next_token(&ptr, end, &token_len, &esc);
+            if (unlikely(!token)) return_err_resolve(false, token - hdr);
+        }
+        
+        /* container is object, create parent nodes */
+        while (ptr != end) { /* not last token */
+            key = ptr_new_key(token, token_len, esc, doc);
+            if (!key) return_err_alloc(false);
+            val = yyjson_mut_obj(doc);
+            if (!val) return_err_alloc(false);
+            
+            /* delay attaching until all operations are completed */
+            if (!sep_ctn) {
+                sep_ctn = ctn;
+                sep_key = key;
+                sep_val = val;
             } else {
-                cur++; /* skip '~' */
-                if (unlikely(!is_escaped(cur))) return NULL;
-                *dst++ = (char)(*cur++ == '0' ? '~' : '/');
+                yyjson_mut_obj_add(ctn, key, val);
             }
+            
+            /* move to next token */
+            ctn = val;
+            val = NULL;
+            token = ptr_next_token(&ptr, end, &token_len, &esc);
+            if (unlikely(!token)) return_err_syntax(false, ptr - hdr);
         }
     }
     
-    /* compare byte by byte */
-    cur = hdr;
-    if (!mut) yyjson_obj_iter_init(i_obj, &i_iter);
-    else yyjson_mut_obj_iter_init(m_obj, &m_iter);
-    while ((key = mut ? (void *)yyjson_mut_obj_iter_next(&m_iter)
-                      : (void *)yyjson_obj_iter_next(&i_iter))) {
-        const char *k_str = unsafe_yyjson_get_str(key);
-        const char *k_end = k_str + unsafe_yyjson_get_len(key);
-        while (k_str < k_end) {
-            if (is_unescaped(cur) && *k_str == *cur) {
-                k_str += 1;
-                cur += 1;
-            } else if (cur < end && *cur == '~' && is_escaped(cur + 1) &&
-                       *k_str == (*(cur + 1) == '0' ? '~' : '/')) {
-                k_str += 1;
-                cur += 2;
+    /* JSON pointer is resolved, insert or replace target value */
+    ctn_len = unsafe_yyjson_get_len(ctn);
+    if (ctn_type == YYJSON_TYPE_OBJ) {
+        if (ctx) ctx->ctn = ctn;
+        if (!val || insert_new) {
+            /* insert new key-value pair */
+            key = ptr_new_key(token, token_len, esc, doc);
+            if (unlikely(!key)) return_err_alloc(false);
+            if (ctx) ctx->pre = ctn_len ? (yyjson_mut_val *)ctn->uni.ptr : key;
+            unsafe_yyjson_mut_obj_add(ctn, key, new_val, ctn_len);
+        } else {
+            /* replace exist value */
+            key = pre->next->next;
+            if (ctx) ctx->pre = pre;
+            if (ctx) ctx->old = val;
+            yyjson_mut_obj_put(ctn, key, new_val);
+        }
+    } else {
+        /* array */
+        if (ctx && (val || idx_is_last)) ctx->ctn = ctn;
+        if (insert_new) {
+            /* append new value */
+            if (val) {
+                pre->next = new_val;
+                new_val->next = val;
+                if (ctx) ctx->pre = pre;
+                unsafe_yyjson_set_len(ctn, ctn_len + 1);
+            } else if (idx_is_last) {
+                if (ctx) ctx->pre = ctn_len ?
+                    (yyjson_mut_val *)ctn->uni.ptr : new_val;
+                yyjson_mut_arr_append(ctn, new_val);
             } else {
-                break;
+                return_err_resolve(false, token - hdr);
             }
-        }
-        if (k_str == k_end && is_completed(cur)) {
-            *ptr = cur;
-            return mut
-                ? (void *)yyjson_mut_obj_iter_get_val((yyjson_mut_val *)key)
-                : (void *)yyjson_obj_iter_get_val((yyjson_val *)key);
+        } else {
+            /* replace exist value */
+            if (!val) return_err_resolve(false, token - hdr);
+            if (ctn_len > 1) {
+                new_val->next = val->next;
+                pre->next = new_val;
+                if (ctn->uni.ptr == val) ctn->uni.ptr = new_val;
+            } else {
+                new_val->next = new_val;
+                ctn->uni.ptr = new_val;
+                pre = new_val;
+            }
+            if (ctx) ctx->pre = pre;
+            if (ctx) ctx->old = val;
         }
     }
-    return NULL;
     
-#undef BUF_SIZE
-#undef is_escaped
-#undef is_unescaped
-#undef is_completed
+    /* all operations are completed, attach the new components to the target */
+    if (unlikely(sep_ctn)) {
+        if (sep_key) yyjson_mut_obj_add(sep_ctn, sep_key, sep_val);
+        else yyjson_mut_arr_append(sep_ctn, sep_val);
+    }
+    return true;
 }
 
-yyjson_api yyjson_val *unsafe_yyjson_get_pointer(yyjson_val *val,
-                                                 const char *ptr,
-                                                 usize len) {
-    const char *end = ptr + len;
-    ptr++; /* skip '/' */
-    while (true) {
-        if (yyjson_is_obj(val)) {
-            val = (yyjson_val *)pointer_read_obj(&ptr, end, val, false);
-        } else if (yyjson_is_arr(val)) {
-            val = (yyjson_val *)pointer_read_arr(&ptr, end, val, false);
+yyjson_mut_val *unsafe_yyjson_mut_ptr_replacex(
+    yyjson_mut_val *val, const char *ptr, size_t len, yyjson_mut_val *new_val,
+    yyjson_ptr_ctx *ctx, yyjson_ptr_err *err) {
+    
+    yyjson_mut_val *cur_val;
+    yyjson_ptr_ctx cur_ctx;
+    memset(&cur_ctx, 0, sizeof(cur_ctx));
+    if (!ctx) ctx = &cur_ctx;
+    cur_val = unsafe_yyjson_mut_ptr_getx(val, ptr, len, ctx, err);
+    if (!cur_val) return NULL;
+    
+    if (yyjson_mut_is_obj(ctx->ctn)) {
+        yyjson_mut_val *key = ctx->pre->next->next;
+        yyjson_mut_obj_put(ctx->ctn, key, new_val);
+    } else {
+        yyjson_ptr_ctx_replace(ctx, new_val);
+    }
+    ctx->old = cur_val;
+    return cur_val;
+}
+
+yyjson_mut_val *unsafe_yyjson_mut_ptr_removex(yyjson_mut_val *val,
+                                              const char *ptr,
+                                              size_t len,
+                                              yyjson_ptr_ctx *ctx,
+                                              yyjson_ptr_err *err) {
+    yyjson_mut_val *cur_val;
+    yyjson_ptr_ctx cur_ctx;
+    memset(&cur_ctx, 0, sizeof(cur_ctx));
+    if (!ctx) ctx = &cur_ctx;
+    cur_val = unsafe_yyjson_mut_ptr_getx(val, ptr, len, ctx, err);
+    if (cur_val) {
+        if (yyjson_mut_is_obj(ctx->ctn)) {
+            yyjson_mut_val *key = ctx->pre->next->next;
+            yyjson_mut_obj_put(ctx->ctn, key, NULL);
         } else {
-            val = NULL;
+            yyjson_ptr_ctx_remove(ctx);
         }
-        if (!val || ptr == end) return val;
-        if (*ptr++ != '/') return NULL;
+        ctx->pre = NULL;
+        ctx->old = cur_val;
     }
+    return cur_val;
 }
 
-yyjson_api yyjson_mut_val *unsafe_yyjson_mut_get_pointer(yyjson_mut_val *val,
-                                                         const char *ptr,
-                                                         usize len) {
-    const char *end = ptr + len;
-    ptr++; /* skip '/' */
-    while (true) {
-        if (yyjson_mut_is_obj(val)) {
-            val = (yyjson_mut_val *)pointer_read_obj(&ptr, end, val, true);
-        } else if (yyjson_mut_is_arr(val)) {
-            val = (yyjson_mut_val *)pointer_read_arr(&ptr, end, val, true);
-        } else {
-            val = NULL;
+/* macros for yyjson_ptr */
+#undef return_err
+#undef return_err_resolve
+#undef return_err_syntax
+#undef return_err_alloc
+
+
+
+/*==============================================================================
+ * JSON Patch API (RFC 6902)
+ *============================================================================*/
+
+/* JSON Patch operation */
+typedef enum patch_op {
+    PATCH_OP_ADD,       /* path, value */
+    PATCH_OP_REMOVE,    /* path */
+    PATCH_OP_REPLACE,   /* path, value */
+    PATCH_OP_MOVE,      /* from, path */
+    PATCH_OP_COPY,      /* from, path */
+    PATCH_OP_TEST,      /* path, value */
+    PATCH_OP_NONE       /* invalid */
+} patch_op;
+
+static patch_op patch_op_get(yyjson_val *op) {
+    const char *str = op->uni.str;
+    switch (unsafe_yyjson_get_len(op)) {
+        case 3:
+            if (!memcmp(str, "add", 3)) return PATCH_OP_ADD;
+            return PATCH_OP_NONE;
+        case 4:
+            if (!memcmp(str, "move", 4)) return PATCH_OP_MOVE;
+            if (!memcmp(str, "copy", 4)) return PATCH_OP_COPY;
+            if (!memcmp(str, "test", 4)) return PATCH_OP_TEST;
+            return PATCH_OP_NONE;
+        case 6:
+            if (!memcmp(str, "remove", 6)) return PATCH_OP_REMOVE;
+            return PATCH_OP_NONE;
+        case 7:
+            if (!memcmp(str, "replace", 7)) return PATCH_OP_REPLACE;
+            return PATCH_OP_NONE;
+        default:
+            return PATCH_OP_NONE;
+    }
+}
+
+/* macros for yyjson_patch */
+#define return_err(_code, _msg) do { \
+    if (err->ptr.code == YYJSON_PTR_ERR_MEMORY_ALLOCATION) { \
+        err->code = YYJSON_PATCH_ERROR_MEMORY_ALLOCATION; \
+        err->msg = _msg; \
+        memset(&err->ptr, 0, sizeof(yyjson_ptr_err)); \
+    } else { \
+        err->code = YYJSON_PATCH_ERROR_##_code; \
+        err->msg = _msg; \
+        err->idx = iter.idx ? iter.idx - 1 : 0; \
+    } \
+    return NULL; \
+} while (false)
+
+#define return_err_copy() \
+    return_err(MEMORY_ALLOCATION, "failed to copy value")
+#define return_err_key(_key) \
+    return_err(MISSING_KEY, "missing key " _key)
+#define return_err_val(_key) \
+    return_err(INVALID_MEMBER, "invalid member " _key)
+
+#define ptr_get(_ptr) yyjson_mut_ptr_getx( \
+    root, _ptr->uni.str, _ptr##_len, NULL, &err->ptr)
+#define ptr_add(_ptr, _val) yyjson_mut_ptr_addx( \
+    root, _ptr->uni.str, _ptr##_len, _val, doc, false, NULL, &err->ptr)
+#define ptr_remove(_ptr) yyjson_mut_ptr_removex( \
+    root, _ptr->uni.str, _ptr##_len, NULL, &err->ptr)
+#define ptr_replace(_ptr, _val)yyjson_mut_ptr_replacex( \
+    root, _ptr->uni.str, _ptr##_len, _val, NULL, &err->ptr)
+    
+yyjson_mut_val *yyjson_patch(yyjson_mut_doc *doc,
+                             yyjson_val *orig,
+                             yyjson_val *patch,
+                             yyjson_patch_err *err) {
+
+    yyjson_mut_val *root;
+    yyjson_val *obj;
+    yyjson_arr_iter iter;
+    yyjson_patch_err err_tmp;
+    if (!err) err = &err_tmp;
+    memset(err, 0, sizeof(*err));
+    memset(&iter, 0, sizeof(iter));
+    
+    if (unlikely(!doc || !orig || !patch)) {
+        return_err(INVALID_PARAMETER, "input parameter is NULL");
+    }
+    if (unlikely(!yyjson_is_arr(patch))) {
+        return_err(INVALID_PARAMETER, "input patch is not array");
+    }
+    root = yyjson_val_mut_copy(doc, orig);
+    if (unlikely(!root)) return_err_copy();
+    
+    /* iterate through the patch array */
+    yyjson_arr_iter_init(patch, &iter);
+    while ((obj = yyjson_arr_iter_next(&iter))) {
+        patch_op op_enum;
+        yyjson_val *op, *path, *from = NULL, *value;
+        yyjson_mut_val *val = NULL, *test;
+        usize path_len, from_len = 0;
+        if (unlikely(!unsafe_yyjson_is_obj(obj))) {
+            return_err(INVALID_OPERATION, "JSON patch operation is not object");
+        }
+        
+        /* get required member: op */
+        op = yyjson_obj_get(obj, "op");
+        if (unlikely(!op)) return_err_key("`op`");
+        if (unlikely(!yyjson_is_str(op))) return_err_val("`op`");
+        op_enum = patch_op_get(op);
+        
+        /* get required member: path */
+        path = yyjson_obj_get(obj, "path");
+        if (unlikely(!path)) return_err_key("`path`");
+        if (unlikely(!yyjson_is_str(path))) return_err_val("`path`");
+        path_len = unsafe_yyjson_get_len(path);
+        
+        /* get required member: value, from */
+        switch (op_enum) {
+            case PATCH_OP_ADD: case PATCH_OP_REPLACE: case PATCH_OP_TEST:
+                value = yyjson_obj_get(obj, "value");
+                if (unlikely(!value)) return_err_key("`value`");
+                val = yyjson_val_mut_copy(doc, value);
+                if (unlikely(!val)) return_err_copy();
+                break;
+            case PATCH_OP_MOVE: case PATCH_OP_COPY:
+                from = yyjson_obj_get(obj, "from");
+                if (unlikely(!from)) return_err_key("`from`");
+                if (unlikely(!yyjson_is_str(from))) return_err_val("`from`");
+                from_len = unsafe_yyjson_get_len(from);
+                break;
+            default:
+                break;
+        }
+        
+        /* perform an operation */
+        switch (op_enum) {
+            case PATCH_OP_ADD: /* add(path, val) */
+                if (unlikely(path_len == 0)) { root = val; break; }
+                if (unlikely(!ptr_add(path, val))) {
+                    return_err(POINTER, "failed to add `path`");
+                }
+                break;
+            case PATCH_OP_REMOVE: /* remove(path) */
+                if (unlikely(!ptr_remove(path))) {
+                    return_err(POINTER, "failed to remove `path`");
+                }
+                break;
+            case PATCH_OP_REPLACE: /* replace(path, val) */
+                if (unlikely(path_len == 0)) { root = val; break; }
+                if (unlikely(!ptr_replace(path, val))) {
+                    return_err(POINTER, "failed to replace `path`");
+                }
+                break;
+            case PATCH_OP_MOVE: /* val = remove(from), add(path, val) */
+                if (unlikely(from_len == 0 && path_len == 0)) break;
+                val = ptr_remove(from);
+                if (unlikely(!val)) {
+                    return_err(POINTER, "failed to remove `from`");
+                }
+                if (unlikely(path_len == 0)) { root = val; break; }
+                if (unlikely(!ptr_add(path, val))) {
+                    return_err(POINTER, "failed to add `path`");
+                }
+                break;
+            case PATCH_OP_COPY: /* val = get(from).copy, add(path, val) */
+                val = ptr_get(from);
+                if (unlikely(!val)) {
+                    return_err(POINTER, "failed to get `from`");
+                }
+                if (unlikely(path_len == 0)) { root = val; break; }
+                val = yyjson_mut_val_mut_copy(doc, val);
+                if (unlikely(!val)) return_err_copy();
+                if (unlikely(!ptr_add(path, val))) {
+                    return_err(POINTER, "failed to add `path`");
+                }
+                break;
+            case PATCH_OP_TEST: /* test = get(path), test.eq(val) */
+                test = ptr_get(path);
+                if (unlikely(!test)) {
+                    return_err(POINTER, "failed to get `path`");
+                }
+                if (unlikely(!yyjson_mut_equals(val, test))) {
+                    return_err(EQUAL, "failed to test equal");
+                }
+                break;
+            default:
+                return_err(INVALID_MEMBER, "unsupported `op`");
         }
-        if (!val || ptr == end) return val;
-        if (*ptr++ != '/') return NULL;
     }
+    return root;
 }
 
+yyjson_mut_val *yyjson_mut_patch(yyjson_mut_doc *doc,
+                                 yyjson_mut_val *orig,
+                                 yyjson_mut_val *patch,
+                                 yyjson_patch_err *err) {
+    yyjson_mut_val *root, *obj;
+    yyjson_mut_arr_iter iter;
+    yyjson_patch_err err_tmp;
+    if (!err) err = &err_tmp;
+    memset(err, 0, sizeof(*err));
+    memset(&iter, 0, sizeof(iter));
+    
+    if (unlikely(!doc || !orig || !patch)) {
+        return_err(INVALID_PARAMETER, "input parameter is NULL");
+    }
+    if (unlikely(!yyjson_mut_is_arr(patch))) {
+        return_err(INVALID_PARAMETER, "input patch is not array");
+    }
+    root = yyjson_mut_val_mut_copy(doc, orig);
+    if (unlikely(!root)) return_err_copy();
+    
+    /* iterate through the patch array */
+    yyjson_mut_arr_iter_init(patch, &iter);
+    while ((obj = yyjson_mut_arr_iter_next(&iter))) {
+        patch_op op_enum;
+        yyjson_mut_val *op, *path, *from = NULL, *value;
+        yyjson_mut_val *val = NULL, *test;
+        usize path_len, from_len = 0;
+        if (!unsafe_yyjson_is_obj(obj)) {
+            return_err(INVALID_OPERATION, "JSON patch operation is not object");
+        }
+        
+        /* get required member: op */
+        op = yyjson_mut_obj_get(obj, "op");
+        if (unlikely(!op)) return_err_key("`op`");
+        if (unlikely(!yyjson_mut_is_str(op))) return_err_val("`op`");
+        op_enum = patch_op_get((yyjson_val *)(void *)op);
+        
+        /* get required member: path */
+        path = yyjson_mut_obj_get(obj, "path");
+        if (unlikely(!path)) return_err_key("`path`");
+        if (unlikely(!yyjson_mut_is_str(path))) return_err_val("`path`");
+        path_len = unsafe_yyjson_get_len(path);
+        
+        /* get required member: value, from */
+        switch (op_enum) {
+            case PATCH_OP_ADD: case PATCH_OP_REPLACE: case PATCH_OP_TEST:
+                value = yyjson_mut_obj_get(obj, "value");
+                if (unlikely(!value)) return_err_key("`value`");
+                val = yyjson_mut_val_mut_copy(doc, value);
+                if (unlikely(!val)) return_err_copy();
+                break;
+            case PATCH_OP_MOVE: case PATCH_OP_COPY:
+                from = yyjson_mut_obj_get(obj, "from");
+                if (unlikely(!from)) return_err_key("`from`");
+                if (unlikely(!yyjson_mut_is_str(from))) {
+                    return_err_val("`from`");
+                }
+                from_len = unsafe_yyjson_get_len(from);
+                break;
+            default:
+                break;
+        }
+        
+        /* perform an operation */
+        switch (op_enum) {
+            case PATCH_OP_ADD: /* add(path, val) */
+                if (unlikely(path_len == 0)) { root = val; break; }
+                if (unlikely(!ptr_add(path, val))) {
+                    return_err(POINTER, "failed to add `path`");
+                }
+                break;
+            case PATCH_OP_REMOVE: /* remove(path) */
+                if (unlikely(!ptr_remove(path))) {
+                    return_err(POINTER, "failed to remove `path`");
+                }
+                break;
+            case PATCH_OP_REPLACE: /* replace(path, val) */
+                if (unlikely(path_len == 0)) { root = val; break; }
+                if (unlikely(!ptr_replace(path, val))) {
+                    return_err(POINTER, "failed to replace `path`");
+                }
+                break;
+            case PATCH_OP_MOVE: /* val = remove(from), add(path, val) */
+                if (unlikely(from_len == 0 && path_len == 0)) break;
+                val = ptr_remove(from);
+                if (unlikely(!val)) {
+                    return_err(POINTER, "failed to remove `from`");
+                }
+                if (unlikely(path_len == 0)) { root = val; break; }
+                if (unlikely(!ptr_add(path, val))) {
+                    return_err(POINTER, "failed to add `path`");
+                }
+                break;
+            case PATCH_OP_COPY: /* val = get(from).copy, add(path, val) */
+                val = ptr_get(from);
+                if (unlikely(!val)) {
+                    return_err(POINTER, "failed to get `from`");
+                }
+                if (unlikely(path_len == 0)) { root = val; break; }
+                val = yyjson_mut_val_mut_copy(doc, val);
+                if (unlikely(!val)) return_err_copy();
+                if (unlikely(!ptr_add(path, val))) {
+                    return_err(POINTER, "failed to add `path`");
+                }
+                break;
+            case PATCH_OP_TEST: /* test = get(path), test.eq(val) */
+                test = ptr_get(path);
+                if (unlikely(!test)) {
+                    return_err(POINTER, "failed to get `path`");
+                }
+                if (unlikely(!yyjson_mut_equals(val, test))) {
+                    return_err(EQUAL, "failed to test equal");
+                }
+                break;
+            default:
+                return_err(INVALID_MEMBER, "unsupported `op`");
+        }
+    }
+    return root;
+}
+
+/* macros for yyjson_patch */
+#undef return_err
+#undef return_err_copy
+#undef return_err_key
+#undef return_err_val
+#undef ptr_get
+#undef ptr_add
+#undef ptr_remove
+#undef ptr_replace
+
 
 
 /*==============================================================================
- * JSON Merge-Patch
+ * JSON Merge-Patch API (RFC 7386)
  *============================================================================*/
 
-yyjson_api yyjson_mut_val *yyjson_merge_patch(yyjson_mut_doc *doc,
-                                              yyjson_val *orig,
-                                              yyjson_val *patch) {
+yyjson_mut_val *yyjson_merge_patch(yyjson_mut_doc *doc,
+                                   yyjson_val *orig,
+                                   yyjson_val *patch) {
     usize idx, max;
     yyjson_val *key, *orig_val, *patch_val, local_orig;
     yyjson_mut_val *builder, *mut_key, *mut_val, *merged_val;
     
     if (unlikely(!yyjson_is_obj(patch))) {
         return yyjson_val_mut_copy(doc, patch);
     }
@@ -1715,51 +2502,49 @@
     
     if (!yyjson_is_obj(orig)) {
         orig = &local_orig;
         orig->tag = builder->tag;
         orig->uni = builder->uni;
     }
     
+    /* If orig is contributing, copy any items not modified by the patch */
+    if (orig != &local_orig)
+    {
+        yyjson_obj_foreach(orig, idx, max, key, orig_val) {
+            patch_val = yyjson_obj_getn(patch,
+                                        unsafe_yyjson_get_str(key),
+                                        unsafe_yyjson_get_len(key));
+            if (!patch_val) {
+                mut_key = yyjson_val_mut_copy(doc, key);
+                mut_val = yyjson_val_mut_copy(doc, orig_val);
+                if (!yyjson_mut_obj_add(builder, mut_key, mut_val)) return NULL;
+            }
+        }
+    }
+
     /* Merge items modified by the patch. */
     yyjson_obj_foreach(patch, idx, max, key, patch_val) {
         /* null indicates the field is removed. */
         if (unsafe_yyjson_is_null(patch_val)) {
             continue;
         }
         mut_key = yyjson_val_mut_copy(doc, key);
         orig_val = yyjson_obj_getn(orig,
                                    unsafe_yyjson_get_str(key),
                                    unsafe_yyjson_get_len(key));
         merged_val = yyjson_merge_patch(doc, orig_val, patch_val);
         if (!yyjson_mut_obj_add(builder, mut_key, merged_val)) return NULL;
     }
     
-    /* Exit early, if orig is not contributing to the final result. */
-    if (orig == &local_orig) {
-        return builder;
-    }
-    
-    /* Copy over any items that weren't modified by the patch. */
-    yyjson_obj_foreach(orig, idx, max, key, orig_val) {
-        patch_val = yyjson_obj_getn(patch,
-                                    unsafe_yyjson_get_str(key),
-                                    unsafe_yyjson_get_len(key));
-        if (!patch_val) {
-            mut_key = yyjson_val_mut_copy(doc, key);
-            mut_val = yyjson_val_mut_copy(doc, orig_val);
-            if (!yyjson_mut_obj_add(builder, mut_key, mut_val)) return NULL;
-        }
-    }
-    
     return builder;
 }
 
-yyjson_api yyjson_mut_val *yyjson_mut_merge_patch(yyjson_mut_doc *doc,
-                                                  yyjson_mut_val *orig,
-                                                  yyjson_mut_val *patch) {
+yyjson_mut_val *yyjson_mut_merge_patch(yyjson_mut_doc *doc,
+                                       yyjson_mut_val *orig,
+                                       yyjson_mut_val *patch) {
     usize idx, max;
     yyjson_mut_val *key, *orig_val, *patch_val, local_orig;
     yyjson_mut_val *builder, *mut_key, *mut_val, *merged_val;
     
     if (unlikely(!yyjson_mut_is_obj(patch))) {
         return yyjson_mut_val_mut_copy(doc, patch);
     }
@@ -1769,48 +2554,48 @@
     
     if (!yyjson_mut_is_obj(orig)) {
         orig = &local_orig;
         orig->tag = builder->tag;
         orig->uni = builder->uni;
     }
     
+    /* If orig is contributing, copy any items not modified by the patch */
+    if (orig != &local_orig)
+    {
+        yyjson_mut_obj_foreach(orig, idx, max, key, orig_val) {
+            patch_val = yyjson_mut_obj_getn(patch,
+                                            unsafe_yyjson_get_str(key),
+                                            unsafe_yyjson_get_len(key));
+            if (!patch_val) {
+                mut_key = yyjson_mut_val_mut_copy(doc, key);
+                mut_val = yyjson_mut_val_mut_copy(doc, orig_val);
+                if (!yyjson_mut_obj_add(builder, mut_key, mut_val)) return NULL;
+            }
+        }
+    }
+
     /* Merge items modified by the patch. */
     yyjson_mut_obj_foreach(patch, idx, max, key, patch_val) {
         /* null indicates the field is removed. */
         if (unsafe_yyjson_is_null(patch_val)) {
             continue;
         }
         mut_key = yyjson_mut_val_mut_copy(doc, key);
         orig_val = yyjson_mut_obj_getn(orig,
                                        unsafe_yyjson_get_str(key),
                                        unsafe_yyjson_get_len(key));
         merged_val = yyjson_mut_merge_patch(doc, orig_val, patch_val);
         if (!yyjson_mut_obj_add(builder, mut_key, merged_val)) return NULL;
     }
     
-    /* Exit early, if orig is not contributing to the final result. */
-    if (orig == &local_orig) {
-        return builder;
-    }
-    
-    /* Copy over any items that weren't modified by the patch. */
-    yyjson_mut_obj_foreach(orig, idx, max, key, orig_val) {
-        patch_val = yyjson_mut_obj_getn(patch,
-                                        unsafe_yyjson_get_str(key),
-                                        unsafe_yyjson_get_len(key));
-        if (!patch_val) {
-            mut_key = yyjson_mut_val_mut_copy(doc, key);
-            mut_val = yyjson_mut_val_mut_copy(doc, orig_val);
-            if (!yyjson_mut_obj_add(builder, mut_key, mut_val)) return NULL;
-        }
-    }
-    
     return builder;
 }
 
+#endif /* YYJSON_DISABLE_UTILS */
+
 
 
 /*==============================================================================
  * Power10 Lookup Table
  * These data are used by the floating-point number reader and writer.
  *============================================================================*/
 
@@ -2552,32 +3337,35 @@
 
 /** JSON container character: '{', '['. */
 static const char_type CHAR_TYPE_CONTAINER  = 1 << 4;
 
 /** Comment character: '/'. */
 static const char_type CHAR_TYPE_COMMENT    = 1 << 5;
 
-/** Line end character '\\n', '\\r', '\0'. */
+/** Line end character: '\\n', '\\r', '\0'. */
 static const char_type CHAR_TYPE_LINE_END   = 1 << 6;
 
+/** Hexadecimal numeric character: [0-9a-fA-F]. */
+static const char_type CHAR_TYPE_HEX        = 1 << 7;
+
 /** Character type table (generate with misc/make_tables.c) */
 static const char_type char_table[256] = {
     0x44, 0x04, 0x04, 0x04, 0x04, 0x04, 0x04, 0x04,
     0x04, 0x05, 0x45, 0x04, 0x04, 0x45, 0x04, 0x04,
     0x04, 0x04, 0x04, 0x04, 0x04, 0x04, 0x04, 0x04,
     0x04, 0x04, 0x04, 0x04, 0x04, 0x04, 0x04, 0x04,
     0x01, 0x00, 0x04, 0x00, 0x00, 0x00, 0x00, 0x00,
     0x00, 0x00, 0x00, 0x00, 0x00, 0x02, 0x00, 0x20,
-    0x02, 0x02, 0x02, 0x02, 0x02, 0x02, 0x02, 0x02,
-    0x02, 0x02, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
-    0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
+    0x82, 0x82, 0x82, 0x82, 0x82, 0x82, 0x82, 0x82,
+    0x82, 0x82, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
+    0x00, 0x80, 0x80, 0x80, 0x80, 0x80, 0x80, 0x00,
     0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
     0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
     0x00, 0x00, 0x00, 0x10, 0x04, 0x00, 0x00, 0x00,
-    0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
+    0x00, 0x80, 0x80, 0x80, 0x80, 0x80, 0x80, 0x00,
     0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
     0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
     0x00, 0x00, 0x00, 0x10, 0x00, 0x00, 0x00, 0x00,
     0x08, 0x08, 0x08, 0x08, 0x08, 0x08, 0x08, 0x08,
     0x08, 0x08, 0x08, 0x08, 0x08, 0x08, 0x08, 0x08,
     0x08, 0x08, 0x08, 0x08, 0x08, 0x08, 0x08, 0x08,
     0x08, 0x08, 0x08, 0x08, 0x08, 0x08, 0x08, 0x08,
@@ -2616,25 +3404,30 @@
 }
 
 /** Match a JSON container: '{', '['. */
 static_inline bool char_is_container(u8 c) {
     return char_is_type(c, (char_type)CHAR_TYPE_CONTAINER);
 }
 
-/** Match a stop character in ASCII string: '"', '\', [0x00-0x1F], [0x80-0xFF]*/
+/** Match a stop character in ASCII string: '"', '\', [0x00-0x1F,0x80-0xFF]. */
 static_inline bool char_is_ascii_stop(u8 c) {
     return char_is_type(c, (char_type)(CHAR_TYPE_ESC_ASCII |
                                        CHAR_TYPE_NON_ASCII));
 }
 
-/** Match a line end character: '\\n', '\\r', '\0'*/
+/** Match a line end character: '\\n', '\\r', '\0'. */
 static_inline bool char_is_line_end(u8 c) {
     return char_is_type(c, (char_type)CHAR_TYPE_LINE_END);
 }
 
+/** Match a hexadecimal numeric character: [0-9a-fA-F]. */
+static_inline bool char_is_hex(u8 c) {
+    return char_is_type(c, (char_type)CHAR_TYPE_HEX);
+}
+
 
 
 /*==============================================================================
  * Digit Character Matcher
  *============================================================================*/
 
 /** Digit type */
@@ -2923,15 +3716,15 @@
     cur += (*cur == '-');
     
     /* read first digit, check leading zero */
     if (unlikely(!digi_is_digit(*cur))) {
         if (unlikely(ext)) {
             if (read_inf_or_nan(*hdr == '-', &cur, pre, val)) return_raw();
         }
-        return_err(cur - 1, "no digit after minus sign");
+        return_err(cur, "no digit after minus sign");
     }
     
     /* read integral part */
     if (*cur == '0') {
         cur++;
         if (unlikely(digi_is_digit(*cur))) {
             return_err(cur - 1, "number with leading zero is not allowed");
@@ -2942,24 +3735,24 @@
         if (!digi_is_fp(*cur)) return_raw();
     }
     
     /* read fraction part */
     if (*cur == '.') {
         cur++;
         if (!digi_is_digit(*cur++)) {
-            return_err(cur - 1, "no digit after decimal point");
+            return_err(cur, "no digit after decimal point");
         }
         while (digi_is_digit(*cur)) cur++;
     }
     
     /* read exponent part */
     if (digi_is_exp(*cur)) {
         cur += 1 + digi_is_sign(cur[1]);
         if (!digi_is_digit(*cur++)) {
-            return_err(cur - 1, "no digit after exponent sign");
+            return_err(cur, "no digit after exponent sign");
         }
         while (digi_is_digit(*cur)) cur++;
     }
     
     return_raw();
     
 #undef return_err
@@ -3007,14 +3800,123 @@
         }
         break;
     }
     *end = cur;
     return hdr != cur;
 }
 
+/**
+ Check truncated string.
+ Returns true if `cur` match `str` but is truncated.
+ */
+static_inline bool is_truncated_str(u8 *cur, u8 *end,
+                                    const char *str,
+                                    bool case_sensitive) {
+    usize len = strlen(str);
+    if (cur + len <= end || end <= cur) return false;
+    if (case_sensitive) {
+        return memcmp(cur, str, (usize)(end - cur)) == 0;
+    }
+    for (; cur < end; cur++, str++) {
+        if ((*cur != (u8)*str) && (*cur != (u8)*str - 'a' + 'A')) {
+            return false;
+        }
+    }
+    return true;
+}
+
+/**
+ Check truncated JSON on parsing errors.
+ Returns true if the input is valid but truncated.
+ */
+static_noinline bool is_truncated_end(u8 *hdr, u8 *cur, u8 *end,
+                                      yyjson_read_code code,
+                                      yyjson_read_flag flg) {
+    if (cur >= end) return true;
+    if (code == YYJSON_READ_ERROR_LITERAL) {
+        if (is_truncated_str(cur, end, "true", true) ||
+            is_truncated_str(cur, end, "false", true) ||
+            is_truncated_str(cur, end, "null", true)) {
+            return true;
+        }
+    }
+    if (code == YYJSON_READ_ERROR_UNEXPECTED_CHARACTER ||
+        code == YYJSON_READ_ERROR_INVALID_NUMBER ||
+        code == YYJSON_READ_ERROR_LITERAL) {
+        if ((flg & YYJSON_READ_ALLOW_INF_AND_NAN)) {
+            if (*cur == '-') cur++;
+            if (is_truncated_str(cur, end, "infinity", false) ||
+                is_truncated_str(cur, end, "nan", false)) {
+                return true;
+            }
+        }
+    }
+    if (code == YYJSON_READ_ERROR_UNEXPECTED_CONTENT) {
+        if (flg & YYJSON_READ_ALLOW_INF_AND_NAN) {
+            if (hdr + 3 <= cur &&
+                is_truncated_str(cur - 3, end, "infinity", false)) {
+                return true; /* e.g. infin would be read as inf + in */
+            }
+        }
+    }
+    if (code == YYJSON_READ_ERROR_INVALID_STRING) {
+        usize len = (usize)(end - cur);
+        
+        /* unicode escape sequence */
+        if (*cur == '\\') {
+            if (len == 1) return true;
+            if (len <= 5) {
+                if (*++cur != 'u') return false;
+                for (++cur; cur < end; cur++) {
+                    if (!char_is_hex(*cur)) return false;
+                }
+                return true;
+            }
+            return false;
+        }
+        
+        /* 2 to 4 bytes UTF-8, see `read_string()` for details. */
+        if (*cur & 0x80) {
+            u8 c0 = cur[0], c1 = cur[1], c2 = cur[2];
+            if (len == 1) {
+                /* 2 bytes UTF-8, truncated */
+                if ((c0 & 0xE0) == 0xC0 && (c0 & 0x1E) != 0x00) return true;
+                /* 3 bytes UTF-8, truncated */
+                if ((c0 & 0xF0) == 0xE0) return true;
+                /* 4 bytes UTF-8, truncated */
+                if ((c0 & 0xF8) == 0xF0 && (c0 & 0x07) <= 0x04) return true;
+            }
+            if (len == 2) {
+                /* 3 bytes UTF-8, truncated */
+                if ((c0 & 0xF0) == 0xE0 &&
+                    (c1 & 0xC0) == 0x80) {
+                    u8 pat = (u8)(((c0 & 0x0F) << 1) | ((c1 & 0x20) >> 5));
+                    return 0x01 <= pat && pat != 0x1B;
+                }
+                /* 4 bytes UTF-8, truncated */
+                if ((c0 & 0xF8) == 0xF0 &&
+                    (c1 & 0xC0) == 0x80) {
+                    u8 pat = (u8)(((c0 & 0x07) << 2) | ((c1 & 0x30) >> 4));
+                    return 0x01 <= pat && pat <= 0x10;
+                }
+            }
+            if (len == 3) {
+                /* 4 bytes UTF-8, truncated */
+                if ((c0 & 0xF8) == 0xF0 &&
+                    (c1 & 0xC0) == 0x80 &&
+                    (c2 & 0xC0) == 0x80) {
+                    u8 pat = (u8)(((c0 & 0x07) << 2) | ((c1 & 0x30) >> 4));
+                    return 0x01 <= pat && pat <= 0x10;
+                }
+            }
+        }
+    }
+    return false;
+}
+
 
 
 #if YYJSON_HAS_IEEE_754 && !YYJSON_DISABLE_FAST_FP_CONV /* FP_READER */
 
 /*==============================================================================
  * BigInt For Floating Point Number Reader
  *
@@ -3305,14 +4207,20 @@
     
 #define return_err(_pos, _msg) do { \
     *msg = _msg; \
     *end = _pos; \
     return false; \
 } while (false)
     
+#define return_0() do { \
+    val->tag = YYJSON_TYPE_NUM | (u8)((u8)sign << 3); \
+    val->uni.u64 = 0; \
+    *end = cur; return true; \
+} while (false)
+
 #define return_i64(_v) do { \
     val->tag = YYJSON_TYPE_NUM | (u8)((u8)sign << 3); \
     val->uni.u64 = (u64)(sign ? (u64)(~(_v) + 1) : (u64)(_v)); \
     *end = cur; return true; \
 } while (false)
     
 #define return_f64(_v) do { \
@@ -3363,22 +4271,22 @@
         if (unlikely(*cur != '0')) { /* non-digit char */
             if (unlikely(ext)) {
                 if (read_inf_or_nan(sign, &cur, pre, val)) {
                     *end = cur;
                     return true;
                 }
             }
-            return_err(cur - 1, "no digit after minus sign");
+            return_err(cur, "no digit after minus sign");
         }
         /* begin with 0 */
-        if (likely(!digi_is_digit_or_fp(*++cur))) return_i64(0);
+        if (likely(!digi_is_digit_or_fp(*++cur))) return_0();
         if (likely(*cur == '.')) {
             dot_pos = cur++;
             if (unlikely(!digi_is_digit(*cur))) {
-                return_err(cur - 1, "no digit after decimal point");
+                return_err(cur, "no digit after decimal point");
             }
             while (unlikely(*cur == '0')) cur++;
             if (likely(digi_is_digit(*cur))) {
                 /* first non-zero digit after decimal point */
                 sig = (u64)(*cur - '0'); /* read first digit */
                 cur--;
                 goto digi_frac_1; /* continue read fraction part */
@@ -3386,44 +4294,37 @@
         }
         if (unlikely(digi_is_digit(*cur))) {
             return_err(cur - 1, "number with leading zero is not allowed");
         }
         if (unlikely(digi_is_exp(*cur))) { /* 0 with any exponent is still 0 */
             cur += (usize)1 + digi_is_sign(cur[1]);
             if (unlikely(!digi_is_digit(*cur))) {
-                return_err(cur - 1, "no digit after exponent sign");
+                return_err(cur, "no digit after exponent sign");
             }
             while (digi_is_digit(*++cur));
         }
         return_f64_raw(0);
     }
     
     /* begin with non-zero digit */
     sig = (u64)(*cur - '0');
     
     /*
      Read integral part, same as the following code.
-     For more explanation, see the comments under label `skip_ascii_begin`.
      
          for (int i = 1; i <= 18; i++) {
             num = cur[i] - '0';
             if (num <= 9) sig = num + sig * 10;
             else goto digi_sepr_i;
          }
      */
-#if YYJSON_IS_REAL_GCC
-#define expr_intg(i) \
-    if (likely((num = (u64)(cur[i] - (u8)'0')) <= 9)) sig = num + sig * 10; \
-    else { __asm volatile("":"=m"(cur[i])::); goto digi_sepr_##i; }
-#else
 #define expr_intg(i) \
     if (likely((num = (u64)(cur[i] - (u8)'0')) <= 9)) sig = num + sig * 10; \
     else { goto digi_sepr_##i; }
-#endif
-    repeat_in_1_18(expr_intg);
+    repeat_in_1_18(expr_intg)
 #undef expr_intg
     
     
     cur += 19; /* skip continuous 19 digits */
     if (!digi_is_digit_or_fp(*cur)) {
         /* this number is an integer consisting of 19 digits */
         if (sign && (sig > ((u64)1 << 63))) { /* overflow */
@@ -3442,27 +4343,19 @@
     if (likely(cur[i] == '.')) goto digi_frac_##i; \
     cur += i; sig_end = cur; goto digi_exp_more;
     repeat_in_1_18(expr_sepr)
 #undef expr_sepr
     
     
     /* read fraction part */
-#if YYJSON_IS_REAL_GCC
-#define expr_frac(i) \
-    digi_frac_##i: \
-    if (likely((num = (u64)(cur[i + 1] - (u8)'0')) <= 9)) \
-        sig = num + sig * 10; \
-    else { __asm volatile("":"=m"(cur[i + 1])::); goto digi_stop_##i; }
-#else
 #define expr_frac(i) \
     digi_frac_##i: \
     if (likely((num = (u64)(cur[i + 1] - (u8)'0')) <= 9)) \
         sig = num + sig * 10; \
     else { goto digi_stop_##i; }
-#endif
     repeat_in_1_18(expr_frac)
 #undef expr_frac
     
     cur += 20; /* skip 19 digits and 1 decimal point */
     if (!digi_is_digit(*cur)) goto digi_frac_end; /* fraction part end */
     goto digi_frac_more; /* read more digits in fraction part */
     
@@ -3535,15 +4428,15 @@
     if (digi_is_exp(*cur)) goto digi_exp_more;
     goto digi_exp_finish;
     
     
     /* fraction part end */
 digi_frac_end:
     if (unlikely(dot_pos + 1 == cur)) {
-        return_err(cur - 1, "no digit after decimal point");
+        return_err(cur, "no digit after decimal point");
     }
     sig_end = cur;
     exp_sig = -(i64)((u64)(cur - dot_pos) - 1);
     if (likely(!digi_is_exp(*cur))) {
         if (unlikely(exp_sig < F64_MIN_DEC_EXP - 19)) {
             return_f64_raw(0); /* underflow */
         }
@@ -3555,15 +4448,15 @@
     
     
     /* read exponent part */
 digi_exp_more:
     exp_sign = (*++cur == '-');
     cur += digi_is_sign(*cur);
     if (unlikely(!digi_is_digit(*cur))) {
-        return_err(cur - 1, "no digit after exponent sign");
+        return_err(cur, "no digit after exponent sign");
     }
     while (*cur == '0') cur++;
     
     /* read exponent literal */
     tmp = cur;
     while (digi_is_digit(*cur)) {
         exp_lit = (i64)((u8)(*cur++ - '0') + (u64)exp_lit * 10);
@@ -3884,14 +4777,15 @@
         if (unlikely(raw == F64_RAW_INF)) return_inf();
         return_f64_raw(raw);
     }
     
 #undef has_flag
 #undef return_err
 #undef return_inf
+#undef return_0
 #undef return_i64
 #undef return_f64
 #undef return_f64_raw
 }
 
 
 
@@ -3910,14 +4804,20 @@
     
 #define return_err(_pos, _msg) do { \
     *msg = _msg; \
     *end = _pos; \
     return false; \
 } while (false)
     
+#define return_0() do { \
+    val->tag = YYJSON_TYPE_NUM | (u64)((u8)sign << 3); \
+    val->uni.u64 = 0; \
+    *end = cur; return true; \
+} while (false)
+
 #define return_i64(_v) do { \
     val->tag = YYJSON_TYPE_NUM | (u64)((u8)sign << 3); \
     val->uni.u64 = (u64)(sign ? (u64)(~(_v) + 1) : (u64)(_v)); \
     *end = cur; return true; \
 } while (false)
     
 #define return_f64(_v) do { \
@@ -3953,30 +4853,30 @@
     if (unlikely(!digi_is_digit(*cur))) {
         if (unlikely(ext)) {
             if (read_inf_or_nan(sign, &cur, pre, val)) {
                 *end = cur;
                 return true;
             }
         }
-        return_err(cur - 1, "no digit after minus sign");
+        return_err(cur, "no digit after minus sign");
     }
     if (*cur == '0') {
         cur++;
         if (unlikely(digi_is_digit(*cur))) {
             return_err(cur - 1, "number with leading zero is not allowed");
         }
-        if (!digi_is_fp(*cur)) return_i64(0);
+        if (!digi_is_fp(*cur)) return_0();
         goto read_double;
     }
     
     /* read continuous digits, up to 19 characters */
 #define expr_intg(i) \
     if (likely((num = (u64)(cur[i] - (u8)'0')) <= 9)) sig = num + sig * 10; \
     else { cur += i; goto intg_end; }
-    repeat_in_1_18(expr_intg);
+    repeat_in_1_18(expr_intg)
 #undef expr_intg
     
     /* here are 19 continuous digits, skip them */
     cur += 19;
     if (digi_is_digit(cur[0]) && !digi_is_digit_or_fp(cur[1])) {
         /* this number is an integer consisting of 20 digits */
         num = (u8)(*cur - '0');
@@ -4002,25 +4902,27 @@
 read_double:
     /* this number should be read as double */
     while (digi_is_digit(*cur)) cur++;
     if (*cur == '.') {
         /* skip fraction part */
         dot = cur;
         cur++;
-        if (!digi_is_digit(*cur++)) {
-            return_err(cur - 1, "no digit after decimal point");
+        if (!digi_is_digit(*cur)) {
+            return_err(cur, "no digit after decimal point");
         }
+        cur++;
         while (digi_is_digit(*cur)) cur++;
     }
     if (digi_is_exp(*cur)) {
         /* skip exponent part */
         cur += 1 + digi_is_sign(cur[1]);
-        if (!digi_is_digit(*cur++)) {
-            return_err(cur - 1, "no digit after exponent sign");
+        if (!digi_is_digit(*cur)) {
+            return_err(cur, "no digit after exponent sign");
         }
+        cur++;
         while (digi_is_digit(*cur)) cur++;
     }
     
     /*
      libc's strtod() is used to parse the floating-point number.
      
      Note that the decimal point character used by strtod() is locale-dependent,
@@ -4039,25 +4941,26 @@
         if (cut) *cur = ' ';
         val->uni.f64 = strtod((const char *)hdr, (char **)&f64_end);
         if (cut) *cur = ',';
         if (unlikely(f64_end != cur)) {
             return_err(hdr, "strtod() failed to parse the number");
         }
     }
-    if (unlikely(val->uni.f64 == HUGE_VAL || val->uni.f64 == -HUGE_VAL)) {
+    if (unlikely(val->uni.f64 >= HUGE_VAL || val->uni.f64 <= -HUGE_VAL)) {
         if (!ext) {
             return_err(hdr, "number is infinity when parsed as double");
         }
     }
     val->tag = YYJSON_TYPE_NUM | YYJSON_SUBTYPE_REAL;
     *end = cur;
     return true;
     
 #undef has_flag
 #undef return_err
+#undef return_0
 #undef return_i64
 #undef return_f64
 }
 
 #endif /* FP_READER */
 
 
@@ -4226,29 +5129,29 @@
      compiler may not generate instructions as expected, so we rewrite it with
      explicit goto statements. We hope the compiler can generate instructions
      like this: https://godbolt.org/z/8vjsYq
      
          while (true) repeat16({
             if (likely(!(char_is_ascii_stop(*src)))) src++;
             else break;
-         });
+         })
      */
 #define expr_jump(i) \
     if (likely(!char_is_ascii_stop(src[i]))) {} \
     else goto skip_ascii_stop##i;
     
 #define expr_stop(i) \
     skip_ascii_stop##i: \
     src += i; \
     goto skip_ascii_end;
     
-    repeat16_incr(expr_jump);
+    repeat16_incr(expr_jump)
     src += 16;
     goto skip_ascii_begin;
-    repeat16_incr(expr_stop);
+    repeat16_incr(expr_stop)
     
 #undef expr_jump
 #undef expr_stop
     
 skip_ascii_end:
     
     /*
@@ -4256,15 +5159,15 @@
      These instructions are useless and will degrade performance.
      This inline asm is a hint for gcc: "the memory has been modified,
      do not cache it".
      
      MSVC, Clang, ICC can generate expected instructions without this hint.
      */
 #if YYJSON_IS_REAL_GCC
-    __asm volatile("":"=m"(*src)::);
+    __asm__ volatile("":"=m"(*src));
 #endif
     if (likely(*src == '"')) {
         val->tag = ((u64)(src - cur) << YYJSON_TAG_BIT) | YYJSON_TYPE_STR;
         val->uni.str = (const char *)cur;
         *src = '\0';
         *end = src + 1;
         return true;
@@ -4312,15 +5215,15 @@
             case 'b':  *dst++ = '\b'; src++; break;
             case 'f':  *dst++ = '\f'; src++; break;
             case 'n':  *dst++ = '\n'; src++; break;
             case 'r':  *dst++ = '\r'; src++; break;
             case 't':  *dst++ = '\t'; src++; break;
             case 'u':
                 if (unlikely(!read_hex_u16(++src, &hi))) {
-                    return_err(src - 2, "invalid escaped unicode in string");
+                    return_err(src - 2, "invalid escaped sequence in string");
                 }
                 src += 4;
                 if (likely((hi & 0xF800) != 0xD800)) {
                     /* a BMP character */
                     if (hi >= 0x800) {
                         *dst++ = (u8)(0xE0 | (hi >> 12));
                         *dst++ = (u8)(0x80 | ((hi >> 6) & 0x3F));
@@ -4332,17 +5235,19 @@
                         *dst++ = (u8)hi;
                     }
                 } else {
                     /* a non-BMP character, represented as a surrogate pair */
                     if (unlikely((hi & 0xFC00) != 0xD800)) {
                         return_err(src - 6, "invalid high surrogate in string");
                     }
-                    if (unlikely(!byte_match_2(src, "\\u")) ||
-                        unlikely(!read_hex_u16(src + 2, &lo))) {
-                        return_err(src, "no matched low surrogate in string");
+                    if (unlikely(!byte_match_2(src, "\\u"))) {
+                        return_err(src, "no low surrogate in string");
+                    }
+                    if (unlikely(!read_hex_u16(src + 2, &lo))) {
+                        return_err(src, "invalid escaped sequence in string");
                     }
                     if (unlikely((lo & 0xFC00) != 0xDC00)) {
                         return_err(src, "invalid low surrogate in string");
                     }
                     uni = ((((u32)hi - 0xD800) << 10) |
                             ((u32)lo - 0xDC00)) + 0x10000;
                     *dst++ = (u8)(0xF0 | (uni >> 18));
@@ -4369,26 +5274,26 @@
 copy_ascii:
     /*
      Copy continuous ASCII, loop unrolling, same as the following code:
      
          while (true) repeat16({
             if (unlikely(char_is_ascii_stop(*src))) break;
             *dst++ = *src++;
-         });
+         })
      */
 #if YYJSON_IS_REAL_GCC
 #   define expr_jump(i) \
     if (likely(!(char_is_ascii_stop(src[i])))) {} \
-    else { __asm volatile("":"=m"(src[i])::); goto copy_ascii_stop_##i; }
+    else { __asm__ volatile("":"=m"(src[i])); goto copy_ascii_stop_##i; }
 #else
 #   define expr_jump(i) \
     if (likely(!(char_is_ascii_stop(src[i])))) {} \
     else { goto copy_ascii_stop_##i; }
 #endif
-    repeat16_incr(expr_jump);
+    repeat16_incr(expr_jump)
 #undef expr_jump
     
     byte_move_16(dst, src);
     src += 16;
     dst += 16;
     goto copy_ascii;
     
@@ -4535,15 +5440,15 @@
                                              yyjson_alc alc,
                                              yyjson_read_flag flg,
                                              yyjson_read_err *err) {
     
 #define has_flag(_flag) unlikely((flg & YYJSON_READ_##_flag) != 0)
     
 #define return_err(_pos, _code, _msg) do { \
-    if (_pos >= end) { \
+    if (is_truncated_end(hdr, _pos, end, YYJSON_READ_ERROR_##_code, flg)) { \
         err->pos = (usize)(end - hdr); \
         err->code = YYJSON_READ_ERROR_UNEXPECTED_END; \
         err->msg = "unexpected end of data"; \
     } else { \
         err->pos = (usize)(_pos - hdr); \
         err->code = YYJSON_READ_ERROR_##_code; \
         err->msg = _msg; \
@@ -4654,15 +5559,15 @@
                                            yyjson_alc alc,
                                            yyjson_read_flag flg,
                                            yyjson_read_err *err) {
     
 #define has_flag(_flag) unlikely((flg & YYJSON_READ_##_flag) != 0)
     
 #define return_err(_pos, _code, _msg) do { \
-    if (_pos >= end) { \
+    if (is_truncated_end(hdr, _pos, end, YYJSON_READ_ERROR_##_code, flg)) { \
         err->pos = (usize)(end - hdr); \
         err->code = YYJSON_READ_ERROR_UNEXPECTED_END; \
         err->msg = "unexpected end of data"; \
     } else { \
         err->pos = (usize)(_pos - hdr); \
         err->code = YYJSON_READ_ERROR_##_code; \
         err->msg = _msg; \
@@ -4670,17 +5575,19 @@
     if (val_hdr) alc.free(alc.ctx, (void *)val_hdr); \
     return NULL; \
 } while (false)
     
 #define val_incr() do { \
     val++; \
     if (unlikely(val >= val_end)) { \
+        usize alc_old = alc_len; \
         alc_len += alc_len / 2; \
         if ((alc_len >= alc_max)) goto fail_alloc; \
         val_tmp = (yyjson_val *)alc.realloc(alc.ctx, (void *)val_hdr, \
+            alc_old * sizeof(yyjson_val), \
             alc_len * sizeof(yyjson_val)); \
         if ((!val_tmp)) goto fail_alloc; \
         val = val_tmp + (usize)(val - val_hdr); \
         ctn = val_tmp + (usize)(ctn - val_hdr); \
         val_hdr = val_tmp; \
         val_end = val_tmp + (alc_len - 2); \
     } \
@@ -4791,14 +5698,15 @@
         }
         goto fail_literal;
     }
     if (*cur == ']') {
         cur++;
         if (likely(ctn_len == 0)) goto arr_end;
         if (has_flag(ALLOW_TRAILING_COMMAS)) goto arr_end;
+        while (*cur != ',') cur--;
         goto fail_trailing_comma;
     }
     if (char_is_space(*cur)) {
         while (char_is_space(*++cur));
         goto arr_val_begin;
     }
     if (unlikely(ext) && (*cur == 'i' || *cur == 'I' || *cur == 'N')) {
@@ -4868,14 +5776,15 @@
         if (likely(read_string(&cur, end, inv, val, &msg))) goto obj_key_end;
         goto fail_string;
     }
     if (likely(*cur == '}')) {
         cur++;
         if (likely(ctn_len == 0)) goto obj_end;
         if (has_flag(ALLOW_TRAILING_COMMAS)) goto obj_end;
+        while (*cur != ',') cur--;
         goto fail_trailing_comma;
     }
     if (char_is_space(*cur)) {
         while (char_is_space(*++cur));
         goto obj_key_begin;
     }
     if (has_flag(ALLOW_COMMENTS)) {
@@ -4990,15 +5899,18 @@
     } else {
         goto arr_val_end;
     }
     
 doc_end:
     /* check invalid contents after json document */
     if (unlikely(cur < end) && !has_flag(STOP_WHEN_DONE)) {
-        if (has_flag(ALLOW_COMMENTS)) skip_spaces_and_comments(&cur);
+        if (has_flag(ALLOW_COMMENTS)) {
+            skip_spaces_and_comments(&cur);
+            if (byte_match_2(cur, "/*")) goto fail_comment;
+        }
         else while (char_is_space(*cur)) cur++;
         if (unlikely(cur < end)) goto fail_garbage;
     }
     
     if (pre && *pre) **pre = '\0';
     doc = (yyjson_doc *)val_hdr;
     doc->root = val_hdr + hdr_len;
@@ -5037,15 +5949,15 @@
                                            yyjson_alc alc,
                                            yyjson_read_flag flg,
                                            yyjson_read_err *err) {
     
 #define has_flag(_flag) unlikely((flg & YYJSON_READ_##_flag) != 0)
     
 #define return_err(_pos, _code, _msg) do { \
-    if (_pos >= end) { \
+    if (is_truncated_end(hdr, _pos, end, YYJSON_READ_ERROR_##_code, flg)) { \
         err->pos = (usize)(end - hdr); \
         err->code = YYJSON_READ_ERROR_UNEXPECTED_END; \
         err->msg = "unexpected end of data"; \
     } else { \
         err->pos = (usize)(_pos - hdr); \
         err->code = YYJSON_READ_ERROR_##_code; \
         err->msg = _msg; \
@@ -5053,17 +5965,19 @@
     if (val_hdr) alc.free(alc.ctx, (void *)val_hdr); \
     return NULL; \
 } while (false)
     
 #define val_incr() do { \
     val++; \
     if (unlikely(val >= val_end)) { \
+        usize alc_old = alc_len; \
         alc_len += alc_len / 2; \
         if ((alc_len >= alc_max)) goto fail_alloc; \
         val_tmp = (yyjson_val *)alc.realloc(alc.ctx, (void *)val_hdr, \
+            alc_old * sizeof(yyjson_val), \
             alc_len * sizeof(yyjson_val)); \
         if ((!val_tmp)) goto fail_alloc; \
         val = val_tmp + (usize)(val - val_hdr); \
         ctn = val_tmp + (usize)(ctn - val_hdr); \
         val_hdr = val_tmp; \
         val_end = val_tmp + (alc_len - 2); \
     } \
@@ -5136,20 +6050,20 @@
     if (*cur == '\n') cur++;
     
 arr_val_begin:
 #if YYJSON_IS_REAL_GCC
     while (true) repeat16({
         if (byte_match_2(cur, "  ")) cur += 2;
         else break;
-    });
+    })
 #else
     while (true) repeat16({
         if (likely(byte_match_2(cur, "  "))) cur += 2;
         else break;
-    });
+    })
 #endif
     
     if (*cur == '{') {
         cur++;
         goto obj_begin;
     }
     if (*cur == '[') {
@@ -5189,14 +6103,15 @@
         }
         goto fail_literal;
     }
     if (*cur == ']') {
         cur++;
         if (likely(ctn_len == 0)) goto arr_end;
         if (has_flag(ALLOW_TRAILING_COMMAS)) goto arr_end;
+        while (*cur != ',') cur--;
         goto fail_trailing_comma;
     }
     if (char_is_space(*cur)) {
         while (char_is_space(*++cur));
         goto arr_val_begin;
     }
     if (unlikely(ext) && (*cur == 'i' || *cur == 'I' || *cur == 'N')) {
@@ -5266,31 +6181,32 @@
     if (*cur == '\n') cur++;
     
 obj_key_begin:
 #if YYJSON_IS_REAL_GCC
     while (true) repeat16({
         if (byte_match_2(cur, "  ")) cur += 2;
         else break;
-    });
+    })
 #else
     while (true) repeat16({
         if (likely(byte_match_2(cur, "  "))) cur += 2;
         else break;
-    });
+    })
 #endif
     if (likely(*cur == '"')) {
         val_incr();
         ctn_len++;
         if (likely(read_string(&cur, end, inv, val, &msg))) goto obj_key_end;
         goto fail_string;
     }
     if (likely(*cur == '}')) {
         cur++;
         if (likely(ctn_len == 0)) goto obj_end;
         if (has_flag(ALLOW_TRAILING_COMMAS)) goto obj_end;
+        while (*cur != ',') cur--;
         goto fail_trailing_comma;
     }
     if (char_is_space(*cur)) {
         while (char_is_space(*++cur));
         goto obj_key_begin;
     }
     if (has_flag(ALLOW_COMMENTS)) {
@@ -5414,15 +6330,18 @@
     } else {
         goto arr_val_end;
     }
     
 doc_end:
     /* check invalid contents after json document */
     if (unlikely(cur < end) && !has_flag(STOP_WHEN_DONE)) {
-        if (has_flag(ALLOW_COMMENTS)) skip_spaces_and_comments(&cur);
+        if (has_flag(ALLOW_COMMENTS)) {
+            skip_spaces_and_comments(&cur);
+            if (byte_match_2(cur, "/*")) goto fail_comment;
+        }
         else while (char_is_space(*cur)) cur++;
         if (unlikely(cur < end)) goto fail_garbage;
     }
     
     if (pre && *pre) **pre = '\0';
     doc = (yyjson_doc *)val_hdr;
     doc->root = val_hdr + hdr_len;
@@ -5637,15 +6556,15 @@
                 return_err(MEMORY_ALLOCATION, "fail to alloc memory");
             }
             buf_size += chunk_now;
             if (!buf) {
                 buf = alc.malloc(alc.ctx, buf_size);
                 if (!buf) return_err(MEMORY_ALLOCATION, "fail to alloc memory");
             } else {
-                tmp = alc.realloc(alc.ctx, buf, buf_size);
+                tmp = alc.realloc(alc.ctx, buf, buf_size - chunk_now, buf_size);
                 if (!tmp) return_err(MEMORY_ALLOCATION, "fail to alloc memory");
                 buf = tmp;
             }
             tmp = ((u8 *)buf) + buf_size - YYJSON_PADDING_SIZE - chunk_now;
             read_size = fread_safe(tmp, chunk_now, file);
             file_size += (long)read_size;
             if (read_size != chunk_now) break;
@@ -5667,14 +6586,92 @@
         alc.free(alc.ctx, buf);
         return NULL;
     }
     
 #undef return_err
 }
 
+const char *yyjson_read_number(const char *dat,
+                               yyjson_val *val,
+                               yyjson_read_flag flg,
+                               const yyjson_alc *alc,
+                               yyjson_read_err *err) {
+#define return_err(_pos, _code, _msg) do { \
+    err->pos = _pos > hdr ? (usize)(_pos - hdr) : 0; \
+    err->msg = _msg; \
+    err->code = YYJSON_READ_ERROR_##_code; \
+    return NULL; \
+} while (false)
+    
+    u8 *hdr = constcast(u8 *)dat, *cur = hdr;
+    bool raw; /* read number as raw */
+    bool ext; /* allow inf and nan */
+    u8 *raw_end; /* raw end for null-terminator */
+    u8 **pre; /* previous raw end pointer */
+    const char *msg;
+    yyjson_read_err dummy_err;
+    
+#if !YYJSON_HAS_IEEE_754 || YYJSON_DISABLE_FAST_FP_CONV
+    u8 buf[128];
+    usize dat_len;
+#endif
+    
+    if (!err) err = &dummy_err;
+    if (unlikely(!dat)) {
+        return_err(cur, INVALID_PARAMETER, "input data is NULL");
+    }
+    if (unlikely(!val)) {
+        return_err(cur, INVALID_PARAMETER, "output value is NULL");
+    }
+    
+#if !YYJSON_HAS_IEEE_754 || YYJSON_DISABLE_FAST_FP_CONV
+    if (!alc) alc = &YYJSON_DEFAULT_ALC;
+    dat_len = strlen(dat);
+    if (dat_len < sizeof(buf)) {
+        memcpy(buf, dat, dat_len + 1);
+        hdr = buf;
+        cur = hdr;
+    } else {
+        hdr = (u8 *)alc->malloc(alc->ctx, dat_len + 1);
+        cur = hdr;
+        if (unlikely(!hdr)) {
+            return_err(cur, MEMORY_ALLOCATION, "memory allocation failed");
+        }
+        memcpy(hdr, dat, dat_len + 1);
+    }
+#endif
+    
+#if YYJSON_DISABLE_NON_STANDARD
+    ext = false;
+#else
+    ext = (flg & YYJSON_READ_ALLOW_INF_AND_NAN) != 0;
+#endif
+    
+    raw = (flg & YYJSON_READ_NUMBER_AS_RAW) != 0;
+    raw_end = NULL;
+    pre = raw ? &raw_end : NULL;
+    
+#if !YYJSON_HAS_IEEE_754 || YYJSON_DISABLE_FAST_FP_CONV
+    if (!read_number(&cur, pre, ext, val, &msg)) {
+        if (dat_len >= sizeof(buf)) alc->free(alc->ctx, hdr);
+        return_err(cur, INVALID_NUMBER, msg);
+    }
+    if (dat_len >= sizeof(buf)) alc->free(alc->ctx, hdr);
+    if (raw) val->uni.str = dat;
+    return dat + (cur - hdr);
+#else
+    if (!read_number(&cur, pre, ext, val, &msg)) {
+        return_err(cur, INVALID_NUMBER, msg);
+    }
+    return (const char *)cur;
+#endif
+    
+#undef return_err
+}
+
 #endif /* YYJSON_DISABLE_READER */
 
 
 
 #if !YYJSON_DISABLE_WRITER
 
 /*==============================================================================
@@ -6016,16 +7013,16 @@
 }
 
 /**
  Convert double number from binary to decimal.
  The output significand is shortest decimal but may have trailing zeros.
  
  This function use the Schubfach algorithm:
- Raffaello Giulietti, The Schubfach way to render doubles (4th version), 2021.
- https://drive.google.com/file/d/1IEeATSVnEE6TkrHlCYNY2GjaraBjOT4f
+ Raffaello Giulietti, The Schubfach way to render doubles (5th version), 2022.
+ https://drive.google.com/file/d/1gp5xv4CAa78SVgCeWfGqqI4FfYYYuNFb
  https://mail.openjdk.java.net/pipermail/core-libs-dev/2021-November/083536.html
  https://github.com/openjdk/jdk/pull/3402 (Java implementation)
  https://github.com/abolz/Drachennest (C++ implementation)
  
  See also:
  Dragonbox: A New Floating-Point Binary-to-Decimal Conversion Algorithm, 2022.
  https://github.com/jk-jeon/dragonbox/blob/master/other_files/Dragonbox.pdf
@@ -6207,14 +7204,15 @@
                 dot_end = hdr + dot_pos + 2;
                 return dot_end < num_end ? num_end : dot_end;
             }
         } else {
             /* write with scientific notation */
             /* such as 1.234e56 */
             u8 *end = write_u64_len_15_to_17_trim(buf + 1, sig_dec);
+            end -= (end == buf + 2); /* remove '.0', e.g. 2.0e34 -> 2e34 */
             exp_dec += sig_len - 1;
             hdr[0] = hdr[1];
             hdr[1] = '.';
             end[0] = 'e';
             buf = write_f64_exp(exp_dec, end + 1);
             return buf;
         }
@@ -6258,15 +7256,15 @@
 /** Write a double number (requires 32 bytes buffer). */
 static_noinline u8 *write_f64_raw(u8 *buf, u64 raw, yyjson_write_flag flg) {
     /*
      For IEEE 754, `DBL_DECIMAL_DIG` is 17 for round-trip.
      For non-IEEE formats, 17 is used to avoid buffer overflow,
      round-trip is not guaranteed.
      */
-#if defined(DBL_DECIMAL_DIG)
+#if defined(DBL_DECIMAL_DIG) && DBL_DECIMAL_DIG != 17
     int dig = DBL_DECIMAL_DIG > 17 ? 17 : DBL_DECIMAL_DIG;
 #else
     int dig = 17;
 #endif
     
     /*
      The snprintf() function is locale-dependent. For currently known locales,
@@ -6301,19 +7299,22 @@
                 return buf + 3;
             }
         }
         return NULL;
     } else {
         /* finite number */
         int i = 0;
+        bool fp = false;
         for (; i < len; i++) {
-            if (buf[i] == ',') {
-                buf[i] = '.';
-                break;
-            }
+            if (buf[i] == ',') buf[i] = '.';
+            if (digi_is_fp((u8)buf[i])) fp = true;
+        }
+        if (!fp) {
+            buf[len++] = '.';
+            buf[len++] = '0';
         }
     }
     return buf + len;
 }
 
 #endif /* FP_WRITER */
 
@@ -6608,15 +7609,15 @@
  @param enc_table Encode type table for character.
  @return The buffer cursor after string, or NULL on invalid unicode.
  */
 static_inline u8 *write_string(u8 *cur, bool esc, bool inv,
                                const u8 *str, usize str_len,
                                const char_enc_type *enc_table) {
     
-    /* UTF-8 character mask and pattern, see `read_string` for details. */
+    /* UTF-8 character mask and pattern, see `read_string()` for details. */
 #if YYJSON_ENDIAN == YYJSON_BIG_ENDIAN
     const u16 b2_mask = 0xE0C0UL;
     const u16 b2_patt = 0xC080UL;
     const u16 b2_requ = 0x1E00UL;
     const u32 b3_mask = 0xF0C0C000UL;
     const u32 b3_patt = 0xE0808000UL;
     const u32 b3_requ = 0x0F200000UL;
@@ -6705,34 +7706,34 @@
     
 #define expr_stop(i) \
     stop_char_##i: \
     memcpy(cur, src, i); \
     cur += i; src += i; goto copy_utf8;
     
     while (end - src >= 16) {
-        repeat16_incr(expr_jump);
+        repeat16_incr(expr_jump)
         byte_copy_16(cur, src);
         cur += 16; src += 16;
     }
     
     while (end - src >= 4) {
-        repeat4_incr(expr_jump);
+        repeat4_incr(expr_jump)
         byte_copy_4(cur, src);
         cur += 4; src += 4;
     }
     
     while (end > src) {
-        expr_jump(0);
+        expr_jump(0)
         *cur++ = *src++;
     }
     
     *cur++ = '"';
     return cur;
     
-    repeat16_incr(expr_stop);
+    repeat16_incr(expr_stop)
     
 #undef expr_jump
 #undef expr_stop
     
 copy_utf8:
     if (unlikely(src + 4 > end)) {
         if (end == src) goto copy_end;
@@ -6896,19 +7897,20 @@
         byte_copy_8(cur, &v1);
     } else {
         byte_copy_8(cur, &v0);
     }
     return cur + 5 - val;
 }
 
-/** Write indent (requires level * 4 bytes buffer). */
-static_inline u8 *write_indent(u8 *cur, usize level) {
+/** Write indent (requires level x 4 bytes buffer).
+    Param spaces should not larger than 4. */
+static_inline u8 *write_indent(u8 *cur, usize level, usize spaces) {
     while (level-- > 0) {
         byte_copy_4(cur, "    ");
-        cur += 4;
+        cur += spaces;
     }
     return cur;
 }
 
 /** Write data to file. */
 static bool write_dat_to_file(const char *path, u8 *dat, usize len,
                               yyjson_write_err *err) {
@@ -7079,15 +8081,15 @@
 #define incr_len(_len) do { \
     ext_len = (usize)(_len); \
     if (unlikely((u8 *)(cur + ext_len) >= (u8 *)ctx)) { \
         alc_inc = yyjson_max(alc_len / 2, ext_len); \
         alc_inc = size_align_up(alc_inc, sizeof(yyjson_write_ctx)); \
         if (size_add_is_overflow(alc_len, alc_inc)) goto fail_alloc; \
         alc_len += alc_inc; \
-        tmp = (u8 *)alc.realloc(alc.ctx, hdr, alc_len); \
+        tmp = (u8 *)alc.realloc(alc.ctx, hdr, alc_len - alc_inc, alc_len); \
         if (unlikely(!tmp)) goto fail_alloc; \
         ctx_len = (usize)(end - (u8 *)ctx); \
         ctx_tmp = (yyjson_write_ctx *)(void *)(tmp + (alc_len - ctx_len)); \
         memmove((void *)ctx_tmp, (void *)(tmp + ((u8 *)ctx - hdr)), ctx_len); \
         ctx = ctx_tmp; \
         cur = tmp + (cur - hdr); \
         end = tmp + alc_len; \
@@ -7118,15 +8120,15 @@
     hdr = (u8 *)alc.malloc(alc.ctx, alc_len);
     if (!hdr) goto fail_alloc;
     cur = hdr;
     end = hdr + alc_len;
     ctx = (yyjson_write_ctx *)(void *)end;
     
 doc_begin:
-    val = (yyjson_val *)root;
+    val = constcast(yyjson_val *)root;
     val_type = unsafe_yyjson_get_type(val);
     ctn_obj = (val_type == YYJSON_TYPE_OBJ);
     ctn_len = unsafe_yyjson_get_len(val) << (u8)ctn_obj;
     *cur++ = (u8)('[' | ((u8)ctn_obj << 5));
     val++;
     
 val_begin:
@@ -7251,15 +8253,15 @@
 #define incr_len(_len) do { \
     ext_len = (usize)(_len); \
     if (unlikely((u8 *)(cur + ext_len) >= (u8 *)ctx)) { \
         alc_inc = yyjson_max(alc_len / 2, ext_len); \
         alc_inc = size_align_up(alc_inc, sizeof(yyjson_write_ctx)); \
         if (size_add_is_overflow(alc_len, alc_inc)) goto fail_alloc; \
         alc_len += alc_inc; \
-        tmp = (u8 *)alc.realloc(alc.ctx, hdr, alc_len); \
+        tmp = (u8 *)alc.realloc(alc.ctx, hdr, alc_len - alc_inc, alc_len); \
         if (unlikely(!tmp)) goto fail_alloc; \
         ctx_len = (usize)(end - (u8 *)ctx); \
         ctx_tmp = (yyjson_write_ctx *)(void *)(tmp + (alc_len - ctx_len)); \
         memmove((void *)ctx_tmp, (void *)(tmp + ((u8 *)ctx - hdr)), ctx_len); \
         ctx = ctx_tmp; \
         cur = tmp + (cur - hdr); \
         end = tmp + alc_len; \
@@ -7279,100 +8281,101 @@
     u8 *hdr, *cur, *end, *tmp;
     yyjson_write_ctx *ctx, *ctx_tmp;
     usize alc_len, alc_inc, ctx_len, ext_len, str_len, level;
     const u8 *str_ptr;
     const char_enc_type *enc_table = get_enc_table_with_flag(flg);
     bool esc = (flg & YYJSON_WRITE_ESCAPE_UNICODE) != 0;
     bool inv = (flg & YYJSON_WRITE_ALLOW_INVALID_UNICODE) != 0;
+    usize spaces = (flg & YYJSON_WRITE_PRETTY_TWO_SPACES) ? 2 : 4;
     
     alc_len = root->uni.ofs / sizeof(yyjson_val);
     alc_len = alc_len * YYJSON_WRITER_ESTIMATED_PRETTY_RATIO + 64;
     alc_len = size_align_up(alc_len, sizeof(yyjson_write_ctx));
     hdr = (u8 *)alc.malloc(alc.ctx, alc_len);
     if (!hdr) goto fail_alloc;
     cur = hdr;
     end = hdr + alc_len;
     ctx = (yyjson_write_ctx *)(void *)end;
     
 doc_begin:
-    val = (yyjson_val *)root;
+    val = constcast(yyjson_val *)root;
     val_type = unsafe_yyjson_get_type(val);
     ctn_obj = (val_type == YYJSON_TYPE_OBJ);
     ctn_len = unsafe_yyjson_get_len(val) << (u8)ctn_obj;
     *cur++ = (u8)('[' | ((u8)ctn_obj << 5));
     *cur++ = '\n';
     val++;
     level = 1;
     
 val_begin:
     val_type = unsafe_yyjson_get_type(val);
     if (val_type == YYJSON_TYPE_STR) {
-        is_key = ((u8)ctn_obj & (u8)~ctn_len);
-        no_indent = ((u8)ctn_obj & (u8)ctn_len);
+        is_key = (bool)((u8)ctn_obj & (u8)~ctn_len);
+        no_indent = (bool)((u8)ctn_obj & (u8)ctn_len);
         str_len = unsafe_yyjson_get_len(val);
         str_ptr = (const u8 *)unsafe_yyjson_get_str(val);
         check_str_len(str_len);
         incr_len(str_len * 6 + 16 + (no_indent ? 0 : level * 4));
-        cur = write_indent(cur, no_indent ? 0 : level);
+        cur = write_indent(cur, no_indent ? 0 : level, spaces);
         cur = write_string(cur, esc, inv, str_ptr, str_len, enc_table);
         if (unlikely(!cur)) goto fail_str;
         *cur++ = is_key ? ':' : ',';
         *cur++ = is_key ? ' ' : '\n';
         goto val_end;
     }
     if (val_type == YYJSON_TYPE_NUM) {
-        no_indent = ((u8)ctn_obj & (u8)ctn_len);
+        no_indent = (bool)((u8)ctn_obj & (u8)ctn_len);
         incr_len(32 + (no_indent ? 0 : level * 4));
-        cur = write_indent(cur, no_indent ? 0 : level);
+        cur = write_indent(cur, no_indent ? 0 : level, spaces);
         cur = write_number(cur, val, flg);
         if (unlikely(!cur)) goto fail_num;
         *cur++ = ',';
         *cur++ = '\n';
         goto val_end;
     }
     if ((val_type & (YYJSON_TYPE_ARR & YYJSON_TYPE_OBJ)) ==
                     (YYJSON_TYPE_ARR & YYJSON_TYPE_OBJ)) {
-        no_indent = ((u8)ctn_obj & (u8)ctn_len);
+        no_indent = (bool)((u8)ctn_obj & (u8)ctn_len);
         ctn_len_tmp = unsafe_yyjson_get_len(val);
         ctn_obj_tmp = (val_type == YYJSON_TYPE_OBJ);
         if (unlikely(ctn_len_tmp == 0)) {
             /* write empty container */
             incr_len(16 + (no_indent ? 0 : level * 4));
-            cur = write_indent(cur, no_indent ? 0 : level);
+            cur = write_indent(cur, no_indent ? 0 : level, spaces);
             *cur++ = (u8)('[' | ((u8)ctn_obj_tmp << 5));
             *cur++ = (u8)(']' | ((u8)ctn_obj_tmp << 5));
             *cur++ = ',';
             *cur++ = '\n';
             goto val_end;
         } else {
             /* push context, setup new container */
             incr_len(32 + (no_indent ? 0 : level * 4));
             yyjson_write_ctx_set(--ctx, ctn_len, ctn_obj);
             ctn_len = ctn_len_tmp << (u8)ctn_obj_tmp;
             ctn_obj = ctn_obj_tmp;
-            cur = write_indent(cur, no_indent ? 0 : level);
+            cur = write_indent(cur, no_indent ? 0 : level, spaces);
             level++;
             *cur++ = (u8)('[' | ((u8)ctn_obj << 5));
             *cur++ = '\n';
             val++;
             goto val_begin;
         }
     }
     if (val_type == YYJSON_TYPE_BOOL) {
-        no_indent = ((u8)ctn_obj & (u8)ctn_len);
+        no_indent = (bool)((u8)ctn_obj & (u8)ctn_len);
         incr_len(16 + (no_indent ? 0 : level * 4));
-        cur = write_indent(cur, no_indent ? 0 : level);
+        cur = write_indent(cur, no_indent ? 0 : level, spaces);
         cur = write_bool(cur, unsafe_yyjson_get_bool(val));
         cur += 2;
         goto val_end;
     }
     if (val_type == YYJSON_TYPE_NULL) {
-        no_indent = ((u8)ctn_obj & (u8)ctn_len);
+        no_indent = (bool)((u8)ctn_obj & (u8)ctn_len);
         incr_len(16 + (no_indent ? 0 : level * 4));
-        cur = write_indent(cur, no_indent ? 0 : level);
+        cur = write_indent(cur, no_indent ? 0 : level, spaces);
         cur = write_null(cur);
         cur += 2;
         goto val_end;
     }
     if (val_type == YYJSON_TYPE_RAW) {
         str_len = unsafe_yyjson_get_len(val);
         str_ptr = (const u8 *)unsafe_yyjson_get_str(val);
@@ -7391,15 +8394,15 @@
     if (unlikely(ctn_len == 0)) goto ctn_end;
     goto val_begin;
     
 ctn_end:
     cur -= 2;
     *cur++ = '\n';
     incr_len(level * 4);
-    cur = write_indent(cur, --level);
+    cur = write_indent(cur, --level, spaces);
     *cur++ = (u8)(']' | ((u8)ctn_obj << 5));
     if (unlikely((u8 *)ctx >= end)) goto doc_end;
     yyjson_write_ctx_get(ctx++, &ctn_len, &ctn_obj);
     ctn_len--;
     *cur++ = ',';
     *cur++ = '\n';
     if (likely(ctn_len > 0)) {
@@ -7432,15 +8435,15 @@
                             yyjson_write_flag flg,
                             const yyjson_alc *alc_ptr,
                             usize *dat_len,
                             yyjson_write_err *err) {
     yyjson_write_err dummy_err;
     usize dummy_dat_len;
     yyjson_alc alc = alc_ptr ? *alc_ptr : YYJSON_DEFAULT_ALC;
-    yyjson_val *root = (yyjson_val *)val;
+    yyjson_val *root = constcast(yyjson_val *)val;
     
     err = err ? err : &dummy_err;
     dat_len = dat_len ? dat_len : &dummy_dat_len;
     
 #if YYJSON_DISABLE_NON_STANDARD
     flg &= ~YYJSON_WRITE_ALLOW_INF_AND_NAN;
     flg &= ~YYJSON_WRITE_ALLOW_INVALID_UNICODE;
@@ -7451,15 +8454,15 @@
         err->msg = "input JSON is NULL";
         err->code = YYJSON_READ_ERROR_INVALID_PARAMETER;
         return NULL;
     }
     
     if (!unsafe_yyjson_is_ctn(root) || unsafe_yyjson_get_len(root) == 0) {
         return (char *)yyjson_write_single(root, flg, alc, dat_len, err);
-    } else if (flg & YYJSON_WRITE_PRETTY) {
+    } else if (flg & (YYJSON_WRITE_PRETTY | YYJSON_WRITE_PRETTY_TWO_SPACES)) {
         return (char *)yyjson_write_pretty(root, flg, alc, dat_len, err);
     } else {
         return (char *)yyjson_write_minify(root, flg, alc, dat_len, err);
     }
 }
 
 char *yyjson_write_opts(const yyjson_doc *doc,
@@ -7475,15 +8478,15 @@
                            const yyjson_val *val,
                            yyjson_write_flag flg,
                            const yyjson_alc *alc_ptr,
                            yyjson_write_err *err) {
     yyjson_write_err dummy_err;
     u8 *dat;
     usize dat_len = 0;
-    yyjson_val *root = (yyjson_val *)val;
+    yyjson_val *root = constcast(yyjson_val *)val;
     bool suc;
     
     alc_ptr = alc_ptr ? alc_ptr : &YYJSON_DEFAULT_ALC;
     err = err ? err : &dummy_err;
     if (unlikely(!path || !*path)) {
         err->msg = "input path is invalid";
         err->code = YYJSON_READ_ERROR_INVALID_PARAMETER;
@@ -7529,26 +8532,42 @@
                                             usize *size, bool *is_obj) {
     usize tag = ctx->tag;
     *size = tag >> 1;
     *is_obj = (bool)(tag & 1);
     *ctn = ctx->ctn;
 }
 
+/** Get the estimated number of values for the mutable JSON document. */
+static_inline usize yyjson_mut_doc_estimated_val_num(
+    const yyjson_mut_doc *doc) {
+    usize sum = 0;
+    yyjson_val_chunk *chunk = doc->val_pool.chunks;
+    while (chunk) {
+        sum += chunk->chunk_size / sizeof(yyjson_mut_val) - 1;
+        if (chunk == doc->val_pool.chunks) {
+            sum -= (usize)(doc->val_pool.end - doc->val_pool.cur);
+        }
+        chunk = chunk->next;
+    }
+    return sum;
+}
+
 /** Write single JSON value. */
 static_inline u8 *yyjson_mut_write_single(yyjson_mut_val *val,
                                           yyjson_write_flag flg,
                                           yyjson_alc alc,
                                           usize *dat_len,
                                           yyjson_write_err *err) {
     return yyjson_write_single((yyjson_val *)val, flg, alc, dat_len, err);
 }
 
 /** Write JSON document minify.
     The root of this document should be a non-empty container. */
 static_inline u8 *yyjson_mut_write_minify(const yyjson_mut_val *root,
+                                          usize estimated_val_num,
                                           yyjson_write_flag flg,
                                           yyjson_alc alc,
                                           usize *dat_len,
                                           yyjson_write_err *err) {
     
 #define return_err(_code, _msg) do { \
     *dat_len = 0; \
@@ -7561,15 +8580,15 @@
 #define incr_len(_len) do { \
     ext_len = (usize)(_len); \
     if (unlikely((u8 *)(cur + ext_len) >= (u8 *)ctx)) { \
         alc_inc = yyjson_max(alc_len / 2, ext_len); \
         alc_inc = size_align_up(alc_inc, sizeof(yyjson_mut_write_ctx)); \
         if (size_add_is_overflow(alc_len, alc_inc)) goto fail_alloc; \
         alc_len += alc_inc; \
-        tmp = (u8 *)alc.realloc(alc.ctx, hdr, alc_len); \
+        tmp = (u8 *)alc.realloc(alc.ctx, hdr, alc_len - alc_inc, alc_len); \
         if (unlikely(!tmp)) goto fail_alloc; \
         ctx_len = (usize)(end - (u8 *)ctx); \
         ctx_tmp = (yyjson_mut_write_ctx *)(void *)(tmp + (alc_len - ctx_len)); \
         memmove((void *)ctx_tmp, (void *)(tmp + ((u8 *)ctx - hdr)), ctx_len); \
         ctx = ctx_tmp; \
         cur = tmp + (cur - hdr); \
         end = tmp + alc_len; \
@@ -7590,24 +8609,24 @@
     yyjson_mut_write_ctx *ctx, *ctx_tmp;
     usize alc_len, alc_inc, ctx_len, ext_len, str_len;
     const u8 *str_ptr;
     const char_enc_type *enc_table = get_enc_table_with_flag(flg);
     bool esc = (flg & YYJSON_WRITE_ESCAPE_UNICODE) != 0;
     bool inv = (flg & YYJSON_WRITE_ALLOW_INVALID_UNICODE) != 0;
     
-    alc_len = 0 * YYJSON_WRITER_ESTIMATED_MINIFY_RATIO + 64;
+    alc_len = estimated_val_num * YYJSON_WRITER_ESTIMATED_MINIFY_RATIO + 64;
     alc_len = size_align_up(alc_len, sizeof(yyjson_mut_write_ctx));
     hdr = (u8 *)alc.malloc(alc.ctx, alc_len);
     if (!hdr) goto fail_alloc;
     cur = hdr;
     end = hdr + alc_len;
     ctx = (yyjson_mut_write_ctx *)(void *)end;
     
 doc_begin:
-    val = (yyjson_mut_val *)root;
+    val = constcast(yyjson_mut_val *)root;
     val_type = unsafe_yyjson_get_type(val);
     ctn_obj = (val_type == YYJSON_TYPE_OBJ);
     ctn_len = unsafe_yyjson_get_len(val) << (u8)ctn_obj;
     *cur++ = (u8)('[' | ((u8)ctn_obj << 5));
     ctn = val;
     val = (yyjson_mut_val *)val->uni.ptr; /* tail */
     val = ctn_obj ? val->next->next : val->next;
@@ -7718,14 +8737,15 @@
 #undef incr_len
 #undef check_str_len
 }
 
 /** Write JSON document pretty.
     The root of this document should be a non-empty container. */
 static_inline u8 *yyjson_mut_write_pretty(const yyjson_mut_val *root,
+                                          usize estimated_val_num,
                                           yyjson_write_flag flg,
                                           yyjson_alc alc,
                                           usize *dat_len,
                                           yyjson_write_err *err) {
     
 #define return_err(_code, _msg) do { \
     *dat_len = 0; \
@@ -7738,15 +8758,15 @@
 #define incr_len(_len) do { \
     ext_len = (usize)(_len); \
     if (unlikely((u8 *)(cur + ext_len) >= (u8 *)ctx)) { \
         alc_inc = yyjson_max(alc_len / 2, ext_len); \
         alc_inc = size_align_up(alc_inc, sizeof(yyjson_mut_write_ctx)); \
         if (size_add_is_overflow(alc_len, alc_inc)) goto fail_alloc; \
         alc_len += alc_inc; \
-        tmp = (u8 *)alc.realloc(alc.ctx, hdr, alc_len); \
+        tmp = (u8 *)alc.realloc(alc.ctx, hdr, alc_len - alc_inc, alc_len); \
         if (unlikely(!tmp)) goto fail_alloc; \
         ctx_len = (usize)(end - (u8 *)ctx); \
         ctx_tmp = (yyjson_mut_write_ctx *)(void *)(tmp + (alc_len - ctx_len)); \
         memmove((void *)ctx_tmp, (void *)(tmp + ((u8 *)ctx - hdr)), ctx_len); \
         ctx = ctx_tmp; \
         cur = tmp + (cur - hdr); \
         end = tmp + alc_len; \
@@ -7766,103 +8786,104 @@
     u8 *hdr, *cur, *end, *tmp;
     yyjson_mut_write_ctx *ctx, *ctx_tmp;
     usize alc_len, alc_inc, ctx_len, ext_len, str_len, level;
     const u8 *str_ptr;
     const char_enc_type *enc_table = get_enc_table_with_flag(flg);
     bool esc = (flg & YYJSON_WRITE_ESCAPE_UNICODE) != 0;
     bool inv = (flg & YYJSON_WRITE_ALLOW_INVALID_UNICODE) != 0;
+    usize spaces = (flg & YYJSON_WRITE_PRETTY_TWO_SPACES) ? 2 : 4;
     
-    alc_len = 0 * YYJSON_WRITER_ESTIMATED_PRETTY_RATIO + 64;
+    alc_len = estimated_val_num * YYJSON_WRITER_ESTIMATED_PRETTY_RATIO + 64;
     alc_len = size_align_up(alc_len, sizeof(yyjson_mut_write_ctx));
     hdr = (u8 *)alc.malloc(alc.ctx, alc_len);
     if (!hdr) goto fail_alloc;
     cur = hdr;
     end = hdr + alc_len;
     ctx = (yyjson_mut_write_ctx *)(void *)end;
     
 doc_begin:
-    val = (yyjson_mut_val *)root;
+    val = constcast(yyjson_mut_val *)root;
     val_type = unsafe_yyjson_get_type(val);
     ctn_obj = (val_type == YYJSON_TYPE_OBJ);
     ctn_len = unsafe_yyjson_get_len(val) << (u8)ctn_obj;
     *cur++ = (u8)('[' | ((u8)ctn_obj << 5));
     *cur++ = '\n';
     ctn = val;
     val = (yyjson_mut_val *)val->uni.ptr; /* tail */
     val = ctn_obj ? val->next->next : val->next;
     level = 1;
     
 val_begin:
     val_type = unsafe_yyjson_get_type(val);
     if (val_type == YYJSON_TYPE_STR) {
-        is_key = ((u8)ctn_obj & (u8)~ctn_len);
-        no_indent = ((u8)ctn_obj & (u8)ctn_len);
+        is_key = (bool)((u8)ctn_obj & (u8)~ctn_len);
+        no_indent = (bool)((u8)ctn_obj & (u8)ctn_len);
         str_len = unsafe_yyjson_get_len(val);
         str_ptr = (const u8 *)unsafe_yyjson_get_str(val);
         check_str_len(str_len);
         incr_len(str_len * 6 + 16 + (no_indent ? 0 : level * 4));
-        cur = write_indent(cur, no_indent ? 0 : level);
+        cur = write_indent(cur, no_indent ? 0 : level, spaces);
         cur = write_string(cur, esc, inv, str_ptr, str_len, enc_table);
         if (unlikely(!cur)) goto fail_str;
         *cur++ = is_key ? ':' : ',';
         *cur++ = is_key ? ' ' : '\n';
         goto val_end;
     }
     if (val_type == YYJSON_TYPE_NUM) {
-        no_indent = ((u8)ctn_obj & (u8)ctn_len);
+        no_indent = (bool)((u8)ctn_obj & (u8)ctn_len);
         incr_len(32 + (no_indent ? 0 : level * 4));
-        cur = write_indent(cur, no_indent ? 0 : level);
+        cur = write_indent(cur, no_indent ? 0 : level, spaces);
         cur = write_number(cur, (yyjson_val *)val, flg);
         if (unlikely(!cur)) goto fail_num;
         *cur++ = ',';
         *cur++ = '\n';
         goto val_end;
     }
     if ((val_type & (YYJSON_TYPE_ARR & YYJSON_TYPE_OBJ)) ==
                     (YYJSON_TYPE_ARR & YYJSON_TYPE_OBJ)) {
-        no_indent = ((u8)ctn_obj & (u8)ctn_len);
+        no_indent = (bool)((u8)ctn_obj & (u8)ctn_len);
         ctn_len_tmp = unsafe_yyjson_get_len(val);
         ctn_obj_tmp = (val_type == YYJSON_TYPE_OBJ);
         if (unlikely(ctn_len_tmp == 0)) {
             /* write empty container */
             incr_len(16 + (no_indent ? 0 : level * 4));
-            cur = write_indent(cur, no_indent ? 0 : level);
+            cur = write_indent(cur, no_indent ? 0 : level, spaces);
             *cur++ = (u8)('[' | ((u8)ctn_obj_tmp << 5));
             *cur++ = (u8)(']' | ((u8)ctn_obj_tmp << 5));
             *cur++ = ',';
             *cur++ = '\n';
             goto val_end;
         } else {
             /* push context, setup new container */
             incr_len(32 + (no_indent ? 0 : level * 4));
             yyjson_mut_write_ctx_set(--ctx, ctn, ctn_len, ctn_obj);
             ctn_len = ctn_len_tmp << (u8)ctn_obj_tmp;
             ctn_obj = ctn_obj_tmp;
-            cur = write_indent(cur, no_indent ? 0 : level);
+            cur = write_indent(cur, no_indent ? 0 : level, spaces);
             level++;
             *cur++ = (u8)('[' | ((u8)ctn_obj << 5));
             *cur++ = '\n';
             ctn = val;
             val = (yyjson_mut_val *)ctn->uni.ptr; /* tail */
             val = ctn_obj ? val->next->next : val->next;
             goto val_begin;
         }
     }
     if (val_type == YYJSON_TYPE_BOOL) {
-        no_indent = ((u8)ctn_obj & (u8)ctn_len);
+        no_indent = (bool)((u8)ctn_obj & (u8)ctn_len);
         incr_len(16 + (no_indent ? 0 : level * 4));
-        cur = write_indent(cur, no_indent ? 0 : level);
+        cur = write_indent(cur, no_indent ? 0 : level, spaces);
         cur = write_bool(cur, unsafe_yyjson_get_bool(val));
         cur += 2;
         goto val_end;
     }
     if (val_type == YYJSON_TYPE_NULL) {
-        no_indent = ((u8)ctn_obj & (u8)ctn_len);
+        no_indent = (bool)((u8)ctn_obj & (u8)ctn_len);
         incr_len(16 + (no_indent ? 0 : level * 4));
-        cur = write_indent(cur, no_indent ? 0 : level);
+        cur = write_indent(cur, no_indent ? 0 : level, spaces);
         cur = write_null(cur);
         cur += 2;
         goto val_end;
     }
     if (val_type == YYJSON_TYPE_RAW) {
         str_len = unsafe_yyjson_get_len(val);
         str_ptr = (const u8 *)unsafe_yyjson_get_str(val);
@@ -7881,15 +8902,15 @@
     val = val->next;
     goto val_begin;
     
 ctn_end:
     cur -= 2;
     *cur++ = '\n';
     incr_len(level * 4);
-    cur = write_indent(cur, --level);
+    cur = write_indent(cur, --level, spaces);
     *cur++ = (u8)(']' | ((u8)ctn_obj << 5));
     if (unlikely((u8 *)ctx >= end)) goto doc_end;
     val = ctn->next;
     yyjson_mut_write_ctx_get(ctx++, &ctn, &ctn_len, &ctn_obj);
     ctn_len--;
     *cur++ = ',';
     *cur++ = '\n';
@@ -7916,23 +8937,24 @@
     return_err(INVALID_STRING, "invalid utf-8 encoding in string");
     
 #undef return_err
 #undef incr_len
 #undef check_str_len
 }
 
-char *yyjson_mut_val_write_opts(const yyjson_mut_val *val,
-                                yyjson_write_flag flg,
-                                const yyjson_alc *alc_ptr,
-                                usize *dat_len,
-                                yyjson_write_err *err) {
+static char *yyjson_mut_write_opts_impl(const yyjson_mut_val *val,
+                                        usize estimated_val_num,
+                                        yyjson_write_flag flg,
+                                        const yyjson_alc *alc_ptr,
+                                        usize *dat_len,
+                                        yyjson_write_err *err) {
     yyjson_write_err dummy_err;
     usize dummy_dat_len;
     yyjson_alc alc = alc_ptr ? *alc_ptr : YYJSON_DEFAULT_ALC;
-    yyjson_mut_val *root = (yyjson_mut_val *)val;
+    yyjson_mut_val *root = constcast(yyjson_mut_val *)val;
     
     err = err ? err : &dummy_err;
     dat_len = dat_len ? dat_len : &dummy_dat_len;
     
 #if YYJSON_DISABLE_NON_STANDARD
     flg &= ~YYJSON_WRITE_ALLOW_INF_AND_NAN;
     flg &= ~YYJSON_WRITE_ALLOW_INVALID_UNICODE;
@@ -7943,39 +8965,58 @@
         err->msg = "input JSON is NULL";
         err->code = YYJSON_WRITE_ERROR_INVALID_PARAMETER;
         return NULL;
     }
     
     if (!unsafe_yyjson_is_ctn(root) || unsafe_yyjson_get_len(root) == 0) {
         return (char *)yyjson_mut_write_single(root, flg, alc, dat_len, err);
-    } else if (flg & YYJSON_WRITE_PRETTY) {
-        return (char *)yyjson_mut_write_pretty(root, flg, alc, dat_len, err);
+    } else if (flg & (YYJSON_WRITE_PRETTY | YYJSON_WRITE_PRETTY_TWO_SPACES)) {
+        return (char *)yyjson_mut_write_pretty(root, estimated_val_num,
+                                               flg, alc, dat_len, err);
     } else {
-        return (char *)yyjson_mut_write_minify(root, flg, alc, dat_len, err);
+        return (char *)yyjson_mut_write_minify(root, estimated_val_num,
+                                               flg, alc, dat_len, err);
     }
 }
 
+char *yyjson_mut_val_write_opts(const yyjson_mut_val *val,
+                                yyjson_write_flag flg,
+                                const yyjson_alc *alc_ptr,
+                                usize *dat_len,
+                                yyjson_write_err *err) {
+    return yyjson_mut_write_opts_impl(val, 0, flg, alc_ptr, dat_len, err);
+}
+
 char *yyjson_mut_write_opts(const yyjson_mut_doc *doc,
                             yyjson_write_flag flg,
                             const yyjson_alc *alc_ptr,
                             usize *dat_len,
                             yyjson_write_err *err) {
-    yyjson_mut_val *root = doc ? doc->root : NULL;
-    return yyjson_mut_val_write_opts(root, flg, alc_ptr, dat_len, err);
+    yyjson_mut_val *root;
+    usize estimated_val_num;
+    if (likely(doc)) {
+        root = doc->root;
+        estimated_val_num = yyjson_mut_doc_estimated_val_num(doc);
+    } else {
+        root = NULL;
+        estimated_val_num = 0;
+    }
+    return yyjson_mut_write_opts_impl(root, estimated_val_num,
+                                      flg, alc_ptr, dat_len, err);
 }
 
 bool yyjson_mut_val_write_file(const char *path,
                                const yyjson_mut_val *val,
                                yyjson_write_flag flg,
                                const yyjson_alc *alc_ptr,
                                yyjson_write_err *err) {
     yyjson_write_err dummy_err;
     u8 *dat;
     usize dat_len = 0;
-    yyjson_mut_val *root = (yyjson_mut_val *)val;
+    yyjson_mut_val *root = constcast(yyjson_mut_val *)val;
     bool suc;
     
     alc_ptr = alc_ptr ? alc_ptr : &YYJSON_DEFAULT_ALC;
     err = err ? err : &dummy_err;
     if (unlikely(!path || !*path)) {
         err->msg = "input path is invalid";
         err->code = YYJSON_WRITE_ERROR_INVALID_PARAMETER;
```

### Comparing `yyjson-1.0.1/yyjson/yyjson.h` & `yyjson-2.0.2/yyjson/yyjson.h`

 * *Files 17% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 /*
  Define as 1 to disable JSON reader if you don't need to parse JSON.
  
  This will disable these functions at compile-time:
     - yyjson_read_opts()
     - yyjson_read_file()
     - yyjson_read()
+    - yyjson_read_number()
+    - yyjson_mut_read_number()
  
  This will reduce the binary size by about 60%.
  */
 #ifndef YYJSON_DISABLE_READER
 #endif
 
 /*
@@ -61,50 +63,67 @@
  
  This will reduce the binary size by about 30%.
  */
 #ifndef YYJSON_DISABLE_WRITER
 #endif
 
 /*
+ Define as 1 to disable JSON Pointer, JSON Patch and JSON Merge Patch supports.
+ 
+ This will disable these functions at compile-time:
+    - yyjson_ptr_xxx()
+    - yyjson_mut_ptr_xxx()
+    - yyjson_doc_ptr_xxx()
+    - yyjson_mut_doc_ptr_xxx()
+    - yyjson_patch()
+    - yyjson_mut_patch()
+    - yyjson_merge_patch()
+    - yyjson_mut_merge_patch()
+ */
+#ifndef YYJSON_DISABLE_UTILS
+#endif
+
+/*
  Define as 1 to disable the fast floating-point number conversion in yyjson,
  and use libc's `strtod/snprintf` instead.
  
- This will reduce binary size by about 30%, but significantly slow down
- floating-point reading and writing speed.
+ This will reduce the binary size by about 30%, but significantly slow down the
+ floating-point read/write speed.
  */
 #ifndef YYJSON_DISABLE_FAST_FP_CONV
 #endif
 
 /*
  Define as 1 to disable non-standard JSON support at compile-time:
-    - Reading and writing inf/nan literal, such as 'NaN', '-Infinity'.
+    - Reading and writing inf/nan literal, such as `NaN`, `-Infinity`.
     - Single line and multiple line comments.
     - Single trailing comma at the end of an object or array.
     - Invalid unicode in string value.
  
  This will also invalidate these run-time options:
     - YYJSON_READ_ALLOW_INF_AND_NAN
     - YYJSON_READ_ALLOW_COMMENTS
     - YYJSON_READ_ALLOW_TRAILING_COMMAS
     - YYJSON_READ_ALLOW_INVALID_UNICODE
     - YYJSON_WRITE_ALLOW_INF_AND_NAN
     - YYJSON_WRITE_ALLOW_INVALID_UNICODE
  
- This will reduce binary size by about 10%, and increase performance slightly.
+ This will reduce the binary size by about 10%, and slightly improve the JSON
+ read/write speed.
  */
 #ifndef YYJSON_DISABLE_NON_STANDARD
 #endif
 
 /*
  Define as 1 to disable unaligned memory access if target architecture does not
  support unaligned memory access (such as some embedded processors).
  
  If this value is not defined, yyjson will perform some automatic detection.
  The wrong definition of this option may cause some performance degradation,
- but will not cause run-time errors.
+ but will not cause any run-time errors.
  */
 #ifndef YYJSON_DISABLE_UNALIGNED_MEMORY_ACCESS
 #endif
 
 /* Define as 1 to export symbols when building this library as Windows DLL. */
 #ifndef YYJSON_EXPORTS
 #endif
@@ -169,14 +188,23 @@
 #   ifdef __has_attribute
 #       define yyjson_has_attribute(x) __has_attribute(x)
 #   else
 #       define yyjson_has_attribute(x) 0
 #   endif
 #endif
 
+/** compiler feature check (since clang 2.6, icc 17) */
+#ifndef yyjson_has_feature
+#   ifdef __has_feature
+#       define yyjson_has_feature(x) __has_feature(x)
+#   else
+#       define yyjson_has_feature(x) 0
+#   endif
+#endif
+
 /** include check (since gcc 5.0, clang 2.7, icc 16, msvc 2017 15.3) */
 #ifndef yyjson_has_include
 #   ifdef __has_include
 #       define yyjson_has_include(x) __has_include(x)
 #   else
 #       define yyjson_has_include(x) 0
 #   endif
@@ -221,30 +249,46 @@
 #   else
 #       define yyjson_align(x)
 #   endif
 #endif
 
 /** likely for compiler */
 #ifndef yyjson_likely
-#   if yyjson_has_builtin(__builtin_expect) || YYJSON_GCC_VER >= 4
+#   if yyjson_has_builtin(__builtin_expect) || \
+    (YYJSON_GCC_VER >= 4 && YYJSON_GCC_VER != 5)
 #       define yyjson_likely(expr) __builtin_expect(!!(expr), 1)
 #   else
 #       define yyjson_likely(expr) (expr)
 #   endif
 #endif
 
 /** unlikely for compiler */
 #ifndef yyjson_unlikely
-#   if yyjson_has_builtin(__builtin_expect) || YYJSON_GCC_VER >= 4
+#   if yyjson_has_builtin(__builtin_expect) || \
+    (YYJSON_GCC_VER >= 4 && YYJSON_GCC_VER != 5)
 #       define yyjson_unlikely(expr) __builtin_expect(!!(expr), 0)
 #   else
 #       define yyjson_unlikely(expr) (expr)
 #   endif
 #endif
 
+/** deprecate warning */
+#ifndef yyjson_deprecated
+#   if YYJSON_MSC_VER >= 1400
+#       define yyjson_deprecated(msg) __declspec(deprecated(msg))
+#   elif yyjson_has_feature(attribute_deprecated_with_message) || \
+        (YYJSON_GCC_VER > 4 || (YYJSON_GCC_VER == 4 && __GNUC_MINOR__ >= 5))
+#       define yyjson_deprecated(msg) __attribute__((deprecated(msg)))
+#   elif YYJSON_GCC_VER >= 3
+#       define yyjson_deprecated(msg) __attribute__((deprecated))
+#   else
+#       define yyjson_deprecated(msg)
+#   endif
+#endif
+
 /** function export */
 #ifndef yyjson_api
 #   if defined(_WIN32)
 #       if defined(YYJSON_EXPORTS) && YYJSON_EXPORTS
 #           define yyjson_api __declspec(dllexport)
 #       elif defined(YYJSON_IMPORTS) && YYJSON_IMPORTS
 #           define yyjson_api __declspec(dllimport)
@@ -365,14 +409,26 @@
 /** char bit check */
 #if defined(CHAR_BIT)
 #   if CHAR_BIT != 8
 #       error non 8-bit char is not supported
 #   endif
 #endif
 
+/**
+ Microsoft Visual C++ 6.0 doesn't support converting number from u64 to f64:
+ error C2520: conversion from unsigned __int64 to double not implemented.
+ */
+#ifndef YYJSON_U64_TO_F64_NO_IMPL
+#   if (0 < YYJSON_MSC_VER) && (YYJSON_MSC_VER <= 1200)
+#       define YYJSON_U64_TO_F64_NO_IMPL 1
+#   else
+#       define YYJSON_U64_TO_F64_NO_IMPL 0
+#   endif
+#endif
+
 
 
 /*==============================================================================
  * Compile Hint Begin
  *============================================================================*/
 
 /* extern "C" begin */
@@ -402,24 +458,24 @@
  * Version
  *============================================================================*/
 
 /** The major version of yyjson. */
 #define YYJSON_VERSION_MAJOR  0
 
 /** The minor version of yyjson. */
-#define YYJSON_VERSION_MINOR  5
+#define YYJSON_VERSION_MINOR  6
 
 /** The patch version of yyjson. */
 #define YYJSON_VERSION_PATCH  0
 
-/** The version of yyjson in hex: (major << 16) | (minor << 8) | (patch). */
-#define YYJSON_VERSION_HEX    0x000500
+/** The version of yyjson in hex: `(major << 16) | (minor << 8) | (patch)`. */
+#define YYJSON_VERSION_HEX    0x000600
 
 /** The version string of yyjson. */
-#define YYJSON_VERSION_STRING "0.5.0"
+#define YYJSON_VERSION_STRING "0.6.0"
 
 /** The version of yyjson in hex, same as `YYJSON_VERSION_HEX`. */
 yyjson_api uint32_t yyjson_version(void);
 
 
 
 /*==============================================================================
@@ -442,15 +498,15 @@
 #define YYJSON_SUBTYPE_NONE     ((uint8_t)(0 << 3)) /* ___00___ */
 #define YYJSON_SUBTYPE_FALSE    ((uint8_t)(0 << 3)) /* ___00___ */
 #define YYJSON_SUBTYPE_TRUE     ((uint8_t)(1 << 3)) /* ___01___ */
 #define YYJSON_SUBTYPE_UINT     ((uint8_t)(0 << 3)) /* ___00___ */
 #define YYJSON_SUBTYPE_SINT     ((uint8_t)(1 << 3)) /* ___01___ */
 #define YYJSON_SUBTYPE_REAL     ((uint8_t)(2 << 3)) /* ___10___ */
 
-/** Mask and bits of JSON value. */
+/** Mask and bits of JSON value tag. */
 #define YYJSON_TYPE_MASK        ((uint8_t)0x07)     /* _____111 */
 #define YYJSON_TYPE_BIT         ((uint8_t)3)
 #define YYJSON_SUBTYPE_MASK     ((uint8_t)0x18)     /* ___11___ */
 #define YYJSON_SUBTYPE_BIT      ((uint8_t)2)
 #define YYJSON_RESERVED_MASK    ((uint8_t)0xE0)     /* 111_____ */
 #define YYJSON_RESERVED_BIT     ((uint8_t)3)
 #define YYJSON_TAG_MASK         ((uint8_t)0xFF)     /* 11111111 */
@@ -468,38 +524,38 @@
 /**
  A memory allocator.
  
  Typically you don't need to use it, unless you want to customize your own
  memory allocator.
  */
 typedef struct yyjson_alc {
-    /** Same as libc's malloc(), should not be NULL. */
+    /** Same as libc's malloc(size), should not be NULL. */
     void *(*malloc)(void *ctx, size_t size);
-    /** Same as libc's realloc(), should not be NULL. */
-    void *(*realloc)(void *ctx, void *ptr, size_t size);
-    /** Same as libc's free(), should not be NULL. */
+    /** Same as libc's realloc(ptr, size), should not be NULL. */
+    void *(*realloc)(void *ctx, void *ptr, size_t old_size, size_t size);
+    /** Same as libc's free(ptr), should not be NULL. */
     void (*free)(void *ctx, void *ptr);
     /** A context for malloc/realloc/free, can be NULL. */
     void *ctx;
 } yyjson_alc;
 
 /**
  A pool allocator uses fixed length pre-allocated memory.
  
- This allocator may used to avoid malloc()/memmove() calls. The pre-allocated
- memory should be held by the caller. The upper limit of memory required to
- read JSON can be calculated using the yyjson_read_max_memory_usage() function,
- but the memory required to write JSON cannot be calculated directly.
+ This allocator may used to avoid malloc/realloc calls. The pre-allocated memory
+ should be held by the caller. The maximum amount of memory required to read a
+ JSON can be calculated using the `yyjson_read_max_memory_usage()` function, but
+ the amount of memory required to write a JSON cannot be directly calculated.
  
  This is not a general-purpose allocator, and should only be used to read or
  write single JSON document.
  
  @param alc The allocator to be initialized.
     If this parameter is NULL, the function will fail and return false.
-    If `buf` or `size` is invalid, this parameter is left unmodified.
+    If `buf` or `size` is invalid, this will be set to an empty allocator.
  @param buf The buffer memory for this allocator.
     If this parameter is NULL, the function will fail and return false.
  @param size The size of `buf`, in bytes.
     If this parameter is less than 8 words (32/64 bytes on 32/64-bit OS), the
     function will fail and return false.
  @return true if the `alc` has been successfully initialized.
  
@@ -522,29 +578,29 @@
 /*==============================================================================
  * JSON Structure
  *============================================================================*/
 
 /**
  An immutable document for reading JSON.
  This document holds memory for all its JSON values and strings. When it is no
- longer used, the user should call yyjson_doc_free() to free its memory.
+ longer used, the user should call `yyjson_doc_free()` to free its memory.
  */
 typedef struct yyjson_doc yyjson_doc;
 
 /**
  An immutable value for reading JSON.
  A JSON Value has the same lifetime as its document. The memory is held by its
  document and and cannot be freed alone.
  */
 typedef struct yyjson_val yyjson_val;
 
 /**
  A mutable document for building JSON.
  This document holds memory for all its JSON values and strings. When it is no
- longer used, the user should call yyjson_mut_doc_free() to free its memory.
+ longer used, the user should call `yyjson_mut_doc_free()` to free its memory.
  */
 typedef struct yyjson_mut_doc yyjson_mut_doc;
 
 /**
  A mutable value for building JSON.
  A JSON Value has the same lifetime as its document. The memory is held by its
  document and and cannot be freed alone.
@@ -571,34 +627,34 @@
 static const yyjson_read_flag YYJSON_READ_NOFLAG                = 0 << 0;
 
 /** Read the input data in-situ.
     This option allows the reader to modify and use input data to store string
     values, which can increase reading speed slightly.
     The caller should hold the input data before free the document.
     The input data must be padded by at least `YYJSON_PADDING_SIZE` bytes.
-    For example: "[1,2]" should be "[1,2]\0\0\0\0", length should be 5. */
+    For example: `[1,2]` should be `[1,2]\0\0\0\0`, input length should be 5. */
 static const yyjson_read_flag YYJSON_READ_INSITU                = 1 << 0;
 
 /** Stop when done instead of issuing an error if there's additional content
     after a JSON document. This option may be used to parse small pieces of JSON
     in larger data, such as `NDJSON`. */
 static const yyjson_read_flag YYJSON_READ_STOP_WHEN_DONE        = 1 << 1;
 
 /** Allow single trailing comma at the end of an object or array,
-    such as [1,2,3,] {"a":1,"b":2,} (non-standard). */
+    such as `[1,2,3,]`, `{"a":1,"b":2,}` (non-standard). */
 static const yyjson_read_flag YYJSON_READ_ALLOW_TRAILING_COMMAS = 1 << 2;
 
 /** Allow C-style single line and multiple line comments (non-standard). */
 static const yyjson_read_flag YYJSON_READ_ALLOW_COMMENTS        = 1 << 3;
 
 /** Allow inf/nan number and literal, case-insensitive,
     such as 1e999, NaN, inf, -Infinity (non-standard). */
 static const yyjson_read_flag YYJSON_READ_ALLOW_INF_AND_NAN     = 1 << 4;
 
-/** Read number as raw string (value with YYJSON_TYPE_RAW type),
+/** Read number as raw string (value with `YYJSON_TYPE_RAW` type),
     inf/nan literal is also read as raw with `ALLOW_INF_AND_NAN` flag. */
 static const yyjson_read_flag YYJSON_READ_NUMBER_AS_RAW         = 1 << 5;
 
 /** Allow reading invalid unicode when parsing string values (non-standard).
     Invalid characters will be allowed to appear in the string values, but
     invalid escape sequences will still be reported as errors.
     This flag does not affect the performance of correctly encoded strings.
@@ -612,45 +668,45 @@
 
 /** Result code for JSON reader. */
 typedef uint32_t yyjson_read_code;
 
 /** Success, no error. */
 static const yyjson_read_code YYJSON_READ_SUCCESS                       = 0;
 
-/** Invalid parameter, such as NULL string or invalid file path. */
+/** Invalid parameter, such as NULL input string or 0 input length. */
 static const yyjson_read_code YYJSON_READ_ERROR_INVALID_PARAMETER       = 1;
 
 /** Memory allocation failure occurs. */
 static const yyjson_read_code YYJSON_READ_ERROR_MEMORY_ALLOCATION       = 2;
 
 /** Input JSON string is empty. */
 static const yyjson_read_code YYJSON_READ_ERROR_EMPTY_CONTENT           = 3;
 
-/** Unexpected content after document, such as "[1]#". */
+/** Unexpected content after document, such as `[123]abc`. */
 static const yyjson_read_code YYJSON_READ_ERROR_UNEXPECTED_CONTENT      = 4;
 
-/** Unexpected ending, such as "[123". */
+/** Unexpected ending, such as `[123`. */
 static const yyjson_read_code YYJSON_READ_ERROR_UNEXPECTED_END          = 5;
 
-/** Unexpected character inside the document, such as "[#]". */
+/** Unexpected character inside the document, such as `[abc]`. */
 static const yyjson_read_code YYJSON_READ_ERROR_UNEXPECTED_CHARACTER    = 6;
 
-/** Invalid JSON structure, such as "[1,]". */
+/** Invalid JSON structure, such as `[1,]`. */
 static const yyjson_read_code YYJSON_READ_ERROR_JSON_STRUCTURE          = 7;
 
 /** Invalid comment, such as unclosed multi-line comment. */
 static const yyjson_read_code YYJSON_READ_ERROR_INVALID_COMMENT         = 8;
 
-/** Invalid number, such as "123.e12", "000". */
+/** Invalid number, such as `123.e12`, `000`. */
 static const yyjson_read_code YYJSON_READ_ERROR_INVALID_NUMBER          = 9;
 
 /** Invalid string, such as invalid escaped character inside a string. */
 static const yyjson_read_code YYJSON_READ_ERROR_INVALID_STRING          = 10;
 
-/** Invalid JSON literal, such as "truu". */
+/** Invalid JSON literal, such as `truu`. */
 static const yyjson_read_code YYJSON_READ_ERROR_LITERAL                 = 11;
 
 /** Failed to open a file. */
 static const yyjson_read_code YYJSON_READ_ERROR_FILE_OPEN               = 12;
 
 /** Failed to read a file. */
 static const yyjson_read_code YYJSON_READ_ERROR_FILE_READ               = 13;
@@ -684,15 +740,15 @@
  @param flg The JSON read options.
     Multiple options can be combined with `|` operator. 0 means no options.
  @param alc The memory allocator used by JSON reader.
     Pass NULL to use the libc's default allocator.
  @param err A pointer to receive error information.
     Pass NULL if you don't need error information.
  @return A new JSON document, or NULL if an error occurs.
-    When it's no longer needed, it should be freed with yyjson_doc_free().
+    When it's no longer needed, it should be freed with `yyjson_doc_free()`.
  */
 yyjson_api yyjson_doc *yyjson_read_opts(char *dat,
                                         size_t len,
                                         yyjson_read_flag flg,
                                         const yyjson_alc *alc,
                                         yyjson_read_err *err);
 
@@ -708,15 +764,15 @@
  @param flg The JSON read options.
     Multiple options can be combined with `|` operator. 0 means no options.
  @param alc The memory allocator used by JSON reader.
     Pass NULL to use the libc's default allocator.
  @param err A pointer to receive error information.
     Pass NULL if you don't need error information.
  @return A new JSON document, or NULL if an error occurs.
-    When it's no longer needed, it should be freed with yyjson_doc_free().
+    When it's no longer needed, it should be freed with `yyjson_doc_free()`.
  
  @warning On 32-bit operating system, files larger than 2GB may fail to read.
  */
 yyjson_api yyjson_doc *yyjson_read_file(const char *path,
                                         yyjson_read_flag flg,
                                         const yyjson_alc *alc,
                                         yyjson_read_err *err);
@@ -729,21 +785,22 @@
  @param dat The JSON data (UTF-8 without BOM), null-terminator is not required.
     If this parameter is NULL, the function will fail and return NULL.
  @param len The length of JSON data in bytes.
     If this parameter is 0, the function will fail and return NULL.
  @param flg The JSON read options.
     Multiple options can be combined with `|` operator. 0 means no options.
  @return A new JSON document, or NULL if an error occurs.
-    When it's no longer needed, it should be freed with yyjson_doc_free().
+    When it's no longer needed, it should be freed with `yyjson_doc_free()`.
  */
 yyjson_api_inline yyjson_doc *yyjson_read(const char *dat,
                                           size_t len,
                                           yyjson_read_flag flg) {
     flg &= ~YYJSON_READ_INSITU; /* const string cannot be modified */
-    return yyjson_read_opts((char *)dat, len, flg, NULL, NULL);
+    return yyjson_read_opts((char *)(void *)(size_t)(const void *)dat,
+                            len, flg, NULL, NULL);
 }
 
 /**
  Returns the size of maximum memory usage to read a JSON data.
  
  You may use this value to avoid malloc() or calloc() call inside the reader
  to get better performance, or read multiple JSON with one piece of memory.
@@ -795,14 +852,69 @@
     size_t pad = 256;
     size_t max = (size_t)(~(size_t)0);
     if (flg & YYJSON_READ_STOP_WHEN_DONE) len = len < 256 ? 256 : len;
     if (len >= (max - pad - mul) / mul) return 0;
     return len * mul + pad;
 }
 
+/**
+ Read a JSON number.
+
+ This function is thread-safe when data is not modified by other threads.
+
+ @param dat The JSON data (UTF-8 without BOM), null-terminator is required.
+    If this parameter is NULL, the function will fail and return NULL.
+ @param val The output value where result is stored.
+    If this parameter is NULL, the function will fail and return NULL.
+    The value will hold either UINT or SINT or REAL number;
+ @param flg The JSON read options.
+    Multiple options can be combined with `|` operator. 0 means no options.
+    Suppors `YYJSON_READ_NUMBER_AS_RAW` and `YYJSON_READ_ALLOW_INF_AND_NAN`.
+ @param alc The memory allocator used for long number.
+    It is only used when the built-in floating point reader is disabled.
+    Pass NULL to use the libc's default allocator.
+ @param err A pointer to receive error information.
+    Pass NULL if you don't need error information.
+ @return If successful, a pointer to the character after the last character
+    used in the conversion, NULL if an error occurs.
+ */
+yyjson_api const char *yyjson_read_number(const char *dat,
+                                          yyjson_val *val,
+                                          yyjson_read_flag flg,
+                                          const yyjson_alc *alc,
+                                          yyjson_read_err *err);
+
+/**
+ Read a JSON number.
+
+ This function is thread-safe when data is not modified by other threads.
+
+ @param dat The JSON data (UTF-8 without BOM), null-terminator is required.
+    If this parameter is NULL, the function will fail and return NULL.
+ @param val The output value where result is stored.
+    If this parameter is NULL, the function will fail and return NULL.
+    The value will hold either UINT or SINT or REAL number;
+ @param flg The JSON read options.
+    Multiple options can be combined with `|` operator. 0 means no options.
+    Suppors `YYJSON_READ_NUMBER_AS_RAW` and `YYJSON_READ_ALLOW_INF_AND_NAN`.
+ @param alc The memory allocator used for long number.
+    It is only used when the built-in floating point reader is disabled.
+    Pass NULL to use the libc's default allocator.
+ @param err A pointer to receive error information.
+    Pass NULL if you don't need error information.
+ @return If successful, a pointer to the character after the last character
+    used in the conversion, NULL if an error occurs.
+ */
+yyjson_api_inline const char *yyjson_mut_read_number(const char *dat,
+                                                     yyjson_mut_val *val,
+                                                     yyjson_read_flag flg,
+                                                     const yyjson_alc *alc,
+                                                     yyjson_read_err *err) {
+    return yyjson_read_number(dat, (yyjson_val *)val, flg, alc, err);
+}
 
 
 /*==============================================================================
  * JSON Writer API
  *============================================================================*/
 
 /** Run-time options for JSON writer. */
@@ -832,15 +944,19 @@
 static const yyjson_write_flag YYJSON_WRITE_INF_AND_NAN_AS_NULL     = 1 << 4;
 
 /** Allow invalid unicode when encoding string values (non-standard).
     Invalid characters in string value will be copied byte by byte.
     If `YYJSON_WRITE_ESCAPE_UNICODE` flag is also set, invalid character will be
     escaped as `U+FFFD` (replacement character).
     This flag does not affect the performance of correctly encoded strings. */
-static const yyjson_read_flag YYJSON_WRITE_ALLOW_INVALID_UNICODE    = 1 << 5;
+static const yyjson_write_flag YYJSON_WRITE_ALLOW_INVALID_UNICODE   = 1 << 5;
+
+/** Write JSON pretty with 2 space indent.
+    This flag will override `YYJSON_WRITE_PRETTY` flag. */
+static const yyjson_write_flag YYJSON_WRITE_PRETTY_TWO_SPACES       = 1 << 6;
 
 
 
 /** Result code for JSON writer */
 typedef uint32_t yyjson_write_code;
 
 /** Success, no error. */
@@ -889,16 +1005,16 @@
  
  @param doc The JSON document.
     If this doc is NULL or has no root, the function will fail and return false.
  @param flg The JSON write options.
     Multiple options can be combined with `|` operator. 0 means no options.
  @param alc The memory allocator used by JSON writer.
     Pass NULL to use the libc's default allocator.
- @param len A pointer to receive output length in bytes.
-    Pass NULL if you don't need length information.
+ @param len A pointer to receive output length in bytes (not including the
+    null-terminator). Pass NULL if you don't need length information.
  @param err A pointer to receive error information.
     Pass NULL if you don't need error information.
  @return A new JSON string, or NULL if an error occurs.
     This string is encoded as UTF-8 with a null-terminator.
     When it's no longer needed, it should be freed with free() or alc->free().
  */
 yyjson_api char *yyjson_write_opts(const yyjson_doc *doc,
@@ -940,16 +1056,16 @@
  
  This function is thread-safe.
  
  @param doc The JSON document.
     If this doc is NULL or has no root, the function will fail and return false.
  @param flg The JSON write options.
     Multiple options can be combined with `|` operator. 0 means no options.
- @param len A pointer to receive output length in bytes.
-    Pass NULL if you don't need length information.
+ @param len A pointer to receive output length in bytes (not including the
+    null-terminator). Pass NULL if you don't need length information.
  @return A new JSON string, or NULL if an error occurs.
     This string is encoded as UTF-8 with a null-terminator.
     When it's no longer needed, it should be freed with free().
  */
 yyjson_api_inline char *yyjson_write(const yyjson_doc *doc,
                                      yyjson_write_flag flg,
                                      size_t *len) {
@@ -967,16 +1083,16 @@
 
  @param doc The mutable JSON document.
     If this doc is NULL or has no root, the function will fail and return false.
  @param flg The JSON write options.
     Multiple options can be combined with `|` operator. 0 means no options.
  @param alc The memory allocator used by JSON writer.
     Pass NULL to use the libc's default allocator.
- @param len A pointer to receive output length in bytes.
-    Pass NULL if you don't need length information.
+ @param len A pointer to receive output length in bytes (not including the
+    null-terminator). Pass NULL if you don't need length information.
  @param err A pointer to receive error information.
     Pass NULL if you don't need error information.
  @return A new JSON string, or NULL if an error occurs.
     This string is encoded as UTF-8 with a null-terminator.
     When it's no longer needed, it should be freed with free() or alc->free().
  */
 yyjson_api char *yyjson_mut_write_opts(const yyjson_mut_doc *doc,
@@ -1014,22 +1130,22 @@
                                       const yyjson_alc *alc,
                                       yyjson_write_err *err);
 
 /**
  Write a document to JSON string.
  
  This function is thread-safe when:
- The `doc` is not is not modified by other threads.
+ The `doc` is not modified by other threads.
  
  @param doc The JSON document.
     If this doc is NULL or has no root, the function will fail and return false.
  @param flg The JSON write options.
     Multiple options can be combined with `|` operator. 0 means no options.
- @param len A pointer to receive output length in bytes.
-    Pass NULL if you don't need length information.
+ @param len A pointer to receive output length in bytes (not including the
+    null-terminator). Pass NULL if you don't need length information.
  @return A new JSON string, or NULL if an error occurs.
     This string is encoded as UTF-8 with a null-terminator.
     When it's no longer needed, it should be freed with free().
  */
 yyjson_api_inline char *yyjson_mut_write(const yyjson_mut_doc *doc,
                                          yyjson_write_flag flg,
                                          size_t *len) {
@@ -1050,16 +1166,16 @@
  
  @param val The JSON root value.
     If this parameter is NULL, the function will fail and return NULL.
  @param flg The JSON write options.
     Multiple options can be combined with `|` operator. 0 means no options.
  @param alc The memory allocator used by JSON writer.
     Pass NULL to use the libc's default allocator.
- @param len A pointer to receive output length in bytes.
-    Pass NULL if you don't need length information.
+ @param len A pointer to receive output length in bytes (not including the
+    null-terminator). Pass NULL if you don't need length information.
  @param err A pointer to receive error information.
     Pass NULL if you don't need error information.
  @return A new JSON string, or NULL if an error occurs.
     This string is encoded as UTF-8 with a null-terminator.
     When it's no longer needed, it should be freed with free() or alc->free().
  */
 yyjson_api char *yyjson_val_write_opts(const yyjson_val *val,
@@ -1101,16 +1217,16 @@
  
  This function is thread-safe.
  
  @param val The JSON root value.
     If this parameter is NULL, the function will fail and return NULL.
  @param flg The JSON write options.
     Multiple options can be combined with `|` operator. 0 means no options.
- @param len A pointer to receive output length in bytes.
-    Pass NULL if you don't need length information.
+ @param len A pointer to receive output length in bytes (not including the
+    null-terminator). Pass NULL if you don't need length information.
  @return A new JSON string, or NULL if an error occurs.
     This string is encoded as UTF-8 with a null-terminator.
     When it's no longer needed, it should be freed with free().
  */
 yyjson_api_inline char *yyjson_val_write(const yyjson_val *val,
                                          yyjson_write_flag flg,
                                          size_t *len) {
@@ -1126,16 +1242,16 @@
  
  @param val The mutable JSON root value.
     If this parameter is NULL, the function will fail and return NULL.
  @param flg The JSON write options.
     Multiple options can be combined with `|` operator. 0 means no options.
  @param alc The memory allocator used by JSON writer.
     Pass NULL to use the libc's default allocator.
- @param len A pointer to receive output length in bytes.
-    Pass NULL if you don't need length information.
+ @param len A pointer to receive output length in bytes (not including the
+    null-terminator). Pass NULL if you don't need length information.
  @param err A pointer to receive error information.
     Pass NULL if you don't need error information.
  @return  A new JSON string, or NULL if an error occurs.
     This string is encoded as UTF-8 with a null-terminator.
     When it's no longer needed, it should be freed with free() or alc->free().
  */
 yyjson_api char *yyjson_mut_val_write_opts(const yyjson_mut_val *val,
@@ -1173,22 +1289,22 @@
                                           const yyjson_alc *alc,
                                           yyjson_write_err *err);
 
 /**
  Write a value to JSON string.
  
  This function is thread-safe when:
- The `val` is not is not modified by other threads.
+ The `val` is not modified by other threads.
  
  @param val The JSON root value.
     If this parameter is NULL, the function will fail and return NULL.
  @param flg The JSON write options.
     Multiple options can be combined with `|` operator. 0 means no options.
- @param len A pointer to receive output length in bytes.
-    Pass NULL if you don't need length information.
+ @param len A pointer to receive output length in bytes (not including the
+    null-terminator). Pass NULL if you don't need length information.
  @return A new JSON string, or NULL if an error occurs.
     This string is encoded as UTF-8 with a null-terminator.
     When it's no longer needed, it should be freed with free().
  */
 yyjson_api_inline char *yyjson_mut_val_write(const yyjson_mut_val *val,
                                              yyjson_write_flag flg,
                                              size_t *len) {
@@ -1203,20 +1319,20 @@
 
 /** Returns the root value of this JSON document.
     Returns NULL if `doc` is NULL. */
 yyjson_api_inline yyjson_val *yyjson_doc_get_root(yyjson_doc *doc);
 
 /** Returns read size of input JSON data.
     Returns 0 if `doc` is NULL.
-    For example: the read size of "[1,2,3]" is 7 bytes.  */
+    For example: the read size of `[1,2,3]` is 7 bytes.  */
 yyjson_api_inline size_t yyjson_doc_get_read_size(yyjson_doc *doc);
 
 /** Returns total value count in this JSON document.
     Returns 0 if `doc` is NULL.
-    For example: the value count of "[1,2,3]" is 4. */
+    For example: the value count of `[1,2,3]` is 4. */
 yyjson_api_inline size_t yyjson_doc_get_val_count(yyjson_doc *doc);
 
 /** Release the JSON document and free the memory.
     After calling this function, the `doc` and all values from the `doc` are no
     longer available. This function will do nothing if the `doc` is NULL. */
 yyjson_api_inline void yyjson_doc_free(yyjson_doc *doc);
 
@@ -1325,14 +1441,18 @@
     Returns 0 if `val` is NULL or type is not integer(sint/uint). */
 yyjson_api_inline int yyjson_get_int(yyjson_val *val);
 
 /** Returns the content if the value is real number, or 0.0 on error.
     Returns 0.0 if `val` is NULL or type is not real(double). */
 yyjson_api_inline double yyjson_get_real(yyjson_val *val);
 
+/** Returns the content and typecast to `double` if the value is number.
+    Returns 0.0 if `val` is NULL or type is not number(uint/sint/real). */
+yyjson_api_inline double yyjson_get_num(yyjson_val *val);
+
 /** Returns the content if the value is string.
     Returns NULL if `val` is NULL or type is not string. */
 yyjson_api_inline const char *yyjson_get_str(yyjson_val *val);
 
 /** Returns the content length (string length, array size, object size.
     Returns 0 if `val` is NULL or type is not string/array/object. */
 yyjson_api_inline size_t yyjson_get_len(yyjson_val *val);
@@ -1344,63 +1464,116 @@
 /** Returns whether the JSON value is equals to a string.
     The `str` should be a UTF-8 string, null-terminator is not required.
     Returns false if input is NULL or type is not string. */
 yyjson_api_inline bool yyjson_equals_strn(yyjson_val *val, const char *str,
                                           size_t len);
 
 /** Returns whether two JSON values are equal (deep compare).
-    Returns false if input is NULL. */
+    Returns false if input is NULL.
+    @note the result may be inaccurate if object has duplicate keys.
+    @warning This function is recursive and may cause a stack overflow
+        if the object level is too deep. */
 yyjson_api_inline bool yyjson_equals(yyjson_val *lhs, yyjson_val *rhs);
 
+/** Set the value to raw.
+    Returns false if input is NULL or `val` is object or array.
+    @warning This will modify the `immutable` value, use with caution. */
+yyjson_api_inline bool yyjson_set_raw(yyjson_val *val,
+                                      const char *raw, size_t len);
+
+/** Set the value to null.
+    Returns false if input is NULL or `val` is object or array.
+    @warning This will modify the `immutable` value, use with caution. */
+yyjson_api_inline bool yyjson_set_null(yyjson_val *val);
+
+/** Set the value to bool.
+    Returns false if input is NULL or `val` is object or array.
+    @warning This will modify the `immutable` value, use with caution. */
+yyjson_api_inline bool yyjson_set_bool(yyjson_val *val, bool num);
+
+/** Set the value to uint.
+    Returns false if input is NULL or `val` is object or array.
+    @warning This will modify the `immutable` value, use with caution. */
+yyjson_api_inline bool yyjson_set_uint(yyjson_val *val, uint64_t num);
+
+/** Set the value to sint.
+    Returns false if input is NULL or `val` is object or array.
+    @warning This will modify the `immutable` value, use with caution. */
+yyjson_api_inline bool yyjson_set_sint(yyjson_val *val, int64_t num);
+
+/** Set the value to int.
+    Returns false if input is NULL or `val` is object or array.
+    @warning This will modify the `immutable` value, use with caution. */
+yyjson_api_inline bool yyjson_set_int(yyjson_val *val, int num);
+
+/** Set the value to real.
+    Returns false if input is NULL or `val` is object or array.
+    @warning This will modify the `immutable` value, use with caution. */
+yyjson_api_inline bool yyjson_set_real(yyjson_val *val, double num);
+
+/** Set the value to string (null-terminated).
+    Returns false if input is NULL or `val` is object or array.
+    @warning This will modify the `immutable` value, use with caution. */
+yyjson_api_inline bool yyjson_set_str(yyjson_val *val, const char *str);
+
+/** Set the value to string (with length).
+    Returns false if input is NULL or `val` is object or array.
+    @warning This will modify the `immutable` value, use with caution. */
+yyjson_api_inline bool yyjson_set_strn(yyjson_val *val,
+                                       const char *str, size_t len);
+
 
 
 /*==============================================================================
  * JSON Array API
  *============================================================================*/
 
 /** Returns the number of elements in this array.
     Returns 0 if `arr` is NULL or type is not array. */
 yyjson_api_inline size_t yyjson_arr_size(yyjson_val *arr);
 
 /** Returns the element at the specified position in this array.
     Returns NULL if array is NULL/empty or the index is out of bounds.
     @warning This function takes a linear search time if array is not flat.
-        For example: [1,{},3] is flat, [1,[2],3] is not flat. */
+        For example: `[1,{},3]` is flat, `[1,[2],3]` is not flat. */
 yyjson_api_inline yyjson_val *yyjson_arr_get(yyjson_val *arr, size_t idx);
 
 /** Returns the first element of this array.
     Returns NULL if `arr` is NULL/empty or type is not array. */
 yyjson_api_inline yyjson_val *yyjson_arr_get_first(yyjson_val *arr);
 
 /** Returns the last element of this array.
     Returns NULL if `arr` is NULL/empty or type is not array.
     @warning This function takes a linear search time if array is not flat.
-        For example: [1,{},3] is flat, [1,[2],3] is not flat.*/
+        For example: `[1,{},3]` is flat, `[1,[2],3]` is not flat.*/
 yyjson_api_inline yyjson_val *yyjson_arr_get_last(yyjson_val *arr);
 
 
 
 /*==============================================================================
  * JSON Array Iterator API
  *============================================================================*/
 
 /**
  A JSON array iterator.
  
  @par Example
  @code
     yyjson_val *val;
-    yyjson_arr_iter iter;
-    yyjson_arr_iter_init(arr, &iter);
+    yyjson_arr_iter iter = yyjson_arr_iter_with(arr);
     while ((val = yyjson_arr_iter_next(&iter))) {
         your_func(val);
     }
  @endcode
  */
-typedef struct yyjson_arr_iter yyjson_arr_iter;
+typedef struct yyjson_arr_iter {
+    size_t idx; /**< next value's index */
+    size_t max; /**< maximum index (arr.size) */
+    yyjson_val *cur; /**< next value */
+} yyjson_arr_iter;
 
 /**
  Initialize an iterator for this array.
  
  @param arr The array to be iterated over.
     If this parameter is NULL or not an array, `iter` will be set to empty.
  @param iter The iterator to be initialized.
@@ -1409,14 +1582,25 @@
  
  @note The iterator does not need to be destroyed.
  */
 yyjson_api_inline bool yyjson_arr_iter_init(yyjson_val *arr,
                                             yyjson_arr_iter *iter);
 
 /**
+ Create an iterator with an array , same as `yyjson_arr_iter_init()`.
+ 
+ @param arr The array to be iterated over.
+    If this parameter is NULL or not an array, an empty iterator will returned.
+ @return A new iterator for the array.
+ 
+ @note The iterator does not need to be destroyed.
+ */
+yyjson_api_inline yyjson_arr_iter yyjson_arr_iter_with(yyjson_val *arr);
+
+/**
  Returns whether the iteration has more elements.
  If `iter` is NULL, this function will return false.
  */
 yyjson_api_inline bool yyjson_arr_iter_has_next(yyjson_arr_iter *iter);
 
 /**
  Returns the next element in the iteration, or NULL on end.
@@ -1483,35 +1667,38 @@
 
 /**
  A JSON object iterator.
  
  @par Example
  @code
     yyjson_val *key, *val;
-    yyjson_obj_iter iter;
-    yyjson_obj_iter_init(obj, &iter);
+    yyjson_obj_iter iter = yyjson_obj_iter_with(obj);
     while ((key = yyjson_obj_iter_next(&iter))) {
         val = yyjson_obj_iter_get_val(key);
         your_func(key, val);
     }
  @endcode
  
  If the ordering of the keys is known at compile-time, you can use this method
  to speed up value lookups:
  @code
     // {"k1":1, "k2": 3, "k3": 3}
     yyjson_val *key, *val;
-    yyjson_obj_iter iter;
-    yyjson_obj_iter_init(obj, &iter);
+    yyjson_obj_iter iter = yyjson_obj_iter_with(obj);
     yyjson_val *v1 = yyjson_obj_iter_get(&iter, "k1");
     yyjson_val *v3 = yyjson_obj_iter_get(&iter, "k3");
  @endcode
  @see yyjson_obj_iter_get() and yyjson_obj_iter_getn()
  */
-typedef struct yyjson_obj_iter yyjson_obj_iter;
+typedef struct yyjson_obj_iter {
+    size_t idx; /**< next key's index */
+    size_t max; /**< maximum key index (obj.size) */
+    yyjson_val *cur; /**< next key */
+    yyjson_val *obj; /**< the object being iterated */
+} yyjson_obj_iter;
 
 /**
  Initialize an iterator for this object.
  
  @param obj The object to be iterated over.
     If this parameter is NULL or not an object, `iter` will be set to empty.
  @param iter The iterator to be initialized.
@@ -1520,14 +1707,25 @@
  
  @note The iterator does not need to be destroyed.
  */
 yyjson_api_inline bool yyjson_obj_iter_init(yyjson_val *obj,
                                             yyjson_obj_iter *iter);
 
 /**
+ Create an iterator with an object, same as `yyjson_obj_iter_init()`.
+ 
+ @param obj The object to be iterated over.
+    If this parameter is NULL or not an object, an empty iterator will returned.
+ @return A new iterator for the object.
+ 
+ @note The iterator does not need to be destroyed.
+ */
+yyjson_api_inline yyjson_obj_iter yyjson_obj_iter_with(yyjson_val *obj);
+
+/**
  Returns whether the iteration has more elements.
  If `iter` is NULL, this function will return false.
  */
 yyjson_api_inline bool yyjson_obj_iter_has_next(yyjson_obj_iter *iter);
 
 /**
  Returns the next key in the iteration, or NULL on end.
@@ -1540,15 +1738,15 @@
  If `iter` is NULL, this function will return NULL.
  */
 yyjson_api_inline yyjson_val *yyjson_obj_iter_get_val(yyjson_val *key);
 
 /**
  Iterates to a specified key and returns the value.
  
- This function does the same thing as yyjson_obj_get(), but is much faster
+ This function does the same thing as `yyjson_obj_get()`, but is much faster
  if the ordering of the keys is known at compile-time and you are using the same
  order to look up the values. If the key exists in this object, then the
  iterator will stop at the next key, otherwise the iterator will not change and
  NULL is returned.
  
  @param iter The object iterator, should not be NULL.
  @param key The key, should be a UTF-8 string with null-terminator.
@@ -1559,15 +1757,15 @@
  */
 yyjson_api_inline yyjson_val *yyjson_obj_iter_get(yyjson_obj_iter *iter,
                                                   const char *key);
 
 /**
  Iterates to a specified key and returns the value.
 
- This function does the same thing as yyjson_obj_getn(), but is much faster
+ This function does the same thing as `yyjson_obj_getn()`, but is much faster
  if the ordering of the keys is known at compile-time and you are using the same
  order to look up the values. If the key exists in this object, then the
  iterator will stop at the next key, otherwise the iterator will not change and
  NULL is returned.
  
  @param iter The object iterator, should not be NULL.
  @param key The key, should be a UTF-8 string, null-terminator is not required.
@@ -1615,50 +1813,103 @@
 yyjson_api_inline yyjson_mut_val *yyjson_mut_doc_get_root(yyjson_mut_doc *doc);
 
 /** Sets the root value of this JSON document.
     Pass NULL to clear root value of the document. */
 yyjson_api_inline void yyjson_mut_doc_set_root(yyjson_mut_doc *doc,
                                                yyjson_mut_val *root);
 
+/**
+ Set the string pool size for a mutable document.
+ This function does not allocate memory immediately, but uses the size when
+ the next memory allocation is needed.
+ 
+ If the caller knows the approximate bytes of strings that the document needs to
+ store (e.g. copy string with `yyjson_mut_strcpy` function), setting a larger
+ size can avoid multiple memory allocations and improve performance.
+ 
+ @param doc The mutable document.
+ @param len The desired string pool size in bytes (total string length).
+ @return true if successful, false if size is 0 or overflow.
+ */
+yyjson_api bool yyjson_mut_doc_set_str_pool_size(yyjson_mut_doc *doc,
+                                                 size_t len);
+
+/**
+ Set the value pool size for a mutable document.
+ This function does not allocate memory immediately, but uses the size when
+ the next memory allocation is needed.
+ 
+ If the caller knows the approximate number of values that the document needs to
+ store (e.g. create new value with `yyjson_mut_xxx` functions), setting a larger
+ size can avoid multiple memory allocations and improve performance.
+ 
+ @param doc The mutable document.
+ @param count The desired value pool size (number of `yyjson_mut_val`).
+ @return true if successful, false if size is 0 or overflow.
+ */
+yyjson_api bool yyjson_mut_doc_set_val_pool_size(yyjson_mut_doc *doc,
+                                                 size_t count);
+
 /** Release the JSON document and free the memory.
     After calling this function, the `doc` and all values from the `doc` are no
     longer available. This function will do nothing if the `doc` is NULL.  */
 yyjson_api void yyjson_mut_doc_free(yyjson_mut_doc *doc);
 
 /** Creates and returns a new mutable JSON document, returns NULL on error.
     If allocator is NULL, the default allocator will be used. */
 yyjson_api yyjson_mut_doc *yyjson_mut_doc_new(const yyjson_alc *alc);
 
 /** Copies and returns a new mutable document from input, returns NULL on error.
     This makes a `deep-copy` on the immutable document.
-    If allocator is NULL, the default allocator will be used. */
+    If allocator is NULL, the default allocator will be used.
+    @note `imut_doc` -> `mut_doc`. */
 yyjson_api yyjson_mut_doc *yyjson_doc_mut_copy(yyjson_doc *doc,
                                                const yyjson_alc *alc);
 
 /** Copies and returns a new mutable document from input, returns NULL on error.
     This makes a `deep-copy` on the mutable document.
-    If allocator is NULL, the default allocator will be used. */
+    If allocator is NULL, the default allocator will be used.
+    @note `mut_doc` -> `mut_doc`. */
 yyjson_api yyjson_mut_doc *yyjson_mut_doc_mut_copy(yyjson_mut_doc *doc,
                                                    const yyjson_alc *alc);
 
 /** Copies and returns a new mutable value from input, returns NULL on error.
     This makes a `deep-copy` on the immutable value.
-    The memory was managed by mutable document. */
+    The memory was managed by mutable document.
+    @note `imut_val` -> `mut_val`. */
 yyjson_api yyjson_mut_val *yyjson_val_mut_copy(yyjson_mut_doc *doc,
                                                yyjson_val *val);
 
-/** Copies and return a new mutable value from input, returns NULL on error,
+/** Copies and returns a new mutable value from input, returns NULL on error.
     This makes a `deep-copy` on the mutable value.
     The memory was managed by mutable document.
-    
+    @note `mut_val` -> `mut_val`.
     @warning This function is recursive and may cause a stack overflow
         if the object level is too deep. */
 yyjson_api yyjson_mut_val *yyjson_mut_val_mut_copy(yyjson_mut_doc *doc,
                                                    yyjson_mut_val *val);
 
+/** Copies and returns a new immutable document from input,
+    returns NULL on error. This makes a `deep-copy` on the mutable document.
+    The returned document should be freed with `yyjson_doc_free()`.
+    @note `mut_doc` -> `imut_doc`.
+    @warning This function is recursive and may cause a stack overflow
+        if the object level is too deep. */
+yyjson_api yyjson_doc *yyjson_mut_doc_imut_copy(yyjson_mut_doc *doc,
+                                                const yyjson_alc *alc);
+
+/** Copies and returns a new immutable document from input,
+    returns NULL on error. This makes a `deep-copy` on the mutable value.
+    The returned document should be freed with `yyjson_doc_free()`.
+    @note `mut_val` -> `imut_doc`.
+    @warning This function is recursive and may cause a stack overflow
+        if the object level is too deep. */
+yyjson_api yyjson_doc *yyjson_mut_val_imut_copy(yyjson_mut_val *val,
+                                                const yyjson_alc *alc);
+
 
 
 /*==============================================================================
  * Mutable JSON Value Type API
  *============================================================================*/
 
 /** Returns whether the JSON value is raw.
@@ -1720,19 +1971,19 @@
 
 
 /*==============================================================================
  * Mutable JSON Value Content API
  *============================================================================*/
 
 /** Returns the JSON value's type.
-    Returns YYJSON_TYPE_NONE if `val` is NULL. */
+    Returns `YYJSON_TYPE_NONE` if `val` is NULL. */
 yyjson_api_inline yyjson_type yyjson_mut_get_type(yyjson_mut_val *val);
 
 /** Returns the JSON value's subtype.
-    Returns YYJSON_SUBTYPE_NONE if `val` is NULL. */
+    Returns `YYJSON_SUBTYPE_NONE` if `val` is NULL. */
 yyjson_api_inline yyjson_subtype yyjson_mut_get_subtype(yyjson_mut_val *val);
 
 /** Returns the JSON value's tag.
     Returns 0 if `val` is NULL. */
 yyjson_api_inline uint8_t yyjson_mut_get_tag(yyjson_mut_val *val);
 
 /** Returns the JSON value's type description.
@@ -1760,14 +2011,18 @@
     Returns 0 if `val` is NULL or type is not integer(sint/uint). */
 yyjson_api_inline int yyjson_mut_get_int(yyjson_mut_val *val);
 
 /** Returns the content if the value is real number.
     Returns 0.0 if `val` is NULL or type is not real(double). */
 yyjson_api_inline double yyjson_mut_get_real(yyjson_mut_val *val);
 
+/** Returns the content and typecast to `double` if the value is number.
+    Returns 0.0 if `val` is NULL or type is not number(uint/sint/real). */
+yyjson_api_inline double yyjson_mut_get_num(yyjson_mut_val *val);
+
 /** Returns the content if the value is string.
     Returns NULL if `val` is NULL or type is not string. */
 yyjson_api_inline const char *yyjson_mut_get_str(yyjson_mut_val *val);
 
 /** Returns the content length (string length, array size, object size.
     Returns 0 if `val` is NULL or type is not string/array/object. */
 yyjson_api_inline size_t yyjson_mut_get_len(yyjson_mut_val *val);
@@ -1782,20 +2037,77 @@
     The `str` should be a UTF-8 string, null-terminator is not required.
     Returns false if input is NULL or type is not string. */
 yyjson_api_inline bool yyjson_mut_equals_strn(yyjson_mut_val *val,
                                               const char *str, size_t len);
 
 /** Returns whether two JSON values are equal (deep compare).
     Returns false if input is NULL.
-    
+    @note the result may be inaccurate if object has duplicate keys.
     @warning This function is recursive and may cause a stack overflow
         if the object level is too deep. */
 yyjson_api_inline bool yyjson_mut_equals(yyjson_mut_val *lhs,
                                          yyjson_mut_val *rhs);
 
+/** Set the value to raw.
+    Returns false if input is NULL.
+    @warning This function should not be used on an existing object or array. */
+yyjson_api_inline bool yyjson_mut_set_raw(yyjson_mut_val *val,
+                                          const char *raw, size_t len);
+
+/** Set the value to null.
+    Returns false if input is NULL.
+    @warning This function should not be used on an existing object or array. */
+yyjson_api_inline bool yyjson_mut_set_null(yyjson_mut_val *val);
+
+/** Set the value to bool.
+    Returns false if input is NULL.
+    @warning This function should not be used on an existing object or array. */
+yyjson_api_inline bool yyjson_mut_set_bool(yyjson_mut_val *val, bool num);
+
+/** Set the value to uint.
+    Returns false if input is NULL.
+    @warning This function should not be used on an existing object or array. */
+yyjson_api_inline bool yyjson_mut_set_uint(yyjson_mut_val *val, uint64_t num);
+
+/** Set the value to sint.
+    Returns false if input is NULL.
+    @warning This function should not be used on an existing object or array. */
+yyjson_api_inline bool yyjson_mut_set_sint(yyjson_mut_val *val, int64_t num);
+
+/** Set the value to int.
+    Returns false if input is NULL.
+    @warning This function should not be used on an existing object or array. */
+yyjson_api_inline bool yyjson_mut_set_int(yyjson_mut_val *val, int num);
+
+/** Set the value to real.
+    Returns false if input is NULL.
+    @warning This function should not be used on an existing object or array. */
+yyjson_api_inline bool yyjson_mut_set_real(yyjson_mut_val *val, double num);
+
+/** Set the value to string (null-terminated).
+    Returns false if input is NULL.
+    @warning This function should not be used on an existing object or array. */
+yyjson_api_inline bool yyjson_mut_set_str(yyjson_mut_val *val, const char *str);
+
+/** Set the value to string (with length).
+    Returns false if input is NULL.
+    @warning This function should not be used on an existing object or array. */
+yyjson_api_inline bool yyjson_mut_set_strn(yyjson_mut_val *val,
+                                           const char *str, size_t len);
+
+/** Set the value to array.
+    Returns false if input is NULL.
+    @warning This function should not be used on an existing object or array. */
+yyjson_api_inline bool yyjson_mut_set_arr(yyjson_mut_val *val);
+
+/** Set the value to array.
+    Returns false if input is NULL.
+    @warning This function should not be used on an existing object or array. */
+yyjson_api_inline bool yyjson_mut_set_obj(yyjson_mut_val *val);
+
 
 
 /*==============================================================================
  * Mutable JSON Value Creation API
  *============================================================================*/
 
 /** Creates and returns a raw value, returns NULL on error.
@@ -1915,30 +2227,35 @@
  * Mutable JSON Array Iterator API
  *============================================================================*/
 
 /**
  A mutable JSON array iterator.
  
  @warning You should not modify the array while iterating over it, but you can
-    use yyjson_mut_arr_iter_remove() to remove current value.
+    use `yyjson_mut_arr_iter_remove()` to remove current value.
  
  @par Example
  @code
     yyjson_mut_val *val;
-    yyjson_mut_arr_iter iter;
-    yyjson_mut_arr_iter_init(arr, &iter);
+    yyjson_mut_arr_iter iter = yyjson_mut_arr_iter_with(arr);
     while ((val = yyjson_mut_arr_iter_next(&iter))) {
         your_func(val);
         if (your_val_is_unused(val)) {
             yyjson_mut_arr_iter_remove(&iter);
         }
     }
  @endcode
  */
-typedef struct yyjson_mut_arr_iter yyjson_mut_arr_iter;
+typedef struct yyjson_mut_arr_iter {
+    size_t idx; /**< next value's index */
+    size_t max; /**< maximum index (arr.size) */
+    yyjson_mut_val *cur; /**< current value */
+    yyjson_mut_val *pre; /**< previous value */
+    yyjson_mut_val *arr; /**< the array being iterated */
+} yyjson_mut_arr_iter;
 
 /**
  Initialize an iterator for this array.
  
  @param arr The array to be iterated over.
     If this parameter is NULL or not an array, `iter` will be set to empty.
  @param iter The iterator to be initialized.
@@ -1947,14 +2264,26 @@
  
  @note The iterator does not need to be destroyed.
  */
 yyjson_api_inline bool yyjson_mut_arr_iter_init(yyjson_mut_val *arr,
     yyjson_mut_arr_iter *iter);
 
 /**
+ Create an iterator with an array , same as `yyjson_mut_arr_iter_init()`.
+ 
+ @param arr The array to be iterated over.
+    If this parameter is NULL or not an array, an empty iterator will returned.
+ @return A new iterator for the array.
+ 
+ @note The iterator does not need to be destroyed.
+ */
+yyjson_api_inline yyjson_mut_arr_iter yyjson_mut_arr_iter_with(
+    yyjson_mut_val *arr);
+
+/**
  Returns whether the iteration has more elements.
  If `iter` is NULL, this function will return false.
  */
 yyjson_api_inline bool yyjson_mut_arr_iter_has_next(
     yyjson_mut_arr_iter *iter);
 
 /**
@@ -2269,15 +2598,15 @@
     If this array contains NULL, the function will fail and return NULL.
  @param count The number of values in `vals`.
     If this value is 0, an empty array will return.
  @return The new array. NULL if input is invalid or memory allocation failed.
  
  @warning The input strings are not copied, you should keep these strings
     unmodified for the lifetime of this JSON document. If these strings will be
-    modified, you should use yyjson_mut_arr_with_strcpy() instead.
+    modified, you should use `yyjson_mut_arr_with_strcpy()` instead.
  
  @par Example
  @code
     const char *vals[3] = { "a", "b", "c" };
     yyjson_mut_val *arr = yyjson_mut_arr_with_str(doc, vals, 3);
  @endcode
  */
@@ -2295,15 +2624,15 @@
  @param lens A C array of string lengths, in bytes.
  @param count The number of strings in `vals`.
     If this value is 0, an empty array will return.
  @return The new array. NULL if input is invalid or memory allocation failed.
  
  @warning The input strings are not copied, you should keep these strings
     unmodified for the lifetime of this JSON document. If these strings will be
-    modified, you should use yyjson_mut_arr_with_strncpy() instead.
+    modified, you should use `yyjson_mut_arr_with_strncpy()` instead.
  
  @par Example
  @code
     const char *vals[3] = { "a", "bb", "c" };
     const size_t lens[3] = { 1, 2, 1 };
     yyjson_mut_val *arr = yyjson_mut_arr_with_strn(doc, vals, lens, 3);
  @endcode
@@ -2456,15 +2785,15 @@
     Returns false if it is NULL or not an array.
  @return Whether successful.
  */
 yyjson_api_inline bool yyjson_mut_arr_clear(yyjson_mut_val *arr);
 
 /**
  Rotates values in this array for the given number of times.
- For example: [1,2,3,4,5] rotate 2 is [3,4,5,1,2].
+ For example: `[1,2,3,4,5]` rotate 2 is `[3,4,5,1,2]`.
  @param arr The array to be rotated.
  @param idx Index (or times) to rotate.
  @warning This function takes a linear search time.
  */
 yyjson_api_inline bool yyjson_mut_arr_rotate(yyjson_mut_val *arr,
                                              size_t idx);
 
@@ -2688,43 +3017,47 @@
  * Mutable JSON Object Iterator API
  *============================================================================*/
 
 /**
  A mutable JSON object iterator.
  
  @warning You should not modify the object while iterating over it, but you can
-    use yyjson_mut_obj_iter_remove() to remove current value.
+    use `yyjson_mut_obj_iter_remove()` to remove current value.
  
  @par Example
  @code
     yyjson_mut_val *key, *val;
-    yyjson_mut_obj_iter iter;
-    yyjson_mut_obj_iter_init(obj, &iter);
+    yyjson_mut_obj_iter iter = yyjson_mut_obj_iter_with(obj);
     while ((key = yyjson_mut_obj_iter_next(&iter))) {
         val = yyjson_mut_obj_iter_get_val(key);
         your_func(key, val);
         if (your_val_is_unused(key, val)) {
             yyjson_mut_obj_iter_remove(&iter);
         }
     }
  @endcode
  
  If the ordering of the keys is known at compile-time, you can use this method
  to speed up value lookups:
  @code
     // {"k1":1, "k2": 3, "k3": 3}
     yyjson_mut_val *key, *val;
-    yyjson_mut_obj_iter iter;
-    yyjson_mut_obj_iter_init(obj, &iter);
+    yyjson_mut_obj_iter iter = yyjson_mut_obj_iter_with(obj);
     yyjson_mut_val *v1 = yyjson_mut_obj_iter_get(&iter, "k1");
     yyjson_mut_val *v3 = yyjson_mut_obj_iter_get(&iter, "k3");
  @endcode
- @see yyjson_mut_obj_iter_get() and yyjson_mut_obj_iter_getn()
+ @see `yyjson_mut_obj_iter_get()` and `yyjson_mut_obj_iter_getn()`
  */
-typedef struct yyjson_mut_obj_iter yyjson_mut_obj_iter;
+typedef struct yyjson_mut_obj_iter {
+    size_t idx; /**< next key's index */
+    size_t max; /**< maximum key index (obj.size) */
+    yyjson_mut_val *cur; /**< current key */
+    yyjson_mut_val *pre; /**< previous key */
+    yyjson_mut_val *obj; /**< the object being iterated */
+} yyjson_mut_obj_iter;
 
 /**
  Initialize an iterator for this object.
  
  @param obj The object to be iterated over.
     If this parameter is NULL or not an array, `iter` will be set to empty.
  @param iter The iterator to be initialized.
@@ -2733,14 +3066,26 @@
  
  @note The iterator does not need to be destroyed.
  */
 yyjson_api_inline bool yyjson_mut_obj_iter_init(yyjson_mut_val *obj,
     yyjson_mut_obj_iter *iter);
 
 /**
+ Create an iterator with an object, same as `yyjson_obj_iter_init()`.
+ 
+ @param obj The object to be iterated over.
+    If this parameter is NULL or not an object, an empty iterator will returned.
+ @return A new iterator for the object.
+ 
+ @note The iterator does not need to be destroyed.
+ */
+yyjson_api_inline yyjson_mut_obj_iter yyjson_mut_obj_iter_with(
+    yyjson_mut_val *obj);
+
+/**
  Returns whether the iteration has more elements.
  If `iter` is NULL, this function will return false.
  */
 yyjson_api_inline bool yyjson_mut_obj_iter_has_next(
     yyjson_mut_obj_iter *iter);
 
 /**
@@ -2754,24 +3099,24 @@
  Returns the value for key inside the iteration.
  If `iter` is NULL, this function will return NULL.
  */
 yyjson_api_inline yyjson_mut_val *yyjson_mut_obj_iter_get_val(
     yyjson_mut_val *key);
 
 /**
- Removes and returns current key-value pair in the iteration.
+ Removes current key-value pair in the iteration, returns the removed value.
  If `iter` is NULL, this function will return NULL.
  */
 yyjson_api_inline yyjson_mut_val *yyjson_mut_obj_iter_remove(
     yyjson_mut_obj_iter *iter);
 
 /**
  Iterates to a specified key and returns the value.
  
- This function does the same thing as yyjson_mut_obj_get(), but is much faster
+ This function does the same thing as `yyjson_mut_obj_get()`, but is much faster
  if the ordering of the keys is known at compile-time and you are using the same
  order to look up the values. If the key exists in this object, then the
  iterator will stop at the next key, otherwise the iterator will not change and
  NULL is returned.
  
  @param iter The object iterator, should not be NULL.
  @param key The key, should be a UTF-8 string with null-terminator.
@@ -2782,15 +3127,15 @@
  */
 yyjson_api_inline yyjson_mut_val *yyjson_mut_obj_iter_get(
     yyjson_mut_obj_iter *iter, const char *key);
 
 /**
  Iterates to a specified key and returns the value.
  
- This function does the same thing as yyjson_mut_obj_getn(), but is much faster
+ This function does the same thing as `yyjson_mut_obj_getn()` but is much faster
  if the ordering of the keys is known at compile-time and you are using the same
  order to look up the values. If the key exists in this object, then the
  iterator will stop at the next key, otherwise the iterator will not change and
  NULL is returned.
  
  @param iter The object iterator, should not be NULL.
  @param key The key, should be a UTF-8 string, null-terminator is not required.
@@ -2881,42 +3226,42 @@
  * Mutable JSON Object Modification API
  *============================================================================*/
 
 /**
  Adds a key-value pair at the end of the object.
  This function allows duplicated key in one object.
  @param obj The object to which the new key-value pair is to be added.
- @param key The key, should be a string which is created by yyjson_mut_str(),
-    yyjson_mut_strn(), yyjson_mut_strcpy() or yyjson_mut_strncpy().
+ @param key The key, should be a string which is created by `yyjson_mut_str()`,
+    `yyjson_mut_strn()`, `yyjson_mut_strcpy()` or `yyjson_mut_strncpy()`.
  @param val The value to add to the object.
  @return Whether successful.
  */
 yyjson_api_inline bool yyjson_mut_obj_add(yyjson_mut_val *obj,
                                           yyjson_mut_val *key,
                                           yyjson_mut_val *val);
 /**
  Sets a key-value pair at the end of the object.
  This function may remove all key-value pairs for the given key before add.
  @param obj The object to which the new key-value pair is to be added.
- @param key The key, should be a string which is created by yyjson_mut_str(),
-    yyjson_mut_strn(), yyjson_mut_strcpy() or yyjson_mut_strncpy().
+ @param key The key, should be a string which is created by `yyjson_mut_str()`,
+    `yyjson_mut_strn()`, `yyjson_mut_strcpy()` or `yyjson_mut_strncpy()`.
  @param val The value to add to the object. If this value is null, the behavior
-    is same as yyjson_mut_obj_remove().
+    is same as `yyjson_mut_obj_remove()`.
  @return Whether successful.
  */
 yyjson_api_inline bool yyjson_mut_obj_put(yyjson_mut_val *obj,
                                           yyjson_mut_val *key,
                                           yyjson_mut_val *val);
 
 /**
  Inserts a key-value pair to the object at the given position.
  This function allows duplicated key in one object.
  @param obj The object to which the new key-value pair is to be added.
- @param key The key, should be a string which is created by yyjson_mut_str(),
-    yyjson_mut_strn(), yyjson_mut_strcpy() or yyjson_mut_strncpy().
+ @param key The key, should be a string which is created by `yyjson_mut_str()`,
+    `yyjson_mut_strn()`, `yyjson_mut_strcpy()` or `yyjson_mut_strncpy()`.
  @param val The value to add to the object.
  @param idx The index to which to insert the new pair.
  @return Whether successful.
  */
 yyjson_api_inline bool yyjson_mut_obj_insert(yyjson_mut_val *obj,
                                              yyjson_mut_val *key,
                                              yyjson_mut_val *val,
@@ -2971,15 +3316,16 @@
  */
 yyjson_api_inline bool yyjson_mut_obj_replace(yyjson_mut_val *obj,
                                               yyjson_mut_val *key,
                                               yyjson_mut_val *val);
 
 /**
  Rotates key-value pairs in the object for the given number of times.
- For example: {"a":1,"b":2,"c":3,"d":4} rotate 1 is {"b":2,"c":3,"d":4,"a":1}.
+ For example: `{"a":1,"b":2,"c":3,"d":4}` rotate 1 is
+ `{"b":2,"c":3,"d":4,"a":1}`.
  @param obj The object to be rotated.
  @param idx Index (or times) to rotate.
  @return Whether successful.
  @warning This function takes a linear search time.
  */
 yyjson_api_inline bool yyjson_mut_obj_rotate(yyjson_mut_val *obj,
                                              size_t idx);
@@ -3144,109 +3490,722 @@
     The `key` should be a UTF-8 string, null-terminator is not required.
     The `len` should be the length of the key, in bytes.
     
     @warning This function takes a linear search time. */
 yyjson_api_inline yyjson_mut_val *yyjson_mut_obj_remove_strn(
     yyjson_mut_val *obj, const char *key, size_t len);
 
+/** Replaces all matching keys with the new key.
+    Returns true if at least one key was renamed.
+    The `key` and `new_key` should be a null-terminated UTF-8 string.
+    The `new_key` is copied and held by doc.
+    
+    @warning This function takes a linear search time.
+    If `new_key` already exists, it will cause duplicate keys.
+ */
+yyjson_api_inline bool yyjson_mut_obj_rename_key(yyjson_mut_doc *doc,
+                                                 yyjson_mut_val *obj,
+                                                 const char *key,
+                                                 const char *new_key);
+
+/** Replaces all matching keys with the new key.
+    Returns true if at least one key was renamed.
+    The `key` and `new_key` should be a UTF-8 string,
+    null-terminator is not required. The `new_key` is copied and held by doc.
+    
+    @warning This function takes a linear search time.
+    If `new_key` already exists, it will cause duplicate keys.
+ */
+yyjson_api_inline bool yyjson_mut_obj_rename_keyn(yyjson_mut_doc *doc,
+                                                  yyjson_mut_val *obj,
+                                                  const char *key,
+                                                  size_t len,
+                                                  const char *new_key,
+                                                  size_t new_len);
+
 
 
 /*==============================================================================
- * JSON Pointer API
+ * JSON Pointer API (RFC 6901)
  * https://tools.ietf.org/html/rfc6901
  *============================================================================*/
 
-/** Get a JSON value with JSON Pointer (RFC 6901).
-    The `ptr` should be a null-terminated UTF-8 string.
-    
-    Returns NULL if there's no matched value.
-    Returns NULL if `val/ptr` is NULL or `val` is not object. */
-yyjson_api_inline yyjson_val *yyjson_get_pointer(yyjson_val *val,
-                                                 const char *ptr);
+/** JSON Pointer error code. */
+typedef uint32_t yyjson_ptr_code;
 
-/** Get a JSON value with JSON Pointer (RFC 6901).
-    The `ptr` should be a UTF-8 string, null-terminator is not required.
-    The `len` should be the length of the `ptr`, in bytes.
-    
-    Returns NULL if there's no matched value.
-    Returns NULL if `val/ptr` is NULL or `val` is not object. */
-yyjson_api_inline yyjson_val *yyjson_get_pointern(yyjson_val *val,
-                                                  const char *ptr,
-                                                  size_t len);
+/** No JSON pointer error. */
+static const yyjson_ptr_code YYJSON_PTR_ERR_NONE = 0;
 
-/** Get a JSON value with JSON Pointer (RFC 6901).
-    The `ptr` should be a null-terminated UTF-8 string.
-    
-    Returns NULL if there's no matched value. */
-yyjson_api_inline yyjson_val *yyjson_doc_get_pointer(yyjson_doc *doc,
-                                                     const char *ptr);
+/** Invalid input parameter, such as NULL input. */
+static const yyjson_ptr_code YYJSON_PTR_ERR_PARAMETER = 1;
+
+/** JSON pointer syntax error, such as invalid escape, token no prefix. */
+static const yyjson_ptr_code YYJSON_PTR_ERR_SYNTAX = 2;
+
+/** JSON pointer resolve failed, such as index out of range, key not found. */
+static const yyjson_ptr_code YYJSON_PTR_ERR_RESOLVE = 3;
+
+/** Document's root is NULL, but it is required for the function call. */
+static const yyjson_ptr_code YYJSON_PTR_ERR_NULL_ROOT = 4;
+
+/** Cannot set root as the target is not a document. */
+static const yyjson_ptr_code YYJSON_PTR_ERR_SET_ROOT = 5;
+
+/** The memory allocation failed and a new value could not be created. */
+static const yyjson_ptr_code YYJSON_PTR_ERR_MEMORY_ALLOCATION = 6;
+
+/** Error information for JSON pointer. */
+typedef struct yyjson_ptr_err {
+    /** Error code, see `yyjson_ptr_code` for all possible values. */
+    yyjson_ptr_code code;
+    /** Error message, constant, no need to free (NULL if no error). */
+    const char *msg;
+    /** Error byte position for input JSON pointer (0 if no error). */
+    size_t pos;
+} yyjson_ptr_err;
 
-/** Get a JSON value with JSON Pointer (RFC 6901).
-    The `ptr` should be a UTF-8 string, null-terminator is not required.
-    The `len` should be the length of the `ptr`, in bytes.
+/**
+ A context for JSON pointer operation.
  
-    Returns NULL if there's no matched value. */
-yyjson_api_inline yyjson_val *yyjson_doc_get_pointern(yyjson_doc *doc,
-                                                     const char *ptr,
-                                                      size_t len);
+ This struct stores the context of JSON Pointer operation result. The struct
+ can be used with three helper functions: `ctx_append()`, `ctx_replace()`, and
+ `ctx_remove()`, which perform the corresponding operations on the container
+ without re-parsing the JSON Pointer.
+ 
+ For example:
+ @code
+    // doc before: {"a":[0,1,null]}
+    // ptr: "/a/2"
+    val = yyjson_mut_doc_ptr_getx(doc, ptr, strlen(ptr), &ctx, &err);
+    if (yyjson_is_null(val)) {
+        yyjson_ptr_ctx_remove(&ctx);
+    }
+    // doc after: {"a":[0,1]}
+ @endcode
+ */
+typedef struct yyjson_ptr_ctx {
+    /**
+     The container (parent) of the target value. It can be either an array or
+     an object. If the target location has no value, but all its parent
+     containers exist, and the target location can be used to insert a new
+     value, then `ctn` is the parent container of the target location.
+     Otherwise, `ctn` is NULL.
+     */
+    yyjson_mut_val *ctn;
+    /**
+     The previous sibling of the target value. It can be either a value in an
+     array or a key in an object. As the container is a `circular linked list`
+     of elements, `pre` is the previous node of the target value. If the
+     operation is `add` or `set`, then `pre` is the previous node of the new
+     value, not the original target value. If the target value does not exist,
+     `pre` is NULL.
+     */
+    yyjson_mut_val *pre;
+    /**
+     The removed value if the operation is `set`, `replace` or `remove`. It can
+     be used to restore the original state of the document if needed.
+     */
+    yyjson_mut_val *old;
+} yyjson_ptr_ctx;
 
-/** Get a JSON value with JSON Pointer (RFC 6901).
-    The `ptr` should be a null-terminated UTF-8 string.
-    
-    Returns NULL if there's no matched value. */
-yyjson_api_inline yyjson_mut_val *yyjson_mut_get_pointer(yyjson_mut_val *val,
+/**
+ Get value by a JSON Pointer.
+ @param doc The JSON document to be queried.
+ @param ptr The JSON pointer string (UTF-8 with null-terminator).
+ @return The value referenced by the JSON pointer.
+    NULL if `doc` or `ptr` is NULL, or the JSON pointer cannot be resolved.
+ */
+yyjson_api_inline yyjson_val *yyjson_doc_ptr_get(yyjson_doc *doc,
+                                                 const char *ptr);
+
+/**
+ Get value by a JSON Pointer.
+ @param doc The JSON document to be queried.
+ @param ptr The JSON pointer string (UTF-8, null-terminator is not required).
+ @param len The length of `ptr` in bytes.
+ @return The value referenced by the JSON pointer.
+    NULL if `doc` or `ptr` is NULL, or the JSON pointer cannot be resolved.
+ */
+yyjson_api_inline yyjson_val *yyjson_doc_ptr_getn(yyjson_doc *doc,
+                                                  const char *ptr, size_t len);
+
+/**
+ Get value by a JSON Pointer.
+ @param doc The JSON document to be queried.
+ @param ptr The JSON pointer string (UTF-8, null-terminator is not required).
+ @param len The length of `ptr` in bytes.
+ @param err A pointer to store the error information, or NULL if not needed.
+ @return The value referenced by the JSON pointer.
+    NULL if `doc` or `ptr` is NULL, or the JSON pointer cannot be resolved.
+ */
+yyjson_api_inline yyjson_val *yyjson_doc_ptr_getx(yyjson_doc *doc,
+                                                  const char *ptr, size_t len,
+                                                  yyjson_ptr_err *err);
+
+/**
+ Get value by a JSON Pointer.
+ @param val The JSON value to be queried.
+ @param ptr The JSON pointer string (UTF-8 with null-terminator).
+ @return The value referenced by the JSON pointer.
+    NULL if `val` or `ptr` is NULL, or the JSON pointer cannot be resolved.
+ */
+yyjson_api_inline yyjson_val *yyjson_ptr_get(yyjson_val *val,
+                                             const char *ptr);
+
+/**
+ Get value by a JSON Pointer.
+ @param val The JSON value to be queried.
+ @param ptr The JSON pointer string (UTF-8, null-terminator is not required).
+ @param len The length of `ptr` in bytes.
+ @return The value referenced by the JSON pointer.
+    NULL if `val` or `ptr` is NULL, or the JSON pointer cannot be resolved.
+ */
+yyjson_api_inline yyjson_val *yyjson_ptr_getn(yyjson_val *val,
+                                              const char *ptr, size_t len);
+
+/**
+ Get value by a JSON Pointer.
+ @param val The JSON value to be queried.
+ @param ptr The JSON pointer string (UTF-8, null-terminator is not required).
+ @param len The length of `ptr` in bytes.
+ @param err A pointer to store the error information, or NULL if not needed.
+ @return The value referenced by the JSON pointer.
+    NULL if `val` or `ptr` is NULL, or the JSON pointer cannot be resolved.
+ */
+yyjson_api_inline yyjson_val *yyjson_ptr_getx(yyjson_val *val,
+                                              const char *ptr, size_t len,
+                                              yyjson_ptr_err *err);
+
+/**
+ Get value by a JSON Pointer.
+ @param doc The JSON document to be queried.
+ @param ptr The JSON pointer string (UTF-8 with null-terminator).
+ @return The value referenced by the JSON pointer.
+    NULL if `doc` or `ptr` is NULL, or the JSON pointer cannot be resolved.
+ */
+yyjson_api_inline yyjson_mut_val *yyjson_mut_doc_ptr_get(yyjson_mut_doc *doc,
                                                          const char *ptr);
 
-/** Get a JSON value with JSON Pointer (RFC 6901).
-    The `ptr` should be a UTF-8 string, null-terminator is not required.
-    The `len` should be the length of the `ptr`, in bytes.
-    
-    Returns NULL if there's no matched value. */
-yyjson_api_inline yyjson_mut_val *yyjson_mut_get_pointern(yyjson_mut_val *val,
+/**
+ Get value by a JSON Pointer.
+ @param doc The JSON document to be queried.
+ @param ptr The JSON pointer string (UTF-8, null-terminator is not required).
+ @param len The length of `ptr` in bytes.
+ @return The value referenced by the JSON pointer.
+    NULL if `doc` or `ptr` is NULL, or the JSON pointer cannot be resolved.
+ */
+yyjson_api_inline yyjson_mut_val *yyjson_mut_doc_ptr_getn(yyjson_mut_doc *doc,
                                                           const char *ptr,
                                                           size_t len);
 
-/** Get a JSON value with JSON Pointer (RFC 6901).
-    The `ptr` should be a null-terminated UTF-8 string.
-    
-    Returns NULL if there's no matched value. */
-yyjson_api_inline yyjson_mut_val *yyjson_mut_doc_get_pointer(
+/**
+ Get value by a JSON Pointer.
+ @param doc The JSON document to be queried.
+ @param ptr The JSON pointer string (UTF-8, null-terminator is not required).
+ @param len The length of `ptr` in bytes.
+ @param ctx A pointer to store the result context, or NULL if not needed.
+ @param err A pointer to store the error information, or NULL if not needed.
+ @return The value referenced by the JSON pointer.
+    NULL if `doc` or `ptr` is NULL, or the JSON pointer cannot be resolved.
+ */
+yyjson_api_inline yyjson_mut_val *yyjson_mut_doc_ptr_getx(yyjson_mut_doc *doc,
+                                                          const char *ptr,
+                                                          size_t len,
+                                                          yyjson_ptr_ctx *ctx,
+                                                          yyjson_ptr_err *err);
+
+/**
+ Get value by a JSON Pointer.
+ @param val The JSON value to be queried.
+ @param ptr The JSON pointer string (UTF-8 with null-terminator).
+ @return The value referenced by the JSON pointer.
+    NULL if `val` or `ptr` is NULL, or the JSON pointer cannot be resolved.
+ */
+yyjson_api_inline yyjson_mut_val *yyjson_mut_ptr_get(yyjson_mut_val *val,
+                                                     const char *ptr);
+
+/**
+ Get value by a JSON Pointer.
+ @param val The JSON value to be queried.
+ @param ptr The JSON pointer string (UTF-8, null-terminator is not required).
+ @param len The length of `ptr` in bytes.
+ @return The value referenced by the JSON pointer.
+    NULL if `val` or `ptr` is NULL, or the JSON pointer cannot be resolved.
+ */
+yyjson_api_inline yyjson_mut_val *yyjson_mut_ptr_getn(yyjson_mut_val *val,
+                                                      const char *ptr,
+                                                      size_t len);
+
+/**
+ Get value by a JSON Pointer.
+ @param val The JSON value to be queried.
+ @param ptr The JSON pointer string (UTF-8, null-terminator is not required).
+ @param len The length of `ptr` in bytes.
+ @param ctx A pointer to store the result context, or NULL if not needed.
+ @param err A pointer to store the error information, or NULL if not needed.
+ @return The value referenced by the JSON pointer.
+    NULL if `val` or `ptr` is NULL, or the JSON pointer cannot be resolved.
+ */
+yyjson_api_inline yyjson_mut_val *yyjson_mut_ptr_getx(yyjson_mut_val *val,
+                                                      const char *ptr,
+                                                      size_t len,
+                                                      yyjson_ptr_ctx *ctx,
+                                                      yyjson_ptr_err *err);
+
+/**
+ Add (insert) value by a JSON pointer.
+ @param doc The target JSON document.
+ @param ptr The JSON pointer string (UTF-8 with null-terminator).
+ @param new_val The value to be added.
+ @return true if JSON pointer is valid and new value is added, false otherwise.
+ @note The parent nodes will be created if they do not exist.
+ */
+yyjson_api_inline bool yyjson_mut_doc_ptr_add(yyjson_mut_doc *doc,
+                                              const char *ptr,
+                                              yyjson_mut_val *new_val);
+
+/**
+ Add (insert) value by a JSON pointer.
+ @param doc The target JSON document.
+ @param ptr The JSON pointer string (UTF-8, null-terminator is not required).
+ @param len The length of `ptr` in bytes.
+ @param new_val The value to be added.
+ @return true if JSON pointer is valid and new value is added, false otherwise.
+ @note The parent nodes will be created if they do not exist.
+ */
+yyjson_api_inline bool yyjson_mut_doc_ptr_addn(yyjson_mut_doc *doc,
+                                               const char *ptr, size_t len,
+                                               yyjson_mut_val *new_val);
+
+/**
+ Add (insert) value by a JSON pointer.
+ @param doc The target JSON document.
+ @param ptr The JSON pointer string (UTF-8, null-terminator is not required).
+ @param len The length of `ptr` in bytes.
+ @param new_val The value to be added.
+ @param create_parent Whether to create parent nodes if not exist.
+ @param ctx A pointer to store the result context, or NULL if not needed.
+ @param err A pointer to store the error information, or NULL if not needed.
+ @return true if JSON pointer is valid and new value is added, false otherwise.
+ */
+yyjson_api_inline bool yyjson_mut_doc_ptr_addx(yyjson_mut_doc *doc,
+                                               const char *ptr, size_t len,
+                                               yyjson_mut_val *new_val,
+                                               bool create_parent,
+                                               yyjson_ptr_ctx *ctx,
+                                               yyjson_ptr_err *err);
+
+/**
+ Add (insert) value by a JSON pointer.
+ @param val The target JSON value.
+ @param ptr The JSON pointer string (UTF-8 with null-terminator).
+ @param doc Only used to create new values when needed.
+ @param new_val The value to be added.
+ @return true if JSON pointer is valid and new value is added, false otherwise.
+ @note The parent nodes will be created if they do not exist.
+ */
+yyjson_api_inline bool yyjson_mut_ptr_add(yyjson_mut_val *val,
+                                          const char *ptr,
+                                          yyjson_mut_val *new_val,
+                                          yyjson_mut_doc *doc);
+
+/**
+ Add (insert) value by a JSON pointer.
+ @param val The target JSON value.
+ @param ptr The JSON pointer string (UTF-8, null-terminator is not required).
+ @param len The length of `ptr` in bytes.
+ @param doc Only used to create new values when needed.
+ @param new_val The value to be added.
+ @return true if JSON pointer is valid and new value is added, false otherwise.
+ @note The parent nodes will be created if they do not exist.
+ */
+yyjson_api_inline bool yyjson_mut_ptr_addn(yyjson_mut_val *val,
+                                           const char *ptr, size_t len,
+                                           yyjson_mut_val *new_val,
+                                           yyjson_mut_doc *doc);
+
+/**
+ Add (insert) value by a JSON pointer.
+ @param val The target JSON value.
+ @param ptr The JSON pointer string (UTF-8, null-terminator is not required).
+ @param len The length of `ptr` in bytes.
+ @param doc Only used to create new values when needed.
+ @param new_val The value to be added.
+ @param create_parent Whether to create parent nodes if not exist.
+ @param ctx A pointer to store the result context, or NULL if not needed.
+ @param err A pointer to store the error information, or NULL if not needed.
+ @return true if JSON pointer is valid and new value is added, false otherwise.
+ */
+yyjson_api_inline bool yyjson_mut_ptr_addx(yyjson_mut_val *val,
+                                           const char *ptr, size_t len,
+                                           yyjson_mut_val *new_val,
+                                           yyjson_mut_doc *doc,
+                                           bool create_parent,
+                                           yyjson_ptr_ctx *ctx,
+                                           yyjson_ptr_err *err);
+
+/**
+ Set value by a JSON pointer.
+ @param doc The target JSON document.
+ @param ptr The JSON pointer string (UTF-8 with null-terminator).
+ @param new_val The value to be set, pass NULL to remove.
+ @return true if JSON pointer is valid and new value is set, false otherwise.
+ @note The parent nodes will be created if they do not exist.
+    If the target value already exists, it will be replaced by the new value.
+ */
+yyjson_api_inline bool yyjson_mut_doc_ptr_set(yyjson_mut_doc *doc,
+                                              const char *ptr,
+                                              yyjson_mut_val *new_val);
+
+/**
+ Set value by a JSON pointer.
+ @param doc The target JSON document.
+ @param ptr The JSON pointer string (UTF-8, null-terminator is not required).
+ @param len The length of `ptr` in bytes.
+ @param new_val The value to be set, pass NULL to remove.
+ @return true if JSON pointer is valid and new value is set, false otherwise.
+ @note The parent nodes will be created if they do not exist.
+    If the target value already exists, it will be replaced by the new value.
+ */
+yyjson_api_inline bool yyjson_mut_doc_ptr_setn(yyjson_mut_doc *doc,
+                                               const char *ptr, size_t len,
+                                               yyjson_mut_val *new_val);
+
+/**
+ Set value by a JSON pointer.
+ @param doc The target JSON document.
+ @param ptr The JSON pointer string (UTF-8, null-terminator is not required).
+ @param len The length of `ptr` in bytes.
+ @param new_val The value to be set, pass NULL to remove.
+ @param create_parent Whether to create parent nodes if not exist.
+ @param ctx A pointer to store the result context, or NULL if not needed.
+ @param err A pointer to store the error information, or NULL if not needed.
+ @return true if JSON pointer is valid and new value is set, false otherwise.
+ @note If the target value already exists, it will be replaced by the new value.
+ */
+yyjson_api_inline bool yyjson_mut_doc_ptr_setx(yyjson_mut_doc *doc,
+                                               const char *ptr, size_t len,
+                                               yyjson_mut_val *new_val,
+                                               bool create_parent,
+                                               yyjson_ptr_ctx *ctx,
+                                               yyjson_ptr_err *err);
+
+/**
+ Set value by a JSON pointer.
+ @param val The target JSON value.
+ @param ptr The JSON pointer string (UTF-8 with null-terminator).
+ @param new_val The value to be set, pass NULL to remove.
+ @param doc Only used to create new values when needed.
+ @return true if JSON pointer is valid and new value is set, false otherwise.
+ @note The parent nodes will be created if they do not exist.
+    If the target value already exists, it will be replaced by the new value.
+ */
+yyjson_api_inline bool yyjson_mut_ptr_set(yyjson_mut_val *val,
+                                          const char *ptr,
+                                          yyjson_mut_val *new_val,
+                                          yyjson_mut_doc *doc);
+
+/**
+ Set value by a JSON pointer.
+ @param val The target JSON value.
+ @param ptr The JSON pointer string (UTF-8, null-terminator is not required).
+ @param len The length of `ptr` in bytes.
+ @param new_val The value to be set, pass NULL to remove.
+ @param doc Only used to create new values when needed.
+ @return true if JSON pointer is valid and new value is set, false otherwise.
+ @note The parent nodes will be created if they do not exist.
+    If the target value already exists, it will be replaced by the new value.
+ */
+yyjson_api_inline bool yyjson_mut_ptr_setn(yyjson_mut_val *val,
+                                           const char *ptr, size_t len,
+                                           yyjson_mut_val *new_val,
+                                           yyjson_mut_doc *doc);
+
+/**
+ Set value by a JSON pointer.
+ @param val The target JSON value.
+ @param ptr The JSON pointer string (UTF-8, null-terminator is not required).
+ @param len The length of `ptr` in bytes.
+ @param new_val The value to be set, pass NULL to remove.
+ @param doc Only used to create new values when needed.
+ @param create_parent Whether to create parent nodes if not exist.
+ @param ctx A pointer to store the result context, or NULL if not needed.
+ @param err A pointer to store the error information, or NULL if not needed.
+ @return true if JSON pointer is valid and new value is set, false otherwise.
+ @note If the target value already exists, it will be replaced by the new value.
+ */
+yyjson_api_inline bool yyjson_mut_ptr_setx(yyjson_mut_val *val,
+                                           const char *ptr, size_t len,
+                                           yyjson_mut_val *new_val,
+                                           yyjson_mut_doc *doc,
+                                           bool create_parent,
+                                           yyjson_ptr_ctx *ctx,
+                                           yyjson_ptr_err *err);
+
+/**
+ Replace value by a JSON pointer.
+ @param doc The target JSON document.
+ @param ptr The JSON pointer string (UTF-8 with null-terminator).
+ @param new_val The new value to replace the old one.
+ @return The old value that was replaced, or NULL if not found.
+ */
+yyjson_api_inline yyjson_mut_val *yyjson_mut_doc_ptr_replace(
+    yyjson_mut_doc *doc, const char *ptr, yyjson_mut_val *new_val);
+
+/**
+ Replace value by a JSON pointer.
+ @param doc The target JSON document.
+ @param ptr The JSON pointer string (UTF-8, null-terminator is not required).
+ @param len The length of `ptr` in bytes.
+ @param new_val The new value to replace the old one.
+ @return The old value that was replaced, or NULL if not found.
+ */
+yyjson_api_inline yyjson_mut_val *yyjson_mut_doc_ptr_replacen(
+    yyjson_mut_doc *doc, const char *ptr, size_t len, yyjson_mut_val *new_val);
+
+/**
+ Replace value by a JSON pointer.
+ @param doc The target JSON document.
+ @param ptr The JSON pointer string (UTF-8, null-terminator is not required).
+ @param len The length of `ptr` in bytes.
+ @param new_val The new value to replace the old one.
+ @param ctx A pointer to store the result context, or NULL if not needed.
+ @param err A pointer to store the error information, or NULL if not needed.
+ @return The old value that was replaced, or NULL if not found.
+ */
+yyjson_api_inline yyjson_mut_val *yyjson_mut_doc_ptr_replacex(
+    yyjson_mut_doc *doc, const char *ptr, size_t len, yyjson_mut_val *new_val,
+    yyjson_ptr_ctx *ctx, yyjson_ptr_err *err);
+
+/**
+ Replace value by a JSON pointer.
+ @param val The target JSON value.
+ @param ptr The JSON pointer string (UTF-8 with null-terminator).
+ @param new_val The new value to replace the old one.
+ @return The old value that was replaced, or NULL if not found.
+ */
+yyjson_api_inline yyjson_mut_val *yyjson_mut_ptr_replace(
+    yyjson_mut_val *val, const char *ptr, yyjson_mut_val *new_val);
+
+/**
+ Replace value by a JSON pointer.
+ @param val The target JSON value.
+ @param ptr The JSON pointer string (UTF-8, null-terminator is not required).
+ @param len The length of `ptr` in bytes.
+ @param new_val The new value to replace the old one.
+ @return The old value that was replaced, or NULL if not found.
+ */
+yyjson_api_inline yyjson_mut_val *yyjson_mut_ptr_replacen(
+    yyjson_mut_val *val, const char *ptr, size_t len, yyjson_mut_val *new_val);
+
+/**
+ Replace value by a JSON pointer.
+ @param val The target JSON value.
+ @param ptr The JSON pointer string (UTF-8, null-terminator is not required).
+ @param len The length of `ptr` in bytes.
+ @param new_val The new value to replace the old one.
+ @param ctx A pointer to store the result context, or NULL if not needed.
+ @param err A pointer to store the error information, or NULL if not needed.
+ @return The old value that was replaced, or NULL if not found.
+ */
+yyjson_api_inline yyjson_mut_val *yyjson_mut_ptr_replacex(
+    yyjson_mut_val *val, const char *ptr, size_t len, yyjson_mut_val *new_val,
+    yyjson_ptr_ctx *ctx, yyjson_ptr_err *err);
+
+/**
+ Remove value by a JSON pointer.
+ @param doc The target JSON document.
+ @param ptr The JSON pointer string (UTF-8 with null-terminator).
+ @return The removed value, or NULL on error.
+ */
+yyjson_api_inline yyjson_mut_val *yyjson_mut_doc_ptr_remove(
     yyjson_mut_doc *doc, const char *ptr);
 
-/** Get a JSON value with JSON Pointer (RFC 6901).
-    The `ptr` should be a UTF-8 string, null-terminator is not required.
-    The `len` should be the length of the `ptr`, in bytes.
-    
-    Returns NULL if there's no matched value. */
-yyjson_api_inline yyjson_mut_val *yyjson_mut_doc_get_pointern(
+/**
+ Remove value by a JSON pointer.
+ @param doc The target JSON document.
+ @param ptr The JSON pointer string (UTF-8, null-terminator is not required).
+ @param len The length of `ptr` in bytes.
+ @return The removed value, or NULL on error.
+ */
+yyjson_api_inline yyjson_mut_val *yyjson_mut_doc_ptr_removen(
     yyjson_mut_doc *doc, const char *ptr, size_t len);
 
+/**
+ Remove value by a JSON pointer.
+ @param doc The target JSON document.
+ @param ptr The JSON pointer string (UTF-8, null-terminator is not required).
+ @param len The length of `ptr` in bytes.
+ @param ctx A pointer to store the result context, or NULL if not needed.
+ @param err A pointer to store the error information, or NULL if not needed.
+ @return The removed value, or NULL on error.
+ */
+yyjson_api_inline yyjson_mut_val *yyjson_mut_doc_ptr_removex(
+    yyjson_mut_doc *doc, const char *ptr, size_t len,
+    yyjson_ptr_ctx *ctx, yyjson_ptr_err *err);
+
+/**
+ Remove value by a JSON pointer.
+ @param val The target JSON value.
+ @param ptr The JSON pointer string (UTF-8 with null-terminator).
+ @return The removed value, or NULL on error.
+ */
+yyjson_api_inline yyjson_mut_val *yyjson_mut_ptr_remove(yyjson_mut_val *val,
+                                                        const char *ptr);
+
+/**
+ Remove value by a JSON pointer.
+ @param val The target JSON value.
+ @param ptr The JSON pointer string (UTF-8, null-terminator is not required).
+ @param len The length of `ptr` in bytes.
+ @return The removed value, or NULL on error.
+ */
+yyjson_api_inline yyjson_mut_val *yyjson_mut_ptr_removen(yyjson_mut_val *val,
+                                                         const char *ptr,
+                                                         size_t len);
+
+/**
+ Remove value by a JSON pointer.
+ @param val The target JSON value.
+ @param ptr The JSON pointer string (UTF-8, null-terminator is not required).
+ @param len The length of `ptr` in bytes.
+ @param ctx A pointer to store the result context, or NULL if not needed.
+ @param err A pointer to store the error information, or NULL if not needed.
+ @return The removed value, or NULL on error.
+ */
+yyjson_api_inline yyjson_mut_val *yyjson_mut_ptr_removex(yyjson_mut_val *val,
+                                                         const char *ptr,
+                                                         size_t len,
+                                                         yyjson_ptr_ctx *ctx,
+                                                         yyjson_ptr_err *err);
+
+/**
+ Append value by JSON pointer context.
+ @param ctx The context from the `yyjson_mut_ptr_xxx()` calls.
+ @param key New key if `ctx->ctn` is object, or NULL if `ctx->ctn` is array.
+ @param val New value to be added.
+ @return true on success or false on fail.
+ */
+yyjson_api_inline bool yyjson_ptr_ctx_append(yyjson_ptr_ctx *ctx,
+                                             yyjson_mut_val *key,
+                                             yyjson_mut_val *val);
+
+/**
+ Replace value by JSON pointer context.
+ @param ctx The context from the `yyjson_mut_ptr_xxx()` calls.
+ @param val New value to be replaced.
+ @return true on success or false on fail.
+ @note If success, the old value will be returned via `ctx->old`.
+ */
+yyjson_api_inline bool yyjson_ptr_ctx_replace(yyjson_ptr_ctx *ctx,
+                                              yyjson_mut_val *val);
+
+/**
+ Remove value by JSON pointer context.
+ @param ctx The context from the `yyjson_mut_ptr_xxx()` calls.
+ @return true on success or false on fail.
+ @note If success, the old value will be returned via `ctx->old`.
+ */
+yyjson_api_inline bool yyjson_ptr_ctx_remove(yyjson_ptr_ctx *ctx);
+
 
 
 /*==============================================================================
- * JSON Merge-Patch API
+ * JSON Patch API (RFC 6902)
+ * https://tools.ietf.org/html/rfc6902
+ *============================================================================*/
+
+/** Result code for JSON patch. */
+typedef uint32_t yyjson_patch_code;
+
+/** Success, no error. */
+static const yyjson_patch_code YYJSON_PATCH_SUCCESS = 0;
+
+/** Invalid parameter, such as NULL input or non-array patch. */
+static const yyjson_patch_code YYJSON_PATCH_ERROR_INVALID_PARAMETER = 1;
+
+/** Memory allocation failure occurs. */
+static const yyjson_patch_code YYJSON_PATCH_ERROR_MEMORY_ALLOCATION = 2;
+
+/** JSON patch operation is not object type. */
+static const yyjson_patch_code YYJSON_PATCH_ERROR_INVALID_OPERATION = 3;
+
+/** JSON patch operation is missing a required key. */
+static const yyjson_patch_code YYJSON_PATCH_ERROR_MISSING_KEY = 4;
+
+/** JSON patch operation member is invalid. */
+static const yyjson_patch_code YYJSON_PATCH_ERROR_INVALID_MEMBER = 5;
+
+/** JSON patch operation `test` not equal. */
+static const yyjson_patch_code YYJSON_PATCH_ERROR_EQUAL = 6;
+
+/** JSON patch operation failed on JSON pointer. */
+static const yyjson_patch_code YYJSON_PATCH_ERROR_POINTER = 7;
+
+/** Error information for JSON patch. */
+typedef struct yyjson_patch_err {
+    /** Error code, see `yyjson_patch_code` for all possible values. */
+    yyjson_patch_code code;
+    /** Index of the error operation (0 if no error). */
+    size_t idx;
+    /** Error message, constant, no need to free (NULL if no error). */
+    const char *msg;
+    /** JSON pointer error if `code == YYJSON_PATCH_ERROR_POINTER`. */
+    yyjson_ptr_err ptr;
+} yyjson_patch_err;
+
+/**
+ Creates and returns a patched JSON value (RFC 6902).
+ The memory of the returned value is allocated by the `doc`.
+ The `err` is used to receive error information, pass NULL if not needed.
+ Returns NULL if the patch could not be applied.
+ */
+yyjson_api yyjson_mut_val *yyjson_patch(yyjson_mut_doc *doc,
+                                        yyjson_val *orig,
+                                        yyjson_val *patch,
+                                        yyjson_patch_err *err);
+
+/**
+ Creates and returns a patched JSON value (RFC 6902).
+ The memory of the returned value is allocated by the `doc`.
+ The `err` is used to receive error information, pass NULL if not needed.
+ Returns NULL if the patch could not be applied.
+ */
+yyjson_api yyjson_mut_val *yyjson_mut_patch(yyjson_mut_doc *doc,
+                                            yyjson_mut_val *orig,
+                                            yyjson_mut_val *patch,
+                                            yyjson_patch_err *err);
+
+
+
+/*==============================================================================
+ * JSON Merge-Patch API (RFC 7386)
  * https://tools.ietf.org/html/rfc7386
  *============================================================================*/
 
-/** Creates and returns a merge-patched JSON value (RFC 7386).
-    The memory of the returned value is allocated by the `doc`.
-    Returns NULL if the patch could not be applied.
-    
-    @warning This function is recursive and may cause a stack overflow if the
-        object level is too deep. */
+/**
+ Creates and returns a merge-patched JSON value (RFC 7386).
+ The memory of the returned value is allocated by the `doc`.
+ Returns NULL if the patch could not be applied.
+
+ @warning This function is recursive and may cause a stack overflow if the
+    object level is too deep.
+ */
 yyjson_api yyjson_mut_val *yyjson_merge_patch(yyjson_mut_doc *doc,
                                               yyjson_val *orig,
                                               yyjson_val *patch);
 
-/** Creates and returns a merge-patched JSON value (RFC 7386).
-    The memory of the returned value is allocated by the `doc`.
-    Returns NULL if the patch could not be applied.
-    
-    @warning This function is recursive and may cause a stack overflow if the
-        object level is too deep. */
+/**
+ Creates and returns a merge-patched JSON value (RFC 7386).
+ The memory of the returned value is allocated by the `doc`.
+ Returns NULL if the patch could not be applied.
+
+ @warning This function is recursive and may cause a stack overflow if the
+    object level is too deep.
+ */
 yyjson_api yyjson_mut_val *yyjson_mut_merge_patch(yyjson_mut_doc *doc,
                                                   yyjson_mut_val *orig,
                                                   yyjson_mut_val *patch);
 
 
 
 /*==============================================================================
@@ -3396,28 +4355,44 @@
     return (int)((yyjson_val *)val)->uni.i64;
 }
 
 yyjson_api_inline double unsafe_yyjson_get_real(void *val) {
     return ((yyjson_val *)val)->uni.f64;
 }
 
+yyjson_api_inline double unsafe_yyjson_get_num(void *val) {
+    uint8_t tag = unsafe_yyjson_get_tag(val);
+    if (tag == (YYJSON_TYPE_NUM | YYJSON_SUBTYPE_REAL)) {
+        return ((yyjson_val *)val)->uni.f64;
+    } else if (tag == (YYJSON_TYPE_NUM | YYJSON_SUBTYPE_SINT)) {
+        return (double)((yyjson_val *)val)->uni.i64;
+    } else if (tag == (YYJSON_TYPE_NUM | YYJSON_SUBTYPE_UINT)) {
+#if YYJSON_U64_TO_F64_NO_IMPL
+        uint64_t msb = ((uint64_t)1) << 63;
+        uint64_t num = ((yyjson_val *)val)->uni.u64;
+        if ((num & msb) == 0) {
+            return (double)(int64_t)num;
+        } else {
+            return ((double)(int64_t)((num >> 1) | (num & 1))) * (double)2.0;
+        }
+#else
+        return (double)((yyjson_val *)val)->uni.u64;
+#endif
+    }
+    return 0.0;
+}
+
 yyjson_api_inline const char *unsafe_yyjson_get_str(void *val) {
     return ((yyjson_val *)val)->uni.str;
 }
 
 yyjson_api_inline size_t unsafe_yyjson_get_len(void *val) {
     return (size_t)(((yyjson_val *)val)->tag >> YYJSON_TAG_BIT);
 }
 
-yyjson_api_inline void unsafe_yyjson_set_len(void *val, size_t len) {
-    uint64_t tag = ((yyjson_val *)val)->tag & YYJSON_TAG_MASK;
-    tag |= (uint64_t)len << YYJSON_TAG_BIT;
-    ((yyjson_val *)val)->tag = tag;
-}
-
 yyjson_api_inline yyjson_val *unsafe_yyjson_get_first(yyjson_val *ctn) {
     return ctn + 1;
 }
 
 yyjson_api_inline yyjson_val *unsafe_yyjson_get_next(yyjson_val *val) {
     bool is_ctn = unsafe_yyjson_is_ctn(val);
     size_t ctn_ofs = val->uni.ofs;
@@ -3432,14 +4407,93 @@
     memcmp(((yyjson_val *)val)->uni.str, str, len) == 0;
 }
 
 yyjson_api_inline bool unsafe_yyjson_equals_str(void *val, const char *str) {
     return unsafe_yyjson_equals_strn(val, str, strlen(str));
 }
 
+yyjson_api_inline void unsafe_yyjson_set_type(void *val, yyjson_type type,
+                                              yyjson_subtype subtype) {
+    uint8_t tag = (type | subtype);
+    uint64_t new_tag = ((yyjson_val *)val)->tag;
+    new_tag = (new_tag & (~(uint64_t)YYJSON_TAG_MASK)) | (uint64_t)tag;
+    ((yyjson_val *)val)->tag = new_tag;
+}
+
+yyjson_api_inline void unsafe_yyjson_set_len(void *val, size_t len) {
+    uint64_t tag = ((yyjson_val *)val)->tag & YYJSON_TAG_MASK;
+    tag |= (uint64_t)len << YYJSON_TAG_BIT;
+    ((yyjson_val *)val)->tag = tag;
+}
+
+yyjson_api_inline void unsafe_yyjson_inc_len(void *val) {
+    uint64_t tag = ((yyjson_val *)val)->tag;
+    tag += (uint64_t)(1 << YYJSON_TAG_BIT);
+    ((yyjson_val *)val)->tag = tag;
+}
+
+yyjson_api_inline void unsafe_yyjson_set_raw(void *val, const char *raw,
+                                             size_t len) {
+    unsafe_yyjson_set_type(val, YYJSON_TYPE_RAW, YYJSON_SUBTYPE_NONE);
+    unsafe_yyjson_set_len(val, len);
+    ((yyjson_val *)val)->uni.str = raw;
+}
+
+yyjson_api_inline void unsafe_yyjson_set_null(void *val) {
+    unsafe_yyjson_set_type(val, YYJSON_TYPE_NULL, YYJSON_SUBTYPE_NONE);
+    unsafe_yyjson_set_len(val, 0);
+}
+
+yyjson_api_inline void unsafe_yyjson_set_bool(void *val, bool num) {
+    yyjson_subtype subtype = num ? YYJSON_SUBTYPE_TRUE : YYJSON_SUBTYPE_FALSE;
+    unsafe_yyjson_set_type(val, YYJSON_TYPE_BOOL, subtype);
+    unsafe_yyjson_set_len(val, 0);
+}
+
+yyjson_api_inline void unsafe_yyjson_set_uint(void *val, uint64_t num) {
+    unsafe_yyjson_set_type(val, YYJSON_TYPE_NUM, YYJSON_SUBTYPE_UINT);
+    unsafe_yyjson_set_len(val, 0);
+    ((yyjson_val *)val)->uni.u64 = num;
+}
+
+yyjson_api_inline void unsafe_yyjson_set_sint(void *val, int64_t num) {
+    unsafe_yyjson_set_type(val, YYJSON_TYPE_NUM, YYJSON_SUBTYPE_SINT);
+    unsafe_yyjson_set_len(val, 0);
+    ((yyjson_val *)val)->uni.i64 = num;
+}
+
+yyjson_api_inline void unsafe_yyjson_set_real(void *val, double num) {
+    unsafe_yyjson_set_type(val, YYJSON_TYPE_NUM, YYJSON_SUBTYPE_REAL);
+    unsafe_yyjson_set_len(val, 0);
+    ((yyjson_val *)val)->uni.f64 = num;
+}
+
+yyjson_api_inline void unsafe_yyjson_set_str(void *val, const char *str) {
+    unsafe_yyjson_set_type(val, YYJSON_TYPE_STR, YYJSON_SUBTYPE_NONE);
+    unsafe_yyjson_set_len(val, strlen(str));
+    ((yyjson_val *)val)->uni.str = str;
+}
+
+yyjson_api_inline void unsafe_yyjson_set_strn(void *val, const char *str,
+                                              size_t len) {
+    unsafe_yyjson_set_type(val, YYJSON_TYPE_STR, YYJSON_SUBTYPE_NONE);
+    unsafe_yyjson_set_len(val, len);
+    ((yyjson_val *)val)->uni.str = str;
+}
+
+yyjson_api_inline void unsafe_yyjson_set_arr(void *val, size_t size) {
+    unsafe_yyjson_set_type(val, YYJSON_TYPE_ARR, YYJSON_SUBTYPE_NONE);
+    unsafe_yyjson_set_len(val, size);
+}
+
+yyjson_api_inline void unsafe_yyjson_set_obj(void *val, size_t size) {
+    unsafe_yyjson_set_type(val, YYJSON_TYPE_OBJ, YYJSON_SUBTYPE_NONE);
+    unsafe_yyjson_set_len(val, size);
+}
+
 
 
 /*==============================================================================
  * JSON Document API (Implementation)
  *============================================================================*/
 
 yyjson_api_inline yyjson_val *yyjson_doc_get_root(yyjson_doc *doc) {
@@ -3578,14 +4632,18 @@
     return yyjson_is_int(val) ? unsafe_yyjson_get_int(val) : 0;
 }
 
 yyjson_api_inline double yyjson_get_real(yyjson_val *val) {
     return yyjson_is_real(val) ? unsafe_yyjson_get_real(val) : 0.0;
 }
 
+yyjson_api_inline double yyjson_get_num(yyjson_val *val) {
+    return val ? unsafe_yyjson_get_num(val) : 0.0;
+}
+
 yyjson_api_inline const char *yyjson_get_str(yyjson_val *val) {
     return yyjson_is_str(val) ? unsafe_yyjson_get_str(val) : NULL;
 }
 
 yyjson_api_inline size_t yyjson_get_len(yyjson_val *val) {
     return val ? unsafe_yyjson_get_len(val) : 0;
 }
@@ -3604,20 +4662,76 @@
     }
     return false;
 }
 
 yyjson_api bool unsafe_yyjson_equals(yyjson_val *lhs, yyjson_val *rhs);
 
 yyjson_api_inline bool yyjson_equals(yyjson_val *lhs, yyjson_val *rhs) {
-    if (yyjson_unlikely(!lhs || !rhs))
-        return false;
-    
+    if (yyjson_unlikely(!lhs || !rhs)) return false;
     return unsafe_yyjson_equals(lhs, rhs);
 }
 
+yyjson_api_inline bool yyjson_set_raw(yyjson_val *val,
+                                      const char *raw, size_t len) {
+    if (yyjson_unlikely(!val || unsafe_yyjson_is_ctn(val))) return false;
+    unsafe_yyjson_set_raw(val, raw, len);
+    return true;
+}
+
+yyjson_api_inline bool yyjson_set_null(yyjson_val *val) {
+    if (yyjson_unlikely(!val || unsafe_yyjson_is_ctn(val))) return false;
+    unsafe_yyjson_set_null(val);
+    return true;
+}
+
+yyjson_api_inline bool yyjson_set_bool(yyjson_val *val, bool num) {
+    if (yyjson_unlikely(!val || unsafe_yyjson_is_ctn(val))) return false;
+    unsafe_yyjson_set_bool(val, num);
+    return true;
+}
+
+yyjson_api_inline bool yyjson_set_uint(yyjson_val *val, uint64_t num) {
+    if (yyjson_unlikely(!val || unsafe_yyjson_is_ctn(val))) return false;
+    unsafe_yyjson_set_uint(val, num);
+    return true;
+}
+
+yyjson_api_inline bool yyjson_set_sint(yyjson_val *val, int64_t num) {
+    if (yyjson_unlikely(!val || unsafe_yyjson_is_ctn(val))) return false;
+    unsafe_yyjson_set_sint(val, num);
+    return true;
+}
+
+yyjson_api_inline bool yyjson_set_int(yyjson_val *val, int num) {
+    if (yyjson_unlikely(!val || unsafe_yyjson_is_ctn(val))) return false;
+    unsafe_yyjson_set_sint(val, (int64_t)num);
+    return true;
+}
+
+yyjson_api_inline bool yyjson_set_real(yyjson_val *val, double num) {
+    if (yyjson_unlikely(!val || unsafe_yyjson_is_ctn(val))) return false;
+    unsafe_yyjson_set_real(val, num);
+    return true;
+}
+
+yyjson_api_inline bool yyjson_set_str(yyjson_val *val, const char *str) {
+    if (yyjson_unlikely(!val || unsafe_yyjson_is_ctn(val))) return false;
+    if (yyjson_unlikely(!str)) return false;
+    unsafe_yyjson_set_str(val, str);
+    return true;
+}
+
+yyjson_api_inline bool yyjson_set_strn(yyjson_val *val,
+                                       const char *str, size_t len) {
+    if (yyjson_unlikely(!val || unsafe_yyjson_is_ctn(val))) return false;
+    if (yyjson_unlikely(!str)) return false;
+    unsafe_yyjson_set_strn(val, str, len);
+    return true;
+}
+
 
 
 /*==============================================================================
  * JSON Array API (Implementation)
  *============================================================================*/
 
 yyjson_api_inline size_t yyjson_arr_size(yyjson_val *arr) {
@@ -3666,32 +4780,32 @@
 
 
 
 /*==============================================================================
  * JSON Array Iterator API (Implementation)
  *============================================================================*/
 
-struct yyjson_arr_iter {
-    size_t idx; /**< current index, from 0 */
-    size_t max; /**< maximum index, idx < max */
-    yyjson_val *cur; /**< current value */
-};
-
 yyjson_api_inline bool yyjson_arr_iter_init(yyjson_val *arr,
                                             yyjson_arr_iter *iter) {
     if (yyjson_likely(yyjson_is_arr(arr) && iter)) {
         iter->idx = 0;
         iter->max = unsafe_yyjson_get_len(arr);
         iter->cur = unsafe_yyjson_get_first(arr);
         return true;
     }
     if (iter) memset(iter, 0, sizeof(yyjson_arr_iter));
     return false;
 }
 
+yyjson_api_inline yyjson_arr_iter yyjson_arr_iter_with(yyjson_val *arr) {
+    yyjson_arr_iter iter;
+    yyjson_arr_iter_init(arr, &iter);
+    return iter;
+}
+
 yyjson_api_inline bool yyjson_arr_iter_has_next(yyjson_arr_iter *iter) {
     return iter ? iter->idx < iter->max : false;
 }
 
 yyjson_api_inline yyjson_val *yyjson_arr_iter_next(yyjson_arr_iter *iter) {
     yyjson_val *val;
     if (iter && iter->idx < iter->max) {
@@ -3738,34 +4852,33 @@
 
 
 
 /*==============================================================================
  * JSON Object Iterator API (Implementation)
  *============================================================================*/
 
-struct yyjson_obj_iter {
-    size_t idx; /**< current key index, from 0 */
-    size_t max; /**< maximum key index, idx < max */
-    yyjson_val *cur; /**< current key */
-    yyjson_val *obj; /**< the object being iterated */
-};
-
 yyjson_api_inline bool yyjson_obj_iter_init(yyjson_val *obj,
                                             yyjson_obj_iter *iter) {
     if (yyjson_likely(yyjson_is_obj(obj) && iter)) {
         iter->idx = 0;
         iter->max = unsafe_yyjson_get_len(obj);
         iter->cur = unsafe_yyjson_get_first(obj);
         iter->obj = obj;
         return true;
     }
     if (iter) memset(iter, 0, sizeof(yyjson_obj_iter));
     return false;
 }
 
+yyjson_api_inline yyjson_obj_iter yyjson_obj_iter_with(yyjson_val *obj) {
+    yyjson_obj_iter iter;
+    yyjson_obj_iter_init(obj, &iter);
+    return iter;
+}
+
 yyjson_api_inline bool yyjson_obj_iter_has_next(yyjson_obj_iter *iter) {
     return iter ? iter->idx < iter->max : false;
 }
 
 yyjson_api_inline yyjson_val *yyjson_obj_iter_next(yyjson_obj_iter *iter) {
     if (iter && iter->idx < iter->max) {
         yyjson_val *key = iter->cur;
@@ -3832,16 +4945,17 @@
     yyjson_mut_val *next; /**< the next value in circular linked list */
 };
 
 /**
  A memory chunk in string memory pool.
  */
 typedef struct yyjson_str_chunk {
-    struct yyjson_str_chunk *next;
-    /* flexible array member here */
+    struct yyjson_str_chunk *next; /* next chunk linked list */
+    size_t chunk_size; /* chunk size in bytes */
+    /* char str[]; flexible array member */
 } yyjson_str_chunk;
 
 /**
  A memory pool to hold all strings in a mutable document.
  */
 typedef struct yyjson_str_pool {
     char *cur; /* cursor inside current chunk */
@@ -3849,18 +4963,21 @@
     size_t chunk_size; /* chunk size in bytes while creating new chunk */
     size_t chunk_size_max; /* maximum chunk size in bytes */
     yyjson_str_chunk *chunks; /* a linked list of chunks, nullable */
 } yyjson_str_pool;
 
 /**
  A memory chunk in value memory pool.
+ `sizeof(yyjson_val_chunk)` should not larger than `sizeof(yyjson_mut_val)`.
  */
 typedef struct yyjson_val_chunk {
-    struct yyjson_val_chunk *next;
-    /* flexible array member here */
+    struct yyjson_val_chunk *next; /* next chunk linked list */
+    size_t chunk_size; /* chunk size in bytes */
+    /* char pad[sizeof(yyjson_mut_val) - sizeof(yyjson_val_chunk)]; padding */
+    /* yyjson_mut_val vals[]; flexible array member */
 } yyjson_val_chunk;
 
 /**
  A memory pool to hold all values in a mutable document.
  */
 typedef struct yyjson_val_pool {
     yyjson_mut_val *cur; /* cursor inside current chunk */
@@ -3875,35 +4992,42 @@
     yyjson_alc alc; /**< a valid allocator, nonnull */
     yyjson_str_pool str_pool; /**< string memory pool */
     yyjson_val_pool val_pool; /**< value memory pool */
 };
 
 /* Ensures the capacity to at least equal to the specified byte length. */
 yyjson_api bool unsafe_yyjson_str_pool_grow(yyjson_str_pool *pool,
-                                            yyjson_alc *alc, size_t len);
+                                            const yyjson_alc *alc,
+                                            size_t len);
 
 /* Ensures the capacity to at least equal to the specified value count. */
 yyjson_api bool unsafe_yyjson_val_pool_grow(yyjson_val_pool *pool,
-                                            yyjson_alc *alc, size_t count);
+                                            const yyjson_alc *alc,
+                                            size_t count);
 
-yyjson_api_inline char *unsafe_yyjson_mut_strncpy(yyjson_mut_doc *doc,
-                                                  const char *str, size_t len) {
+/* Allocate memory for string. */
+yyjson_api_inline char *unsafe_yyjson_mut_str_alc(yyjson_mut_doc *doc,
+                                                  size_t len) {
     char *mem;
-    yyjson_alc *alc = &doc->alc;
+    const yyjson_alc *alc = &doc->alc;
     yyjson_str_pool *pool = &doc->str_pool;
-    
-    if (!str) return NULL;
     if (yyjson_unlikely((size_t)(pool->end - pool->cur) <= len)) {
         if (yyjson_unlikely(!unsafe_yyjson_str_pool_grow(pool, alc, len + 1))) {
             return NULL;
         }
     }
-    
     mem = pool->cur;
     pool->cur = mem + len + 1;
+    return mem;
+}
+
+yyjson_api_inline char *unsafe_yyjson_mut_strncpy(yyjson_mut_doc *doc,
+                                                  const char *str, size_t len) {
+    char *mem = unsafe_yyjson_mut_str_alc(doc, len);
+    if (yyjson_unlikely(!mem)) return NULL;
     memcpy((void *)mem, (const void *)str, len);
     mem[len] = '\0';
     return mem;
 }
 
 yyjson_api_inline yyjson_mut_val *unsafe_yyjson_mut_val(yyjson_mut_doc *doc,
                                                         size_t count) {
@@ -3911,15 +5035,14 @@
     yyjson_alc *alc = &doc->alc;
     yyjson_val_pool *pool = &doc->val_pool;
     if (yyjson_unlikely((size_t)(pool->end - pool->cur) < count)) {
         if (yyjson_unlikely(!unsafe_yyjson_val_pool_grow(pool, alc, count))) {
             return NULL;
         }
     }
-    
     val = pool->cur;
     pool->cur += count;
     return val;
 }
 
 
 
@@ -4040,14 +5163,18 @@
     return yyjson_get_int((yyjson_val *)val);
 }
 
 yyjson_api_inline double yyjson_mut_get_real(yyjson_mut_val *val) {
     return yyjson_get_real((yyjson_val *)val);
 }
 
+yyjson_api_inline double yyjson_mut_get_num(yyjson_mut_val *val) {
+    return yyjson_get_num((yyjson_val *)val);
+}
+
 yyjson_api_inline const char *yyjson_mut_get_str(yyjson_mut_val *val) {
     return yyjson_get_str((yyjson_val *)val);
 }
 
 yyjson_api_inline size_t yyjson_mut_get_len(yyjson_mut_val *val) {
     return yyjson_get_len((yyjson_val *)val);
 }
@@ -4067,14 +5194,83 @@
 
 yyjson_api_inline bool yyjson_mut_equals(yyjson_mut_val *lhs,
                                          yyjson_mut_val *rhs) {
     if (yyjson_unlikely(!lhs || !rhs)) return false;
     return unsafe_yyjson_mut_equals(lhs, rhs);
 }
 
+yyjson_api_inline bool yyjson_mut_set_raw(yyjson_mut_val *val,
+                                          const char *raw, size_t len) {
+    if (yyjson_unlikely(!val || !raw)) return false;
+    unsafe_yyjson_set_raw(val, raw, len);
+    return true;
+}
+
+yyjson_api_inline bool yyjson_mut_set_null(yyjson_mut_val *val) {
+    if (yyjson_unlikely(!val)) return false;
+    unsafe_yyjson_set_null(val);
+    return true;
+}
+
+yyjson_api_inline bool yyjson_mut_set_bool(yyjson_mut_val *val, bool num) {
+    if (yyjson_unlikely(!val)) return false;
+    unsafe_yyjson_set_bool(val, num);
+    return true;
+}
+
+yyjson_api_inline bool yyjson_mut_set_uint(yyjson_mut_val *val, uint64_t num) {
+    if (yyjson_unlikely(!val)) return false;
+    unsafe_yyjson_set_uint(val, num);
+    return true;
+}
+
+yyjson_api_inline bool yyjson_mut_set_sint(yyjson_mut_val *val, int64_t num) {
+    if (yyjson_unlikely(!val)) return false;
+    unsafe_yyjson_set_sint(val, num);
+    return true;
+}
+
+yyjson_api_inline bool yyjson_mut_set_int(yyjson_mut_val *val, int num) {
+    if (yyjson_unlikely(!val)) return false;
+    unsafe_yyjson_set_sint(val, (int64_t)num);
+    return true;
+}
+
+yyjson_api_inline bool yyjson_mut_set_real(yyjson_mut_val *val, double num) {
+    if (yyjson_unlikely(!val)) return false;
+    unsafe_yyjson_set_real(val, num);
+    return true;
+}
+
+yyjson_api_inline bool yyjson_mut_set_str(yyjson_mut_val *val,
+                                          const char *str) {
+    if (yyjson_unlikely(!val || !str)) return false;
+    unsafe_yyjson_set_str(val, str);
+    return true;
+}
+
+yyjson_api_inline bool yyjson_mut_set_strn(yyjson_mut_val *val,
+                                           const char *str, size_t len) {
+    if (yyjson_unlikely(!val || !str)) return false;
+    unsafe_yyjson_set_strn(val, str, len);
+    return true;
+}
+
+yyjson_api_inline bool yyjson_mut_set_arr(yyjson_mut_val *val) {
+    if (yyjson_unlikely(!val)) return false;
+    unsafe_yyjson_set_arr(val, 0);
+    return true;
+}
+
+yyjson_api_inline bool yyjson_mut_set_obj(yyjson_mut_val *val) {
+    if (yyjson_unlikely(!val)) return false;
+    unsafe_yyjson_set_obj(val, 0);
+    return true;
+}
+
 
 
 /*==============================================================================
  * Mutable JSON Value Creation API (Implementation)
  *============================================================================*/
 
 yyjson_api_inline yyjson_mut_val *yyjson_mut_raw(yyjson_mut_doc *doc,
@@ -4286,36 +5482,35 @@
 
 
 
 /*==============================================================================
  * Mutable JSON Array Iterator API (Implementation)
  *============================================================================*/
 
-struct yyjson_mut_arr_iter {
-    size_t idx; /**< current index, from 0 */
-    size_t max; /**< maximum index, idx < max */
-    yyjson_mut_val *cur; /**< current value */
-    yyjson_mut_val *pre; /**< previous value */
-    yyjson_mut_val *arr; /**< the array being iterated */
-};
-
 yyjson_api_inline bool yyjson_mut_arr_iter_init(yyjson_mut_val *arr,
                                                 yyjson_mut_arr_iter *iter) {
     if (yyjson_likely(yyjson_mut_is_arr(arr) && iter)) {
         iter->idx = 0;
         iter->max = unsafe_yyjson_get_len(arr);
         iter->cur = iter->max ? (yyjson_mut_val *)arr->uni.ptr : NULL;
         iter->pre = NULL;
         iter->arr = arr;
         return true;
     }
     if (iter) memset(iter, 0, sizeof(yyjson_mut_arr_iter));
     return false;
 }
 
+yyjson_api_inline yyjson_mut_arr_iter yyjson_mut_arr_iter_with(
+    yyjson_mut_val *arr) {
+    yyjson_mut_arr_iter iter;
+    yyjson_mut_arr_iter_init(arr, &iter);
+    return iter;
+}
+
 yyjson_api_inline bool yyjson_mut_arr_iter_has_next(yyjson_mut_arr_iter *iter) {
     return iter ? iter->idx < iter->max : false;
 }
 
 yyjson_api_inline yyjson_mut_val *yyjson_mut_arr_iter_next(
     yyjson_mut_arr_iter *iter) {
     if (iter && iter->idx < iter->max) {
@@ -4926,36 +6121,35 @@
 
 
 
 /*==============================================================================
  * Mutable JSON Object Iterator API (Implementation)
  *============================================================================*/
 
-struct yyjson_mut_obj_iter {
-    size_t idx; /**< current key index, from 0 */
-    size_t max; /**< maximum key index, idx < max */
-    yyjson_mut_val *cur; /**< current key */
-    yyjson_mut_val *pre; /**< previous key */
-    yyjson_mut_val *obj; /**< the object being iterated */
-};
-
 yyjson_api_inline bool yyjson_mut_obj_iter_init(yyjson_mut_val *obj,
                                                 yyjson_mut_obj_iter *iter) {
     if (yyjson_likely(yyjson_mut_is_obj(obj) && iter)) {
         iter->idx = 0;
         iter->max = unsafe_yyjson_get_len(obj);
         iter->cur = iter->max ? (yyjson_mut_val *)obj->uni.ptr : NULL;
         iter->pre = NULL;
         iter->obj = obj;
         return true;
     }
     if (iter) memset(iter, 0, sizeof(yyjson_mut_obj_iter));
     return false;
 }
 
+yyjson_api_inline yyjson_mut_obj_iter yyjson_mut_obj_iter_with(
+    yyjson_mut_val *obj) {
+    yyjson_mut_obj_iter iter;
+    yyjson_mut_obj_iter_init(obj, &iter);
+    return iter;
+}
+
 yyjson_api_inline bool yyjson_mut_obj_iter_has_next(yyjson_mut_obj_iter *iter) {
     return iter ? iter->idx < iter->max : false;
 }
 
 yyjson_api_inline yyjson_mut_val *yyjson_mut_obj_iter_next(
     yyjson_mut_obj_iter *iter) {
     if (iter && iter->idx < iter->max) {
@@ -4980,16 +6174,16 @@
         yyjson_mut_val *cur = iter->cur;
         yyjson_mut_val *next = cur->next->next;
         if (yyjson_unlikely(iter->idx == iter->max)) iter->obj->uni.ptr = prev;
         iter->idx--;
         iter->max--;
         unsafe_yyjson_set_len(iter->obj, iter->max);
         prev->next->next = next;
-        iter->cur = next;
-        return cur;
+        iter->cur = prev;
+        return cur->next;
     }
     return NULL;
 }
 
 yyjson_api_inline yyjson_mut_val *yyjson_mut_obj_iter_get(
     yyjson_mut_obj_iter *iter, const char *key) {
     return yyjson_mut_obj_iter_getn(iter, key, key ? strlen(key) : 0);
@@ -5189,25 +6383,36 @@
     }
     return false;
 }
 
 yyjson_api_inline bool yyjson_mut_obj_put(yyjson_mut_val *obj,
                                           yyjson_mut_val *key,
                                           yyjson_mut_val *val) {
-    if (yyjson_likely(yyjson_mut_is_obj(obj) &&
-                      yyjson_mut_is_str(key))) {
-        unsafe_yyjson_mut_obj_remove(obj, key->uni.str,
-                                     unsafe_yyjson_get_len(key), key->tag);
-        if (yyjson_likely(val)) {
-            unsafe_yyjson_mut_obj_add(obj, key, val,
-                                      unsafe_yyjson_get_len(obj));
+    bool replaced = false;
+    size_t key_len;
+    yyjson_mut_obj_iter iter;
+    yyjson_mut_val *cur_key;
+    if (yyjson_unlikely(!yyjson_mut_is_obj(obj) ||
+                        !yyjson_mut_is_str(key))) return false;
+    key_len = unsafe_yyjson_get_len(key);
+    yyjson_mut_obj_iter_init(obj, &iter);
+    while ((cur_key = yyjson_mut_obj_iter_next(&iter))) {
+        if (key->tag == cur_key->tag &&
+            memcmp(key->uni.str, cur_key->uni.ptr, key_len) == 0) {
+            if (!replaced && val) {
+                replaced = true;
+                val->next = cur_key->next->next;
+                cur_key->next = val;
+            } else {
+                yyjson_mut_obj_iter_remove(&iter);
+            }
         }
-        return true;
     }
-    return false;
+    if (!replaced && val) unsafe_yyjson_mut_obj_add(obj, key, val, iter.max);
+    return true;
 }
 
 yyjson_api_inline bool yyjson_mut_obj_insert(yyjson_mut_val *obj,
                                              yyjson_mut_val *key,
                                              yyjson_mut_val *val,
                                              size_t idx) {
     if (yyjson_likely(yyjson_mut_is_obj(obj) &&
@@ -5459,79 +6664,882 @@
             }
         }
         return val_removed;
     }
     return NULL;
 }
 
+yyjson_api_inline bool yyjson_mut_obj_rename_key(yyjson_mut_doc *doc,
+                                                 yyjson_mut_val *obj,
+                                                 const char *key,
+                                                 const char *new_key) {
+    if (!key || !new_key) return false;
+    return yyjson_mut_obj_rename_keyn(doc, obj, key, strlen(key),
+                                      new_key, strlen(new_key));
+}
+
+yyjson_api_inline bool yyjson_mut_obj_rename_keyn(yyjson_mut_doc *doc,
+                                                  yyjson_mut_val *obj,
+                                                  const char *key,
+                                                  size_t len,
+                                                  const char *new_key,
+                                                  size_t new_len) {
+    char *cpy_key = NULL;
+    yyjson_mut_val *old_key;
+    yyjson_mut_obj_iter iter;
+    if (!doc || !obj || !key || !new_key) return false;
+    yyjson_mut_obj_iter_init(obj, &iter);
+    while ((old_key = yyjson_mut_obj_iter_next(&iter))) {
+        if (unsafe_yyjson_equals_strn((void *)old_key, key, len)) {
+            if (!cpy_key) {
+                cpy_key = unsafe_yyjson_mut_strncpy(doc, new_key, new_len);
+                if (!cpy_key) return false;
+            }
+            yyjson_mut_set_strn(old_key, cpy_key, new_len);
+        }
+    }
+    return cpy_key != NULL;
+}
+
 
 
 /*==============================================================================
  * JSON Pointer API (Implementation)
  *============================================================================*/
 
-/* `val` not null, `ptr` start with '/', `len` > 0. */
-yyjson_api yyjson_val *unsafe_yyjson_get_pointer(yyjson_val *val,
-                                                 const char *ptr,
-                                                 size_t len);
+#define yyjson_ptr_set_err(_code, _msg) do { \
+    if (err) { \
+        err->code = YYJSON_PTR_ERR_##_code; \
+        err->msg = _msg; \
+        err->pos = 0; \
+    } \
+} while(false)
+
+/* require: val != NULL, *ptr == '/', len > 0 */
+yyjson_api yyjson_val *unsafe_yyjson_ptr_getx(yyjson_val *val,
+                                              const char *ptr, size_t len,
+                                              yyjson_ptr_err *err);
 
-/* `val` not null, `ptr` start with '/', `len` > 0. */
-yyjson_api yyjson_mut_val *unsafe_yyjson_mut_get_pointer(yyjson_mut_val *val,
+/* require: val != NULL, *ptr == '/', len > 0 */
+yyjson_api yyjson_mut_val *unsafe_yyjson_mut_ptr_getx(yyjson_mut_val *val,
+                                                      const char *ptr,
+                                                      size_t len,
+                                                      yyjson_ptr_ctx *ctx,
+                                                      yyjson_ptr_err *err);
+
+/* require: val/new_val/doc != NULL, *ptr == '/', len > 0 */
+yyjson_api bool unsafe_yyjson_mut_ptr_putx(yyjson_mut_val *val,
+                                           const char *ptr, size_t len,
+                                           yyjson_mut_val *new_val,
+                                           yyjson_mut_doc *doc,
+                                           bool create_parent, bool insert_new,
+                                           yyjson_ptr_ctx *ctx,
+                                           yyjson_ptr_err *err);
+
+/* require: val/err != NULL, *ptr == '/', len > 0 */
+yyjson_api yyjson_mut_val *unsafe_yyjson_mut_ptr_replacex(
+    yyjson_mut_val *val, const char *ptr, size_t len, yyjson_mut_val *new_val,
+    yyjson_ptr_ctx *ctx, yyjson_ptr_err *err);
+
+/* require: val/err != NULL, *ptr == '/', len > 0 */
+yyjson_api yyjson_mut_val *unsafe_yyjson_mut_ptr_removex(yyjson_mut_val *val,
                                                          const char *ptr,
-                                                         size_t len);
+                                                         size_t len,
+                                                         yyjson_ptr_ctx *ctx,
+                                                         yyjson_ptr_err *err);
 
-yyjson_api_inline yyjson_val *yyjson_get_pointern(yyjson_val *val,
-                                                  const char *ptr,
-                                                  size_t len) {
-    if (!val || !ptr) return NULL;
-    if (len == 0) return val;
-    if (*ptr != '/') return NULL;
-    return unsafe_yyjson_get_pointer(val, ptr, len);
+yyjson_api_inline yyjson_val *yyjson_doc_ptr_get(yyjson_doc *doc,
+                                                 const char *ptr) {
+    if (yyjson_unlikely(!ptr)) return NULL;
+    return yyjson_doc_ptr_getn(doc, ptr, strlen(ptr));
 }
 
-yyjson_api_inline yyjson_val *yyjson_get_pointer(yyjson_val *val,
-                                                 const char *ptr) {
-    if (!val || !ptr) return NULL;
-    return yyjson_get_pointern(val, ptr, strlen(ptr));
+yyjson_api_inline yyjson_val *yyjson_doc_ptr_getn(yyjson_doc *doc,
+                                                  const char *ptr, size_t len) {
+    return yyjson_doc_ptr_getx(doc, ptr, len, NULL);
 }
 
-yyjson_api_inline yyjson_val *yyjson_doc_get_pointern(yyjson_doc *doc,
+yyjson_api_inline yyjson_val *yyjson_doc_ptr_getx(yyjson_doc *doc,
+                                                  const char *ptr, size_t len,
+                                                  yyjson_ptr_err *err) {
+    yyjson_ptr_set_err(NONE, NULL);
+    if (yyjson_unlikely(!doc || !ptr)) {
+        yyjson_ptr_set_err(PARAMETER, "input parameter is NULL");
+        return NULL;
+    }
+    if (yyjson_unlikely(!doc->root)) {
+        yyjson_ptr_set_err(NULL_ROOT, "document's root is NULL");
+        return NULL;
+    }
+    if (yyjson_unlikely(len == 0)) {
+        return doc->root;
+    }
+    if (yyjson_unlikely(*ptr != '/')) {
+        yyjson_ptr_set_err(SYNTAX, "no prefix '/'");
+        return NULL;
+    }
+    return unsafe_yyjson_ptr_getx(doc->root, ptr, len, err);
+}
+
+yyjson_api_inline yyjson_val *yyjson_ptr_get(yyjson_val *val,
+                                             const char *ptr) {
+    if (yyjson_unlikely(!ptr)) return NULL;
+    return yyjson_ptr_getn(val, ptr, strlen(ptr));
+}
+
+yyjson_api_inline yyjson_val *yyjson_ptr_getn(yyjson_val *val,
+                                              const char *ptr, size_t len) {
+    return yyjson_ptr_getx(val, ptr, len, NULL);
+}
+
+yyjson_api_inline yyjson_val *yyjson_ptr_getx(yyjson_val *val,
+                                              const char *ptr, size_t len,
+                                              yyjson_ptr_err *err) {
+    yyjson_ptr_set_err(NONE, NULL);
+    if (yyjson_unlikely(!val || !ptr)) {
+        yyjson_ptr_set_err(PARAMETER, "input parameter is NULL");
+        return NULL;
+    }
+    if (yyjson_unlikely(len == 0)) {
+        return val;
+    }
+    if (yyjson_unlikely(*ptr != '/')) {
+        yyjson_ptr_set_err(SYNTAX, "no prefix '/'");
+        return NULL;
+    }
+    return unsafe_yyjson_ptr_getx(val, ptr, len, err);
+}
+
+yyjson_api_inline yyjson_mut_val *yyjson_mut_doc_ptr_get(yyjson_mut_doc *doc,
+                                                         const char *ptr) {
+    if (!ptr) return NULL;
+    return yyjson_mut_doc_ptr_getn(doc, ptr, strlen(ptr));
+}
+
+yyjson_api_inline yyjson_mut_val *yyjson_mut_doc_ptr_getn(yyjson_mut_doc *doc,
+                                                          const char *ptr,
+                                                          size_t len) {
+    return yyjson_mut_doc_ptr_getx(doc, ptr, len, NULL, NULL);
+}
+
+yyjson_api_inline yyjson_mut_val *yyjson_mut_doc_ptr_getx(yyjson_mut_doc *doc,
+                                                          const char *ptr,
+                                                          size_t len,
+                                                          yyjson_ptr_ctx *ctx,
+                                                          yyjson_ptr_err *err) {
+    yyjson_ptr_set_err(NONE, NULL);
+    if (ctx) memset(ctx, 0, sizeof(*ctx));
+    
+    if (yyjson_unlikely(!doc || !ptr)) {
+        yyjson_ptr_set_err(PARAMETER, "input parameter is NULL");
+        return NULL;
+    }
+    if (yyjson_unlikely(!doc->root)) {
+        yyjson_ptr_set_err(NULL_ROOT, "document's root is NULL");
+        return NULL;
+    }
+    if (yyjson_unlikely(len == 0)) {
+        return doc->root;
+    }
+    if (yyjson_unlikely(*ptr != '/')) {
+        yyjson_ptr_set_err(SYNTAX, "no prefix '/'");
+        return NULL;
+    }
+    return unsafe_yyjson_mut_ptr_getx(doc->root, ptr, len, ctx, err);
+}
+
+yyjson_api_inline yyjson_mut_val *yyjson_mut_ptr_get(yyjson_mut_val *val,
+                                                     const char *ptr) {
+    if (!ptr) return NULL;
+    return yyjson_mut_ptr_getn(val, ptr, strlen(ptr));
+}
+
+yyjson_api_inline yyjson_mut_val *yyjson_mut_ptr_getn(yyjson_mut_val *val,
                                                       const char *ptr,
                                                       size_t len) {
-    return yyjson_get_pointern(doc ? doc->root : NULL, ptr, len);
+    return yyjson_mut_ptr_getx(val, ptr, len, NULL, NULL);
+}
+
+yyjson_api_inline yyjson_mut_val *yyjson_mut_ptr_getx(yyjson_mut_val *val,
+                                                      const char *ptr,
+                                                      size_t len,
+                                                      yyjson_ptr_ctx *ctx,
+                                                      yyjson_ptr_err *err) {
+    yyjson_ptr_set_err(NONE, NULL);
+    if (ctx) memset(ctx, 0, sizeof(*ctx));
+    
+    if (yyjson_unlikely(!val || !ptr)) {
+        yyjson_ptr_set_err(PARAMETER, "input parameter is NULL");
+        return NULL;
+    }
+    if (yyjson_unlikely(len == 0)) {
+        return val;
+    }
+    if (yyjson_unlikely(*ptr != '/')) {
+        yyjson_ptr_set_err(SYNTAX, "no prefix '/'");
+        return NULL;
+    }
+    return unsafe_yyjson_mut_ptr_getx(val, ptr, len, ctx, err);
+}
+
+yyjson_api_inline bool yyjson_mut_doc_ptr_add(yyjson_mut_doc *doc,
+                                              const char *ptr,
+                                              yyjson_mut_val *new_val) {
+    if (yyjson_unlikely(!ptr)) return false;
+    return yyjson_mut_doc_ptr_addn(doc, ptr, strlen(ptr), new_val);
+}
+
+yyjson_api_inline bool yyjson_mut_doc_ptr_addn(yyjson_mut_doc *doc,
+                                               const char *ptr,
+                                               size_t len,
+                                               yyjson_mut_val *new_val) {
+    return yyjson_mut_doc_ptr_addx(doc, ptr, len, new_val, true, NULL, NULL);
+}
+
+yyjson_api_inline bool yyjson_mut_doc_ptr_addx(yyjson_mut_doc *doc,
+                                               const char *ptr, size_t len,
+                                               yyjson_mut_val *new_val,
+                                               bool create_parent,
+                                               yyjson_ptr_ctx *ctx,
+                                               yyjson_ptr_err *err) {
+    yyjson_ptr_set_err(NONE, NULL);
+    if (ctx) memset(ctx, 0, sizeof(*ctx));
+    
+    if (yyjson_unlikely(!doc || !ptr || !new_val)) {
+        yyjson_ptr_set_err(PARAMETER, "input parameter is NULL");
+        return false;
+    }
+    if (yyjson_unlikely(len == 0)) {
+        if (doc->root) {
+            yyjson_ptr_set_err(SET_ROOT, "cannot set document's root");
+            return false;
+        } else {
+            doc->root = new_val;
+            return true;
+        }
+    }
+    if (yyjson_unlikely(*ptr != '/')) {
+        yyjson_ptr_set_err(SYNTAX, "no prefix '/'");
+        return false;
+    }
+    if (yyjson_unlikely(!doc->root && !create_parent)) {
+        yyjson_ptr_set_err(NULL_ROOT, "document's root is NULL");
+        return false;
+    }
+    if (yyjson_unlikely(!doc->root)) {
+        yyjson_mut_val *root = yyjson_mut_obj(doc);
+        if (yyjson_unlikely(!root)) {
+            yyjson_ptr_set_err(MEMORY_ALLOCATION, "failed to create value");
+            return false;
+        }
+        if (unsafe_yyjson_mut_ptr_putx(root, ptr, len, new_val, doc,
+                                       create_parent, true, ctx, err)) {
+            doc->root = root;
+            return true;
+        }
+        return false;
+    }
+    return unsafe_yyjson_mut_ptr_putx(doc->root, ptr, len, new_val, doc,
+                                      create_parent, true, ctx, err);
 }
 
+yyjson_api_inline bool yyjson_mut_ptr_add(yyjson_mut_val *val,
+                                          const char *ptr,
+                                          yyjson_mut_val *new_val,
+                                          yyjson_mut_doc *doc) {
+    if (yyjson_unlikely(!ptr)) return false;
+    return yyjson_mut_ptr_addn(val, ptr, strlen(ptr), new_val, doc);
+}
+
+yyjson_api_inline bool yyjson_mut_ptr_addn(yyjson_mut_val *val,
+                                           const char *ptr, size_t len,
+                                           yyjson_mut_val *new_val,
+                                           yyjson_mut_doc *doc) {
+    return yyjson_mut_ptr_addx(val, ptr, len, new_val, doc, true, NULL, NULL);
+}
+
+yyjson_api_inline bool yyjson_mut_ptr_addx(yyjson_mut_val *val,
+                                           const char *ptr, size_t len,
+                                           yyjson_mut_val *new_val,
+                                           yyjson_mut_doc *doc,
+                                           bool create_parent,
+                                           yyjson_ptr_ctx *ctx,
+                                           yyjson_ptr_err *err) {
+    yyjson_ptr_set_err(NONE, NULL);
+    if (ctx) memset(ctx, 0, sizeof(*ctx));
+    
+    if (yyjson_unlikely(!val || !ptr || !new_val || !doc)) {
+        yyjson_ptr_set_err(PARAMETER, "input parameter is NULL");
+        return false;
+    }
+    if (yyjson_unlikely(len == 0)) {
+        yyjson_ptr_set_err(SET_ROOT, "cannot set root");
+        return false;
+    }
+    if (yyjson_unlikely(*ptr != '/')) {
+        yyjson_ptr_set_err(SYNTAX, "no prefix '/'");
+        return false;
+    }
+    return unsafe_yyjson_mut_ptr_putx(val, ptr, len, new_val,
+                                       doc, create_parent, true, ctx, err);
+}
+
+yyjson_api_inline bool yyjson_mut_doc_ptr_set(yyjson_mut_doc *doc,
+                                              const char *ptr,
+                                              yyjson_mut_val *new_val) {
+    if (yyjson_unlikely(!ptr)) return false;
+    return yyjson_mut_doc_ptr_setn(doc, ptr, strlen(ptr), new_val);
+}
+
+yyjson_api_inline bool yyjson_mut_doc_ptr_setn(yyjson_mut_doc *doc,
+                                               const char *ptr, size_t len,
+                                               yyjson_mut_val *new_val) {
+    return yyjson_mut_doc_ptr_setx(doc, ptr, len, new_val, true, NULL, NULL);
+}
+
+yyjson_api_inline bool yyjson_mut_doc_ptr_setx(yyjson_mut_doc *doc,
+                                               const char *ptr, size_t len,
+                                               yyjson_mut_val *new_val,
+                                               bool create_parent,
+                                               yyjson_ptr_ctx *ctx,
+                                               yyjson_ptr_err *err) {
+    yyjson_ptr_set_err(NONE, NULL);
+    if (ctx) memset(ctx, 0, sizeof(*ctx));
+    
+    if (yyjson_unlikely(!doc || !ptr)) {
+        yyjson_ptr_set_err(PARAMETER, "input parameter is NULL");
+        return false;
+    }
+    if (yyjson_unlikely(len == 0)) {
+        if (ctx) ctx->old = doc->root;
+        doc->root = new_val;
+        return true;
+    }
+    if (yyjson_unlikely(*ptr != '/')) {
+        yyjson_ptr_set_err(SYNTAX, "no prefix '/'");
+        return false;
+    }
+    if (!new_val) {
+        if (!doc->root) {
+            yyjson_ptr_set_err(RESOLVE, "JSON pointer cannot be resolved");
+            return false;
+        }
+        return !!unsafe_yyjson_mut_ptr_removex(doc->root, ptr, len, ctx, err);
+    }
+    if (yyjson_unlikely(!doc->root && !create_parent)) {
+        yyjson_ptr_set_err(NULL_ROOT, "document's root is NULL");
+        return false;
+    }
+    if (yyjson_unlikely(!doc->root)) {
+        yyjson_mut_val *root = yyjson_mut_obj(doc);
+        if (yyjson_unlikely(!root)) {
+            yyjson_ptr_set_err(MEMORY_ALLOCATION, "failed to create value");
+            return false;
+        }
+        if (unsafe_yyjson_mut_ptr_putx(root, ptr, len, new_val, doc,
+                                       create_parent, false, ctx, err)) {
+            doc->root = root;
+            return true;
+        }
+        return false;
+    }
+    return unsafe_yyjson_mut_ptr_putx(doc->root, ptr, len, new_val, doc,
+                                      create_parent, false, ctx, err);
+}
+
+yyjson_api_inline bool yyjson_mut_ptr_set(yyjson_mut_val *val,
+                                          const char *ptr,
+                                          yyjson_mut_val *new_val,
+                                          yyjson_mut_doc *doc) {
+    if (yyjson_unlikely(!ptr)) return false;
+    return yyjson_mut_ptr_setn(val, ptr, strlen(ptr), new_val, doc);
+}
+
+yyjson_api_inline bool yyjson_mut_ptr_setn(yyjson_mut_val *val,
+                                           const char *ptr, size_t len,
+                                           yyjson_mut_val *new_val,
+                                           yyjson_mut_doc *doc) {
+    return yyjson_mut_ptr_setx(val, ptr, len, new_val, doc, true, NULL, NULL);
+}
+
+yyjson_api_inline bool yyjson_mut_ptr_setx(yyjson_mut_val *val,
+                                           const char *ptr, size_t len,
+                                           yyjson_mut_val *new_val,
+                                           yyjson_mut_doc *doc,
+                                           bool create_parent,
+                                           yyjson_ptr_ctx *ctx,
+                                           yyjson_ptr_err *err) {
+    yyjson_ptr_set_err(NONE, NULL);
+    if (ctx) memset(ctx, 0, sizeof(*ctx));
+    
+    if (yyjson_unlikely(!val || !ptr || !doc)) {
+        yyjson_ptr_set_err(PARAMETER, "input parameter is NULL");
+        return false;
+    }
+    if (yyjson_unlikely(len == 0)) {
+        yyjson_ptr_set_err(SET_ROOT, "cannot set root");
+        return false;
+    }
+    if (yyjson_unlikely(*ptr != '/')) {
+        yyjson_ptr_set_err(SYNTAX, "no prefix '/'");
+        return false;
+    }
+    if (!new_val) {
+        return !!unsafe_yyjson_mut_ptr_removex(val, ptr, len, ctx, err);
+    }
+    return unsafe_yyjson_mut_ptr_putx(val, ptr, len, new_val, doc,
+                                      create_parent, false, ctx, err);
+}
+
+yyjson_api_inline yyjson_mut_val *yyjson_mut_doc_ptr_replace(
+    yyjson_mut_doc *doc, const char *ptr, yyjson_mut_val *new_val) {
+    if (!ptr) return NULL;
+    return yyjson_mut_doc_ptr_replacen(doc, ptr, strlen(ptr), new_val);
+}
+
+yyjson_api_inline yyjson_mut_val *yyjson_mut_doc_ptr_replacen(
+    yyjson_mut_doc *doc, const char *ptr, size_t len, yyjson_mut_val *new_val) {
+    return yyjson_mut_doc_ptr_replacex(doc, ptr, len, new_val, NULL, NULL);
+}
+
+yyjson_api_inline yyjson_mut_val *yyjson_mut_doc_ptr_replacex(
+    yyjson_mut_doc *doc, const char *ptr, size_t len, yyjson_mut_val *new_val,
+    yyjson_ptr_ctx *ctx, yyjson_ptr_err *err) {
+    
+    yyjson_ptr_set_err(NONE, NULL);
+    if (ctx) memset(ctx, 0, sizeof(*ctx));
+    
+    if (yyjson_unlikely(!doc || !ptr || !new_val)) {
+        yyjson_ptr_set_err(PARAMETER, "input parameter is NULL");
+        return NULL;
+    }
+    if (yyjson_unlikely(len == 0)) {
+        yyjson_mut_val *root = doc->root;
+        if (yyjson_unlikely(!root)) {
+            yyjson_ptr_set_err(RESOLVE, "JSON pointer cannot be resolved");
+            return NULL;
+        }
+        if (ctx) ctx->old = root;
+        doc->root = new_val;
+        return root;
+    }
+    if (yyjson_unlikely(!doc->root)) {
+        yyjson_ptr_set_err(NULL_ROOT, "document's root is NULL");
+        return NULL;
+    }
+    if (yyjson_unlikely(*ptr != '/')) {
+        yyjson_ptr_set_err(SYNTAX, "no prefix '/'");
+        return NULL;
+    }
+    return unsafe_yyjson_mut_ptr_replacex(doc->root, ptr, len, new_val,
+                                          ctx, err);
+}
+
+yyjson_api_inline yyjson_mut_val *yyjson_mut_ptr_replace(
+    yyjson_mut_val *val, const char *ptr, yyjson_mut_val *new_val) {
+    if (!ptr) return NULL;
+    return yyjson_mut_ptr_replacen(val, ptr, strlen(ptr), new_val);
+}
+
+yyjson_api_inline yyjson_mut_val *yyjson_mut_ptr_replacen(
+    yyjson_mut_val *val, const char *ptr, size_t len, yyjson_mut_val *new_val) {
+    return yyjson_mut_ptr_replacex(val, ptr, len, new_val, NULL, NULL);
+}
+
+yyjson_api_inline yyjson_mut_val *yyjson_mut_ptr_replacex(
+    yyjson_mut_val *val, const char *ptr, size_t len, yyjson_mut_val *new_val,
+    yyjson_ptr_ctx *ctx, yyjson_ptr_err *err) {
+    
+    yyjson_ptr_set_err(NONE, NULL);
+    if (ctx) memset(ctx, 0, sizeof(*ctx));
+    
+    if (yyjson_unlikely(!val || !ptr || !new_val)) {
+        yyjson_ptr_set_err(PARAMETER, "input parameter is NULL");
+        return NULL;
+    }
+    if (yyjson_unlikely(len == 0)) {
+        yyjson_ptr_set_err(SET_ROOT, "cannot set root");
+        return NULL;
+    }
+    if (yyjson_unlikely(*ptr != '/')) {
+        yyjson_ptr_set_err(SYNTAX, "no prefix '/'");
+        return NULL;
+    }
+    return unsafe_yyjson_mut_ptr_replacex(val, ptr, len, new_val, ctx, err);
+}
+
+yyjson_api_inline yyjson_mut_val *yyjson_mut_doc_ptr_remove(
+    yyjson_mut_doc *doc, const char *ptr) {
+    if (!ptr) return NULL;
+    return yyjson_mut_doc_ptr_removen(doc, ptr, strlen(ptr));
+}
+
+yyjson_api_inline yyjson_mut_val *yyjson_mut_doc_ptr_removen(
+    yyjson_mut_doc *doc, const char *ptr, size_t len) {
+    return yyjson_mut_doc_ptr_removex(doc, ptr, len, NULL, NULL);
+}
+
+yyjson_api_inline yyjson_mut_val *yyjson_mut_doc_ptr_removex(
+    yyjson_mut_doc *doc, const char *ptr, size_t len,
+    yyjson_ptr_ctx *ctx, yyjson_ptr_err *err) {
+    
+    yyjson_ptr_set_err(NONE, NULL);
+    if (ctx) memset(ctx, 0, sizeof(*ctx));
+    
+    if (yyjson_unlikely(!doc || !ptr)) {
+        yyjson_ptr_set_err(PARAMETER, "input parameter is NULL");
+        return NULL;
+    }
+    if (yyjson_unlikely(!doc->root)) {
+        yyjson_ptr_set_err(NULL_ROOT, "document's root is NULL");
+        return NULL;
+    }
+    if (yyjson_unlikely(len == 0)) {
+        yyjson_mut_val *root = doc->root;
+        if (ctx) ctx->old = root;
+        doc->root = NULL;
+        return root;
+    }
+    if (yyjson_unlikely(*ptr != '/')) {
+        yyjson_ptr_set_err(SYNTAX, "no prefix '/'");
+        return NULL;
+    }
+    return unsafe_yyjson_mut_ptr_removex(doc->root, ptr, len, ctx, err);
+}
+
+yyjson_api_inline yyjson_mut_val *yyjson_mut_ptr_remove(yyjson_mut_val *val,
+                                                        const char *ptr) {
+    if (!ptr) return NULL;
+    return yyjson_mut_ptr_removen(val, ptr, strlen(ptr));
+}
+
+yyjson_api_inline yyjson_mut_val *yyjson_mut_ptr_removen(yyjson_mut_val *val,
+                                                         const char *ptr,
+                                                         size_t len) {
+    return yyjson_mut_ptr_removex(val, ptr, len, NULL, NULL);
+}
+
+yyjson_api_inline yyjson_mut_val *yyjson_mut_ptr_removex(yyjson_mut_val *val,
+                                                         const char *ptr,
+                                                         size_t len,
+                                                         yyjson_ptr_ctx *ctx,
+                                                         yyjson_ptr_err *err) {
+    yyjson_ptr_set_err(NONE, NULL);
+    if (ctx) memset(ctx, 0, sizeof(*ctx));
+    
+    if (yyjson_unlikely(!val || !ptr)) {
+        yyjson_ptr_set_err(PARAMETER, "input parameter is NULL");
+        return NULL;
+    }
+    if (yyjson_unlikely(len == 0)) {
+        yyjson_ptr_set_err(SET_ROOT, "cannot set root");
+        return NULL;
+    }
+    if (yyjson_unlikely(*ptr != '/')) {
+        yyjson_ptr_set_err(SYNTAX, "no prefix '/'");
+        return NULL;
+    }
+    return unsafe_yyjson_mut_ptr_removex(val, ptr, len, ctx, err);
+}
+
+yyjson_api_inline bool yyjson_ptr_ctx_append(yyjson_ptr_ctx *ctx,
+                                             yyjson_mut_val *key,
+                                             yyjson_mut_val *val) {
+    yyjson_mut_val *ctn, *pre_key, *pre_val, *cur_key, *cur_val;
+    if (!ctx || !ctx->ctn || !val) return false;
+    ctn = ctx->ctn;
+    
+    if (yyjson_mut_is_obj(ctn)) {
+        if (!key) return false;
+        key->next = val;
+        pre_key = ctx->pre;
+        if (unsafe_yyjson_get_len(ctn) == 0) {
+            val->next = key;
+            ctn->uni.ptr = key;
+            ctx->pre = key;
+        } else if (!pre_key) {
+            pre_key = (yyjson_mut_val *)ctn->uni.ptr;
+            pre_val = pre_key->next;
+            val->next = pre_val->next;
+            pre_val->next = key;
+            ctn->uni.ptr = key;
+            ctx->pre = pre_key;
+        } else {
+            cur_key = pre_key->next->next;
+            cur_val = cur_key->next;
+            val->next = cur_val->next;
+            cur_val->next = key;
+            if (ctn->uni.ptr == cur_key) ctn->uni.ptr = key;
+            ctx->pre = cur_key;
+        }
+    } else {
+        pre_val = ctx->pre;
+        if (unsafe_yyjson_get_len(ctn) == 0) {
+            val->next = val;
+            ctn->uni.ptr = val;
+            ctx->pre = val;
+        } else if (!pre_val) {
+            pre_val = (yyjson_mut_val *)ctn->uni.ptr;
+            val->next = pre_val->next;
+            pre_val->next = val;
+            ctn->uni.ptr = val;
+            ctx->pre = pre_val;
+        } else {
+            cur_val = pre_val->next;
+            val->next = cur_val->next;
+            cur_val->next = val;
+            if (ctn->uni.ptr == cur_val) ctn->uni.ptr = val;
+            ctx->pre = cur_val;
+        }
+    }
+    unsafe_yyjson_inc_len(ctn);
+    return true;
+}
+
+yyjson_api_inline bool yyjson_ptr_ctx_replace(yyjson_ptr_ctx *ctx,
+                                              yyjson_mut_val *val) {
+    yyjson_mut_val *ctn, *pre_key, *cur_key, *pre_val, *cur_val;
+    if (!ctx || !ctx->ctn || !ctx->pre || !val) return false;
+    ctn = ctx->ctn;
+    if (yyjson_mut_is_obj(ctn)) {
+        pre_key = ctx->pre;
+        pre_val = pre_key->next;
+        cur_key = pre_val->next;
+        cur_val = cur_key->next;
+        /* replace current value */
+        cur_key->next = val;
+        val->next = cur_val->next;
+        ctx->old = cur_val;
+    } else {
+        pre_val = ctx->pre;
+        cur_val = pre_val->next;
+        /* replace current value */
+        if (pre_val != cur_val) {
+            val->next = cur_val->next;
+            pre_val->next = val;
+            if (ctn->uni.ptr == cur_val) ctn->uni.ptr = val;
+        } else {
+            val->next = val;
+            ctn->uni.ptr = val;
+            ctx->pre = val;
+        }
+        ctx->old = cur_val;
+    }
+    return true;
+}
+
+yyjson_api_inline bool yyjson_ptr_ctx_remove(yyjson_ptr_ctx *ctx) {
+    yyjson_mut_val *ctn, *pre_key, *pre_val, *cur_key, *cur_val;
+    size_t len;
+    if (!ctx || !ctx->ctn || !ctx->pre) return false;
+    ctn = ctx->ctn;
+    if (yyjson_mut_is_obj(ctn)) {
+        pre_key = ctx->pre;
+        pre_val = pre_key->next;
+        cur_key = pre_val->next;
+        cur_val = cur_key->next;
+        /* remove current key-value */
+        pre_val->next = cur_val->next;
+        if (ctn->uni.ptr == cur_key) ctn->uni.ptr = pre_key;
+        ctx->pre = NULL;
+        ctx->old = cur_val;
+    } else {
+        pre_val = ctx->pre;
+        cur_val = pre_val->next;
+        /* remove current key-value */
+        pre_val->next = cur_val->next;
+        if (ctn->uni.ptr == cur_val) ctn->uni.ptr = pre_val;
+        ctx->pre = NULL;
+        ctx->old = cur_val;
+    }
+    len = unsafe_yyjson_get_len(ctn) - 1;
+    if (len == 0) ctn->uni.ptr = NULL;
+    unsafe_yyjson_set_len(ctn, len);
+    return true;
+}
+
+#undef yyjson_ptr_set_err
+
+
+
+/*==============================================================================
+ * JSON Value at Pointer API (Implementation)
+ *============================================================================*/
+
+/**
+ Set provided `value` if the JSON Pointer (RFC 6901) exists and is type bool.
+ Returns true if value at `ptr` exists and is the correct type, otherwise false.
+ */
+yyjson_api_inline bool yyjson_ptr_get_bool(
+    yyjson_val *root, const char *ptr, bool *value) {
+    yyjson_val *val = yyjson_ptr_get(root, ptr);
+    if (value && yyjson_is_bool(val)) {
+        *value = unsafe_yyjson_get_bool(val);
+        return true;
+    } else {
+        return false;
+    }
+}
+
+/**
+ Set provided `value` if the JSON Pointer (RFC 6901) exists and is type uint.
+ Returns true if value at `ptr` exists and is the correct type, otherwise false.
+ */
+yyjson_api_inline bool yyjson_ptr_get_uint(
+    yyjson_val *root, const char *ptr, uint64_t *value) {
+    yyjson_val *val = yyjson_ptr_get(root, ptr);
+    if (value && yyjson_is_uint(val)) {
+        *value = unsafe_yyjson_get_uint(val);
+        return true;
+    } else {
+        return false;
+    }
+}
+
+/**
+ Set provided `value` if the JSON Pointer (RFC 6901) exists and is type sint.
+ Returns true if value at `ptr` exists and is the correct type, otherwise false.
+ */
+yyjson_api_inline bool yyjson_ptr_get_sint(
+    yyjson_val *root, const char *ptr, int64_t *value) {
+    yyjson_val *val = yyjson_ptr_get(root, ptr);
+    if (value && yyjson_is_sint(val)) {
+        *value = unsafe_yyjson_get_sint(val);
+        return true;
+    } else {
+        return false;
+    }
+}
+
+/**
+ Set provided `value` if the JSON Pointer (RFC 6901) exists and is type real.
+ Returns true if value at `ptr` exists and is the correct type, otherwise false.
+ */
+yyjson_api_inline bool yyjson_ptr_get_real(
+    yyjson_val *root, const char *ptr, double *value) {
+    yyjson_val *val = yyjson_ptr_get(root, ptr);
+    if (value && yyjson_is_real(val)) {
+        *value = unsafe_yyjson_get_real(val);
+        return true;
+    } else {
+        return false;
+    }
+}
+
+/**
+ Set provided `value` if the JSON Pointer (RFC 6901) exists and is type sint,
+ uint or real.
+ Returns true if value at `ptr` exists and is the correct type, otherwise false.
+ */
+yyjson_api_inline bool yyjson_ptr_get_num(
+    yyjson_val *root, const char *ptr, double *value) {
+    yyjson_val *val = yyjson_ptr_get(root, ptr);
+    if (value && yyjson_is_num(val)) {
+        *value = unsafe_yyjson_get_num(val);
+        return true;
+    } else {
+        return false;
+    }
+}
+
+/**
+ Set provided `value` if the JSON Pointer (RFC 6901) exists and is type string.
+ Returns true if value at `ptr` exists and is the correct type, otherwise false.
+ */
+yyjson_api_inline bool yyjson_ptr_get_str(
+    yyjson_val *root, const char *ptr, const char **value) {
+    yyjson_val *val = yyjson_ptr_get(root, ptr);
+    if (value && yyjson_is_str(val)) {
+        *value = unsafe_yyjson_get_str(val);
+        return true;
+    } else {
+        return false;
+    }
+}
+
+
+
+/*==============================================================================
+ * Deprecated
+ *============================================================================*/
+
+/** @deprecated renamed to `yyjson_doc_ptr_get` */
+yyjson_deprecated("renamed to yyjson_doc_ptr_get")
 yyjson_api_inline yyjson_val *yyjson_doc_get_pointer(yyjson_doc *doc,
                                                      const char *ptr) {
-    return yyjson_get_pointer(doc ? doc->root : NULL, ptr);
+    return yyjson_doc_ptr_get(doc, ptr);
 }
 
-yyjson_api_inline yyjson_mut_val *yyjson_mut_get_pointern(yyjson_mut_val *val,
-                                                          const char *ptr,
-                                                          size_t len) {
-    if (!val || !ptr) return NULL;
-    if (len == 0) return val;
-    if (*ptr != '/') return NULL;
-    return unsafe_yyjson_mut_get_pointer(val, ptr, len);
+/** @deprecated renamed to `yyjson_doc_ptr_getn` */
+yyjson_deprecated("renamed to yyjson_doc_ptr_getn")
+yyjson_api_inline yyjson_val *yyjson_doc_get_pointern(yyjson_doc *doc,
+                                                      const char *ptr,
+                                                      size_t len) {
+    return yyjson_doc_ptr_getn(doc, ptr, len);
 }
 
-yyjson_api_inline yyjson_mut_val *yyjson_mut_get_pointer(yyjson_mut_val *val,
-                                                         const char *ptr) {
-    if (!val || !ptr) return NULL;
-    return yyjson_mut_get_pointern(val, ptr, strlen(ptr));
+/** @deprecated renamed to `yyjson_mut_doc_ptr_get` */
+yyjson_deprecated("renamed to yyjson_mut_doc_ptr_get")
+yyjson_api_inline yyjson_mut_val *yyjson_mut_doc_get_pointer(
+    yyjson_mut_doc *doc, const char *ptr) {
+    return yyjson_mut_doc_ptr_get(doc, ptr);
 }
 
+/** @deprecated renamed to `yyjson_mut_doc_ptr_getn` */
+yyjson_deprecated("renamed to yyjson_mut_doc_ptr_getn")
 yyjson_api_inline yyjson_mut_val *yyjson_mut_doc_get_pointern(
     yyjson_mut_doc *doc, const char *ptr, size_t len) {
-    return yyjson_mut_get_pointern(doc ? doc->root : NULL, ptr, len);
+    return yyjson_mut_doc_ptr_getn(doc, ptr, len);
 }
 
-yyjson_api_inline yyjson_mut_val *yyjson_mut_doc_get_pointer(
-    yyjson_mut_doc *doc, const char *ptr) {
-    return yyjson_mut_get_pointer(doc ? doc->root : NULL, ptr);
+/** @deprecated renamed to `yyjson_ptr_get` */
+yyjson_deprecated("renamed to yyjson_ptr_get")
+yyjson_api_inline yyjson_val *yyjson_get_pointer(yyjson_val *val,
+                                                 const char *ptr) {
+    return yyjson_ptr_get(val, ptr);
+}
+
+/** @deprecated renamed to `yyjson_ptr_getn` */
+yyjson_deprecated("renamed to yyjson_ptr_getn")
+yyjson_api_inline yyjson_val *yyjson_get_pointern(yyjson_val *val,
+                                                  const char *ptr,
+                                                  size_t len) {
+    return yyjson_ptr_getn(val, ptr, len);
+}
+
+/** @deprecated renamed to `yyjson_mut_ptr_get` */
+yyjson_deprecated("renamed to yyjson_mut_ptr_get")
+yyjson_api_inline yyjson_mut_val *yyjson_mut_get_pointer(yyjson_mut_val *val,
+                                                         const char *ptr) {
+    return yyjson_mut_ptr_get(val, ptr);
+}
+
+/** @deprecated renamed to `yyjson_mut_ptr_getn` */
+yyjson_deprecated("renamed to yyjson_mut_ptr_getn")
+yyjson_api_inline yyjson_mut_val *yyjson_mut_get_pointern(yyjson_mut_val *val,
+                                                          const char *ptr,
+                                                          size_t len) {
+    return yyjson_mut_ptr_getn(val, ptr, len);
+}
+
+/** @deprecated renamed to `yyjson_mut_ptr_getn` */
+yyjson_deprecated("renamed to unsafe_yyjson_ptr_getn")
+yyjson_api_inline yyjson_val *unsafe_yyjson_get_pointer(yyjson_val *val,
+                                                        const char *ptr,
+                                                        size_t len) {
+    yyjson_ptr_err err;
+    return unsafe_yyjson_ptr_getx(val, ptr, len, &err);
+}
+
+/** @deprecated renamed to `unsafe_yyjson_mut_ptr_getx` */
+yyjson_deprecated("renamed to unsafe_yyjson_mut_ptr_getx")
+yyjson_api_inline yyjson_mut_val *unsafe_yyjson_mut_get_pointer(
+    yyjson_mut_val *val, const char *ptr, size_t len) {
+    yyjson_ptr_err err;
+    return unsafe_yyjson_mut_ptr_getx(val, ptr, len, NULL, &err);
 }
 
 
 
 /*==============================================================================
  * Compiler Hint End
  *============================================================================*/
```

