# Comparing `tmp/constellation-1.1.0.tar.gz` & `tmp/constellation-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "constellation-1.1.0.tar", last modified: Thu Jul 27 10:30:54 2023, max compression
+gzip compressed data, was "constellation-1.1.1.tar", last modified: Mon Jul 31 12:57:03 2023, max compression
```

## Comparing `constellation-1.1.0.tar` & `constellation-1.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 aehill    (1000) aehill    (1000)        0 2023-07-27 10:30:54.495949 constellation-1.1.0/
--rw-rw-r--   0 aehill    (1000) aehill    (1000)     1096 2023-05-23 18:31:17.000000 constellation-1.1.0/LICENSE
--rw-rw-r--   0 aehill    (1000) aehill    (1000)      960 2023-07-27 10:30:54.495949 constellation-1.1.0/PKG-INFO
--rw-rw-r--   0 aehill    (1000) aehill    (1000)      481 2023-05-23 18:31:17.000000 constellation-1.1.0/README.md
-drwxrwxr-x   0 aehill    (1000) aehill    (1000)        0 2023-07-27 10:30:54.495949 constellation-1.1.0/constellation/
--rw-rw-r--   0 aehill    (1000) aehill    (1000)      337 2023-05-23 18:31:17.000000 constellation-1.1.0/constellation/__init__.py
--rw-rw-r--   0 aehill    (1000) aehill    (1000)     4910 2023-07-27 08:12:12.000000 constellation-1.1.0/constellation/config.py
--rw-rw-r--   0 aehill    (1000) aehill    (1000)    10451 2023-07-27 08:09:53.000000 constellation-1.1.0/constellation/constellation.py
--rw-rw-r--   0 aehill    (1000) aehill    (1000)     6866 2023-05-23 18:31:17.000000 constellation-1.1.0/constellation/docker_util.py
--rw-rw-r--   0 aehill    (1000) aehill    (1000)     1460 2023-05-23 18:31:17.000000 constellation-1.1.0/constellation/notifier.py
--rw-rw-r--   0 aehill    (1000) aehill    (1000)      536 2023-05-23 18:31:17.000000 constellation-1.1.0/constellation/util.py
--rw-rw-r--   0 aehill    (1000) aehill    (1000)     2737 2023-05-23 18:31:17.000000 constellation-1.1.0/constellation/vault.py
-drwxrwxr-x   0 aehill    (1000) aehill    (1000)        0 2023-07-27 10:30:54.495949 constellation-1.1.0/constellation.egg-info/
--rw-rw-r--   0 aehill    (1000) aehill    (1000)      960 2023-07-27 10:30:54.000000 constellation-1.1.0/constellation.egg-info/PKG-INFO
--rw-rw-r--   0 aehill    (1000) aehill    (1000)      566 2023-07-27 10:30:54.000000 constellation-1.1.0/constellation.egg-info/SOURCES.txt
--rw-rw-r--   0 aehill    (1000) aehill    (1000)        1 2023-07-27 10:30:54.000000 constellation-1.1.0/constellation.egg-info/dependency_links.txt
--rw-rw-r--   0 aehill    (1000) aehill    (1000)        1 2023-07-27 10:30:54.000000 constellation-1.1.0/constellation.egg-info/not-zip-safe
--rw-rw-r--   0 aehill    (1000) aehill    (1000)       36 2023-07-27 10:30:54.000000 constellation-1.1.0/constellation.egg-info/requires.txt
--rw-rw-r--   0 aehill    (1000) aehill    (1000)       14 2023-07-27 10:30:54.000000 constellation-1.1.0/constellation.egg-info/top_level.txt
--rw-rw-r--   0 aehill    (1000) aehill    (1000)       63 2023-07-27 10:30:54.495949 constellation-1.1.0/setup.cfg
--rw-rw-r--   0 aehill    (1000) aehill    (1000)     1007 2023-07-27 10:25:34.000000 constellation-1.1.0/setup.py
-drwxrwxr-x   0 aehill    (1000) aehill    (1000)        0 2023-07-27 10:30:54.495949 constellation-1.1.0/test/
--rw-rw-r--   0 aehill    (1000) aehill    (1000)     7550 2023-07-27 08:12:46.000000 constellation-1.1.0/test/test_config.py
--rw-rw-r--   0 aehill    (1000) aehill    (1000)    14233 2023-07-27 08:09:53.000000 constellation-1.1.0/test/test_constellation.py
--rw-rw-r--   0 aehill    (1000) aehill    (1000)     7595 2023-05-23 18:31:17.000000 constellation-1.1.0/test/test_docker_util.py
--rw-rw-r--   0 aehill    (1000) aehill    (1000)     1805 2023-05-23 18:31:17.000000 constellation-1.1.0/test/test_notify.py
--rw-rw-r--   0 aehill    (1000) aehill    (1000)      398 2023-05-23 18:31:17.000000 constellation-1.1.0/test/test_util.py
--rw-rw-r--   0 aehill    (1000) aehill    (1000)     4892 2023-05-23 18:31:17.000000 constellation-1.1.0/test/test_vault.py
+drwxrwxr-x   0 aehill    (1000) aehill    (1000)        0 2023-07-31 12:57:03.882646 constellation-1.1.1/
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)     1096 2023-05-23 18:31:17.000000 constellation-1.1.1/LICENSE
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)      960 2023-07-31 12:57:03.882646 constellation-1.1.1/PKG-INFO
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)      481 2023-05-23 18:31:17.000000 constellation-1.1.1/README.md
+drwxrwxr-x   0 aehill    (1000) aehill    (1000)        0 2023-07-31 12:57:03.882646 constellation-1.1.1/constellation/
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)      337 2023-05-23 18:31:17.000000 constellation-1.1.1/constellation/__init__.py
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)     4910 2023-07-31 11:59:53.000000 constellation-1.1.1/constellation/config.py
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)    10451 2023-07-27 08:09:53.000000 constellation-1.1.1/constellation/constellation.py
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)     6866 2023-05-23 18:31:17.000000 constellation-1.1.1/constellation/docker_util.py
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)     1460 2023-05-23 18:31:17.000000 constellation-1.1.1/constellation/notifier.py
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)      536 2023-05-23 18:31:17.000000 constellation-1.1.1/constellation/util.py
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)     2811 2023-07-31 11:59:51.000000 constellation-1.1.1/constellation/vault.py
+drwxrwxr-x   0 aehill    (1000) aehill    (1000)        0 2023-07-31 12:57:03.882646 constellation-1.1.1/constellation.egg-info/
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)      960 2023-07-31 12:57:03.000000 constellation-1.1.1/constellation.egg-info/PKG-INFO
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)      566 2023-07-31 12:57:03.000000 constellation-1.1.1/constellation.egg-info/SOURCES.txt
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)        1 2023-07-31 12:57:03.000000 constellation-1.1.1/constellation.egg-info/dependency_links.txt
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)        1 2023-07-31 12:57:03.000000 constellation-1.1.1/constellation.egg-info/not-zip-safe
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)       36 2023-07-31 12:57:03.000000 constellation-1.1.1/constellation.egg-info/requires.txt
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)       14 2023-07-31 12:57:03.000000 constellation-1.1.1/constellation.egg-info/top_level.txt
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)       63 2023-07-31 12:57:03.882646 constellation-1.1.1/setup.cfg
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)     1007 2023-07-31 12:00:02.000000 constellation-1.1.1/setup.py
+drwxrwxr-x   0 aehill    (1000) aehill    (1000)        0 2023-07-31 12:57:03.882646 constellation-1.1.1/test/
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)     7550 2023-07-31 11:59:53.000000 constellation-1.1.1/test/test_config.py
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)    14233 2023-07-27 08:09:53.000000 constellation-1.1.1/test/test_constellation.py
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)     7595 2023-05-23 18:31:17.000000 constellation-1.1.1/test/test_docker_util.py
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)     1805 2023-05-23 18:31:17.000000 constellation-1.1.1/test/test_notify.py
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)      398 2023-05-23 18:31:17.000000 constellation-1.1.1/test/test_util.py
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)     5322 2023-07-31 11:59:51.000000 constellation-1.1.1/test/test_vault.py
```

### Comparing `constellation-1.1.0/LICENSE` & `constellation-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `constellation-1.1.0/PKG-INFO` & `constellation-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: constellation
-Version: 1.1.0
+Version: 1.1.1
 Summary: Deploy scripts for constellations of docker containers
 Home-page: https://github.com/reside-ic/constellation
 Author: Rich FitzJohn
 Author-email: r.fitzjohn@imperial.ac.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `constellation-1.1.0/constellation/config.py` & `constellation-1.1.1/constellation/config.py`

 * *Files identical despite different names*

### Comparing `constellation-1.1.0/constellation/constellation.py` & `constellation-1.1.1/constellation/constellation.py`

 * *Files identical despite different names*

### Comparing `constellation-1.1.0/constellation/docker_util.py` & `constellation-1.1.1/constellation/docker_util.py`

 * *Files identical despite different names*

### Comparing `constellation-1.1.0/constellation/notifier.py` & `constellation-1.1.1/constellation/notifier.py`

 * *Files identical despite different names*

### Comparing `constellation-1.1.0/constellation/util.py` & `constellation-1.1.1/constellation/util.py`

 * *Files identical despite different names*

### Comparing `constellation-1.1.0/constellation/vault.py` & `constellation-1.1.1/constellation/vault.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,16 @@
 
 def resolve_secrets_dict(d, client):
     for k, v, in d.items():
         if type(v) == str:
             updated, v = resolve_secret(v, client)
             if updated:
                 d[k] = v
+        elif type(v) == dict:
+            resolve_secrets_dict(v, client)
 
 
 class vault_config:
     def __init__(self, url, auth_method, auth_args):
         self.url = url
         self.auth_method = auth_method
         self.auth_args = auth_args
```

### Comparing `constellation-1.1.0/constellation.egg-info/PKG-INFO` & `constellation-1.1.1/constellation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: constellation
-Version: 1.1.0
+Version: 1.1.1
 Summary: Deploy scripts for constellations of docker containers
 Home-page: https://github.com/reside-ic/constellation
 Author: Rich FitzJohn
 Author-email: r.fitzjohn@imperial.ac.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `constellation-1.1.0/constellation.egg-info/SOURCES.txt` & `constellation-1.1.1/constellation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `constellation-1.1.0/setup.py` & `constellation-1.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "docker",
     "hvac",
     "pytest",
     "pyyaml",
     "vault_dev"]
 
 setup(name="constellation",
-      version="1.1.0",
+      version="1.1.1",
       description="Deploy scripts for constellations of docker containers",
       long_description=long_description,
       classifiers=[
           "Programming Language :: Python :: 3",
           "License :: OSI Approved :: MIT License",
           "Operating System :: OS Independent",
       ],
```

### Comparing `constellation-1.1.0/test/test_config.py` & `constellation-1.1.1/test/test_config.py`

 * *Files identical despite different names*

### Comparing `constellation-1.1.0/test/test_constellation.py` & `constellation-1.1.1/test/test_constellation.py`

 * *Files identical despite different names*

### Comparing `constellation-1.1.0/test/test_docker_util.py` & `constellation-1.1.1/test/test_docker_util.py`

 * *Files identical despite different names*

### Comparing `constellation-1.1.0/test/test_notify.py` & `constellation-1.1.1/test/test_notify.py`

 * *Files identical despite different names*

### Comparing `constellation-1.1.0/test/test_vault.py` & `constellation-1.1.1/test/test_vault.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 def test_secret_reading():
     with vault_dev.server() as s:
         client = s.client()
         client.write("secret/foo", value="s3cret")
         assert resolve_secret("foo", client) == (False, "foo")
         assert resolve_secret("VAULT:secret/foo:value", client) == \
-            (True, "s3cret")
+               (True, "s3cret")
 
 
 def test_secret_reading_of_dicts():
     with vault_dev.server() as s:
         client = s.client()
         client.write("secret/foo", value="s3cret")
         # With data
@@ -27,14 +27,28 @@
         assert dat == {"foo": "s3cret", "bar": "constant"}
         # Without
         empty = {}
         resolve_secrets(empty, client)
         assert empty == {}
 
 
+def test_secret_reading_of_dicts_recursive():
+    with vault_dev.server() as s:
+        client = s.client()
+        client.write("secret/foo", value="s3cret")
+        # With data
+        dat = {"foo": {"bar": "VAULT:secret/foo:value"}}
+        resolve_secrets(dat, client)
+        assert dat == {"foo": {"bar": "s3cret"}}
+        # Without
+        empty = {}
+        resolve_secrets(empty, client)
+        assert empty == {}
+
+
 def test_secret_reading_of_objects():
     with vault_dev.server() as s:
         client = s.client()
         client.write("secret/foo", value="s3cret")
 
         class Data:
             def __init__(self):
```

