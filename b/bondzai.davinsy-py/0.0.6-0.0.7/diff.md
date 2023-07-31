# Comparing `tmp/bondzai.davinsy-py-0.0.6.tar.gz` & `tmp/bondzai.davinsy-py-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bondzai.davinsy-py-0.0.6.tar", last modified: Tue Jul 11 18:21:52 2023, max compression
+gzip compressed data, was "bondzai.davinsy-py-0.0.7.tar", last modified: Mon Jul 31 12:27:48 2023, max compression
```

## Comparing `bondzai.davinsy-py-0.0.6.tar` & `bondzai.davinsy-py-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:21:52.695822 bondzai.davinsy-py-0.0.6/
--rw-r--r--   0 theo       (501) staff       (20)      547 2023-07-11 18:20:53.000000 bondzai.davinsy-py-0.0.6/NOTICE
--rw-r--r--   0 theo       (501) staff       (20)      491 2023-07-11 18:21:52.696174 bondzai.davinsy-py-0.0.6/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)       72 2023-07-11 18:20:53.000000 bondzai.davinsy-py-0.0.6/README.md
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:21:52.679568 bondzai.davinsy-py-0.0.6/bondzai/
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:21:52.689847 bondzai.davinsy-py-0.0.6/bondzai/davinsy_py/
--rw-r--r--   0 theo       (501) staff       (20)       24 2023-07-11 18:20:53.000000 bondzai.davinsy-py-0.0.6/bondzai/davinsy_py/__init__.py
--rw-r--r--   0 theo       (501) staff       (20)     3989 2023-07-11 18:20:53.000000 bondzai.davinsy-py-0.0.6/bondzai/davinsy_py/davinsy.py
--rw-r--r--   0 theo       (501) staff       (20)     7213 2023-07-11 18:20:53.000000 bondzai.davinsy-py-0.0.6/bondzai/davinsy_py/enums.py
--rw-r--r--   0 theo       (501) staff       (20)      333 2023-07-11 18:20:53.000000 bondzai.davinsy-py-0.0.6/bondzai/davinsy_py/logger.py
--rw-r--r--   0 theo       (501) staff       (20)    21765 2023-07-11 18:20:53.000000 bondzai.davinsy-py-0.0.6/bondzai/davinsy_py/model.py
--rw-r--r--   0 theo       (501) staff       (20)    24433 2023-07-11 18:20:53.000000 bondzai.davinsy-py-0.0.6/bondzai/davinsy_py/operations.py
--rw-r--r--   0 theo       (501) staff       (20)     3346 2023-07-11 18:20:53.000000 bondzai.davinsy-py-0.0.6/bondzai/davinsy_py/preproc.py
--rw-r--r--   0 theo       (501) staff       (20)     1034 2023-07-11 18:20:53.000000 bondzai.davinsy-py-0.0.6/bondzai/davinsy_py/utils.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:21:52.695258 bondzai.davinsy-py-0.0.6/bondzai.davinsy_py.egg-info/
--rw-r--r--   0 theo       (501) staff       (20)      491 2023-07-11 18:21:52.000000 bondzai.davinsy-py-0.0.6/bondzai.davinsy_py.egg-info/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)      591 2023-07-11 18:21:52.000000 bondzai.davinsy-py-0.0.6/bondzai.davinsy_py.egg-info/SOURCES.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-11 18:21:52.000000 bondzai.davinsy-py-0.0.6/bondzai.davinsy_py.egg-info/dependency_links.txt
--rw-r--r--   0 theo       (501) staff       (20)        8 2023-07-11 18:21:52.000000 bondzai.davinsy-py-0.0.6/bondzai.davinsy_py.egg-info/namespace_packages.txt
--rw-r--r--   0 theo       (501) staff       (20)       26 2023-07-11 18:21:52.000000 bondzai.davinsy-py-0.0.6/bondzai.davinsy_py.egg-info/requires.txt
--rw-r--r--   0 theo       (501) staff       (20)       13 2023-07-11 18:21:52.000000 bondzai.davinsy-py-0.0.6/bondzai.davinsy_py.egg-info/top_level.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-11 18:21:52.000000 bondzai.davinsy-py-0.0.6/bondzai.davinsy_py.egg-info/zip-safe
--rw-r--r--   0 theo       (501) staff       (20)       71 2023-07-11 18:20:53.000000 bondzai.davinsy-py-0.0.6/pyproject.toml
--rw-r--r--   0 theo       (501) staff       (20)      700 2023-07-11 18:21:52.698365 bondzai.davinsy-py-0.0.6/setup.cfg
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-31 12:27:48.192952 bondzai.davinsy-py-0.0.7/
+-rw-r--r--   0 theo       (501) staff       (20)      547 2023-07-31 12:26:27.000000 bondzai.davinsy-py-0.0.7/NOTICE
+-rw-r--r--   0 theo       (501) staff       (20)      491 2023-07-31 12:27:48.193110 bondzai.davinsy-py-0.0.7/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)       72 2023-07-31 12:26:27.000000 bondzai.davinsy-py-0.0.7/README.md
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-31 12:27:48.186174 bondzai.davinsy-py-0.0.7/bondzai/
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-31 12:27:48.190438 bondzai.davinsy-py-0.0.7/bondzai/davinsy_py/
+-rw-r--r--   0 theo       (501) staff       (20)       24 2023-07-31 12:27:38.000000 bondzai.davinsy-py-0.0.7/bondzai/davinsy_py/__init__.py
+-rw-r--r--   0 theo       (501) staff       (20)     3989 2023-07-31 12:26:27.000000 bondzai.davinsy-py-0.0.7/bondzai/davinsy_py/davinsy.py
+-rw-r--r--   0 theo       (501) staff       (20)     7572 2023-07-31 12:27:38.000000 bondzai.davinsy-py-0.0.7/bondzai/davinsy_py/enums.py
+-rw-r--r--   0 theo       (501) staff       (20)      333 2023-07-31 12:26:27.000000 bondzai.davinsy-py-0.0.7/bondzai/davinsy_py/logger.py
+-rw-r--r--   0 theo       (501) staff       (20)    21776 2023-07-31 12:27:38.000000 bondzai.davinsy-py-0.0.7/bondzai/davinsy_py/model.py
+-rw-r--r--   0 theo       (501) staff       (20)    26545 2023-07-31 12:27:38.000000 bondzai.davinsy-py-0.0.7/bondzai/davinsy_py/operations.py
+-rw-r--r--   0 theo       (501) staff       (20)     3346 2023-07-31 12:26:27.000000 bondzai.davinsy-py-0.0.7/bondzai/davinsy_py/preproc.py
+-rw-r--r--   0 theo       (501) staff       (20)     1034 2023-07-31 12:26:27.000000 bondzai.davinsy-py-0.0.7/bondzai/davinsy_py/utils.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-31 12:27:48.192695 bondzai.davinsy-py-0.0.7/bondzai.davinsy_py.egg-info/
+-rw-r--r--   0 theo       (501) staff       (20)      491 2023-07-31 12:27:48.000000 bondzai.davinsy-py-0.0.7/bondzai.davinsy_py.egg-info/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)      591 2023-07-31 12:27:48.000000 bondzai.davinsy-py-0.0.7/bondzai.davinsy_py.egg-info/SOURCES.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-31 12:27:48.000000 bondzai.davinsy-py-0.0.7/bondzai.davinsy_py.egg-info/dependency_links.txt
+-rw-r--r--   0 theo       (501) staff       (20)        8 2023-07-31 12:27:48.000000 bondzai.davinsy-py-0.0.7/bondzai.davinsy_py.egg-info/namespace_packages.txt
+-rw-r--r--   0 theo       (501) staff       (20)       26 2023-07-31 12:27:48.000000 bondzai.davinsy-py-0.0.7/bondzai.davinsy_py.egg-info/requires.txt
+-rw-r--r--   0 theo       (501) staff       (20)       13 2023-07-31 12:27:48.000000 bondzai.davinsy-py-0.0.7/bondzai.davinsy_py.egg-info/top_level.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-31 12:27:48.000000 bondzai.davinsy-py-0.0.7/bondzai.davinsy_py.egg-info/zip-safe
+-rw-r--r--   0 theo       (501) staff       (20)       71 2023-07-31 12:26:27.000000 bondzai.davinsy-py-0.0.7/pyproject.toml
+-rw-r--r--   0 theo       (501) staff       (20)      700 2023-07-31 12:27:48.193764 bondzai.davinsy-py-0.0.7/setup.cfg
```

### Comparing `bondzai.davinsy-py-0.0.6/NOTICE` & `bondzai.davinsy-py-0.0.7/NOTICE`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.6/bondzai/davinsy_py/davinsy.py` & `bondzai.davinsy-py-0.0.7/bondzai/davinsy_py/davinsy.py`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.6/bondzai/davinsy_py/enums.py` & `bondzai.davinsy-py-0.0.7/bondzai/davinsy_py/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 class EventOperationID(Enum):
     EVT_EXT_EXCEPTION = 0x00
     EVT_EXT_DATA_IN = 0x01
     EVT_EXT_CMD_STATUS = 0x100
     EVT_EXT_LOG = 0x101
     EVT_EXT_VM_RESULT = 0x200
     EVT_EXT_ASL_RESULT = 0x201
+    EVT_EXT_PROCESS_ACK = 0x210
     EVT_EXT_SET_MODE = 0x300
     EVT_EXT_CORRECTION = 0x301
     EVT_EXT_TRIGGER = 0x302
     EVT_EXT_CUSTOM_1 = 0xF00
     EVT_EXT_CUSTOM_2 = 0xF01
     EVT_EXT_CUSTOM_3 = 0xF02
     EVT_EXT_CUSTOM_4 = 0xF03
@@ -78,35 +79,40 @@
     APP_AI_TYPE_CLASSIFICATION = 0
     APP_AI_TYPE_REGRESSION = 1
 
 
 class PPOperationUID(Enum):
     OPS_ID_EXT = 0x80000000
     OPS_ID = 0x00000000
+    OP_CUST_MIN = OPS_ID_EXT
+    OP_CUST_FIRST = 0x80000100
     OPS_MISC = 0x00000000
     OPS_MATH = 0x01000000
     OPS_DSP = 0x02000000
     OPS_IMG = 0x03000000
     OPS_STR = 0x04000000
     OPS_DBM = 0x05000000
     OPS_PST = 0x0E000000
     OPS_DIST = 0x0F000000
-    OPS_UID_NOP = 0x00
-    OPS_UID_NOPEND = 0x01
     OPS_UID_CP1D = 0x02
     OPS_UID_CP2D = 0x03
     OPS_UID_CP2X1D = 0x04
     OPS_UID_RMNFIRST1D_F32 = 0x05
     OPS_UID_LOGANF32 = 0x1000001
     OPS_UID_LOGA10F32 = 0x1000002
     OPS_UID_MEANF32 = 0x1000011
     OPS_UID_VARF32 = 0x1000012
     OPS_UID_RESHAPEF32 = 0x1000013
     OPS_UID_HISTOGRAMF32 = 0x1000014
-    OPS_UID_SLICEF32 = 0x1000015
+    OPS_UID_VECTORMATRIX_PRODUCTF32 = 0x1000015
+    OPS_UID_FLATTENMATRIXF32 = 0x1000016
+    OPS_UID_TRANSPOSEMATRIXF32 = 0x1000017
+    OPS_UID_SLICEF32 = 0x1000018
+    OPS_UID_SLICEMATRIXROWSF32 = 0x1000019
+    OPS_UID_SLICEMATRIXCOLSF32 = 0x100001A
     OPS_UID_FFT2048F32 = 0x2000011
     OPS_UID_FFT1024F32 = 0x2000012
     OPS_UID_FFT16F32 = 0x2000018
     OPS_UID_MFCC2048F32 = 0x2000019
     OPS_UID_MFCC1024F32 = 0x200001A
     OPS_UID_MEL2048F32 = 0x2000021
     OPS_UID_MEL1024F32 = 0x2000022
@@ -114,14 +120,16 @@
     OPS_UID_DCT2048F32 = 0x2000031
     OPS_UID_DCT1024F32 = 0x2000032
     OPS_UID_DCT512F32 = 0x2000033
     OPS_UID_DCT256F32 = 0x2000034
     OPS_UID_DCT128F32 = 0x2000035
     OPS_UID_NOISEMIXF32 = 0x2000061
     OPS_UID_PWSPANF32 = 0x2000062
+    OPS_UID_DCT2D = 0x3000001
+    OPS_UID_RGB_TO_GRAYF32 = 0x3000002
     OPS_UID_PUSHSIG2DBM = 0x5000001
     OPS_UID_PST_BYPASS = 0xE000001
     OPS_UID_PST_EXT = 0x8E000001
 
 
 class CommandOperationID(Enum):
     CMD_OPEN_SESSION = 0x00
@@ -162,14 +170,15 @@
     DBM_IMPORT_ROW = 0x201
     DBM_DELETE_ROW = 0x202
     DBM_CHECK_POINT = 0x300
     DBM_RESTORE = 0x301
     DBM_DEL_CHECK_POINT = 0x302
     DBM_GET_CHECK_POINT = 0x303
     DBM_CREATE_TABLE = 0x400
+    DBM_DELETE_TABLE = 0x401
 
 
 class DBMTable(Enum):
     DBM_VM = 0x00
     DBM_LBL = 0x01
     DBM_DAT = 0x02
     DBM_KEY = 0x03
```

### Comparing `bondzai.davinsy-py-0.0.6/bondzai/davinsy_py/model.py` & `bondzai.davinsy-py-0.0.7/bondzai/davinsy_py/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -485,15 +485,15 @@
                     nb_next=len(n["next"]),
                     next=(14 * c_ubyte)(*n["next"]),
                     parameters=fill_params(self.defaultData, n["parameters"])
                 )
                 for n in preproc["nodes"]])
         )
 
-        self._update_graph_sizes(graph)
+        # self._update_graph_sizes(graph) # LEGACY
         return graph
     def get_C_preproc_size(self, phase):
         
         size = 0
 
         if not phase in self.model["preprocess"]:
             phaselist = self.model["preprocess"].keys()
```

### Comparing `bondzai.davinsy-py-0.0.6/bondzai/davinsy_py/operations.py` & `bondzai.davinsy-py-0.0.7/bondzai/davinsy_py/operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -222,14 +222,34 @@
     return CPARAM_SHAPE
 
 def CPARAM_SHAPE_to_pyDict(param):
 
     structheader = CPARAM_SHAPE_factory().from_address(param)
     return structheader
 
+# CPARAM_SLICE
+class CPARAM_SLICE(Structure):
+    _fields_ = [
+        ("typeid", c_uint),
+        ("size", c_uint),
+        ("start", c_int),
+        ("stop", c_int),
+    ]
+    def check_node(self):
+        return True
+    
+def CPARAM_SLICE_factory():
+
+    return CPARAM_SLICE
+
+def CPARAM_SLICE_to_pyDict(param):
+
+    structheader = CPARAM_SLICE_factory().from_address(param)
+    return structheader
+
 # CPARAMSPECTRUM
 class CPARAMSPECTRUM(Structure):
     _fields_ = [
         ("typeid", c_uint),
         ("size", c_uint),
         ("mode", c_uint),
         ("wintype", c_uint),
@@ -369,32 +389,57 @@
     def get_temp_len(self, previous, op_uid):
         return 0
 
     def check_node(self):
         return True
 
 
+# CPARAM_HIST
+class CPARAM_HIST(Structure):
+    _fields_ = [
+        ("typeid", c_uint),
+        ("size", c_uint),
+        ("mode", c_uint),
+        ("nbbins", c_uint),
+        ("min", c_float),
+        ("max", c_float),
+    ]    
+    def check_node(self):
+        return True
+    
+def CPARAM_HIST_factory():
+
+    return CPARAM_HIST
+
+def CPARAM_HIST_to_pyDict(param):
+
+    structheader = CPARAM_HIST_factory().from_address(param)
+    return structheader
+
+
 class CALLPARAMS(Union):
     _fields_ = [
         ("param", CPARAM),
         ("param_mel", CPARAMMEL),
         ("param_dct", CPARAMDCT),
         ("param_mfcc", CPARAMMFCC),
         ("param_noisemix", CPARAMNOISEMIX),
         ("param_pwspan", CPARAMSPAN),
         ("param_mode", CPARAMMODE),
         ("param_dct2d", CPARAMDCT2D),
         ("param_compress", CPARAM_COMPRESS),
-        ("param_shape", CPARAM_SHAPE)
+        ("param_shape", CPARAM_SHAPE),
+        ("param_slice", CPARAM_SLICE),
+        ("param_hist", CPARAM_HIST)
     ]
 
 
 def fill_params(defaultData, parameters):
     if parameters["typeid"] == PPParam.OP_PARAM_MFCC.value:
-        logger.info("Setting MFCC params", parameters)
+        logger.debug("Setting MFCC params", parameters)
 
         if parameters["nmfcc"] > 127:
             raise RuntimeError(f"WARNING n MFCC too high {parameters['nmfcc']}, max value is 127")
 
         res = CALLPARAMS(
             param_mfcc=CPARAMMFCC(
                 typeid=parameters["typeid"],
@@ -438,77 +483,105 @@
                 _=(c_float * MAX_PARAM_DATA_SIZE_VECTOR2DF32)(*parameters["span_data"])
             )
         )
         # res.param_pwspan.span.data = cast(pointer(res.param_pwspan.span._), c_void_p)
         if not res.param_pwspan.check_node():
             logger.warn("Node : Parameters inconsistency in pwspan")
     elif parameters["typeid"] == PPParam.OP_PARAM_NOISEMIX.value:
-        logger.info("Setting NoiseMix params", parameters)
+        logger.debug("Setting NoiseMix params", parameters)
         res = CALLPARAMS(
             param_noisemix=CPARAMNOISEMIX(
                 typeid=parameters["typeid"],
                 size=parameters["size"],
                 mode=parameters["mode"],
                 snr=parameters["snr"],
                 option=parameters["option"]
             )
         )
         if not res.param_noisemix.check_node():
             logger.warn("Node : Parameters inconsistency in NoiseMix")
     elif parameters["typeid"] == PPParam.OP_PARAM_MODE.value:
-        logger.info("Setting param_mode params", parameters)
+        logger.debug("Setting param_mode params", parameters)
         res = CALLPARAMS(
             param_mode=CPARAMMODE(
                 typeid=parameters["typeid"],
                 size=parameters["size"],
                 mode=parameters["mode"]
             )
         )
         if not res.param_mode.check_node():
             logger.warn("Node : Parameters inconsistency in param_mode")
     elif parameters["typeid"] == PPParam.OP_PARAM_DCT_2D.value:
-        logger.info(f"Setting param_dct2d params  {parameters}")
+        logger.debug(f"Setting param_dct2d params  {parameters}")
         res = CALLPARAMS(
             param_dct2d=CPARAMDCT2D(
                 typeid=parameters["typeid"],
                 size=parameters["size"],
                 dct_length=parameters["dct_length"],
                 width=parameters["width"],
                 skipfirst=parameters["skipfirst"]
             )
         )
         if not res.param_mode.check_node():
             logger.warn("Node : Parameters inconsistency in param_dct2d")
     elif parameters["typeid"] == PPParam.OP_PARAM_COMPRESS.value:
-        logger.info("Setting OP_PARAM_COMPRESS params", parameters)
+        logger.debug("Setting OP_PARAM_COMPRESS params", parameters)
         res = CALLPARAMS(
             param_compress=CPARAM_COMPRESS(
                 typeid=parameters["typeid"],
                 size=parameters["size"],
                 dimIn=parameters["dimIn"],
                 dimOut=parameters["dimOut"],
             )
         )
         if not res.param_compress.check_node():
             logger.warn("Node : Parameters inconsistency in param_compress")
 
     elif parameters["typeid"] == PPParam.OP_PARAM_SHAPE.value:
-        logger.info("Setting CPARAM_SHAPE params", parameters)
+        logger.debug("Setting CPARAM_SHAPE params", parameters)
         res = CALLPARAMS(
             param_shape=CPARAM_SHAPE(
                 typeid=parameters["typeid"],
                 size=parameters["size"],
                 nbrows=parameters["nbrows"],
                 nbcols=parameters["nbcols"],
             )
         )
         if not res.param_shape.check_node():
-            logger.warn("Node : Parameters inconsistency in param_compress")
+            logger.warn("Node : Parameters inconsistency in param shape")
+    elif parameters["typeid"] == PPParam.OP_PARAM_SLICE.value:
+        logger.debug("Setting CPARAM_SLICE params", parameters)
+        res = CALLPARAMS(
+            param_shape=CPARAM_SLICE(
+                typeid=parameters["typeid"],
+                size=parameters["size"],
+                start=parameters["start"],
+                stop=parameters["stop"],
+            )
+        )
+        if not res.param_shape.check_node():
+            logger.warn("Node : Parameters inconsistency in param slice")
+    elif parameters["typeid"] == PPParam.OP_PARAM_HIST.value:
+        logger.debug("Setting CPARAM_HIST params", parameters)
+        res = CALLPARAMS(
+            param_hist=CPARAM_HIST(
+                typeid=parameters["typeid"],
+                size=parameters["size"],
+                mode=parameters["mode"],
+                nbbins=parameters["nbbins"], # a.k.a nbbins
+                min=parameters["min"],
+                max=parameters["max"],
+            )
+        )
+        if not res.param_hist.check_node():
+            logger.warn("Node : Parameters inconsistency in param slice")
+
+
     else:
-        raise RuntimeError("Unknown param type: %08x" % parameters["typeid"])
+        raise RuntimeError("Unknown param type: 0x%08x" % parameters["typeid"])
 
     return res
 
 
 class CUST_OP(Enum):
     OP_INIT_FILE_DLM = 0x80000000
     OP_INIT_FILE_PST = 0x80000001
```

### Comparing `bondzai.davinsy-py-0.0.6/bondzai/davinsy_py/preproc.py` & `bondzai.davinsy-py-0.0.7/bondzai/davinsy_py/preproc.py`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.6/bondzai/davinsy_py/utils.py` & `bondzai.davinsy-py-0.0.7/bondzai/davinsy_py/utils.py`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.6/bondzai.davinsy_py.egg-info/SOURCES.txt` & `bondzai.davinsy-py-0.0.7/bondzai.davinsy_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bondzai.davinsy-py-0.0.6/setup.cfg` & `bondzai.davinsy-py-0.0.7/setup.cfg`

 * *Files identical despite different names*

