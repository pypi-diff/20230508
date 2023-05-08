# Comparing `tmp/fastqueue-lib-0.0.4.tar.gz` & `tmp/fastqueue-lib-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastqueue-lib-0.0.4.tar", last modified: Sat Apr 22 00:23:21 2023, max compression
+gzip compressed data, was "fastqueue-lib-0.0.5.tar", last modified: Mon May  8 11:43:31 2023, max compression
```

## Comparing `fastqueue-lib-0.0.4.tar` & `fastqueue-lib-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:23:21.707372 fastqueue-lib-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-22 00:23:06.000000 fastqueue-lib-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-22 00:23:06.000000 fastqueue-lib-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-22 00:23:21.707372 fastqueue-lib-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-22 00:23:06.000000 fastqueue-lib-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:23:21.707372 fastqueue-lib-0.0.4/fastqueue/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-22 00:23:06.000000 fastqueue-lib-0.0.4/fastqueue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-04-22 00:23:06.000000 fastqueue-lib-0.0.4/fastqueue/prototypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:23:21.707372 fastqueue-lib-0.0.4/fastqueue_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-22 00:23:21.000000 fastqueue-lib-0.0.4/fastqueue_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-22 00:23:21.000000 fastqueue-lib-0.0.4/fastqueue_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 00:23:21.000000 fastqueue-lib-0.0.4/fastqueue_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-22 00:23:21.000000 fastqueue-lib-0.0.4/fastqueue_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-22 00:23:21.000000 fastqueue-lib-0.0.4/fastqueue_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-22 00:23:06.000000 fastqueue-lib-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 00:23:21.707372 fastqueue-lib-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-22 00:23:06.000000 fastqueue-lib-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:23:21.707372 fastqueue-lib-0.0.4/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-04-22 00:23:06.000000 fastqueue-lib-0.0.4/src/ccqueue.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-04-22 00:23:06.000000 fastqueue-lib-0.0.4/src/cllqueue.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    25282 2023-04-22 00:23:06.000000 fastqueue-lib-0.0.4/src/fastqueue.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:23:21.707372 fastqueue-lib-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-22 00:23:06.000000 fastqueue-lib-0.0.4/tests/test_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:43:31.083974 fastqueue-lib-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-08 11:43:10.000000 fastqueue-lib-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-08 11:43:10.000000 fastqueue-lib-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-05-08 11:43:31.083974 fastqueue-lib-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-08 11:43:10.000000 fastqueue-lib-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:43:31.079974 fastqueue-lib-0.0.5/fastqueue/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-08 11:43:10.000000 fastqueue-lib-0.0.5/fastqueue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-05-08 11:43:10.000000 fastqueue-lib-0.0.5/fastqueue/prototypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:43:31.083974 fastqueue-lib-0.0.5/fastqueue_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-05-08 11:43:31.000000 fastqueue-lib-0.0.5/fastqueue_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-08 11:43:31.000000 fastqueue-lib-0.0.5/fastqueue_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 11:43:31.000000 fastqueue-lib-0.0.5/fastqueue_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-08 11:43:31.000000 fastqueue-lib-0.0.5/fastqueue_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-08 11:43:31.000000 fastqueue-lib-0.0.5/fastqueue_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-08 11:43:10.000000 fastqueue-lib-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 11:43:31.083974 fastqueue-lib-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-08 11:43:10.000000 fastqueue-lib-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:43:31.083974 fastqueue-lib-0.0.5/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-08 11:43:10.000000 fastqueue-lib-0.0.5/src/ccqueue.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-08 11:43:10.000000 fastqueue-lib-0.0.5/src/cllqueue.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25926 2023-05-08 11:43:10.000000 fastqueue-lib-0.0.5/src/fastqueue.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:43:31.083974 fastqueue-lib-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-05-08 11:43:10.000000 fastqueue-lib-0.0.5/tests/test_queue.py
```

### Comparing `fastqueue-lib-0.0.4/LICENSE` & `fastqueue-lib-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fastqueue-lib-0.0.4/PKG-INFO` & `fastqueue-lib-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastqueue-lib
-Version: 0.0.4
+Version: 0.0.5
 Summary: Fast single ended queue library for python
 Author-email: Matthew Taylor <matthew.taylor.andre@gmail.com>
 Project-URL: Homepage, https://github.com/MatthewAndreTaylor/mqueue
 Keywords: Queue
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fastqueue-lib-0.0.4/README.md` & `fastqueue-lib-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fastqueue-lib-0.0.4/fastqueue/prototypes.py` & `fastqueue-lib-0.0.5/fastqueue/prototypes.py`

 * *Files identical despite different names*

### Comparing `fastqueue-lib-0.0.4/fastqueue_lib.egg-info/PKG-INFO` & `fastqueue-lib-0.0.5/fastqueue_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastqueue-lib
-Version: 0.0.4
+Version: 0.0.5
 Summary: Fast single ended queue library for python
 Author-email: Matthew Taylor <matthew.taylor.andre@gmail.com>
 Project-URL: Homepage, https://github.com/MatthewAndreTaylor/mqueue
 Keywords: Queue
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fastqueue-lib-0.0.4/pyproject.toml` & `fastqueue-lib-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastqueue-lib"
-version = "0.0.4"
+version = "0.0.5"
 description="Fast single ended queue library for python"
 authors = [
     {name = "Matthew Taylor", email = "matthew.taylor.andre@gmail.com"},
 ]
 urls = {Homepage = "https://github.com/MatthewAndreTaylor/mqueue"}
 requires-python = ">=3.9"
 keywords = [ "Queue" ]
```

### Comparing `fastqueue-lib-0.0.4/setup.py` & `fastqueue-lib-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,21 +22,22 @@
     Extension(
         "fastqueue.cllqueue",
         ["src/cllqueue.cpp"],
     ),
     Extension(
         "fastqueue.ccqueue",
         ["src/ccqueue.cpp"],
-    )
+    ),
 ]
 
 setup(
     include_package_data=True,
     packages=["fastqueue"],
-    ext_modules=ctype_ext + [
+    ext_modules=ctype_ext
+    + [
         Extension(
             "_fastqueue",
             ["src/fastqueue.c"],
         )
     ],
-    cmdclass={"build_ext": build_ext}
+    cmdclass={"build_ext": build_ext},
 )
```

### Comparing `fastqueue-lib-0.0.4/src/ccqueue.cpp` & `fastqueue-lib-0.0.5/src/ccqueue.cpp`

 * *Files identical despite different names*

### Comparing `fastqueue-lib-0.0.4/src/cllqueue.cpp` & `fastqueue-lib-0.0.5/src/cllqueue.cpp`

 * *Files identical despite different names*

### Comparing `fastqueue-lib-0.0.4/src/fastqueue.c` & `fastqueue-lib-0.0.5/src/fastqueue.c`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #include "pythread.h"
 
 /**
  * Single ended Contiguous Python Queue
  * --- fastqueue.QueueC ---
  */
 typedef struct {
-    PyObject_VAR_HEAD
+    PyObject_HEAD
     PyObject** objects;
     int length;
     int capacity;
     int front;
     int back;
 } QueueC;
 
@@ -81,30 +81,35 @@
     if (newObjects == NULL) {
         PyErr_NoMemory();
         return;
     }
     for (int i = 0; i < self->length; ++i) {
         newObjects[i] = self->objects[(self->back + i) % self->capacity];
     }
-
+    self->front = self->length - 1;
+    self->back = 0;
     free(self->objects);
     self->objects = newObjects;
     self->capacity = newCapacity;
 }
 
+static inline void QueueC_put(QueueC* self, PyObject* object) {
+    Py_INCREF(object);
+    self->front = (self->front + 1) % self->capacity;
+    self->objects[self->front] = object;
+    self->length++;
+}
+
 static PyObject* QueueC_enqueue(QueueC* self, PyObject* object) {
     if (object == Py_None)
         Py_RETURN_NONE;
     if (self->length == self->capacity)
         QueueC_resize(self, self->capacity * 2);
 
-    Py_INCREF(object);
-    self->front = (self->front + 1) % self->capacity;
-    self->objects[self->front] = object;
-    self->length++;
+    QueueC_put(self, object);
     Py_RETURN_NONE;
 }
 
 static PyObject* QueueC_dequeue(QueueC* self) {
     if (self->length == 0) {
         PyErr_SetString(PyExc_IndexError, "dequeue from an empty Queue");
         return NULL;
@@ -120,17 +125,33 @@
     PyObject* iterable = PyObject_GetIter(iterator);
     if (iterable == NULL)
         return NULL;
 
     PyObject* py_object;
     PyObject* (*next)(PyObject*);
     next = *Py_TYPE(iterable)->tp_iternext;
-    while ((py_object = next(iterable)) != NULL) {
-        QueueC_enqueue(self, py_object);
+
+    if (PySequence_Check(iterable)) {
+        // Small optimization sizing, amortized approach is still very good
+        int len = (int) PyObject_Size(iterable);
+        printf("Len %d", len);
+        if (self->length + len > self->capacity) {
+            QueueC_resize(self, (self->capacity + len) * 2);
+        }
+
+        while ((py_object = next(iterable)) != NULL) {
+            QueueC_put(self, py_object);
+        }
     }
+    else {
+        while ((py_object = next(iterable)) != NULL) {
+            QueueC_enqueue(self, py_object);
+        }
+    }
+
     Py_DECREF(iterable);
     Py_RETURN_NONE;
 }
 
 static Py_ssize_t QueueC_len(QueueC* self) {
     return (Py_ssize_t)self->length;
 }
@@ -685,15 +706,15 @@
     "Singly linked, small overhead implementations of the Queue data structure.",
     -1,
     NULL, NULL, NULL, NULL, NULL
 };
 
 PyMODINIT_FUNC PyInit__fastqueue(void) {
     PyObject* module;
-    if (PyType_Ready(&QueueType) < 0 || PyType_Ready(&QueueCType) < 0)
+    if (PyType_Ready(&QueueType) < 0 || PyType_Ready(&QueueCType) < 0 || PyType_Ready(&LockQueueType) < 0)
         return NULL;
 
     module = PyModule_Create(&QueueModuleDef);
     if (module == NULL)
         return NULL;
     PyModule_AddType(module, &QueueCType);
     PyModule_AddType(module, &QueueType);
```

