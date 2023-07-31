# Comparing `tmp/openai_parallel_toolkit-1.0.0-py3-none-any.whl.zip` & `tmp/openai_parallel_toolkit-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5560 bytes, number of entries: 7
+Zip file size: 6584 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       77 b- defN 23-Jul-28 11:58 openai_parallel_toolkit/__init__.py
--rw-r--r--  2.0 unx     2897 b- defN 23-Jul-28 12:53 openai_parallel_toolkit/main.py
--rw-r--r--  2.0 unx     1063 b- defN 23-Jul-28 12:54 openai_parallel_toolkit-1.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     6002 b- defN 23-Jul-28 12:54 openai_parallel_toolkit-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-28 12:54 openai_parallel_toolkit-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       24 b- defN 23-Jul-28 12:54 openai_parallel_toolkit-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      644 b- defN 23-Jul-28 12:54 openai_parallel_toolkit-1.0.0.dist-info/RECORD
-7 files, 10799 bytes uncompressed, 4396 bytes compressed:  59.3%
+-rw-r--r--  2.0 unx     3100 b- defN 23-Jul-31 02:05 openai_parallel_toolkit/main.py
+-rw-r--r--  2.0 unx     1063 b- defN 23-Jul-31 02:57 openai_parallel_toolkit-1.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8218 b- defN 23-Jul-31 02:57 openai_parallel_toolkit-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-31 02:57 openai_parallel_toolkit-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       24 b- defN 23-Jul-31 02:57 openai_parallel_toolkit-1.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      644 b- defN 23-Jul-31 02:57 openai_parallel_toolkit-1.1.0.dist-info/RECORD
+7 files, 13218 bytes uncompressed, 5420 bytes compressed:  59.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: openai_parallel_toolkit/__init__.py
 Comment: 
 
 Filename: openai_parallel_toolkit/main.py
 Comment: 
 
-Filename: openai_parallel_toolkit-1.0.0.dist-info/LICENSE
+Filename: openai_parallel_toolkit-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: openai_parallel_toolkit-1.0.0.dist-info/METADATA
+Filename: openai_parallel_toolkit-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: openai_parallel_toolkit-1.0.0.dist-info/WHEEL
+Filename: openai_parallel_toolkit-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: openai_parallel_toolkit-1.0.0.dist-info/top_level.txt
+Filename: openai_parallel_toolkit-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: openai_parallel_toolkit-1.0.0.dist-info/RECORD
+Filename: openai_parallel_toolkit-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openai_parallel_toolkit/main.py

```diff
@@ -1,17 +1,18 @@
 import logging
 import multiprocessing
-from typing import Dict, Type
+from typing import Dict
 
 from openai_parallel_toolkit.api.keys import KeyManager
 from openai_parallel_toolkit.api.model import OpenAIModel, Prompt
 from openai_parallel_toolkit.api.request import parallel_request_openai, request_openai_api
 from openai_parallel_toolkit.utils.logger import LOG_LABEL, Logger
-from openai_parallel_toolkit.utils.reader import filter, read_jsonl_to_dict, read_sort_write_jsonl
 from openai_parallel_toolkit.utils.process_bar import ProgressBar
+from openai_parallel_toolkit.utils.reader import filter, merge_jsonl_files, read_jsonl_to_dict, read_sort_write_jsonl, \
+    remove_nulls_from_jsonl
 
 
 class ParallelToolkit:
     def __init__(self,
                  config_path: str,
                  openai_model: OpenAIModel = OpenAIModel(),
                  input_path: str = None,
@@ -27,14 +28,15 @@
         self.threads = threads
         self.openai_model = openai_model
         self.name = name
         self.max_retries = max_retries
 
     def run(self):
         logging.warning(f"{LOG_LABEL}Data is being processed, waiting for the first returned result")
+        remove_nulls_from_jsonl(self.output_path)
         data = read_jsonl_to_dict(self.input_path)
         filtered_data = filter(data, self.output_path)
         if len(filtered_data) == 0:
             logging.warning(f"{LOG_LABEL}No data to process")
             return
         threads = min(len(filtered_data), self.threads, self.key_manager.get_key_length() // 2)
         threads = max(threads, 1)
@@ -51,7 +53,10 @@
 
     def parallel_api(self, data: Dict[int, Prompt]):
         logging.warning(f"{LOG_LABEL}Data is being processed, waiting for the first returned result")
         process_bar = ProgressBar(total=len(data), desc=self.name)
         return parallel_request_openai(data=data, openai_model=self.openai_model,
                                        key_manager=self.key_manager, threads=self.threads, max_retries=self.max_retries,
                                        process_bar=process_bar, output_path=self.output_path)
+
+    def merge(self, merged_file):
+        merge_jsonl_files(self.input_path, self.output_path, merged_file)
```

## Comparing `openai_parallel_toolkit-1.0.0.dist-info/LICENSE` & `openai_parallel_toolkit-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `openai_parallel_toolkit-1.0.0.dist-info/RECORD` & `openai_parallel_toolkit-1.1.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 openai_parallel_toolkit/__init__.py,sha256=ZZxiwZF7ASUBX-pVvy-lD2UMguKiuTxJpKlesjkiXYs,77
-openai_parallel_toolkit/main.py,sha256=4Cn6GsVfEICEG5Z-nBSCsWZ9Peupq_ov2oYtAgcyd_o,2897
-openai_parallel_toolkit-1.0.0.dist-info/LICENSE,sha256=GcBhJWMnrpUPC70Dvfs6cFG8fLIitA0WwucEgQjGWcw,1063
-openai_parallel_toolkit-1.0.0.dist-info/METADATA,sha256=BMkvHKdwWaq6eprqfm1e9bQhCgvFh15KueTKRX0Mb_0,6002
-openai_parallel_toolkit-1.0.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-openai_parallel_toolkit-1.0.0.dist-info/top_level.txt,sha256=EaHQWFuNRtse4G2kzDTEMstiiaGFy0zIAHBJ0Mm9a_E,24
-openai_parallel_toolkit-1.0.0.dist-info/RECORD,,
+openai_parallel_toolkit/main.py,sha256=tulufpdSmKdkMSw-N-RS_aYg9Dt7jxF0ZvsqPXOc1Kc,3100
+openai_parallel_toolkit-1.1.0.dist-info/LICENSE,sha256=GcBhJWMnrpUPC70Dvfs6cFG8fLIitA0WwucEgQjGWcw,1063
+openai_parallel_toolkit-1.1.0.dist-info/METADATA,sha256=4S0yBCUf9NGl9143roj9oT0YOuh8nQoqgC1k5DkIOR4,8218
+openai_parallel_toolkit-1.1.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+openai_parallel_toolkit-1.1.0.dist-info/top_level.txt,sha256=EaHQWFuNRtse4G2kzDTEMstiiaGFy0zIAHBJ0Mm9a_E,24
+openai_parallel_toolkit-1.1.0.dist-info/RECORD,,
```

