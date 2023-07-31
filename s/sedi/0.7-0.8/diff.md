# Comparing `tmp/sedi-0.7.tar.gz` & `tmp/sedi-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sedi-0.7.tar", last modified: Sat Jul 29 13:40:17 2023, max compression
+gzip compressed data, was "sedi-0.8.tar", last modified: Sat Jul 29 13:44:22 2023, max compression
```

## Comparing `sedi-0.7.tar` & `sedi-0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 aleksa    (1000) aleksa    (1000)        0 2023-07-29 13:40:17.897451 sedi-0.7/
--rw-rw-r--   0 aleksa    (1000) aleksa    (1000)      127 2023-07-29 13:40:17.897451 sedi-0.7/PKG-INFO
--rw-rw-r--   0 aleksa    (1000) aleksa    (1000)     6383 2023-07-29 13:12:19.000000 sedi-0.7/provision.py
--rw-r--r--   0 aleksa    (1000) aleksa    (1000)     2493 2023-07-29 11:36:14.000000 sedi-0.7/sed.py
-drwxrwxr-x   0 aleksa    (1000) aleksa    (1000)        0 2023-07-29 13:40:17.897451 sedi-0.7/sedi.egg-info/
--rw-rw-r--   0 aleksa    (1000) aleksa    (1000)      127 2023-07-29 13:40:17.000000 sedi-0.7/sedi.egg-info/PKG-INFO
--rw-rw-r--   0 aleksa    (1000) aleksa    (1000)      171 2023-07-29 13:40:17.000000 sedi-0.7/sedi.egg-info/SOURCES.txt
--rw-rw-r--   0 aleksa    (1000) aleksa    (1000)        1 2023-07-29 13:40:17.000000 sedi-0.7/sedi.egg-info/dependency_links.txt
--rw-rw-r--   0 aleksa    (1000) aleksa    (1000)       59 2023-07-29 13:40:17.000000 sedi-0.7/sedi.egg-info/entry_points.txt
--rw-rw-r--   0 aleksa    (1000) aleksa    (1000)       14 2023-07-29 13:40:17.000000 sedi-0.7/sedi.egg-info/top_level.txt
--rw-rw-r--   0 aleksa    (1000) aleksa    (1000)       38 2023-07-29 13:40:17.897451 sedi-0.7/setup.cfg
--rw-rw-r--   0 aleksa    (1000) aleksa    (1000)      348 2023-07-29 13:40:16.000000 sedi-0.7/setup.py
+drwxrwxr-x   0 aleksa    (1000) aleksa    (1000)        0 2023-07-29 13:44:22.248590 sedi-0.8/
+-rw-rw-r--   0 aleksa    (1000) aleksa    (1000)      127 2023-07-29 13:44:22.248590 sedi-0.8/PKG-INFO
+-rw-rw-r--   0 aleksa    (1000) aleksa    (1000)     6405 2023-07-29 13:42:43.000000 sedi-0.8/provision.py
+-rw-r--r--   0 aleksa    (1000) aleksa    (1000)     2493 2023-07-29 11:36:14.000000 sedi-0.8/sed.py
+drwxrwxr-x   0 aleksa    (1000) aleksa    (1000)        0 2023-07-29 13:44:22.248590 sedi-0.8/sedi.egg-info/
+-rw-rw-r--   0 aleksa    (1000) aleksa    (1000)      127 2023-07-29 13:44:22.000000 sedi-0.8/sedi.egg-info/PKG-INFO
+-rw-rw-r--   0 aleksa    (1000) aleksa    (1000)      171 2023-07-29 13:44:22.000000 sedi-0.8/sedi.egg-info/SOURCES.txt
+-rw-rw-r--   0 aleksa    (1000) aleksa    (1000)        1 2023-07-29 13:44:22.000000 sedi-0.8/sedi.egg-info/dependency_links.txt
+-rw-rw-r--   0 aleksa    (1000) aleksa    (1000)       59 2023-07-29 13:44:22.000000 sedi-0.8/sedi.egg-info/entry_points.txt
+-rw-rw-r--   0 aleksa    (1000) aleksa    (1000)       14 2023-07-29 13:44:22.000000 sedi-0.8/sedi.egg-info/top_level.txt
+-rw-rw-r--   0 aleksa    (1000) aleksa    (1000)       38 2023-07-29 13:44:22.248590 sedi-0.8/setup.cfg
+-rw-rw-r--   0 aleksa    (1000) aleksa    (1000)     3725 2023-07-29 13:44:08.000000 sedi-0.8/setup.py
```

### Comparing `sedi-0.7/provision.py` & `sedi-0.8/provision.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 	# Publish dummy message to a test topic in order to see if everything works:
 	pubCmd = "mosquitto_pub -d --cafile ./certs/AmazonRootCA1.pem  --cert ./certs/deviceName.crt --key ./certs/deviceName.key -h " + endpoint
 	pubCmd += " -p 8883 -q 0 -t deviceName -i deviceName --tls-version tlsv1.2 -m \"hello from python\""
 	pubCmd = pubCmd.replace("deviceName", imei)
 	proc = subprocess.run([pubCmd], shell=True, check=True, capture_output=True)
 	print(proc.stdout)
 
-def main(imei):
+def main(imei = "defaultDeviceName"):
 	try:
 		generateRootCertificate()
 		registerRootCertificate()
 		generateDeviceCertificate(imei)
 		provisionDevice(imei)
 		publish(imei)  # test publish, not needed
 	except Exception as ex:
```

### Comparing `sedi-0.7/sed.py` & `sedi-0.8/sed.py`

 * *Files identical despite different names*

