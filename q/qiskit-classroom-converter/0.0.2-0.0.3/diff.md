# Comparing `tmp/qiskit-classroom-converter-0.0.2.tar.gz` & `tmp/qiskit-classroom-converter-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-classroom-converter-0.0.2.tar", last modified: Sun Jul 30 00:20:44 2023, max compression
+gzip compressed data, was "qiskit-classroom-converter-0.0.3.tar", last modified: Mon Jul 31 10:46:27 2023, max compression
```

## Comparing `qiskit-classroom-converter-0.0.2.tar` & `qiskit-classroom-converter-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,26 @@
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-07-30 00:20:44.058942 qiskit-classroom-converter-0.0.2/
--rw-r--r--   0 minwook-shin   (501) staff       (20)    11350 2023-07-28 05:38:56.000000 qiskit-classroom-converter-0.0.2/LICENSE
--rw-r--r--   0 minwook-shin   (501) staff       (20)       24 2023-06-25 02:07:36.000000 qiskit-classroom-converter-0.0.2/MANIFEST.in
--rw-r--r--   0 minwook-shin   (501) staff       (20)     2565 2023-07-30 00:20:44.059136 qiskit-classroom-converter-0.0.2/PKG-INFO
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1958 2023-07-28 06:54:58.000000 qiskit-classroom-converter-0.0.2/README.md
--rw-r--r--   0 minwook-shin   (501) staff       (20)      951 2023-07-30 00:19:08.000000 qiskit-classroom-converter-0.0.2/pyproject.toml
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-07-30 00:20:44.048997 qiskit-classroom-converter-0.0.2/qiskit_class_converter/
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1653 2023-07-28 06:43:21.000000 qiskit-classroom-converter-0.0.2/qiskit_class_converter/__init__.py
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-07-30 00:20:44.053207 qiskit-classroom-converter-0.0.2/qiskit_class_converter/converters/
--rw-r--r--   0 minwook-shin   (501) staff       (20)        0 2023-05-26 12:59:36.000000 qiskit-classroom-converter-0.0.2/qiskit_class_converter/converters/__init__.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1629 2023-07-28 05:38:56.000000 qiskit-classroom-converter-0.0.2/qiskit_class_converter/converters/base.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     3710 2023-07-28 05:39:05.000000 qiskit-classroom-converter-0.0.2/qiskit_class_converter/converters/braket_notation_to_matrix.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1409 2023-07-28 06:43:21.000000 qiskit-classroom-converter-0.0.2/qiskit_class_converter/converters/matrix_to_quantum_circuit.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     2440 2023-07-28 05:38:56.000000 qiskit-classroom-converter-0.0.2/qiskit_class_converter/converters/quantum_circuit_to_braket_notation.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1526 2023-07-28 05:38:56.000000 qiskit-classroom-converter-0.0.2/qiskit_class_converter/converters/quantum_circuit_to_matrix.py
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-07-30 00:20:44.054452 qiskit-classroom-converter-0.0.2/qiskit_class_converter/services/
--rw-r--r--   0 minwook-shin   (501) staff       (20)        0 2023-05-26 12:59:36.000000 qiskit-classroom-converter-0.0.2/qiskit_class_converter/services/__init__.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     4310 2023-07-28 06:43:21.000000 qiskit-classroom-converter-0.0.2/qiskit_class_converter/services/converter_service.py
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-07-30 00:20:44.057050 qiskit-classroom-converter-0.0.2/qiskit_classroom_converter.egg-info/
--rw-r--r--   0 minwook-shin   (501) staff       (20)     2565 2023-07-30 00:20:44.000000 qiskit-classroom-converter-0.0.2/qiskit_classroom_converter.egg-info/PKG-INFO
--rw-r--r--   0 minwook-shin   (501) staff       (20)      861 2023-07-30 00:20:44.000000 qiskit-classroom-converter-0.0.2/qiskit_classroom_converter.egg-info/SOURCES.txt
--rw-r--r--   0 minwook-shin   (501) staff       (20)        1 2023-07-30 00:20:44.000000 qiskit-classroom-converter-0.0.2/qiskit_classroom_converter.egg-info/dependency_links.txt
--rw-r--r--   0 minwook-shin   (501) staff       (20)      165 2023-07-30 00:20:44.000000 qiskit-classroom-converter-0.0.2/qiskit_classroom_converter.egg-info/requires.txt
--rw-r--r--   0 minwook-shin   (501) staff       (20)       23 2023-07-30 00:20:44.000000 qiskit-classroom-converter-0.0.2/qiskit_classroom_converter.egg-info/top_level.txt
--rw-r--r--   0 minwook-shin   (501) staff       (20)       88 2023-07-30 00:19:08.000000 qiskit-classroom-converter-0.0.2/requirements.txt
--rw-r--r--   0 minwook-shin   (501) staff       (20)       79 2023-07-30 00:20:44.059740 qiskit-classroom-converter-0.0.2/setup.cfg
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-07-30 00:20:44.058252 qiskit-classroom-converter-0.0.2/tests/
--rw-r--r--   0 minwook-shin   (501) staff       (20)     3813 2023-07-28 06:43:21.000000 qiskit-classroom-converter-0.0.2/tests/test_convert_class.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     5698 2023-07-28 06:03:19.000000 qiskit-classroom-converter-0.0.2/tests/test_converter_service.py
+drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-07-31 10:46:27.009857 qiskit-classroom-converter-0.0.3/
+-rw-r--r--   0 minwook-shin   (501) staff       (20)    11350 2023-07-28 05:38:56.000000 qiskit-classroom-converter-0.0.3/LICENSE
+-rw-r--r--   0 minwook-shin   (501) staff       (20)       36 2023-07-31 10:43:34.000000 qiskit-classroom-converter-0.0.3/MANIFEST.in
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     2565 2023-07-31 10:46:27.010008 qiskit-classroom-converter-0.0.3/PKG-INFO
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     1958 2023-07-28 06:54:58.000000 qiskit-classroom-converter-0.0.3/README.md
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     1188 2023-07-31 10:43:34.000000 qiskit-classroom-converter-0.0.3/pyproject.toml
+drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-07-31 10:46:27.002976 qiskit-classroom-converter-0.0.3/qiskit_class_converter/
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     1653 2023-07-28 06:43:21.000000 qiskit-classroom-converter-0.0.3/qiskit_class_converter/__init__.py
+drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-07-31 10:46:27.006780 qiskit-classroom-converter-0.0.3/qiskit_class_converter/converters/
+-rw-r--r--   0 minwook-shin   (501) staff       (20)        0 2023-05-26 12:59:36.000000 qiskit-classroom-converter-0.0.3/qiskit_class_converter/converters/__init__.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     1629 2023-07-28 05:38:56.000000 qiskit-classroom-converter-0.0.3/qiskit_class_converter/converters/base.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     3710 2023-07-28 05:39:05.000000 qiskit-classroom-converter-0.0.3/qiskit_class_converter/converters/braket_notation_to_matrix.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     1409 2023-07-28 06:43:21.000000 qiskit-classroom-converter-0.0.3/qiskit_class_converter/converters/matrix_to_quantum_circuit.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     2440 2023-07-28 05:38:56.000000 qiskit-classroom-converter-0.0.3/qiskit_class_converter/converters/quantum_circuit_to_braket_notation.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     1526 2023-07-28 05:38:56.000000 qiskit-classroom-converter-0.0.3/qiskit_class_converter/converters/quantum_circuit_to_matrix.py
+drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-07-31 10:46:27.007692 qiskit-classroom-converter-0.0.3/qiskit_class_converter/services/
+-rw-r--r--   0 minwook-shin   (501) staff       (20)        0 2023-05-26 12:59:36.000000 qiskit-classroom-converter-0.0.3/qiskit_class_converter/services/__init__.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     4310 2023-07-28 06:43:21.000000 qiskit-classroom-converter-0.0.3/qiskit_class_converter/services/converter_service.py
+drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-07-31 10:46:27.009588 qiskit-classroom-converter-0.0.3/qiskit_classroom_converter.egg-info/
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     2565 2023-07-31 10:46:26.000000 qiskit-classroom-converter-0.0.3/qiskit_classroom_converter.egg-info/PKG-INFO
+-rw-r--r--   0 minwook-shin   (501) staff       (20)      801 2023-07-31 10:46:26.000000 qiskit-classroom-converter-0.0.3/qiskit_classroom_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 minwook-shin   (501) staff       (20)        1 2023-07-31 10:46:26.000000 qiskit-classroom-converter-0.0.3/qiskit_classroom_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 minwook-shin   (501) staff       (20)      165 2023-07-31 10:46:26.000000 qiskit-classroom-converter-0.0.3/qiskit_classroom_converter.egg-info/requires.txt
+-rw-r--r--   0 minwook-shin   (501) staff       (20)       23 2023-07-31 10:46:26.000000 qiskit-classroom-converter-0.0.3/qiskit_classroom_converter.egg-info/top_level.txt
+-rw-r--r--   0 minwook-shin   (501) staff       (20)       88 2023-07-30 00:19:08.000000 qiskit-classroom-converter-0.0.3/requirements.txt
+-rw-r--r--   0 minwook-shin   (501) staff       (20)       79 2023-07-31 10:46:27.010441 qiskit-classroom-converter-0.0.3/setup.cfg
```

### Comparing `qiskit-classroom-converter-0.0.2/LICENSE` & `qiskit-classroom-converter-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.0.2/PKG-INFO` & `qiskit-classroom-converter-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-classroom-converter
-Version: 0.0.2
+Version: 0.0.3
 Summary: extend the Qiskit classroom applications.
 Author: KMU-quantum-classroom
 Project-URL: Homepage, https://github.com/KMU-quantum-classroom/qiskit-classroom-converter
 Project-URL: Bug Tracker, https://github.com/KMU-quantum-classroom/qiskit-classroom-converter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `qiskit-classroom-converter-0.0.2/README.md` & `qiskit-classroom-converter-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.0.2/qiskit_class_converter/__init__.py` & `qiskit-classroom-converter-0.0.3/qiskit_class_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.0.2/qiskit_class_converter/converters/base.py` & `qiskit-classroom-converter-0.0.3/qiskit_class_converter/converters/base.py`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.0.2/qiskit_class_converter/converters/braket_notation_to_matrix.py` & `qiskit-classroom-converter-0.0.3/qiskit_class_converter/converters/braket_notation_to_matrix.py`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.0.2/qiskit_class_converter/converters/matrix_to_quantum_circuit.py` & `qiskit-classroom-converter-0.0.3/qiskit_class_converter/converters/matrix_to_quantum_circuit.py`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.0.2/qiskit_class_converter/converters/quantum_circuit_to_braket_notation.py` & `qiskit-classroom-converter-0.0.3/qiskit_class_converter/converters/quantum_circuit_to_braket_notation.py`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.0.2/qiskit_class_converter/converters/quantum_circuit_to_matrix.py` & `qiskit-classroom-converter-0.0.3/qiskit_class_converter/converters/quantum_circuit_to_matrix.py`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.0.2/qiskit_class_converter/services/converter_service.py` & `qiskit-classroom-converter-0.0.3/qiskit_class_converter/services/converter_service.py`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.0.2/qiskit_classroom_converter.egg-info/PKG-INFO` & `qiskit-classroom-converter-0.0.3/qiskit_classroom_converter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-classroom-converter
-Version: 0.0.2
+Version: 0.0.3
 Summary: extend the Qiskit classroom applications.
 Author: KMU-quantum-classroom
 Project-URL: Homepage, https://github.com/KMU-quantum-classroom/qiskit-classroom-converter
 Project-URL: Bug Tracker, https://github.com/KMU-quantum-classroom/qiskit-classroom-converter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `qiskit-classroom-converter-0.0.2/qiskit_classroom_converter.egg-info/SOURCES.txt` & `qiskit-classroom-converter-0.0.3/qiskit_classroom_converter.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -13,10 +13,8 @@
 qiskit_class_converter/converters/quantum_circuit_to_matrix.py
 qiskit_class_converter/services/__init__.py
 qiskit_class_converter/services/converter_service.py
 qiskit_classroom_converter.egg-info/PKG-INFO
 qiskit_classroom_converter.egg-info/SOURCES.txt
 qiskit_classroom_converter.egg-info/dependency_links.txt
 qiskit_classroom_converter.egg-info/requires.txt
-qiskit_classroom_converter.egg-info/top_level.txt
-tests/test_convert_class.py
-tests/test_converter_service.py
+qiskit_classroom_converter.egg-info/top_level.txt
```

