# Comparing `tmp/neural_data_simulator-0.2.2.tar.gz` & `tmp/neural_data_simulator-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural_data_simulator-0.2.2.tar", max compression
+gzip compressed data, was "neural_data_simulator-0.2.4.tar", max compression
```

## Comparing `neural_data_simulator-0.2.2.tar` & `neural_data_simulator-0.2.4.tar`

### file list

```diff
@@ -1,58 +1,59 @@
--rw-r--r--   0        0        0    11339 2023-07-06 08:31:26.514233 neural_data_simulator-0.2.2/LICENSE
--rw-r--r--   0        0        0     1881 2023-07-06 08:31:26.514233 neural_data_simulator-0.2.2/README.md
--rw-r--r--   0        0        0     3282 2023-07-06 08:31:48.754514 neural_data_simulator-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      970 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/decoder/__init__.py
--rw-r--r--   0        0        0      999 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/decoder/config/settings_decoder.yaml
--rw-r--r--   0        0        0     7657 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/decoder/decoders.py
--rw-r--r--   0        0        0     5114 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/decoder/run_decoder.py
--rw-r--r--   0        0        0     2487 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/__init__.py
--rw-r--r--   0        0        0      607 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/config/lsl.config
--rw-r--r--   0        0        0     5069 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/config/settings.yaml
--rw-r--r--   0        0        0     1297 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/config/settings_streamer.yaml
--rw-r--r--   0        0        0     3887 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/encoder.py
--rw-r--r--   0        0        0    27939 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/ephys_generator.py
--rw-r--r--   0        0        0     9464 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/filters.py
--rw-r--r--   0        0        0     2591 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/health_checker.py
--rw-r--r--   0        0        0    11823 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/inputs.py
--rw-r--r--   0        0        0     1792 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/models.py
--rw-r--r--   0        0        0    14019 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/outputs.py
--rw-r--r--   0        0        0     3129 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/runner.py
--rw-r--r--   0        0        0     4198 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/samples.py
--rw-r--r--   0        0        0       65 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/scripts/__init__.py
--rw-r--r--   0        0        0      103 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/scripts/errors.py
--rw-r--r--   0        0        0     4723 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/scripts/post_install_config.py
--rw-r--r--   0        0        0     9969 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/scripts/run_encoder.py
--rw-r--r--   0        0        0     9186 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/scripts/run_ephys_generator.py
--rw-r--r--   0        0        0    12118 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/scripts/run_streamer.py
--rw-r--r--   0        0        0     6979 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/settings.py
--rw-r--r--   0        0        0     5574 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/streamers.py
--rw-r--r--   0        0        0     2765 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/timing.py
--rw-r--r--   0        0        0       56 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/util/__init__.py
--rw-r--r--   0        0        0     3775 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/util/buffer.py
--rw-r--r--   0        0        0      961 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/util/circular_dequeue.py
--rw-r--r--   0        0        0     4046 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/util/runtime.py
--rw-r--r--   0        0        0     1291 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/neural_data_simulator/util/settings_loader.py
--rw-r--r--   0        0        0       48 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/plugins/__init__.py
--rw-r--r--   0        0        0     1000 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/plugins/examples/gamepad_preprocessor.py
--rw-r--r--   0        0        0     5294 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/plugins/examples/model.py
--rw-r--r--   0        0        0      572 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/plugins/examples/postprocessor.py
--rw-r--r--   0        0        0      498 2023-07-06 08:31:26.566234 neural_data_simulator-0.2.2/src/plugins/examples/preprocessor.py
--rw-r--r--   0        0        0     4005 2023-07-06 08:31:26.570234 neural_data_simulator-0.2.2/src/plugins/examples/tests/test_model.py
--rw-r--r--   0        0        0      288 2023-07-06 08:31:26.570234 neural_data_simulator-0.2.2/src/recorder/__init__.py
--rw-r--r--   0        0        0     3201 2023-07-06 08:31:26.570234 neural_data_simulator-0.2.2/src/recorder/run_recorder.py
--rw-r--r--   0        0        0      251 2023-07-06 08:31:26.570234 neural_data_simulator-0.2.2/src/tasks/__init__.py
--rw-r--r--   0        0        0      872 2023-07-06 08:31:26.570234 neural_data_simulator-0.2.2/src/tasks/center_out_reach/__init__.py
--rw-r--r--   0        0        0     2125 2023-07-06 08:31:26.570234 neural_data_simulator-0.2.2/src/tasks/center_out_reach/buttons.py
--rw-r--r--   0        0        0     2901 2023-07-06 08:31:26.570234 neural_data_simulator-0.2.2/src/tasks/center_out_reach/input_events.py
--rw-r--r--   0        0        0     1628 2023-07-06 08:31:26.570234 neural_data_simulator-0.2.2/src/tasks/center_out_reach/joystick.py
--rw-r--r--   0        0        0     9827 2023-07-06 08:31:26.570234 neural_data_simulator-0.2.2/src/tasks/center_out_reach/metrics.py
--rw-r--r--   0        0        0     4049 2023-07-06 08:31:26.570234 neural_data_simulator-0.2.2/src/tasks/center_out_reach/scalers.py
--rw-r--r--   0        0        0     1583 2023-07-06 08:31:26.570234 neural_data_simulator-0.2.2/src/tasks/center_out_reach/screen_info.py
--rw-r--r--   0        0        0     2778 2023-07-06 08:31:26.570234 neural_data_simulator-0.2.2/src/tasks/center_out_reach/sprites.py
--rw-r--r--   0        0        0     6563 2023-07-06 08:31:26.570234 neural_data_simulator-0.2.2/src/tasks/center_out_reach/task_runner.py
--rw-r--r--   0        0        0    11351 2023-07-06 08:31:26.570234 neural_data_simulator-0.2.2/src/tasks/center_out_reach/task_state.py
--rw-r--r--   0        0        0    13249 2023-07-06 08:31:26.570234 neural_data_simulator-0.2.2/src/tasks/center_out_reach/task_window.py
--rw-r--r--   0        0        0     1593 2023-07-06 08:31:26.570234 neural_data_simulator-0.2.2/src/tasks/config/settings_center_out_reach.yaml
--rw-r--r--   0        0        0    12028 2023-07-06 08:31:26.570234 neural_data_simulator-0.2.2/src/tasks/run_center_out_reach.py
--rw-r--r--   0        0        0     2014 2023-07-06 08:31:26.570234 neural_data_simulator-0.2.2/src/tasks/run_closed_loop.py
--rw-r--r--   0        0        0     3672 1970-01-01 00:00:00.000000 neural_data_simulator-0.2.2/PKG-INFO
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

### Comparing `neural_data_simulator-0.2.2/LICENSE` & `neural_data_simulator-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/README.md` & `neural_data_simulator-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/pyproject.toml` & `neural_data_simulator-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neural-data-simulator"
-version = "v0.2.2"
+version = "v0.2.4"
 description = "Electrophysiology simulator data for developing Brain-Computer Interfaces"
 authors = ["AE Studio <bci@ae.studio>", "Chadwick Boulay <chadwick.boulay@gmail.com>"]
 maintainers = ["Chadwick Boulay <chadwick.boulay@gmail.com>", "AE Studio <bci@ae.studio>"]
 packages = [
     {include = "neural_data_simulator", from = "src"},
     {include = "decoder", from = "src"},
     {include = "recorder", from = "src"},
```

### Comparing `neural_data_simulator-0.2.2/src/decoder/__init__.py` & `neural_data_simulator-0.2.4/src/decoder/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/decoder/config/settings_decoder.yaml` & `neural_data_simulator-0.2.4/src/decoder/config/settings_decoder.yaml`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/decoder/decoders.py` & `neural_data_simulator-0.2.4/src/decoder/decoders.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/decoder/run_decoder.py` & `neural_data_simulator-0.2.4/src/decoder/run_decoder.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/neural_data_simulator/__init__.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/neural_data_simulator/config/lsl.config` & `neural_data_simulator-0.2.4/src/neural_data_simulator/config/lsl.config`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/neural_data_simulator/config/settings.yaml` & `neural_data_simulator-0.2.4/src/neural_data_simulator/config/settings.yaml`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/neural_data_simulator/config/settings_streamer.yaml` & `neural_data_simulator-0.2.4/src/neural_data_simulator/config/settings_streamer.yaml`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/neural_data_simulator/encoder.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/encoder.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/neural_data_simulator/ephys_generator.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/ephys_generator.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/neural_data_simulator/filters.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/filters.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/neural_data_simulator/health_checker.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/health_checker.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/neural_data_simulator/inputs.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/inputs.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/neural_data_simulator/models.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/models.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/neural_data_simulator/outputs.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/outputs.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/neural_data_simulator/runner.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/runner.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/neural_data_simulator/samples.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/samples.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/neural_data_simulator/scripts/post_install_config.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/scripts/post_install_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from neural_data_simulator.util.runtime import get_sample_data_dir
 
 plugin_files = [
     ("model.py", plugins.__file__),
     ("preprocessor.py", plugins.__file__),
     ("postprocessor.py", plugins.__file__),
     ("gamepad_preprocessor.py", plugins.__file__),
+    ("custom_script.py", plugins.__file__),
 ]
 
 plugin_test_files = [
     ("test_model.py", os.path.join(os.path.dirname(plugins.__file__), "examples"))
 ]
```

### Comparing `neural_data_simulator-0.2.2/src/neural_data_simulator/scripts/run_encoder.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/scripts/run_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     return data_input
 
 
 def _load_module(module_path: str, module_name: str) -> ModuleType:
     """Load an external module and return it."""
     module_path = get_abs_path(module_path)
     module_dir_path = Path(module_path).parent
-    sys.path.append(str(module_dir_path.parent.absolute()))
+    sys.path.append(str(module_dir_path.absolute()))
 
     loader = importlib.machinery.SourceFileLoader(module_name, module_path)
     spec = importlib.util.spec_from_loader(module_name, loader)
     if spec:
         plugin_module = importlib.util.module_from_spec(spec)
         loader.exec_module(plugin_module)
         return plugin_module
```

### Comparing `neural_data_simulator-0.2.2/src/neural_data_simulator/scripts/run_ephys_generator.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/scripts/run_ephys_generator.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/neural_data_simulator/scripts/run_streamer.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/scripts/run_streamer.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/neural_data_simulator/settings.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/settings.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/neural_data_simulator/streamers.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/streamers.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/neural_data_simulator/timing.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/timing.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/neural_data_simulator/util/buffer.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/util/buffer.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/neural_data_simulator/util/circular_dequeue.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/util/circular_dequeue.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/neural_data_simulator/util/runtime.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/util/runtime.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/neural_data_simulator/util/settings_loader.py` & `neural_data_simulator-0.2.4/src/neural_data_simulator/util/settings_loader.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/plugins/examples/gamepad_preprocessor.py` & `neural_data_simulator-0.2.4/src/plugins/examples/gamepad_preprocessor.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/plugins/examples/model.py` & `neural_data_simulator-0.2.4/src/plugins/examples/model.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/plugins/examples/postprocessor.py` & `neural_data_simulator-0.2.4/src/plugins/examples/postprocessor.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Example of a custom Postprocessor implementation."""
-import numpy as np
+
+# This is how a custom script can be imported from the same directory as this one
+import custom_script
 
 from neural_data_simulator.encoder import Processor
 from neural_data_simulator.samples import Samples
 
 
 class PassThroughPostprocessor(Processor):
     """Custom Postprocessor implementation."""
 
     def execute(self, data: Samples) -> Samples:
         """Process the data and return the transformation."""
-        data.data = np.clip(data.data, 0, None)
-        return data
+        return custom_script.run_post_transformation(data)
 
 
 def create_postprocessor() -> Processor:
     """Instantiate the Postprocessor."""
     return PassThroughPostprocessor()
```

### Comparing `neural_data_simulator-0.2.2/src/plugins/examples/tests/test_model.py` & `neural_data_simulator-0.2.4/src/plugins/examples/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/recorder/run_recorder.py` & `neural_data_simulator-0.2.4/src/recorder/run_recorder.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/tasks/center_out_reach/__init__.py` & `neural_data_simulator-0.2.4/src/tasks/center_out_reach/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/tasks/center_out_reach/buttons.py` & `neural_data_simulator-0.2.4/src/tasks/center_out_reach/buttons.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/tasks/center_out_reach/input_events.py` & `neural_data_simulator-0.2.4/src/tasks/center_out_reach/input_events.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/tasks/center_out_reach/joystick.py` & `neural_data_simulator-0.2.4/src/tasks/center_out_reach/joystick.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/tasks/center_out_reach/metrics.py` & `neural_data_simulator-0.2.4/src/tasks/center_out_reach/metrics.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/tasks/center_out_reach/scalers.py` & `neural_data_simulator-0.2.4/src/tasks/center_out_reach/scalers.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/tasks/center_out_reach/screen_info.py` & `neural_data_simulator-0.2.4/src/tasks/center_out_reach/screen_info.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/tasks/center_out_reach/sprites.py` & `neural_data_simulator-0.2.4/src/tasks/center_out_reach/sprites.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/tasks/center_out_reach/task_runner.py` & `neural_data_simulator-0.2.4/src/tasks/center_out_reach/task_runner.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/tasks/center_out_reach/task_state.py` & `neural_data_simulator-0.2.4/src/tasks/center_out_reach/task_state.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/tasks/center_out_reach/task_window.py` & `neural_data_simulator-0.2.4/src/tasks/center_out_reach/task_window.py`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/tasks/config/settings_center_out_reach.yaml` & `neural_data_simulator-0.2.4/src/tasks/config/settings_center_out_reach.yaml`

 * *Files identical despite different names*

### Comparing `neural_data_simulator-0.2.2/src/tasks/run_center_out_reach.py` & `neural_data_simulator-0.2.4/src/tasks/run_center_out_reach.py`

 * *Files 4% similar despite different names*

```diff
@@ -254,19 +254,24 @@
     initialize_logger(SCRIPT_NAME)
     parser = argparse.ArgumentParser(description="Run GUI.")
     parser.add_argument(
         "--settings-path",
         type=Path,
         help="Path to the settings_center_out_reach.yaml file.",
     )
-
+    parser.add_argument(
+        "--control-file",
+        type=Path,
+        help="Path to the control file that will receive control messages.",
+    )
+    args = parser.parse_args()
     settings = cast(
         _Settings,
         get_script_settings(
-            parser.parse_args().settings_path,
+            args.settings_path,
             "settings_center_out_reach.yaml",
             _Settings,
         ),
     )
     configure_logger(SCRIPT_NAME, settings.log_level)
 
     if settings.center_out_reach.input.enabled:
@@ -332,28 +337,46 @@
             user_input.input_device_name,
         )
     else:
         menu_text = _get_training_text(
             "black", window_settings.colors.target, user_input.input_device_name
         )
 
-    with open_connection(data_output), open_connection(data_input):
-        task_window = TaskWindow(window_rect, window_params, menu_text)
-        task_state = TaskState(task_window, state_params)
-        task_runner = TaskRunner(
-            sampling_rate,
-            data_input,
-            data_output,
-            velocity_scaler,
-            with_decoded_cursor,
-            metrics_collector,
-        )
-        task_runner.run(task_state, user_input)
-
-        if not task_window.show_menu_screen and _metrics_enabled(settings):
-            unwrap(metrics_collector).plot_metrics(task_window.target_positions)
+    interrupted = False
+    task_window = None
+    try:
+        with open_connection(data_output), open_connection(data_input):
+            task_window = TaskWindow(window_rect, window_params, menu_text)
+            task_state = TaskState(task_window, state_params)
+            task_runner = TaskRunner(
+                sampling_rate,
+                data_input,
+                data_output,
+                velocity_scaler,
+                with_decoded_cursor,
+                metrics_collector,
+            )
+            logger.info("Running task")
+            task_runner.run(task_state, user_input)
+    except KeyboardInterrupt:
+        logger.info("CTRL+C received. Exiting...")
+        interrupted = True
+
+    # This is used as a signal to a parent process that the main task has finished
+    if args.control_file is not None:
+        with open(args.control_file, "w") as control_file:
+            control_file.write("main_task_finished\n")
+
+    if (
+        not interrupted
+        and task_window is not None
+        and not task_window.show_menu_screen
+        and _metrics_enabled(settings)
+    ):
+        unwrap(metrics_collector).plot_metrics(task_window.target_positions)
 
+    if task_window is not None:
         task_window.leave()
 
 
 if __name__ == "__main__":
     run()
```

### Comparing `neural_data_simulator-0.2.2/PKG-INFO` & `neural_data_simulator-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural-data-simulator
-Version: 0.2.2
+Version: 0.2.4
 Summary: Electrophysiology simulator data for developing Brain-Computer Interfaces
 License: Apache-2.0
 Author: AE Studio
 Author-email: bci@ae.studio
 Maintainer: Chadwick Boulay
 Maintainer-email: chadwick.boulay@gmail.com
 Requires-Python: >=3.9,<3.12
```

