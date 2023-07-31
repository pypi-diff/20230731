# Comparing `tmp/data_serialize-0.2.1-py3-none-any.whl.zip` & `tmp/data_serialize-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,17 @@
-Zip file size: 8540 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat      163 b- defN 22-Nov-07 01:59 data_serialize/__init__.py
--rw-rw-rw-  2.0 fat     1823 b- defN 22-Nov-07 06:12 data_serialize/demo.py
--rw-rw-rw-  2.0 fat     4003 b- defN 22-Nov-07 02:00 data_serialize/example_pb2.py
--rw-rw-rw-  2.0 fat    14902 b- defN 22-Nov-07 01:57 data_serialize/feature_pb2.py
--rw-rw-rw-  2.0 fat     9345 b- defN 22-Nov-07 06:14 data_serialize/numpyobject_pb2.py
--rw-rw-rw-  2.0 fat     1083 b- defN 22-Nov-07 06:09 data_serialize/setup.py
--rw-rw-rw-  2.0 fat     2266 b- defN 22-Nov-07 06:15 data_serialize-0.2.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Nov-07 06:15 data_serialize-0.2.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 22-Nov-07 06:15 data_serialize-0.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      830 b- defN 22-Nov-07 06:15 data_serialize-0.2.1.dist-info/RECORD
-10 files, 34522 bytes uncompressed, 7122 bytes compressed:  79.4%
+Zip file size: 12518 bytes, number of entries: 15
+-rw-rw-rw-  2.0 fat      498 b- defN 23-Jul-31 05:09 data_serialize/__init__.py
+-rw-rw-rw-  2.0 fat     1833 b- defN 22-Nov-07 07:50 data_serialize/demo.py
+-rw-rw-rw-  2.0 fat     1067 b- defN 23-Jul-31 05:06 data_serialize/setup.py
+-rw-rw-rw-  2.0 fat       77 b- defN 23-Jul-31 04:45 data_serialize/pb/__init__.py
+-rw-rw-rw-  2.0 fat     4003 b- defN 23-Jul-31 04:53 data_serialize/pb/example_pb2.py
+-rw-rw-rw-  2.0 fat    14902 b- defN 22-Nov-07 01:57 data_serialize/pb/feature_pb2.py
+-rw-rw-rw-  2.0 fat     9345 b- defN 22-Nov-07 06:14 data_serialize/pb/numpyobject_pb2.py
+-rw-rw-rw-  2.0 fat       77 b- defN 23-Jul-31 04:45 data_serialize/pb4/__init__.py
+-rw-rw-rw-  2.0 fat     1836 b- defN 23-Jul-31 04:56 data_serialize/pb4/example_pb2.py
+-rw-rw-rw-  2.0 fat     6063 b- defN 23-Jul-31 04:40 data_serialize/pb4/feature_pb2.py
+-rw-rw-rw-  2.0 fat     3832 b- defN 23-Jul-31 04:40 data_serialize/pb4/numpyobject_pb2.py
+-rw-rw-rw-  2.0 fat     2251 b- defN 23-Jul-31 05:12 data_serialize-0.2.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-31 05:12 data_serialize-0.2.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-Jul-31 05:12 data_serialize-0.2.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1282 b- defN 23-Jul-31 05:12 data_serialize-0.2.2.dist-info/RECORD
+15 files, 47173 bytes uncompressed, 10378 bytes compressed:  78.0%
```

## zipnote {}

```diff
@@ -1,31 +1,46 @@
 Filename: data_serialize/__init__.py
 Comment: 
 
 Filename: data_serialize/demo.py
 Comment: 
 
-Filename: data_serialize/example_pb2.py
+Filename: data_serialize/setup.py
 Comment: 
 
-Filename: data_serialize/feature_pb2.py
+Filename: data_serialize/pb/__init__.py
 Comment: 
 
-Filename: data_serialize/numpyobject_pb2.py
+Filename: data_serialize/pb/example_pb2.py
 Comment: 
 
-Filename: data_serialize/setup.py
+Filename: data_serialize/pb/feature_pb2.py
+Comment: 
+
+Filename: data_serialize/pb/numpyobject_pb2.py
+Comment: 
+
+Filename: data_serialize/pb4/__init__.py
+Comment: 
+
+Filename: data_serialize/pb4/example_pb2.py
+Comment: 
+
+Filename: data_serialize/pb4/feature_pb2.py
+Comment: 
+
+Filename: data_serialize/pb4/numpyobject_pb2.py
 Comment: 
 
-Filename: data_serialize-0.2.1.dist-info/METADATA
+Filename: data_serialize-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: data_serialize-0.2.1.dist-info/WHEEL
+Filename: data_serialize-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: data_serialize-0.2.1.dist-info/top_level.txt
+Filename: data_serialize-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: data_serialize-0.2.1.dist-info/RECORD
+Filename: data_serialize-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## data_serialize/__init__.py

```diff
@@ -1,7 +1,19 @@
 # @Time    : 2022/9/15 13:51
 # @Author  : tk
 # @FileName: __init__.py
+import inspect
 
-from .feature_pb2 import *
-from .example_pb2 import *
-from .numpyobject_pb2 import *
+try:
+    from google.protobuf import __version__ as pb_ver
+
+except:
+    pb_ver = '3'
+
+if pb_ver.startswith('4') or pb_ver.startswith('3.20') or pb_ver.startswith('3.21') :
+    from .pb4.feature_pb2 import *
+    from .pb4.example_pb2 import *
+    from .pb4.numpyobject_pb2 import *
+else:
+    from .pb.feature_pb2 import *
+    from .pb.example_pb2 import *
+    from .pb.numpyobject_pb2 import *
```

## data_serialize/demo.py

```diff
@@ -27,15 +27,15 @@
     example.ParseFromString(serialize)
     print(example)
 
 
 def test_numpyobject():
     a = np.random.randint(0, 21128, size=(10,), dtype=np.int64)
     b = np.random.rand(3, 4)
-    c = np.asarray(b'The china')
+    c = np.asarray(b'111111111aaaaaaaaaa')
 
     val1 = data_serialize.NumpyObject(
         header='',
         dtype=str(a.dtype),
         shape=list(a.shape),
         int64=a.reshape((-1,)).tolist(),
     )
```

## data_serialize/setup.py

```diff
@@ -8,24 +8,24 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 
 # List of runtime dependencies required by this built package
 install_requires = []
 
-install_requires += ['protobuf >= 3.8 , <4.0.0']
+install_requires += ['protobuf']
 
 # read the contents of README file
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'),mode='r',encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='data_serialize',
-    version='0.2.1',
+    version='0.2.2',
     description='data serialize',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='ssbuild',
     author_email='9727464@qq.com',
     url='https://github.com/ssbuild/fastdatasets',
     packages=find_packages(),
```

## Comparing `data_serialize/example_pb2.py` & `data_serialize/pb/example_pb2.py`

 * *Files identical despite different names*

## Comparing `data_serialize/feature_pb2.py` & `data_serialize/pb/feature_pb2.py`

 * *Files identical despite different names*

## Comparing `data_serialize/numpyobject_pb2.py` & `data_serialize/pb/numpyobject_pb2.py`

 * *Files identical despite different names*

## Comparing `data_serialize-0.2.1.dist-info/METADATA` & `data_serialize-0.2.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: data-serialize
-Version: 0.2.1
+Version: 0.2.2
 Summary: data serialize
 Home-page: https://github.com/ssbuild/fastdatasets
 Author: ssbuild
 Author-email: 9727464@qq.com
 License: MIT
 Keywords: data_serialize,serialize,deserialize
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-Requires-Dist: protobuf (<4.0.0,>=3.8)
+Requires-Dist: protobuf
 
 # data_serialize
 
 This library allows reading and writing binary to string 
 
 ## Installation
```

