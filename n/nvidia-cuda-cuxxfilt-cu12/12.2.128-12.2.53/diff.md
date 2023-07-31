# Comparing `tmp/nvidia_cuda_cuxxfilt_cu12-12.2.128-py3-none-manylinux1_x86_64.whl.zip` & `tmp/nvidia_cuda_cuxxfilt_cu12-12.2.53-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 17630 bytes, number of entries: 9
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 10:19 nvidia/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 10:19 nvidia/cuda_cuxxfilt/__init__.py
--rw-r--r--  2.0 unx     1912 b- defN 23-Jul-11 10:19 nvidia/cuda_cuxxfilt/include/nv_decode.h
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 10:19 nvidia/cuda_cuxxfilt/lib/__init__.py
--rw-r--r--  2.0 unx    59262 b- defN 23-Jul-11 10:19 nvidia_cuda_cuxxfilt_cu12-12.2.128.dist-info/License.txt
--rw-r--r--  2.0 unx     1730 b- defN 23-Jul-11 10:19 nvidia_cuda_cuxxfilt_cu12-12.2.128.dist-info/METADATA
--rw-r--r--  2.0 unx      106 b- defN 23-Jul-11 10:19 nvidia_cuda_cuxxfilt_cu12-12.2.128.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Jul-11 10:19 nvidia_cuda_cuxxfilt_cu12-12.2.128.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      841 b- defN 23-Jul-11 10:19 nvidia_cuda_cuxxfilt_cu12-12.2.128.dist-info/RECORD
-9 files, 63858 bytes uncompressed, 16136 bytes compressed:  74.7%
+Zip file size: 67326 bytes, number of entries: 9
+-rw-r--r--  2.0 unx        0 b- defN 23-May-01 02:56 nvidia/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-01 02:56 nvidia/cuda_cuxxfilt/__init__.py
+-rw-r--r--  2.0 unx     1970 b- defN 23-May-01 02:56 nvidia/cuda_cuxxfilt/include/nv_decode.h
+-rw-r--r--  2.0 unx   155384 b- defN 23-May-01 02:56 nvidia/cuda_cuxxfilt/lib/x64/cufilt.lib
+-rw-r--r--  2.0 unx    59262 b- defN 23-May-01 02:56 nvidia_cuda_cuxxfilt_cu12-12.2.53.dist-info/License.txt
+-rw-r--r--  2.0 unx     1729 b- defN 23-May-01 02:56 nvidia_cuda_cuxxfilt_cu12-12.2.53.dist-info/METADATA
+-rw-r--r--  2.0 unx       98 b- defN 23-May-01 02:56 nvidia_cuda_cuxxfilt_cu12-12.2.53.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-May-01 02:56 nvidia_cuda_cuxxfilt_cu12-12.2.53.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      843 b- defN 23-May-01 02:56 nvidia_cuda_cuxxfilt_cu12-12.2.53.dist-info/RECORD
+9 files, 219293 bytes uncompressed, 65836 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: nvidia/cuda_cuxxfilt/__init__.py
 Comment: 
 
 Filename: nvidia/cuda_cuxxfilt/include/nv_decode.h
 Comment: 
 
-Filename: nvidia/cuda_cuxxfilt/lib/__init__.py
+Filename: nvidia/cuda_cuxxfilt/lib/x64/cufilt.lib
 Comment: 
 
-Filename: nvidia_cuda_cuxxfilt_cu12-12.2.128.dist-info/License.txt
+Filename: nvidia_cuda_cuxxfilt_cu12-12.2.53.dist-info/License.txt
 Comment: 
 
-Filename: nvidia_cuda_cuxxfilt_cu12-12.2.128.dist-info/METADATA
+Filename: nvidia_cuda_cuxxfilt_cu12-12.2.53.dist-info/METADATA
 Comment: 
 
-Filename: nvidia_cuda_cuxxfilt_cu12-12.2.128.dist-info/WHEEL
+Filename: nvidia_cuda_cuxxfilt_cu12-12.2.53.dist-info/WHEEL
 Comment: 
 
-Filename: nvidia_cuda_cuxxfilt_cu12-12.2.128.dist-info/top_level.txt
+Filename: nvidia_cuda_cuxxfilt_cu12-12.2.53.dist-info/top_level.txt
 Comment: 
 
-Filename: nvidia_cuda_cuxxfilt_cu12-12.2.128.dist-info/RECORD
+Filename: nvidia_cuda_cuxxfilt_cu12-12.2.53.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nvidia/cuda_cuxxfilt/include/nv_decode.h

 * *Ordering differences only*

```diff
@@ -1,58 +1,58 @@
-/*
- * NVIDIA_COPYRIGHT_BEGIN
- *
- * Copyright (c) 2021, NVIDIA CORPORATION.  All rights reserved.
- *
- * NVIDIA_COPYRIGHT_END
- */
-
-/*
-nv_decode.h -- API for the CUDA C++ name demangler.
-*/
-
-/* Avoid including these declarations more than once: */
-#ifndef DECODE_H
-#define DECODE_H 1
-
-#ifdef __cplusplus
-extern "C" {
-#endif
-
-/* Cuda C++ demangling API.
-
-   Parameters:
-     id: Input mangled string
-     output_buffer: Pointer to where the demangled buffer will
-                    be stored. This memory must be allocated with malloc.
-                    If output-buffer is NULL, memory will be malloc'd to
-                    store the demangled name and returned through the 
-                    function return value.
-                    If the output-buffer is too small, it is expanded using
-                    realloc.
-     length: It is necessary to provide the size of the output buffer if the user
-             is providing pre-allocated memory. This is needed by the demangler 
-             in case the size needs to be reallocated.
-             If the length is non-null, the length of the demangled buffer
-             is placed in length.
-     status: *status is set to one of the following values. 0 - The
-             demangling operation succeeded; -1 - A memory allocation
-             failure occurred. -2 - Not a valid mangled id. -3 - An
-             input validation failure has occurred (one or more
-             arguments are invalid).
-
-   Return Value: A pointer to the start of the NUL-terminated demangled name,
-                 or NULL if the demangling fails. The caller is responsible for
-                 deallocating this memory using free.
-
-   Note: This function is thread-safe.
-*/
-
-char* __cu_demangle(const char *id,
-	                char *output_buffer,
-	                size_t *length,
-	                int *status);
-
-#ifdef __cplusplus
-}
-#endif
-#endif /* ifndef DECODE_H */
+/*
+ * NVIDIA_COPYRIGHT_BEGIN
+ *
+ * Copyright (c) 2021, NVIDIA CORPORATION.  All rights reserved.
+ *
+ * NVIDIA_COPYRIGHT_END
+ */
+
+/*
+nv_decode.h -- API for the CUDA C++ name demangler.
+*/
+
+/* Avoid including these declarations more than once: */
+#ifndef DECODE_H
+#define DECODE_H 1
+
+#ifdef __cplusplus
+extern "C" {
+#endif
+
+/* Cuda C++ demangling API.
+
+   Parameters:
+     id: Input mangled string
+     output_buffer: Pointer to where the demangled buffer will
+                    be stored. This memory must be allocated with malloc.
+                    If output-buffer is NULL, memory will be malloc'd to
+                    store the demangled name and returned through the 
+                    function return value.
+                    If the output-buffer is too small, it is expanded using
+                    realloc.
+     length: It is necessary to provide the size of the output buffer if the user
+             is providing pre-allocated memory. This is needed by the demangler 
+             in case the size needs to be reallocated.
+             If the length is non-null, the length of the demangled buffer
+             is placed in length.
+     status: *status is set to one of the following values. 0 - The
+             demangling operation succeeded; -1 - A memory allocation
+             failure occurred. -2 - Not a valid mangled id. -3 - An
+             input validation failure has occurred (one or more
+             arguments are invalid).
+
+   Return Value: A pointer to the start of the NUL-terminated demangled name,
+                 or NULL if the demangling fails. The caller is responsible for
+                 deallocating this memory using free.
+
+   Note: This function is thread-safe.
+*/
+
+char* __cu_demangle(const char *id,
+	                char *output_buffer,
+	                size_t *length,
+	                int *status);
+
+#ifdef __cplusplus
+}
+#endif
+#endif /* ifndef DECODE_H */
```

## Comparing `nvidia_cuda_cuxxfilt_cu12-12.2.128.dist-info/License.txt` & `nvidia_cuda_cuxxfilt_cu12-12.2.53.dist-info/License.txt`

 * *Files identical despite different names*

## Comparing `nvidia_cuda_cuxxfilt_cu12-12.2.128.dist-info/METADATA` & `nvidia_cuda_cuxxfilt_cu12-12.2.53.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-cuda-cuxxfilt-cu12
-Version: 12.2.128
+Version: 12.2.53
 Summary: CUDA cuxxfilt
 Home-page: https://developer.nvidia.com/cuda-zone
 Author: Nvidia CUDA Installer Team
 Author-email: cuda_installer@nvidia.com
 License: NVIDIA Proprietary Software
 Keywords: cuda,nvidia,runtime,machine learning,deep learning
 Classifier: Development Status :: 4 - Beta
```

