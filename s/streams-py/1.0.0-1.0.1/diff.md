# Comparing `tmp/streams_py-1.0.0.tar.gz` & `tmp/streams_py-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streams_py-1.0.0.tar", max compression
+gzip compressed data, was "streams_py-1.0.1.tar", max compression
```

## Comparing `streams_py-1.0.0.tar` & `streams_py-1.0.1.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0    35149 2023-07-25 15:31:42.633015 streams_py-1.0.0/LICENSE
--rw-r--r--   0        0        0    11424 2023-07-25 15:31:42.633015 streams_py-1.0.0/README.md
--rw-r--r--   0        0        0      733 2023-07-25 15:31:42.637014 streams_py-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      157 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/__init__.py
--rw-r--r--   0        0        0      336 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/__iterate.py
--rw-r--r--   0        0        0     3910 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/__optional.py
--rw-r--r--   0        0        0     3483 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/__stream.py
--rw-r--r--   0        0        0     1654 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/__stream_converter.py
--rw-r--r--   0        0        0        0 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/_itertools/__init__.py
--rw-r--r--   0        0        0     1713 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/_itertools/tools.py
--rw-r--r--   0        0        0        0 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/_lazy/__init__.py
--rw-r--r--   0        0        0      626 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/_lazy/process.py
--rw-r--r--   0        0        0      593 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/_lazy/queue.py
--rw-r--r--   0        0        0        0 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/_parallel/__init__.py
--rw-r--r--   0        0        0     3885 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/_parallel/fork_and_join.py
--rw-r--r--   0        0        0      787 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/_parallel/parallelizer.py
--rw-r--r--   0        0        0    16037 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/_streams/__base_stream.py
--rw-r--r--   0        0        0        0 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/_streams/__init__.py
--rw-r--r--   0        0        0     3380 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/_streams/__parallel_stream.py
--rw-r--r--   0        0        0     2227 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/_streams/__sequential_stream.py
--rw-r--r--   0        0        0     3062 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/_streams/error/__error.py
--rw-r--r--   0        0        0      258 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/_streams/error/__levels.py
--rw-r--r--   0        0        0      307 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/_streams/error/__sentinel.py
--rw-r--r--   0        0        0     3595 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/_streams/numeric/__numeric_base_stream.py
--rw-r--r--   0        0        0      861 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/_streams/numeric/__parallel_numeric_stream.py
--rw-r--r--   0        0        0      686 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/_streams/numeric/__sequential_numeric_stream.py
--rw-r--r--   0        0        0      221 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/conditions/__init__.py
--rw-r--r--   0        0        0      307 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/conditions/combiners.py
--rw-r--r--   0        0        0    10878 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/conditions/date.py
--rw-r--r--   0        0        0     4937 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/conditions/numeric.py
--rw-r--r--   0        0        0     1385 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/conditions/string.py
--rw-r--r--   0        0        0      735 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/conditions/types.py
--rw-r--r--   0        0        0     1688 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/loaders/__csv_loader.py
--rw-r--r--   0        0        0       74 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/loaders/__init__.py
--rw-r--r--   0        0        0    12279 1970-01-01 00:00:00.000000 streams_py-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-31 13:58:43.081161 streams_py-1.0.1/LICENSE
+-rw-r--r--   0        0        0    11514 2023-07-31 13:58:43.081161 streams_py-1.0.1/README.md
+-rw-r--r--   0        0        0      733 2023-07-31 13:58:43.081161 streams_py-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      157 2023-07-31 13:58:43.081161 streams_py-1.0.1/pystreamapi/__init__.py
+-rw-r--r--   0        0        0      336 2023-07-31 13:58:43.081161 streams_py-1.0.1/pystreamapi/__iterate.py
+-rw-r--r--   0        0        0     3910 2023-07-31 13:58:43.081161 streams_py-1.0.1/pystreamapi/__optional.py
+-rw-r--r--   0        0        0     3483 2023-07-31 13:58:43.081161 streams_py-1.0.1/pystreamapi/__stream.py
+-rw-r--r--   0        0        0     1654 2023-07-31 13:58:43.081161 streams_py-1.0.1/pystreamapi/__stream_converter.py
+-rw-r--r--   0        0        0        0 2023-07-31 13:58:43.085162 streams_py-1.0.1/pystreamapi/_itertools/__init__.py
+-rw-r--r--   0        0        0     1713 2023-07-31 13:58:43.085162 streams_py-1.0.1/pystreamapi/_itertools/tools.py
+-rw-r--r--   0        0        0        0 2023-07-31 13:58:43.085162 streams_py-1.0.1/pystreamapi/_lazy/__init__.py
+-rw-r--r--   0        0        0      626 2023-07-31 13:58:43.085162 streams_py-1.0.1/pystreamapi/_lazy/process.py
+-rw-r--r--   0        0        0      593 2023-07-31 13:58:43.085162 streams_py-1.0.1/pystreamapi/_lazy/queue.py
+-rw-r--r--   0        0        0        0 2023-07-31 13:58:43.085162 streams_py-1.0.1/pystreamapi/_parallel/__init__.py
+-rw-r--r--   0        0        0     3885 2023-07-31 13:58:43.085162 streams_py-1.0.1/pystreamapi/_parallel/fork_and_join.py
+-rw-r--r--   0        0        0      787 2023-07-31 13:58:43.085162 streams_py-1.0.1/pystreamapi/_parallel/parallelizer.py
+-rw-r--r--   0        0        0    16037 2023-07-31 13:58:43.085162 streams_py-1.0.1/pystreamapi/_streams/__base_stream.py
+-rw-r--r--   0        0        0        0 2023-07-31 13:58:43.085162 streams_py-1.0.1/pystreamapi/_streams/__init__.py
+-rw-r--r--   0        0        0     3380 2023-07-31 13:58:43.085162 streams_py-1.0.1/pystreamapi/_streams/__parallel_stream.py
+-rw-r--r--   0        0        0     2227 2023-07-31 13:58:43.085162 streams_py-1.0.1/pystreamapi/_streams/__sequential_stream.py
+-rw-r--r--   0        0        0     3062 2023-07-31 13:58:43.085162 streams_py-1.0.1/pystreamapi/_streams/error/__error.py
+-rw-r--r--   0        0        0      258 2023-07-31 13:58:43.085162 streams_py-1.0.1/pystreamapi/_streams/error/__levels.py
+-rw-r--r--   0        0        0      307 2023-07-31 13:58:43.085162 streams_py-1.0.1/pystreamapi/_streams/error/__sentinel.py
+-rw-r--r--   0        0        0     3595 2023-07-31 13:58:43.085162 streams_py-1.0.1/pystreamapi/_streams/numeric/__numeric_base_stream.py
+-rw-r--r--   0        0        0      861 2023-07-31 13:58:43.085162 streams_py-1.0.1/pystreamapi/_streams/numeric/__parallel_numeric_stream.py
+-rw-r--r--   0        0        0      686 2023-07-31 13:58:43.085162 streams_py-1.0.1/pystreamapi/_streams/numeric/__sequential_numeric_stream.py
+-rw-r--r--   0        0        0      221 2023-07-31 13:58:43.085162 streams_py-1.0.1/pystreamapi/conditions/__init__.py
+-rw-r--r--   0        0        0      307 2023-07-31 13:58:43.085162 streams_py-1.0.1/pystreamapi/conditions/combiners.py
+-rw-r--r--   0        0        0    10878 2023-07-31 13:58:43.085162 streams_py-1.0.1/pystreamapi/conditions/date.py
+-rw-r--r--   0        0        0     4937 2023-07-31 13:58:43.085162 streams_py-1.0.1/pystreamapi/conditions/numeric.py
+-rw-r--r--   0        0        0     1385 2023-07-31 13:58:43.085162 streams_py-1.0.1/pystreamapi/conditions/string.py
+-rw-r--r--   0        0        0      735 2023-07-31 13:58:43.085162 streams_py-1.0.1/pystreamapi/conditions/types.py
+-rw-r--r--   0        0        0     1943 2023-07-31 13:58:43.085162 streams_py-1.0.1/pystreamapi/loaders/__csv_loader.py
+-rw-r--r--   0        0        0       74 2023-07-31 13:58:43.085162 streams_py-1.0.1/pystreamapi/loaders/__init__.py
+-rw-r--r--   0        0        0      647 2023-07-31 13:58:43.085162 streams_py-1.0.1/pystreamapi/loaders/__lazy_file_iterable.py
+-rw-r--r--   0        0        0    12369 1970-01-01 00:00:00.000000 streams_py-1.0.1/PKG-INFO
```

### Comparing `streams_py-1.0.0/LICENSE` & `streams_py-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `streams_py-1.0.0/README.md` & `streams_py-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -222,17 +222,18 @@
 ```python
 from pystreamapi.loaders import csv
 ```
 Now you can use the loader directly when creating your Stream:
 
 ```python
 Stream.of(csv("data.csv", delimiter=";")) \
-    .map(lambda x: x["name"]) \
+    .map(lambda x: x.attr1) \
     .for_each(print)
 ```
+You can access the attributes of the CSV rows directly like you would with a normal object.
 
 ## API Reference
 For a more detailed documentation view the docs on GitBook: [PyStreamAPI Docs](https://pystreamapi.pickwicksoft.org/)
 
 ## Complex Examples
 
 #### Get all numbers from list of different types. Use parallelization.
```

#### html2text {}

```diff
@@ -111,22 +111,23 @@
 Stream.of([1, 2, 3, 4]) ``` Creates a new Stream from multiple Streams. Order
 doesn't change. ## Use loaders: Load data from CSV files in just one line
 PyStreamAPI offers a convenient way to load data from CSV files. Like that you
 can start processing your CSV right away without having to worry about reading
 and parsing the file. You can import the loader with: ```python from
 pystreamapi.loaders import csv ``` Now you can use the loader directly when
 creating your Stream: ```python Stream.of(csv("data.csv", delimiter=";")) \
-.map(lambda x: x["name"]) \ .for_each(print) ``` ## API Reference For a more
-detailed documentation view the docs on GitBook: [PyStreamAPI Docs](https://
-pystreamapi.pickwicksoft.org/) ## Complex Examples #### Get all numbers from
-list of different types. Use parallelization. ```python Stream.parallel_of(["
-", '3', None, "2", 1, ""]) \ .filter(lambda x: x is not None) \ .map(str) \
-.map(lambda x: x.strip()) \ .filter(lambda x: len(x) > 0) \ .map(int) \ .sorted
-()\ .for_each(print) # 1 2 3 ``` #### Generate a Stream of 10 Fibonacci numbers
-```python def fib(): a, b = 0, 1 while True: yield a a, b = b, a + b Stream.of
-(fib()) \ .limit(10) \ .for_each(print) # 0 1 1 2 3 5 8 13 21 34 ``` ##
-Performance Note that parallel Streams are not always faster than sequential
-Streams. Especially when the number of elements is small, we can expect
-sequential Streams to be faster. ## Bug Reports Bug reports can be submitted in
-GitHub's [issue tracker](https://github.com/PickwickSoft/pystreamapi/issues).
-## Contributing Contributions are welcome! Please submit a pull request or open
-an issue.
+.map(lambda x: x.attr1) \ .for_each(print) ``` You can access the attributes of
+the CSV rows directly like you would with a normal object. ## API Reference For
+a more detailed documentation view the docs on GitBook: [PyStreamAPI Docs]
+(https://pystreamapi.pickwicksoft.org/) ## Complex Examples #### Get all
+numbers from list of different types. Use parallelization. ```python
+Stream.parallel_of([" ", '3', None, "2", 1, ""]) \ .filter(lambda x: x is not
+None) \ .map(str) \ .map(lambda x: x.strip()) \ .filter(lambda x: len(x) > 0) \
+.map(int) \ .sorted()\ .for_each(print) # 1 2 3 ``` #### Generate a Stream of
+10 Fibonacci numbers ```python def fib(): a, b = 0, 1 while True: yield a a, b
+= b, a + b Stream.of(fib()) \ .limit(10) \ .for_each(print) # 0 1 1 2 3 5 8 13
+21 34 ``` ## Performance Note that parallel Streams are not always faster than
+sequential Streams. Especially when the number of elements is small, we can
+expect sequential Streams to be faster. ## Bug Reports Bug reports can be
+submitted in GitHub's [issue tracker](https://github.com/PickwickSoft/
+pystreamapi/issues). ## Contributing Contributions are welcome! Please submit a
+pull request or open an issue.
```

### Comparing `streams_py-1.0.0/pyproject.toml` & `streams_py-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "streams.py"
-version = "1.0.0"
+version = "1.0.1"
 authors = ["Stefan Garlonta <stefan@pickwicksoft.org>"]
 description = "A stream library for Python inspired by Java Stream API"
 keywords = ["streams", "parallel", "data"]
 license = "GPL-3.0-or-later"
 homepage = "https://github.com/PickwickSoft/pystreamapi"
 repository = "https://github.com/PickwickSoft/pystreamapi"
 readme = "README.md"
```

### Comparing `streams_py-1.0.0/pystreamapi/__optional.py` & `streams_py-1.0.1/pystreamapi/__optional.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.0.0/pystreamapi/__stream.py` & `streams_py-1.0.1/pystreamapi/__stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.0.0/pystreamapi/__stream_converter.py` & `streams_py-1.0.1/pystreamapi/__stream_converter.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.0.0/pystreamapi/_itertools/tools.py` & `streams_py-1.0.1/pystreamapi/_itertools/tools.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.0.0/pystreamapi/_lazy/process.py` & `streams_py-1.0.1/pystreamapi/_lazy/process.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.0.0/pystreamapi/_lazy/queue.py` & `streams_py-1.0.1/pystreamapi/_lazy/queue.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.0.0/pystreamapi/_parallel/fork_and_join.py` & `streams_py-1.0.1/pystreamapi/_parallel/fork_and_join.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.0.0/pystreamapi/_parallel/parallelizer.py` & `streams_py-1.0.1/pystreamapi/_parallel/parallelizer.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.0.0/pystreamapi/_streams/__base_stream.py` & `streams_py-1.0.1/pystreamapi/_streams/__base_stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.0.0/pystreamapi/_streams/__parallel_stream.py` & `streams_py-1.0.1/pystreamapi/_streams/__parallel_stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.0.0/pystreamapi/_streams/__sequential_stream.py` & `streams_py-1.0.1/pystreamapi/_streams/__sequential_stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.0.0/pystreamapi/_streams/error/__error.py` & `streams_py-1.0.1/pystreamapi/_streams/error/__error.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.0.0/pystreamapi/_streams/numeric/__numeric_base_stream.py` & `streams_py-1.0.1/pystreamapi/_streams/numeric/__numeric_base_stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.0.0/pystreamapi/_streams/numeric/__parallel_numeric_stream.py` & `streams_py-1.0.1/pystreamapi/_streams/numeric/__parallel_numeric_stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.0.0/pystreamapi/_streams/numeric/__sequential_numeric_stream.py` & `streams_py-1.0.1/pystreamapi/_streams/numeric/__sequential_numeric_stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.0.0/pystreamapi/conditions/date.py` & `streams_py-1.0.1/pystreamapi/conditions/date.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.0.0/pystreamapi/conditions/numeric.py` & `streams_py-1.0.1/pystreamapi/conditions/numeric.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.0.0/pystreamapi/conditions/string.py` & `streams_py-1.0.1/pystreamapi/conditions/string.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.0.0/pystreamapi/conditions/types.py` & `streams_py-1.0.1/pystreamapi/conditions/types.py`

 * *Files identical despite different names*

### Comparing `streams_py-1.0.0/PKG-INFO` & `streams_py-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streams-py
-Version: 1.0.0
+Version: 1.0.1
 Summary: A stream library for Python inspired by Java Stream API
 Home-page: https://github.com/PickwickSoft/pystreamapi
 License: GPL-3.0-or-later
 Keywords: streams,parallel,data
 Author: Stefan Garlonta
 Author-email: stefan@pickwicksoft.org
 Requires-Python: >=3.7,<4.0
@@ -243,17 +243,18 @@
 ```python
 from pystreamapi.loaders import csv
 ```
 Now you can use the loader directly when creating your Stream:
 
 ```python
 Stream.of(csv("data.csv", delimiter=";")) \
-    .map(lambda x: x["name"]) \
+    .map(lambda x: x.attr1) \
     .for_each(print)
 ```
+You can access the attributes of the CSV rows directly like you would with a normal object.
 
 ## API Reference
 For a more detailed documentation view the docs on GitBook: [PyStreamAPI Docs](https://pystreamapi.pickwicksoft.org/)
 
 ## Complex Examples
 
 #### Get all numbers from list of different types. Use parallelization.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: streams-py Version: 1.0.0 Summary: A stream library
+Metadata-Version: 2.1 Name: streams-py Version: 1.0.1 Summary: A stream library
 for Python inspired by Java Stream API Home-page: https://github.com/
 PickwickSoft/pystreamapi License: GPL-3.0-or-later Keywords:
 streams,parallel,data Author: Stefan Garlonta Author-email:
 stefan@pickwicksoft.org Requires-Python: >=3.7,<4.0 Classifier: License :: OSI
 Approved :: GNU General Public License v3 or later (GPLv3+) Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
@@ -123,22 +123,23 @@
 Stream.of([1, 2, 3, 4]) ``` Creates a new Stream from multiple Streams. Order
 doesn't change. ## Use loaders: Load data from CSV files in just one line
 PyStreamAPI offers a convenient way to load data from CSV files. Like that you
 can start processing your CSV right away without having to worry about reading
 and parsing the file. You can import the loader with: ```python from
 pystreamapi.loaders import csv ``` Now you can use the loader directly when
 creating your Stream: ```python Stream.of(csv("data.csv", delimiter=";")) \
-.map(lambda x: x["name"]) \ .for_each(print) ``` ## API Reference For a more
-detailed documentation view the docs on GitBook: [PyStreamAPI Docs](https://
-pystreamapi.pickwicksoft.org/) ## Complex Examples #### Get all numbers from
-list of different types. Use parallelization. ```python Stream.parallel_of(["
-", '3', None, "2", 1, ""]) \ .filter(lambda x: x is not None) \ .map(str) \
-.map(lambda x: x.strip()) \ .filter(lambda x: len(x) > 0) \ .map(int) \ .sorted
-()\ .for_each(print) # 1 2 3 ``` #### Generate a Stream of 10 Fibonacci numbers
-```python def fib(): a, b = 0, 1 while True: yield a a, b = b, a + b Stream.of
-(fib()) \ .limit(10) \ .for_each(print) # 0 1 1 2 3 5 8 13 21 34 ``` ##
-Performance Note that parallel Streams are not always faster than sequential
-Streams. Especially when the number of elements is small, we can expect
-sequential Streams to be faster. ## Bug Reports Bug reports can be submitted in
-GitHub's [issue tracker](https://github.com/PickwickSoft/pystreamapi/issues).
-## Contributing Contributions are welcome! Please submit a pull request or open
-an issue.
+.map(lambda x: x.attr1) \ .for_each(print) ``` You can access the attributes of
+the CSV rows directly like you would with a normal object. ## API Reference For
+a more detailed documentation view the docs on GitBook: [PyStreamAPI Docs]
+(https://pystreamapi.pickwicksoft.org/) ## Complex Examples #### Get all
+numbers from list of different types. Use parallelization. ```python
+Stream.parallel_of([" ", '3', None, "2", 1, ""]) \ .filter(lambda x: x is not
+None) \ .map(str) \ .map(lambda x: x.strip()) \ .filter(lambda x: len(x) > 0) \
+.map(int) \ .sorted()\ .for_each(print) # 1 2 3 ``` #### Generate a Stream of
+10 Fibonacci numbers ```python def fib(): a, b = 0, 1 while True: yield a a, b
+= b, a + b Stream.of(fib()) \ .limit(10) \ .for_each(print) # 0 1 1 2 3 5 8 13
+21 34 ``` ## Performance Note that parallel Streams are not always faster than
+sequential Streams. Especially when the number of elements is small, we can
+expect sequential Streams to be faster. ## Bug Reports Bug reports can be
+submitted in GitHub's [issue tracker](https://github.com/PickwickSoft/
+pystreamapi/issues). ## Contributing Contributions are welcome! Please submit a
+pull request or open an issue.
```

