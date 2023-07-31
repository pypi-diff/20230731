# Comparing `tmp/nvidia_nvml_dev_cu12-12.2.128-py3-none-manylinux1_x86_64.whl.zip` & `tmp/nvidia_nvml_dev_cu12-12.2.81-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 96846 bytes, number of entries: 9
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 10:21 nvidia/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 10:21 nvidia/nvml_dev/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 10:21 nvidia/nvml_dev/include/__init__.py
--rw-r--r--  2.0 unx   535670 b- defN 23-Jul-11 10:21 nvidia/nvml_dev/include/nvml.h
--rw-r--r--  2.0 unx    59262 b- defN 23-Jul-11 10:21 nvidia_nvml_dev_cu12-12.2.128.dist-info/License.txt
--rw-r--r--  2.0 unx     1505 b- defN 23-Jul-11 10:21 nvidia_nvml_dev_cu12-12.2.128.dist-info/METADATA
--rw-r--r--  2.0 unx      106 b- defN 23-Jul-11 10:21 nvidia_nvml_dev_cu12-12.2.128.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Jul-11 10:21 nvidia_nvml_dev_cu12-12.2.128.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      802 b- defN 23-Jul-11 10:21 nvidia_nvml_dev_cu12-12.2.128.dist-info/RECORD
-9 files, 597352 bytes uncompressed, 95434 bytes compressed:  84.0%
+Zip file size: 111462 bytes, number of entries: 10
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 05:12 nvidia/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 05:12 nvidia/nvml_dev/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 05:12 nvidia/nvml_dev/include/__init__.py
+-rw-r--r--  2.0 unx   535622 b- defN 23-Jun-02 05:12 nvidia/nvml_dev/include/nvml.h
+-rw-r--r--  2.0 unx    89192 b- defN 23-Jun-02 05:12 nvidia/nvml_dev/lib/x64/nvml.lib
+-rw-r--r--  2.0 unx    59262 b- defN 23-Jun-02 05:12 nvidia_nvml_dev_cu12-12.2.81.dist-info/License.txt
+-rw-r--r--  2.0 unx     1504 b- defN 23-Jun-02 05:12 nvidia_nvml_dev_cu12-12.2.81.dist-info/METADATA
+-rw-r--r--  2.0 unx       98 b- defN 23-Jun-02 05:12 nvidia_nvml_dev_cu12-12.2.81.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-02 05:12 nvidia_nvml_dev_cu12-12.2.81.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      886 b- defN 23-Jun-02 05:12 nvidia_nvml_dev_cu12-12.2.81.dist-info/RECORD
+10 files, 686571 bytes uncompressed, 109920 bytes compressed:  84.0%
```

## zipnote {}

```diff
@@ -6,23 +6,26 @@
 
 Filename: nvidia/nvml_dev/include/__init__.py
 Comment: 
 
 Filename: nvidia/nvml_dev/include/nvml.h
 Comment: 
 
-Filename: nvidia_nvml_dev_cu12-12.2.128.dist-info/License.txt
+Filename: nvidia/nvml_dev/lib/x64/nvml.lib
 Comment: 
 
-Filename: nvidia_nvml_dev_cu12-12.2.128.dist-info/METADATA
+Filename: nvidia_nvml_dev_cu12-12.2.81.dist-info/License.txt
 Comment: 
 
-Filename: nvidia_nvml_dev_cu12-12.2.128.dist-info/WHEEL
+Filename: nvidia_nvml_dev_cu12-12.2.81.dist-info/METADATA
 Comment: 
 
-Filename: nvidia_nvml_dev_cu12-12.2.128.dist-info/top_level.txt
+Filename: nvidia_nvml_dev_cu12-12.2.81.dist-info/WHEEL
 Comment: 
 
-Filename: nvidia_nvml_dev_cu12-12.2.128.dist-info/RECORD
+Filename: nvidia_nvml_dev_cu12-12.2.81.dist-info/top_level.txt
+Comment: 
+
+Filename: nvidia_nvml_dev_cu12-12.2.81.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nvidia/nvml_dev/include/nvml.h

```diff
@@ -2327,17 +2327,16 @@
 /** @defgroup nvmlSystem/nvmlDevice definitions related to Confidential Computing
  *  @{
  */
 /***************************************************************************************************/
 /**
  * Confidential Compute CPU Capabilities values
  */
-#define NVML_CC_SYSTEM_CPU_CAPS_NONE      0
-#define NVML_CC_SYSTEM_CPU_CAPS_AMD_SEV   1
-#define NVML_CC_SYSTEM_CPU_CAPS_INTEL_TDX 2
+#define NVML_CC_SYSTEM_CPU_CAPS_NONE    0
+#define NVML_CC_SYSTEM_CPU_CAPS_AMD_SEV 1
 
 /**
  * Confidenial Compute GPU Capabilities values
  */
 #define NVML_CC_SYSTEM_GPUS_CC_NOT_CAPABLE 0
 #define NVML_CC_SYSTEM_GPUS_CC_CAPABLE     1
```

## Comparing `nvidia_nvml_dev_cu12-12.2.128.dist-info/License.txt` & `nvidia_nvml_dev_cu12-12.2.81.dist-info/License.txt`

 * *Files identical despite different names*

## Comparing `nvidia_nvml_dev_cu12-12.2.128.dist-info/METADATA` & `nvidia_nvml_dev_cu12-12.2.81.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-nvml-dev-cu12
-Version: 12.2.128
+Version: 12.2.81
 Summary: NVML native dev links, headers
 Home-page: https://developer.nvidia.com/cuda-zone
 Author: Nvidia CUDA Installer Team
 Author-email: cuda_installer@nvidia.com
 License: NVIDIA Proprietary Software
 Keywords: cuda,nvidia,runtime,machine learning,deep learning
 Classifier: Development Status :: 4 - Beta
```

## Comparing `nvidia_nvml_dev_cu12-12.2.128.dist-info/RECORD` & `nvidia_nvml_dev_cu12-12.2.81.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 nvidia/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nvidia/nvml_dev/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nvidia/nvml_dev/include/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-nvidia/nvml_dev/include/nvml.h,sha256=VSSFQZsOlU1aYJ5aX0TrLBZuxWquBYf_1EWUQbp54K4,535670
-nvidia_nvml_dev_cu12-12.2.128.dist-info/License.txt,sha256=rW9YU_ugyg0VnQ9Y1JrkmDDC-Mk_epJki5zpCttMbM0,59262
-nvidia_nvml_dev_cu12-12.2.128.dist-info/METADATA,sha256=9nP9I9W51GHR6Usd_ciPDh3IW8KM0HlBty98Or9_P9U,1505
-nvidia_nvml_dev_cu12-12.2.128.dist-info/WHEEL,sha256=-kQi_VMfvRQozZJT7HUPMfY-5vLo0LVTmAylNJ3Ft98,106
-nvidia_nvml_dev_cu12-12.2.128.dist-info/top_level.txt,sha256=fTkAtiFuL16nUrB9ytDDtpytz2t0B4NvYTnRzwAhO14,7
-nvidia_nvml_dev_cu12-12.2.128.dist-info/RECORD,,
+nvidia/nvml_dev/include/nvml.h,sha256=qN0EXxg9v3MknRMFepwCCQeBzJ02SrJ1fucLzqpvUmE,535622
+nvidia/nvml_dev/lib/x64/nvml.lib,sha256=cELqtgnpEs75n-oWinJgO7Oadlhwhy_pLvgLd6Yhtgw,89192
+nvidia_nvml_dev_cu12-12.2.81.dist-info/License.txt,sha256=rW9YU_ugyg0VnQ9Y1JrkmDDC-Mk_epJki5zpCttMbM0,59262
+nvidia_nvml_dev_cu12-12.2.81.dist-info/METADATA,sha256=xQcH-aWGv7KuD6sf2dwC488NOG74KTIjDqRWX9wEA3Y,1504
+nvidia_nvml_dev_cu12-12.2.81.dist-info/WHEEL,sha256=i9qQj8KaD8_YEW0Vc2oS56fKju23RkQ-FVz-QmzVakQ,98
+nvidia_nvml_dev_cu12-12.2.81.dist-info/top_level.txt,sha256=fTkAtiFuL16nUrB9ytDDtpytz2t0B4NvYTnRzwAhO14,7
+nvidia_nvml_dev_cu12-12.2.81.dist-info/RECORD,,
```

