# Comparing `tmp/grapes-graph-0.0.2.tar.gz` & `tmp/grapes-graph-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grapes-graph-0.0.2.tar", last modified: Tue Jul 25 00:07:11 2023, max compression
+gzip compressed data, was "grapes-graph-0.0.3.tar", last modified: Mon Jul 31 03:13:09 2023, max compression
```

## Comparing `grapes-graph-0.0.2.tar` & `grapes-graph-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 ericwang   (501) staff       (20)        0 2023-07-25 00:07:11.983910 grapes-graph-0.0.2/
--rw-r--r--   0 ericwang   (501) staff       (20)     1069 2023-07-23 02:02:04.000000 grapes-graph-0.0.2/LICENSE.txt
--rw-r--r--   0 ericwang   (501) staff       (20)       27 2023-07-24 20:57:07.000000 grapes-graph-0.0.2/MANIFEST.in
--rw-r--r--   0 ericwang   (501) staff       (20)      808 2023-07-25 00:07:11.983776 grapes-graph-0.0.2/PKG-INFO
--rw-r--r--   0 ericwang   (501) staff       (20)      128 2023-07-24 23:13:12.000000 grapes-graph-0.0.2/README.md
--rw-r--r--   0 ericwang   (501) staff       (20)      896 2023-07-25 00:05:22.000000 grapes-graph-0.0.2/pyproject.toml
--rw-r--r--   0 ericwang   (501) staff       (20)       24 2023-07-24 23:55:23.000000 grapes-graph-0.0.2/requirements.txt
--rw-r--r--   0 ericwang   (501) staff       (20)       38 2023-07-25 00:07:11.983948 grapes-graph-0.0.2/setup.cfg
--rw-r--r--   0 ericwang   (501) staff       (20)      208 2023-07-24 20:57:29.000000 grapes-graph-0.0.2/setup.py
-drwxr-xr-x   0 ericwang   (501) staff       (20)        0 2023-07-25 00:07:11.980259 grapes-graph-0.0.2/src/
-drwxr-xr-x   0 ericwang   (501) staff       (20)        0 2023-07-25 00:07:11.981580 grapes-graph-0.0.2/src/grapes/
--rw-r--r--   0 ericwang   (501) staff       (20)       43 2023-07-24 19:27:07.000000 grapes-graph-0.0.2/src/grapes/__init__.py
-drwxr-xr-x   0 ericwang   (501) staff       (20)        0 2023-07-25 00:07:11.982728 grapes-graph-0.0.2/src/grapes/cgraph/
--rw-r--r--   0 ericwang   (501) staff       (20)     1682 2023-07-24 23:52:20.000000 grapes-graph-0.0.2/src/grapes/cgraph/__init__.pyi
--rw-r--r--   0 ericwang   (501) staff       (20)    13485 2023-07-24 20:14:45.000000 grapes-graph-0.0.2/src/grapes/cgraph/cgraph.c
--rw-r--r--   0 ericwang   (501) staff       (20)     1058 2023-07-24 19:26:38.000000 grapes-graph-0.0.2/src/grapes/cgraph/cgraph.h
--rw-r--r--   0 ericwang   (501) staff       (20)     3040 2023-07-22 23:29:47.000000 grapes-graph-0.0.2/src/grapes/cgraph/heap.c
--rw-r--r--   0 ericwang   (501) staff       (20)      559 2023-07-22 23:29:49.000000 grapes-graph-0.0.2/src/grapes/cgraph/heap.h
-drwxr-xr-x   0 ericwang   (501) staff       (20)        0 2023-07-25 00:07:11.983491 grapes-graph-0.0.2/src/grapes_graph.egg-info/
--rw-r--r--   0 ericwang   (501) staff       (20)      808 2023-07-25 00:07:11.000000 grapes-graph-0.0.2/src/grapes_graph.egg-info/PKG-INFO
--rw-r--r--   0 ericwang   (501) staff       (20)      454 2023-07-25 00:07:11.000000 grapes-graph-0.0.2/src/grapes_graph.egg-info/SOURCES.txt
--rw-r--r--   0 ericwang   (501) staff       (20)        1 2023-07-25 00:07:11.000000 grapes-graph-0.0.2/src/grapes_graph.egg-info/dependency_links.txt
--rw-r--r--   0 ericwang   (501) staff       (20)       25 2023-07-25 00:07:11.000000 grapes-graph-0.0.2/src/grapes_graph.egg-info/requires.txt
--rw-r--r--   0 ericwang   (501) staff       (20)       14 2023-07-25 00:07:11.000000 grapes-graph-0.0.2/src/grapes_graph.egg-info/top_level.txt
-drwxr-xr-x   0 ericwang   (501) staff       (20)        0 2023-07-25 00:07:11.983611 grapes-graph-0.0.2/tests/
--rw-r--r--   0 ericwang   (501) staff       (20)      248 2023-07-23 01:49:03.000000 grapes-graph-0.0.2/tests/test_dijkstra.py
+drwxr-xr-x   0 ericwang   (501) staff       (20)        0 2023-07-31 03:13:09.113387 grapes-graph-0.0.3/
+-rw-r--r--   0 ericwang   (501) staff       (20)     1069 2023-07-23 02:02:04.000000 grapes-graph-0.0.3/LICENSE.txt
+-rw-r--r--   0 ericwang   (501) staff       (20)       27 2023-07-24 20:57:07.000000 grapes-graph-0.0.3/MANIFEST.in
+-rw-r--r--   0 ericwang   (501) staff       (20)      783 2023-07-31 03:13:09.113222 grapes-graph-0.0.3/PKG-INFO
+-rw-r--r--   0 ericwang   (501) staff       (20)      153 2023-07-31 01:25:30.000000 grapes-graph-0.0.3/README.md
+-rw-r--r--   0 ericwang   (501) staff       (20)      851 2023-07-31 03:12:23.000000 grapes-graph-0.0.3/pyproject.toml
+-rw-r--r--   0 ericwang   (501) staff       (20)       24 2023-07-24 23:55:23.000000 grapes-graph-0.0.3/requirements.txt
+-rw-r--r--   0 ericwang   (501) staff       (20)       38 2023-07-31 03:13:09.113441 grapes-graph-0.0.3/setup.cfg
+-rw-r--r--   0 ericwang   (501) staff       (20)      268 2023-07-30 05:43:41.000000 grapes-graph-0.0.3/setup.py
+drwxr-xr-x   0 ericwang   (501) staff       (20)        0 2023-07-31 03:13:09.108455 grapes-graph-0.0.3/src/
+drwxr-xr-x   0 ericwang   (501) staff       (20)        0 2023-07-31 03:13:09.109688 grapes-graph-0.0.3/src/grapes/
+-rw-r--r--   0 ericwang   (501) staff       (20)       43 2023-07-24 19:27:07.000000 grapes-graph-0.0.3/src/grapes/__init__.py
+drwxr-xr-x   0 ericwang   (501) staff       (20)        0 2023-07-31 03:13:09.111817 grapes-graph-0.0.3/src/grapes/cgraph/
+-rw-r--r--   0 ericwang   (501) staff       (20)     2668 2023-07-31 03:03:53.000000 grapes-graph-0.0.3/src/grapes/cgraph/__init__.pyi
+-rw-r--r--   0 ericwang   (501) staff       (20)    18397 2023-07-31 03:09:10.000000 grapes-graph-0.0.3/src/grapes/cgraph/cgraph.c
+-rw-r--r--   0 ericwang   (501) staff       (20)     2013 2023-07-31 03:08:41.000000 grapes-graph-0.0.3/src/grapes/cgraph/cgraph.h
+-rw-r--r--   0 ericwang   (501) staff       (20)     2331 2023-07-31 01:23:45.000000 grapes-graph-0.0.3/src/grapes/cgraph/deque.c
+-rw-r--r--   0 ericwang   (501) staff       (20)      579 2023-07-31 01:23:47.000000 grapes-graph-0.0.3/src/grapes/cgraph/deque.h
+-rw-r--r--   0 ericwang   (501) staff       (20)     2993 2023-07-31 01:23:50.000000 grapes-graph-0.0.3/src/grapes/cgraph/heap.c
+-rw-r--r--   0 ericwang   (501) staff       (20)      657 2023-07-31 01:23:52.000000 grapes-graph-0.0.3/src/grapes/cgraph/heap.h
+drwxr-xr-x   0 ericwang   (501) staff       (20)        0 2023-07-31 03:13:09.112900 grapes-graph-0.0.3/src/grapes_graph.egg-info/
+-rw-r--r--   0 ericwang   (501) staff       (20)      783 2023-07-31 03:13:09.000000 grapes-graph-0.0.3/src/grapes_graph.egg-info/PKG-INFO
+-rw-r--r--   0 ericwang   (501) staff       (20)      506 2023-07-31 03:13:09.000000 grapes-graph-0.0.3/src/grapes_graph.egg-info/SOURCES.txt
+-rw-r--r--   0 ericwang   (501) staff       (20)        1 2023-07-31 03:13:09.000000 grapes-graph-0.0.3/src/grapes_graph.egg-info/dependency_links.txt
+-rw-r--r--   0 ericwang   (501) staff       (20)       25 2023-07-31 03:13:09.000000 grapes-graph-0.0.3/src/grapes_graph.egg-info/requires.txt
+-rw-r--r--   0 ericwang   (501) staff       (20)       14 2023-07-31 03:13:09.000000 grapes-graph-0.0.3/src/grapes_graph.egg-info/top_level.txt
+drwxr-xr-x   0 ericwang   (501) staff       (20)        0 2023-07-31 03:13:09.113025 grapes-graph-0.0.3/tests/
+-rw-r--r--   0 ericwang   (501) staff       (20)      248 2023-07-23 01:49:03.000000 grapes-graph-0.0.3/tests/test_dijkstra.py
```

### Comparing `grapes-graph-0.0.2/LICENSE.txt` & `grapes-graph-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `grapes-graph-0.0.2/pyproject.toml` & `grapes-graph-0.0.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [build-system]
 requires = ["setuptools >= 63.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "grapes-graph"
-version = "0.0.2"
+version = "0.0.3"
 description = "Python graph library written in C"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 license = { text = "MIT License" }
 authors = [{ name = "Eric Wang", email = "ericwangyy@ucla.edu" }]
 keywords = ["graph"]
 classifiers = [
     "Development Status :: 1 - Planning",
     "Programming Language :: C",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
 ]
 dynamic = ["dependencies"]
```

### Comparing `grapes-graph-0.0.2/src/grapes/cgraph/__init__.pyi` & `grapes-graph-0.0.3/src/grapes/cgraph/__init__.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -19,14 +19,29 @@
         :type node_count: int
         """
     def get_node_count(self: Self) -> int:
         """Get the number of nodes in the graph.
 
         :rtype: int
         """
+    def get_edge_count(self: Self) -> int:
+        """Get the number of edges in the graph.
+
+        :rtype: int
+        """
+    def get_edges(self: Self) -> list[tuple[int, int]]:
+        """Get the edges in the graph.
+
+        .. warning::
+            If (u, v) is in edges, (v, u) will not also be returned. However,
+            duplicate inserted edges will still be duplicated.
+
+        :returns: List of edges
+        :rtype: list[tuple[int, int]]
+        """
     def add_node(self: Self) -> int:
         """Add a node to the graph.
 
         :returns: The index to the new node added.
         :rtype: int
         """
     def add_edge(self: Self, u: int, v: int) -> None:
@@ -42,16 +57,33 @@
         :rtype: None
         """
     def dijkstra_path(
         self: Self, src: int, dst: int, weight: Callable[[int, int], float]
     ) -> list[int]:
         """Get the shortest path in the graph using Dijkstra's algorithm.
 
+        .. note::
+            The weight function should accept both (u, v) and (v, u) as
+            potential inputs.
+
         :param src: Begin (source) node
         :type src: int
         :param dst: End (destination) node
         :type dst: int
-        :param weight: Weight function that accepts two integers and returns the weight as a float.
+        :param weight: Weight function that accepts two nodes and returns the
+            weight as a float.
         :type weight: Callable[[int, int], float]
-        :return: List of nodes, starting from `src` and ending with `dst`. Returns an empty list if no path found.
+        :return: List of nodes, starting from `src` and ending with `dst`.
+            Returns an empty list if no path found.
+        :rtype: list[int]
+        """
+    def get_component_sizes(self: Self) -> list[int]:
+        """Return the sizes of the (connected) components in the graph.
+
         :rtype: list[int]
         """
+    def is_bipartite(self: Self) -> bool:
+        """Return whether the graph is bipartite or not.
+
+        :returns: Returns `True` if the graph is bipartite; otherwise, `False`.
+        :rtype: bool
+        """
```

### Comparing `grapes-graph-0.0.2/src/grapes/cgraph/cgraph.c` & `grapes-graph-0.0.3/src/grapes/cgraph/cgraph.c`

 * *Files 20% similar despite different names*

```diff
@@ -1,450 +1,595 @@
 #define PY_SSIZE_T_CLEAN
 #include <Python.h>
 
 #include "cgraph.h"
 
+#include "deque.h"
 #include "heap.h"
 
-PyMODINIT_FUNC PyInit_cgraph(void)
+PyMODINIT_FUNC
+PyInit_cgraph(void)
 {
-    PyObject* m;
-    if (PyType_Ready(&GraphType) < 0)
-    {
+    PyObject *m;
+    if (PyType_Ready(&GraphType) < 0) {
         return NULL;
     }
 
     m = PyModule_Create(&cgraphmodule);
-    if (m == NULL)
-    {
+    if (m == NULL) {
         return NULL;
     }
 
     Py_INCREF(&GraphType);
-    if (PyModule_AddObject(m, "Graph", (PyObject*) &GraphType) < 0)
-    {
+    if (PyModule_AddObject(m, "Graph", (PyObject *) &GraphType) < 0) {
         Py_DECREF(&GraphType);
         Py_DECREF(m);
         return NULL;
     }
 
     return m;
 }
 
 static struct PyModuleDef cgraphmodule = {
-    // clang-format off
     PyModuleDef_HEAD_INIT,
     .m_name = "cgraph",
     .m_doc = PyDoc_STR("Grapes core functionality written in C"),
     .m_size = -1,
-}; // clang-format on
+};
 
-typedef struct GraphObject
-{ // clang-format off
-    PyObject_HEAD
-    Py_ssize_t** adj_list; // list of adjacency lists (adj_list[i] = array of neighbors to node i)
-    Py_ssize_t node_count;
-    Py_ssize_t max_node_count; // current maximum number of nodes allocated
-    Py_ssize_t* neighbor_count;
-    Py_ssize_t* max_neighbor_count; // current maximum number of neighbors (max_neighbor_count[i] = current maximum number of neighbors allocated to node i)
-} GraphObject; // clang-format on
+typedef struct GraphObject {
+    PyObject_HEAD Py_ssize_t *
+        *adj_list;  // list of adjacency lists (adj_list[i]
+                    // = array of neighbors to node i)
+    Py_ssize_t  node_count;
+    Py_ssize_t  max_node_count;  // current maximum number of nodes allocated
+    Py_ssize_t *neighbor_count;
+    Py_ssize_t
+        *max_neighbor_count;  // current maximum number of neighbors
+                              // (max_neighbor_count[i] = current maximum
+                              // number of neighbors allocated to node i)
+    Py_ssize_t edge_count;
+} GraphObject;
 
-// clang-format off
 static PyTypeObject GraphType = {
-    PyVarObject_HEAD_INIT(NULL, 0)
-    .tp_name = "grapes.cgraph.Graph",
+    PyVarObject_HEAD_INIT(NULL, 0).tp_name = "grapes.cgraph.Graph",
     .tp_doc = PyDoc_STR("Undirected graph object."),
     .tp_basicsize = sizeof(GraphObject),
     .tp_itemsize = 0,
     .tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_BASETYPE,
     .tp_dealloc = (destructor) Graph_dealloc,
     .tp_new = Graph_new,
     .tp_init = (initproc) Graph_init,
     .tp_methods = Graph_methods,
 };
-// clang-format on
 
-static void Graph_dealloc(GraphObject* self)
+static void
+Graph_dealloc(GraphObject *self)
 {
-    for (Py_ssize_t i = 0; i < self->max_node_count; ++i)
-    {
+    for (Py_ssize_t i = 0; i < self->max_node_count; ++i) {
         free(self->adj_list[i]);
         self->adj_list[i] = NULL;
     }
     free(self->adj_list);
     self->adj_list = NULL;
     free(self->neighbor_count);
     self->neighbor_count = NULL;
     free(self->max_neighbor_count);
     self->max_neighbor_count = NULL;
-    Py_TYPE(self)->tp_free((PyObject*) self);
+    Py_TYPE(self)->tp_free((PyObject *) self);
 }
 
-static PyObject* Graph_new(PyTypeObject* type, PyObject* args, PyObject* kwds)
+static PyObject *
+Graph_new(PyTypeObject *type, PyObject *args, PyObject *kwds)
 {
-    GraphObject* self;
-    self = (GraphObject*) type->tp_alloc(type, 0);
-    if (self != NULL)
-    {
+    GraphObject *self;
+    self = (GraphObject *) type->tp_alloc(type, 0);
+    if (self != NULL) {
         self->adj_list = NULL;
         self->node_count = 0;
         self->max_node_count = 0;
         self->neighbor_count = NULL;
         self->max_neighbor_count = NULL;
+        self->edge_count = 0;
     }
-    return (PyObject*) self;
+    return (PyObject *) self;
 }
 
-static int Graph_init(GraphObject* self, PyObject* args, PyObject* kwds)
+static int
+Graph_init(GraphObject *self, PyObject *args, PyObject *kwds)
 {
-    static char* kwlist[] = {"node_count", NULL};
+    static char *kwlist[] = {"node_count", NULL};
     Py_ssize_t   node_count;
-    if (!PyArg_ParseTupleAndKeywords(args, kwds, "n", kwlist, &node_count))
-    {
+    if (!PyArg_ParseTupleAndKeywords(args, kwds, "n", kwlist, &node_count)) {
         return -1;
     }
 
-    if (node_count < 0)
-    {
+    if (node_count < 0) {
         PyErr_Format(PyExc_ValueError,
                      "node_count should be nonnegative, but given %ld",
                      node_count);
         return -1;
     }
 
     self->adj_list = malloc(sizeof(*self->adj_list) * node_count);
-    if (self->adj_list == NULL)
-    {
+    if (self->adj_list == NULL) {
         PyErr_Format(PyExc_MemoryError,
                      "Unable to malloc adj_list at memory address %p",
-                     (void*) self->adj_list);
+                     (void *) self->adj_list);
         return -1;
     }
-    for (Py_ssize_t i = 0; i < node_count; ++i)
-    {
+    for (Py_ssize_t i = 0; i < node_count; ++i) {
         self->adj_list[i] = NULL;
     }
 
     self->node_count = node_count;
     self->max_node_count = node_count;
 
     self->neighbor_count = malloc(sizeof(*self->neighbor_count) * node_count);
-    if (self->neighbor_count == NULL)
-    {
+    if (self->neighbor_count == NULL) {
         PyErr_Format(PyExc_MemoryError,
                      "Unable to malloc neighbor_count at memory address %p",
-                     (void*) self->neighbor_count);
+                     (void *) self->neighbor_count);
         return -1;
     }
-    for (Py_ssize_t i = 0; i < node_count; ++i)
-    {
+    for (Py_ssize_t i = 0; i < node_count; ++i) {
         self->neighbor_count[i] = 0;
     }
 
     self->max_neighbor_count =
         malloc(sizeof(*self->max_neighbor_count) * node_count);
-    if (self->max_neighbor_count == NULL)
-    {
-        PyErr_Format(PyExc_MemoryError,
-                     "Unable to malloc max_neighbor_count at memory address %p",
-                     (void*) self->max_neighbor_count);
+    if (self->max_neighbor_count == NULL) {
+        PyErr_Format(
+            PyExc_MemoryError,
+            "Unable to malloc max_neighbor_count at memory address %p",
+            (void *) self->max_neighbor_count);
         return -1;
     }
-    for (Py_ssize_t i = 0; i < node_count; ++i)
-    {
+    for (Py_ssize_t i = 0; i < node_count; ++i) {
         self->max_neighbor_count[i] = 0;
     }
+
+    self->edge_count = 0;
+
     return 0;
 }
 
-// clang-format off
 static PyMethodDef Graph_methods[] = {
-    {"get_node_count", (PyCFunction) Graph_get_node_count, METH_NOARGS, 
-     "Return the number of nodes in the graph."
-    },
-    {"add_node", (PyCFunction) Graph_add_node, METH_NOARGS, 
+    {"get_node_count", (PyCFunction) Graph_get_node_count, METH_NOARGS,
+     "Return the number of nodes in the graph."},
+    {"get_edge_count", (PyCFunction) Graph_get_edge_count, METH_NOARGS,
+     "Return the number of edges in the graph."},
+    {"get_edges", (PyCFunction) Graph_get_edges, METH_NOARGS,
+     "Return the edges in the graph."},
+    {"add_node", (PyCFunction) Graph_add_node, METH_NOARGS,
      "Add a node to the graph, returning the newest node."},
     {"add_edge", (PyCFunction) Graph_add_edge, METH_VARARGS | METH_KEYWORDS,
      "Add an undirected edge to the graph given existing nodes."},
-    {"dijkstra_path", (PyCFunction) Graph_dijkstra_path, METH_VARARGS | METH_KEYWORDS,
+    {"dijkstra_path", (PyCFunction) Graph_dijkstra_path,
+     METH_VARARGS | METH_KEYWORDS,
      "Find the shortest path between two nodes using Dijkstra's algorithm"},
-    {NULL}
-};
-// clang-format on
+    {"get_component_sizes", (PyCFunction) Graph_get_component_sizes,
+     METH_NOARGS, "Return the sizes of the components in the graph."},
+    {"is_bipartite", (PyCFunction) Graph_is_bipartite, METH_NOARGS,
+     "Return whether the graph is bipartite or not."},
+    {NULL}};
 
-static PyObject* Graph_get_node_count(GraphObject* self,
-                                      PyObject*    Py_UNUSED(ignored))
+static PyObject *
+Graph_get_node_count(GraphObject *self, PyObject *Py_UNUSED(ignored))
 {
     return PyLong_FromSsize_t(self->node_count);
 }
 
-static PyObject* Graph_add_node(GraphObject* self, PyObject* Py_UNUSED(ignored))
+static PyObject *
+Graph_get_edge_count(GraphObject *self, PyObject *Py_UNUSED(ignored))
+{
+    return PyLong_FromSsize_t(self->edge_count);
+}
+
+static PyObject *
+Graph_get_edges(GraphObject *self, PyObject *Py_UNUSED(ignored))
+{
+    PyObject *edges = PyList_New(self->edge_count);
+    if (edges == NULL) {
+        PyErr_SetString(PyExc_MemoryError, "Unable to initialize edges list");
+    }
+
+    Py_ssize_t i = 0;
+    PyObject  *uv;
+    for (Py_ssize_t u = 0; u < self->node_count; ++u) {
+        for (Py_ssize_t j = 0; j < self->neighbor_count[u]; ++j) {
+            Py_ssize_t v = self->adj_list[u][j];
+            if (u > v) {
+                continue;
+            }
+            uv = Py_BuildValue("(nn)", u, v);
+            if (uv == NULL) {
+                PyErr_Format(PyExc_TypeError,
+                             "Unable to format uv given u=%ld and v=%ld", u,
+                             v);
+                return NULL;
+            }
+            if (PyList_SetItem(edges, i, uv) == -1) {
+                return NULL;
+            }
+            ++i;
+        }
+    }
+    return edges;
+}
+
+static PyObject *
+Graph_add_node(GraphObject *self, PyObject *Py_UNUSED(ignored))
 {
-    if (self->node_count >= self->max_node_count)
-    {
+    if (self->node_count >= self->max_node_count) {
         // approximately a growth factor of 112.5%
         self->max_node_count =
             (self->max_node_count + (self->max_node_count >> 3) + 6) &
             (~(Py_ssize_t) 3);
-        self->adj_list = realloc(self->adj_list, sizeof(*self->adj_list) *
-                                                     self->max_node_count);
-        if (self->adj_list == NULL)
-        {
+        self->adj_list = realloc(
+            self->adj_list, sizeof(*self->adj_list) * self->max_node_count);
+        if (self->adj_list == NULL) {
             PyErr_Format(PyExc_MemoryError,
                          "Unable to realloc adj_list at memory address %p",
-                         (void*) self->adj_list);
+                         (void *) self->adj_list);
             return NULL;
         }
-        for (Py_ssize_t i = self->node_count; i < self->max_node_count; ++i)
-        {
+        for (Py_ssize_t i = self->node_count; i < self->max_node_count; ++i) {
             self->adj_list[i] = NULL;
         }
 
         self->neighbor_count =
             realloc(self->neighbor_count,
                     sizeof(*self->neighbor_count) * self->max_node_count);
-        if (self->neighbor_count == NULL)
-        {
+        if (self->neighbor_count == NULL) {
             PyErr_Format(
                 PyExc_MemoryError,
                 "Unable to realloc neighbor_count at memory address %p",
-                (void*) self->neighbor_count);
+                (void *) self->neighbor_count);
             return NULL;
         }
-        for (Py_ssize_t i = self->node_count; i < self->max_node_count; ++i)
-        {
+        for (Py_ssize_t i = self->node_count; i < self->max_node_count; ++i) {
             self->neighbor_count[i] = 0;
         }
 
         self->max_neighbor_count =
             realloc(self->max_neighbor_count,
                     sizeof(*self->max_neighbor_count) * self->max_node_count);
-        if (self->max_neighbor_count == NULL)
-        {
+        if (self->max_neighbor_count == NULL) {
             PyErr_Format(
                 PyExc_MemoryError,
                 "Unable to realloc max_neighbor_count at memory address %p",
-                (void*) self->max_neighbor_count);
+                (void *) self->max_neighbor_count);
             return NULL;
         }
-        for (Py_ssize_t i = self->node_count; i < self->max_node_count; ++i)
-        {
+        for (Py_ssize_t i = self->node_count; i < self->max_node_count; ++i) {
             self->max_neighbor_count[i] = 0;
         }
     }
 
     return PyLong_FromSsize_t(self->node_count++);
 }
 
-static PyObject* Graph_add_edge(GraphObject* self, PyObject* args,
-                                PyObject* kwds)
+static PyObject *
+Graph_add_edge(GraphObject *self, PyObject *args, PyObject *kwds)
 {
-    static char* kwlist[] = {"u", "v", NULL};
+    static char *kwlist[] = {"u", "v", NULL};
     Py_ssize_t   u, v;
 
-    if (!PyArg_ParseTupleAndKeywords(args, kwds, "nn", kwlist, &u, &v))
-    {
+    if (!PyArg_ParseTupleAndKeywords(args, kwds, "nn", kwlist, &u, &v)) {
         return NULL;
     }
 
-    if (u < 0 || u >= self->node_count || v < 0 || v >= self->node_count)
-    {
+    if (u < 0 || u >= self->node_count || v < 0 || v >= self->node_count) {
         PyErr_Format(PyExc_ValueError,
                      "u and v should be existing nodes. Graph has "
                      "node_count=%ld but given u=%ld and v=%ld",
                      self->node_count, u, v);
         return NULL;
     }
 
-    if (self->neighbor_count[u] >= self->max_neighbor_count[u])
-    {
-        self->max_neighbor_count[u] = (self->max_neighbor_count[u] +
-                                       (self->max_neighbor_count[u] >> 3) + 6) &
-                                      (~(Py_ssize_t) 3);
+    if (self->neighbor_count[u] >= self->max_neighbor_count[u]) {
+        self->max_neighbor_count[u] =
+            (self->max_neighbor_count[u] + (self->max_neighbor_count[u] >> 3) +
+             6) &
+            (~(Py_ssize_t) 3);
         self->adj_list[u] =
             realloc(self->adj_list[u],
                     sizeof(*self->adj_list[u]) * self->max_neighbor_count[u]);
-        if (self->adj_list[u] == NULL)
-        {
+        if (self->adj_list[u] == NULL) {
             PyErr_Format(PyExc_MemoryError,
                          "Unable to realloc adj_list[u] at memory address %p "
                          "with u=%ld",
-                         (void*) self->adj_list[u], u);
+                         (void *) self->adj_list[u], u);
             return NULL;
         }
     }
     self->adj_list[u][self->neighbor_count[u]++] = v;
 
-    if (self->neighbor_count[v] >= self->max_neighbor_count[v])
-    {
-        self->max_neighbor_count[v] = (self->max_neighbor_count[v] +
-                                       (self->max_neighbor_count[v] >> 3) + 6) &
-                                      (~(Py_ssize_t) 3);
+    if (self->neighbor_count[v] >= self->max_neighbor_count[v]) {
+        self->max_neighbor_count[v] =
+            (self->max_neighbor_count[v] + (self->max_neighbor_count[v] >> 3) +
+             6) &
+            (~(Py_ssize_t) 3);
         self->adj_list[v] =
             realloc(self->adj_list[v],
                     sizeof(*self->adj_list[v]) * self->max_neighbor_count[v]);
-        if (self->adj_list[v] == NULL)
-        {
+        if (self->adj_list[v] == NULL) {
             PyErr_Format(PyExc_MemoryError,
                          "Unable to realloc adj_list[v] at memory address %p "
                          "with v=%ld",
-                         (void*) self->adj_list[v], v);
+                         (void *) self->adj_list[v], v);
             return NULL;
         }
     }
     self->adj_list[v][self->neighbor_count[v]++] = u;
 
+    ++self->edge_count;
+
     Py_RETURN_NONE;
 }
 
-static PyObject* Graph_dijkstra_path(GraphObject* self, PyObject* args,
-                                     PyObject* kwds)
+static PyObject *
+Graph_dijkstra_path(GraphObject *self, PyObject *args, PyObject *kwds)
 {
-    static char* kwlist[] = {"src", "dst", "weight", NULL};
+    static char *kwlist[] = {"src", "dst", "weight", NULL};
     Py_ssize_t   src, dst;
-    PyObject*    weight = NULL;
+    PyObject    *weight = NULL;
 
     if (!PyArg_ParseTupleAndKeywords(args, kwds, "nnO", kwlist, &src, &dst,
-                                     &weight))
-    {
+                                     &weight)) {
         return NULL;
     }
 
-    if (!PyCallable_Check(weight))
-    {
+    if (!PyCallable_Check(weight)) {
         PyErr_SetString(PyExc_TypeError, "weight must be callable.");
         return NULL;
     }
 
-    Py_ssize_t* dist = malloc(sizeof(*dist) * self->node_count);
-    if (dist == NULL)
-    {
+    Py_ssize_t *dist = malloc(sizeof(*dist) * self->node_count);
+    if (dist == NULL) {
         PyErr_Format(PyExc_MemoryError,
                      "Unable to malloc dist at memory address %p",
-                     (void*) dist);
+                     (void *) dist);
         return NULL;
     }
 
-    short* visited = malloc(sizeof(*visited) * self->node_count);
-    if (visited == NULL)
-    {
+    short *visited = malloc(sizeof(*visited) * self->node_count);
+    if (visited == NULL) {
         PyErr_Format(PyExc_MemoryError,
                      "Unable to malloc visited at memory address %p",
-                     (void*) visited);
+                     (void *) visited);
         return NULL;
     }
 
-    Py_ssize_t* prev = malloc(sizeof(*prev) * self->node_count);
-    if (prev == NULL)
-    {
+    Py_ssize_t *prev = malloc(sizeof(*prev) * self->node_count);
+    if (prev == NULL) {
         PyErr_Format(PyExc_MemoryError,
                      "Unable to malloc prev at memory address %p",
-                     (void*) prev);
+                     (void *) prev);
         return NULL;
     }
 
-    for (Py_ssize_t i = 0; i < self->node_count; ++i)
-    {
+    for (Py_ssize_t i = 0; i < self->node_count; ++i) {
         dist[i] = PY_SSIZE_T_MAX;
-        visited[i] = 0;
+        visited[i] = GRAPES_FALSE;
         prev[i] = self->node_count;
     }
     dist[src] = 0;
-    visited[src] = 1;
+    visited[src] = GRAPES_TRUE;
     prev[src] = src;
 
-    MinHeap* heap =
+    MinHeap *heap =
         MinHeap_alloc((self->node_count * (self->node_count - 1)) / 2);
     MinHeap_insert(heap, src, 0);
     Py_ssize_t u, v;
     double     w;
-    PyObject*  uvargs;
-    PyObject*  ret_value;
-    while (!MinHeap_is_empty(heap))
-    {
+    while (!MinHeap_is_empty(heap)) {
         u = MinHeap_extract_min(heap);
-        visited[u] = 1;
-        for (Py_ssize_t i = 0; i < self->neighbor_count[u]; ++i)
-        {
+        visited[u] = GRAPES_TRUE;
+        for (Py_ssize_t i = 0; i < self->neighbor_count[u]; ++i) {
             v = self->adj_list[u][i];
-            if (visited[v])
-            {
+            if (visited[v]) {
                 continue;
             }
-            uvargs = Py_BuildValue("(nn)", u, v);
-            if (args == NULL)
-            {
-                PyErr_Format(PyExc_TypeError,
-                             "Unable to format args given u=%ld and v=%ld", u,
-                             v);
-                return NULL;
-            }
-            ret_value = PyObject_Call(weight, uvargs, NULL);
-            if (ret_value == NULL)
-            {
-                PyErr_Format(PyExc_TypeError,
-                             "Unable to call weight function on args given "
-                             "weight=%R and args=%R",
-                             weight, args);
-                return NULL;
-            }
-            w = PyFloat_AsDouble(ret_value);
-            if (w == -1 && PyErr_Occurred() != NULL)
-            {
-                PyErr_Format(PyExc_ValueError,
-                             "weight function returned a non-float value "
-                             "given ret_value=%R",
-                             ret_value);
+            w = get_weight(weight, u, v);
+            if (w == -1 && PyErr_Occurred() != NULL) {
                 return NULL;
             }
 
-            if (dist[v] - dist[u] > w)
-            {
+            if (dist[v] - dist[u] > w) {
                 dist[v] = dist[u] + w;
                 prev[v] = u;
                 MinHeap_insert(heap, v, dist[v]);
             }
         }
     }
 
-    PyObject* path = PyList_New(0);
-    if (path == NULL)
-    {
+    PyObject *path = PyList_New(0);
+    if (path == NULL) {
         PyErr_SetString(PyExc_MemoryError, "Unable to initialize path");
     }
-    if (prev[dst] == self->node_count)
-    {
+    if (prev[dst] == self->node_count) {
         return path;
     }
 
-    if (PyList_Append(path, PyLong_FromSsize_t(dst)) == -1)
-    {
-
+    if (PyList_Append(path, PyLong_FromSsize_t(dst)) == -1) {
         return NULL;
     }
     Py_ssize_t curr = dst;
-    do
-    {
+    do {
         curr = prev[curr];
-        if (PyList_Append(path, PyLong_FromSsize_t(curr)) == -1)
-        {
-
+        if (PyList_Append(path, PyLong_FromSsize_t(curr)) == -1) {
             return NULL;
         }
     } while (curr != src);
 
-    if (PyList_Reverse(path) == -1)
-    {
+    if (PyList_Reverse(path) == -1) {
         return NULL;
     }
 
     free(dist);
     dist = NULL;
     free(visited);
     visited = NULL;
     free(prev);
     prev = NULL;
     MinHeap_free(heap);
     heap = NULL;
 
     return path;
 }
+
+static PyObject *
+Graph_get_component_sizes(GraphObject *self, PyObject *args, PyObject *kwds)
+{
+    Py_ssize_t *sizes = malloc(sizeof(*sizes) * self->node_count);
+    if (sizes == NULL) {
+        PyErr_Format(PyExc_MemoryError,
+                     "Unable to malloc sizes at memory address %p",
+                     (void *) sizes);
+        return NULL;
+    }
+    short *visited = malloc(sizeof(*visited) * self->node_count);
+    if (visited == NULL) {
+        PyErr_Format(PyExc_MemoryError,
+                     "Unable to malloc visited at memory address %p",
+                     (void *) visited);
+        return NULL;
+    }
+    for (Py_ssize_t i = 0; i < self->node_count; ++i) {
+        sizes[i] = 0;
+        visited[i] = GRAPES_FALSE;
+    }
+
+    Py_ssize_t count = 0;
+    for (Py_ssize_t i = 0; i < self->node_count; ++i) {
+        if (!visited[i]) {
+            sizes[count++] = visit(self, i, visited);
+        }
+    }
+
+    PyObject *component_sizes = PyList_New(count);
+    if (component_sizes == NULL) {
+        PyErr_SetString(PyExc_MemoryError,
+                        "Unable to initialize component_sizes");
+    }
+
+    for (Py_ssize_t i = 0; i < count; ++i) {
+        if (PyList_SetItem(component_sizes, i, PyLong_FromSsize_t(sizes[i])) ==
+            -1) {
+            return NULL;
+        }
+    }
+
+    free(sizes);
+    sizes = NULL;
+    free(visited);
+    visited = NULL;
+    return component_sizes;
+}
+
+static PyObject *
+Graph_is_bipartite(GraphObject *self, PyObject *args, PyObject *kwds)
+{
+    short *color = malloc(sizeof(*color) * self->node_count);
+    if (color == NULL) {
+        PyErr_Format(PyExc_MemoryError,
+                     "Unable to malloc color at memory address %p",
+                     (void *) color);
+        return NULL;
+    }
+    for (Py_ssize_t i = 0; i < self->node_count; ++i) {
+        color[i] = GRAPES_NO_COLOR;
+    }
+
+    for (Py_ssize_t i = 0; i < self->node_count; ++i) {
+        if (!visit_color(self, i, color)) {
+            Py_RETURN_FALSE;
+        }
+    }
+    Py_RETURN_TRUE;
+}
+
+double
+get_weight(PyObject *weight, Py_ssize_t u, Py_ssize_t v)
+{
+    const int failed = -1;
+    double    w;
+    PyObject *uvargs;
+    PyObject *ret_value;
+
+    uvargs = Py_BuildValue("(nn)", u, v);
+    if (uvargs == NULL) {
+        PyErr_Format(PyExc_TypeError,
+                     "Unable to format args given u=%ld and v=%ld", u, v);
+        return failed;
+    }
+    ret_value = PyObject_Call(weight, uvargs, NULL);
+    if (ret_value == NULL) {
+        PyErr_Format(PyExc_TypeError,
+                     "Unable to call weight function on args given "
+                     "weight=%R and uvargs=%R",
+                     weight, uvargs);
+        return failed;
+    }
+    w = PyFloat_AsDouble(ret_value);
+    if (w == -1 && PyErr_Occurred() != NULL) {
+        PyErr_Format(PyExc_ValueError,
+                     "weight function returned a non-float value "
+                     "given ret_value=%R",
+                     ret_value);
+        return failed;
+    }
+
+    return w;
+}
+
+Py_ssize_t
+visit(GraphObject *graph, Py_ssize_t src, short *visited)
+{
+    visited[src] = GRAPES_TRUE;
+    Py_ssize_t size = 1;
+    Deque     *queue = Deque_alloc();  // push_back, pop_front
+    Deque_push_back(queue, src);
+    while (!Deque_is_empty(queue)) {
+        Py_ssize_t curr = Deque_pop_front(queue);
+        for (Py_ssize_t j = 0; j < graph->neighbor_count[curr]; ++j) {
+            Py_ssize_t neighbor = graph->adj_list[curr][j];
+            if (!visited[neighbor]) {
+                visited[neighbor] = GRAPES_TRUE;
+                ++size;
+                Deque_push_back(queue, neighbor);
+            }
+        }
+    }
+    Deque_free(queue);
+    return size;
+}
+
+short
+visit_color(GraphObject *graph, Py_ssize_t src, short *color)
+{
+    if (color[src] != GRAPES_NO_COLOR) {
+        return GRAPES_TRUE;
+    }
+    color[src] = GRAPES_RED;
+    Deque *queue = Deque_alloc();  // push_back, pop_front
+    Deque_push_back(queue, src);
+    while (!Deque_is_empty(queue)) {
+        Py_ssize_t curr = Deque_pop_front(queue);
+        for (Py_ssize_t j = 0; j < graph->neighbor_count[curr]; ++j) {
+            Py_ssize_t neighbor = graph->adj_list[curr][j];
+            if (color[neighbor] == GRAPES_NO_COLOR) {
+                color[neighbor] =
+                    (color[curr] == GRAPES_RED) ? GRAPES_BLUE : GRAPES_RED;
+                Deque_push_back(queue, neighbor);
+            }
+            else if (color[neighbor] == color[curr]) {
+                Deque_free(queue);
+                return GRAPES_FALSE;
+            }
+        }
+    }
+    Deque_free(queue);
+    return GRAPES_TRUE;
+}
```

### Comparing `grapes-graph-0.0.2/src/grapes/cgraph/heap.c` & `grapes-graph-0.0.3/src/grapes/cgraph/heap.c`

 * *Files 8% similar despite different names*

```diff
@@ -1,142 +1,138 @@
 #define PY_SSIZE_T_CLEAN
 #include <Python.h>
 
 #include "heap.h"
 
-typedef struct MinHeapNode
-{
+typedef struct MinHeapNode {
     Py_ssize_t priority;
     Py_ssize_t key;
 } MinHeapNode;
 
-typedef struct MinHeap
-{
+typedef struct MinHeap {
     Py_ssize_t   size;
     Py_ssize_t   max_size;
-    MinHeapNode* array;
+    MinHeapNode *array;
 } MinHeap;
 
-MinHeap* MinHeap_alloc(Py_ssize_t max_size)
+MinHeap *
+MinHeap_alloc(Py_ssize_t max_size)
 {
-    MinHeap* heap = malloc(sizeof(*heap));
-    if (heap == NULL)
-    {
+    MinHeap *heap = malloc(sizeof(*heap));
+    if (heap == NULL) {
         fprintf(stderr, "Failed to allocate heap\n");
         return NULL;
     }
 
     heap->size = 0;
     heap->max_size = max_size;
     heap->array = malloc(sizeof(*heap->array) * max_size);
-    if (heap->array == NULL)
-    {
+    if (heap->array == NULL) {
         fprintf(stderr, "Failed to allocate heap array\n");
         return NULL;
     }
 
     return heap;
 }
 
-void MinHeap_free(MinHeap* heap)
+void
+MinHeap_free(MinHeap *heap)
 {
-    if (heap == NULL)
-    {
+    if (heap == NULL) {
         return;
     }
 
     free(heap->array);
     heap->array = NULL;
     free(heap);
     heap = NULL;
     return;
 }
 
-void MinHeap_insert(MinHeap* heap, Py_ssize_t key, Py_ssize_t priority)
+void
+MinHeap_insert(MinHeap *heap, Py_ssize_t key, Py_ssize_t priority)
 {
-    if (heap->size >= heap->max_size)
-    {
+    if (heap->size >= heap->max_size) {
         fprintf(stderr, "Cannot insert key %ld. Heap is already full!\n", key);
         return;
     }
 
     Py_ssize_t i = heap->size++;
     heap->array[i].priority = priority;
     heap->array[i].key = key;
 
     MinHeap_siftdown(heap, 0, heap->size - 1);
     return;
 }
 
-Py_ssize_t MinHeap_extract_min(MinHeap* heap)
+Py_ssize_t
+MinHeap_extract_min(MinHeap *heap)
 {
-    if (heap == NULL || heap->size == 0)
-    {
+    if (heap == NULL || heap->size == 0) {
         return -1;
     }
 
     MinHeapNode lastelt = heap->array[--heap->size];
     Py_ssize_t  min_key = heap->array[0].key;
     heap->array[0] = lastelt;
     MinHeap_siftup(heap, 0);
     return min_key;
 }
 
-int MinHeap_is_empty(MinHeap* heap)
+int
+MinHeap_is_empty(MinHeap *heap)
 {
     return heap->size == 0;
 }
 
-void MinHeap_siftdown(MinHeap* heap, Py_ssize_t startpos, Py_ssize_t pos)
+void
+MinHeap_siftdown(MinHeap *heap, Py_ssize_t startpos, Py_ssize_t pos)
 {
     MinHeapNode newitem = heap->array[pos];
     Py_ssize_t  parentpos;
     MinHeapNode parent;
-    while (pos > startpos)
-    {
+    while (pos > startpos) {
         parentpos = (pos - 1) >> 1;
         parent = heap->array[parentpos];
-        if (newitem.priority < parent.priority)
-        {
+        if (newitem.priority < parent.priority) {
             heap->array[pos] = parent;
             pos = parentpos;
             continue;
         }
         break;
     }
     heap->array[pos] = newitem;
     return;
 }
 
-void MinHeap_siftup(MinHeap* heap, Py_ssize_t pos)
+void
+MinHeap_siftup(MinHeap *heap, Py_ssize_t pos)
 {
     Py_ssize_t  endpos = heap->size;
     Py_ssize_t  startpos = pos;
     MinHeapNode newitem = heap->array[pos];
     Py_ssize_t  childpos = 2 * pos + 1;
     Py_ssize_t  rightpos;
-    while (childpos < endpos)
-    {
+    while (childpos < endpos) {
         rightpos = childpos + 1;
         if (rightpos < endpos &&
-            heap->array[childpos].priority >= heap->array[rightpos].priority)
-        {
+            heap->array[childpos].priority >= heap->array[rightpos].priority) {
             childpos = rightpos;
         }
         heap->array[pos] = heap->array[childpos];
         pos = childpos;
         childpos = 2 * pos + 1;
     }
     heap->array[pos] = newitem;
     MinHeap_siftdown(heap, startpos, pos);
     return;
 }
 
-void MinHeap_print(MinHeap* heap)
+void
+MinHeap_print(MinHeap *heap)
 {
     printf("heap size=%ld values=", heap->size);
-    for (Py_ssize_t i = 0; i < heap->size; ++i)
-    {
+    for (Py_ssize_t i = 0; i < heap->size; ++i) {
         printf("%ld, ", heap->array[i].key);
     }
     printf("\n");
 }
```

### Comparing `grapes-graph-0.0.2/src/grapes/cgraph/heap.h` & `grapes-graph-0.0.3/src/grapes/cgraph/heap.h`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,19 @@
+#ifndef GRAPES_GRAPES_CGRAPH_HEAP_H_
+#define GRAPES_GRAPES_CGRAPH_HEAP_H_
+
 #define PY_SSIZE_T_CLEAN
 #include <Python.h>
 
 typedef struct MinHeapNode MinHeapNode;
 typedef struct MinHeap     MinHeap;
 
-MinHeap*   MinHeap_alloc(Py_ssize_t max_size);
-void       MinHeap_free(MinHeap* heap);
-void       MinHeap_insert(MinHeap* heap, Py_ssize_t key, Py_ssize_t priority);
-Py_ssize_t MinHeap_extract_min(MinHeap* heap);
-int        MinHeap_is_empty(MinHeap* heap);
-void       MinHeap_siftdown(MinHeap* heap, Py_ssize_t startpos, Py_ssize_t pos);
-void       MinHeap_siftup(MinHeap* heap, Py_ssize_t pos);
-void       MinHeap_print(MinHeap* heap);
+MinHeap   *MinHeap_alloc(Py_ssize_t max_size);
+void       MinHeap_free(MinHeap *heap);
+void       MinHeap_insert(MinHeap *heap, Py_ssize_t key, Py_ssize_t priority);
+Py_ssize_t MinHeap_extract_min(MinHeap *heap);
+int        MinHeap_is_empty(MinHeap *heap);
+void MinHeap_siftdown(MinHeap *heap, Py_ssize_t startpos, Py_ssize_t pos);
+void MinHeap_siftup(MinHeap *heap, Py_ssize_t pos);
+void MinHeap_print(MinHeap *heap);
+
+#endif  // GRAPES_GRAPES_CGRAPH_HEAP_H_
```

