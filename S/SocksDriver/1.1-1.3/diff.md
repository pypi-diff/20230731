# Comparing `tmp/SocksDriver-1.1.tar.gz` & `tmp/SocksDriver-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SocksDriver-1.1.tar", last modified: Thu Jul 27 06:35:01 2023, max compression
+gzip compressed data, was "SocksDriver-1.3.tar", last modified: Mon Jul 31 09:30:37 2023, max compression
```

## Comparing `SocksDriver-1.1.tar` & `SocksDriver-1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 dsw       (1000) dsw       (1000)        0 2023-07-27 06:35:01.061635 SocksDriver-1.1/
--rw-r--r--   0 dsw       (1000) dsw       (1000)     1068 2023-07-25 21:34:45.000000 SocksDriver-1.1/LICENSE
--rw-r--r--   0 dsw       (1000) dsw       (1000)      419 2023-07-27 06:35:01.060637 SocksDriver-1.1/PKG-INFO
--rw-r--r--   0 dsw       (1000) dsw       (1000)       60 2023-07-27 06:33:28.000000 SocksDriver-1.1/README.md
-drwxr-xr-x   0 dsw       (1000) dsw       (1000)        0 2023-07-27 06:35:01.036701 SocksDriver-1.1/SocksDriver/
--rw-r--r--   0 dsw       (1000) dsw       (1000)       43 2023-07-23 10:49:49.000000 SocksDriver-1.1/SocksDriver/__init__.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)     8403 2023-07-27 06:33:28.000000 SocksDriver-1.1/SocksDriver/client.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)      483 2023-07-24 10:07:13.000000 SocksDriver-1.1/SocksDriver/complex_types.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)      249 2023-07-24 07:59:31.000000 SocksDriver-1.1/SocksDriver/errors.py
-drwxr-xr-x   0 dsw       (1000) dsw       (1000)        0 2023-07-27 06:35:01.044680 SocksDriver-1.1/SocksDriver.egg-info/
--rw-r--r--   0 dsw       (1000) dsw       (1000)      419 2023-07-27 06:35:01.000000 SocksDriver-1.1/SocksDriver.egg-info/PKG-INFO
--rw-r--r--   0 dsw       (1000) dsw       (1000)      559 2023-07-27 06:35:01.000000 SocksDriver-1.1/SocksDriver.egg-info/SOURCES.txt
--rw-r--r--   0 dsw       (1000) dsw       (1000)        1 2023-07-27 06:35:01.000000 SocksDriver-1.1/SocksDriver.egg-info/dependency_links.txt
--rw-r--r--   0 dsw       (1000) dsw       (1000)       12 2023-07-27 06:35:01.000000 SocksDriver-1.1/SocksDriver.egg-info/top_level.txt
--rw-r--r--   0 dsw       (1000) dsw       (1000)      425 2023-07-27 06:33:28.000000 SocksDriver-1.1/pyproject.toml
--rw-r--r--   0 dsw       (1000) dsw       (1000)       38 2023-07-27 06:35:01.061635 SocksDriver-1.1/setup.cfg
-drwxr-xr-x   0 dsw       (1000) dsw       (1000)        0 2023-07-27 06:35:01.059639 SocksDriver-1.1/tests/
--rw-r--r--   0 dsw       (1000) dsw       (1000)     2090 2023-07-24 09:58:57.000000 SocksDriver-1.1/tests/test_command_blockdev.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)      703 2023-07-27 06:33:28.000000 SocksDriver-1.1/tests/test_command_help.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)      329 2023-07-25 07:34:53.000000 SocksDriver-1.1/tests/test_command_meminfo.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)      290 2023-07-24 09:12:37.000000 SocksDriver-1.1/tests/test_command_sleep.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)      469 2023-07-24 09:12:17.000000 SocksDriver-1.1/tests/test_command_sysinfo.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)      564 2023-07-24 09:11:50.000000 SocksDriver-1.1/tests/test_command_uptime.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)      231 2023-07-27 06:33:28.000000 SocksDriver-1.1/tests/test_command_version.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)      514 2023-07-25 06:00:12.000000 SocksDriver-1.1/tests/test_connect_disconnect.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)     1381 2023-07-25 04:53:01.000000 SocksDriver-1.1/tests/test_error_handling.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)     2732 2023-07-23 12:30:43.000000 SocksDriver-1.1/tests/test_protocol.py
+drwxr-xr-x   0 dsw       (1000) dsw       (1000)        0 2023-07-31 09:30:37.920050 SocksDriver-1.3/
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     1068 2023-07-25 21:34:45.000000 SocksDriver-1.3/LICENSE
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      419 2023-07-31 09:30:37.918056 SocksDriver-1.3/PKG-INFO
+-rw-r--r--   0 dsw       (1000) dsw       (1000)       60 2023-07-27 06:33:28.000000 SocksDriver-1.3/README.md
+drwxr-xr-x   0 dsw       (1000) dsw       (1000)        0 2023-07-31 09:30:37.885144 SocksDriver-1.3/SocksDriver/
+-rw-r--r--   0 dsw       (1000) dsw       (1000)       43 2023-07-23 10:49:49.000000 SocksDriver-1.3/SocksDriver/__init__.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     8366 2023-07-31 09:21:44.000000 SocksDriver-1.3/SocksDriver/client.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      483 2023-07-24 10:07:13.000000 SocksDriver-1.3/SocksDriver/complex_types.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      249 2023-07-24 07:59:31.000000 SocksDriver-1.3/SocksDriver/errors.py
+drwxr-xr-x   0 dsw       (1000) dsw       (1000)        0 2023-07-31 09:30:37.897112 SocksDriver-1.3/SocksDriver.egg-info/
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      419 2023-07-31 09:30:37.000000 SocksDriver-1.3/SocksDriver.egg-info/PKG-INFO
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      559 2023-07-31 09:30:37.000000 SocksDriver-1.3/SocksDriver.egg-info/SOURCES.txt
+-rw-r--r--   0 dsw       (1000) dsw       (1000)        1 2023-07-31 09:30:37.000000 SocksDriver-1.3/SocksDriver.egg-info/dependency_links.txt
+-rw-r--r--   0 dsw       (1000) dsw       (1000)       12 2023-07-31 09:30:37.000000 SocksDriver-1.3/SocksDriver.egg-info/top_level.txt
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      425 2023-07-31 09:29:08.000000 SocksDriver-1.3/pyproject.toml
+-rw-r--r--   0 dsw       (1000) dsw       (1000)       38 2023-07-31 09:30:37.920050 SocksDriver-1.3/setup.cfg
+drwxr-xr-x   0 dsw       (1000) dsw       (1000)        0 2023-07-31 09:30:37.916062 SocksDriver-1.3/tests/
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     2090 2023-07-24 09:58:57.000000 SocksDriver-1.3/tests/test_command_blockdev.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      703 2023-07-27 06:33:28.000000 SocksDriver-1.3/tests/test_command_help.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      329 2023-07-25 07:34:53.000000 SocksDriver-1.3/tests/test_command_meminfo.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      290 2023-07-24 09:12:37.000000 SocksDriver-1.3/tests/test_command_sleep.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      469 2023-07-24 09:12:17.000000 SocksDriver-1.3/tests/test_command_sysinfo.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      564 2023-07-24 09:11:50.000000 SocksDriver-1.3/tests/test_command_uptime.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      231 2023-07-27 06:33:28.000000 SocksDriver-1.3/tests/test_command_version.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      514 2023-07-25 06:00:12.000000 SocksDriver-1.3/tests/test_connect_disconnect.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     1381 2023-07-25 04:53:01.000000 SocksDriver-1.3/tests/test_error_handling.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     3632 2023-07-27 08:58:49.000000 SocksDriver-1.3/tests/test_protocol.py
```

### Comparing `SocksDriver-1.1/LICENSE` & `SocksDriver-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `SocksDriver-1.1/SocksDriver/client.py` & `SocksDriver-1.3/SocksDriver/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -190,31 +190,33 @@
             results = loads(results_s)
         except JSONDecodeError as exc:
             raise SocksTransmissionError('Could not decode data. Buffer size is possibly too small') from exc
 
         if results['status'] != 'Success':
             raise SocksInternalServerError(results['status'])
 
-        devices = []
+        devices: list[complex_types.TYPE_BLOCKDEV] = []
 
-        for i in range(int(results['num_devices'])):
-            device: complex_types.TYPE_BLOCKDEV = {
-                'avail_blocks': int(results[f'available_blocks_{i}']),
-                'avail_size': int(results[f'available_size_{i}']),
-                'block_size': int(results[f'block_size_{i}']),
-                'fstype': results[f'filesystem_type_{i}'],
+        if not results['devices']:
+            return devices
+
+        for device in results['devices']:
+            devices.append({
+                'avail_blocks': results[device]['available_blocks'],
+                'avail_size': results[device]['available_size'],
+                'block_size': results[device]['block_size'],
+                'fstype': results[device]['filesystem_type'],
                 'host': results['host'],
-                'mounted_device': results[f'mounted_device_{i}'],
-                'mountpoint': results[f'mountpoint_{i}'],
-                'name': results[f'name_{i}'],
-                'path': results[f'path_{i}'],
-                'total_blocks': int(results[f'total_blocks_{i}']),
-                'total_size': int(results[f'total_size_{i}']),
-            }
-            devices.append(device)
+                'mounted_device': results[device]['mounted_device'],
+                'mountpoint': results[device]['mountpoint'],
+                'name': device,
+                'path': results[device]['path'],
+                'total_blocks': results[device]['total_blocks'],
+                'total_size': results[device]['total_size'],
+            })
 
         return devices
 
     def meminfo(self) -> complex_types.TYPE_MEMINFO:
 
         """Ask peer to list virtual memory.
 
@@ -231,15 +233,14 @@
             raise SocksTransmissionError('Could not decode data. Buffer size is possibly too small') from exc
 
         if results['status'] != 'Success':
             raise SocksInternalServerError(results['status'])
 
         del results['status']
 
-        results['totalram'] = int(results['totalram'])
         return results
 
     def version(self) -> dict[str, str]:
 
         """Ask peer to return the ChristmasSocks server version.
 
         :return dict[str, str]
```

### Comparing `SocksDriver-1.1/SocksDriver.egg-info/SOURCES.txt` & `SocksDriver-1.3/SocksDriver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SocksDriver-1.1/tests/test_command_blockdev.py` & `SocksDriver-1.3/tests/test_command_blockdev.py`

 * *Files identical despite different names*

### Comparing `SocksDriver-1.1/tests/test_command_help.py` & `SocksDriver-1.3/tests/test_command_help.py`

 * *Files identical despite different names*

### Comparing `SocksDriver-1.1/tests/test_command_uptime.py` & `SocksDriver-1.3/tests/test_command_uptime.py`

 * *Files identical despite different names*

### Comparing `SocksDriver-1.1/tests/test_connect_disconnect.py` & `SocksDriver-1.3/tests/test_connect_disconnect.py`

 * *Files identical despite different names*

### Comparing `SocksDriver-1.1/tests/test_error_handling.py` & `SocksDriver-1.3/tests/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `SocksDriver-1.1/tests/test_protocol.py` & `SocksDriver-1.3/tests/test_protocol.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from json import loads
 from random import choice
 from string import ascii_letters, digits, punctuation
 from pytest import mark
 from SocksDriver import SocksClient
 
 ALPHANUMERIC = ascii_letters + digits
 
@@ -20,46 +21,65 @@
         result.append(''.join(choice(punctuation) for _ in range(len_strings)))
 
     return result
 
 # OS specific line break tests
 
 def test_handle_line_feed(client: SocksClient) -> None:
-    assert client.send('foobar\n') == 'foobar\n'
+    result = loads(client.send('foobar\nabc'))
+    assert result['status'] == 'foobar\nabc'
+
+def test_handle_line_feed_strip_newline(client: SocksClient) -> None:
+    result = loads(client.send('foobar\n'))
+    assert result['status'] == 'foobar'
 
 def test_handle_carriage_return(client: SocksClient) -> None:
-    assert client.send('foobar\r') == 'foobar\r'
+    result = loads(client.send('foobar\rabc'))
+    assert result['status'] == 'foobar\rabc'
 
-def test_handle_end_of_line(client: SocksClient) -> None:
-    assert client.send('foobar\r\n') == 'foobar\r\n'
+def test_handle_carriage_return_strip_carriage_return(client: SocksClient) -> None:
+    result = loads(client.send('foobar\r'))
+    assert result['status'] == 'foobar'
+
+@mark.xfail(reason='The nlohmann/json library strips the newline but not the carriage return')
+def test_handle_end_of_line_strip_end_of_line(client: SocksClient) -> None:
+    result = loads(client.send('foobar\r\n'))
+    assert result['status'] == 'foobar'
 
-def test_handle_no_line_break(client: SocksClient) -> None:
-    assert client.send('foobar') == 'foobar'
+def test_handle_end_of_line(client: SocksClient) -> None:
+    result = loads(client.send('foobar\r\nabc'))
+    assert result['status'] == 'foobar\r\nabc'
 
 # Test "empty" messages
 # Note that a true empty message, '', would be considered an EOF / hangup by the server
 
 def test_handle_single_line_feed(client: SocksClient) -> None:
-    assert client.send('\n') == '\n'
+    result = loads(client.send('\n'))
+    assert result['status'] == ''
 
 def test_handle_single_carriage_return(client: SocksClient) -> None:
-    assert client.send('\r') == '\r'
+    result = loads(client.send('\r'))
+    assert result['status'] == ''
 
+@mark.xfail(reason='The nlohmann/json library strips the newline but not the carriage return')
 def test_handle_single_end_of_line(client: SocksClient) -> None:
-    assert client.send('\r\n') == '\r\n'
+    result = loads(client.send('\r\n'))
+    assert result['status'] == ''
 
 # Echo tests
 
 @mark.parametrize('string', generate_random_string(num_strings=10, len_strings=15))
 def test_echo_15_byte_string(client: SocksClient, string: str) -> None:
-    assert string == client.send(string)
+    result = loads(client.send(string))
+    assert string == result['status']
 
 @mark.parametrize('string', generate_random_punctuation(num_strings=10, len_strings=15))
 def test_echo_15_byte_punctuation(client: SocksClient, string: str) -> None:
-    assert string == client.send(string)
+    result = loads(client.send(string))
+    assert string == result['status']
 
 @mark.skip(reason='Driver does not know how to handle buffer overflow')
 def test_echo_max_size_minus_one_byte_string(client: SocksClient) -> None:
 
     string = generate_random_string(num_strings=1, len_strings=client.BUFFER_SIZE)
     assert string[0] == client.send(string[0])
```

