# Comparing `tmp/cads_sdk-0.0.26-py3-none-any.whl.zip` & `tmp/cads_sdk-0.0.27-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,22 @@
-Zip file size: 56540 bytes, number of entries: 18
--rw-rw-r--  2.0 unx     1265 b- defN 23-Jun-08 03:23 cads_sdk/__init__.py
+Zip file size: 58871 bytes, number of entries: 20
+-rw-rw-r--  2.0 unx     1265 b- defN 23-Jul-31 03:24 cads_sdk/__init__.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-31 03:22 cads_sdk/id_card/__init__.py
+-rw-rw-r--  2.0 unx     5330 b- defN 23-Jul-31 03:20 cads_sdk/id_card/display.py
 -rw-rw-r--  2.0 unx     1264 b- defN 23-Apr-01 02:59 cads_sdk/nosql/__init__.py
--rw-rw-r--  2.0 unx    11231 b- defN 23-Apr-17 08:04 cads_sdk/nosql/codec.py
--rw-rw-r--  2.0 unx    86938 b- defN 23-May-18 09:04 cads_sdk/nosql/converter.py
--rw-rw-r--  2.0 unx    20961 b- defN 23-Jun-08 03:25 cads_sdk/nosql/display.py
+-rw-rw-r--  2.0 unx    11250 b- defN 23-Jun-30 10:12 cads_sdk/nosql/codec.py
+-rw-rw-r--  2.0 unx    86993 b- defN 23-Jul-31 03:24 cads_sdk/nosql/converter.py
+-rw-rw-r--  2.0 unx    22061 b- defN 23-Jul-31 03:15 cads_sdk/nosql/display.py
 -rw-rw-r--  2.0 unx     1187 b- defN 23-Apr-10 10:46 cads_sdk/nosql/etl.py
 -rw-rw-r--  2.0 unx     1291 b- defN 23-May-19 02:11 cads_sdk/nosql/utils.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-09 14:03 cads_sdk/petastorm/__init__.py
 -rw-rw-r--  2.0 unx    19967 b- defN 23-Apr-10 04:34 cads_sdk/petastorm/dataset_metadata.py
 -rw-rw-r--  2.0 unx    10508 b- defN 23-Apr-10 07:19 cads_sdk/petastorm/fs_utils.py
 -rw-rw-r--  2.0 unx     5427 b- defN 23-Apr-10 04:42 cads_sdk/petastorm/utils.py
 -rw-rw-r--  2.0 unx    22554 b- defN 23-Apr-18 15:18 cads_sdk/pytorch/__init__.py
 -rw-rw-r--  2.0 unx    10653 b- defN 23-Apr-17 08:05 cads_sdk/pytorch/codec.py
 -rw-rw-r--  2.0 unx    78369 b- defN 23-Apr-20 08:23 cads_sdk/pytorch/converter.py
--rw-rw-r--  2.0 unx     7123 b- defN 23-Jun-08 03:27 cads_sdk-0.0.26.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-08 03:27 cads_sdk-0.0.26.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-Jun-08 03:27 cads_sdk-0.0.26.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1480 b- defN 23-Jun-08 03:27 cads_sdk-0.0.26.dist-info/RECORD
-18 files, 280319 bytes uncompressed, 54134 bytes compressed:  80.7%
+-rw-rw-r--  2.0 unx     7111 b- defN 23-Jul-31 03:25 cads_sdk-0.0.27.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-31 03:25 cads_sdk-0.0.27.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-Jul-31 03:25 cads_sdk-0.0.27.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1646 b- defN 23-Jul-31 03:25 cads_sdk-0.0.27.dist-info/RECORD
+20 files, 286977 bytes uncompressed, 56203 bytes compressed:  80.4%
```

## zipnote {}

```diff
@@ -1,10 +1,16 @@
 Filename: cads_sdk/__init__.py
 Comment: 
 
+Filename: cads_sdk/id_card/__init__.py
+Comment: 
+
+Filename: cads_sdk/id_card/display.py
+Comment: 
+
 Filename: cads_sdk/nosql/__init__.py
 Comment: 
 
 Filename: cads_sdk/nosql/codec.py
 Comment: 
 
 Filename: cads_sdk/nosql/converter.py
@@ -36,20 +42,20 @@
 
 Filename: cads_sdk/pytorch/codec.py
 Comment: 
 
 Filename: cads_sdk/pytorch/converter.py
 Comment: 
 
-Filename: cads_sdk-0.0.26.dist-info/METADATA
+Filename: cads_sdk-0.0.27.dist-info/METADATA
 Comment: 
 
-Filename: cads_sdk-0.0.26.dist-info/WHEEL
+Filename: cads_sdk-0.0.27.dist-info/WHEEL
 Comment: 
 
-Filename: cads_sdk-0.0.26.dist-info/top_level.txt
+Filename: cads_sdk-0.0.27.dist-info/top_level.txt
 Comment: 
 
-Filename: cads_sdk-0.0.26.dist-info/RECORD
+Filename: cads_sdk-0.0.27.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cads_sdk/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.0.26'
+__version__ = '0.0.27'
 
 __doc__ = """
 cads-sdk: Functions to help Data Scientist work more effectively with unstructured data and datalake
 =====================================================================
 **cads-sdk**
 Function to convert 
 -------------
```

## cads_sdk/nosql/codec.py

```diff
@@ -30,15 +30,17 @@
  'copy_reg',
  'decimal',
  'numpy',
  'petastorm',
  'pyspark',
  'cads_sdk',
  'spark_sdk'}
-petastorm.etl.legacy.safe_modules = safe_modules
+
+import petastorm.etl as ETL
+ETL.legacy.safe_modules = safe_modules
 
 
 class DataframeColumnCodec(object):
     """The abstract base class of codecs."""
 
     @abstractmethod
     def encode(self, unischema_field, value):
```

## cads_sdk/nosql/converter.py

```diff
@@ -162,16 +162,15 @@
                     return spark_df.repartition(numPartition)
                 else:
                     return spark_df.coalesce(numPartition)
         return spark_df
     
     
     def get_spark(self):
-        return ss.PySpark(driver_memory='32G', num_executors='8', executor_memory='4G', port='', yarn=False, 
-                         optimze_file_size=("spark.databricks.delta.optimize.maxFileSize", 536870912)).spark
+        return ss.PySpark(driver_memory='32G', num_executors='8', executor_memory='4G', port='', yarn=False).spark
     
     def create_dataframe(self, 
                          spark, 
                          Schema, 
                          input_files):
         from pyspark.sql.functions import expr
         self.unischema = Schema
@@ -491,19 +490,26 @@
                         'path': path,
                         'size': img.size.__str__(),
                         'image': open(path, 'rb').read()
                     }
 
                     yield dict_to_spark_row(self.unischema, row_dict)
             else:
-                row_dict = {
-                    'path': path,
-                    'size': "Can not get size",
-                    'image': open(path, 'rb').read()
-                }
+                try:
+                    row_dict = {
+                        'path': path,
+                        'size': "Can not get size",
+                        'image': open(path, 'rb').read()
+                    }
+                except:
+                    row_dict = {
+                        'path': path,
+                        'size': "Can not open image, image damage",
+                        'image': b''
+                    }
 
                 yield dict_to_spark_row(self.unischema, row_dict)
 
        
                     
     def get_schema(self, size, image_type, image_color):
         """
@@ -1606,16 +1612,15 @@
         
         self.thumbnail_width = frame_size[0]
         self.thumbnail_height = frame_size[1]
         
         return spark.createDataFrame(spark_df.rdd.mapPartitions(self.row_generator), Schema.as_spark_schema())
         
     def get_spark(self):
-        return ss.PySpark(driver_memory='32G', num_executors='8', executor_memory='4G', port='', yarn=False, 
-                         optimze_file_size=("spark.databricks.delta.optimize.maxFileSize", 536870912)).spark
+        return ss.PySpark(driver_memory='32G', num_executors='8', executor_memory='4G', port='', yarn=False).spark
     
     def get_schema(self):
         return Unischema('VideoImage', [
             UnischemaField('frame_id', np.int, (), ScalarCodec(IntegerType()), False),
             UnischemaField('path', np.str_, (), ScalarCodec(StringType()), False),
             UnischemaField('duration', np.float_, (), ScalarCodec(FloatType()), False),
             UnischemaField('frame_size', np.str_, (), ScalarCodec(StringType()), False),
```

## cads_sdk/nosql/display.py

```diff
@@ -197,23 +197,59 @@
                 pdf[c_name] = pdf[c_name].apply(openImage)
             need_convert_dict[c_name] = image_formatter
     DataFrame.need_convert_dict = need_convert_dict
     pdf.need_convert_dict = need_convert_dict
     return pdf
 
 
+def toPandasImagePyarrow(self, limit:int = 100, mode='RGB'):
+    """
+    Function to display image in parquet as a DataFrame
+    Parameters
+    ----------
+    limit : int
+        Default: 100
+        Limit number of display image at the same time
+        Maxium is 100
+    mode : str
+        Color mode 
+        Default: 'RGB'
+        RGB or BGR
+        
+    """
+    if limit > 100:
+        limit = 100
+    pdf = self.to_pandas()
+    # pdf = self.limit(limit).toPandas()
+    
+    need_convert_dict = {}
+    for c in df.schema:
+        if "binary" in str(c.type):
+            c_name = c.name
+            # pdf[c_name] = pdf[c_name].apply(lambda x: Image.open(io.BytesIO(x)))
+            if mode=='BGR':
+                pdf[c_name] = pdf[c_name].apply(cvtColor)
+            else:
+                pdf[c_name] = pdf[c_name].apply(openImage)
+            need_convert_dict[c_name] = image_formatter
+    DataFrame.need_convert_dict = need_convert_dict
+    pdf.need_convert_dict = need_convert_dict
+    return pdf
+
+
 from pyspark.sql import DataFrame as SparkDataFrame
 SparkDataFrame.__getitem__ = __getitem__
 SparkDataFrame.convert_to_index_sliceable = convert_to_index_sliceable
 SparkDataFrame._create_idx_dataframe = _create_idx_dataframe
 SparkDataFrame._filter_idx = _filter_idx
 
 
 SparkDataFrame.toPandasImage = toPandasImage
 
+####################################
 from pandas._config import get_option
 from io import StringIO
 from pandas.io.formats import format as fmt
 from typing import Optional
 
 def _repr_html_(self) -> Optional[str]:
     """
@@ -264,15 +300,15 @@
         
         return fmt.DataFrameRenderer(formatter).to_html()
     else:
         return None
 
 from pandas import DataFrame
 DataFrame._repr_html_ = _repr_html_
-
+####################################
 import os
 import tempfile
 
 
 from spark_sdk.utils import import_or_install
 import_or_install("ipywidgets")
 try:
@@ -529,15 +565,15 @@
         os.environ['JAVA_HOME'] = "/usr/jdk64/jdk1.8.0_112"
         os.environ['HADOOP_HOME'] = "/usr/hdp/3.1.0.0-78/hadoop"
         os.environ['ARROW_LIBHDFS_DIR'] = "/usr/hdp/3.1.0.0-78/usr/lib/"
         os.environ['CLASSPATH'] = subprocess.check_output("$HADOOP_HOME/bin/hadoop classpath --glob", shell=True).decode('utf-8')
 
         hdfs = fs.HadoopFileSystem(host="hdfs://hdfs-cluster.datalake.bigdata.local", port=8020)
 
-        df_pq = pq.read_table(parquet_file)
+        df_pq = pq.read_table(parquet_file, filesystem = hdfs)
         pdf = df_pq.to_pandas()
         pdf = pdf[pdf['path']==path].iloc[0]
         self.write_to_folder(pdf)
         
             
     def displayAudio(self, ex):
         get_value = ex.value
```

## Comparing `cads_sdk-0.0.26.dist-info/METADATA` & `cads_sdk-0.0.27.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: cads-sdk
-Version: 0.0.26
+Version: 0.0.27
 Summary: Function to help Data Scientist work more effectively with DWH
 Home-page: http://git.bigdata.local/data-engineers/sdk/utilities
 Author: duyvnc
 Author-email: duyvnc@fpt.com.vn
 License: duyvnc
+Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
-Requires-Dist: spark-sdk (>=0.4.20)
+Requires-Dist: spark-sdk (>=0.4.23)
 Requires-Dist: opencv-python
 Requires-Dist: Pillow
 Requires-Dist: scipy
 Requires-Dist: pydub
 Requires-Dist: ipywidgets
 Requires-Dist: petastorm
 
 -----------------
 
 # cads-sdk: Functions to help Data Scientist work more effectively with unstructured data and datalake
-[![PyPI Latest Release](https://img.shields.io/badge/pypi-0.0.23-blue)](https://pypi.org/project/cads-sdk/)
+[![PyPI Latest Release](https://img.shields.io/badge/pypi-0.0.26-blue)](https://pypi.org/project/cads-sdk/)
 [![Package Status](https://img.shields.io/badge/status-stable-green)](https://pypi.org/project/cads-sdk/)
 [![Downloads](https://static.pepy.tech/personalized-badge/cads-sdk?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/cads-sdk)
 [![Powered by NumFOCUS](https://img.shields.io/badge/powered%20by-CADS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://blog.cads.live/)
 
 
 
 ## What is it?
@@ -82,18 +83,18 @@
 ```python
 from cads_sdk.nosql.converter import ConvertFromFolderImage
 
 converter = ConvertFromFolderImage(
               input_path="/path/to/folder/**/*.jpg",
               input_type = 'jpg' # 'jpg' | ('jpg', 'png')
               input_recursive = True,
-              
+
               #setting output
               output_path = f"file:/output/path/image_storage",
-              
+
               # setting converter
               image_type = 'jpg',
               image_color = 3,
               resize_mode=None, # |padding|resize
               size = [(212,212),
                      (597, 597)],
              )
@@ -103,15 +104,15 @@
 # convert directly from .zip file to parquet
 from cads_sdk.nosql.converter import ConvertFromZipImage
 
 converter = ConvertFromZipImage(
               input_path="/path/to/image_storage/ETHZ.zip",
               input_recursive = True, # will loop through folder to get all pattern
               input_type = 'jpg' # 'jpg' | ('jpg', 'png')
-    
+
               #setting output
               output_path = f"file:/output/path/img_ethz.parquet",
               table_name = 'img_ethz',
               database = 'default',
               file_format = 'parquet', # delta|parquet
               compression = 'zstd', # zstd|snappy
               # setting converter
@@ -206,7 +207,9 @@
 converter.execute()
 ```
 ### For more information use class instance
 ```python
 ConvertFromFolderImage.__doc__
 ```
 
+
+
```

## Comparing `cads_sdk-0.0.26.dist-info/RECORD` & `cads_sdk-0.0.27.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-cads_sdk/__init__.py,sha256=NvUb-g5CIN1tFa1dnXVjSzIBIrIYax3v3fewap5c6Fs,1265
+cads_sdk/__init__.py,sha256=smBGL2a0WuVoqU6ocu6le3XLZJaI6M7pE12lP69dy_c,1265
+cads_sdk/id_card/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+cads_sdk/id_card/display.py,sha256=1pqhu2BaRJgawGRw0yKf7RNieegqqJRwHbBWJqe2YSc,5330
 cads_sdk/nosql/__init__.py,sha256=Yu2Zt5cpSXSLqIRAvIxaXOtoyj3yBisGTbnFlH4UD2A,1264
-cads_sdk/nosql/codec.py,sha256=Z0RdndLtSHAnqHOpDGE-Wb_jD9eIWvKiuX4Yj1KudX4,11231
-cads_sdk/nosql/converter.py,sha256=TUVOQIEqE60zpoxZbyc9fcgaFOVkYy37ZmwtBVG8LoI,86938
-cads_sdk/nosql/display.py,sha256=pUA_qTcNP3Vra3oZtUd4RAR3aXmyMqCZIZ3wrF8p_QE,20961
+cads_sdk/nosql/codec.py,sha256=OShyfDDuWxxFwts-1bHvAFxEhMDtPxjPlXBaHajZUQM,11250
+cads_sdk/nosql/converter.py,sha256=euUAqh1AKrsH_2cR53rvI9IQ-pu2my3Osm-yGvIll3M,86993
+cads_sdk/nosql/display.py,sha256=3AbZKScDmeuN6IRJpuqELLY2r0c5IVmTEMiKdwt5pks,22061
 cads_sdk/nosql/etl.py,sha256=PWhXNWZyIFFEEvTIoUNuKK5cDqTy8A4FPn07BGMr0Vk,1187
 cads_sdk/nosql/utils.py,sha256=nQVGBLBx7mhIgLulY1_bUefBEOqHhZbht4jI9E9azuY,1291
 cads_sdk/petastorm/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cads_sdk/petastorm/dataset_metadata.py,sha256=3sXVulFmpZEJC7mM0cwEXBVmB-0TD-U746ltLcsqIno,19967
 cads_sdk/petastorm/fs_utils.py,sha256=qFAzfi_VM4Rr2mBW8JsgxPUojLFFQGZI93MpI4sL_Xo,10508
 cads_sdk/petastorm/utils.py,sha256=CyeRPL_ih9wC1BdElvf1VknF1lBdNvJxgldSiU1OkFs,5427
 cads_sdk/pytorch/__init__.py,sha256=qyLEDZ_2BXLQBqievSj4wg2h4EQf9AdbIi_1SKFyIsM,22554
 cads_sdk/pytorch/codec.py,sha256=5XZulM21El-lsL3jZMexnJAHc2cIeRZj721PMuPhsJU,10653
 cads_sdk/pytorch/converter.py,sha256=lT2c3ix8Q35TEOUdFzlQVIzf7GfRklomwrdfRaXcY7k,78369
-cads_sdk-0.0.26.dist-info/METADATA,sha256=t10vIrxsXhYZt0FD3P8CcVK64838n_HewHWAz1Wga8g,7123
-cads_sdk-0.0.26.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-cads_sdk-0.0.26.dist-info/top_level.txt,sha256=OaTWVG-YiGPwrATCivDFDqvFPPP_T6y0TYXz8dkujOU,9
-cads_sdk-0.0.26.dist-info/RECORD,,
+cads_sdk-0.0.27.dist-info/METADATA,sha256=1kkvflc8AYoAhyC_dn5DHM3IbfItrC19e7ZKtMRzCrs,7111
+cads_sdk-0.0.27.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+cads_sdk-0.0.27.dist-info/top_level.txt,sha256=OaTWVG-YiGPwrATCivDFDqvFPPP_T6y0TYXz8dkujOU,9
+cads_sdk-0.0.27.dist-info/RECORD,,
```

