# Comparing `tmp/bondzai.validation-framework-0.0.2.tar.gz` & `tmp/bondzai.validation-framework-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bondzai.validation-framework-0.0.2.tar", last modified: Tue Jul 11 19:03:39 2023, max compression
+gzip compressed data, was "bondzai.validation-framework-0.0.3.tar", last modified: Mon Jul 31 12:29:24 2023, max compression
```

## Comparing `bondzai.validation-framework-0.0.2.tar` & `bondzai.validation-framework-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 19:03:39.087244 bondzai.validation-framework-0.0.2/
--rw-r--r--   0 theo       (501) staff       (20)      547 2023-07-11 19:03:04.000000 bondzai.validation-framework-0.0.2/NOTICE
--rw-r--r--   0 theo       (501) staff       (20)      567 2023-07-11 19:03:39.087345 bondzai.validation-framework-0.0.2/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)       97 2023-07-11 19:03:04.000000 bondzai.validation-framework-0.0.2/README.md
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 19:03:39.081330 bondzai.validation-framework-0.0.2/bondzai/
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 19:03:39.084702 bondzai.validation-framework-0.0.2/bondzai/validation_framework/
--rw-r--r--   0 theo       (501) staff       (20)       21 2023-07-11 19:03:04.000000 bondzai.validation-framework-0.0.2/bondzai/validation_framework/__init__.py
--rw-r--r--   0 theo       (501) staff       (20)     2913 2023-07-11 19:03:04.000000 bondzai.validation-framework-0.0.2/bondzai/validation_framework/connector_handler.py
--rw-r--r--   0 theo       (501) staff       (20)    10835 2023-07-11 19:03:04.000000 bondzai.validation-framework-0.0.2/bondzai/validation_framework/dataset_handler.py
--rw-r--r--   0 theo       (501) staff       (20)     9244 2023-07-11 19:03:04.000000 bondzai.validation-framework-0.0.2/bondzai/validation_framework/event_catcher.py
--rw-r--r--   0 theo       (501) staff       (20)     3540 2023-07-11 19:03:04.000000 bondzai.validation-framework-0.0.2/bondzai/validation_framework/log_handler.py
--rw-r--r--   0 theo       (501) staff       (20)     9752 2023-07-11 19:03:04.000000 bondzai.validation-framework-0.0.2/bondzai/validation_framework/result_handler.py
--rw-r--r--   0 theo       (501) staff       (20)     2028 2023-07-11 19:03:04.000000 bondzai.validation-framework-0.0.2/bondzai/validation_framework/tar_handler.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 19:03:39.087031 bondzai.validation-framework-0.0.2/bondzai.validation_framework.egg-info/
--rw-r--r--   0 theo       (501) staff       (20)      567 2023-07-11 19:03:39.000000 bondzai.validation-framework-0.0.2/bondzai.validation_framework.egg-info/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)      793 2023-07-11 19:03:39.000000 bondzai.validation-framework-0.0.2/bondzai.validation_framework.egg-info/SOURCES.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-11 19:03:39.000000 bondzai.validation-framework-0.0.2/bondzai.validation_framework.egg-info/dependency_links.txt
--rw-r--r--   0 theo       (501) staff       (20)        8 2023-07-11 19:03:39.000000 bondzai.validation-framework-0.0.2/bondzai.validation_framework.egg-info/namespace_packages.txt
--rw-r--r--   0 theo       (501) staff       (20)      134 2023-07-11 19:03:39.000000 bondzai.validation-framework-0.0.2/bondzai.validation_framework.egg-info/requires.txt
--rw-r--r--   0 theo       (501) staff       (20)       22 2023-07-11 19:03:39.000000 bondzai.validation-framework-0.0.2/bondzai.validation_framework.egg-info/top_level.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-11 19:03:38.000000 bondzai.validation-framework-0.0.2/bondzai.validation_framework.egg-info/zip-safe
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 19:03:39.085214 bondzai.validation-framework-0.0.2/examples/
--rw-r--r--   0 theo       (501) staff       (20)     5098 2023-07-11 19:03:04.000000 bondzai.validation-framework-0.0.2/examples/live_scenario.py
--rw-r--r--   0 theo       (501) staff       (20)    12310 2023-07-11 19:03:04.000000 bondzai.validation-framework-0.0.2/examples/scenario.py
--rw-r--r--   0 theo       (501) staff       (20)       97 2023-07-11 19:03:04.000000 bondzai.validation-framework-0.0.2/pyproject.toml
--rw-r--r--   0 theo       (501) staff       (20)      882 2023-07-11 19:03:39.087930 bondzai.validation-framework-0.0.2/setup.cfg
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-31 12:29:24.608267 bondzai.validation-framework-0.0.3/
+-rw-r--r--   0 theo       (501) staff       (20)      547 2023-07-31 12:26:43.000000 bondzai.validation-framework-0.0.3/NOTICE
+-rw-r--r--   0 theo       (501) staff       (20)      567 2023-07-31 12:29:24.608433 bondzai.validation-framework-0.0.3/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)       97 2023-07-31 12:26:43.000000 bondzai.validation-framework-0.0.3/README.md
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-31 12:29:24.598905 bondzai.validation-framework-0.0.3/bondzai/
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-31 12:29:24.604259 bondzai.validation-framework-0.0.3/bondzai/validation_framework/
+-rw-r--r--   0 theo       (501) staff       (20)       21 2023-07-31 12:29:08.000000 bondzai.validation-framework-0.0.3/bondzai/validation_framework/__init__.py
+-rw-r--r--   0 theo       (501) staff       (20)     2913 2023-07-31 12:26:43.000000 bondzai.validation-framework-0.0.3/bondzai/validation_framework/connector_handler.py
+-rw-r--r--   0 theo       (501) staff       (20)    10754 2023-07-31 12:29:08.000000 bondzai.validation-framework-0.0.3/bondzai/validation_framework/dataset_handler.py
+-rw-r--r--   0 theo       (501) staff       (20)     9244 2023-07-31 12:26:43.000000 bondzai.validation-framework-0.0.3/bondzai/validation_framework/event_catcher.py
+-rw-r--r--   0 theo       (501) staff       (20)     2696 2023-07-31 12:29:08.000000 bondzai.validation-framework-0.0.3/bondzai/validation_framework/log_handler.py
+-rw-r--r--   0 theo       (501) staff       (20)     9752 2023-07-31 12:29:08.000000 bondzai.validation-framework-0.0.3/bondzai/validation_framework/result_handler.py
+-rw-r--r--   0 theo       (501) staff       (20)     2028 2023-07-31 12:26:43.000000 bondzai.validation-framework-0.0.3/bondzai/validation_framework/tar_handler.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-31 12:29:24.607939 bondzai.validation-framework-0.0.3/bondzai.validation_framework.egg-info/
+-rw-r--r--   0 theo       (501) staff       (20)      567 2023-07-31 12:29:24.000000 bondzai.validation-framework-0.0.3/bondzai.validation_framework.egg-info/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)      793 2023-07-31 12:29:24.000000 bondzai.validation-framework-0.0.3/bondzai.validation_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-31 12:29:24.000000 bondzai.validation-framework-0.0.3/bondzai.validation_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 theo       (501) staff       (20)        8 2023-07-31 12:29:24.000000 bondzai.validation-framework-0.0.3/bondzai.validation_framework.egg-info/namespace_packages.txt
+-rw-r--r--   0 theo       (501) staff       (20)      117 2023-07-31 12:29:24.000000 bondzai.validation-framework-0.0.3/bondzai.validation_framework.egg-info/requires.txt
+-rw-r--r--   0 theo       (501) staff       (20)       22 2023-07-31 12:29:24.000000 bondzai.validation-framework-0.0.3/bondzai.validation_framework.egg-info/top_level.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-31 12:29:24.000000 bondzai.validation-framework-0.0.3/bondzai.validation_framework.egg-info/zip-safe
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-31 12:29:24.605425 bondzai.validation-framework-0.0.3/examples/
+-rw-r--r--   0 theo       (501) staff       (20)     5098 2023-07-31 12:26:43.000000 bondzai.validation-framework-0.0.3/examples/live_scenario.py
+-rw-r--r--   0 theo       (501) staff       (20)    13066 2023-07-31 12:29:08.000000 bondzai.validation-framework-0.0.3/examples/scenario.py
+-rw-r--r--   0 theo       (501) staff       (20)       97 2023-07-31 12:26:43.000000 bondzai.validation-framework-0.0.3/pyproject.toml
+-rw-r--r--   0 theo       (501) staff       (20)      864 2023-07-31 12:29:24.609371 bondzai.validation-framework-0.0.3/setup.cfg
```

### Comparing `bondzai.validation-framework-0.0.2/NOTICE` & `bondzai.validation-framework-0.0.3/NOTICE`

 * *Files identical despite different names*

### Comparing `bondzai.validation-framework-0.0.2/PKG-INFO` & `bondzai.validation-framework-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.validation-framework
-Version: 0.0.2
+Version: 0.0.3
 Summary: Bondzai Validation Framework
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai,validation
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.validation-framework-0.0.2/bondzai/validation_framework/connector_handler.py` & `bondzai.validation-framework-0.0.3/bondzai/validation_framework/connector_handler.py`

 * *Files identical despite different names*

### Comparing `bondzai.validation-framework-0.0.2/bondzai/validation_framework/dataset_handler.py` & `bondzai.validation-framework-0.0.3/bondzai/validation_framework/dataset_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 # All that is needed to load the dataset
-import shutil
-import tempfile
 
 import yaml
 import struct
-import json
 from pathlib import Path
 from .tar_handler import Tar
 from bondzai.gateway_sdk.agent import Agent
 from bondzai.gateway_sdk.enums import AgentAIType
 from .result_handler import ResultGatherer
 from typing import Union
 
+UNKNOWN = "unknown"
 
-# TODO : link infer_done label_type with different label names
 
 class Data:
     """
     Class representing one recording to be end for inference, enrollment or correction, generated exclusively by Dataset
     """
     def __init__(self,  id: str, agent_input: list[float] = [], agent_output: list[float] = [],
                  agent_source: int = None, metadata: dict = {}, output: dict = {}):
@@ -251,30 +248,30 @@
         Args:
             label_type_id: ID of type of the label
 
         Returns:
             label_type: type of the label
 
         """
-        label_type = self.lookup_table["labels"].get(str(label_type_id), 0)
+        label_type = self.lookup_table["labels"].get(str(label_type_id), UNKNOWN)
         return label_type
 
     def _label_int_to_name(self, label_type: str, value: int) -> str:
         """
         Convert a given label from int to string
         Args:
             label_type: type of the label
             value: value of the label as used by agent (int)
 
         Returns:
             label: label value as string
 
         """
         label_dict = self.reversed_outputs.get(label_type, {})
-        label = label_dict.get(value, "Unknown")
+        label = label_dict.get(value, UNKNOWN)
         return label
 
     def _label_name_to_int(self, label_type: str, label: str) -> int:
         """
         Convert a given label from string to int
         Args:
             label_type: type of the label
```

### Comparing `bondzai.validation-framework-0.0.2/bondzai/validation_framework/event_catcher.py` & `bondzai.validation-framework-0.0.3/bondzai/validation_framework/event_catcher.py`

 * *Files identical despite different names*

### Comparing `bondzai.validation-framework-0.0.2/bondzai/validation_framework/log_handler.py` & `bondzai.validation-framework-0.0.3/bondzai/validation_framework/log_handler.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import logging
 from texttable import Texttable
-from asciiplot import asciiize, Color
-import typing_extensions  # TODO : add to requirements
 import numpy as np
 import sys
 import time
 
 logging.basicConfig(
     format='%(asctime)s.%(msecs)03d | %(levelname)-8s | %(message)s',
     datefmt='%Y-%m-%d %H:%M:%S',
@@ -74,29 +72,7 @@
                 if idx == int(len(table_list) / 2):
                     table_list[idx] = row_title_str + row
                 else:
                     table_list[idx] = " " * len(row_title_str) + row
             offset = int((col_size + 3) * len(array) / 2)
             table_str = " " * (offset - 4 + len(row_title_str)) + f"{col_title}\n" + "\n".join(table_list)
     return table_str
-
-
-def lines_to_str(*sequences, colors: list = None, title: str = "Title", x_title: str = "x_title",
-                 y_title: str = "y_title") -> str:
-    if colors is None:
-        colors = [Color.DEFAULT] * len(sequences)
-    max_point_nb = np.max([len(_seq) for _seq in sequences])
-    plot_str = asciiize(
-        *sequences,
-        sequence_colors=colors,
-        inter_points_margin=int(100 / max_point_nb),
-        height=20,
-        background_color=Color.GREY_7,
-        title=title,
-        title_color=Color.MEDIUM_PURPLE,
-        label_color=Color.MEDIUM_PURPLE,
-        x_axis_description=x_title,
-        y_axis_description=y_title,
-        y_axis_tick_label_decimal_places=2,
-        center_horizontally=True
-    )
-    return plot_str
```

### Comparing `bondzai.validation-framework-0.0.2/bondzai/validation_framework/result_handler.py` & `bondzai.validation-framework-0.0.3/bondzai/validation_framework/result_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         expected_data: list of expected output
         predicted_data: list of predicted output
         percent: It True, display the confusion matrix in percent
     Returns:
         confusion_matrix: each column represent a predicted class, each row an expected class
     """
     label_list = np.unique(np.concatenate((expected_data, predicted_data))).tolist()
-    for unknown in ["Unknown", 0]:
+    for unknown in ["unknown", 0]:
         if unknown in label_list:
             label_list.pop(label_list.index(unknown))
             label_list.append(unknown)
     n_dim_out = len(label_list)
     confusion_matrix = np.zeros((n_dim_out + 1, n_dim_out + 1))
     for index, data in enumerate(expected_data):
         confusion_matrix[label_list.index(data) + 1, label_list.index(predicted_data[index]) + 1] += 1
```

### Comparing `bondzai.validation-framework-0.0.2/bondzai/validation_framework/tar_handler.py` & `bondzai.validation-framework-0.0.3/bondzai/validation_framework/tar_handler.py`

 * *Files identical despite different names*

### Comparing `bondzai.validation-framework-0.0.2/bondzai.validation_framework.egg-info/PKG-INFO` & `bondzai.validation-framework-0.0.3/bondzai.validation_framework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.validation-framework
-Version: 0.0.2
+Version: 0.0.3
 Summary: Bondzai Validation Framework
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai,validation
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.validation-framework-0.0.2/bondzai.validation_framework.egg-info/SOURCES.txt` & `bondzai.validation-framework-0.0.3/bondzai.validation_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bondzai.validation-framework-0.0.2/examples/live_scenario.py` & `bondzai.validation-framework-0.0.3/examples/live_scenario.py`

 * *Files identical despite different names*

### Comparing `bondzai.validation-framework-0.0.2/examples/scenario.py` & `bondzai.validation-framework-0.0.3/examples/scenario.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import threading
 import time
+import json
 
 import numpy as np
 from bondzai.gateway_sdk import Gateway, AgentAIMode, Agent, AgentTriggerType
 from bondzai.gateway_sdk.enums import EventOperationID, DBMTable
-from bondzai.validation_framework.log_handler import array_to_str, logger, lines_to_str, Color
+from bondzai.validation_framework.log_handler import array_to_str, logger
 from bondzai.validation_framework.result_handler import EXPECTED, PREDICTED
 from bondzai.validation_framework.dataset_handler import Dataset, Data
 from bondzai.validation_framework.event_catcher import EventCatcher
-from bondzai.validation_framework.result_handler import ResultGatherer
+from bondzai.validation_framework.result_handler import ResultGatherer, NumpyEncoder
 from pathlib import Path
 import argparse
 
+
 # To be run with OCR agent
 DEFAULT_CHUNK_RATE = 100
 DEFAULT_CHUNK_SIZE = 1024
 
 
 def training_is_done(agent: Agent, status):
     logger.info(f"EVT TRAIN : {status}")
@@ -91,24 +93,32 @@
         chunk_rate: chunk rate (in chunk/s)
         save_path: path of JSON file to save data
     Returns:
         results: results as dict
     """
     res = ResultGatherer(agent)
     event_catcher = EventCatcher()
+    data_len = len(dataset.data_list)
+    i = 0
     for data in dataset.iter_source():
         infer_one(agent, data, start_trigger, end_trigger, chunk_size, chunk_rate)
         wait_time, infer_result = event_catcher.wait_final_process(agent)
         logger.info(f"Wait for {np.round(wait_time, 2)}s")
         if infer_result is None:
             logger.warning("Missed inference")
         else:
             infer_data = dataset.update_data_from_event(data, infer_result)
             data.add_to_expected_result(res)
             infer_data.add_to_predicted_result(res)
+        
+        i += 1
+        send_to_clients({
+            "data-type": "run-progress",
+            "progress": (i * 100) / data_len
+        })
     results = res.get_results(save_path)
     return results
 
 
 def infer_all_no_wait(agent: Agent, res: ResultGatherer, dataset: Dataset,
                       start_trigger: AgentTriggerType = AgentTriggerType.TRIGGER_ON,
                       end_trigger: AgentTriggerType = AgentTriggerType.TRIGGER_OFF,
@@ -189,14 +199,16 @@
     for key, value in results.items():
         accuracy = np.round(value['accuracy'] * 100, 2) if value["accuracy"] is not None else None
         logger.info(f"\n{key}\n{array_to_str(value['confusion_matrix'])}"
                     f"\n\nAccuracy : {accuracy}%")
 
     kill(agent)
 
+    return results
+
 
 def incremental_learning(dataset_path: Path, agent: Agent, chunk_size: int = DEFAULT_CHUNK_SIZE,
                          chunk_rate: int = DEFAULT_CHUNK_RATE):
     CORRECTION_RATIO_THRESHOLD = 0.20
     ACCURACY_THRESHOLD = 0.9
 
     set_callbacks(agent)
@@ -241,35 +253,45 @@
                     infer_one(agent, data, start_trigger=AgentTriggerType.TRIGGER_ON,
                               end_trigger=AgentTriggerType.TRIGGER_OFF, chunk_rate=DEFAULT_CHUNK_RATE)
                     event_catcher.wait_final_process(agent)
                     data.send_correction_to_agent(agent, position=0)
                     force_train(agent)
                     break
 
-    logger.info(lines_to_str(accuracy_vect[1:], colors=[Color.RED],
-                             title="Incremental learning",
-                             x_title="Number of corrections",
-                             y_title="Accuracy"))
+    logger.info(accuracy_vect[1:])
 
     time.sleep(0.5)
 
     agent.kill()
 
+    return {"accuracy": accuracy_vect[1:]}
+
 
 def kill(agent: Agent):
     agent.kill()
 
 
 def export_dataset(agent: Agent):
     data = agent.export_table_data(DBMTable.DBM_DAT)
     logger.info(data)
 
     agent.kill()
 
 
+class R:
+    gateway: Gateway = None
+    current_agent: Agent = None
+
+
+def send_to_clients(data):
+    if not R.gateway:
+        return
+    R.gateway.send_to_clients(data)
+
+
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description=f"Run standard scenario")
     parser.add_argument("dataset", type=Path, help="Path of the dataset tar.gz file")
     parser.add_argument("-o", "--output", type=Path, default=None,
                         help="Path of the JSON file where inference results are saved")
     parser.add_argument("-s", "--size", type=int, default=DEFAULT_CHUNK_SIZE,
                         help=f"Chunk size (by default {DEFAULT_CHUNK_SIZE})")
@@ -279,29 +301,42 @@
                         help="If given, run scenario in async mode")
     parser.add_argument("-gh", "--host", type=str, default="127.0.0.1", help="Gateway host")
     parser.add_argument("-gp", "--port", type=int, default=8765, help="Gateway port")
     parser.add_argument("-i", "--incremental", action="store_true",
                         help="If given, run incremental learning scenario instead")
     args = parser.parse_args()
 
-    gateway = Gateway(args.host, args.port)
-    gateway.connect()
+    R.gateway = Gateway(args.host, args.port, secure=args.port == 443)
+    R.gateway.connect()
     logger.info("WAITING")
-    agents = gateway.wait_for_agent()
+    agents = R.gateway.wait_for_agent()
+
+    results = None
     if agents:
         logger.info("STARTING")
-        current_agent = agents[0]
-        current_agent.subscribe()
+        R.current_agent = agents[0]
+        R.current_agent.subscribe()
         if args.incremental:
-            incremental_learning(dataset_path=args.dataset,
-                                 agent=current_agent,
+            results = incremental_learning(dataset_path=args.dataset,
+                                 agent=R.current_agent,
                                  chunk_size=args.size,
                                  chunk_rate=args.rate)
         else:
-            standard(dataset_path=args.dataset,
-                     agent=current_agent,
-                     sync=not args.asynchro,
-                     save_path=args.output,
-                     chunk_size=args.size,
-                     chunk_rate=args.rate)
+            results = standard(dataset_path=args.dataset,
+                        agent=R.current_agent,
+                        sync=not args.asynchro,
+                        save_path=args.output,
+                        chunk_size=args.size,
+                        chunk_rate=args.rate)
+            
+    if results:
+        try:
+            # TMP Solution to pass numy object to gateway JSON encoder
+            results_json = json.dumps(results, cls=NumpyEncoder)
+            send_to_clients({
+                "data-type": "scenario-results",
+                "data": json.loads(results_json)
+            })
+        except Exception as e:
+            logger.error(f"Unable to send results to gateway : {str(e)}")
 
-    gateway.close()
+    R.gateway.close()
```

### Comparing `bondzai.validation-framework-0.0.2/setup.cfg` & `bondzai.validation-framework-0.0.3/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -20,16 +20,15 @@
 package_dir = 
 	= .
 zip_safe = True
 include_package_data = True
 namespace_packages = 
 	bondzai
 install_requires = 
-	asciiplot==1.0.0
-	bondzai.gateway-sdk==0.0.8
+	bondzai.gateway-sdk==0.0.9
 	numpy==1.24.3
 	PyYAML==6.0
 	texttable==1.6.7
 	typing_extensions==4.7.1
 
 [options.extras_require]
 dev =
```

