# Comparing `tmp/nginx-set-conf-equitania-0.9.2.tar.gz` & `tmp/nginx-set-conf-equitania-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nginx-set-conf-equitania-0.9.2.tar", last modified: Mon Jul 10 15:42:09 2023, max compression
+gzip compressed data, was "nginx-set-conf-equitania-0.9.3.tar", last modified: Mon Jul 31 08:56:14 2023, max compression
```

## Comparing `nginx-set-conf-equitania-0.9.2.tar` & `nginx-set-conf-equitania-0.9.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-07-10 15:42:09.342374 nginx-set-conf-equitania-0.9.2/
--rw-r--r--   0 picard     (501) staff       (20)    33892 2021-05-25 14:23:55.000000 nginx-set-conf-equitania-0.9.2/LICENSE.txt
--rw-r--r--   0 picard     (501) staff       (20)     3340 2023-07-10 15:42:09.342250 nginx-set-conf-equitania-0.9.2/PKG-INFO
--rw-r--r--   0 picard     (501) staff       (20)     2861 2023-07-10 09:23:12.000000 nginx-set-conf-equitania-0.9.2/README.md
-drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-07-10 15:42:09.341224 nginx-set-conf-equitania-0.9.2/nginx_set_conf/
--rw-r--r--   0 picard     (501) staff       (20)       50 2021-05-27 17:15:29.000000 nginx-set-conf-equitania-0.9.2/nginx_set_conf/__init__.py
--rw-r--r--   0 picard     (501) staff       (20)    19765 2023-07-10 15:40:25.000000 nginx-set-conf-equitania-0.9.2/nginx_set_conf/config_templates.py
--rw-r--r--   0 picard     (501) staff       (20)     3953 2023-07-10 15:39:14.000000 nginx-set-conf-equitania-0.9.2/nginx_set_conf/nginx_set_conf.py
--rw-r--r--   0 picard     (501) staff       (20)     7078 2023-05-02 13:16:56.000000 nginx-set-conf-equitania-0.9.2/nginx_set_conf/utils.py
-drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-07-10 15:42:09.342069 nginx-set-conf-equitania-0.9.2/nginx_set_conf_equitania.egg-info/
--rw-r--r--   0 picard     (501) staff       (20)     3340 2023-07-10 15:42:09.000000 nginx-set-conf-equitania-0.9.2/nginx_set_conf_equitania.egg-info/PKG-INFO
--rw-r--r--   0 picard     (501) staff       (20)      439 2023-07-10 15:42:09.000000 nginx-set-conf-equitania-0.9.2/nginx_set_conf_equitania.egg-info/SOURCES.txt
--rw-r--r--   0 picard     (501) staff       (20)        1 2023-07-10 15:42:09.000000 nginx-set-conf-equitania-0.9.2/nginx_set_conf_equitania.egg-info/dependency_links.txt
--rw-r--r--   0 picard     (501) staff       (20)       86 2023-07-10 15:42:09.000000 nginx-set-conf-equitania-0.9.2/nginx_set_conf_equitania.egg-info/entry_points.txt
--rw-r--r--   0 picard     (501) staff       (20)       27 2023-07-10 15:42:09.000000 nginx-set-conf-equitania-0.9.2/nginx_set_conf_equitania.egg-info/requires.txt
--rw-r--r--   0 picard     (501) staff       (20)       15 2023-07-10 15:42:09.000000 nginx-set-conf-equitania-0.9.2/nginx_set_conf_equitania.egg-info/top_level.txt
--rw-r--r--   0 picard     (501) staff       (20)       38 2023-07-10 15:42:09.342410 nginx-set-conf-equitania-0.9.2/setup.cfg
--rw-r--r--   0 picard     (501) staff       (20)      880 2023-07-10 15:41:11.000000 nginx-set-conf-equitania-0.9.2/setup.py
+drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-07-31 08:56:14.861703 nginx-set-conf-equitania-0.9.3/
+-rw-r--r--   0 picard     (501) staff       (20)    33892 2021-05-25 14:23:55.000000 nginx-set-conf-equitania-0.9.3/LICENSE.txt
+-rw-r--r--   0 picard     (501) staff       (20)     3340 2023-07-31 08:56:14.861392 nginx-set-conf-equitania-0.9.3/PKG-INFO
+-rw-r--r--   0 picard     (501) staff       (20)     2861 2023-07-10 09:23:12.000000 nginx-set-conf-equitania-0.9.3/README.md
+drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-07-31 08:56:14.854026 nginx-set-conf-equitania-0.9.3/nginx_set_conf/
+-rw-r--r--   0 picard     (501) staff       (20)       50 2021-05-27 17:15:29.000000 nginx-set-conf-equitania-0.9.3/nginx_set_conf/__init__.py
+-rw-r--r--   0 picard     (501) staff       (20)    19747 2023-07-31 08:10:16.000000 nginx-set-conf-equitania-0.9.3/nginx_set_conf/config_templates.py
+-rw-r--r--   0 picard     (501) staff       (20)     3953 2023-07-10 15:39:14.000000 nginx-set-conf-equitania-0.9.3/nginx_set_conf/nginx_set_conf.py
+-rw-r--r--   0 picard     (501) staff       (20)     7078 2023-05-02 13:16:56.000000 nginx-set-conf-equitania-0.9.3/nginx_set_conf/utils.py
+drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-07-31 08:56:14.860892 nginx-set-conf-equitania-0.9.3/nginx_set_conf_equitania.egg-info/
+-rw-r--r--   0 picard     (501) staff       (20)     3340 2023-07-31 08:56:14.000000 nginx-set-conf-equitania-0.9.3/nginx_set_conf_equitania.egg-info/PKG-INFO
+-rw-r--r--   0 picard     (501) staff       (20)      439 2023-07-31 08:56:14.000000 nginx-set-conf-equitania-0.9.3/nginx_set_conf_equitania.egg-info/SOURCES.txt
+-rw-r--r--   0 picard     (501) staff       (20)        1 2023-07-31 08:56:14.000000 nginx-set-conf-equitania-0.9.3/nginx_set_conf_equitania.egg-info/dependency_links.txt
+-rw-r--r--   0 picard     (501) staff       (20)       86 2023-07-31 08:56:14.000000 nginx-set-conf-equitania-0.9.3/nginx_set_conf_equitania.egg-info/entry_points.txt
+-rw-r--r--   0 picard     (501) staff       (20)       27 2023-07-31 08:56:14.000000 nginx-set-conf-equitania-0.9.3/nginx_set_conf_equitania.egg-info/requires.txt
+-rw-r--r--   0 picard     (501) staff       (20)       15 2023-07-31 08:56:14.000000 nginx-set-conf-equitania-0.9.3/nginx_set_conf_equitania.egg-info/top_level.txt
+-rw-r--r--   0 picard     (501) staff       (20)       38 2023-07-31 08:56:14.861782 nginx-set-conf-equitania-0.9.3/setup.cfg
+-rw-r--r--   0 picard     (501) staff       (20)      880 2023-07-31 08:55:32.000000 nginx-set-conf-equitania-0.9.3/setup.py
```

### Comparing `nginx-set-conf-equitania-0.9.2/LICENSE.txt` & `nginx-set-conf-equitania-0.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nginx-set-conf-equitania-0.9.2/PKG-INFO` & `nginx-set-conf-equitania-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nginx-set-conf-equitania
-Version: 0.9.2
+Version: 0.9.3
 Summary: A package to create configurations for nginx for different web applications
 Author: Equitania Software GmbH
 Author-email: info@equitania.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `nginx-set-conf-equitania-0.9.2/README.md` & `nginx-set-conf-equitania-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `nginx-set-conf-equitania-0.9.2/nginx_set_conf/config_templates.py` & `nginx-set-conf-equitania-0.9.3/nginx_set_conf/config_templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 server {
     listen server.domain.de:443 ssl http2;
     server_name server.domain.de;
 
     add_header Strict-Transport-Security "max-age=15552000; includeSubDomains" always;
 
     access_log /var/log/nginx/server.domain.de-access.log combined buffer=512k flush=1m;
-    error_log /var/log/nginx/server.domain.de-error.log warn flush=2m;
+    error_log /var/log/nginx/server.domain.de-error.log warn;
 
     # ssl certificate files
     ssl_certificate /etc/letsencrypt/live/zertifikat.crt/fullchain.pem;
     ssl_certificate_key /etc/letsencrypt/live/zertifikat.key/privkey.pem;
 
     # add ssl specific settings
     keepalive_timeout    60;
@@ -84,15 +84,15 @@
 server {
     listen server.domain.de:443 ssl http2;
     server_name server.domain.de;
 
     add_header Strict-Transport-Security "max-age=15552000; includeSubDomains" always;
 
     access_log /var/log/nginx/server.domain.de-access.log combined buffer=512k flush=1m;
-    error_log /var/log/nginx/server.domain.de-error.log warn flush=2m;
+    error_log /var/log/nginx/server.domain.de-error.log warn;
 
     # ssl certificate files
     ssl_certificate /etc/letsencrypt/live/zertifikat.crt/fullchain.pem;
     ssl_certificate_key /etc/letsencrypt/live/zertifikat.key/privkey.pem;
 
     # add ssl specific settings
     keepalive_timeout    60;
```

### Comparing `nginx-set-conf-equitania-0.9.2/nginx_set_conf/nginx_set_conf.py` & `nginx-set-conf-equitania-0.9.3/nginx_set_conf/nginx_set_conf.py`

 * *Files identical despite different names*

### Comparing `nginx-set-conf-equitania-0.9.2/nginx_set_conf/utils.py` & `nginx-set-conf-equitania-0.9.3/nginx_set_conf/utils.py`

 * *Files identical despite different names*

### Comparing `nginx-set-conf-equitania-0.9.2/nginx_set_conf_equitania.egg-info/PKG-INFO` & `nginx-set-conf-equitania-0.9.3/nginx_set_conf_equitania.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nginx-set-conf-equitania
-Version: 0.9.2
+Version: 0.9.3
 Summary: A package to create configurations for nginx for different web applications
 Author: Equitania Software GmbH
 Author-email: info@equitania.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `nginx-set-conf-equitania-0.9.2/setup.py` & `nginx-set-conf-equitania-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nginx-set-conf-equitania",
-    version="0.9.2",
+    version="0.9.3",
     author="Equitania Software GmbH",
     author_email="info@equitania.de",
     description="A package to create configurations for nginx for different web applications",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=['nginx_set_conf'],
     classifiers=[
```

