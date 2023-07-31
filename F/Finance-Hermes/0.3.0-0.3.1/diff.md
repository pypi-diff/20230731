# Comparing `tmp/Finance-Hermes-0.3.0.tar.gz` & `tmp/Finance-Hermes-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Finance-Hermes-0.3.0.tar", last modified: Sat Jul 29 06:12:45 2023, max compression
+gzip compressed data, was "dist/Finance-Hermes-0.3.1.tar", last modified: Mon Jul 31 12:11:45 2023, max compression
```

## Comparing `Finance-Hermes-0.3.0.tar` & `Finance-Hermes-0.3.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.0/Finance_Hermes.egg-info/
--rw-r--r--   0 root         (0) root         (0)      233 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.0/Finance_Hermes.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      829 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.0/Finance_Hermes.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.0/Finance_Hermes.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.0/Finance_Hermes.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.0/Finance_Hermes.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    11357 2022-11-01 07:48:09.000000 Finance-Hermes-0.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      358 2023-07-29 01:53:47.000000 Finance-Hermes-0.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      233 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      195 2022-11-06 15:36:04.000000 Finance-Hermes-0.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.0/hermes/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-29 06:12:04.000000 Finance-Hermes-0.3.0/hermes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.0/hermes/factors/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.3.0/hermes/factors/__init__.py
--rw-r--r--   0 root         (0) root         (0)   339800 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.0/hermes/factors/base.c
--rw-r--r--   0 root         (0) root         (0)     4452 2023-07-29 02:06:34.000000 Finance-Hermes-0.3.0/hermes/factors/base.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.0/hermes/factors/test/
--rw-r--r--   0 root         (0) root         (0)   241941 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.0/hermes/factors/test/factor_test.c
--rw-r--r--   0 root         (0) root         (0)     2062 2023-07-29 06:11:05.000000 Finance-Hermes-0.3.0/hermes/factors/test/factor_test.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.0/hermes/kdutils/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.3.0/hermes/kdutils/__init__.py
--rw-r--r--   0 root         (0) root         (0)   271147 2023-07-29 02:01:44.000000 Finance-Hermes-0.3.0/hermes/kdutils/base.c
--rw-r--r--   0 root         (0) root         (0)     2338 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.0/hermes/kdutils/base.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.0/hermes/kdutils/core/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.3.0/hermes/kdutils/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)   678491 2023-07-29 02:01:44.000000 Finance-Hermes-0.3.0/hermes/kdutils/core/fixes.c
--rw-r--r--   0 root         (0) root         (0)     9714 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.0/hermes/kdutils/core/fixes.pyx
--rw-r--r--   0 root         (0) root         (0)   392670 2023-07-29 02:01:44.000000 Finance-Hermes-0.3.0/hermes/kdutils/core/helper.c
--rw-r--r--   0 root         (0) root         (0)     7825 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.0/hermes/kdutils/core/helper.pyx
--rw-r--r--   0 root         (0) root         (0)   190192 2023-07-29 02:01:44.000000 Finance-Hermes-0.3.0/hermes/kdutils/create_id.c
--rw-r--r--   0 root         (0) root         (0)      870 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.0/hermes/kdutils/create_id.pyx
--rw-r--r--   0 root         (0) root         (0)   235985 2023-07-29 02:01:44.000000 Finance-Hermes-0.3.0/hermes/kdutils/lazy.c
--rw-r--r--   0 root         (0) root         (0)     1578 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.0/hermes/kdutils/lazy.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.0/hermes/lzador/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.0/hermes/lzador/__init__.py
--rw-r--r--   0 root         (0) root         (0)   161732 2023-07-29 02:01:44.000000 Finance-Hermes-0.3.0/hermes/lzador/calculater.c
--rw-r--r--   0 root         (0) root         (0)      657 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.0/hermes/lzador/calculater.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.0/requirements/
--rw-r--r--   0 root         (0) root         (0)       90 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.0/requirements/py3.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3331 2023-07-29 01:55:31.000000 Finance-Hermes-0.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 12:11:45.000000 Finance-Hermes-0.3.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 12:11:45.000000 Finance-Hermes-0.3.1/Finance_Hermes.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      233 2023-07-31 12:11:45.000000 Finance-Hermes-0.3.1/Finance_Hermes.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      829 2023-07-31 12:11:45.000000 Finance-Hermes-0.3.1/Finance_Hermes.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 12:11:45.000000 Finance-Hermes-0.3.1/Finance_Hermes.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2023-07-31 12:11:45.000000 Finance-Hermes-0.3.1/Finance_Hermes.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-31 12:11:45.000000 Finance-Hermes-0.3.1/Finance_Hermes.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-11-01 07:48:09.000000 Finance-Hermes-0.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      358 2023-07-29 01:53:47.000000 Finance-Hermes-0.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      233 2023-07-31 12:11:45.000000 Finance-Hermes-0.3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      195 2022-11-06 15:36:04.000000 Finance-Hermes-0.3.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 12:11:45.000000 Finance-Hermes-0.3.1/hermes/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-31 12:11:22.000000 Finance-Hermes-0.3.1/hermes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 12:11:45.000000 Finance-Hermes-0.3.1/hermes/factors/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.3.1/hermes/factors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   360795 2023-07-31 12:08:41.000000 Finance-Hermes-0.3.1/hermes/factors/base.c
+-rw-r--r--   0 root         (0) root         (0)     4919 2023-07-31 12:05:26.000000 Finance-Hermes-0.3.1/hermes/factors/base.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 12:11:45.000000 Finance-Hermes-0.3.1/hermes/factors/test/
+-rw-r--r--   0 root         (0) root         (0)   241941 2023-07-29 06:12:45.000000 Finance-Hermes-0.3.1/hermes/factors/test/factor_test.c
+-rw-r--r--   0 root         (0) root         (0)     2062 2023-07-29 06:11:05.000000 Finance-Hermes-0.3.1/hermes/factors/test/factor_test.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 12:11:45.000000 Finance-Hermes-0.3.1/hermes/kdutils/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.3.1/hermes/kdutils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   271147 2023-07-29 02:01:44.000000 Finance-Hermes-0.3.1/hermes/kdutils/base.c
+-rw-r--r--   0 root         (0) root         (0)     2338 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.1/hermes/kdutils/base.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 12:11:45.000000 Finance-Hermes-0.3.1/hermes/kdutils/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.3.1/hermes/kdutils/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   678491 2023-07-29 02:01:44.000000 Finance-Hermes-0.3.1/hermes/kdutils/core/fixes.c
+-rw-r--r--   0 root         (0) root         (0)     9714 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.1/hermes/kdutils/core/fixes.pyx
+-rw-r--r--   0 root         (0) root         (0)   392670 2023-07-29 02:01:44.000000 Finance-Hermes-0.3.1/hermes/kdutils/core/helper.c
+-rw-r--r--   0 root         (0) root         (0)     7825 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.1/hermes/kdutils/core/helper.pyx
+-rw-r--r--   0 root         (0) root         (0)   190192 2023-07-29 02:01:44.000000 Finance-Hermes-0.3.1/hermes/kdutils/create_id.c
+-rw-r--r--   0 root         (0) root         (0)      870 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.1/hermes/kdutils/create_id.pyx
+-rw-r--r--   0 root         (0) root         (0)   235985 2023-07-29 02:01:44.000000 Finance-Hermes-0.3.1/hermes/kdutils/lazy.c
+-rw-r--r--   0 root         (0) root         (0)     1578 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.1/hermes/kdutils/lazy.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 12:11:45.000000 Finance-Hermes-0.3.1/hermes/lzador/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.1/hermes/lzador/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   161732 2023-07-29 02:01:44.000000 Finance-Hermes-0.3.1/hermes/lzador/calculater.c
+-rw-r--r--   0 root         (0) root         (0)      657 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.1/hermes/lzador/calculater.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 12:11:45.000000 Finance-Hermes-0.3.1/requirements/
+-rw-r--r--   0 root         (0) root         (0)       90 2023-07-29 01:51:21.000000 Finance-Hermes-0.3.1/requirements/py3.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 12:11:45.000000 Finance-Hermes-0.3.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3337 2023-07-31 12:08:25.000000 Finance-Hermes-0.3.1/setup.py
```

### Comparing `Finance-Hermes-0.3.0/Finance_Hermes.egg-info/SOURCES.txt` & `Finance-Hermes-0.3.1/Finance_Hermes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.3.0/LICENSE` & `Finance-Hermes-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.3.0/hermes/factors/base.c` & `Finance-Hermes-0.3.1/hermes/factors/base.c`

 * *Files 2% similar despite different names*

```diff
@@ -827,15 +827,15 @@
 static const char *__pyx_f[] = {
   "hermes/factors/base.pyx",
 };
 
 /*--- Type declarations ---*/
 struct __pyx_obj_6hermes_7factors_4base___pyx_scope_struct__factors_list;
 
-/* "hermes/factors/base.pyx":140
+/* "hermes/factors/base.pyx":144
  *         return data
  * 
  *     def factors_list(self):             # <<<<<<<<<<<<<<
  *         return list(
  *             filter(
  */
 struct __pyx_obj_6hermes_7factors_4base___pyx_scope_struct__factors_list {
@@ -995,14 +995,23 @@
     (likely(PyDict_CheckExact(obj)) ?\
      __Pyx_PyDict_GetItem(obj, name) : PyObject_GetItem(obj, name))
 #else
 #define __Pyx_PyDict_GetItem(d, key) PyObject_GetItem(d, key)
 #define __Pyx_PyObject_Dict_GetItem(obj, name)  PyObject_GetItem(obj, name)
 #endif
 
+/* PyObjectSetAttrStr.proto */
+#if CYTHON_USE_TYPE_SLOTS
+#define __Pyx_PyObject_DelAttrStr(o,n) __Pyx_PyObject_SetAttrStr(o, n, NULL)
+static CYTHON_INLINE int __Pyx_PyObject_SetAttrStr(PyObject* obj, PyObject* attr_name, PyObject* value);
+#else
+#define __Pyx_PyObject_DelAttrStr(o,n)   PyObject_DelAttr(o,n)
+#define __Pyx_PyObject_SetAttrStr(o,n,v) PyObject_SetAttr(o,n,v)
+#endif
+
 /* PyDictVersioning.proto */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 #define __PYX_DICT_VERSION_INIT  ((PY_UINT64_T) -1)
 #define __PYX_GET_DICT_VERSION(dict)  (((PyDictObject*)(dict))->ma_version_tag)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)\
     (version_var) = __PYX_GET_DICT_VERSION(dict);\
     (cache_var) = (value);
@@ -1042,41 +1051,38 @@
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
-/* GetAttr.proto */
-static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *, PyObject *);
-
 /* PyObjectCall2Args.proto */
 static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
 
+/* GetAttr.proto */
+static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *, PyObject *);
+
 /* PySequenceContains.proto */
 static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
     int result = PySequence_Contains(seq, item);
     return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
 }
 
+/* SliceObject.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetSlice(
+        PyObject* obj, Py_ssize_t cstart, Py_ssize_t cstop,
+        PyObject** py_start, PyObject** py_stop, PyObject** py_slice,
+        int has_cstart, int has_cstop, int wraparound);
+
 /* HasAttr.proto */
 static CYTHON_INLINE int __Pyx_HasAttr(PyObject *, PyObject *);
 
 /* PyIntCompare.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_EqObjC(PyObject *op1, PyObject *op2, long intval, long inplace);
 
-/* PyObjectSetAttrStr.proto */
-#if CYTHON_USE_TYPE_SLOTS
-#define __Pyx_PyObject_DelAttrStr(o,n) __Pyx_PyObject_SetAttrStr(o, n, NULL)
-static CYTHON_INLINE int __Pyx_PyObject_SetAttrStr(PyObject* obj, PyObject* attr_name, PyObject* value);
-#else
-#define __Pyx_PyObject_DelAttrStr(o,n)   PyObject_DelAttr(o,n)
-#define __Pyx_PyObject_SetAttrStr(o,n,v) PyObject_SetAttr(o,n,v)
-#endif
-
 /* IterFinish.proto */
 static CYTHON_INLINE int __Pyx_IterFinish(void);
 
 /* PyObjectGetMethod.proto */
 static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method);
 
 /* PyObjectCallMethod0.proto */
@@ -1313,14 +1319,17 @@
 #else
 #define __Pyx_TypeCheck(obj, type) PyObject_TypeCheck(obj, (PyTypeObject *)type)
 #define __Pyx_PyErr_GivenExceptionMatches(err, type) PyErr_GivenExceptionMatches(err, type)
 #define __Pyx_PyErr_GivenExceptionMatches2(err, type1, type2) (PyErr_GivenExceptionMatches(err, type1) || PyErr_GivenExceptionMatches(err, type2))
 #endif
 #define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
 
+/* CStringEquals.proto */
+static CYTHON_INLINE int __Pyx_StrEq(const char *, const char *);
+
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 
@@ -1331,31 +1340,36 @@
 int __pyx_module_is_main_hermes__factors__base = 0;
 
 /* Implementation of 'hermes.factors.base' */
 static PyObject *__pyx_builtin_filter;
 static const char __pyx_k_[] = "_";
 static const char __pyx_k_0[] = "{0}";
 static const char __pyx_k_s[] = "s";
+static const char __pyx_k__2[] = "*";
+static const char __pyx_k_by[] = "by";
 static const char __pyx_k_id[] = "id";
+static const char __pyx_k_0_b[] = "-{0}b";
 static const char __pyx_k_abc[] = "abc";
 static const char __pyx_k_ddb[] = "ddb";
 static const char __pyx_k_doc[] = "__doc__";
+static const char __pyx_k_loc[] = "loc";
 static const char __pyx_k_md5[] = "md5";
 static const char __pyx_k_pdb[] = "pdb";
 static const char __pyx_k_six[] = "six";
 static const char __pyx_k_copy[] = "copy";
 static const char __pyx_k_data[] = "data";
 static const char __pyx_k_func[] = "func";
 static const char __pyx_k_init[] = "__init__";
 static const char __pyx_k_json[] = "json";
 static const char __pyx_k_long[] = "long";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "name";
 static const char __pyx_k_self[] = "self";
 static const char __pyx_k_test[] = "__test__";
+static const char __pyx_k_Y_m_d[] = "%Y-%m-%d";
 static const char __pyx_k_digit[] = "digit";
 static const char __pyx_k_dumps[] = "dumps";
 static const char __pyx_k_items[] = "items";
 static const char __pyx_k_short[] = "short";
 static const char __pyx_k_stack[] = "stack";
 static const char __pyx_k_utf_8[] = "utf-8";
 static const char __pyx_k_value[] = "value";
@@ -1363,14 +1377,15 @@
 static const char __pyx_k_filter[] = "filter";
 static const char __pyx_k_format[] = "format";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_kwargs[] = "kwargs";
 static const char __pyx_k_method[] = "method";
 static const char __pyx_k_module[] = "__module__";
 static const char __pyx_k_name_2[] = "__name__";
+static const char __pyx_k_window[] = "window";
 static const char __pyx_k_ABCMeta[] = "ABCMeta";
 static const char __pyx_k_buy_put[] = "\n        \346\267\267\345\205\245\347\261\273\357\274\214\346\267\267\345\205\245\344\273\243\350\241\250\347\251\272\345\244\264\357\274\214\345\272\224\347\224\250\345\234\272\346\231\257\345\234\250\344\272\216\346\234\237\346\235\203\357\274\214\346\234\237\350\264\247\347\255\226\347\225\245\344\270\255\357\274\214\n        \344\270\215\345\256\214\345\205\250\346\230\257\346\234\237\346\235\203\344\270\255buy put\347\232\204\346\246\202\345\277\265\357\274\214\345\217\252\344\273\243\347\234\213\350\267\214\345\217\215\345\220\221\346\223\215\344\275\234\357\274\214\n        \345\215\263\346\234\237\346\234\233\344\271\260\345\205\245\345\220\216\344\272\244\346\230\223\347\233\256\346\240\207\344\273\267\346\240\274\344\270\213\350\267\214\357\274\214\344\270\213\350\267\214\345\270\246\346\235\245\346\224\266\347\233\212\n    ";
 static const char __pyx_k_columns[] = "columns";
 static const char __pyx_k_default[] = "default";
 static const char __pyx_k_feature[] = "feature";
 static const char __pyx_k_hashlib[] = "hashlib";
 static const char __pyx_k_inspect[] = "inspect";
@@ -1380,32 +1395,38 @@
 static const char __pyx_k_category[] = "category";
 static const char __pyx_k_deepcopy[] = "deepcopy";
 static const char __pyx_k_encoding[] = "encoding";
 static const char __pyx_k_end_date[] = "end_date";
 static const char __pyx_k_format_2[] = "_format";
 static const char __pyx_k_original[] = "original";
 static const char __pyx_k_qualname[] = "__qualname__";
+static const char __pyx_k_strftime[] = "strftime";
 static const char __pyx_k_ParamBase[] = "ParamBase";
+static const char __pyx_k_china_sse[] = "china.sse";
 static const char __pyx_k_create_id[] = "create_id";
 static const char __pyx_k_fun_param[] = "fun_param";
 static const char __pyx_k_hexdigest[] = "hexdigest";
 static const char __pyx_k_init_data[] = "init_data";
 static const char __pyx_k_init_self[] = "_init_self";
 static const char __pyx_k_metaclass[] = "__metaclass__";
 static const char __pyx_k_signature[] = "signature";
 static const char __pyx_k_FactorBase[] = "FactorBase";
 static const char __pyx_k_ShortMixin[] = "ShortMixin";
 static const char __pyx_k_begin_date[] = "begin_date";
 static const char __pyx_k_parameters[] = "parameters";
+static const char __pyx_k_start_date[] = "start_date";
 static const char __pyx_k_startswith[] = "startswith";
+static const char __pyx_k_trade_date[] = "trade_date";
 static const char __pyx_k_create_id_2[] = "_create_id";
 static const char __pyx_k_data_format[] = "_data_format";
 static const char __pyx_k_func_module[] = "func_module";
+static const char __pyx_k_jdwdate_api[] = "jdwdate.api";
 static const char __pyx_k_member_func[] = "member_func";
 static const char __pyx_k_reset_index[] = "reset_index";
+static const char __pyx_k_sort_values[] = "sort_values";
 static const char __pyx_k_dependencies[] = "dependencies";
 static const char __pyx_k_factors_list[] = "factors_list";
 static const char __pyx_k_LongCallMixin[] = "LongCallMixin";
 static const char __pyx_k_data_format_2[] = "data_format";
 static const char __pyx_k_long_type_str[] = "long_type_str";
 static const char __pyx_k_ShortCallMixin[] = "ShortCallMixin";
 static const char __pyx_k_abstractmethod[] = "abstractmethod";
@@ -1422,27 +1443,29 @@
 static const char __pyx_k_hermes_factors_base[] = "hermes.factors.base";
 static const char __pyx_k_hermes_kdutils_base[] = "hermes.kdutils.base";
 static const char __pyx_k_hermes_kdutils_lazy[] = "hermes.kdutils.lazy";
 static const char __pyx_k_FactorBase_init_data[] = "FactorBase.init_data";
 static const char __pyx_k_jdwdata_RetrievalAPI[] = "jdwdata.RetrievalAPI";
 static const char __pyx_k_FactorBase__create_id[] = "FactorBase._create_id";
 static const char __pyx_k_FactorBase__init_self[] = "FactorBase._init_self";
+static const char __pyx_k_advanceDateByCalendar[] = "advanceDateByCalendar";
 static const char __pyx_k_FactorBase_factors_list[] = "FactorBase.factors_list";
 static const char __pyx_k_hermes_factors_base_pyx[] = "hermes/factors/base.pyx";
 static const char __pyx_k_hermes_kdutils_create_id[] = "hermes.kdutils.create_id";
 static const char __pyx_k_ShortMixin_short_type_str[] = "ShortMixin.short_type_str";
 static const char __pyx_k_FactorBase_get_dependencies[] = "FactorBase.get_dependencies";
 static const char __pyx_k_LongCallMixin_long_type_str[] = "LongCallMixin.long_type_str";
 static const char __pyx_k_ShortMixin_expect_direction[] = "ShortMixin.expect_direction";
 static const char __pyx_k_ShortCallMixin_short_type_str[] = "ShortCallMixin.short_type_str";
 static const char __pyx_k_LongCallMixin_expect_direction[] = "LongCallMixin.expect_direction";
 static const char __pyx_k_ShortCallMixin_expect_direction[] = "ShortCallMixin.expect_direction";
 static const char __pyx_k_FactorBase_factors_list_locals_l[] = "FactorBase.factors_list.<locals>.<lambda>";
 static PyObject *__pyx_n_s_;
 static PyObject *__pyx_kp_s_0;
+static PyObject *__pyx_kp_s_0_b;
 static PyObject *__pyx_n_s_ABCMeta;
 static PyObject *__pyx_n_s_FactorBase;
 static PyObject *__pyx_n_s_FactorBase___init;
 static PyObject *__pyx_n_s_FactorBase__create_id;
 static PyObject *__pyx_n_s_FactorBase__format;
 static PyObject *__pyx_n_s_FactorBase__init_self;
 static PyObject *__pyx_n_s_FactorBase_factors_list;
@@ -1457,20 +1480,25 @@
 static PyObject *__pyx_n_s_ParamBase;
 static PyObject *__pyx_n_s_ShortCallMixin;
 static PyObject *__pyx_n_s_ShortCallMixin_expect_direction;
 static PyObject *__pyx_n_s_ShortCallMixin_short_type_str;
 static PyObject *__pyx_n_s_ShortMixin;
 static PyObject *__pyx_n_s_ShortMixin_expect_direction;
 static PyObject *__pyx_n_s_ShortMixin_short_type_str;
+static PyObject *__pyx_kp_s_Y_m_d;
+static PyObject *__pyx_n_s__2;
 static PyObject *__pyx_n_s_abc;
 static PyObject *__pyx_n_s_abstractmethod;
+static PyObject *__pyx_n_s_advanceDateByCalendar;
 static PyObject *__pyx_n_s_begin_date;
 static PyObject *__pyx_kp_s_buy_call;
 static PyObject *__pyx_kp_s_buy_put;
+static PyObject *__pyx_n_s_by;
 static PyObject *__pyx_n_s_category;
+static PyObject *__pyx_kp_s_china_sse;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_columns;
 static PyObject *__pyx_n_s_copy;
 static PyObject *__pyx_n_s_create_id;
 static PyObject *__pyx_n_s_create_id_2;
 static PyObject *__pyx_n_s_data;
 static PyObject *__pyx_n_s_data_format;
@@ -1508,16 +1536,18 @@
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_init;
 static PyObject *__pyx_n_s_init_data;
 static PyObject *__pyx_n_s_init_self;
 static PyObject *__pyx_n_s_inspect;
 static PyObject *__pyx_n_s_items;
 static PyObject *__pyx_n_s_jdwdata_RetrievalAPI;
+static PyObject *__pyx_n_s_jdwdate_api;
 static PyObject *__pyx_n_s_json;
 static PyObject *__pyx_n_s_kwargs;
+static PyObject *__pyx_n_s_loc;
 static PyObject *__pyx_n_s_long;
 static PyObject *__pyx_n_s_long_type_str;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_md5;
 static PyObject *__pyx_n_s_member_func;
 static PyObject *__pyx_n_s_metaclass;
 static PyObject *__pyx_n_s_method;
@@ -1532,19 +1562,24 @@
 static PyObject *__pyx_n_s_reset_index;
 static PyObject *__pyx_n_s_s;
 static PyObject *__pyx_n_s_self;
 static PyObject *__pyx_n_s_short;
 static PyObject *__pyx_n_s_short_type_str;
 static PyObject *__pyx_n_s_signature;
 static PyObject *__pyx_n_s_six;
+static PyObject *__pyx_n_s_sort_values;
 static PyObject *__pyx_n_s_stack;
+static PyObject *__pyx_n_s_start_date;
 static PyObject *__pyx_n_s_startswith;
+static PyObject *__pyx_n_s_strftime;
 static PyObject *__pyx_n_s_test;
+static PyObject *__pyx_n_s_trade_date;
 static PyObject *__pyx_kp_s_utf_8;
 static PyObject *__pyx_n_s_value;
+static PyObject *__pyx_n_s_window;
 static PyObject *__pyx_n_s_with_metaclass;
 static PyObject *__pyx_pf_6hermes_7factors_4base_13LongCallMixin_long_type_str(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_6hermes_7factors_4base_13LongCallMixin_2expect_direction(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_6hermes_7factors_4base_10ShortMixin_short_type_str(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_6hermes_7factors_4base_10ShortMixin_2expect_direction(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_6hermes_7factors_4base_10ShortMixin_4short_type_str(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_6hermes_7factors_4base_10ShortMixin_6expect_direction(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self); /* proto */
@@ -1557,50 +1592,51 @@
 static PyObject *__pyx_pf_6hermes_7factors_4base_10FactorBase_8_create_id(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_kwargs); /* proto */
 static PyObject *__pyx_pf_6hermes_7factors_4base_10FactorBase_10_format(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_data, PyObject *__pyx_v_name, PyObject *__pyx_v_kwargs); /* proto */
 static PyObject *__pyx_lambda_funcdef_lambda(PyObject *__pyx_self, PyObject *__pyx_v_x); /* proto */
 static PyObject *__pyx_pf_6hermes_7factors_4base_10FactorBase_12factors_list(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_tp_new_6hermes_7factors_4base___pyx_scope_struct__factors_list(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_float_1_0;
 static PyObject *__pyx_float_neg_1_0;
+static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_int_2;
 static PyObject *__pyx_int_10;
-static PyObject *__pyx_tuple__2;
-static PyObject *__pyx_tuple__4;
-static PyObject *__pyx_tuple__6;
-static PyObject *__pyx_tuple__8;
-static PyObject *__pyx_tuple__10;
-static PyObject *__pyx_tuple__12;
-static PyObject *__pyx_tuple__14;
-static PyObject *__pyx_tuple__16;
-static PyObject *__pyx_tuple__18;
-static PyObject *__pyx_tuple__20;
-static PyObject *__pyx_tuple__22;
-static PyObject *__pyx_tuple__24;
-static PyObject *__pyx_tuple__26;
-static PyObject *__pyx_tuple__28;
-static PyObject *__pyx_tuple__30;
-static PyObject *__pyx_codeobj__3;
-static PyObject *__pyx_codeobj__5;
-static PyObject *__pyx_codeobj__7;
-static PyObject *__pyx_codeobj__9;
-static PyObject *__pyx_codeobj__11;
-static PyObject *__pyx_codeobj__13;
-static PyObject *__pyx_codeobj__15;
-static PyObject *__pyx_codeobj__17;
-static PyObject *__pyx_codeobj__19;
-static PyObject *__pyx_codeobj__21;
-static PyObject *__pyx_codeobj__23;
-static PyObject *__pyx_codeobj__25;
-static PyObject *__pyx_codeobj__27;
-static PyObject *__pyx_codeobj__29;
-static PyObject *__pyx_codeobj__31;
+static PyObject *__pyx_tuple__3;
+static PyObject *__pyx_tuple__5;
+static PyObject *__pyx_tuple__7;
+static PyObject *__pyx_tuple__9;
+static PyObject *__pyx_tuple__11;
+static PyObject *__pyx_tuple__13;
+static PyObject *__pyx_tuple__15;
+static PyObject *__pyx_tuple__17;
+static PyObject *__pyx_tuple__19;
+static PyObject *__pyx_tuple__21;
+static PyObject *__pyx_tuple__23;
+static PyObject *__pyx_tuple__25;
+static PyObject *__pyx_tuple__27;
+static PyObject *__pyx_tuple__29;
+static PyObject *__pyx_tuple__31;
+static PyObject *__pyx_codeobj__4;
+static PyObject *__pyx_codeobj__6;
+static PyObject *__pyx_codeobj__8;
+static PyObject *__pyx_codeobj__10;
+static PyObject *__pyx_codeobj__12;
+static PyObject *__pyx_codeobj__14;
+static PyObject *__pyx_codeobj__16;
+static PyObject *__pyx_codeobj__18;
+static PyObject *__pyx_codeobj__20;
+static PyObject *__pyx_codeobj__22;
+static PyObject *__pyx_codeobj__24;
+static PyObject *__pyx_codeobj__26;
+static PyObject *__pyx_codeobj__28;
+static PyObject *__pyx_codeobj__30;
+static PyObject *__pyx_codeobj__32;
 /* Late includes */
 
-/* "hermes/factors/base.pyx":17
+/* "hermes/factors/base.pyx":18
  * 
  *     @LazyFunc
  *     def long_type_str(self):             # <<<<<<<<<<<<<<
  *         """unique call"""
  *         return "long"
  */
 
@@ -1620,42 +1656,42 @@
 }
 
 static PyObject *__pyx_pf_6hermes_7factors_4base_13LongCallMixin_long_type_str(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("long_type_str", 0);
 
-  /* "hermes/factors/base.pyx":19
+  /* "hermes/factors/base.pyx":20
  *     def long_type_str(self):
  *         """unique call"""
  *         return "long"             # <<<<<<<<<<<<<<
  * 
  *     @LazyFunc
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_n_s_long);
   __pyx_r = __pyx_n_s_long;
   goto __pyx_L0;
 
-  /* "hermes/factors/base.pyx":17
+  /* "hermes/factors/base.pyx":18
  * 
  *     @LazyFunc
  *     def long_type_str(self):             # <<<<<<<<<<<<<<
  *         """unique call"""
  *         return "long"
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "hermes/factors/base.pyx":22
+/* "hermes/factors/base.pyx":23
  * 
  *     @LazyFunc
  *     def expect_direction(self):             # <<<<<<<<<<<<<<
  *         """1.0"""
  *         return 1.0
  */
 
@@ -1675,42 +1711,42 @@
 }
 
 static PyObject *__pyx_pf_6hermes_7factors_4base_13LongCallMixin_2expect_direction(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("expect_direction", 0);
 
-  /* "hermes/factors/base.pyx":24
+  /* "hermes/factors/base.pyx":25
  *     def expect_direction(self):
  *         """1.0"""
  *         return 1.0             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_float_1_0);
   __pyx_r = __pyx_float_1_0;
   goto __pyx_L0;
 
-  /* "hermes/factors/base.pyx":22
+  /* "hermes/factors/base.pyx":23
  * 
  *     @LazyFunc
  *     def expect_direction(self):             # <<<<<<<<<<<<<<
  *         """1.0"""
  *         return 1.0
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "hermes/factors/base.pyx":35
+/* "hermes/factors/base.pyx":36
  * 
  *     @LazyFunc
  *     def short_type_str(self):             # <<<<<<<<<<<<<<
  *         """unique put"""
  *         return "short"
  */
 
@@ -1730,42 +1766,42 @@
 }
 
 static PyObject *__pyx_pf_6hermes_7factors_4base_10ShortMixin_short_type_str(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("short_type_str", 0);
 
-  /* "hermes/factors/base.pyx":37
+  /* "hermes/factors/base.pyx":38
  *     def short_type_str(self):
  *         """unique put"""
  *         return "short"             # <<<<<<<<<<<<<<
  * 
  *     @LazyFunc
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_n_s_short);
   __pyx_r = __pyx_n_s_short;
   goto __pyx_L0;
 
-  /* "hermes/factors/base.pyx":35
+  /* "hermes/factors/base.pyx":36
  * 
  *     @LazyFunc
  *     def short_type_str(self):             # <<<<<<<<<<<<<<
  *         """unique put"""
  *         return "short"
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "hermes/factors/base.pyx":40
+/* "hermes/factors/base.pyx":41
  * 
  *     @LazyFunc
  *     def expect_direction(self):             # <<<<<<<<<<<<<<
  *         """1.0"""
  *         return -1.0
  */
 
@@ -1785,27 +1821,27 @@
 }
 
 static PyObject *__pyx_pf_6hermes_7factors_4base_10ShortMixin_2expect_direction(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("expect_direction", 0);
 
-  /* "hermes/factors/base.pyx":42
+  /* "hermes/factors/base.pyx":43
  *     def expect_direction(self):
  *         """1.0"""
  *         return -1.0             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_float_neg_1_0);
   __pyx_r = __pyx_float_neg_1_0;
   goto __pyx_L0;
 
-  /* "hermes/factors/base.pyx":40
+  /* "hermes/factors/base.pyx":41
  * 
  *     @LazyFunc
  *     def expect_direction(self):             # <<<<<<<<<<<<<<
  *         """1.0"""
  *         return -1.0
  */
 
@@ -2115,15 +2151,15 @@
   __Pyx_RefNannySetupContext("__init__", 0);
 
   /* "hermes/factors/base.pyx":86
  *     def __init__(self, **kwargs):
  *         #
  *         self._init_self(**kwargs)             # <<<<<<<<<<<<<<
  * 
- * 
+ *     @abstractmethod
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_init_self); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_v_kwargs); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
@@ -2146,15 +2182,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "hermes/factors/base.pyx":90
+/* "hermes/factors/base.pyx":89
  * 
  *     @abstractmethod
  *     def _init_self(self, **kwargs):             # <<<<<<<<<<<<<<
  *         """"""
  *         pass
  */
 
@@ -2188,26 +2224,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "_init_self") < 0)) __PYX_ERR(0, 90, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "_init_self") < 0)) __PYX_ERR(0, 89, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_init_self", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 90, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_init_self", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 89, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
   __Pyx_AddTraceback("hermes.factors.base.FactorBase._init_self", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6hermes_7factors_4base_10FactorBase_2_init_self(__pyx_self, __pyx_v_self, __pyx_v_kwargs);
@@ -2226,15 +2262,15 @@
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "hermes/factors/base.pyx":94
+/* "hermes/factors/base.pyx":93
  *         pass
  * 
  *     def init_data(self, **kwargs):             # <<<<<<<<<<<<<<
  *         dependencies_list = self.get_dependencies()
  *         method = 'ddb' if 'method' not in kwargs else kwargs['method']
  */
 
@@ -2268,26 +2304,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "init_data") < 0)) __PYX_ERR(0, 94, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "init_data") < 0)) __PYX_ERR(0, 93, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("init_data", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 94, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("init_data", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 93, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
   __Pyx_AddTraceback("hermes.factors.base.FactorBase.init_data", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6hermes_7factors_4base_10FactorBase_4init_data(__pyx_self, __pyx_v_self, __pyx_v_kwargs);
@@ -2297,171 +2333,345 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_6hermes_7factors_4base_10FactorBase_4init_data(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_kwargs) {
   PyObject *__pyx_v_dependencies_list = NULL;
   PyObject *__pyx_v_method = NULL;
+  PyObject *__pyx_v_window = NULL;
+  PyObject *__pyx_v_start_date = NULL;
   PyObject *__pyx_v_data = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
+  int __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("init_data", 0);
 
-  /* "hermes/factors/base.pyx":95
+  /* "hermes/factors/base.pyx":94
  * 
  *     def init_data(self, **kwargs):
  *         dependencies_list = self.get_dependencies()             # <<<<<<<<<<<<<<
  *         method = 'ddb' if 'method' not in kwargs else kwargs['method']
- *         data = get_data_by_map(columns=dependencies_list,
+ *         self.begin_date = kwargs['begin_date']
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_get_dependencies); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_get_dependencies); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 95, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_dependencies_list = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/base.pyx":96
+  /* "hermes/factors/base.pyx":95
  *     def init_data(self, **kwargs):
  *         dependencies_list = self.get_dependencies()
  *         method = 'ddb' if 'method' not in kwargs else kwargs['method']             # <<<<<<<<<<<<<<
- *         data = get_data_by_map(columns=dependencies_list,
- *                       begin_date=kwargs['begin_date'],
+ *         self.begin_date = kwargs['begin_date']
+ *         self.end_date = kwargs['end_date']
  */
-  __pyx_t_4 = (__Pyx_PyDict_ContainsTF(__pyx_n_s_method, __pyx_v_kwargs, Py_NE)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 96, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyDict_ContainsTF(__pyx_n_s_method, __pyx_v_kwargs, Py_NE)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 95, __pyx_L1_error)
   if ((__pyx_t_4 != 0)) {
     __Pyx_INCREF(__pyx_n_s_ddb);
     __pyx_t_1 = __pyx_n_s_ddb;
   } else {
-    __pyx_t_2 = __Pyx_PyDict_GetItem(__pyx_v_kwargs, __pyx_n_s_method); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 96, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyDict_GetItem(__pyx_v_kwargs, __pyx_n_s_method); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 95, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_1 = __pyx_t_2;
     __pyx_t_2 = 0;
   }
   __pyx_v_method = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/base.pyx":97
+  /* "hermes/factors/base.pyx":96
  *         dependencies_list = self.get_dependencies()
  *         method = 'ddb' if 'method' not in kwargs else kwargs['method']
- *         data = get_data_by_map(columns=dependencies_list,             # <<<<<<<<<<<<<<
- *                       begin_date=kwargs['begin_date'],
- *                       end_date=kwargs['end_date'],
+ *         self.begin_date = kwargs['begin_date']             # <<<<<<<<<<<<<<
+ *         self.end_date = kwargs['end_date']
+ *         window = 0 if 'window' not in kwargs else int(kwargs['window'])
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_get_data_by_map); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_kwargs, __pyx_n_s_begin_date); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 97, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_columns, __pyx_v_dependencies_list) < 0) __PYX_ERR(0, 97, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_begin_date, __pyx_t_1) < 0) __PYX_ERR(0, 96, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "hermes/factors/base.pyx":98
+  /* "hermes/factors/base.pyx":97
  *         method = 'ddb' if 'method' not in kwargs else kwargs['method']
+ *         self.begin_date = kwargs['begin_date']
+ *         self.end_date = kwargs['end_date']             # <<<<<<<<<<<<<<
+ *         window = 0 if 'window' not in kwargs else int(kwargs['window'])
+ *         start_date = advanceDateByCalendar(
+ */
+  __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_kwargs, __pyx_n_s_end_date); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_end_date, __pyx_t_1) < 0) __PYX_ERR(0, 97, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "hermes/factors/base.pyx":98
+ *         self.begin_date = kwargs['begin_date']
+ *         self.end_date = kwargs['end_date']
+ *         window = 0 if 'window' not in kwargs else int(kwargs['window'])             # <<<<<<<<<<<<<<
+ *         start_date = advanceDateByCalendar(
+ *             'china.sse', self.begin_date,
+ */
+  __pyx_t_4 = (__Pyx_PyDict_ContainsTF(__pyx_n_s_window, __pyx_v_kwargs, Py_NE)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 98, __pyx_L1_error)
+  if ((__pyx_t_4 != 0)) {
+    __Pyx_INCREF(__pyx_int_0);
+    __pyx_t_1 = __pyx_int_0;
+  } else {
+    __pyx_t_2 = __Pyx_PyDict_GetItem(__pyx_v_kwargs, __pyx_n_s_window); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 98, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_3 = __Pyx_PyNumber_Int(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 98, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __pyx_t_3;
+    __pyx_t_3 = 0;
+  }
+  __pyx_v_window = __pyx_t_1;
+  __pyx_t_1 = 0;
+
+  /* "hermes/factors/base.pyx":99
+ *         self.end_date = kwargs['end_date']
+ *         window = 0 if 'window' not in kwargs else int(kwargs['window'])
+ *         start_date = advanceDateByCalendar(             # <<<<<<<<<<<<<<
+ *             'china.sse', self.begin_date,
+ *             '-{0}b'.format(window)).strftime('%Y-%m-%d')
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_advanceDateByCalendar); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+
+  /* "hermes/factors/base.pyx":100
+ *         window = 0 if 'window' not in kwargs else int(kwargs['window'])
+ *         start_date = advanceDateByCalendar(
+ *             'china.sse', self.begin_date,             # <<<<<<<<<<<<<<
+ *             '-{0}b'.format(window)).strftime('%Y-%m-%d')
  *         data = get_data_by_map(columns=dependencies_list,
- *                       begin_date=kwargs['begin_date'],             # <<<<<<<<<<<<<<
- *                       end_date=kwargs['end_date'],
- *                       method=method)
  */
-  __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_kwargs, __pyx_n_s_begin_date); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 98, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_begin_date, __pyx_t_3) < 0) __PYX_ERR(0, 97, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_begin_date); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+
+  /* "hermes/factors/base.pyx":101
+ *         start_date = advanceDateByCalendar(
+ *             'china.sse', self.begin_date,
+ *             '-{0}b'.format(window)).strftime('%Y-%m-%d')             # <<<<<<<<<<<<<<
+ *         data = get_data_by_map(columns=dependencies_list,
+ *                                begin_date=start_date,
+ */
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_kp_s_0_b, __pyx_n_s_format); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_8 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
+    __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
+    if (likely(__pyx_t_8)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
+      __Pyx_INCREF(__pyx_t_8);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_7, function);
+    }
+  }
+  __pyx_t_6 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_8, __pyx_v_window) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_v_window);
+  __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_7 = NULL;
+  __pyx_t_9 = 0;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_7)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_7);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __pyx_t_9 = 1;
+    }
+  }
+  #if CYTHON_FAST_PYCALL
+  if (PyFunction_Check(__pyx_t_2)) {
+    PyObject *__pyx_temp[4] = {__pyx_t_7, __pyx_kp_s_china_sse, __pyx_t_5, __pyx_t_6};
+    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_9, 3+__pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  } else
+  #endif
+  #if CYTHON_FAST_PYCCALL
+  if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
+    PyObject *__pyx_temp[4] = {__pyx_t_7, __pyx_kp_s_china_sse, __pyx_t_5, __pyx_t_6};
+    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_9, 3+__pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  } else
+  #endif
+  {
+    __pyx_t_8 = PyTuple_New(3+__pyx_t_9); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 99, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    if (__pyx_t_7) {
+      __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_7); __pyx_t_7 = NULL;
+    }
+    __Pyx_INCREF(__pyx_kp_s_china_sse);
+    __Pyx_GIVEREF(__pyx_kp_s_china_sse);
+    PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_9, __pyx_kp_s_china_sse);
+    __Pyx_GIVEREF(__pyx_t_5);
+    PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_9, __pyx_t_5);
+    __Pyx_GIVEREF(__pyx_t_6);
+    PyTuple_SET_ITEM(__pyx_t_8, 2+__pyx_t_9, __pyx_t_6);
+    __pyx_t_5 = 0;
+    __pyx_t_6 = 0;
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  }
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_strftime); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_3)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_3);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
+    }
+  }
+  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_kp_s_Y_m_d) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_s_Y_m_d);
+  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_v_start_date = __pyx_t_1;
+  __pyx_t_1 = 0;
 
-  /* "hermes/factors/base.pyx":99
+  /* "hermes/factors/base.pyx":102
+ *             'china.sse', self.begin_date,
+ *             '-{0}b'.format(window)).strftime('%Y-%m-%d')
+ *         data = get_data_by_map(columns=dependencies_list,             # <<<<<<<<<<<<<<
+ *                                begin_date=start_date,
+ *                                end_date=self.end_date,
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_get_data_by_map); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 102, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 102, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_columns, __pyx_v_dependencies_list) < 0) __PYX_ERR(0, 102, __pyx_L1_error)
+
+  /* "hermes/factors/base.pyx":103
+ *             '-{0}b'.format(window)).strftime('%Y-%m-%d')
+ *         data = get_data_by_map(columns=dependencies_list,
+ *                                begin_date=start_date,             # <<<<<<<<<<<<<<
+ *                                end_date=self.end_date,
+ *                                method=method)
+ */
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_begin_date, __pyx_v_start_date) < 0) __PYX_ERR(0, 102, __pyx_L1_error)
+
+  /* "hermes/factors/base.pyx":104
  *         data = get_data_by_map(columns=dependencies_list,
- *                       begin_date=kwargs['begin_date'],
- *                       end_date=kwargs['end_date'],             # <<<<<<<<<<<<<<
- *                       method=method)
+ *                                begin_date=start_date,
+ *                                end_date=self.end_date,             # <<<<<<<<<<<<<<
+ *                                method=method)
  *         return data
  */
-  __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_kwargs, __pyx_n_s_end_date); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_end_date); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 104, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_end_date, __pyx_t_3) < 0) __PYX_ERR(0, 97, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_end_date, __pyx_t_3) < 0) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "hermes/factors/base.pyx":100
- *                       begin_date=kwargs['begin_date'],
- *                       end_date=kwargs['end_date'],
- *                       method=method)             # <<<<<<<<<<<<<<
+  /* "hermes/factors/base.pyx":105
+ *                                begin_date=start_date,
+ *                                end_date=self.end_date,
+ *                                method=method)             # <<<<<<<<<<<<<<
  *         return data
  * 
  */
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_method, __pyx_v_method) < 0) __PYX_ERR(0, 97, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_method, __pyx_v_method) < 0) __PYX_ERR(0, 102, __pyx_L1_error)
 
-  /* "hermes/factors/base.pyx":97
- *         dependencies_list = self.get_dependencies()
- *         method = 'ddb' if 'method' not in kwargs else kwargs['method']
+  /* "hermes/factors/base.pyx":102
+ *             'china.sse', self.begin_date,
+ *             '-{0}b'.format(window)).strftime('%Y-%m-%d')
  *         data = get_data_by_map(columns=dependencies_list,             # <<<<<<<<<<<<<<
- *                       begin_date=kwargs['begin_date'],
- *                       end_date=kwargs['end_date'],
+ *                                begin_date=start_date,
+ *                                end_date=self.end_date,
  */
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_data = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "hermes/factors/base.pyx":101
- *                       end_date=kwargs['end_date'],
- *                       method=method)
+  /* "hermes/factors/base.pyx":106
+ *                                end_date=self.end_date,
+ *                                method=method)
  *         return data             # <<<<<<<<<<<<<<
  * 
- * 
+ *     def get_dependencies(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_data);
   __pyx_r = __pyx_v_data;
   goto __pyx_L0;
 
-  /* "hermes/factors/base.pyx":94
+  /* "hermes/factors/base.pyx":93
  *         pass
  * 
  *     def init_data(self, **kwargs):             # <<<<<<<<<<<<<<
  *         dependencies_list = self.get_dependencies()
  *         method = 'ddb' if 'method' not in kwargs else kwargs['method']
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
   __Pyx_AddTraceback("hermes.factors.base.FactorBase.init_data", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_dependencies_list);
   __Pyx_XDECREF(__pyx_v_method);
+  __Pyx_XDECREF(__pyx_v_window);
+  __Pyx_XDECREF(__pyx_v_start_date);
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "hermes/factors/base.pyx":105
- * 
+/* "hermes/factors/base.pyx":108
+ *         return data
  * 
  *     def get_dependencies(self):             # <<<<<<<<<<<<<<
  *         dependencies_list = []
  *         member_func = self.factors_list()
  */
 
 /* Python wrapper */
@@ -2497,223 +2707,223 @@
   int __pyx_t_7;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_dependencies", 0);
 
-  /* "hermes/factors/base.pyx":106
+  /* "hermes/factors/base.pyx":109
  * 
  *     def get_dependencies(self):
  *         dependencies_list = []             # <<<<<<<<<<<<<<
  *         member_func = self.factors_list()
  *         for func in member_func:
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 106, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_dependencies_list = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/base.pyx":107
+  /* "hermes/factors/base.pyx":110
  *     def get_dependencies(self):
  *         dependencies_list = []
  *         member_func = self.factors_list()             # <<<<<<<<<<<<<<
  *         for func in member_func:
  *             func_module = getattr(self, func)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_factors_list); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_factors_list); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 107, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_member_func = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "hermes/factors/base.pyx":108
+  /* "hermes/factors/base.pyx":111
  *         dependencies_list = []
  *         member_func = self.factors_list()
  *         for func in member_func:             # <<<<<<<<<<<<<<
  *             func_module = getattr(self, func)
  *             fun_param = inspect.signature(func_module).parameters
  */
   if (likely(PyList_CheckExact(__pyx_v_member_func)) || PyTuple_CheckExact(__pyx_v_member_func)) {
     __pyx_t_1 = __pyx_v_member_func; __Pyx_INCREF(__pyx_t_1); __pyx_t_4 = 0;
     __pyx_t_5 = NULL;
   } else {
-    __pyx_t_4 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_member_func); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error)
+    __pyx_t_4 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_member_func); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 108, __pyx_L1_error)
+    __pyx_t_5 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 111, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_5)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 108, __pyx_L1_error)
+        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 111, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 108, __pyx_L1_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 111, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       } else {
         if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 108, __pyx_L1_error)
+        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 111, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 108, __pyx_L1_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 111, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       }
     } else {
       __pyx_t_2 = __pyx_t_5(__pyx_t_1);
       if (unlikely(!__pyx_t_2)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 108, __pyx_L1_error)
+          else __PYX_ERR(0, 111, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_2);
     }
     __Pyx_XDECREF_SET(__pyx_v_func, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "hermes/factors/base.pyx":109
+    /* "hermes/factors/base.pyx":112
  *         member_func = self.factors_list()
  *         for func in member_func:
  *             func_module = getattr(self, func)             # <<<<<<<<<<<<<<
  *             fun_param = inspect.signature(func_module).parameters
  *             if 'dependencies' in fun_param:
  */
-    __pyx_t_2 = __Pyx_GetAttr(__pyx_v_self, __pyx_v_func); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 109, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_GetAttr(__pyx_v_self, __pyx_v_func); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 112, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_XDECREF_SET(__pyx_v_func_module, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "hermes/factors/base.pyx":110
+    /* "hermes/factors/base.pyx":113
  *         for func in member_func:
  *             func_module = getattr(self, func)
  *             fun_param = inspect.signature(func_module).parameters             # <<<<<<<<<<<<<<
  *             if 'dependencies' in fun_param:
  *                 dependencies = fun_param['dependencies'].default
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_inspect); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 110, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_inspect); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 113, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_signature); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 110, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_signature); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 113, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_6, function);
       }
     }
     __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_3, __pyx_v_func_module) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_v_func_module);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 110, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_parameters); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 110, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_parameters); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 113, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF_SET(__pyx_v_fun_param, __pyx_t_6);
     __pyx_t_6 = 0;
 
-    /* "hermes/factors/base.pyx":111
+    /* "hermes/factors/base.pyx":114
  *             func_module = getattr(self, func)
  *             fun_param = inspect.signature(func_module).parameters
  *             if 'dependencies' in fun_param:             # <<<<<<<<<<<<<<
  *                 dependencies = fun_param['dependencies'].default
  *                 dependencies_list += dependencies
  */
-    __pyx_t_7 = (__Pyx_PySequence_ContainsTF(__pyx_n_s_dependencies, __pyx_v_fun_param, Py_EQ)); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 111, __pyx_L1_error)
+    __pyx_t_7 = (__Pyx_PySequence_ContainsTF(__pyx_n_s_dependencies, __pyx_v_fun_param, Py_EQ)); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 114, __pyx_L1_error)
     __pyx_t_8 = (__pyx_t_7 != 0);
     if (__pyx_t_8) {
 
-      /* "hermes/factors/base.pyx":112
+      /* "hermes/factors/base.pyx":115
  *             fun_param = inspect.signature(func_module).parameters
  *             if 'dependencies' in fun_param:
  *                 dependencies = fun_param['dependencies'].default             # <<<<<<<<<<<<<<
  *                 dependencies_list += dependencies
  *         return list(set(dependencies_list))
  */
-      __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_v_fun_param, __pyx_n_s_dependencies); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 112, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_v_fun_param, __pyx_n_s_dependencies); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 115, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_default); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 112, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_default); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 115, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_XDECREF_SET(__pyx_v_dependencies, __pyx_t_2);
       __pyx_t_2 = 0;
 
-      /* "hermes/factors/base.pyx":113
+      /* "hermes/factors/base.pyx":116
  *             if 'dependencies' in fun_param:
  *                 dependencies = fun_param['dependencies'].default
  *                 dependencies_list += dependencies             # <<<<<<<<<<<<<<
  *         return list(set(dependencies_list))
  * 
  */
-      __pyx_t_2 = PyNumber_InPlaceAdd(__pyx_v_dependencies_list, __pyx_v_dependencies); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L1_error)
+      __pyx_t_2 = PyNumber_InPlaceAdd(__pyx_v_dependencies_list, __pyx_v_dependencies); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 116, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF_SET(__pyx_v_dependencies_list, __pyx_t_2);
       __pyx_t_2 = 0;
 
-      /* "hermes/factors/base.pyx":111
+      /* "hermes/factors/base.pyx":114
  *             func_module = getattr(self, func)
  *             fun_param = inspect.signature(func_module).parameters
  *             if 'dependencies' in fun_param:             # <<<<<<<<<<<<<<
  *                 dependencies = fun_param['dependencies'].default
  *                 dependencies_list += dependencies
  */
     }
 
-    /* "hermes/factors/base.pyx":108
+    /* "hermes/factors/base.pyx":111
  *         dependencies_list = []
  *         member_func = self.factors_list()
  *         for func in member_func:             # <<<<<<<<<<<<<<
  *             func_module = getattr(self, func)
  *             fun_param = inspect.signature(func_module).parameters
  */
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "hermes/factors/base.pyx":114
+  /* "hermes/factors/base.pyx":117
  *                 dependencies = fun_param['dependencies'].default
  *                 dependencies_list += dependencies
  *         return list(set(dependencies_list))             # <<<<<<<<<<<<<<
  * 
- * 
+ *     def _create_id(self, **kwargs):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PySet_New(__pyx_v_dependencies_list); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 114, __pyx_L1_error)
+  __pyx_t_1 = PySet_New(__pyx_v_dependencies_list); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 117, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PySequence_List(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 114, __pyx_L1_error)
+  __pyx_t_2 = PySequence_List(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 117, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "hermes/factors/base.pyx":105
- * 
+  /* "hermes/factors/base.pyx":108
+ *         return data
  * 
  *     def get_dependencies(self):             # <<<<<<<<<<<<<<
  *         dependencies_list = []
  *         member_func = self.factors_list()
  */
 
   /* function exit code */
@@ -2733,15 +2943,15 @@
   __Pyx_XDECREF(__pyx_v_dependencies);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "hermes/factors/base.pyx":119
- * 
+ *         return list(set(dependencies_list))
  * 
  *     def _create_id(self, **kwargs):             # <<<<<<<<<<<<<<
  *         feature = copy.deepcopy(kwargs)
  *         feature['category'] = self.category
  */
 
 /* Python wrapper */
@@ -2986,15 +3196,15 @@
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "hermes/factors/base.pyx":119
- * 
+ *         return list(set(dependencies_list))
  * 
  *     def _create_id(self, **kwargs):             # <<<<<<<<<<<<<<
  *         feature = copy.deepcopy(kwargs)
  *         feature['category'] = self.category
  */
 
   /* function exit code */
@@ -3015,16 +3225,16 @@
   return __pyx_r;
 }
 
 /* "hermes/factors/base.pyx":126
  *         return "{0}".format(create_id(original=s, digit=10))
  * 
  *     def _format(self, data, name, **kwargs):             # <<<<<<<<<<<<<<
- *         #0 matrix  1 serise  2 DatFrame
- *         data_format = 1 if not hasattr(self,'_data_format') else self._data_format
+ *         # 0 matrix  1 serise  2 DatFrame
+ *         data = data.sort_values(by=['trade_date'])
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_6hermes_7factors_4base_10FactorBase_11_format(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_6hermes_7factors_4base_10FactorBase_10_format[] = "FactorBase._format(self, data, name, **kwargs)";
 static PyMethodDef __pyx_mdef_6hermes_7factors_4base_10FactorBase_11_format = {"_format", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6hermes_7factors_4base_10FactorBase_11_format, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6hermes_7factors_4base_10FactorBase_10_format};
 static PyObject *__pyx_pw_6hermes_7factors_4base_10FactorBase_11_format(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
@@ -3106,215 +3316,270 @@
 }
 
 static PyObject *__pyx_pf_6hermes_7factors_4base_10FactorBase_10_format(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_data, PyObject *__pyx_v_name, PyObject *__pyx_v_kwargs) {
   PyObject *__pyx_v_data_format = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  int __pyx_t_2;
+  PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
-  int __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  int __pyx_t_5;
+  int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_format", 0);
   __Pyx_INCREF(__pyx_v_data);
 
   /* "hermes/factors/base.pyx":128
  *     def _format(self, data, name, **kwargs):
- *         #0 matrix  1 serise  2 DatFrame
- *         data_format = 1 if not hasattr(self,'_data_format') else self._data_format             # <<<<<<<<<<<<<<
- *         if data_format == 1 or data_format == 2:
- *             data = data.stack()
+ *         # 0 matrix  1 serise  2 DatFrame
+ *         data = data.sort_values(by=['trade_date'])             # <<<<<<<<<<<<<<
+ *         data = data.loc[self.begin_date:self.end_date]
+ *         data_format = 1 if not hasattr(self,
  */
-  __pyx_t_2 = __Pyx_HasAttr(__pyx_v_self, __pyx_n_s_data_format); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 128, __pyx_L1_error)
-  if (((!(__pyx_t_2 != 0)) != 0)) {
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_sort_values); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 128, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 128, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 128, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_INCREF(__pyx_n_s_trade_date);
+  __Pyx_GIVEREF(__pyx_n_s_trade_date);
+  PyList_SET_ITEM(__pyx_t_3, 0, __pyx_n_s_trade_date);
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_by, __pyx_t_3) < 0) __PYX_ERR(0, 128, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 128, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_3);
+  __pyx_t_3 = 0;
+
+  /* "hermes/factors/base.pyx":129
+ *         # 0 matrix  1 serise  2 DatFrame
+ *         data = data.sort_values(by=['trade_date'])
+ *         data = data.loc[self.begin_date:self.end_date]             # <<<<<<<<<<<<<<
+ *         data_format = 1 if not hasattr(self,
+ *                                        '_data_format') else self._data_format
+ */
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_loc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 129, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_begin_date); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 129, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_end_date); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 129, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_4 = __Pyx_PyObject_GetSlice(__pyx_t_3, 0, 0, &__pyx_t_2, &__pyx_t_1, NULL, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 129, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_4);
+  __pyx_t_4 = 0;
+
+  /* "hermes/factors/base.pyx":130
+ *         data = data.sort_values(by=['trade_date'])
+ *         data = data.loc[self.begin_date:self.end_date]
+ *         data_format = 1 if not hasattr(self,             # <<<<<<<<<<<<<<
+ *                                        '_data_format') else self._data_format
+ * 
+ */
+  __pyx_t_5 = __Pyx_HasAttr(__pyx_v_self, __pyx_n_s_data_format); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 130, __pyx_L1_error)
+  if (((!(__pyx_t_5 != 0)) != 0)) {
     __Pyx_INCREF(__pyx_int_1);
-    __pyx_t_1 = __pyx_int_1;
+    __pyx_t_4 = __pyx_int_1;
   } else {
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data_format); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 128, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_1 = __pyx_t_3;
-    __pyx_t_3 = 0;
+
+    /* "hermes/factors/base.pyx":131
+ *         data = data.loc[self.begin_date:self.end_date]
+ *         data_format = 1 if not hasattr(self,
+ *                                        '_data_format') else self._data_format             # <<<<<<<<<<<<<<
+ * 
+ *         if data_format == 1 or data_format == 2:
+ */
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data_format); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 131, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = __pyx_t_1;
+    __pyx_t_1 = 0;
   }
-  __pyx_v_data_format = __pyx_t_1;
-  __pyx_t_1 = 0;
+  __pyx_v_data_format = __pyx_t_4;
+  __pyx_t_4 = 0;
 
-  /* "hermes/factors/base.pyx":129
- *         #0 matrix  1 serise  2 DatFrame
- *         data_format = 1 if not hasattr(self,'_data_format') else self._data_format
+  /* "hermes/factors/base.pyx":133
+ *                                        '_data_format') else self._data_format
+ * 
  *         if data_format == 1 or data_format == 2:             # <<<<<<<<<<<<<<
  *             data = data.stack()
  *             if data_format == 2:
  */
-  __pyx_t_1 = __Pyx_PyInt_EqObjC(__pyx_v_data_format, __pyx_int_1, 1, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 129, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 129, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (!__pyx_t_4) {
+  __pyx_t_4 = __Pyx_PyInt_EqObjC(__pyx_v_data_format, __pyx_int_1, 1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (!__pyx_t_6) {
   } else {
-    __pyx_t_2 = __pyx_t_4;
+    __pyx_t_5 = __pyx_t_6;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_1 = __Pyx_PyInt_EqObjC(__pyx_v_data_format, __pyx_int_2, 2, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 129, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 129, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_2 = __pyx_t_4;
+  __pyx_t_4 = __Pyx_PyInt_EqObjC(__pyx_v_data_format, __pyx_int_2, 2, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_5 = __pyx_t_6;
   __pyx_L4_bool_binop_done:;
-  if (__pyx_t_2) {
+  if (__pyx_t_5) {
 
-    /* "hermes/factors/base.pyx":130
- *         data_format = 1 if not hasattr(self,'_data_format') else self._data_format
+    /* "hermes/factors/base.pyx":134
+ * 
  *         if data_format == 1 or data_format == 2:
  *             data = data.stack()             # <<<<<<<<<<<<<<
  *             if data_format == 2:
  *                 data.name = 'value'
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_stack); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 130, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_stack); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 134, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_2 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_2)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_3, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 130, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_1);
-    __pyx_t_1 = 0;
+    __pyx_t_4 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_1);
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 134, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_4);
+    __pyx_t_4 = 0;
 
-    /* "hermes/factors/base.pyx":131
+    /* "hermes/factors/base.pyx":135
  *         if data_format == 1 or data_format == 2:
  *             data = data.stack()
  *             if data_format == 2:             # <<<<<<<<<<<<<<
  *                 data.name = 'value'
  *                 data = data.reset_index()
  */
-    __pyx_t_1 = __Pyx_PyInt_EqObjC(__pyx_v_data_format, __pyx_int_2, 2, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 131, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 131, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (__pyx_t_2) {
+    __pyx_t_4 = __Pyx_PyInt_EqObjC(__pyx_v_data_format, __pyx_int_2, 2, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 135, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 135, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (__pyx_t_5) {
 
-      /* "hermes/factors/base.pyx":132
+      /* "hermes/factors/base.pyx":136
  *             data = data.stack()
  *             if data_format == 2:
  *                 data.name = 'value'             # <<<<<<<<<<<<<<
  *                 data = data.reset_index()
  *                 data['name'] = name
  */
-      if (__Pyx_PyObject_SetAttrStr(__pyx_v_data, __pyx_n_s_name, __pyx_n_s_value) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
+      if (__Pyx_PyObject_SetAttrStr(__pyx_v_data, __pyx_n_s_name, __pyx_n_s_value) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
 
-      /* "hermes/factors/base.pyx":133
+      /* "hermes/factors/base.pyx":137
  *             if data_format == 2:
  *                 data.name = 'value'
  *                 data = data.reset_index()             # <<<<<<<<<<<<<<
  *                 data['name'] = name
  *         data.name = name
  */
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_reset_index); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 133, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_5 = NULL;
-      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-        __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
-        if (likely(__pyx_t_5)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-          __Pyx_INCREF(__pyx_t_5);
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_reset_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 137, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_t_2 = NULL;
+      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+        __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
+        if (likely(__pyx_t_2)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+          __Pyx_INCREF(__pyx_t_2);
           __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_3, function);
+          __Pyx_DECREF_SET(__pyx_t_1, function);
         }
       }
-      __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
-      __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 133, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_1);
-      __pyx_t_1 = 0;
+      __pyx_t_4 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_1);
+      __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 137, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_4);
+      __pyx_t_4 = 0;
 
-      /* "hermes/factors/base.pyx":134
+      /* "hermes/factors/base.pyx":138
  *                 data.name = 'value'
  *                 data = data.reset_index()
  *                 data['name'] = name             # <<<<<<<<<<<<<<
  *         data.name = name
  *         data.category = self.category
  */
-      if (unlikely(PyObject_SetItem(__pyx_v_data, __pyx_n_s_name, __pyx_v_name) < 0)) __PYX_ERR(0, 134, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(__pyx_v_data, __pyx_n_s_name, __pyx_v_name) < 0)) __PYX_ERR(0, 138, __pyx_L1_error)
 
-      /* "hermes/factors/base.pyx":131
+      /* "hermes/factors/base.pyx":135
  *         if data_format == 1 or data_format == 2:
  *             data = data.stack()
  *             if data_format == 2:             # <<<<<<<<<<<<<<
  *                 data.name = 'value'
  *                 data = data.reset_index()
  */
     }
 
-    /* "hermes/factors/base.pyx":129
- *         #0 matrix  1 serise  2 DatFrame
- *         data_format = 1 if not hasattr(self,'_data_format') else self._data_format
+    /* "hermes/factors/base.pyx":133
+ *                                        '_data_format') else self._data_format
+ * 
  *         if data_format == 1 or data_format == 2:             # <<<<<<<<<<<<<<
  *             data = data.stack()
  *             if data_format == 2:
  */
   }
 
-  /* "hermes/factors/base.pyx":135
+  /* "hermes/factors/base.pyx":139
  *                 data = data.reset_index()
  *                 data['name'] = name
  *         data.name = name             # <<<<<<<<<<<<<<
  *         data.category = self.category
  *         data.id = self._create_id(name=name, **kwargs)
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_data, __pyx_n_s_name, __pyx_v_name) < 0) __PYX_ERR(0, 135, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_data, __pyx_n_s_name, __pyx_v_name) < 0) __PYX_ERR(0, 139, __pyx_L1_error)
 
-  /* "hermes/factors/base.pyx":136
+  /* "hermes/factors/base.pyx":140
  *                 data['name'] = name
  *         data.name = name
  *         data.category = self.category             # <<<<<<<<<<<<<<
  *         data.id = self._create_id(name=name, **kwargs)
  *         return data
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_category); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 136, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_data, __pyx_n_s_category, __pyx_t_1) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_category); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 140, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_data, __pyx_n_s_category, __pyx_t_4) < 0) __PYX_ERR(0, 140, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "hermes/factors/base.pyx":137
+  /* "hermes/factors/base.pyx":141
  *         data.name = name
  *         data.category = self.category
  *         data.id = self._create_id(name=name, **kwargs)             # <<<<<<<<<<<<<<
  *         return data
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_create_id_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 137, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 137, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_name, __pyx_v_name) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
-  __pyx_t_3 = __pyx_t_5;
-  __pyx_t_5 = 0;
-  if (__Pyx_MergeKeywords(__pyx_t_3, __pyx_v_kwargs) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 137, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_create_id_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 141, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 141, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_name, __pyx_v_name) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
+  __pyx_t_1 = __pyx_t_2;
+  __pyx_t_2 = 0;
+  if (__Pyx_MergeKeywords(__pyx_t_1, __pyx_v_kwargs) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 141, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_data, __pyx_n_s_id, __pyx_t_5) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_data, __pyx_n_s_id, __pyx_t_2) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "hermes/factors/base.pyx":138
+  /* "hermes/factors/base.pyx":142
  *         data.category = self.category
  *         data.id = self._create_id(name=name, **kwargs)
  *         return data             # <<<<<<<<<<<<<<
  * 
  *     def factors_list(self):
  */
   __Pyx_XDECREF(__pyx_r);
@@ -3322,34 +3587,35 @@
   __pyx_r = __pyx_v_data;
   goto __pyx_L0;
 
   /* "hermes/factors/base.pyx":126
  *         return "{0}".format(create_id(original=s, digit=10))
  * 
  *     def _format(self, data, name, **kwargs):             # <<<<<<<<<<<<<<
- *         #0 matrix  1 serise  2 DatFrame
- *         data_format = 1 if not hasattr(self,'_data_format') else self._data_format
+ *         # 0 matrix  1 serise  2 DatFrame
+ *         data = data.sort_values(by=['trade_date'])
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_4);
   __Pyx_AddTraceback("hermes.factors.base.FactorBase._format", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_data_format);
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "hermes/factors/base.pyx":140
+/* "hermes/factors/base.pyx":144
  *         return data
  * 
  *     def factors_list(self):             # <<<<<<<<<<<<<<
  *         return list(
  *             filter(
  */
 
@@ -3364,19 +3630,19 @@
   __pyx_r = __pyx_pf_6hermes_7factors_4base_10FactorBase_12factors_list(__pyx_self, ((PyObject *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "hermes/factors/base.pyx":143
+/* "hermes/factors/base.pyx":147
  *         return list(
  *             filter(
- *                 lambda x: not x.startswith('_')  and             # <<<<<<<<<<<<<<
- *                 callable(getattr(self, x)), dir(self)))
+ *                 lambda x: not x.startswith('_') and callable(getattr(self, x)),             # <<<<<<<<<<<<<<
+ *                 dir(self)))
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_6hermes_7factors_4base_10FactorBase_12factors_list_lambda(PyObject *__pyx_self, PyObject *__pyx_v_x); /*proto*/
 static PyMethodDef __pyx_mdef_6hermes_7factors_4base_10FactorBase_12factors_list_lambda = {"lambda", (PyCFunction)__pyx_pw_6hermes_7factors_4base_10FactorBase_12factors_list_lambda, METH_O, 0};
 static PyObject *__pyx_pw_6hermes_7factors_4base_10FactorBase_12factors_list_lambda(PyObject *__pyx_self, PyObject *__pyx_v_x) {
   PyObject *__pyx_r = 0;
@@ -3403,87 +3669,74 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("lambda", 0);
   __pyx_outer_scope = (struct __pyx_obj_6hermes_7factors_4base___pyx_scope_struct__factors_list *) __Pyx_CyFunction_GetClosure(__pyx_self);
   __pyx_cur_scope = __pyx_outer_scope;
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_x, __pyx_n_s_startswith); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 143, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_x, __pyx_n_s_startswith); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 147, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_n_s_) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_n_s_);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 143, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 147, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 143, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 147, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_6 = (!__pyx_t_5);
   if (__pyx_t_6) {
   } else {
-    __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 143, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 147, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_1 = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L3_bool_binop_done;
   }
-
-  /* "hermes/factors/base.pyx":144
- *             filter(
- *                 lambda x: not x.startswith('_')  and
- *                 callable(getattr(self, x)), dir(self)))             # <<<<<<<<<<<<<<
- */
-  if (unlikely(!__pyx_cur_scope->__pyx_v_self)) { __Pyx_RaiseClosureNameError("self"); __PYX_ERR(0, 144, __pyx_L1_error) }
+  if (unlikely(!__pyx_cur_scope->__pyx_v_self)) { __Pyx_RaiseClosureNameError("self"); __PYX_ERR(0, 147, __pyx_L1_error) }
   __pyx_t_2 = __pyx_cur_scope->__pyx_v_self;
   __Pyx_INCREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_GetAttr(__pyx_t_2, __pyx_v_x); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 144, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetAttr(__pyx_t_2, __pyx_v_x); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 147, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_6 = __Pyx_PyCallable_Check(__pyx_t_3); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 144, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyCallable_Check(__pyx_t_3); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 147, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyBool_FromLong(__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 144, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyBool_FromLong(__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 147, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_1 = __pyx_t_3;
   __pyx_t_3 = 0;
   __pyx_L3_bool_binop_done:;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "hermes/factors/base.pyx":143
- *         return list(
- *             filter(
- *                 lambda x: not x.startswith('_')  and             # <<<<<<<<<<<<<<
- *                 callable(getattr(self, x)), dir(self)))
- */
-
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_AddTraceback("hermes.factors.base.FactorBase.factors_list.lambda", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "hermes/factors/base.pyx":140
+/* "hermes/factors/base.pyx":144
  *         return data
  * 
  *     def factors_list(self):             # <<<<<<<<<<<<<<
  *         return list(
  *             filter(
  */
 
@@ -3498,85 +3751,85 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("factors_list", 0);
   __pyx_cur_scope = (struct __pyx_obj_6hermes_7factors_4base___pyx_scope_struct__factors_list *)__pyx_tp_new_6hermes_7factors_4base___pyx_scope_struct__factors_list(__pyx_ptype_6hermes_7factors_4base___pyx_scope_struct__factors_list, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_6hermes_7factors_4base___pyx_scope_struct__factors_list *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 140, __pyx_L1_error)
+    __PYX_ERR(0, 144, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_self);
 
-  /* "hermes/factors/base.pyx":141
+  /* "hermes/factors/base.pyx":145
  * 
  *     def factors_list(self):
  *         return list(             # <<<<<<<<<<<<<<
  *             filter(
- *                 lambda x: not x.startswith('_')  and
+ *                 lambda x: not x.startswith('_') and callable(getattr(self, x)),
  */
   __Pyx_XDECREF(__pyx_r);
 
-  /* "hermes/factors/base.pyx":143
+  /* "hermes/factors/base.pyx":147
  *         return list(
  *             filter(
- *                 lambda x: not x.startswith('_')  and             # <<<<<<<<<<<<<<
- *                 callable(getattr(self, x)), dir(self)))
+ *                 lambda x: not x.startswith('_') and callable(getattr(self, x)),             # <<<<<<<<<<<<<<
+ *                 dir(self)))
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_12factors_list_lambda, 0, __pyx_n_s_FactorBase_factors_list_locals_l, ((PyObject*)__pyx_cur_scope), __pyx_n_s_hermes_factors_base, __pyx_d, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_12factors_list_lambda, 0, __pyx_n_s_FactorBase_factors_list_locals_l, ((PyObject*)__pyx_cur_scope), __pyx_n_s_hermes_factors_base, __pyx_d, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 147, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "hermes/factors/base.pyx":144
+  /* "hermes/factors/base.pyx":148
  *             filter(
- *                 lambda x: not x.startswith('_')  and
- *                 callable(getattr(self, x)), dir(self)))             # <<<<<<<<<<<<<<
+ *                 lambda x: not x.startswith('_') and callable(getattr(self, x)),
+ *                 dir(self)))             # <<<<<<<<<<<<<<
  */
   __pyx_t_2 = __pyx_cur_scope->__pyx_v_self;
   __Pyx_INCREF(__pyx_t_2);
-  __pyx_t_3 = PyObject_Dir(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 144, __pyx_L1_error)
+  __pyx_t_3 = PyObject_Dir(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 148, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "hermes/factors/base.pyx":142
+  /* "hermes/factors/base.pyx":146
  *     def factors_list(self):
  *         return list(
  *             filter(             # <<<<<<<<<<<<<<
- *                 lambda x: not x.startswith('_')  and
- *                 callable(getattr(self, x)), dir(self)))
+ *                 lambda x: not x.startswith('_') and callable(getattr(self, x)),
+ *                 dir(self)))
  */
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 142, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_3);
   __pyx_t_1 = 0;
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_filter, __pyx_t_2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 142, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_filter, __pyx_t_2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "hermes/factors/base.pyx":141
+  /* "hermes/factors/base.pyx":145
  * 
  *     def factors_list(self):
  *         return list(             # <<<<<<<<<<<<<<
  *             filter(
- *                 lambda x: not x.startswith('_')  and
+ *                 lambda x: not x.startswith('_') and callable(getattr(self, x)),
  */
-  __pyx_t_2 = PySequence_List(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 141, __pyx_L1_error)
+  __pyx_t_2 = PySequence_List(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 145, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "hermes/factors/base.pyx":140
+  /* "hermes/factors/base.pyx":144
  *         return data
  * 
  *     def factors_list(self):             # <<<<<<<<<<<<<<
  *         return list(
  *             filter(
  */
 
@@ -3709,14 +3962,143 @@
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
 
+static int __pyx_import_star_set(PyObject *o, PyObject* py_name, char *name) {
+  static const char* internal_type_names[] = {
+    "__pyx_scope_struct__factors_list",
+    0
+  };
+  const char** type_name = internal_type_names;
+  while (*type_name) {
+    if (__Pyx_StrEq(name, *type_name)) {
+      PyErr_Format(PyExc_TypeError, "Cannot overwrite C type %s", name);
+      goto bad;
+    }
+    type_name++;
+  }
+  if (0);
+  else {
+    if (PyObject_SetAttr(__pyx_m, py_name, o) < 0) goto bad;
+  }
+  return 0;
+  bad:
+  return -1;
+}
+
+static int
+__Pyx_import_all_from(PyObject *locals, PyObject *v)
+{
+    PyObject *all = PyObject_GetAttrString(v, "__all__");
+    PyObject *dict, *name, *value;
+    int skip_leading_underscores = 0;
+    int pos, err;
+    if (all == NULL) {
+        if (!PyErr_ExceptionMatches(PyExc_AttributeError))
+            return -1;
+        PyErr_Clear();
+        dict = PyObject_GetAttrString(v, "__dict__");
+        if (dict == NULL) {
+            if (!PyErr_ExceptionMatches(PyExc_AttributeError))
+                return -1;
+            PyErr_SetString(PyExc_ImportError,
+            "from-import-* object has no __dict__ and no __all__");
+            return -1;
+        }
+#if PY_MAJOR_VERSION < 3
+        all = PyObject_CallMethod(dict, (char *)"keys", NULL);
+#else
+        all = PyMapping_Keys(dict);
+#endif
+        Py_DECREF(dict);
+        if (all == NULL)
+            return -1;
+        skip_leading_underscores = 1;
+    }
+    for (pos = 0, err = 0; ; pos++) {
+        name = PySequence_GetItem(all, pos);
+        if (name == NULL) {
+            if (!PyErr_ExceptionMatches(PyExc_IndexError))
+                err = -1;
+            else
+                PyErr_Clear();
+            break;
+        }
+        if (skip_leading_underscores &&
+#if PY_MAJOR_VERSION < 3
+            likely(PyString_Check(name)) &&
+            PyString_AS_STRING(name)[0] == '_')
+#else
+            likely(PyUnicode_Check(name)) &&
+            likely(__Pyx_PyUnicode_GET_LENGTH(name)) &&
+            __Pyx_PyUnicode_READ_CHAR(name, 0) == '_')
+#endif
+        {
+            Py_DECREF(name);
+            continue;
+        }
+        value = PyObject_GetAttr(v, name);
+        if (value == NULL)
+            err = -1;
+        else if (PyDict_CheckExact(locals))
+            err = PyDict_SetItem(locals, name, value);
+        else
+            err = PyObject_SetItem(locals, name, value);
+        Py_DECREF(name);
+        Py_XDECREF(value);
+        if (err != 0)
+            break;
+    }
+    Py_DECREF(all);
+    return err;
+}
+static int __pyx_import_star(PyObject* m) {
+    int i;
+    int ret = -1;
+    char* s;
+    PyObject *locals = 0;
+    PyObject *list = 0;
+#if PY_MAJOR_VERSION >= 3
+    PyObject *utf8_name = 0;
+#endif
+    PyObject *name;
+    PyObject *item;
+    locals = PyDict_New();              if (!locals) goto bad;
+    if (__Pyx_import_all_from(locals, m) < 0) goto bad;
+    list = PyDict_Items(locals);        if (!list) goto bad;
+    for(i=0; i<PyList_GET_SIZE(list); i++) {
+        name = PyTuple_GET_ITEM(PyList_GET_ITEM(list, i), 0);
+        item = PyTuple_GET_ITEM(PyList_GET_ITEM(list, i), 1);
+#if PY_MAJOR_VERSION >= 3
+        utf8_name = PyUnicode_AsUTF8String(name);
+        if (!utf8_name) goto bad;
+        s = PyBytes_AS_STRING(utf8_name);
+        if (__pyx_import_star_set(item, name, s) < 0) goto bad;
+        Py_DECREF(utf8_name); utf8_name = 0;
+#else
+        s = PyString_AsString(name);
+        if (!s) goto bad;
+        if (__pyx_import_star_set(item, name, s) < 0) goto bad;
+#endif
+    }
+    ret = 0;
+bad:
+    Py_XDECREF(locals);
+    Py_XDECREF(list);
+#if PY_MAJOR_VERSION >= 3
+    Py_XDECREF(utf8_name);
+#endif
+    return ret;
+}
+
+
+
 #if PY_MAJOR_VERSION >= 3
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
 static int __pyx_pymod_exec_base(PyObject* module); /*proto*/
 static PyModuleDef_Slot __pyx_moduledef_slots[] = {
   {Py_mod_create, (void*)__pyx_pymod_create},
   {Py_mod_exec, (void*)__pyx_pymod_exec_base},
@@ -3753,14 +4135,15 @@
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
   {&__pyx_n_s_, __pyx_k_, sizeof(__pyx_k_), 0, 0, 1, 1},
   {&__pyx_kp_s_0, __pyx_k_0, sizeof(__pyx_k_0), 0, 0, 1, 0},
+  {&__pyx_kp_s_0_b, __pyx_k_0_b, sizeof(__pyx_k_0_b), 0, 0, 1, 0},
   {&__pyx_n_s_ABCMeta, __pyx_k_ABCMeta, sizeof(__pyx_k_ABCMeta), 0, 0, 1, 1},
   {&__pyx_n_s_FactorBase, __pyx_k_FactorBase, sizeof(__pyx_k_FactorBase), 0, 0, 1, 1},
   {&__pyx_n_s_FactorBase___init, __pyx_k_FactorBase___init, sizeof(__pyx_k_FactorBase___init), 0, 0, 1, 1},
   {&__pyx_n_s_FactorBase__create_id, __pyx_k_FactorBase__create_id, sizeof(__pyx_k_FactorBase__create_id), 0, 0, 1, 1},
   {&__pyx_n_s_FactorBase__format, __pyx_k_FactorBase__format, sizeof(__pyx_k_FactorBase__format), 0, 0, 1, 1},
   {&__pyx_n_s_FactorBase__init_self, __pyx_k_FactorBase__init_self, sizeof(__pyx_k_FactorBase__init_self), 0, 0, 1, 1},
   {&__pyx_n_s_FactorBase_factors_list, __pyx_k_FactorBase_factors_list, sizeof(__pyx_k_FactorBase_factors_list), 0, 0, 1, 1},
@@ -3775,20 +4158,25 @@
   {&__pyx_n_s_ParamBase, __pyx_k_ParamBase, sizeof(__pyx_k_ParamBase), 0, 0, 1, 1},
   {&__pyx_n_s_ShortCallMixin, __pyx_k_ShortCallMixin, sizeof(__pyx_k_ShortCallMixin), 0, 0, 1, 1},
   {&__pyx_n_s_ShortCallMixin_expect_direction, __pyx_k_ShortCallMixin_expect_direction, sizeof(__pyx_k_ShortCallMixin_expect_direction), 0, 0, 1, 1},
   {&__pyx_n_s_ShortCallMixin_short_type_str, __pyx_k_ShortCallMixin_short_type_str, sizeof(__pyx_k_ShortCallMixin_short_type_str), 0, 0, 1, 1},
   {&__pyx_n_s_ShortMixin, __pyx_k_ShortMixin, sizeof(__pyx_k_ShortMixin), 0, 0, 1, 1},
   {&__pyx_n_s_ShortMixin_expect_direction, __pyx_k_ShortMixin_expect_direction, sizeof(__pyx_k_ShortMixin_expect_direction), 0, 0, 1, 1},
   {&__pyx_n_s_ShortMixin_short_type_str, __pyx_k_ShortMixin_short_type_str, sizeof(__pyx_k_ShortMixin_short_type_str), 0, 0, 1, 1},
+  {&__pyx_kp_s_Y_m_d, __pyx_k_Y_m_d, sizeof(__pyx_k_Y_m_d), 0, 0, 1, 0},
+  {&__pyx_n_s__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 0, 1, 1},
   {&__pyx_n_s_abc, __pyx_k_abc, sizeof(__pyx_k_abc), 0, 0, 1, 1},
   {&__pyx_n_s_abstractmethod, __pyx_k_abstractmethod, sizeof(__pyx_k_abstractmethod), 0, 0, 1, 1},
+  {&__pyx_n_s_advanceDateByCalendar, __pyx_k_advanceDateByCalendar, sizeof(__pyx_k_advanceDateByCalendar), 0, 0, 1, 1},
   {&__pyx_n_s_begin_date, __pyx_k_begin_date, sizeof(__pyx_k_begin_date), 0, 0, 1, 1},
   {&__pyx_kp_s_buy_call, __pyx_k_buy_call, sizeof(__pyx_k_buy_call), 0, 0, 1, 0},
   {&__pyx_kp_s_buy_put, __pyx_k_buy_put, sizeof(__pyx_k_buy_put), 0, 0, 1, 0},
+  {&__pyx_n_s_by, __pyx_k_by, sizeof(__pyx_k_by), 0, 0, 1, 1},
   {&__pyx_n_s_category, __pyx_k_category, sizeof(__pyx_k_category), 0, 0, 1, 1},
+  {&__pyx_kp_s_china_sse, __pyx_k_china_sse, sizeof(__pyx_k_china_sse), 0, 0, 1, 0},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_columns, __pyx_k_columns, sizeof(__pyx_k_columns), 0, 0, 1, 1},
   {&__pyx_n_s_copy, __pyx_k_copy, sizeof(__pyx_k_copy), 0, 0, 1, 1},
   {&__pyx_n_s_create_id, __pyx_k_create_id, sizeof(__pyx_k_create_id), 0, 0, 1, 1},
   {&__pyx_n_s_create_id_2, __pyx_k_create_id_2, sizeof(__pyx_k_create_id_2), 0, 0, 1, 1},
   {&__pyx_n_s_data, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
   {&__pyx_n_s_data_format, __pyx_k_data_format, sizeof(__pyx_k_data_format), 0, 0, 1, 1},
@@ -3826,16 +4214,18 @@
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_init, __pyx_k_init, sizeof(__pyx_k_init), 0, 0, 1, 1},
   {&__pyx_n_s_init_data, __pyx_k_init_data, sizeof(__pyx_k_init_data), 0, 0, 1, 1},
   {&__pyx_n_s_init_self, __pyx_k_init_self, sizeof(__pyx_k_init_self), 0, 0, 1, 1},
   {&__pyx_n_s_inspect, __pyx_k_inspect, sizeof(__pyx_k_inspect), 0, 0, 1, 1},
   {&__pyx_n_s_items, __pyx_k_items, sizeof(__pyx_k_items), 0, 0, 1, 1},
   {&__pyx_n_s_jdwdata_RetrievalAPI, __pyx_k_jdwdata_RetrievalAPI, sizeof(__pyx_k_jdwdata_RetrievalAPI), 0, 0, 1, 1},
+  {&__pyx_n_s_jdwdate_api, __pyx_k_jdwdate_api, sizeof(__pyx_k_jdwdate_api), 0, 0, 1, 1},
   {&__pyx_n_s_json, __pyx_k_json, sizeof(__pyx_k_json), 0, 0, 1, 1},
   {&__pyx_n_s_kwargs, __pyx_k_kwargs, sizeof(__pyx_k_kwargs), 0, 0, 1, 1},
+  {&__pyx_n_s_loc, __pyx_k_loc, sizeof(__pyx_k_loc), 0, 0, 1, 1},
   {&__pyx_n_s_long, __pyx_k_long, sizeof(__pyx_k_long), 0, 0, 1, 1},
   {&__pyx_n_s_long_type_str, __pyx_k_long_type_str, sizeof(__pyx_k_long_type_str), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_md5, __pyx_k_md5, sizeof(__pyx_k_md5), 0, 0, 1, 1},
   {&__pyx_n_s_member_func, __pyx_k_member_func, sizeof(__pyx_k_member_func), 0, 0, 1, 1},
   {&__pyx_n_s_metaclass, __pyx_k_metaclass, sizeof(__pyx_k_metaclass), 0, 0, 1, 1},
   {&__pyx_n_s_method, __pyx_k_method, sizeof(__pyx_k_method), 0, 0, 1, 1},
@@ -3850,223 +4240,229 @@
   {&__pyx_n_s_reset_index, __pyx_k_reset_index, sizeof(__pyx_k_reset_index), 0, 0, 1, 1},
   {&__pyx_n_s_s, __pyx_k_s, sizeof(__pyx_k_s), 0, 0, 1, 1},
   {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
   {&__pyx_n_s_short, __pyx_k_short, sizeof(__pyx_k_short), 0, 0, 1, 1},
   {&__pyx_n_s_short_type_str, __pyx_k_short_type_str, sizeof(__pyx_k_short_type_str), 0, 0, 1, 1},
   {&__pyx_n_s_signature, __pyx_k_signature, sizeof(__pyx_k_signature), 0, 0, 1, 1},
   {&__pyx_n_s_six, __pyx_k_six, sizeof(__pyx_k_six), 0, 0, 1, 1},
+  {&__pyx_n_s_sort_values, __pyx_k_sort_values, sizeof(__pyx_k_sort_values), 0, 0, 1, 1},
   {&__pyx_n_s_stack, __pyx_k_stack, sizeof(__pyx_k_stack), 0, 0, 1, 1},
+  {&__pyx_n_s_start_date, __pyx_k_start_date, sizeof(__pyx_k_start_date), 0, 0, 1, 1},
   {&__pyx_n_s_startswith, __pyx_k_startswith, sizeof(__pyx_k_startswith), 0, 0, 1, 1},
+  {&__pyx_n_s_strftime, __pyx_k_strftime, sizeof(__pyx_k_strftime), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
+  {&__pyx_n_s_trade_date, __pyx_k_trade_date, sizeof(__pyx_k_trade_date), 0, 0, 1, 1},
   {&__pyx_kp_s_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 0, 1, 0},
   {&__pyx_n_s_value, __pyx_k_value, sizeof(__pyx_k_value), 0, 0, 1, 1},
+  {&__pyx_n_s_window, __pyx_k_window, sizeof(__pyx_k_window), 0, 0, 1, 1},
   {&__pyx_n_s_with_metaclass, __pyx_k_with_metaclass, sizeof(__pyx_k_with_metaclass), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_filter = __Pyx_GetBuiltinName(__pyx_n_s_filter); if (!__pyx_builtin_filter) __PYX_ERR(0, 142, __pyx_L1_error)
+  __pyx_builtin_filter = __Pyx_GetBuiltinName(__pyx_n_s_filter); if (!__pyx_builtin_filter) __PYX_ERR(0, 146, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "hermes/factors/base.pyx":17
+  /* "hermes/factors/base.pyx":18
  * 
  *     @LazyFunc
  *     def long_type_str(self):             # <<<<<<<<<<<<<<
  *         """unique call"""
  *         return "long"
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__2);
-  __Pyx_GIVEREF(__pyx_tuple__2);
-  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__2, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_long_type_str, 17, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__3);
+  __Pyx_GIVEREF(__pyx_tuple__3);
+  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_long_type_str, 18, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 18, __pyx_L1_error)
 
-  /* "hermes/factors/base.pyx":22
+  /* "hermes/factors/base.pyx":23
  * 
  *     @LazyFunc
  *     def expect_direction(self):             # <<<<<<<<<<<<<<
  *         """1.0"""
  *         return 1.0
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 22, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__4);
-  __Pyx_GIVEREF(__pyx_tuple__4);
-  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_expect_direction, 22, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 22, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 23, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__5);
+  __Pyx_GIVEREF(__pyx_tuple__5);
+  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_expect_direction, 23, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 23, __pyx_L1_error)
 
-  /* "hermes/factors/base.pyx":35
+  /* "hermes/factors/base.pyx":36
  * 
  *     @LazyFunc
  *     def short_type_str(self):             # <<<<<<<<<<<<<<
  *         """unique put"""
  *         return "short"
  */
-  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 35, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__6);
-  __Pyx_GIVEREF(__pyx_tuple__6);
-  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_short_type_str, 35, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__7);
+  __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_short_type_str, 36, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 36, __pyx_L1_error)
 
-  /* "hermes/factors/base.pyx":40
+  /* "hermes/factors/base.pyx":41
  * 
  *     @LazyFunc
  *     def expect_direction(self):             # <<<<<<<<<<<<<<
  *         """1.0"""
  *         return -1.0
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 40, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
-  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_expect_direction, 40, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_expect_direction, 41, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 41, __pyx_L1_error)
 
   /* "hermes/factors/base.pyx":54
  * 
  *     @LazyFunc
  *     def short_type_str(self):             # <<<<<<<<<<<<<<
  *         """unique put"""
  *         return "short"
  */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 54, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__10);
-  __Pyx_GIVEREF(__pyx_tuple__10);
-  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_short_type_str, 54, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 54, __pyx_L1_error)
+  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 54, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
+  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_short_type_str, 54, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 54, __pyx_L1_error)
 
   /* "hermes/factors/base.pyx":59
  * 
  *     @LazyFunc
  *     def expect_direction(self):             # <<<<<<<<<<<<<<
  *         """1.0"""
  *         return -1.0
  */
-  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 59, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__12);
-  __Pyx_GIVEREF(__pyx_tuple__12);
-  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_expect_direction, 59, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 59, __pyx_L1_error)
+  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 59, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__13);
+  __Pyx_GIVEREF(__pyx_tuple__13);
+  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_expect_direction, 59, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 59, __pyx_L1_error)
 
   /* "hermes/factors/base.pyx":72
  * 
  *     @LazyFunc
  *     def short_type_str(self):             # <<<<<<<<<<<<<<
  *         """unique put"""
  *         return "short"
  */
-  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 72, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__14);
-  __Pyx_GIVEREF(__pyx_tuple__14);
-  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_short_type_str, 72, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__15);
+  __Pyx_GIVEREF(__pyx_tuple__15);
+  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_short_type_str, 72, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 72, __pyx_L1_error)
 
   /* "hermes/factors/base.pyx":77
  * 
  *     @LazyFunc
  *     def expect_direction(self):             # <<<<<<<<<<<<<<
  *         """1.0"""
  *         return -1.0
  */
-  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 77, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__16);
-  __Pyx_GIVEREF(__pyx_tuple__16);
-  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_expect_direction, 77, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__17);
+  __Pyx_GIVEREF(__pyx_tuple__17);
+  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_expect_direction, 77, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 77, __pyx_L1_error)
 
   /* "hermes/factors/base.pyx":84
  * class FactorBase(six.with_metaclass(ABCMeta, ParamBase)):
  * 
  *     def __init__(self, **kwargs):             # <<<<<<<<<<<<<<
  *         #
  *         self._init_self(**kwargs)
  */
-  __pyx_tuple__18 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_kwargs); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 84, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__18);
-  __Pyx_GIVEREF(__pyx_tuple__18);
-  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_init, 84, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __pyx_tuple__19 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_kwargs); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__19);
+  __Pyx_GIVEREF(__pyx_tuple__19);
+  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_init, 84, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 84, __pyx_L1_error)
 
-  /* "hermes/factors/base.pyx":90
+  /* "hermes/factors/base.pyx":89
  * 
  *     @abstractmethod
  *     def _init_self(self, **kwargs):             # <<<<<<<<<<<<<<
  *         """"""
  *         pass
  */
-  __pyx_tuple__20 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_kwargs); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 90, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__20);
-  __Pyx_GIVEREF(__pyx_tuple__20);
-  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_init_self, 90, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __pyx_tuple__21 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_kwargs); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__21);
+  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_init_self, 89, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 89, __pyx_L1_error)
 
-  /* "hermes/factors/base.pyx":94
+  /* "hermes/factors/base.pyx":93
  *         pass
  * 
  *     def init_data(self, **kwargs):             # <<<<<<<<<<<<<<
  *         dependencies_list = self.get_dependencies()
  *         method = 'ddb' if 'method' not in kwargs else kwargs['method']
  */
-  __pyx_tuple__22 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_kwargs, __pyx_n_s_dependencies_list, __pyx_n_s_method, __pyx_n_s_data); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 94, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__22);
-  __Pyx_GIVEREF(__pyx_tuple__22);
-  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(1, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_init_data, 94, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_tuple__23 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_kwargs, __pyx_n_s_dependencies_list, __pyx_n_s_method, __pyx_n_s_window, __pyx_n_s_start_date, __pyx_n_s_data); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__23);
+  __Pyx_GIVEREF(__pyx_tuple__23);
+  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(1, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_init_data, 93, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 93, __pyx_L1_error)
 
-  /* "hermes/factors/base.pyx":105
- * 
+  /* "hermes/factors/base.pyx":108
+ *         return data
  * 
  *     def get_dependencies(self):             # <<<<<<<<<<<<<<
  *         dependencies_list = []
  *         member_func = self.factors_list()
  */
-  __pyx_tuple__24 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_dependencies_list, __pyx_n_s_member_func, __pyx_n_s_func, __pyx_n_s_func_module, __pyx_n_s_fun_param, __pyx_n_s_dependencies); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 105, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__24);
-  __Pyx_GIVEREF(__pyx_tuple__24);
-  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(1, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_get_dependencies, 105, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __pyx_tuple__25 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_dependencies_list, __pyx_n_s_member_func, __pyx_n_s_func, __pyx_n_s_func_module, __pyx_n_s_fun_param, __pyx_n_s_dependencies); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 108, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__25);
+  __Pyx_GIVEREF(__pyx_tuple__25);
+  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(1, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_get_dependencies, 108, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(0, 108, __pyx_L1_error)
 
   /* "hermes/factors/base.pyx":119
- * 
+ *         return list(set(dependencies_list))
  * 
  *     def _create_id(self, **kwargs):             # <<<<<<<<<<<<<<
  *         feature = copy.deepcopy(kwargs)
  *         feature['category'] = self.category
  */
-  __pyx_tuple__26 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_kwargs, __pyx_n_s_feature, __pyx_n_s_s); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 119, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__26);
-  __Pyx_GIVEREF(__pyx_tuple__26);
-  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_create_id_2, 119, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __pyx_tuple__27 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_kwargs, __pyx_n_s_feature, __pyx_n_s_s); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__27);
+  __Pyx_GIVEREF(__pyx_tuple__27);
+  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_create_id_2, 119, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(0, 119, __pyx_L1_error)
 
   /* "hermes/factors/base.pyx":126
  *         return "{0}".format(create_id(original=s, digit=10))
  * 
  *     def _format(self, data, name, **kwargs):             # <<<<<<<<<<<<<<
- *         #0 matrix  1 serise  2 DatFrame
- *         data_format = 1 if not hasattr(self,'_data_format') else self._data_format
+ *         # 0 matrix  1 serise  2 DatFrame
+ *         data = data.sort_values(by=['trade_date'])
  */
-  __pyx_tuple__28 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_data, __pyx_n_s_name, __pyx_n_s_kwargs, __pyx_n_s_data_format_2); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 126, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__28);
-  __Pyx_GIVEREF(__pyx_tuple__28);
-  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_format_2, 126, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 126, __pyx_L1_error)
+  __pyx_tuple__29 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_data, __pyx_n_s_name, __pyx_n_s_kwargs, __pyx_n_s_data_format_2); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(0, 126, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__29);
+  __Pyx_GIVEREF(__pyx_tuple__29);
+  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_format_2, 126, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 126, __pyx_L1_error)
 
-  /* "hermes/factors/base.pyx":140
+  /* "hermes/factors/base.pyx":144
  *         return data
  * 
  *     def factors_list(self):             # <<<<<<<<<<<<<<
  *         return list(
  *             filter(
  */
-  __pyx_tuple__30 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(0, 140, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__30);
-  __Pyx_GIVEREF(__pyx_tuple__30);
-  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__30, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_factors_list, 140, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 140, __pyx_L1_error)
+  __pyx_tuple__31 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 144, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__31);
+  __Pyx_GIVEREF(__pyx_tuple__31);
+  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hermes_factors_base_pyx, __pyx_n_s_factors_list, 144, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   __pyx_float_1_0 = PyFloat_FromDouble(1.0); if (unlikely(!__pyx_float_1_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_neg_1_0 = PyFloat_FromDouble(-1.0); if (unlikely(!__pyx_float_neg_1_0)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_2 = PyInt_FromLong(2); if (unlikely(!__pyx_int_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_10 = PyInt_FromLong(10); if (unlikely(!__pyx_int_10)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
@@ -4106,15 +4502,15 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  if (PyType_Ready(&__pyx_type_6hermes_7factors_4base___pyx_scope_struct__factors_list) < 0) __PYX_ERR(0, 140, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6hermes_7factors_4base___pyx_scope_struct__factors_list) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6hermes_7factors_4base___pyx_scope_struct__factors_list.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6hermes_7factors_4base___pyx_scope_struct__factors_list.tp_dictoffset && __pyx_type_6hermes_7factors_4base___pyx_scope_struct__factors_list.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6hermes_7factors_4base___pyx_scope_struct__factors_list.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_6hermes_7factors_4base___pyx_scope_struct__factors_list = &__pyx_type_6hermes_7factors_4base___pyx_scope_struct__factors_list;
@@ -4398,15 +4794,15 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "hermes/factors/base.pyx":4
  * import copy, hashlib, json, inspect, pdb
  * import six as six
  * from abc import ABCMeta, abstractmethod             # <<<<<<<<<<<<<<
  * from jdwdata.RetrievalAPI import get_data_by_map
- * from hermes.kdutils.create_id import create_id
+ * from jdwdate.api import *
  */
   __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_ABCMeta);
   __Pyx_GIVEREF(__pyx_n_s_ABCMeta);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_ABCMeta);
   __Pyx_INCREF(__pyx_n_s_abstractmethod);
@@ -4425,16 +4821,16 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "hermes/factors/base.pyx":5
  * import six as six
  * from abc import ABCMeta, abstractmethod
  * from jdwdata.RetrievalAPI import get_data_by_map             # <<<<<<<<<<<<<<
+ * from jdwdate.api import *
  * from hermes.kdutils.create_id import create_id
- * from hermes.kdutils.lazy import LazyFunc
  */
   __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_get_data_by_map);
   __Pyx_GIVEREF(__pyx_n_s_get_data_by_map);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_get_data_by_map);
   __pyx_t_1 = __Pyx_Import(__pyx_n_s_jdwdata_RetrievalAPI, __pyx_t_2, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 5, __pyx_L1_error)
@@ -4445,318 +4841,336 @@
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_data_by_map, __pyx_t_2) < 0) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "hermes/factors/base.pyx":6
  * from abc import ABCMeta, abstractmethod
  * from jdwdata.RetrievalAPI import get_data_by_map
- * from hermes.kdutils.create_id import create_id             # <<<<<<<<<<<<<<
+ * from jdwdate.api import *             # <<<<<<<<<<<<<<
+ * from hermes.kdutils.create_id import create_id
  * from hermes.kdutils.lazy import LazyFunc
- * from hermes.kdutils.base import ParamBase, FreezeAttrMixin
  */
   __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_INCREF(__pyx_n_s_create_id);
-  __Pyx_GIVEREF(__pyx_n_s_create_id);
-  PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_create_id);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_hermes_kdutils_create_id, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 6, __pyx_L1_error)
+  __Pyx_INCREF(__pyx_n_s__2);
+  __Pyx_GIVEREF(__pyx_n_s__2);
+  PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s__2);
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_jdwdate_api, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_create_id); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 6, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_create_id, __pyx_t_1) < 0) __PYX_ERR(0, 6, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (__pyx_import_star(__pyx_t_2) < 0) __PYX_ERR(0, 6, __pyx_L1_error);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "hermes/factors/base.pyx":7
  * from jdwdata.RetrievalAPI import get_data_by_map
- * from hermes.kdutils.create_id import create_id
- * from hermes.kdutils.lazy import LazyFunc             # <<<<<<<<<<<<<<
+ * from jdwdate.api import *
+ * from hermes.kdutils.create_id import create_id             # <<<<<<<<<<<<<<
+ * from hermes.kdutils.lazy import LazyFunc
  * from hermes.kdutils.base import ParamBase, FreezeAttrMixin
- * 
  */
   __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_INCREF(__pyx_n_s_LazyFunc);
-  __Pyx_GIVEREF(__pyx_n_s_LazyFunc);
-  PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_LazyFunc);
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_hermes_kdutils_lazy, __pyx_t_2, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 7, __pyx_L1_error)
+  __Pyx_INCREF(__pyx_n_s_create_id);
+  __Pyx_GIVEREF(__pyx_n_s_create_id);
+  PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_create_id);
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_hermes_kdutils_create_id, __pyx_t_2, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_LazyFunc); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 7, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_create_id); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_LazyFunc, __pyx_t_2) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_create_id, __pyx_t_2) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "hermes/factors/base.pyx":8
+ * from jdwdate.api import *
+ * from hermes.kdutils.create_id import create_id
+ * from hermes.kdutils.lazy import LazyFunc             # <<<<<<<<<<<<<<
+ * from hermes.kdutils.base import ParamBase, FreezeAttrMixin
+ * 
+ */
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 8, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_INCREF(__pyx_n_s_LazyFunc);
+  __Pyx_GIVEREF(__pyx_n_s_LazyFunc);
+  PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_LazyFunc);
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_hermes_kdutils_lazy, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 8, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_LazyFunc); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 8, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_LazyFunc, __pyx_t_1) < 0) __PYX_ERR(0, 8, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "hermes/factors/base.pyx":9
  * from hermes.kdutils.create_id import create_id
  * from hermes.kdutils.lazy import LazyFunc
  * from hermes.kdutils.base import ParamBase, FreezeAttrMixin             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 8, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = PyList_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_ParamBase);
   __Pyx_GIVEREF(__pyx_n_s_ParamBase);
-  PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_ParamBase);
+  PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_ParamBase);
   __Pyx_INCREF(__pyx_n_s_FreezeAttrMixin);
   __Pyx_GIVEREF(__pyx_n_s_FreezeAttrMixin);
-  PyList_SET_ITEM(__pyx_t_1, 1, __pyx_n_s_FreezeAttrMixin);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_hermes_kdutils_base, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 8, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_ParamBase); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 8, __pyx_L1_error)
+  PyList_SET_ITEM(__pyx_t_2, 1, __pyx_n_s_FreezeAttrMixin);
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_hermes_kdutils_base, __pyx_t_2, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ParamBase, __pyx_t_1) < 0) __PYX_ERR(0, 8, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_FreezeAttrMixin); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 8, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_FreezeAttrMixin, __pyx_t_1) < 0) __PYX_ERR(0, 8, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_ParamBase); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ParamBase, __pyx_t_2) < 0) __PYX_ERR(0, 9, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_FreezeAttrMixin); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_FreezeAttrMixin, __pyx_t_2) < 0) __PYX_ERR(0, 9, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "hermes/factors/base.pyx":11
+  /* "hermes/factors/base.pyx":12
  * 
  * 
  * class LongCallMixin(FreezeAttrMixin):             # <<<<<<<<<<<<<<
  *     """
  *         buy call
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_FreezeAttrMixin); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 11, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 11, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_FreezeAttrMixin); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GIVEREF(__pyx_t_2);
-  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_2);
-  __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 11, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_1, __pyx_n_s_LongCallMixin, __pyx_n_s_LongCallMixin, (PyObject *) NULL, __pyx_n_s_hermes_factors_base, __pyx_kp_s_buy_call); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 11, __pyx_L1_error)
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
+  __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_t_2, __pyx_n_s_LongCallMixin, __pyx_n_s_LongCallMixin, (PyObject *) NULL, __pyx_n_s_hermes_factors_base, __pyx_kp_s_buy_call); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "hermes/factors/base.pyx":16
+  /* "hermes/factors/base.pyx":17
  *     """
  * 
  *     @LazyFunc             # <<<<<<<<<<<<<<
  *     def long_type_str(self):
  *         """unique call"""
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_LazyFunc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_LazyFunc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
 
-  /* "hermes/factors/base.pyx":17
+  /* "hermes/factors/base.pyx":18
  * 
  *     @LazyFunc
  *     def long_type_str(self):             # <<<<<<<<<<<<<<
  *         """unique call"""
  *         return "long"
  */
-  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_13LongCallMixin_1long_type_str, 0, __pyx_n_s_LongCallMixin_long_type_str, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__3)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_13LongCallMixin_1long_type_str, 0, __pyx_n_s_LongCallMixin_long_type_str, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__4)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_4 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_7, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 16, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_long_type_str, __pyx_t_4) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_long_type_str, __pyx_t_4) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "hermes/factors/base.pyx":21
+  /* "hermes/factors/base.pyx":22
  *         return "long"
  * 
  *     @LazyFunc             # <<<<<<<<<<<<<<
  *     def expect_direction(self):
  *         """1.0"""
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_LazyFunc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_LazyFunc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 22, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
 
-  /* "hermes/factors/base.pyx":22
+  /* "hermes/factors/base.pyx":23
  * 
  *     @LazyFunc
  *     def expect_direction(self):             # <<<<<<<<<<<<<<
  *         """1.0"""
  *         return 1.0
  */
-  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_13LongCallMixin_3expect_direction, 0, __pyx_n_s_LongCallMixin_expect_direction, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 22, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_13LongCallMixin_3expect_direction, 0, __pyx_n_s_LongCallMixin_expect_direction, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_4 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_7, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 21, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 22, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_expect_direction, __pyx_t_4) < 0) __PYX_ERR(0, 22, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_expect_direction, __pyx_t_4) < 0) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "hermes/factors/base.pyx":11
+  /* "hermes/factors/base.pyx":12
  * 
  * 
  * class LongCallMixin(FreezeAttrMixin):             # <<<<<<<<<<<<<<
  *     """
  *         buy call
  */
-  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_LongCallMixin, __pyx_t_1, __pyx_t_3, NULL, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 11, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_LongCallMixin, __pyx_t_2, __pyx_t_3, NULL, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_LongCallMixin, __pyx_t_4) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_LongCallMixin, __pyx_t_4) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "hermes/factors/base.pyx":27
+  /* "hermes/factors/base.pyx":28
  * 
  * 
  * class ShortMixin(FreezeAttrMixin):             # <<<<<<<<<<<<<<
  *     """
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_FreezeAttrMixin); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 27, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 27, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_FreezeAttrMixin); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
-  __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 27, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_t_2, __pyx_n_s_ShortMixin, __pyx_n_s_ShortMixin, (PyObject *) NULL, __pyx_n_s_hermes_factors_base, __pyx_kp_s_buy_put); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 27, __pyx_L1_error)
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_2);
+  __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_1, __pyx_n_s_ShortMixin, __pyx_n_s_ShortMixin, (PyObject *) NULL, __pyx_n_s_hermes_factors_base, __pyx_kp_s_buy_put); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "hermes/factors/base.pyx":34
+  /* "hermes/factors/base.pyx":35
  *     """
  * 
  *     @LazyFunc             # <<<<<<<<<<<<<<
  *     def short_type_str(self):
  *         """unique put"""
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_LazyFunc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_LazyFunc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
 
-  /* "hermes/factors/base.pyx":35
+  /* "hermes/factors/base.pyx":36
  * 
  *     @LazyFunc
  *     def short_type_str(self):             # <<<<<<<<<<<<<<
  *         """unique put"""
  *         return "short"
  */
-  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10ShortMixin_1short_type_str, 0, __pyx_n_s_ShortMixin_short_type_str, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10ShortMixin_1short_type_str, 0, __pyx_n_s_ShortMixin_short_type_str, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_4 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_7, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 34, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_short_type_str, __pyx_t_4) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_short_type_str, __pyx_t_4) < 0) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "hermes/factors/base.pyx":39
+  /* "hermes/factors/base.pyx":40
  *         return "short"
  * 
  *     @LazyFunc             # <<<<<<<<<<<<<<
  *     def expect_direction(self):
  *         """1.0"""
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_LazyFunc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_LazyFunc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
 
-  /* "hermes/factors/base.pyx":40
+  /* "hermes/factors/base.pyx":41
  * 
  *     @LazyFunc
  *     def expect_direction(self):             # <<<<<<<<<<<<<<
  *         """1.0"""
  *         return -1.0
  */
-  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10ShortMixin_3expect_direction, 0, __pyx_n_s_ShortMixin_expect_direction, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10ShortMixin_3expect_direction, 0, __pyx_n_s_ShortMixin_expect_direction, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 41, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_4 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_7, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 39, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_expect_direction, __pyx_t_4) < 0) __PYX_ERR(0, 40, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_expect_direction, __pyx_t_4) < 0) __PYX_ERR(0, 41, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "hermes/factors/base.pyx":27
+  /* "hermes/factors/base.pyx":28
  * 
  * 
  * class ShortMixin(FreezeAttrMixin):             # <<<<<<<<<<<<<<
  *     """
  * 
  */
-  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_ShortMixin, __pyx_t_2, __pyx_t_3, NULL, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 27, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_ShortMixin, __pyx_t_1, __pyx_t_3, NULL, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ShortMixin, __pyx_t_4) < 0) __PYX_ERR(0, 27, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ShortMixin, __pyx_t_4) < 0) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "hermes/factors/base.pyx":46
  * 
  * 
  * class ShortMixin(FreezeAttrMixin):             # <<<<<<<<<<<<<<
  *     """
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_FreezeAttrMixin); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 46, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_FreezeAttrMixin); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GIVEREF(__pyx_t_2);
-  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_2);
-  __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_1, __pyx_n_s_ShortMixin, __pyx_n_s_ShortMixin, (PyObject *) NULL, __pyx_n_s_hermes_factors_base, __pyx_kp_s_buy_put); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
+  __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_t_2, __pyx_n_s_ShortMixin, __pyx_n_s_ShortMixin, (PyObject *) NULL, __pyx_n_s_hermes_factors_base, __pyx_kp_s_buy_put); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
   /* "hermes/factors/base.pyx":53
  *     """
  * 
  *     @LazyFunc             # <<<<<<<<<<<<<<
  *     def short_type_str(self):
@@ -4768,15 +5182,15 @@
   /* "hermes/factors/base.pyx":54
  * 
  *     @LazyFunc
  *     def short_type_str(self):             # <<<<<<<<<<<<<<
  *         """unique put"""
  *         return "short"
  */
-  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10ShortMixin_5short_type_str, 0, __pyx_n_s_ShortMixin_short_type_str, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 54, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10ShortMixin_5short_type_str, 0, __pyx_n_s_ShortMixin_short_type_str, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_7);
@@ -4806,15 +5220,15 @@
   /* "hermes/factors/base.pyx":59
  * 
  *     @LazyFunc
  *     def expect_direction(self):             # <<<<<<<<<<<<<<
  *         """1.0"""
  *         return -1.0
  */
-  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10ShortMixin_7expect_direction, 0, __pyx_n_s_ShortMixin_expect_direction, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 59, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10ShortMixin_7expect_direction, 0, __pyx_n_s_ShortMixin_expect_direction, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 59, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_7);
@@ -4834,39 +5248,39 @@
   /* "hermes/factors/base.pyx":46
  * 
  * 
  * class ShortMixin(FreezeAttrMixin):             # <<<<<<<<<<<<<<
  *     """
  * 
  */
-  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_ShortMixin, __pyx_t_1, __pyx_t_3, NULL, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_ShortMixin, __pyx_t_2, __pyx_t_3, NULL, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_ShortMixin, __pyx_t_4) < 0) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "hermes/factors/base.pyx":64
  * 
  * 
  * class ShortCallMixin(FreezeAttrMixin):             # <<<<<<<<<<<<<<
  *     """
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_FreezeAttrMixin); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_FreezeAttrMixin); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
-  __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_t_2, __pyx_n_s_ShortCallMixin, __pyx_n_s_ShortCallMixin, (PyObject *) NULL, __pyx_n_s_hermes_factors_base, __pyx_kp_s_buy_put); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_2);
+  __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_1, __pyx_n_s_ShortCallMixin, __pyx_n_s_ShortCallMixin, (PyObject *) NULL, __pyx_n_s_hermes_factors_base, __pyx_kp_s_buy_put); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
   /* "hermes/factors/base.pyx":71
  *     """
  * 
  *     @LazyFunc             # <<<<<<<<<<<<<<
  *     def short_type_str(self):
@@ -4878,15 +5292,15 @@
   /* "hermes/factors/base.pyx":72
  * 
  *     @LazyFunc
  *     def short_type_str(self):             # <<<<<<<<<<<<<<
  *         """unique put"""
  *         return "short"
  */
-  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_14ShortCallMixin_1short_type_str, 0, __pyx_n_s_ShortCallMixin_short_type_str, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_14ShortCallMixin_1short_type_str, 0, __pyx_n_s_ShortCallMixin_short_type_str, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_7);
@@ -4916,15 +5330,15 @@
   /* "hermes/factors/base.pyx":77
  * 
  *     @LazyFunc
  *     def expect_direction(self):             # <<<<<<<<<<<<<<
  *         """1.0"""
  *         return -1.0
  */
-  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_14ShortCallMixin_3expect_direction, 0, __pyx_n_s_ShortCallMixin_expect_direction, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_14ShortCallMixin_3expect_direction, 0, __pyx_n_s_ShortCallMixin_expect_direction, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 77, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_7);
@@ -4944,36 +5358,36 @@
   /* "hermes/factors/base.pyx":64
  * 
  * 
  * class ShortCallMixin(FreezeAttrMixin):             # <<<<<<<<<<<<<<
  *     """
  * 
  */
-  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_ShortCallMixin, __pyx_t_2, __pyx_t_3, NULL, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_ShortCallMixin, __pyx_t_1, __pyx_t_3, NULL, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_ShortCallMixin, __pyx_t_4) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "hermes/factors/base.pyx":82
  * 
  * 
  * class FactorBase(six.with_metaclass(ABCMeta, ParamBase)):             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self, **kwargs):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_six); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_with_metaclass); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_six); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_with_metaclass); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_ABCMeta); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_ABCMeta); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_ParamBase); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   __pyx_t_8 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_5)) {
@@ -4982,182 +5396,182 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_8 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_1, __pyx_t_4};
-    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 82, __pyx_L1_error)
+    PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_2, __pyx_t_4};
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_1, __pyx_t_4};
-    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 82, __pyx_L1_error)
+    PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_2, __pyx_t_4};
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else
   #endif
   {
     __pyx_t_6 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 82, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     if (__pyx_t_5) {
       __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_5); __pyx_t_5 = NULL;
     }
-    __Pyx_GIVEREF(__pyx_t_1);
-    PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_8, __pyx_t_1);
+    __Pyx_GIVEREF(__pyx_t_2);
+    PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_8, __pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_8, __pyx_t_4);
-    __pyx_t_1 = 0;
+    __pyx_t_2 = 0;
     __pyx_t_4 = 0;
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 82, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GIVEREF(__pyx_t_2);
-  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
-  __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 82, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_3, __pyx_n_s_FactorBase, __pyx_n_s_FactorBase, (PyObject *) NULL, __pyx_n_s_hermes_factors_base, (PyObject *) NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
+  __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_6 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_t_3, __pyx_n_s_FactorBase, __pyx_n_s_FactorBase, (PyObject *) NULL, __pyx_n_s_hermes_factors_base, (PyObject *) NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
 
   /* "hermes/factors/base.pyx":84
  * class FactorBase(six.with_metaclass(ABCMeta, ParamBase)):
  * 
  *     def __init__(self, **kwargs):             # <<<<<<<<<<<<<<
  *         #
  *         self._init_self(**kwargs)
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_1__init__, 0, __pyx_n_s_FactorBase___init, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_1__init__, 0, __pyx_n_s_FactorBase___init, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__20)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "hermes/factors/base.pyx":89
- * 
+  /* "hermes/factors/base.pyx":88
+ *         self._init_self(**kwargs)
  * 
  *     @abstractmethod             # <<<<<<<<<<<<<<
  *     def _init_self(self, **kwargs):
  *         """"""
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_abstractmethod); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 89, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_abstractmethod); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
 
-  /* "hermes/factors/base.pyx":90
+  /* "hermes/factors/base.pyx":89
  * 
  *     @abstractmethod
  *     def _init_self(self, **kwargs):             # <<<<<<<<<<<<<<
  *         """"""
  *         pass
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_3_init_self, 0, __pyx_n_s_FactorBase__init_self, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_3_init_self, 0, __pyx_n_s_FactorBase__init_self, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__22)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 89, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_7 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
-    __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_1);
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_7)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_1, function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
-  __pyx_t_4 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_7, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+  __pyx_t_4 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_7, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_5);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 89, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_init_self, __pyx_t_4) < 0) __PYX_ERR(0, 90, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_init_self, __pyx_t_4) < 0) __PYX_ERR(0, 89, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "hermes/factors/base.pyx":94
+  /* "hermes/factors/base.pyx":93
  *         pass
  * 
  *     def init_data(self, **kwargs):             # <<<<<<<<<<<<<<
  *         dependencies_list = self.get_dependencies()
  *         method = 'ddb' if 'method' not in kwargs else kwargs['method']
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_5init_data, 0, __pyx_n_s_FactorBase_init_data, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_5init_data, 0, __pyx_n_s_FactorBase_init_data, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__24)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_init_data, __pyx_t_4) < 0) __PYX_ERR(0, 94, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_init_data, __pyx_t_4) < 0) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "hermes/factors/base.pyx":105
- * 
+  /* "hermes/factors/base.pyx":108
+ *         return data
  * 
  *     def get_dependencies(self):             # <<<<<<<<<<<<<<
  *         dependencies_list = []
  *         member_func = self.factors_list()
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_7get_dependencies, 0, __pyx_n_s_FactorBase_get_dependencies, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__25)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_7get_dependencies, 0, __pyx_n_s_FactorBase_get_dependencies, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__26)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_get_dependencies, __pyx_t_4) < 0) __PYX_ERR(0, 105, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_get_dependencies, __pyx_t_4) < 0) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "hermes/factors/base.pyx":119
- * 
+ *         return list(set(dependencies_list))
  * 
  *     def _create_id(self, **kwargs):             # <<<<<<<<<<<<<<
  *         feature = copy.deepcopy(kwargs)
  *         feature['category'] = self.category
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_9_create_id, 0, __pyx_n_s_FactorBase__create_id, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__27)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_9_create_id, 0, __pyx_n_s_FactorBase__create_id, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__28)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 119, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_create_id_2, __pyx_t_4) < 0) __PYX_ERR(0, 119, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "hermes/factors/base.pyx":126
  *         return "{0}".format(create_id(original=s, digit=10))
  * 
  *     def _format(self, data, name, **kwargs):             # <<<<<<<<<<<<<<
- *         #0 matrix  1 serise  2 DatFrame
- *         data_format = 1 if not hasattr(self,'_data_format') else self._data_format
+ *         # 0 matrix  1 serise  2 DatFrame
+ *         data = data.sort_values(by=['trade_date'])
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_11_format, 0, __pyx_n_s_FactorBase__format, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__29)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 126, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_11_format, 0, __pyx_n_s_FactorBase__format, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__30)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 126, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_format_2, __pyx_t_4) < 0) __PYX_ERR(0, 126, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "hermes/factors/base.pyx":140
+  /* "hermes/factors/base.pyx":144
  *         return data
  * 
  *     def factors_list(self):             # <<<<<<<<<<<<<<
  *         return list(
  *             filter(
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_13factors_list, 0, __pyx_n_s_FactorBase_factors_list, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__31)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 140, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6hermes_7factors_4base_10FactorBase_13factors_list, 0, __pyx_n_s_FactorBase_factors_list, NULL, __pyx_n_s_hermes_factors_base, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_factors_list, __pyx_t_4) < 0) __PYX_ERR(0, 140, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_factors_list, __pyx_t_4) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "hermes/factors/base.pyx":82
  * 
  * 
  * class FactorBase(six.with_metaclass(ABCMeta, ParamBase)):             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self, **kwargs):
  */
-  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_FactorBase, __pyx_t_3, __pyx_t_6, NULL, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_FactorBase, __pyx_t_3, __pyx_t_6, NULL, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_FactorBase, __pyx_t_4) < 0) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "hermes/factors/base.pyx":1
  * # -*- encoding:utf-8 -*-             # <<<<<<<<<<<<<<
  * import copy, hashlib, json, inspect, pdb
  * import six as six
  */
@@ -5648,14 +6062,28 @@
         return NULL;
     }
     Py_INCREF(value);
     return value;
 }
 #endif
 
+/* PyObjectSetAttrStr */
+#if CYTHON_USE_TYPE_SLOTS
+static CYTHON_INLINE int __Pyx_PyObject_SetAttrStr(PyObject* obj, PyObject* attr_name, PyObject* value) {
+    PyTypeObject* tp = Py_TYPE(obj);
+    if (likely(tp->tp_setattro))
+        return tp->tp_setattro(obj, attr_name, value);
+#if PY_MAJOR_VERSION < 3
+    if (likely(tp->tp_setattr))
+        return tp->tp_setattr(obj, PyString_AS_STRING(attr_name), value);
+#endif
+    return PyObject_SetAttr(obj, attr_name, value);
+}
+#endif
+
 /* PyDictVersioning */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
     PyObject *dict = Py_TYPE(obj)->tp_dict;
     return likely(dict) ? __PYX_GET_DICT_VERSION(dict) : 0;
 }
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_object_dict_version(PyObject *obj) {
@@ -5709,27 +6137,14 @@
         return __Pyx_NewRef(result);
     }
     PyErr_Clear();
 #endif
     return __Pyx_GetBuiltinName(name);
 }
 
-/* GetAttr */
-static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *o, PyObject *n) {
-#if CYTHON_USE_TYPE_SLOTS
-#if PY_MAJOR_VERSION >= 3
-    if (likely(PyUnicode_Check(n)))
-#else
-    if (likely(PyString_Check(n)))
-#endif
-        return __Pyx_PyObject_GetAttrStr(o, n);
-#endif
-    return PyObject_GetAttr(o, n);
-}
-
 /* PyObjectCall2Args */
 static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
     PyObject *args, *result = NULL;
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(function)) {
         PyObject *args[2] = {arg1, arg2};
         return __Pyx_PyFunction_FastCall(function, args, 2);
@@ -5751,14 +6166,124 @@
     result = __Pyx_PyObject_Call(function, args, NULL);
     Py_DECREF(args);
     Py_DECREF(function);
 done:
     return result;
 }
 
+/* GetAttr */
+static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *o, PyObject *n) {
+#if CYTHON_USE_TYPE_SLOTS
+#if PY_MAJOR_VERSION >= 3
+    if (likely(PyUnicode_Check(n)))
+#else
+    if (likely(PyString_Check(n)))
+#endif
+        return __Pyx_PyObject_GetAttrStr(o, n);
+#endif
+    return PyObject_GetAttr(o, n);
+}
+
+/* SliceObject */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetSlice(PyObject* obj,
+        Py_ssize_t cstart, Py_ssize_t cstop,
+        PyObject** _py_start, PyObject** _py_stop, PyObject** _py_slice,
+        int has_cstart, int has_cstop, CYTHON_UNUSED int wraparound) {
+#if CYTHON_USE_TYPE_SLOTS
+    PyMappingMethods* mp;
+#if PY_MAJOR_VERSION < 3
+    PySequenceMethods* ms = Py_TYPE(obj)->tp_as_sequence;
+    if (likely(ms && ms->sq_slice)) {
+        if (!has_cstart) {
+            if (_py_start && (*_py_start != Py_None)) {
+                cstart = __Pyx_PyIndex_AsSsize_t(*_py_start);
+                if ((cstart == (Py_ssize_t)-1) && PyErr_Occurred()) goto bad;
+            } else
+                cstart = 0;
+        }
+        if (!has_cstop) {
+            if (_py_stop && (*_py_stop != Py_None)) {
+                cstop = __Pyx_PyIndex_AsSsize_t(*_py_stop);
+                if ((cstop == (Py_ssize_t)-1) && PyErr_Occurred()) goto bad;
+            } else
+                cstop = PY_SSIZE_T_MAX;
+        }
+        if (wraparound && unlikely((cstart < 0) | (cstop < 0)) && likely(ms->sq_length)) {
+            Py_ssize_t l = ms->sq_length(obj);
+            if (likely(l >= 0)) {
+                if (cstop < 0) {
+                    cstop += l;
+                    if (cstop < 0) cstop = 0;
+                }
+                if (cstart < 0) {
+                    cstart += l;
+                    if (cstart < 0) cstart = 0;
+                }
+            } else {
+                if (!PyErr_ExceptionMatches(PyExc_OverflowError))
+                    goto bad;
+                PyErr_Clear();
+            }
+        }
+        return ms->sq_slice(obj, cstart, cstop);
+    }
+#endif
+    mp = Py_TYPE(obj)->tp_as_mapping;
+    if (likely(mp && mp->mp_subscript))
+#endif
+    {
+        PyObject* result;
+        PyObject *py_slice, *py_start, *py_stop;
+        if (_py_slice) {
+            py_slice = *_py_slice;
+        } else {
+            PyObject* owned_start = NULL;
+            PyObject* owned_stop = NULL;
+            if (_py_start) {
+                py_start = *_py_start;
+            } else {
+                if (has_cstart) {
+                    owned_start = py_start = PyInt_FromSsize_t(cstart);
+                    if (unlikely(!py_start)) goto bad;
+                } else
+                    py_start = Py_None;
+            }
+            if (_py_stop) {
+                py_stop = *_py_stop;
+            } else {
+                if (has_cstop) {
+                    owned_stop = py_stop = PyInt_FromSsize_t(cstop);
+                    if (unlikely(!py_stop)) {
+                        Py_XDECREF(owned_start);
+                        goto bad;
+                    }
+                } else
+                    py_stop = Py_None;
+            }
+            py_slice = PySlice_New(py_start, py_stop, Py_None);
+            Py_XDECREF(owned_start);
+            Py_XDECREF(owned_stop);
+            if (unlikely(!py_slice)) goto bad;
+        }
+#if CYTHON_USE_TYPE_SLOTS
+        result = mp->mp_subscript(obj, py_slice);
+#else
+        result = PyObject_GetItem(obj, py_slice);
+#endif
+        if (!_py_slice) {
+            Py_DECREF(py_slice);
+        }
+        return result;
+    }
+    PyErr_Format(PyExc_TypeError,
+        "'%.200s' object is unsliceable", Py_TYPE(obj)->tp_name);
+bad:
+    return NULL;
+}
+
 /* HasAttr */
 static CYTHON_INLINE int __Pyx_HasAttr(PyObject *o, PyObject *n) {
     PyObject *r;
     if (unlikely(!__Pyx_PyBaseString_Check(n))) {
         PyErr_SetString(PyExc_TypeError,
                         "hasattr(): attribute name must be string");
         return -1;
@@ -5836,28 +6361,14 @@
         double a = PyFloat_AS_DOUBLE(op1);
         if ((double)a == (double)b) Py_RETURN_TRUE; else Py_RETURN_FALSE;
     }
     return (
         PyObject_RichCompare(op1, op2, Py_EQ));
 }
 
-/* PyObjectSetAttrStr */
-#if CYTHON_USE_TYPE_SLOTS
-static CYTHON_INLINE int __Pyx_PyObject_SetAttrStr(PyObject* obj, PyObject* attr_name, PyObject* value) {
-    PyTypeObject* tp = Py_TYPE(obj);
-    if (likely(tp->tp_setattro))
-        return tp->tp_setattro(obj, attr_name, value);
-#if PY_MAJOR_VERSION < 3
-    if (likely(tp->tp_setattr))
-        return tp->tp_setattr(obj, PyString_AS_STRING(attr_name), value);
-#endif
-    return PyObject_SetAttr(obj, attr_name, value);
-}
-#endif
-
 /* IterFinish */
 static CYTHON_INLINE int __Pyx_IterFinish(void) {
 #if CYTHON_FAST_THREAD_STATE
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
     PyObject* exc_type = tstate->curexc_type;
     if (unlikely(exc_type)) {
         if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) {
@@ -7958,14 +8469,20 @@
     if (likely(PyExceptionClass_Check(err))) {
         return __Pyx_inner_PyErr_GivenExceptionMatches2(err, exc_type1, exc_type2);
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
+/* CStringEquals */
+static CYTHON_INLINE int __Pyx_StrEq(const char *s1, const char *s2) {
+    while (*s1 != '\0' && *s1 == *s2) { s1++; s2++; }
+    return *s1 == *s2;
+}
+
 /* CheckBinaryVersion */
 static int __Pyx_check_binary_version(void) {
     char ctversion[4], rtversion[4];
     PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
     PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
     if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
         char message[200];
```

### Comparing `Finance-Hermes-0.3.0/hermes/factors/base.pyx` & `Finance-Hermes-0.3.1/hermes/factors/base.pyx`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- encoding:utf-8 -*-
 import copy, hashlib, json, inspect, pdb
 import six as six
 from abc import ABCMeta, abstractmethod
 from jdwdata.RetrievalAPI import get_data_by_map
+from jdwdate.api import *
 from hermes.kdutils.create_id import create_id
 from hermes.kdutils.lazy import LazyFunc
 from hermes.kdutils.base import ParamBase, FreezeAttrMixin
 
 
 class LongCallMixin(FreezeAttrMixin):
     """
@@ -38,15 +39,14 @@
 
     @LazyFunc
     def expect_direction(self):
         """期望收益方向，1.0即反向期望"""
         return -1.0
 
 
-
 class ShortMixin(FreezeAttrMixin):
     """
         混入类，混入代表空头，应用场景在于期权，期货策略中，
         不完全是期权中buy put的概念，只代看跌反向操作，
         即期望买入后交易目标价格下跌，下跌带来收益
     """
 
@@ -55,15 +55,15 @@
         """用来区别买入类型unique 值为put"""
         return "short"
 
     @LazyFunc
     def expect_direction(self):
         """期望收益方向，1.0即反向期望"""
         return -1.0
-    
+
 
 class ShortCallMixin(FreezeAttrMixin):
     """
         混入类，混入代表空头，应用场景在于期权，期货策略中，
         不完全是期权中buy put的概念，只代看跌反向操作，
         即期望买入后交易目标价格下跌，下跌带来收益
     """
@@ -80,65 +80,69 @@
 
 
 class FactorBase(six.with_metaclass(ABCMeta, ParamBase)):
 
     def __init__(self, **kwargs):
         # 子类继续完成自有的构造
         self._init_self(**kwargs)
-        
 
     @abstractmethod
     def _init_self(self, **kwargs):
         """子类因子针对可扩展参数的初始化"""
         pass
 
     def init_data(self, **kwargs):
         dependencies_list = self.get_dependencies()
         method = 'ddb' if 'method' not in kwargs else kwargs['method']
+        self.begin_date = kwargs['begin_date']
+        self.end_date = kwargs['end_date']
+        window = 0 if 'window' not in kwargs else int(kwargs['window'])
+        start_date = advanceDateByCalendar(
+            'china.sse', self.begin_date,
+            '-{0}b'.format(window)).strftime('%Y-%m-%d')
         data = get_data_by_map(columns=dependencies_list,
-                      begin_date=kwargs['begin_date'],
-                      end_date=kwargs['end_date'],
-                      method=method)
+                               begin_date=start_date,
+                               end_date=self.end_date,
+                               method=method)
         return data
 
-
-    
     def get_dependencies(self):
         dependencies_list = []
         member_func = self.factors_list()
         for func in member_func:
             func_module = getattr(self, func)
             fun_param = inspect.signature(func_module).parameters
             if 'dependencies' in fun_param:
                 dependencies = fun_param['dependencies'].default
                 dependencies_list += dependencies
         return list(set(dependencies_list))
 
-
-
-
     def _create_id(self, **kwargs):
         feature = copy.deepcopy(kwargs)
         feature['category'] = self.category
         s = hashlib.md5(
             json.dumps(feature).encode(encoding="utf-8")).hexdigest()
         return "{0}".format(create_id(original=s, digit=10))
 
     def _format(self, data, name, **kwargs):
-        #0 matrix  1 serise  2 DatFrame
-        data_format = 1 if not hasattr(self,'_data_format') else self._data_format
+        # 0 matrix  1 serise  2 DatFrame
+        data = data.sort_values(by=['trade_date'])
+        data = data.loc[self.begin_date:self.end_date]
+        data_format = 1 if not hasattr(self,
+                                       '_data_format') else self._data_format
+
         if data_format == 1 or data_format == 2:
             data = data.stack()
             if data_format == 2:
                 data.name = 'value'
                 data = data.reset_index()
                 data['name'] = name
         data.name = name
         data.category = self.category
         data.id = self._create_id(name=name, **kwargs)
         return data
 
     def factors_list(self):
         return list(
             filter(
-                lambda x: not x.startswith('_')  and
-                callable(getattr(self, x)), dir(self)))
+                lambda x: not x.startswith('_') and callable(getattr(self, x)),
+                dir(self)))
```

### Comparing `Finance-Hermes-0.3.0/hermes/factors/test/factor_test.c` & `Finance-Hermes-0.3.1/hermes/factors/test/factor_test.c`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.3.0/hermes/factors/test/factor_test.pyx` & `Finance-Hermes-0.3.1/hermes/factors/test/factor_test.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.3.0/hermes/kdutils/base.c` & `Finance-Hermes-0.3.1/hermes/kdutils/base.c`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.3.0/hermes/kdutils/base.pyx` & `Finance-Hermes-0.3.1/hermes/kdutils/base.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.3.0/hermes/kdutils/core/fixes.c` & `Finance-Hermes-0.3.1/hermes/kdutils/core/fixes.c`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.3.0/hermes/kdutils/core/fixes.pyx` & `Finance-Hermes-0.3.1/hermes/kdutils/core/fixes.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.3.0/hermes/kdutils/core/helper.c` & `Finance-Hermes-0.3.1/hermes/kdutils/core/helper.c`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.3.0/hermes/kdutils/core/helper.pyx` & `Finance-Hermes-0.3.1/hermes/kdutils/core/helper.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.3.0/hermes/kdutils/create_id.c` & `Finance-Hermes-0.3.1/hermes/kdutils/create_id.c`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.3.0/hermes/kdutils/create_id.pyx` & `Finance-Hermes-0.3.1/hermes/kdutils/create_id.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.3.0/hermes/kdutils/lazy.c` & `Finance-Hermes-0.3.1/hermes/kdutils/lazy.c`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.3.0/hermes/kdutils/lazy.pyx` & `Finance-Hermes-0.3.1/hermes/kdutils/lazy.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.3.0/hermes/lzador/calculater.c` & `Finance-Hermes-0.3.1/hermes/lzador/calculater.c`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.3.0/hermes/lzador/calculater.pyx` & `Finance-Hermes-0.3.1/hermes/lzador/calculater.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.3.0/setup.py` & `Finance-Hermes-0.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,21 +19,23 @@
 
 def git_version():
     from subprocess import Popen, PIPE
     gitproc = Popen(['git', 'rev-parse', 'HEAD'], stdout=PIPE)
     (stdout, _) = gitproc.communicate()
     return stdout.strip()
 
+
 if "--line_trace" in sys.argv:
     line_trace = True
     print("Build with line trace enabled ...")
     sys.argv.remove("--line_trace")
 else:
     line_trace = False
 
+
 class version_build(Command):
 
     description = "test the distribution prior to install"
 
     user_options = [
         ('test-dir=', None, "directory that contains the test definitions"),
     ]
@@ -66,19 +68,22 @@
 requirements = "requirements/py3.txt"
 
 if platform.system() != "Windows":
     import multiprocessing
     n_cpu = multiprocessing.cpu_count()
 else:
     n_cpu = 0
-    
 
+ext_modules = [
+    'hermes/kdutils/core/fixes.pyx', 'hermes/kdutils/core/helper.pyx',
+    'hermes/factors/base.pyx', 'hermes/kdutils/base.pyx',
+    'hermes/kdutils/create_id.pyx', 'hermes/kdutils/lazy.pyx',
+    'hermes/lzador/calculater.pyx', 'hermes/factors/test/factor_test.pyx'
+]
 
-ext_modules = ['hermes/kdutils/core/fixes.pyx','hermes/kdutils/core/helper.pyx','hermes/factors/base.pyx', 'hermes/kdutils/base.pyx','hermes/kdutils/create_id.pyx','hermes/kdutils/lazy.pyx',
-               'hermes/lzador/calculater.pyx','hermes/factors/test/factor_test.pyx']
 
 def generate_extensions(ext_modules, line_trace=True):
 
     extensions = []
 
     if line_trace:
         print("define cython trace to True ...")
@@ -89,14 +94,15 @@
     for pyxfile in ext_modules:
         ext = Extension(name='.'.join(pyxfile.split('/'))[:-4],
                         sources=[pyxfile],
                         define_macros=define_macros)
         extensions.append(ext)
     return extensions
 
+
 ext_modules_settings = cythonize(generate_extensions(ext_modules, line_trace),
                                  compiler_directives={
                                      'embedsignature': True,
                                      'linetrace': line_trace
                                  },
                                  nthreads=n_cpu)
```

