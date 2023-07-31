# Comparing `tmp/Jetson.GPIO-2.1.1.tar.gz` & `tmp/Jetson.GPIO-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Jetson.GPIO-2.1.1.tar", last modified: Wed Apr 12 19:18:31 2023, max compression
+gzip compressed data, was "Jetson.GPIO-2.1.2.tar", last modified: Mon Jul 31 21:11:44 2023, max compression
```

## Comparing `Jetson.GPIO-2.1.1.tar` & `Jetson.GPIO-2.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 lhoang    (1000) lhoang    (1000)        0 2023-04-12 19:18:31.001806 Jetson.GPIO-2.1.1/
--rw-------   0 lhoang    (1000) lhoang    (1000)     1178 2021-04-29 15:58:52.000000 Jetson.GPIO-2.1.1/LICENSE.txt
--rw-------   0 lhoang    (1000) lhoang    (1000)       83 2021-04-29 15:58:52.000000 Jetson.GPIO-2.1.1/MANIFEST.in
--rw-rw-r--   0 lhoang    (1000) lhoang    (1000)    15864 2023-04-12 19:18:31.001806 Jetson.GPIO-2.1.1/PKG-INFO
--rw-rw-r--   0 lhoang    (1000) lhoang    (1000)    15229 2023-03-30 03:11:38.000000 Jetson.GPIO-2.1.1/README.md
-drwxrwxr-x   0 lhoang    (1000) lhoang    (1000)        0 2023-04-12 19:18:30.997806 Jetson.GPIO-2.1.1/lib/
-drwxrwxr-x   0 lhoang    (1000) lhoang    (1000)        0 2023-04-12 19:18:30.997806 Jetson.GPIO-2.1.1/lib/python/
-drwxrwxr-x   0 lhoang    (1000) lhoang    (1000)        0 2023-04-12 19:18:30.997806 Jetson.GPIO-2.1.1/lib/python/Jetson/
-drwxrwxr-x   0 lhoang    (1000) lhoang    (1000)        0 2023-04-12 19:18:31.001806 Jetson.GPIO-2.1.1/lib/python/Jetson/GPIO/
--rw-rw-r--   0 lhoang    (1000) lhoang    (1000)     1749 2023-03-30 03:11:38.000000 Jetson.GPIO-2.1.1/lib/python/Jetson/GPIO/99-gpio.rules
--rw-rw-r--   0 lhoang    (1000) lhoang    (1000)       38 2023-03-30 03:11:38.000000 Jetson.GPIO-2.1.1/lib/python/Jetson/GPIO/__init__.py
--rw-rw-r--   0 lhoang    (1000) lhoang    (1000)    19821 2023-04-12 19:17:23.000000 Jetson.GPIO-2.1.1/lib/python/Jetson/GPIO/gpio.py
--rw-rw-r--   0 lhoang    (1000) lhoang    (1000)     8300 2023-04-12 19:17:23.000000 Jetson.GPIO-2.1.1/lib/python/Jetson/GPIO/gpio_cdev.py
--rw-rw-r--   0 lhoang    (1000) lhoang    (1000)    11205 2023-04-12 19:17:13.000000 Jetson.GPIO-2.1.1/lib/python/Jetson/GPIO/gpio_event.py
--rw-rw-r--   0 lhoang    (1000) lhoang    (1000)    29648 2023-03-30 03:11:38.000000 Jetson.GPIO-2.1.1/lib/python/Jetson/GPIO/gpio_pin_data.py
--rw-------   0 lhoang    (1000) lhoang    (1000)        1 2021-04-29 15:58:52.000000 Jetson.GPIO-2.1.1/lib/python/Jetson/__init__.py
-drwxrwxr-x   0 lhoang    (1000) lhoang    (1000)        0 2023-04-12 19:18:30.997806 Jetson.GPIO-2.1.1/lib/python/Jetson.GPIO.egg-info/
--rw-rw-r--   0 lhoang    (1000) lhoang    (1000)    15864 2023-04-12 19:18:30.000000 Jetson.GPIO-2.1.1/lib/python/Jetson.GPIO.egg-info/PKG-INFO
--rw-rw-r--   0 lhoang    (1000) lhoang    (1000)      531 2023-04-12 19:18:30.000000 Jetson.GPIO-2.1.1/lib/python/Jetson.GPIO.egg-info/SOURCES.txt
--rw-rw-r--   0 lhoang    (1000) lhoang    (1000)        1 2023-04-12 19:18:30.000000 Jetson.GPIO-2.1.1/lib/python/Jetson.GPIO.egg-info/dependency_links.txt
--rw-rw-r--   0 lhoang    (1000) lhoang    (1000)       11 2023-04-12 19:18:30.000000 Jetson.GPIO-2.1.1/lib/python/Jetson.GPIO.egg-info/top_level.txt
-drwxrwxr-x   0 lhoang    (1000) lhoang    (1000)        0 2023-04-12 19:18:31.001806 Jetson.GPIO-2.1.1/lib/python/RPi/
-drwxrwxr-x   0 lhoang    (1000) lhoang    (1000)        0 2023-04-12 19:18:31.001806 Jetson.GPIO-2.1.1/lib/python/RPi/GPIO/
--rw-------   0 lhoang    (1000) lhoang    (1000)       44 2021-04-29 15:58:52.000000 Jetson.GPIO-2.1.1/lib/python/RPi/GPIO/__init__.py
--rw-------   0 lhoang    (1000) lhoang    (1000)        1 2021-04-29 15:58:52.000000 Jetson.GPIO-2.1.1/lib/python/RPi/__init__.py
--rw-rw-r--   0 lhoang    (1000) lhoang    (1000)       38 2023-04-12 19:18:31.001806 Jetson.GPIO-2.1.1/setup.cfg
--rw-rw-r--   0 lhoang    (1000) lhoang    (1000)     2432 2023-03-30 03:11:38.000000 Jetson.GPIO-2.1.1/setup.py
+drwxrwxr-x   0 lhoang    (1000) lhoang    (1000)        0 2023-07-31 21:11:44.098630 Jetson.GPIO-2.1.2/
+-rw-------   0 lhoang    (1000) lhoang    (1000)     1178 2021-04-29 15:58:52.000000 Jetson.GPIO-2.1.2/LICENSE.txt
+-rw-------   0 lhoang    (1000) lhoang    (1000)       83 2021-04-29 15:58:52.000000 Jetson.GPIO-2.1.2/MANIFEST.in
+-rw-rw-r--   0 lhoang    (1000) lhoang    (1000)    16882 2023-07-31 21:11:44.098630 Jetson.GPIO-2.1.2/PKG-INFO
+-rw-rw-r--   0 lhoang    (1000) lhoang    (1000)    16247 2023-07-31 20:18:02.000000 Jetson.GPIO-2.1.2/README.md
+drwxrwxr-x   0 lhoang    (1000) lhoang    (1000)        0 2023-07-31 21:11:44.094630 Jetson.GPIO-2.1.2/lib/
+drwxrwxr-x   0 lhoang    (1000) lhoang    (1000)        0 2023-07-31 21:11:44.094630 Jetson.GPIO-2.1.2/lib/python/
+drwxrwxr-x   0 lhoang    (1000) lhoang    (1000)        0 2023-07-31 21:11:44.094630 Jetson.GPIO-2.1.2/lib/python/Jetson/
+drwxrwxr-x   0 lhoang    (1000) lhoang    (1000)        0 2023-07-31 21:11:44.098630 Jetson.GPIO-2.1.2/lib/python/Jetson/GPIO/
+-rw-rw-r--   0 lhoang    (1000) lhoang    (1000)     1749 2023-03-30 03:11:38.000000 Jetson.GPIO-2.1.2/lib/python/Jetson/GPIO/99-gpio.rules
+-rw-rw-r--   0 lhoang    (1000) lhoang    (1000)       38 2023-07-31 21:04:28.000000 Jetson.GPIO-2.1.2/lib/python/Jetson/GPIO/__init__.py
+-rwxrwxr-x   0 lhoang    (1000) lhoang    (1000)    23548 2023-07-31 20:18:02.000000 Jetson.GPIO-2.1.2/lib/python/Jetson/GPIO/gpio.py
+-rwxrwxr-x   0 lhoang    (1000) lhoang    (1000)     9782 2023-07-31 20:18:02.000000 Jetson.GPIO-2.1.2/lib/python/Jetson/GPIO/gpio_cdev.py
+-rwxrwxr-x   0 lhoang    (1000) lhoang    (1000)    19080 2023-07-31 20:18:02.000000 Jetson.GPIO-2.1.2/lib/python/Jetson/GPIO/gpio_event.py
+-rwxrwxr-x   0 lhoang    (1000) lhoang    (1000)    30342 2023-07-31 20:18:02.000000 Jetson.GPIO-2.1.2/lib/python/Jetson/GPIO/gpio_pin_data.py
+-rw-------   0 lhoang    (1000) lhoang    (1000)        1 2021-04-29 15:58:52.000000 Jetson.GPIO-2.1.2/lib/python/Jetson/__init__.py
+drwxrwxr-x   0 lhoang    (1000) lhoang    (1000)        0 2023-07-31 21:11:44.094630 Jetson.GPIO-2.1.2/lib/python/Jetson.GPIO.egg-info/
+-rw-rw-r--   0 lhoang    (1000) lhoang    (1000)    16882 2023-07-31 21:11:44.000000 Jetson.GPIO-2.1.2/lib/python/Jetson.GPIO.egg-info/PKG-INFO
+-rw-rw-r--   0 lhoang    (1000) lhoang    (1000)      531 2023-07-31 21:11:44.000000 Jetson.GPIO-2.1.2/lib/python/Jetson.GPIO.egg-info/SOURCES.txt
+-rw-rw-r--   0 lhoang    (1000) lhoang    (1000)        1 2023-07-31 21:11:44.000000 Jetson.GPIO-2.1.2/lib/python/Jetson.GPIO.egg-info/dependency_links.txt
+-rw-rw-r--   0 lhoang    (1000) lhoang    (1000)       11 2023-07-31 21:11:44.000000 Jetson.GPIO-2.1.2/lib/python/Jetson.GPIO.egg-info/top_level.txt
+drwxrwxr-x   0 lhoang    (1000) lhoang    (1000)        0 2023-07-31 21:11:44.098630 Jetson.GPIO-2.1.2/lib/python/RPi/
+drwxrwxr-x   0 lhoang    (1000) lhoang    (1000)        0 2023-07-31 21:11:44.098630 Jetson.GPIO-2.1.2/lib/python/RPi/GPIO/
+-rw-------   0 lhoang    (1000) lhoang    (1000)       44 2021-04-29 15:58:52.000000 Jetson.GPIO-2.1.2/lib/python/RPi/GPIO/__init__.py
+-rw-------   0 lhoang    (1000) lhoang    (1000)        1 2021-04-29 15:58:52.000000 Jetson.GPIO-2.1.2/lib/python/RPi/__init__.py
+-rw-rw-r--   0 lhoang    (1000) lhoang    (1000)       38 2023-07-31 21:11:44.098630 Jetson.GPIO-2.1.2/setup.cfg
+-rw-rw-r--   0 lhoang    (1000) lhoang    (1000)     2432 2023-07-31 21:04:38.000000 Jetson.GPIO-2.1.2/setup.py
```

### Comparing `Jetson.GPIO-2.1.1/LICENSE.txt` & `Jetson.GPIO-2.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Jetson.GPIO-2.1.1/PKG-INFO` & `Jetson.GPIO-2.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: Jetson.GPIO
-Version: 2.1.1
-Summary: A module to control Jetson GPIO channels
-Home-page: https://github.com/NVIDIA/jetson-gpio
-Author: NVIDIA
-Author-email: linux-tegra-bugs@nvidia.com
-License: MIT
-Keywords: Jetson GPIO
-Classifier: Operating System :: POSIX :: Linux
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development
-Classifier: Topic :: System :: Hardware
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # Jetson.GPIO - Linux for Tegra
 
 Jetson TX1, TX2, AGX Xavier, and Nano development boards contain a 40 pin GPIO
 header, similar to the 40 pin header in the Raspberry Pi. These GPIOs can be
 controlled for digital input and output using the Python library provided in the
 Jetson GPIO Library package. The library has the same API as the RPi.GPIO
 library for Raspberry Pi in order to provide an easy way to move applications
@@ -47,14 +28,16 @@
 and write to a GPIO pin respectively, while the `button_led.py`,
 `button_event.py` and `button_interrupt.py` show how a button press may be used
 to blink an LED using busy-waiting, blocking wait and interrupt callbacks
 respectively.
 
 # Installation
 
+These are the way to install Jetson.GPIO python modules on your system. For the samples applications, please clone this repository to your system. 
+
 ## Using pip
 
 The easiest way to install this library is using `pip`:
 ```shell
 sudo pip install Jetson.GPIO
 ```
 
@@ -378,21 +361,43 @@
 multiple events in to a single one, a debounce time can be optionally set:
 
 ```python
 # bouncetime set in milliseconds
 GPIO.add_event_detect(channel, GPIO.RISING, callback=callback_fn,
 bouncetime=200)
 ```
+The thread running in the background will be idle waiting for an event until
+timeout, which can be optionally set as the following. The default polling
+timeout is 0.2 sec. When the poll time times out, the thread will wake up and
+check the thread status. If the thread is in the running state, it will go back
+to the idle state waiting for another event, otherwise, the thread will exit
+(event detection removal). This process will go on until the thread is in the
+exit state.
+
+```python
+# polltime set in seconds
+GPIO.add_event_detect(channel, GPIO.RISING, callback=callback_fn,
+polltime=1)
+```
 
 If the edge detection is not longer required it can be removed as follows:
 
 ```python
 GPIO.remove_event_detect(channel)
 ```
 
+A timeout option can be set to wait for an event detection
+to be removed, or else it is 0.5 seconds by default. It is
+recommended that the timeout for removal should be at
+least twice as much as the poll time.
+
+```python
+GPIO.remove_event_detect(channel, timeout=0.5)
+```
+
 #### 10. Check function of GPIO channels
 
 This feature allows you to check the function of the provided GPIO channel:
 
 ```python
 GPIO.gpio_function(channel)
 ```
```

### Comparing `Jetson.GPIO-2.1.1/README.md` & `Jetson.GPIO-2.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: Jetson.GPIO
+Version: 2.1.2
+Summary: A module to control Jetson GPIO channels
+Home-page: https://github.com/NVIDIA/jetson-gpio
+Author: NVIDIA
+Author-email: linux-tegra-bugs@nvidia.com
+License: MIT
+Keywords: Jetson GPIO
+Classifier: Operating System :: POSIX :: Linux
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development
+Classifier: Topic :: System :: Hardware
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # Jetson.GPIO - Linux for Tegra
 
 Jetson TX1, TX2, AGX Xavier, and Nano development boards contain a 40 pin GPIO
 header, similar to the 40 pin header in the Raspberry Pi. These GPIOs can be
 controlled for digital input and output using the Python library provided in the
 Jetson GPIO Library package. The library has the same API as the RPi.GPIO
 library for Raspberry Pi in order to provide an easy way to move applications
@@ -28,14 +47,16 @@
 and write to a GPIO pin respectively, while the `button_led.py`,
 `button_event.py` and `button_interrupt.py` show how a button press may be used
 to blink an LED using busy-waiting, blocking wait and interrupt callbacks
 respectively.
 
 # Installation
 
+These are the way to install Jetson.GPIO python modules on your system. For the samples applications, please clone this repository to your system. 
+
 ## Using pip
 
 The easiest way to install this library is using `pip`:
 ```shell
 sudo pip install Jetson.GPIO
 ```
 
@@ -359,21 +380,43 @@
 multiple events in to a single one, a debounce time can be optionally set:
 
 ```python
 # bouncetime set in milliseconds
 GPIO.add_event_detect(channel, GPIO.RISING, callback=callback_fn,
 bouncetime=200)
 ```
+The thread running in the background will be idle waiting for an event until
+timeout, which can be optionally set as the following. The default polling
+timeout is 0.2 sec. When the poll time times out, the thread will wake up and
+check the thread status. If the thread is in the running state, it will go back
+to the idle state waiting for another event, otherwise, the thread will exit
+(event detection removal). This process will go on until the thread is in the
+exit state.
+
+```python
+# polltime set in seconds
+GPIO.add_event_detect(channel, GPIO.RISING, callback=callback_fn,
+polltime=1)
+```
 
 If the edge detection is not longer required it can be removed as follows:
 
 ```python
 GPIO.remove_event_detect(channel)
 ```
 
+A timeout option can be set to wait for an event detection
+to be removed, or else it is 0.5 seconds by default. It is
+recommended that the timeout for removal should be at
+least twice as much as the poll time.
+
+```python
+GPIO.remove_event_detect(channel, timeout=0.5)
+```
+
 #### 10. Check function of GPIO channels
 
 This feature allows you to check the function of the provided GPIO channel:
 
 ```python
 GPIO.gpio_function(channel)
 ```
```

### Comparing `Jetson.GPIO-2.1.1/lib/python/Jetson/GPIO/99-gpio.rules` & `Jetson.GPIO-2.1.2/lib/python/Jetson/GPIO/99-gpio.rules`

 * *Files identical despite different names*

### Comparing `Jetson.GPIO-2.1.1/lib/python/Jetson/GPIO/gpio.py` & `Jetson.GPIO-2.1.2/lib/python/Jetson/GPIO/gpio.py`

 * *Files 16% similar despite different names*

```diff
@@ -65,20 +65,26 @@
 OUT = 0
 IN = 1
 HARD_PWM = 43
 
 model, JETSON_INFO, _channel_data_by_mode = gpio_pin_data.get_data()
 RPI_INFO = JETSON_INFO
 
-# Dictionary objects used as lookup tables for pin to linux gpio mapping
+# Dictionary used as a lookup table for pin to its info object (_Gpios) mapping
+# key: channel, value: ChannelInfo object
 _channel_data = {}
 
 _gpio_warnings = True
 _gpio_mode = None
+
+# Dictionary used as a lookup table for pin to its configuration
+# key: channel, value: GPIO directions (IN/OUT deprecated)
 _channel_configuration = {}
+
+# Dictionary used as a lookup table from GPIO chip name to chip fd
 _chip_fd = {}
 
 
 def _validate_mode_set():
     if _gpio_mode is None:
         raise RuntimeError("Please set pin numbering mode using "
                            "GPIO.setmode(GPIO.BOARD), GPIO.setmode(GPIO.BCM), "
@@ -228,33 +234,46 @@
         f.write("1")
 
 
 def _disable_pwm(ch_info):
     with open(_pwm_enable_path(ch_info), 'w') as f:
         f.write("0")
 
-
+# Clean up all resources taken by a channel,
+# including pwm, chip and lines
 def _cleanup_one(ch_info):
     #clean up pwm config
     app_cfg = _channel_configuration[ch_info.channel]
     if app_cfg == HARD_PWM:
         _disable_pwm(ch_info)
         _unexport_pwm(ch_info)
+    else:
+        event.event_cleanup(ch_info.gpio_chip, ch_info.channel)
     del _channel_configuration[ch_info.channel]
+
     # clean gpio config
+    # clean up chip
+    if ch_info.chip_fd:
+        gpio_cdev.close_chip(ch_info.chip_fd)
+        ch_info.chip_fd = None
+        if ch_info.gpio_chip in _chip_fd:
+            del _chip_fd[ch_info.gpio_chip]
+
+    # clean up line
     if ch_info.line_handle:
         gpio_cdev.close_line(ch_info.line_handle)
         ch_info.line_handle = None
 
 
 def _cleanup_all():
     global _gpio_mode
 
     for channel in list(_channel_configuration.keys()):
         ch_info = _channel_to_info(channel)
+
         _cleanup_one(ch_info)
 
     _gpio_mode = None
 
 
 # Function used to enable/disable warnings during setup and cleanup.
 # Param -> state is a bool
@@ -399,16 +418,19 @@
     for ch_info, value in zip(ch_infos, values):
         gpio_cdev.set_value(ch_info.line_handle, value)
 
 
 # Function used to add threaded event detection for a specified gpio channel.
 # Param gpio must be an integer specifying the channel, edge must be RISING,
 # FALLING or BOTH. A callback function to be called when the event is detected
-# and an integer bounctime in milliseconds can be optionally provided
-def add_event_detect(channel, edge, callback=None, bouncetime=None):
+# and an integer bounctime in milliseconds can be optionally provided. A optional
+# polltime in second can be provided to indicate the max time waiting for an edge.
+# Note that one channel only allows one event, which the duplicated event will
+# be ignored.
+def add_event_detect(channel, edge, callback=None, bouncetime=None, polltime=0.2):
     ch_info = _channel_to_info(channel, need_gpio=True)
     if (not callable(callback)) and callback is not None:
         raise TypeError("Callback Parameter must be callable")
 
     # channel must be setup as input
     if _app_channel_configuration(ch_info) != IN:
         raise RuntimeError("You must setup() the GPIO channel as an input "
@@ -428,17 +450,64 @@
         elif bouncetime < 0:
             raise ValueError("bouncetime must be an integer greater than 0")
 
     if ch_info.line_handle:
         gpio_cdev.close_line(ch_info.line_handle)
 
     request = gpio_cdev.request_event(ch_info.line_offset, edge, ch_info.consumer)
-    gpio_cdev.add_edge_detect(ch_info.chip_fd, channel, request, callback, bouncetime)
+    event.add_edge_detect(ch_info.chip_fd, ch_info.gpio_chip, channel, request, bouncetime, polltime)
+
+    if callback is not None:
+        event.add_edge_callback(ch_info.gpio_chip, channel, lambda: callback(channel))
+
+    # We should wait until the thread is up, which the device buffer cleaning takes time
+    time.sleep(1)
+
+# Function used to remove event detection for channel
+# Timeout param for the max time to wait for thread (event detecion) to end
+def remove_event_detect(channel, timeout=0.5):
+    ch_info = _channel_to_info(channel, need_gpio=True)
+    event.remove_edge_detect(ch_info.gpio_chip, channel, timeout)
+
+
+# Function used to check if an event occurred on the specified channel.
+# Param channel must be an integer.
+# This function return True or False
+def event_detected(channel):
+    ch_info = _channel_to_info(channel, need_gpio=True)
+
+    # channel must be setup as input
+    if _app_channel_configuration(ch_info) != IN:
+        raise RuntimeError("You must setup() the GPIO channel as an "
+                           "input first")
 
+    return event.edge_event_detected(ch_info.gpio_chip, channel)
+
+
+# Function used to add a callback function to channel, after it has been
+# registered for events using add_event_detect()
+def add_event_callback(channel, callback):
+    ch_info = _channel_to_info(channel, need_gpio=True)
+    if not callable(callback):
+        raise TypeError("Parameter must be callable")
 
+    if _app_channel_configuration(ch_info) != IN:
+        raise RuntimeError("You must setup() the GPIO channel as an "
+                           "input first")
+
+    if not event.gpio_event_added(ch_info.gpio_chip, channel):
+        raise RuntimeError("Add event detection using add_event_detect first "
+                           "before adding a callback")
+
+    event.add_edge_callback(ch_info.gpio_chip, channel, lambda: callback(channel))
+
+    # We should wait until the thread is up, which the device buffer cleaning takes time
+    time.sleep(1)
+
+# Function used to wait for a edge event in blocking mode, it is also one-shoot.
 def wait_for_edge(channel, edge, bouncetime=None, timeout=None):
     ch_info = _channel_to_info(channel, need_gpio=True)
 
     # channel must be setup as input
     if _app_channel_configuration(ch_info) != IN:
         raise RuntimeError("You must setup() the GPIO channel as an input "
                            "first")
@@ -466,15 +535,41 @@
         elif timeout < 0:
             raise ValueError("Timeout must greater than 0")
 
     if ch_info.line_handle:
         gpio_cdev.close_line(ch_info.line_handle)
 
     request = gpio_cdev.request_event(ch_info.line_offset, edge, ch_info.consumer)
-    gpio_cdev.blocking_wait_for_edge(ch_info.chip_fd, channel, request, bouncetime, timeout)
+    result = event.blocking_wait_for_edge(ch_info.chip_fd, ch_info.gpio_chip, channel, request, bouncetime, timeout)
+
+    # If not error, result == channel. If timeout occurs while waiting,
+    # result == None. If error occurs, result == -1 means channel is
+    # registered for conflicting edge detection, result == -2 means an error
+    # occurred while registering event or polling
+    if not result:
+        return None
+    elif result == -1:
+        raise RuntimeError("Conflicting edge detection event already exists "
+                           "for this GPIO channel")
+
+    elif result == -2:
+        raise RuntimeError("Error waiting for edge")
+
+    return channel
+
+
+# Function used to check the currently set function of the channel specified.
+# Param channel must be an integers. The function returns either IN, OUT,
+# or UNKNOWN
+def gpio_function(channel):
+    ch_info = _channel_to_info(channel)
+    func = _app_channel_configuration(ch_info)
+    if func is None:
+        func = UNKNOWN
+    return func
 
 
 class PWM(object):
     def __init__(self, channel, frequency_hz):
         self._ch_info = _channel_to_info(channel, need_pwm=True)
 
         app_cfg = _app_channel_configuration(self._ch_info)
```

### Comparing `Jetson.GPIO-2.1.1/lib/python/Jetson/GPIO/gpio_pin_data.py` & `Jetson.GPIO-2.1.2/lib/python/Jetson/GPIO/gpio_pin_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     (134, 'PZ.04', "tegra234-gpio", 21, 9, 'SPI0_MISO', 'GP48_SPI1_MISO', None, None),
     (123, 'PY.01', "tegra234-gpio", 22, 25, 'SPI1_MISO', 'GP37_SPI3_MISO', None, None),
     (133, 'PZ.03', "tegra234-gpio", 23, 11, 'SPI0_SCK', 'GP47_SPI1_CLK', None, None),
     (136, 'PZ.06', "tegra234-gpio", 24, 8, 'SPI0_CS0', 'GP50_SPI1_CS0_N', None, None),
     (137, 'PZ.07', "tegra234-gpio", 26, 7, 'SPI0_CS1', 'GP51_SPI1_CS1_N', None, None),
     (105, 'PQ.05', "tegra234-gpio", 29, 5, 'GPIO01', 'GP65', None, None),
     (106, 'PQ.06', "tegra234-gpio", 31, 6, 'GPIO11', 'GP66', None, None),
-    (41, 'PG.06', "tegra234-gpio", 32, 12, 'GPIO07', 'GP113_PWM7', None, None),
+    (41, 'PG.06', "tegra234-gpio", 32, 12, 'GPIO07', 'GP113_PWM7', '32e0000.pwm', 0),
     (43, 'PH.00', "tegra234-gpio", 33, 13, 'GPIO13', 'GP115', '32c0000.pwm', 0),
     (53, 'PI.02', "tegra234-gpio", 35, 19, 'I2S0_FS', 'GP125', None, None),
     (113, 'PR.05', "tegra234-gpio", 36, 16, 'UART1_CTS', 'GP73_UART1_CTS_N', None, None),
     (124, 'PY.02', "tegra234-gpio", 37, 26, 'SPI1_MOSI', 'GP38_SPI3_MOSI', None, None),
     (52, 'PI.01', "tegra234-gpio", 38, 20, 'I2S0_SDIN', 'GP124', None, None),
     (51, 'PI.00', "tegra234-gpio", 40, 21, 'I2S0_SDOUT', 'GP123', None, None)
 ]
@@ -461,14 +461,23 @@
             'PROCESSOR': 'ARM A57'
         }
     ),
 }
 
 
 class ChannelInfo(object):
+    # @channel the pin number in specified mode (board or bcm)
+    # @chip_fd the file descriptor of the chip 
+    # @line_handle the file descriptor of the line
+    # @line_offset Linux GPIO pin number (line offset inside chip, not global)
+    # @direction the direction of a pin is configured (in or out)
+    # @edge rising and/or falling edge being monitored
+    # @consumer consumer label
+    # @gpio_name Linux exported GPIO name
+    # @gpio_chip GPIO chip name/instance
     def __init__(self, channel, line_offset, gpio_name, gpio_chip, pwm_chip_dir, pwm_id):
         self.channel = channel
         self.chip_fd = None
         self.line_handle = None
         self.line_offset = line_offset
         self.direction = None
         self.edge = None
@@ -585,15 +594,18 @@
             return model_name
         else:
             msg = f"Environment variable 'JETSON_MODEL_NAME={model_name}' is invalid."
             sys.stderr.write(msg)
 
     raise Exception('Could not determine Jetson model')
 
-
+# @brief Retrieve all the data before connecting to any ports
+# @param[out] model: model number of an Jetson platform
+# @param[out] jetson_info:
+# @param[out] channel_info: the information related to pin/line, in
 def get_data():
     model = get_model()
 
     pin_defs, jetson_info = jetson_gpio_data[model]
     gpio_chip_dirs = {}
     gpio_chip_base = {}
     gpio_chip_ngpio = {}
```

### Comparing `Jetson.GPIO-2.1.1/lib/python/Jetson.GPIO.egg-info/PKG-INFO` & `Jetson.GPIO-2.1.2/lib/python/Jetson.GPIO.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jetson.GPIO
-Version: 2.1.1
+Version: 2.1.2
 Summary: A module to control Jetson GPIO channels
 Home-page: https://github.com/NVIDIA/jetson-gpio
 Author: NVIDIA
 Author-email: linux-tegra-bugs@nvidia.com
 License: MIT
 Keywords: Jetson GPIO
 Classifier: Operating System :: POSIX :: Linux
@@ -47,14 +47,16 @@
 and write to a GPIO pin respectively, while the `button_led.py`,
 `button_event.py` and `button_interrupt.py` show how a button press may be used
 to blink an LED using busy-waiting, blocking wait and interrupt callbacks
 respectively.
 
 # Installation
 
+These are the way to install Jetson.GPIO python modules on your system. For the samples applications, please clone this repository to your system. 
+
 ## Using pip
 
 The easiest way to install this library is using `pip`:
 ```shell
 sudo pip install Jetson.GPIO
 ```
 
@@ -378,21 +380,43 @@
 multiple events in to a single one, a debounce time can be optionally set:
 
 ```python
 # bouncetime set in milliseconds
 GPIO.add_event_detect(channel, GPIO.RISING, callback=callback_fn,
 bouncetime=200)
 ```
+The thread running in the background will be idle waiting for an event until
+timeout, which can be optionally set as the following. The default polling
+timeout is 0.2 sec. When the poll time times out, the thread will wake up and
+check the thread status. If the thread is in the running state, it will go back
+to the idle state waiting for another event, otherwise, the thread will exit
+(event detection removal). This process will go on until the thread is in the
+exit state.
+
+```python
+# polltime set in seconds
+GPIO.add_event_detect(channel, GPIO.RISING, callback=callback_fn,
+polltime=1)
+```
 
 If the edge detection is not longer required it can be removed as follows:
 
 ```python
 GPIO.remove_event_detect(channel)
 ```
 
+A timeout option can be set to wait for an event detection
+to be removed, or else it is 0.5 seconds by default. It is
+recommended that the timeout for removal should be at
+least twice as much as the poll time.
+
+```python
+GPIO.remove_event_detect(channel, timeout=0.5)
+```
+
 #### 10. Check function of GPIO channels
 
 This feature allows you to check the function of the provided GPIO channel:
 
 ```python
 GPIO.gpio_function(channel)
 ```
```

### Comparing `Jetson.GPIO-2.1.1/lib/python/Jetson.GPIO.egg-info/SOURCES.txt` & `Jetson.GPIO-2.1.2/lib/python/Jetson.GPIO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Jetson.GPIO-2.1.1/setup.py` & `Jetson.GPIO-2.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
                'Intended Audience :: Developers',
                'Programming Language :: Python :: 2.7',
                'Programming Language :: Python :: 3',
                'Topic :: Software Development',
                'Topic :: System :: Hardware']
 
 setup(name                          = 'Jetson.GPIO',
-      version                       = '2.1.1',
+      version                       = '2.1.2',
       author                        = 'NVIDIA',
       author_email                  = 'linux-tegra-bugs@nvidia.com',
       description                   = 'A module to control Jetson GPIO channels',
       long_description              = open('README.md').read(),
       long_description_content_type = 'text/markdown',
       license                       = 'MIT',
       keywords                      = 'Jetson GPIO',
```

