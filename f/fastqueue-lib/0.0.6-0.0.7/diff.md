# Comparing `tmp/fastqueue-lib-0.0.6.tar.gz` & `tmp/fastqueue-lib-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastqueue-lib-0.0.6.tar", last modified: Thu May 11 04:32:26 2023, max compression
+gzip compressed data, was "fastqueue-lib-0.0.7.tar", last modified: Mon May 15 05:09:41 2023, max compression
```

## Comparing `fastqueue-lib-0.0.6.tar` & `fastqueue-lib-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 04:32:26.117212 fastqueue-lib-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-11 04:32:08.000000 fastqueue-lib-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-11 04:32:08.000000 fastqueue-lib-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-11 04:32:26.117212 fastqueue-lib-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-05-11 04:32:08.000000 fastqueue-lib-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 04:32:26.117212 fastqueue-lib-0.0.6/fastqueue/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-11 04:32:08.000000 fastqueue-lib-0.0.6/fastqueue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-05-11 04:32:08.000000 fastqueue-lib-0.0.6/fastqueue/prototypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 04:32:26.117212 fastqueue-lib-0.0.6/fastqueue_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-11 04:32:26.000000 fastqueue-lib-0.0.6/fastqueue_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-11 04:32:26.000000 fastqueue-lib-0.0.6/fastqueue_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 04:32:26.000000 fastqueue-lib-0.0.6/fastqueue_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-11 04:32:26.000000 fastqueue-lib-0.0.6/fastqueue_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-11 04:32:26.000000 fastqueue-lib-0.0.6/fastqueue_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-11 04:32:08.000000 fastqueue-lib-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 04:32:26.117212 fastqueue-lib-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-11 04:32:08.000000 fastqueue-lib-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 04:32:26.117212 fastqueue-lib-0.0.6/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-11 04:32:08.000000 fastqueue-lib-0.0.6/src/ccqueue.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-11 04:32:08.000000 fastqueue-lib-0.0.6/src/cllqueue.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    26137 2023-05-11 04:32:08.000000 fastqueue-lib-0.0.6/src/fastqueue.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 04:32:26.117212 fastqueue-lib-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-05-11 04:32:08.000000 fastqueue-lib-0.0.6/tests/test_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:09:41.501569 fastqueue-lib-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-15 05:09:24.000000 fastqueue-lib-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-15 05:09:24.000000 fastqueue-lib-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-05-15 05:09:41.501569 fastqueue-lib-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-15 05:09:24.000000 fastqueue-lib-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:09:41.501569 fastqueue-lib-0.0.7/fastqueue/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 05:09:24.000000 fastqueue-lib-0.0.7/fastqueue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-05-15 05:09:24.000000 fastqueue-lib-0.0.7/fastqueue/prototypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:09:41.501569 fastqueue-lib-0.0.7/fastqueue_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-05-15 05:09:41.000000 fastqueue-lib-0.0.7/fastqueue_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-15 05:09:41.000000 fastqueue-lib-0.0.7/fastqueue_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 05:09:41.000000 fastqueue-lib-0.0.7/fastqueue_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-15 05:09:41.000000 fastqueue-lib-0.0.7/fastqueue_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-15 05:09:41.000000 fastqueue-lib-0.0.7/fastqueue_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-15 05:09:24.000000 fastqueue-lib-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 05:09:41.501569 fastqueue-lib-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-15 05:09:24.000000 fastqueue-lib-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:09:41.501569 fastqueue-lib-0.0.7/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-15 05:09:24.000000 fastqueue-lib-0.0.7/src/ccqueue.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-15 05:09:24.000000 fastqueue-lib-0.0.7/src/cllqueue.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28848 2023-05-15 05:09:24.000000 fastqueue-lib-0.0.7/src/fastqueue.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:09:41.501569 fastqueue-lib-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-05-15 05:09:24.000000 fastqueue-lib-0.0.7/tests/test_queue.py
```

### Comparing `fastqueue-lib-0.0.6/LICENSE` & `fastqueue-lib-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fastqueue-lib-0.0.6/PKG-INFO` & `fastqueue-lib-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastqueue-lib
-Version: 0.0.6
+Version: 0.0.7
 Summary: Fast single ended queue library for python
 Author-email: Matthew Taylor <matthew.taylor.andre@gmail.com>
 Project-URL: Homepage, https://github.com/MatthewAndreTaylor/fastqueue
 Keywords: Queue
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -109,14 +109,15 @@
 ![Queue_types](https://user-images.githubusercontent.com/100451342/232172490-bd90b021-7aeb-47b8-99e0-2481ccbc1f8f.png)
 
 ### Iteration
 
 
 Ubuntu
 
-![Iterable_Instantiation](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/c1028e20-d47c-4ec1-a602-263deefb4e05)
-![Iterable_Iteration](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/792e21b2-08b9-4e76-b75c-473caa90cdde)
+![Iterable_Instantiation](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/85939d12-73ed-42a5-a8bd-b2bea4ee599c)
+![Iterable_Iteration](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/b17f5f66-26b5-4e21-b5e5-c8fcbe5433a9)
 
 Windows
 
-![Iterable_Instantiation](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/7cc9866f-869e-466d-ac50-28a370f73cf7)
-![Iterable_Iteration](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/b5f53f09-a02a-472d-9ac7-f8cd9ceb3355)
+![Iterable_Instantiation](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/a7f89750-3b3b-475a-ac93-849c62d0c4a6)
+![Iterable_Iteration](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/9ee2feed-28a5-44a1-b72d-eff17804ebdd)
+
```

### Comparing `fastqueue-lib-0.0.6/README.md` & `fastqueue-lib-0.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -86,14 +86,15 @@
 ![Queue_types](https://user-images.githubusercontent.com/100451342/232172490-bd90b021-7aeb-47b8-99e0-2481ccbc1f8f.png)
 
 ### Iteration
 
 
 Ubuntu
 
-![Iterable_Instantiation](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/c1028e20-d47c-4ec1-a602-263deefb4e05)
-![Iterable_Iteration](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/792e21b2-08b9-4e76-b75c-473caa90cdde)
+![Iterable_Instantiation](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/85939d12-73ed-42a5-a8bd-b2bea4ee599c)
+![Iterable_Iteration](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/b17f5f66-26b5-4e21-b5e5-c8fcbe5433a9)
 
 Windows
 
-![Iterable_Instantiation](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/7cc9866f-869e-466d-ac50-28a370f73cf7)
-![Iterable_Iteration](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/b5f53f09-a02a-472d-9ac7-f8cd9ceb3355)
+![Iterable_Instantiation](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/a7f89750-3b3b-475a-ac93-849c62d0c4a6)
+![Iterable_Iteration](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/9ee2feed-28a5-44a1-b72d-eff17804ebdd)
+
```

### Comparing `fastqueue-lib-0.0.6/fastqueue/prototypes.py` & `fastqueue-lib-0.0.7/fastqueue/prototypes.py`

 * *Files identical despite different names*

### Comparing `fastqueue-lib-0.0.6/fastqueue_lib.egg-info/PKG-INFO` & `fastqueue-lib-0.0.7/fastqueue_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastqueue-lib
-Version: 0.0.6
+Version: 0.0.7
 Summary: Fast single ended queue library for python
 Author-email: Matthew Taylor <matthew.taylor.andre@gmail.com>
 Project-URL: Homepage, https://github.com/MatthewAndreTaylor/fastqueue
 Keywords: Queue
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -109,14 +109,15 @@
 ![Queue_types](https://user-images.githubusercontent.com/100451342/232172490-bd90b021-7aeb-47b8-99e0-2481ccbc1f8f.png)
 
 ### Iteration
 
 
 Ubuntu
 
-![Iterable_Instantiation](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/c1028e20-d47c-4ec1-a602-263deefb4e05)
-![Iterable_Iteration](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/792e21b2-08b9-4e76-b75c-473caa90cdde)
+![Iterable_Instantiation](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/85939d12-73ed-42a5-a8bd-b2bea4ee599c)
+![Iterable_Iteration](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/b17f5f66-26b5-4e21-b5e5-c8fcbe5433a9)
 
 Windows
 
-![Iterable_Instantiation](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/7cc9866f-869e-466d-ac50-28a370f73cf7)
-![Iterable_Iteration](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/b5f53f09-a02a-472d-9ac7-f8cd9ceb3355)
+![Iterable_Instantiation](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/a7f89750-3b3b-475a-ac93-849c62d0c4a6)
+![Iterable_Iteration](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/9ee2feed-28a5-44a1-b72d-eff17804ebdd)
+
```

### Comparing `fastqueue-lib-0.0.6/pyproject.toml` & `fastqueue-lib-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastqueue-lib"
-version = "0.0.6"
+version = "0.0.7"
 description="Fast single ended queue library for python"
 authors = [
     {name = "Matthew Taylor", email = "matthew.taylor.andre@gmail.com"},
 ]
 urls = {Homepage = "https://github.com/MatthewAndreTaylor/fastqueue"}
 requires-python = ">=3.9"
 keywords = [ "Queue" ]
```

### Comparing `fastqueue-lib-0.0.6/setup.py` & `fastqueue-lib-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `fastqueue-lib-0.0.6/src/ccqueue.cpp` & `fastqueue-lib-0.0.7/src/ccqueue.cpp`

 * *Files identical despite different names*

### Comparing `fastqueue-lib-0.0.6/src/cllqueue.cpp` & `fastqueue-lib-0.0.7/src/cllqueue.cpp`

 * *Files identical despite different names*

### Comparing `fastqueue-lib-0.0.6/src/fastqueue.c` & `fastqueue-lib-0.0.7/src/fastqueue.c`

 * *Files 5% similar despite different names*

```diff
@@ -38,20 +38,41 @@
     self->length = 0;
     self->capacity = 1024;
     self->front = 1023;
     self->back = 0;
     return (PyObject*)self;
 }
 
+static PyObject* QueueC_copy(QueueC* self, PyObject* args) {
+    QueueC* copy = (QueueC*)Py_TYPE(self)->tp_alloc(Py_TYPE(self), 0);
+    if (copy == NULL)
+        return PyErr_NoMemory();
+
+    copy->objects = (PyObject**) malloc(self->capacity * sizeof(PyObject*));
+    if (copy->objects == NULL) {
+        Py_DECREF(copy);
+        return PyErr_NoMemory();
+    }
+    for (int i = 0; i < self->length; ++i) {
+        int index = (self->back + i) % self->capacity;
+        copy->objects[index] = self->objects[index];
+        Py_INCREF(copy->objects[index]);
+    }
+    copy->length = self->length;
+    copy->capacity = self->capacity;
+    copy->front = self->front;
+    copy->back = self->back;
+    return (PyObject*)copy;
+}
+
 static void QueueC_dealloc(QueueC* self) {
     if (self == NULL)
         return;
     PyObject_GC_UnTrack(self);
     free(self->objects);
-    self->objects = NULL;
     Py_TYPE(self)->tp_free(self);
 }
 
 static int QueueC_clear(QueueC* self) {
     if (self->length == 0)
         return 0;
 
@@ -147,14 +168,22 @@
         }
     }
 
     Py_DECREF(iterable);
     Py_RETURN_NONE;
 }
 
+static int QueueC_init(QueueC* self, PyObject* args, PyObject* kwargs) {
+    if (PyTuple_GET_SIZE(args) > 0) {
+        PyObject* iterable = PyTuple_GET_ITEM(args, 0);
+        QueueC_extend(self, iterable);
+    }
+    return 0;
+}
+
 static Py_ssize_t QueueC_len(QueueC* self) {
     return (Py_ssize_t)self->length;
 }
 
 static PyObject* QueueC_item(QueueC* self, Py_ssize_t index) {
     if (index < 0)
         index = index + QueueC_len(self);
@@ -210,14 +239,16 @@
 };
 
 static PyMethodDef QueueC_methods[] = {
     {"enqueue", (PyCFunction)QueueC_enqueue, METH_O, "Add an object to the front of the QueueC."},
     {"dequeue", (PyCFunction)QueueC_dequeue, METH_NOARGS, "Remove and return an object from the back of the QueueC."},
     {"is_empty", (PyCFunction)QueueC_is_empty, METH_NOARGS, "Check if the QueueC is empty."},
     {"extend", (PyCFunction)QueueC_extend, METH_O, "Add an objects from an iterator front of the QueueC."},
+    {"__copy__", (PyCFunction)QueueC_copy, METH_NOARGS, "Return a shallow copy of the QueueC."},
+    {"copy", (PyCFunction)QueueC_copy, METH_NOARGS, "Return a shallow copy of the QueueC."},
     {NULL, NULL, 0, NULL}
 };
 
 PyDoc_STRVAR(queuec_doc, "QueueC() -> Contiguous Single ended Queue object.");
 static PyTypeObject QueueCType = {
     PyVarObject_HEAD_INIT(NULL, 0)
     "QueueC",                                   /* tp_name */
@@ -250,15 +281,15 @@
     0,                                          /* tp_members */
     0,                                          /* tp_getset */
     0,                                          /* tp_base */
     0,                                          /* tp_dict */
     0,                                          /* tp_descr_get */
     0,                                          /* tp_descr_set */
     0,                                          /* tp_dictoffset */
-    0,                                          /* tp_init */
+    (initproc)QueueC_init,                      /* tp_init */
     PyType_GenericAlloc,                        /* tp_alloc */
     QueueC_new,                                 /* tp_new */
     PyObject_GC_Del,                            /* tp_free */
 };
 
 
 /**
@@ -305,24 +336,64 @@
 
     self->head = NULL;
     self->tail = NULL;
     self->length = 0;
     return (PyObject*)self;
 }
 
+PyDoc_STRVAR(copy_doc, "Return a shallow copy of the Queue.");
+static PyObject* Queue_copy(Queue_t* self, PyObject* args) {
+    Queue_t* newQueue = (Queue_t*)Queue_new(Py_TYPE(self), args, NULL);
+    if (newQueue == NULL)
+        return PyErr_NoMemory();
+
+    newQueue->length = self->length;
+    newQueue->head = NULL;
+    newQueue->tail = NULL;
+
+    QueueNode_t* current = self->head;
+    while (current != NULL) {
+        QueueNode_t* newNode = QueueNode_new();
+        if (newNode == NULL) {
+            PyErr_NoMemory();
+            return NULL;
+        }
+
+        for (int i = 0; i < current->numEntries; ++i) {
+            int index = (current->back + i) & 255;
+            newNode->py_objects[index] = current->py_objects[index];
+            Py_INCREF(current->py_objects[index]);
+        }
+
+        newNode->numEntries = current->numEntries;
+        newNode->front = current->front;
+        newNode->back = current->back;
+
+        if (newQueue->head == NULL) {
+            newQueue->head = newNode;
+        }  
+        else {
+            newQueue->tail->next = newNode;
+        }
+        newQueue->tail = newNode;
+        current = current->next;
+    }
+    return (PyObject*)newQueue;
+}
+
 // Add a py_object to the front of the QueueNode
 static inline void QueueNode_put(QueueNode_t* queue_node, PyObject* py_object) {
     Py_INCREF(py_object);
     queue_node->front = (queue_node->front + 1) & 255;
     queue_node->py_objects[queue_node->front] = py_object;
     queue_node->numEntries++;
 }
 
 // Add a py_object to the last QueueNode in the Queue
-PyDoc_STRVAR(enqueue_doc, "Add an item to the front of the queue.");
+PyDoc_STRVAR(enqueue_doc, "Add an item to the front of the Queue.");
 static PyObject* Queue_enqueue(Queue_t* self, PyObject* object) {
     if (object == Py_None)
         Py_RETURN_NONE;
 
     if (self->tail == NULL) {
         self->head = QueueNode_new();
         self->tail = self->head;
@@ -338,15 +409,15 @@
 
     QueueNode_put(self->tail, object);
     self->length++;
     Py_RETURN_NONE;
 }
 
 // Remove a py_object from the first QueueNode in the Queue
-PyDoc_STRVAR(dequeue_doc, "Remove and return an item from the end of the queue.");
+PyDoc_STRVAR(dequeue_doc, "Remove and return an item from the end of the Queue.");
 static PyObject* Queue_dequeue(Queue_t* self) {
     if (self->length == 0) {
         PyErr_SetString(PyExc_IndexError, "dequeue from an empty Queue");
         return NULL;
     }
 
     PyObject* py_object = self->head->py_objects[self->head->back];
@@ -500,14 +571,16 @@
 };
 
 static PyMethodDef Queue_methods[] = {
     {"enqueue", (PyCFunction)Queue_enqueue, METH_O, enqueue_doc},
     {"dequeue", (PyCFunction)Queue_dequeue, METH_NOARGS, dequeue_doc},
     {"is_empty", (PyCFunction)Queue_is_empty, METH_NOARGS, is_empty_doc},
     {"extend", (PyCFunction)Queue_extend, METH_O, extend_doc},
+    {"__copy__", (PyCFunction)Queue_copy, METH_NOARGS, copy_doc},
+    {"copy", (PyCFunction)Queue_copy, METH_NOARGS, copy_doc},
     {NULL, NULL, 0, NULL}
 };
 
 PyDoc_STRVAR(queue_doc,"Queue() -> Single ended Queue object.");
 static PyTypeObject QueueType = {
     PyVarObject_HEAD_INIT(NULL, 0)
     "Queue",                                    /* tp_name */
@@ -598,14 +671,18 @@
     return result;
 }
 
 static PyObject* LockQueue_is_empty(LockQueue_t* self, PyObject* args) {
     return LockQueue_call_with_lock(self, args, &Queue_is_empty);
 }
 
+static PyObject* LockQueue_copy(LockQueue_t* self, PyObject* args) {
+    return LockQueue_call_with_lock(self, args, &Queue_copy);
+}
+
 static PyObject* LockQueue_enqueue(LockQueue_t* self, PyObject* args) {
     return LockQueue_call_with_lock(self, args, &Queue_enqueue);
 }
 
 static PyObject* LockQueue_dequeue(LockQueue_t* self) {
     PyThread_acquire_lock(self->lock, 1);
     PyObject* result = Queue_dequeue(self->queue);
@@ -646,14 +723,16 @@
 }
 
 static PyMethodDef LockQueue_methods[] = {
     {"is_empty", (PyCFunction)LockQueue_is_empty, METH_NOARGS, is_empty_doc},
     {"enqueue", (PyCFunction)LockQueue_enqueue, METH_O, enqueue_doc},
     {"dequeue", (PyCFunction)LockQueue_dequeue, METH_NOARGS, dequeue_doc},
     {"extend", (PyCFunction)LockQueue_extend, METH_O, extend_doc},
+    {"__copy__", (PyCFunction)LockQueue_copy, METH_NOARGS, copy_doc},
+    {"copy", (PyCFunction)LockQueue_copy, METH_NOARGS, copy_doc},
     {NULL, NULL, 0, NULL}
 };
 
 static PySequenceMethods LockQueue_sequence_methods = {
     (lenfunc)LockQueue_len,               /* sq_length */
     0,                                    /* sq_concat */
     NULL,                                 /* sq_repeat */
```

### Comparing `fastqueue-lib-0.0.6/tests/test_queue.py` & `fastqueue-lib-0.0.7/tests/test_queue.py`

 * *Files 18% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     queue.extend(lst)
     assert len(queue) == 3
     assert lst == [1, 2, 3]
     assert lst[2] == 3
     assert queue[2] == 3
 
 
-@pytest.mark.parametrize("queue", [Queue(), LockQueue(), QueueC()])
+@pytest.mark.parametrize("queue", [LockQueue(), Queue(), QueueC()])
 def test_mixed_extendQueue(queue):
     size = 50
     queue.enqueue(1)
     queue.enqueue(2)
     queue.enqueue(3)
     queue.extend(range(size))
     queue.enqueue(4)
@@ -149,7 +149,26 @@
     queue.extend(range(queue_size))
     assert not (queue_size in queue)
     for i in range(258):
         assert i in queue
     assert (queue_size - 1) in queue
     queue.dequeue()
     assert not (0 in queue)
+
+
+@pytest.mark.parametrize("queue", [LockQueue(), Queue(), QueueC()])
+def test_copy(queue):
+    queue.extend([1, 2, 3, 4])
+    copy = queue.copy()
+    assert copy != queue
+    queue[0] = 0
+    assert copy[0] == 1
+    assert [copy.dequeue() for _ in range(len(copy))] == [1, 2, 3, 4]
+    assert len(copy) == 0
+    assert len(queue) == 4
+    assert [queue.dequeue() for _ in range(len(queue))] == [0, 2, 3, 4]
+    queue.enqueue("🎈")
+    copy = queue.copy()
+    assert len(queue) == 1
+    assert len(copy) == 1
+    assert copy[0] == "🎈"
+    assert queue[0] == "🎈"
```

