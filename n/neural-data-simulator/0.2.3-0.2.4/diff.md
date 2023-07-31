# Comparing `tmp/neural_data_simulator-0.2.3.tar.gz` & `tmp/neural_data_simulator-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural_data_simulator-0.2.3.tar", max compression
+gzip compressed data, was "neural_data_simulator-0.2.4.tar", max compression
```

## Comparing `neural_data_simulator-0.2.3.tar` & `neural_data_simulator-0.2.4.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0    11339 2023-07-31 17:01:45.055440 neural_data_simulator-0.2.3/LICENSE
--rw-r--r--   0        0        0     1881 2023-07-31 17:01:45.055440 neural_data_simulator-0.2.3/README.md
--rw-r--r--   0        0        0     3282 2023-07-31 17:02:00.647585 neural_data_simulator-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      970 2023-07-31 17:01:45.115440 neural_data_simulator-0.2.3/src/decoder/__init__.py
--rw-r--r--   0        0        0      999 2023-07-31 17:01:45.115440 neural_data_simulator-0.2.3/src/decoder/config/settings_decoder.yaml
--rw-r--r--   0        0        0     7657 2023-07-31 17:01:45.115440 neural_data_simulator-0.2.3/src/decoder/decoders.py
--rw-r--r--   0        0        0     5114 2023-07-31 17:01:45.115440 neural_data_simulator-0.2.3/src/decoder/run_decoder.py
--rw-r--r--   0        0        0     2487 2023-07-31 17:01:45.115440 neural_data_simulator-0.2.3/src/neural_data_simulator/__init__.py
--rw-r--r--   0        0        0      607 2023-07-31 17:01:45.115440 neural_data_simulator-0.2.3/src/neural_data_simulator/config/lsl.config
--rw-r--r--   0        0        0     5069 2023-07-31 17:01:45.115440 neural_data_simulator-0.2.3/src/neural_data_simulator/config/settings.yaml
--rw-r--r--   0        0        0     1297 2023-07-31 17:01:45.115440 neural_data_simulator-0.2.3/src/neural_data_simulator/config/settings_streamer.yaml
--rw-r--r--   0        0        0     3887 2023-07-31 17:01:45.115440 neural_data_simulator-0.2.3/src/neural_data_simulator/encoder.py
--rw-r--r--   0        0        0    27939 2023-07-31 17:01:45.115440 neural_data_simulator-0.2.3/src/neural_data_simulator/ephys_generator.py
--rw-r--r--   0        0        0     9464 2023-07-31 17:01:45.115440 neural_data_simulator-0.2.3/src/neural_data_simulator/filters.py
--rw-r--r--   0        0        0     2591 2023-07-31 17:01:45.115440 neural_data_simulator-0.2.3/src/neural_data_simulator/health_checker.py
--rw-r--r--   0        0        0    11823 2023-07-31 17:01:45.115440 neural_data_simulator-0.2.3/src/neural_data_simulator/inputs.py
--rw-r--r--   0        0        0     1792 2023-07-31 17:01:45.115440 neural_data_simulator-0.2.3/src/neural_data_simulator/models.py
--rw-r--r--   0        0        0    14019 2023-07-31 17:01:45.115440 neural_data_simulator-0.2.3/src/neural_data_simulator/outputs.py
--rw-r--r--   0        0        0     3129 2023-07-31 17:01:45.115440 neural_data_simulator-0.2.3/src/neural_data_simulator/runner.py
--rw-r--r--   0        0        0     4198 2023-07-31 17:01:45.115440 neural_data_simulator-0.2.3/src/neural_data_simulator/samples.py
--rw-r--r--   0        0        0       65 2023-07-31 17:01:45.115440 neural_data_simulator-0.2.3/src/neural_data_simulator/scripts/__init__.py
--rw-r--r--   0        0        0      103 2023-07-31 17:01:45.115440 neural_data_simulator-0.2.3/src/neural_data_simulator/scripts/errors.py
--rw-r--r--   0        0        0     4767 2023-07-31 17:01:45.115440 neural_data_simulator-0.2.3/src/neural_data_simulator/scripts/post_install_config.py
--rw-r--r--   0        0        0     9962 2023-07-31 17:01:45.115440 neural_data_simulator-0.2.3/src/neural_data_simulator/scripts/run_encoder.py
--rw-r--r--   0        0        0     9186 2023-07-31 17:01:45.119440 neural_data_simulator-0.2.3/src/neural_data_simulator/scripts/run_ephys_generator.py
--rw-r--r--   0        0        0    12118 2023-07-31 17:01:45.119440 neural_data_simulator-0.2.3/src/neural_data_simulator/scripts/run_streamer.py
--rw-r--r--   0        0        0     6979 2023-07-31 17:01:45.119440 neural_data_simulator-0.2.3/src/neural_data_simulator/settings.py
--rw-r--r--   0        0        0     5574 2023-07-31 17:01:45.119440 neural_data_simulator-0.2.3/src/neural_data_simulator/streamers.py
--rw-r--r--   0        0        0     2765 2023-07-31 17:01:45.119440 neural_data_simulator-0.2.3/src/neural_data_simulator/timing.py
--rw-r--r--   0        0        0       56 2023-07-31 17:01:45.119440 neural_data_simulator-0.2.3/src/neural_data_simulator/util/__init__.py
--rw-r--r--   0        0        0     3775 2023-07-31 17:01:45.119440 neural_data_simulator-0.2.3/src/neural_data_simulator/util/buffer.py
--rw-r--r--   0        0        0      961 2023-07-31 17:01:45.119440 neural_data_simulator-0.2.3/src/neural_data_simulator/util/circular_dequeue.py
--rw-r--r--   0        0        0     4046 2023-07-31 17:01:45.119440 neural_data_simulator-0.2.3/src/neural_data_simulator/util/runtime.py
--rw-r--r--   0        0        0     1291 2023-07-31 17:01:45.119440 neural_data_simulator-0.2.3/src/neural_data_simulator/util/settings_loader.py
--rw-r--r--   0        0        0       48 2023-07-31 17:01:45.119440 neural_data_simulator-0.2.3/src/plugins/__init__.py
--rw-r--r--   0        0        0      291 2023-07-31 17:01:45.119440 neural_data_simulator-0.2.3/src/plugins/examples/custom_script.py
--rw-r--r--   0        0        0     1000 2023-07-31 17:01:45.119440 neural_data_simulator-0.2.3/src/plugins/examples/gamepad_preprocessor.py
--rw-r--r--   0        0        0     5294 2023-07-31 17:01:45.119440 neural_data_simulator-0.2.3/src/plugins/examples/model.py
--rw-r--r--   0        0        0      648 2023-07-31 17:01:45.119440 neural_data_simulator-0.2.3/src/plugins/examples/postprocessor.py
--rw-r--r--   0        0        0      498 2023-07-31 17:01:45.119440 neural_data_simulator-0.2.3/src/plugins/examples/preprocessor.py
--rw-r--r--   0        0        0     4005 2023-07-31 17:01:45.119440 neural_data_simulator-0.2.3/src/plugins/examples/tests/test_model.py
--rw-r--r--   0        0        0      288 2023-07-31 17:01:45.119440 neural_data_simulator-0.2.3/src/recorder/__init__.py
--rw-r--r--   0        0        0     3201 2023-07-31 17:01:45.119440 neural_data_simulator-0.2.3/src/recorder/run_recorder.py
--rw-r--r--   0        0        0      251 2023-07-31 17:01:45.119440 neural_data_simulator-0.2.3/src/tasks/__init__.py
--rw-r--r--   0        0        0      872 2023-07-31 17:01:45.119440 neural_data_simulator-0.2.3/src/tasks/center_out_reach/__init__.py
--rw-r--r--   0        0        0     2125 2023-07-31 17:01:45.119440 neural_data_simulator-0.2.3/src/tasks/center_out_reach/buttons.py
--rw-r--r--   0        0        0     2901 2023-07-31 17:01:45.119440 neural_data_simulator-0.2.3/src/tasks/center_out_reach/input_events.py
--rw-r--r--   0        0        0     1628 2023-07-31 17:01:45.119440 neural_data_simulator-0.2.3/src/tasks/center_out_reach/joystick.py
--rw-r--r--   0        0        0     9827 2023-07-31 17:01:45.119440 neural_data_simulator-0.2.3/src/tasks/center_out_reach/metrics.py
--rw-r--r--   0        0        0     4049 2023-07-31 17:01:45.119440 neural_data_simulator-0.2.3/src/tasks/center_out_reach/scalers.py
--rw-r--r--   0        0        0     1583 2023-07-31 17:01:45.119440 neural_data_simulator-0.2.3/src/tasks/center_out_reach/screen_info.py
--rw-r--r--   0        0        0     2778 2023-07-31 17:01:45.119440 neural_data_simulator-0.2.3/src/tasks/center_out_reach/sprites.py
--rw-r--r--   0        0        0     6563 2023-07-31 17:01:45.119440 neural_data_simulator-0.2.3/src/tasks/center_out_reach/task_runner.py
--rw-r--r--   0        0        0    11351 2023-07-31 17:01:45.119440 neural_data_simulator-0.2.3/src/tasks/center_out_reach/task_state.py
--rw-r--r--   0        0        0    13249 2023-07-31 17:01:45.119440 neural_data_simulator-0.2.3/src/tasks/center_out_reach/task_window.py
--rw-r--r--   0        0        0     1593 2023-07-31 17:01:45.119440 neural_data_simulator-0.2.3/src/tasks/config/settings_center_out_reach.yaml
--rw-r--r--   0        0        0    12796 2023-07-31 17:01:45.119440 neural_data_simulator-0.2.3/src/tasks/run_center_out_reach.py
--rw-r--r--   0        0        0     4765 2023-07-31 17:01:45.119440 neural_data_simulator-0.2.3/src/tasks/run_closed_loop.py
--rw-r--r--   0        0        0     3672 1970-01-01 00:00:00.000000 neural_data_simulator-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-07-31 17:02:16.213808 neural_data_simulator-0.2.4/LICENSE
+-rw-r--r--   0        0        0     1881 2023-07-31 17:02:16.213808 neural_data_simulator-0.2.4/README.md
+-rw-r--r--   0        0        0     3282 2023-07-31 17:02:37.332004 neural_data_simulator-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      970 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/decoder/__init__.py
+-rw-r--r--   0        0        0      999 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/decoder/config/settings_decoder.yaml
+-rw-r--r--   0        0        0     7657 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/decoder/decoders.py
+-rw-r--r--   0        0        0     5114 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/decoder/run_decoder.py
+-rw-r--r--   0        0        0     2487 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/neural_data_simulator/__init__.py
+-rw-r--r--   0        0        0      607 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/neural_data_simulator/config/lsl.config
+-rw-r--r--   0        0        0     5069 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/neural_data_simulator/config/settings.yaml
+-rw-r--r--   0        0        0     1297 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/neural_data_simulator/config/settings_streamer.yaml
+-rw-r--r--   0        0        0     3887 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/neural_data_simulator/encoder.py
+-rw-r--r--   0        0        0    27939 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/neural_data_simulator/ephys_generator.py
+-rw-r--r--   0        0        0     9464 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/neural_data_simulator/filters.py
+-rw-r--r--   0        0        0     2591 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/neural_data_simulator/health_checker.py
+-rw-r--r--   0        0        0    11823 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/neural_data_simulator/inputs.py
+-rw-r--r--   0        0        0     1792 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/neural_data_simulator/models.py
+-rw-r--r--   0        0        0    14019 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/neural_data_simulator/outputs.py
+-rw-r--r--   0        0        0     3129 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/neural_data_simulator/runner.py
+-rw-r--r--   0        0        0     4198 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/neural_data_simulator/samples.py
+-rw-r--r--   0        0        0       65 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/neural_data_simulator/scripts/__init__.py
+-rw-r--r--   0        0        0      103 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/neural_data_simulator/scripts/errors.py
+-rw-r--r--   0        0        0     4767 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/neural_data_simulator/scripts/post_install_config.py
+-rw-r--r--   0        0        0     9962 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/neural_data_simulator/scripts/run_encoder.py
+-rw-r--r--   0        0        0     9186 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/neural_data_simulator/scripts/run_ephys_generator.py
+-rw-r--r--   0        0        0    12118 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/neural_data_simulator/scripts/run_streamer.py
+-rw-r--r--   0        0        0     6979 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/neural_data_simulator/settings.py
+-rw-r--r--   0        0        0     5574 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/neural_data_simulator/streamers.py
+-rw-r--r--   0        0        0     2765 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/neural_data_simulator/timing.py
+-rw-r--r--   0        0        0       56 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/neural_data_simulator/util/__init__.py
+-rw-r--r--   0        0        0     3775 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/neural_data_simulator/util/buffer.py
+-rw-r--r--   0        0        0      961 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/neural_data_simulator/util/circular_dequeue.py
+-rw-r--r--   0        0        0     4046 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/neural_data_simulator/util/runtime.py
+-rw-r--r--   0        0        0     1291 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/neural_data_simulator/util/settings_loader.py
+-rw-r--r--   0        0        0       48 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/plugins/__init__.py
+-rw-r--r--   0        0        0      291 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/plugins/examples/custom_script.py
+-rw-r--r--   0        0        0     1000 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/plugins/examples/gamepad_preprocessor.py
+-rw-r--r--   0        0        0     5294 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/plugins/examples/model.py
+-rw-r--r--   0        0        0      648 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/plugins/examples/postprocessor.py
+-rw-r--r--   0        0        0      498 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/plugins/examples/preprocessor.py
+-rw-r--r--   0        0        0     4005 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/plugins/examples/tests/test_model.py
+-rw-r--r--   0        0        0      288 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/recorder/__init__.py
+-rw-r--r--   0        0        0     3201 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/recorder/run_recorder.py
+-rw-r--r--   0        0        0      251 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/tasks/__init__.py
+-rw-r--r--   0        0        0      872 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/tasks/center_out_reach/__init__.py
+-rw-r--r--   0        0        0     2125 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/tasks/center_out_reach/buttons.py
+-rw-r--r--   0        0        0     2901 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/tasks/center_out_reach/input_events.py
+-rw-r--r--   0        0        0     1628 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/tasks/center_out_reach/joystick.py
+-rw-r--r--   0        0        0     9827 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/tasks/center_out_reach/metrics.py
+-rw-r--r--   0        0        0     4049 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/tasks/center_out_reach/scalers.py
+-rw-r--r--   0        0        0     1583 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/tasks/center_out_reach/screen_info.py
+-rw-r--r--   0        0        0     2778 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/tasks/center_out_reach/sprites.py
+-rw-r--r--   0        0        0     6563 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/tasks/center_out_reach/task_runner.py
+-rw-r--r--   0        0        0    11351 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/tasks/center_out_reach/task_state.py
+-rw-r--r--   0        0        0    13249 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/tasks/center_out_reach/task_window.py
+-rw-r--r--   0        0        0     1593 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/tasks/config/settings_center_out_reach.yaml
+-rw-r--r--   0        0        0    12796 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/tasks/run_center_out_reach.py
+-rw-r--r--   0        0        0     4765 2023-07-31 17:02:16.269814 neural_data_simulator-0.2.4/src/tasks/run_closed_loop.py
+-rw-r--r--   0        0        0     3672 1970-01-01 00:00:00.000000 neural_data_simulator-0.2.4/PKG-INFO
```

### Comparing `neural_data_simulator-0.2.3/LICENSE` & `neural_data_simulator-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/README.md` & `neural_data_simulator-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/pyproject.toml` & `neural_data_simulator-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neural-data-simulator"
-version = "v0.2.3"
+version = "v0.2.4"
 description = "Electrophysiology simulator data for developing Brain-Computer Interfaces"
 authors = ["AE Studio <bci@ae.studio>", "Chadwick Boulay <chadwick.boulay@gmail.com>"]
 maintainers = ["Chadwick Boulay <chadwick.boulay@gmail.com>", "AE Studio <bci@ae.studio>"]
 packages = [
     {include = "neural_data_simulator", from = "src"},
     {include = "decoder", from = "src"},
     {include = "recorder", from = "src"},
```

### Comparing `neural_data_simulator-0.2.3/src/decoder/__init__.py` & `neural_data_simulator-0.2.4/src/decoder/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/decoder/config/settings_decoder.yaml` & `neural_data_simulator-0.2.4/src/decoder/config/settings_decoder.yaml`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/decoder/decoders.py` & `neural_data_simulator-0.2.4/src/decoder/decoders.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/decoder/run_decoder.py` & `neural_data_simulator-0.2.4/src/decoder/run_decoder.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/neural_data_simulator/__init__.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/neural_data_simulator/config/lsl.config` & `neural_data_simulator-0.2.4/src/neural_data_simulator/config/lsl.config`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/neural_data_simulator/config/settings.yaml` & `neural_data_simulator-0.2.4/src/neural_data_simulator/config/settings.yaml`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/neural_data_simulator/config/settings_streamer.yaml` & `neural_data_simulator-0.2.4/src/neural_data_simulator/config/settings_streamer.yaml`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/neural_data_simulator/encoder.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/encoder.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/neural_data_simulator/ephys_generator.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/ephys_generator.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/neural_data_simulator/filters.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/filters.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/neural_data_simulator/health_checker.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/health_checker.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/neural_data_simulator/inputs.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/inputs.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/neural_data_simulator/models.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/models.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/neural_data_simulator/outputs.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/outputs.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/neural_data_simulator/runner.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/runner.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/neural_data_simulator/samples.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/samples.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/neural_data_simulator/scripts/post_install_config.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/scripts/post_install_config.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/neural_data_simulator/scripts/run_encoder.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/scripts/run_encoder.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/neural_data_simulator/scripts/run_ephys_generator.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/scripts/run_ephys_generator.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/neural_data_simulator/scripts/run_streamer.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/scripts/run_streamer.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/neural_data_simulator/settings.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/settings.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/neural_data_simulator/streamers.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/streamers.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/neural_data_simulator/timing.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/timing.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/neural_data_simulator/util/buffer.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/util/buffer.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/neural_data_simulator/util/circular_dequeue.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/util/circular_dequeue.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/neural_data_simulator/util/runtime.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/util/runtime.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/neural_data_simulator/util/settings_loader.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/util/settings_loader.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/plugins/examples/gamepad_preprocessor.py` & `neural_data_simulator-0.2.4/src/plugins/examples/gamepad_preprocessor.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/plugins/examples/model.py` & `neural_data_simulator-0.2.4/src/plugins/examples/model.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/plugins/examples/postprocessor.py` & `neural_data_simulator-0.2.4/src/plugins/examples/postprocessor.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/plugins/examples/tests/test_model.py` & `neural_data_simulator-0.2.4/src/plugins/examples/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/recorder/run_recorder.py` & `neural_data_simulator-0.2.4/src/recorder/run_recorder.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/tasks/center_out_reach/__init__.py` & `neural_data_simulator-0.2.4/src/tasks/center_out_reach/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/tasks/center_out_reach/buttons.py` & `neural_data_simulator-0.2.4/src/tasks/center_out_reach/buttons.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/tasks/center_out_reach/input_events.py` & `neural_data_simulator-0.2.4/src/tasks/center_out_reach/input_events.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/tasks/center_out_reach/joystick.py` & `neural_data_simulator-0.2.4/src/tasks/center_out_reach/joystick.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/tasks/center_out_reach/metrics.py` & `neural_data_simulator-0.2.4/src/tasks/center_out_reach/metrics.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/tasks/center_out_reach/scalers.py` & `neural_data_simulator-0.2.4/src/tasks/center_out_reach/scalers.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/tasks/center_out_reach/screen_info.py` & `neural_data_simulator-0.2.4/src/tasks/center_out_reach/screen_info.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/tasks/center_out_reach/sprites.py` & `neural_data_simulator-0.2.4/src/tasks/center_out_reach/sprites.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/tasks/center_out_reach/task_runner.py` & `neural_data_simulator-0.2.4/src/tasks/center_out_reach/task_runner.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/tasks/center_out_reach/task_state.py` & `neural_data_simulator-0.2.4/src/tasks/center_out_reach/task_state.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/tasks/center_out_reach/task_window.py` & `neural_data_simulator-0.2.4/src/tasks/center_out_reach/task_window.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/tasks/config/settings_center_out_reach.yaml` & `neural_data_simulator-0.2.4/src/tasks/config/settings_center_out_reach.yaml`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/tasks/run_center_out_reach.py` & `neural_data_simulator-0.2.4/src/tasks/run_center_out_reach.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/src/tasks/run_closed_loop.py` & `neural_data_simulator-0.2.4/src/tasks/run_closed_loop.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.3/PKG-INFO` & `neural_data_simulator-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural-data-simulator
-Version: 0.2.3
+Version: 0.2.4
 Summary: Electrophysiology simulator data for developing Brain-Computer Interfaces
 License: Apache-2.0
 Author: AE Studio
 Author-email: bci@ae.studio
 Maintainer: Chadwick Boulay
 Maintainer-email: chadwick.boulay@gmail.com
 Requires-Python: >=3.9,<3.12
```

