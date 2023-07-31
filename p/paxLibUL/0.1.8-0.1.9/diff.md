# Comparing `tmp/paxLibUL-0.1.8.tar.gz` & `tmp/paxLibUL-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paxLibUL-0.1.8.tar", last modified: Wed Apr 13 15:26:38 2022, max compression
+gzip compressed data, was "paxLibUL-0.1.9.tar", last modified: Wed Apr 13 15:40:00 2022, max compression
```

## Comparing `paxLibUL-0.1.8.tar` & `paxLibUL-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 15:26:38.951431 paxLibUL-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1060 2022-04-13 15:26:28.000000 paxLibUL-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-04-13 15:26:38.955431 paxLibUL-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-04-13 15:26:28.000000 paxLibUL-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 15:26:38.951431 paxLibUL-0.1.8/paxLibUL/
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-04-13 15:26:28.000000 paxLibUL-0.1.8/paxLibUL/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 15:26:38.951431 paxLibUL-0.1.8/paxLibUL/convolution/
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-04-13 15:26:28.000000 paxLibUL-0.1.8/paxLibUL/convolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8898 2022-04-13 15:26:28.000000 paxLibUL-0.1.8/paxLibUL/convolution/architectures.py
--rw-r--r--   0 runner    (1001) docker     (121)      358 2022-04-13 15:26:28.000000 paxLibUL-0.1.8/paxLibUL/convolution/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (121)     2737 2022-04-13 15:26:28.000000 paxLibUL-0.1.8/paxLibUL/convolution/datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)     8800 2022-04-13 15:26:28.000000 paxLibUL-0.1.8/paxLibUL/convolution/visualisation.py
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-04-13 15:26:28.000000 paxLibUL-0.1.8/paxLibUL/convolution/weights_init.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 15:26:38.951431 paxLibUL-0.1.8/paxLibUL/nlp/
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-04-13 15:26:28.000000 paxLibUL-0.1.8/paxLibUL/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2186 2022-04-13 15:26:28.000000 paxLibUL-0.1.8/paxLibUL/nlp/data_transformer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-04-13 15:26:28.000000 paxLibUL-0.1.8/paxLibUL/nlp/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-04-13 15:26:38.000000 paxLibUL-0.1.8/paxLibUL/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 15:26:38.951431 paxLibUL-0.1.8/paxLibUL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-04-13 15:26:38.000000 paxLibUL-0.1.8/paxLibUL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      547 2022-04-13 15:26:38.000000 paxLibUL-0.1.8/paxLibUL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-13 15:26:38.000000 paxLibUL-0.1.8/paxLibUL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-04-13 15:26:38.000000 paxLibUL-0.1.8/paxLibUL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-04-13 15:26:38.000000 paxLibUL-0.1.8/paxLibUL.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-04-13 15:26:28.000000 paxLibUL-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-04-13 15:26:38.955431 paxLibUL-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2662 2022-04-13 15:26:28.000000 paxLibUL-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 15:40:00.745426 paxLibUL-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1060 2022-04-13 15:39:48.000000 paxLibUL-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-04-13 15:40:00.745426 paxLibUL-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      218 2022-04-13 15:39:48.000000 paxLibUL-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 15:40:00.741426 paxLibUL-0.1.9/paxLibUL/
+-rw-r--r--   0 runner    (1001) docker     (121)       80 2022-04-13 15:39:48.000000 paxLibUL-0.1.9/paxLibUL/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 15:40:00.745426 paxLibUL-0.1.9/paxLibUL/convolution/
+-rw-r--r--   0 runner    (1001) docker     (121)      169 2022-04-13 15:39:48.000000 paxLibUL-0.1.9/paxLibUL/convolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8901 2022-04-13 15:39:48.000000 paxLibUL-0.1.9/paxLibUL/convolution/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (121)      358 2022-04-13 15:39:48.000000 paxLibUL-0.1.9/paxLibUL/convolution/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2737 2022-04-13 15:39:48.000000 paxLibUL-0.1.9/paxLibUL/convolution/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8800 2022-04-13 15:39:48.000000 paxLibUL-0.1.9/paxLibUL/convolution/visualisation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      295 2022-04-13 15:39:48.000000 paxLibUL-0.1.9/paxLibUL/convolution/weights_init.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 15:40:00.745426 paxLibUL-0.1.9/paxLibUL/nlp/
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2022-04-13 15:39:48.000000 paxLibUL-0.1.9/paxLibUL/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2186 2022-04-13 15:39:48.000000 paxLibUL-0.1.9/paxLibUL/nlp/data_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-04-13 15:39:48.000000 paxLibUL-0.1.9/paxLibUL/nlp/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-04-13 15:40:00.000000 paxLibUL-0.1.9/paxLibUL/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 15:40:00.741426 paxLibUL-0.1.9/paxLibUL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-04-13 15:40:00.000000 paxLibUL-0.1.9/paxLibUL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      547 2022-04-13 15:40:00.000000 paxLibUL-0.1.9/paxLibUL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-13 15:40:00.000000 paxLibUL-0.1.9/paxLibUL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2022-04-13 15:40:00.000000 paxLibUL-0.1.9/paxLibUL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-04-13 15:40:00.000000 paxLibUL-0.1.9/paxLibUL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      122 2022-04-13 15:39:48.000000 paxLibUL-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-04-13 15:40:00.745426 paxLibUL-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2662 2022-04-13 15:39:48.000000 paxLibUL-0.1.9/setup.py
```

### Comparing `paxLibUL-0.1.8/LICENSE` & `paxLibUL-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `paxLibUL-0.1.8/PKG-INFO` & `paxLibUL-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: paxLibUL
-Version: 0.1.8
+Version: 0.1.9
 Summary: A library for internal formation tools use in PaX ULaval formations.
 Home-page: https://pax.ulaval.ca/
 Author: PaX-UL
 License: LGPLv3
-Download-URL: https://github.com/PAX-ULaval/pax-libraries/archive/v0.1.8.zip
+Download-URL: https://github.com/PAX-ULaval/pax-libraries/archive/v0.1.9.zip
 Description: # A library for internal formation tools used in PaX ULaval formations
         Most of the content is to reduce code duplication into our formation and to ease the release of those tools among 
         the formations in the platform.
         
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `paxLibUL-0.1.8/paxLibUL/convolution/architectures.py` & `paxLibUL-0.1.9/paxLibUL/convolution/architectures.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import functools
+from functools import partial
 
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 
@@ -189,15 +189,15 @@
             outermost (bool): If this module is the outermost module.
             innermost (bool): If this module is the innermost module.
             norm_layer: Normalization layer.
             use_dropout (bool): If use dropout layers.
         """
         super().__init__()
         self.outermost = outermost
-        if type(norm_layer) == functools.partial:
+        if type(norm_layer) == partial:
             use_bias = norm_layer.func == nn.InstanceNorm2d
         else:
             use_bias = norm_layer == nn.InstanceNorm2d
         if input_nc is None:
             input_nc = outer_nc
         downconv = nn.Conv2d(input_nc, inner_nc, kernel_size=4, stride=2, padding=1, bias=use_bias)
         downrelu = nn.LeakyReLU(0.2, True)
```

### Comparing `paxLibUL-0.1.8/paxLibUL/convolution/datasets.py` & `paxLibUL-0.1.9/paxLibUL/convolution/datasets.py`

 * *Files identical despite different names*

### Comparing `paxLibUL-0.1.8/paxLibUL/convolution/visualisation.py` & `paxLibUL-0.1.9/paxLibUL/convolution/visualisation.py`

 * *Files identical despite different names*

### Comparing `paxLibUL-0.1.8/paxLibUL/nlp/data_transformer.py` & `paxLibUL-0.1.9/paxLibUL/nlp/data_transformer.py`

 * *Files identical despite different names*

### Comparing `paxLibUL-0.1.8/paxLibUL/nlp/evaluate.py` & `paxLibUL-0.1.9/paxLibUL/nlp/evaluate.py`

 * *Files identical despite different names*

### Comparing `paxLibUL-0.1.8/paxLibUL.egg-info/PKG-INFO` & `paxLibUL-0.1.9/paxLibUL.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: paxLibUL
-Version: 0.1.8
+Version: 0.1.9
 Summary: A library for internal formation tools use in PaX ULaval formations.
 Home-page: https://pax.ulaval.ca/
 Author: PaX-UL
 License: LGPLv3
-Download-URL: https://github.com/PAX-ULaval/pax-libraries/archive/v0.1.8.zip
+Download-URL: https://github.com/PAX-ULaval/pax-libraries/archive/v0.1.9.zip
 Description: # A library for internal formation tools used in PaX ULaval formations
         Most of the content is to reduce code duplication into our formation and to ease the release of those tools among 
         the formations in the platform.
         
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `paxLibUL-0.1.8/paxLibUL.egg-info/SOURCES.txt` & `paxLibUL-0.1.9/paxLibUL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paxLibUL-0.1.8/setup.py` & `paxLibUL-0.1.9/setup.py`

 * *Files identical despite different names*

