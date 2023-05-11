# Comparing `tmp/fastqueue-lib-0.0.5.tar.gz` & `tmp/fastqueue-lib-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastqueue-lib-0.0.5.tar", last modified: Mon May  8 11:43:31 2023, max compression
+gzip compressed data, was "fastqueue-lib-0.0.6.tar", last modified: Thu May 11 04:32:26 2023, max compression
```

## Comparing `fastqueue-lib-0.0.5.tar` & `fastqueue-lib-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:43:31.083974 fastqueue-lib-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-08 11:43:10.000000 fastqueue-lib-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-08 11:43:10.000000 fastqueue-lib-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-05-08 11:43:31.083974 fastqueue-lib-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-08 11:43:10.000000 fastqueue-lib-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:43:31.079974 fastqueue-lib-0.0.5/fastqueue/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-08 11:43:10.000000 fastqueue-lib-0.0.5/fastqueue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-05-08 11:43:10.000000 fastqueue-lib-0.0.5/fastqueue/prototypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:43:31.083974 fastqueue-lib-0.0.5/fastqueue_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-05-08 11:43:31.000000 fastqueue-lib-0.0.5/fastqueue_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-08 11:43:31.000000 fastqueue-lib-0.0.5/fastqueue_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 11:43:31.000000 fastqueue-lib-0.0.5/fastqueue_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-08 11:43:31.000000 fastqueue-lib-0.0.5/fastqueue_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-08 11:43:31.000000 fastqueue-lib-0.0.5/fastqueue_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-08 11:43:10.000000 fastqueue-lib-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 11:43:31.083974 fastqueue-lib-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-08 11:43:10.000000 fastqueue-lib-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:43:31.083974 fastqueue-lib-0.0.5/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-08 11:43:10.000000 fastqueue-lib-0.0.5/src/ccqueue.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-08 11:43:10.000000 fastqueue-lib-0.0.5/src/cllqueue.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    25926 2023-05-08 11:43:10.000000 fastqueue-lib-0.0.5/src/fastqueue.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:43:31.083974 fastqueue-lib-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-05-08 11:43:10.000000 fastqueue-lib-0.0.5/tests/test_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 04:32:26.117212 fastqueue-lib-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-11 04:32:08.000000 fastqueue-lib-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-11 04:32:08.000000 fastqueue-lib-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-11 04:32:26.117212 fastqueue-lib-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-05-11 04:32:08.000000 fastqueue-lib-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 04:32:26.117212 fastqueue-lib-0.0.6/fastqueue/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-11 04:32:08.000000 fastqueue-lib-0.0.6/fastqueue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-05-11 04:32:08.000000 fastqueue-lib-0.0.6/fastqueue/prototypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 04:32:26.117212 fastqueue-lib-0.0.6/fastqueue_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-11 04:32:26.000000 fastqueue-lib-0.0.6/fastqueue_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-11 04:32:26.000000 fastqueue-lib-0.0.6/fastqueue_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 04:32:26.000000 fastqueue-lib-0.0.6/fastqueue_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-11 04:32:26.000000 fastqueue-lib-0.0.6/fastqueue_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-11 04:32:26.000000 fastqueue-lib-0.0.6/fastqueue_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-11 04:32:08.000000 fastqueue-lib-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 04:32:26.117212 fastqueue-lib-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-11 04:32:08.000000 fastqueue-lib-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 04:32:26.117212 fastqueue-lib-0.0.6/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-11 04:32:08.000000 fastqueue-lib-0.0.6/src/ccqueue.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-11 04:32:08.000000 fastqueue-lib-0.0.6/src/cllqueue.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26137 2023-05-11 04:32:08.000000 fastqueue-lib-0.0.6/src/fastqueue.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 04:32:26.117212 fastqueue-lib-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-05-11 04:32:08.000000 fastqueue-lib-0.0.6/tests/test_queue.py
```

### Comparing `fastqueue-lib-0.0.5/LICENSE` & `fastqueue-lib-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fastqueue-lib-0.0.5/PKG-INFO` & `fastqueue-lib-0.0.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fastqueue-lib
-Version: 0.0.5
+Version: 0.0.6
 Summary: Fast single ended queue library for python
 Author-email: Matthew Taylor <matthew.taylor.andre@gmail.com>
-Project-URL: Homepage, https://github.com/MatthewAndreTaylor/mqueue
+Project-URL: Homepage, https://github.com/MatthewAndreTaylor/fastqueue
 Keywords: Queue
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
@@ -72,14 +72,15 @@
 The enqueue and dequeue methods perform similarly well over a large sequence of arbitrary operations.
 `fastqueue.QueueC()` handles memory differently by doubling the capacity when full.
 This increases the complexity but maintains fast amortized cost.
 The benefit of this approach is even faster `__getitem__` and `__setitem__` speeds
 
 ```py
 >>> from fastqueue import QueueC
+
 >>> queue_c = QueueC()
 >>> queue_c.extend(['🚒', '🛴'])
 >>> queue_c[0]
 '🚒'
 >>> '🛴' in queue_c
 True
 >>> queue_c.enqueue('🚅')
@@ -90,11 +91,32 @@
 ['🚒', '🛴', '🚅', '🚗']
 ```
 
 Another alternative is `fastqueue.LockQueue()` which supports all queue operations.
 `fastqueue.LockQueue()` is built as a thread-safe alternative to the other queue types.
 
 ## Example Benchmarks
+
+### Queue operations
+
+Ubuntu
+
+![Queue_times](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/1c47cdc5-e7cc-4c89-8902-91359f660002)
+![Queue_types_linux](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/59a6d2c6-51c6-45e1-aa4e-eb6679616a75)
+
+Windows
+
 ![Queue_times](https://user-images.githubusercontent.com/100451342/232172485-c17b6b33-986f-461b-b0bf-b26b3f6e8304.png)
 ![Queue_types](https://user-images.githubusercontent.com/100451342/232172490-bd90b021-7aeb-47b8-99e0-2481ccbc1f8f.png)
 
+### Iteration
+
+
+Ubuntu
+
+![Iterable_Instantiation](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/c1028e20-d47c-4ec1-a602-263deefb4e05)
+![Iterable_Iteration](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/792e21b2-08b9-4e76-b75c-473caa90cdde)
+
+Windows
 
+![Iterable_Instantiation](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/7cc9866f-869e-466d-ac50-28a370f73cf7)
+![Iterable_Iteration](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/b5f53f09-a02a-472d-9ac7-f8cd9ceb3355)
```

### Comparing `fastqueue-lib-0.0.5/README.md` & `fastqueue-lib-0.0.6/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 The enqueue and dequeue methods perform similarly well over a large sequence of arbitrary operations.
 `fastqueue.QueueC()` handles memory differently by doubling the capacity when full.
 This increases the complexity but maintains fast amortized cost.
 The benefit of this approach is even faster `__getitem__` and `__setitem__` speeds
 
 ```py
 >>> from fastqueue import QueueC
+
 >>> queue_c = QueueC()
 >>> queue_c.extend(['🚒', '🛴'])
 >>> queue_c[0]
 '🚒'
 >>> '🛴' in queue_c
 True
 >>> queue_c.enqueue('🚅')
@@ -67,11 +68,32 @@
 ['🚒', '🛴', '🚅', '🚗']
 ```
 
 Another alternative is `fastqueue.LockQueue()` which supports all queue operations.
 `fastqueue.LockQueue()` is built as a thread-safe alternative to the other queue types.
 
 ## Example Benchmarks
+
+### Queue operations
+
+Ubuntu
+
+![Queue_times](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/1c47cdc5-e7cc-4c89-8902-91359f660002)
+![Queue_types_linux](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/59a6d2c6-51c6-45e1-aa4e-eb6679616a75)
+
+Windows
+
 ![Queue_times](https://user-images.githubusercontent.com/100451342/232172485-c17b6b33-986f-461b-b0bf-b26b3f6e8304.png)
 ![Queue_types](https://user-images.githubusercontent.com/100451342/232172490-bd90b021-7aeb-47b8-99e0-2481ccbc1f8f.png)
 
+### Iteration
+
+
+Ubuntu
+
+![Iterable_Instantiation](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/c1028e20-d47c-4ec1-a602-263deefb4e05)
+![Iterable_Iteration](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/792e21b2-08b9-4e76-b75c-473caa90cdde)
+
+Windows
 
+![Iterable_Instantiation](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/7cc9866f-869e-466d-ac50-28a370f73cf7)
+![Iterable_Iteration](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/b5f53f09-a02a-472d-9ac7-f8cd9ceb3355)
```

### Comparing `fastqueue-lib-0.0.5/fastqueue/prototypes.py` & `fastqueue-lib-0.0.6/fastqueue/prototypes.py`

 * *Files identical despite different names*

### Comparing `fastqueue-lib-0.0.5/fastqueue_lib.egg-info/PKG-INFO` & `fastqueue-lib-0.0.6/fastqueue_lib.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fastqueue-lib
-Version: 0.0.5
+Version: 0.0.6
 Summary: Fast single ended queue library for python
 Author-email: Matthew Taylor <matthew.taylor.andre@gmail.com>
-Project-URL: Homepage, https://github.com/MatthewAndreTaylor/mqueue
+Project-URL: Homepage, https://github.com/MatthewAndreTaylor/fastqueue
 Keywords: Queue
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
@@ -72,14 +72,15 @@
 The enqueue and dequeue methods perform similarly well over a large sequence of arbitrary operations.
 `fastqueue.QueueC()` handles memory differently by doubling the capacity when full.
 This increases the complexity but maintains fast amortized cost.
 The benefit of this approach is even faster `__getitem__` and `__setitem__` speeds
 
 ```py
 >>> from fastqueue import QueueC
+
 >>> queue_c = QueueC()
 >>> queue_c.extend(['🚒', '🛴'])
 >>> queue_c[0]
 '🚒'
 >>> '🛴' in queue_c
 True
 >>> queue_c.enqueue('🚅')
@@ -90,11 +91,32 @@
 ['🚒', '🛴', '🚅', '🚗']
 ```
 
 Another alternative is `fastqueue.LockQueue()` which supports all queue operations.
 `fastqueue.LockQueue()` is built as a thread-safe alternative to the other queue types.
 
 ## Example Benchmarks
+
+### Queue operations
+
+Ubuntu
+
+![Queue_times](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/1c47cdc5-e7cc-4c89-8902-91359f660002)
+![Queue_types_linux](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/59a6d2c6-51c6-45e1-aa4e-eb6679616a75)
+
+Windows
+
 ![Queue_times](https://user-images.githubusercontent.com/100451342/232172485-c17b6b33-986f-461b-b0bf-b26b3f6e8304.png)
 ![Queue_types](https://user-images.githubusercontent.com/100451342/232172490-bd90b021-7aeb-47b8-99e0-2481ccbc1f8f.png)
 
+### Iteration
+
+
+Ubuntu
+
+![Iterable_Instantiation](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/c1028e20-d47c-4ec1-a602-263deefb4e05)
+![Iterable_Iteration](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/792e21b2-08b9-4e76-b75c-473caa90cdde)
+
+Windows
 
+![Iterable_Instantiation](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/7cc9866f-869e-466d-ac50-28a370f73cf7)
+![Iterable_Iteration](https://github.com/MatthewAndreTaylor/fastqueue/assets/100451342/b5f53f09-a02a-472d-9ac7-f8cd9ceb3355)
```

### Comparing `fastqueue-lib-0.0.5/pyproject.toml` & `fastqueue-lib-0.0.6/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastqueue-lib"
-version = "0.0.5"
+version = "0.0.6"
 description="Fast single ended queue library for python"
 authors = [
     {name = "Matthew Taylor", email = "matthew.taylor.andre@gmail.com"},
 ]
-urls = {Homepage = "https://github.com/MatthewAndreTaylor/mqueue"}
+urls = {Homepage = "https://github.com/MatthewAndreTaylor/fastqueue"}
 requires-python = ">=3.9"
 keywords = [ "Queue" ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
@@ -26,9 +26,9 @@
 ]
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [project.optional-dependencies]
-examples = [ "matplotlib" ]
+examples = [ "matplotlib", "numpy" ]
 tests = [ "pytest" ]
```

### Comparing `fastqueue-lib-0.0.5/setup.py` & `fastqueue-lib-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `fastqueue-lib-0.0.5/src/ccqueue.cpp` & `fastqueue-lib-0.0.6/src/ccqueue.cpp`

 * *Files identical despite different names*

### Comparing `fastqueue-lib-0.0.5/src/cllqueue.cpp` & `fastqueue-lib-0.0.6/src/cllqueue.cpp`

 * *Files identical despite different names*

### Comparing `fastqueue-lib-0.0.5/src/fastqueue.c` & `fastqueue-lib-0.0.6/src/fastqueue.c`

 * *Files 2% similar despite different names*

```diff
@@ -126,18 +126,17 @@
     if (iterable == NULL)
         return NULL;
 
     PyObject* py_object;
     PyObject* (*next)(PyObject*);
     next = *Py_TYPE(iterable)->tp_iternext;
 
-    if (PySequence_Check(iterable)) {
-        // Small optimization sizing, amortized approach is still very good
-        int len = (int) PyObject_Size(iterable);
-        printf("Len %d", len);
+    // Small optimization sizing, amortized approach is still very good
+    Py_ssize_t len = PyObject_Size(iterator);
+    if (len > self->length) {
         if (self->length + len > self->capacity) {
             QueueC_resize(self, (self->capacity + len) * 2);
         }
 
         while ((py_object = next(iterable)) != NULL) {
             QueueC_put(self, py_object);
         }
@@ -582,42 +581,51 @@
 }
 
 static int LockQueue_traverse(LockQueue_t* self, visitproc visit, void* arg) {
     return Queue_traverse(self->queue, visit, arg);
 }
 
 static int LockQueue_clear(LockQueue_t* self) {
-    return Queue_clear(self->queue);
+    PyThread_acquire_lock(self->lock, 1);
+    int res = Queue_clear(self->queue);
+    PyThread_release_lock(self->lock);
+    return res;
 }
 
 static PyObject* LockQueue_call_with_lock(LockQueue_t* self, PyObject* args, PyObject* (*func)(Queue_t*, PyObject*)) {
-    PyThread_acquire_lock(self->lock, WAIT_LOCK);
+    PyThread_acquire_lock(self->lock, 1);
     PyObject* result = func(self->queue, args);
     PyThread_release_lock(self->lock);
     return result;
 }
 
 static PyObject* LockQueue_is_empty(LockQueue_t* self, PyObject* args) {
     return LockQueue_call_with_lock(self, args, &Queue_is_empty);
 }
 
 static PyObject* LockQueue_enqueue(LockQueue_t* self, PyObject* args) {
     return LockQueue_call_with_lock(self, args, &Queue_enqueue);
 }
 
-static PyObject* LockQueue_dequeue(LockQueue_t* self, PyObject* args) {
-    return LockQueue_call_with_lock(self, args, &Queue_dequeue);
+static PyObject* LockQueue_dequeue(LockQueue_t* self) {
+    PyThread_acquire_lock(self->lock, 1);
+    PyObject* result = Queue_dequeue(self->queue);
+    PyThread_release_lock(self->lock);
+    return result;
 }
 
 static PyObject* LockQueue_extend(LockQueue_t* self, PyObject* args) {
     return LockQueue_call_with_lock(self, args, &Queue_extend);
 }
 
-static PyObject* LockQueue_item(LockQueue_t* self, PyObject* args) {
-    return LockQueue_call_with_lock(self, args, &Queue_item);
+static PyObject* LockQueue_item(LockQueue_t* self, Py_ssize_t index) {
+    PyThread_acquire_lock(self->lock, 1);
+    PyObject* result = Queue_item(self->queue, index);
+    PyThread_release_lock(self->lock);
+    return result;
 }
 
 static Py_ssize_t LockQueue_len(LockQueue_t* self) {
     PyThread_acquire_lock(self->lock, 1);
     Py_ssize_t res = (Py_ssize_t)self->queue->length;
     PyThread_release_lock(self->lock);
     return res;
```

### Comparing `fastqueue-lib-0.0.5/tests/test_queue.py` & `fastqueue-lib-0.0.6/tests/test_queue.py`

 * *Files identical despite different names*

