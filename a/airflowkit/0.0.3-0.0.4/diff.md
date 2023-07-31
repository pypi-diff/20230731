# Comparing `tmp/airflowkit-0.0.3.tar.gz` & `tmp/airflowkit-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflowkit-0.0.3.tar", last modified: Thu Jul 27 09:42:56 2023, max compression
+gzip compressed data, was "airflowkit-0.0.4.tar", last modified: Mon Jul 31 13:47:06 2023, max compression
```

## Comparing `airflowkit-0.0.3.tar` & `airflowkit-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-07-27 09:42:56.475052 airflowkit-0.0.3/
--rw-r--r--   0 marc       (501) staff       (20)      458 2023-07-27 09:42:03.000000 airflowkit-0.0.3/CHANGELOG.md
--rw-r--r--   0 marc       (501) staff       (20)     1069 2023-03-25 13:22:59.000000 airflowkit-0.0.3/LICENSE
--rw-r--r--   0 marc       (501) staff       (20)       21 2023-03-25 13:22:59.000000 airflowkit-0.0.3/MANIFEST.in
--rw-r--r--   0 marc       (501) staff       (20)      460 2023-07-27 09:42:56.474911 airflowkit-0.0.3/PKG-INFO
--rw-r--r--   0 marc       (501) staff       (20)      142 2023-03-25 13:25:40.000000 airflowkit-0.0.3/README.md
--rw-r--r--   0 marc       (501) staff       (20)       38 2023-07-27 09:42:56.475094 airflowkit-0.0.3/setup.cfg
--rw-r--r--   0 marc       (501) staff       (20)     1043 2023-07-27 09:41:18.000000 airflowkit-0.0.3/setup.py
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-07-27 09:42:56.472218 airflowkit-0.0.3/src/
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-07-27 09:42:56.473331 airflowkit-0.0.3/src/airflowkit/
--rw-r--r--   0 marc       (501) staff       (20)        0 2023-03-25 13:33:15.000000 airflowkit-0.0.3/src/airflowkit/__init__.py
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-07-27 09:42:56.474316 airflowkit-0.0.3/src/airflowkit/sensors/
--rw-r--r--   0 marc       (501) staff       (20)        0 2023-03-25 13:27:19.000000 airflowkit-0.0.3/src/airflowkit/sensors/__init__.py
--rw-r--r--   0 marc       (501) staff       (20)     4536 2023-07-27 08:27:10.000000 airflowkit-0.0.3/src/airflowkit/sensors/gcs_any_objects_existence_async_sensor.py
--rw-r--r--   0 marc       (501) staff       (20)     4501 2023-07-27 08:17:47.000000 airflowkit-0.0.3/src/airflowkit/sensors/gcs_objects_existence_async_sensor.py
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-07-27 09:42:56.474641 airflowkit-0.0.3/src/airflowkit/triggers/
--rw-r--r--   0 marc       (501) staff       (20)        0 2023-03-25 13:27:19.000000 airflowkit-0.0.3/src/airflowkit/triggers/__init__.py
--rw-r--r--   0 marc       (501) staff       (20)     3625 2023-07-27 08:26:10.000000 airflowkit-0.0.3/src/airflowkit/triggers/gcs_any_blobs_trigger.py
--rw-r--r--   0 marc       (501) staff       (20)     3566 2023-07-27 09:28:44.000000 airflowkit-0.0.3/src/airflowkit/triggers/gcs_blobs_trigger.py
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-07-27 09:42:56.473947 airflowkit-0.0.3/src/airflowkit.egg-info/
--rw-r--r--   0 marc       (501) staff       (20)      460 2023-07-27 09:42:56.000000 airflowkit-0.0.3/src/airflowkit.egg-info/PKG-INFO
--rw-r--r--   0 marc       (501) staff       (20)      580 2023-07-27 09:42:56.000000 airflowkit-0.0.3/src/airflowkit.egg-info/SOURCES.txt
--rw-r--r--   0 marc       (501) staff       (20)        1 2023-07-27 09:42:56.000000 airflowkit-0.0.3/src/airflowkit.egg-info/dependency_links.txt
--rw-r--r--   0 marc       (501) staff       (20)       62 2023-07-27 09:42:56.000000 airflowkit-0.0.3/src/airflowkit.egg-info/requires.txt
--rw-r--r--   0 marc       (501) staff       (20)       11 2023-07-27 09:42:56.000000 airflowkit-0.0.3/src/airflowkit.egg-info/top_level.txt
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-07-27 09:42:56.474753 airflowkit-0.0.3/tests/
--rw-r--r--   0 marc       (501) staff       (20)      215 2023-03-25 13:47:24.000000 airflowkit-0.0.3/tests/test_imports.py
+drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-07-31 13:47:06.129293 airflowkit-0.0.4/
+-rw-r--r--   0 marc       (501) staff       (20)      562 2023-07-31 13:41:44.000000 airflowkit-0.0.4/CHANGELOG.md
+-rw-r--r--   0 marc       (501) staff       (20)     1069 2023-03-25 13:22:59.000000 airflowkit-0.0.4/LICENSE
+-rw-r--r--   0 marc       (501) staff       (20)       21 2023-03-25 13:22:59.000000 airflowkit-0.0.4/MANIFEST.in
+-rw-r--r--   0 marc       (501) staff       (20)      460 2023-07-31 13:47:06.129142 airflowkit-0.0.4/PKG-INFO
+-rw-r--r--   0 marc       (501) staff       (20)      142 2023-03-25 13:25:40.000000 airflowkit-0.0.4/README.md
+-rw-r--r--   0 marc       (501) staff       (20)       38 2023-07-31 13:47:06.129334 airflowkit-0.0.4/setup.cfg
+-rw-r--r--   0 marc       (501) staff       (20)     1043 2023-07-27 09:41:18.000000 airflowkit-0.0.4/setup.py
+drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-07-31 13:47:06.125578 airflowkit-0.0.4/src/
+drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-07-31 13:47:06.126709 airflowkit-0.0.4/src/airflowkit/
+-rw-r--r--   0 marc       (501) staff       (20)        0 2023-03-25 13:33:15.000000 airflowkit-0.0.4/src/airflowkit/__init__.py
+drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-07-31 13:47:06.127925 airflowkit-0.0.4/src/airflowkit/sensors/
+-rw-r--r--   0 marc       (501) staff       (20)        0 2023-03-25 13:27:19.000000 airflowkit-0.0.4/src/airflowkit/sensors/__init__.py
+-rw-r--r--   0 marc       (501) staff       (20)     4556 2023-07-27 14:29:35.000000 airflowkit-0.0.4/src/airflowkit/sensors/gcs_any_objects_existence_async_sensor.py
+-rw-r--r--   0 marc       (501) staff       (20)     4501 2023-07-27 08:17:47.000000 airflowkit-0.0.4/src/airflowkit/sensors/gcs_objects_existence_async_sensor.py
+drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-07-31 13:47:06.128580 airflowkit-0.0.4/src/airflowkit/triggers/
+-rw-r--r--   0 marc       (501) staff       (20)        0 2023-03-25 13:27:19.000000 airflowkit-0.0.4/src/airflowkit/triggers/__init__.py
+-rw-r--r--   0 marc       (501) staff       (20)     3652 2023-07-31 13:40:51.000000 airflowkit-0.0.4/src/airflowkit/triggers/gcs_any_blobs_trigger.py
+-rw-r--r--   0 marc       (501) staff       (20)     3566 2023-07-27 09:28:44.000000 airflowkit-0.0.4/src/airflowkit/triggers/gcs_blobs_trigger.py
+drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-07-31 13:47:06.127333 airflowkit-0.0.4/src/airflowkit.egg-info/
+-rw-r--r--   0 marc       (501) staff       (20)      460 2023-07-31 13:47:06.000000 airflowkit-0.0.4/src/airflowkit.egg-info/PKG-INFO
+-rw-r--r--   0 marc       (501) staff       (20)      580 2023-07-31 13:47:06.000000 airflowkit-0.0.4/src/airflowkit.egg-info/SOURCES.txt
+-rw-r--r--   0 marc       (501) staff       (20)        1 2023-07-31 13:47:06.000000 airflowkit-0.0.4/src/airflowkit.egg-info/dependency_links.txt
+-rw-r--r--   0 marc       (501) staff       (20)       62 2023-07-31 13:47:06.000000 airflowkit-0.0.4/src/airflowkit.egg-info/requires.txt
+-rw-r--r--   0 marc       (501) staff       (20)       11 2023-07-31 13:47:06.000000 airflowkit-0.0.4/src/airflowkit.egg-info/top_level.txt
+drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-07-31 13:47:06.128837 airflowkit-0.0.4/tests/
+-rw-r--r--   0 marc       (501) staff       (20)      215 2023-03-25 13:47:24.000000 airflowkit-0.0.4/tests/test_imports.py
```

### Comparing `airflowkit-0.0.3/LICENSE` & `airflowkit-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `airflowkit-0.0.3/setup.py` & `airflowkit-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `airflowkit-0.0.3/src/airflowkit/sensors/gcs_any_objects_existence_async_sensor.py` & `airflowkit-0.0.4/src/airflowkit/sensors/gcs_any_objects_existence_async_sensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,13 +107,13 @@
         Callback for when the trigger fires - returns immediately.
         Relies on trigger to throw an exception, otherwise it assumes execution was
         successful.
         """
         if event["status"] == "error":
             raise AirflowException(event["message"])
         self.log.info(
-            "%d files %s were found in bucket %s.",
+            "At least one of the %d files %s were found in bucket %s.",
             len(self.objects),
             self.objects,
             self.bucket,
         )
         return event["message"]
```

### Comparing `airflowkit-0.0.3/src/airflowkit/sensors/gcs_objects_existence_async_sensor.py` & `airflowkit-0.0.4/src/airflowkit/sensors/gcs_objects_existence_async_sensor.py`

 * *Files identical despite different names*

### Comparing `airflowkit-0.0.3/src/airflowkit/triggers/gcs_any_blobs_trigger.py` & `airflowkit-0.0.4/src/airflowkit/triggers/gcs_any_blobs_trigger.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,10 +84,10 @@
                 if object_response:
                     self.log.debug(f"Found GCS blob {object_name}!")
                     responses.append(True)
                 else:
                     self.log.debug(f"Not found GCS blob: {object_name}!")
                     responses.append(False)
 
-            if any(responses):
+            if any(responses) or len(objects_names) == 0:
                 return "success"
             return "pending"
```

### Comparing `airflowkit-0.0.3/src/airflowkit/triggers/gcs_blobs_trigger.py` & `airflowkit-0.0.4/src/airflowkit/triggers/gcs_blobs_trigger.py`

 * *Files identical despite different names*

### Comparing `airflowkit-0.0.3/src/airflowkit.egg-info/SOURCES.txt` & `airflowkit-0.0.4/src/airflowkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

