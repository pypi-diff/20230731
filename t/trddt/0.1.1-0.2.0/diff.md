# Comparing `tmp/trddt-0.1.1.tar.gz` & `tmp/trddt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trddt-0.1.1.tar", last modified: Sun Mar 26 08:22:43 2023, max compression
+gzip compressed data, was "trddt-0.2.0.tar", last modified: Mon Jul 31 05:20:50 2023, max compression
```

## Comparing `trddt-0.1.1.tar` & `trddt-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-26 08:22:43.887329 trddt-0.1.1/
--rw-rw-rw-   0        0        0     1085 2023-03-20 13:07:23.000000 trddt-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      531 2023-03-26 08:22:43.886328 trddt-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       69 2023-03-20 13:07:23.000000 trddt-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-03-26 08:22:43.887329 trddt-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      813 2023-03-26 08:22:26.000000 trddt-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-26 08:22:43.862322 trddt-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-03-26 08:22:43.884327 trddt-0.1.1/src/trddt.egg-info/
--rw-rw-rw-   0        0        0      531 2023-03-26 08:22:43.000000 trddt-0.1.1/src/trddt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-03-26 08:22:43.000000 trddt-0.1.1/src/trddt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-26 08:22:43.000000 trddt-0.1.1/src/trddt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-03-26 08:22:43.000000 trddt-0.1.1/src/trddt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-03-26 08:22:43.000000 trddt-0.1.1/src/trddt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 05:20:50.431042 trddt-0.2.0/
+-rw-rw-rw-   0        0        0     1086 2023-07-31 05:08:10.000000 trddt-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      678 2023-07-31 05:20:50.430041 trddt-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-07-31 05:13:45.000000 trddt-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-31 05:20:50.432042 trddt-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      869 2023-07-31 05:12:43.000000 trddt-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 05:20:50.389033 trddt-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-31 05:20:50.399035 trddt-0.2.0/src/trddt/
+-rw-rw-rw-   0        0        0    10486 2023-06-07 08:52:40.000000 trddt-0.2.0/src/trddt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 05:20:50.427042 trddt-0.2.0/src/trddt.egg-info/
+-rw-rw-rw-   0        0        0      678 2023-07-31 05:20:50.000000 trddt-0.2.0/src/trddt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-07-31 05:20:50.000000 trddt-0.2.0/src/trddt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 05:20:50.000000 trddt-0.2.0/src/trddt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-07-31 05:20:50.000000 trddt-0.2.0/src/trddt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-31 05:20:50.000000 trddt-0.2.0/src/trddt.egg-info/top_level.txt
```

### Comparing `trddt-0.1.1/LICENSE` & `trddt-0.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `trddt-0.1.1/PKG-INFO` & `trddt-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,30 @@
 Metadata-Version: 2.1
 Name: trddt
-Version: 0.1.1
+Version: 0.2.0
 Summary: 한국거래소 기준 Datetime Functions 패키지
 Home-page: https://github.com/innovata/TradeDatetime
 Author: innovata
 Author-email: iinnovata@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TradeDatetime
- 한국거래소 기준 Datetime Functions 패키지
+한국거래소 기준 Datetime Functions 패키지
+
+
+
+
+
+<!-- ============================================================ -->
+## Dependancy
+
+    holidays==0.21
+
+    pandas
+
+    ipylib
+
```

### Comparing `trddt-0.1.1/setup.py` & `trddt-0.2.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # -*- coding: utf-8 -*-
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
+SOURCE_DIRECTORY = 'src'
+
 setuptools.setup(
     name="trddt",
-    version="0.1.1",
+    version="0.2.0",
     author="innovata",
     author_email="iinnovata@gmail.com",
     description='한국거래소 기준 Datetime Functions 패키지',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=f"https://github.com/innovata/TradeDatetime",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    package_dir={"":"src"},
-    packages=setuptools.find_packages(),
+    package_dir={"": SOURCE_DIRECTORY},
+    packages=setuptools.find_packages(SOURCE_DIRECTORY),
     python_requires=">=3.8",
     install_requires=['ipylib', 'holidays', 'pandas'],
 )
```

### Comparing `trddt-0.1.1/src/trddt.egg-info/PKG-INFO` & `trddt-0.2.0/src/trddt.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,30 @@
 Metadata-Version: 2.1
 Name: trddt
-Version: 0.1.1
+Version: 0.2.0
 Summary: 한국거래소 기준 Datetime Functions 패키지
 Home-page: https://github.com/innovata/TradeDatetime
 Author: innovata
 Author-email: iinnovata@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TradeDatetime
- 한국거래소 기준 Datetime Functions 패키지
+한국거래소 기준 Datetime Functions 패키지
+
+
+
+
+
+<!-- ============================================================ -->
+## Dependancy
+
+    holidays==0.21
+
+    pandas
+
+    ipylib
+
```

