# Comparing `tmp/nginx-set-conf-equitania-0.9.3.tar.gz` & `tmp/nginx-set-conf-equitania-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nginx-set-conf-equitania-0.9.3.tar", last modified: Mon Jul 31 08:56:14 2023, max compression
+gzip compressed data, was "nginx-set-conf-equitania-0.9.4.tar", last modified: Mon Jul 31 13:08:25 2023, max compression
```

## Comparing `nginx-set-conf-equitania-0.9.3.tar` & `nginx-set-conf-equitania-0.9.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-07-31 08:56:14.861703 nginx-set-conf-equitania-0.9.3/
--rw-r--r--   0 picard     (501) staff       (20)    33892 2021-05-25 14:23:55.000000 nginx-set-conf-equitania-0.9.3/LICENSE.txt
--rw-r--r--   0 picard     (501) staff       (20)     3340 2023-07-31 08:56:14.861392 nginx-set-conf-equitania-0.9.3/PKG-INFO
--rw-r--r--   0 picard     (501) staff       (20)     2861 2023-07-10 09:23:12.000000 nginx-set-conf-equitania-0.9.3/README.md
-drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-07-31 08:56:14.854026 nginx-set-conf-equitania-0.9.3/nginx_set_conf/
--rw-r--r--   0 picard     (501) staff       (20)       50 2021-05-27 17:15:29.000000 nginx-set-conf-equitania-0.9.3/nginx_set_conf/__init__.py
--rw-r--r--   0 picard     (501) staff       (20)    19747 2023-07-31 08:10:16.000000 nginx-set-conf-equitania-0.9.3/nginx_set_conf/config_templates.py
--rw-r--r--   0 picard     (501) staff       (20)     3953 2023-07-10 15:39:14.000000 nginx-set-conf-equitania-0.9.3/nginx_set_conf/nginx_set_conf.py
--rw-r--r--   0 picard     (501) staff       (20)     7078 2023-05-02 13:16:56.000000 nginx-set-conf-equitania-0.9.3/nginx_set_conf/utils.py
-drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-07-31 08:56:14.860892 nginx-set-conf-equitania-0.9.3/nginx_set_conf_equitania.egg-info/
--rw-r--r--   0 picard     (501) staff       (20)     3340 2023-07-31 08:56:14.000000 nginx-set-conf-equitania-0.9.3/nginx_set_conf_equitania.egg-info/PKG-INFO
--rw-r--r--   0 picard     (501) staff       (20)      439 2023-07-31 08:56:14.000000 nginx-set-conf-equitania-0.9.3/nginx_set_conf_equitania.egg-info/SOURCES.txt
--rw-r--r--   0 picard     (501) staff       (20)        1 2023-07-31 08:56:14.000000 nginx-set-conf-equitania-0.9.3/nginx_set_conf_equitania.egg-info/dependency_links.txt
--rw-r--r--   0 picard     (501) staff       (20)       86 2023-07-31 08:56:14.000000 nginx-set-conf-equitania-0.9.3/nginx_set_conf_equitania.egg-info/entry_points.txt
--rw-r--r--   0 picard     (501) staff       (20)       27 2023-07-31 08:56:14.000000 nginx-set-conf-equitania-0.9.3/nginx_set_conf_equitania.egg-info/requires.txt
--rw-r--r--   0 picard     (501) staff       (20)       15 2023-07-31 08:56:14.000000 nginx-set-conf-equitania-0.9.3/nginx_set_conf_equitania.egg-info/top_level.txt
--rw-r--r--   0 picard     (501) staff       (20)       38 2023-07-31 08:56:14.861782 nginx-set-conf-equitania-0.9.3/setup.cfg
--rw-r--r--   0 picard     (501) staff       (20)      880 2023-07-31 08:55:32.000000 nginx-set-conf-equitania-0.9.3/setup.py
+drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-07-31 13:08:25.944729 nginx-set-conf-equitania-0.9.4/
+-rw-r--r--   0 picard     (501) staff       (20)    33892 2021-05-25 14:23:55.000000 nginx-set-conf-equitania-0.9.4/LICENSE.txt
+-rw-r--r--   0 picard     (501) staff       (20)     3340 2023-07-31 13:08:25.944549 nginx-set-conf-equitania-0.9.4/PKG-INFO
+-rw-r--r--   0 picard     (501) staff       (20)     2861 2023-07-10 09:23:12.000000 nginx-set-conf-equitania-0.9.4/README.md
+drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-07-31 13:08:25.940920 nginx-set-conf-equitania-0.9.4/nginx_set_conf/
+-rw-r--r--   0 picard     (501) staff       (20)       50 2021-05-27 17:15:29.000000 nginx-set-conf-equitania-0.9.4/nginx_set_conf/__init__.py
+-rw-r--r--   0 picard     (501) staff       (20)    20839 2023-07-31 13:06:20.000000 nginx-set-conf-equitania-0.9.4/nginx_set_conf/config_templates.py
+-rw-r--r--   0 picard     (501) staff       (20)     3953 2023-07-10 15:39:14.000000 nginx-set-conf-equitania-0.9.4/nginx_set_conf/nginx_set_conf.py
+-rw-r--r--   0 picard     (501) staff       (20)     7078 2023-05-02 13:16:56.000000 nginx-set-conf-equitania-0.9.4/nginx_set_conf/utils.py
+drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-07-31 13:08:25.944179 nginx-set-conf-equitania-0.9.4/nginx_set_conf_equitania.egg-info/
+-rw-r--r--   0 picard     (501) staff       (20)     3340 2023-07-31 13:08:25.000000 nginx-set-conf-equitania-0.9.4/nginx_set_conf_equitania.egg-info/PKG-INFO
+-rw-r--r--   0 picard     (501) staff       (20)      439 2023-07-31 13:08:25.000000 nginx-set-conf-equitania-0.9.4/nginx_set_conf_equitania.egg-info/SOURCES.txt
+-rw-r--r--   0 picard     (501) staff       (20)        1 2023-07-31 13:08:25.000000 nginx-set-conf-equitania-0.9.4/nginx_set_conf_equitania.egg-info/dependency_links.txt
+-rw-r--r--   0 picard     (501) staff       (20)       86 2023-07-31 13:08:25.000000 nginx-set-conf-equitania-0.9.4/nginx_set_conf_equitania.egg-info/entry_points.txt
+-rw-r--r--   0 picard     (501) staff       (20)       27 2023-07-31 13:08:25.000000 nginx-set-conf-equitania-0.9.4/nginx_set_conf_equitania.egg-info/requires.txt
+-rw-r--r--   0 picard     (501) staff       (20)       15 2023-07-31 13:08:25.000000 nginx-set-conf-equitania-0.9.4/nginx_set_conf_equitania.egg-info/top_level.txt
+-rw-r--r--   0 picard     (501) staff       (20)       38 2023-07-31 13:08:25.944783 nginx-set-conf-equitania-0.9.4/setup.cfg
+-rw-r--r--   0 picard     (501) staff       (20)      880 2023-07-31 13:08:19.000000 nginx-set-conf-equitania-0.9.4/setup.py
```

### Comparing `nginx-set-conf-equitania-0.9.3/LICENSE.txt` & `nginx-set-conf-equitania-0.9.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nginx-set-conf-equitania-0.9.3/PKG-INFO` & `nginx-set-conf-equitania-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nginx-set-conf-equitania
-Version: 0.9.3
+Version: 0.9.4
 Summary: A package to create configurations for nginx for different web applications
 Author: Equitania Software GmbH
 Author-email: info@equitania.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `nginx-set-conf-equitania-0.9.3/README.md` & `nginx-set-conf-equitania-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `nginx-set-conf-equitania-0.9.3/nginx_set_conf/config_templates.py` & `nginx-set-conf-equitania-0.9.4/nginx_set_conf/config_templates.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,14 +38,21 @@
     include                 nginxconfig.io/general.conf;
 
     location = /robots.txt {
         add_header Content-Type text/plain;
         return 200 "User-agent: *Disallow: /";
     }
 
+    # error pages
+    error_page 500 502 503 504 /custom_50x.html;
+        location = /custom_50x.html {
+        root /etc/nginx/html/;
+        internal;
+    }
+
     #general proxy settings
     # force timeouts if the backend dies
     proxy_connect_timeout 1200s;
     proxy_send_timeout 1200s;
     proxy_read_timeout 1200s;
     proxy_next_upstream error timeout invalid_header http_500 http_502 http_503;
 
@@ -114,14 +121,21 @@
     include                 nginxconfig.io/general.conf;
 
     location = /robots.txt {
         add_header Content-Type text/plain;
         return 200 "User-agent: *Disallow: /";
     }
 
+    # error pages
+    error_page 500 502 503 504 /custom_50x.html;
+        location = /custom_50x.html {
+        root /etc/nginx/html/;
+        internal;
+    }
+
     #general proxy settings
     # force timeouts if the backend dies
     proxy_connect_timeout 1200s;
     proxy_send_timeout 1200s;
     proxy_read_timeout 1200s;
     proxy_next_upstream error timeout invalid_header http_500 http_502 http_503;
 
@@ -179,19 +193,26 @@
 
     # security
     include                 nginxconfig.io/security.conf;
 
     # additional config
     include                 nginxconfig.io/general.conf;
 
-        location = /robots.txt {
+    location = /robots.txt {
         add_header Content-Type text/plain;
         return 200 "User-agent: *Disallow: /";
     }
 
+    # error pages
+    error_page 500 502 503 504 /custom_50x.html;
+        location = /custom_50x.html {
+        root /etc/nginx/html/;
+        internal;
+    }
+
     # Raise file upload size
     client_max_body_size 10G;
     # Limit download size
     proxy_max_temp_file_size 4096m;
 
     #general proxy settings
     # force timeouts if the backend dies
@@ -256,15 +277,26 @@
 
     # security
     include                 nginxconfig.io/security.conf;
 
     # additional config
     include                 nginxconfig.io/general.conf;
 
-        #general proxy settings
+    # error pages
+    error_page 500 502 503 504 /custom_50x.html;
+        location = /custom_50x.html {
+        root /etc/nginx/html/;
+        internal;
+    }
+    location = /robots.txt {
+        add_header Content-Type text/plain;
+        return 200 "User-agent: *Disallow: /";
+    }
+
+    #general proxy settings
     # force timeouts if the backend dies
     proxy_connect_timeout 1200s;
     proxy_send_timeout 1200s;
     proxy_read_timeout 1200s;
     proxy_next_upstream error timeout invalid_header http_500 http_502 http_503;
 
     # Proxy for portainer docker
@@ -398,18 +430,18 @@
     # error pages
     error_page 500 502 503 504 /custom_50x.html;
     location = /custom_50x.html {
         root /etc/nginx/html/;
         internal;
     }
 
-    location = /robots.txt {
-        add_header Content-Type text/plain;
-        return 200 "User-agent: *Disallow: /";
-    }
+    #location = /robots.txt {
+    #    add_header Content-Type text/plain;
+    #    return 200 "User-agent: *Disallow: /";
+    #}
 
     # security
     include                 nginxconfig.io/security.conf;
 
     # additional config
     include                 nginxconfig.io/general.conf;
 
@@ -473,14 +505,21 @@
     ssl_session_timeout  5m;
 
     location = /robots.txt {
         add_header Content-Type text/plain;
         return 200 "User-agent: *Disallow: /";
     }
 
+    # error pages
+    error_page 500 502 503 504 /custom_50x.html;
+        location = /custom_50x.html {
+        root /etc/nginx/html/;
+        internal;
+    }
+
     # security
     include                 nginxconfig.io/security.conf;
 
     # additional config
     include                 nginxconfig.io/general.conf;
 
     #general proxy settings
@@ -544,15 +583,22 @@
     proxy_next_upstream error timeout invalid_header http_500 http_502 http_503;
 
     location = /robots.txt {
         add_header Content-Type text/plain;
         return 200 "User-agent: *Disallow: /";
     }
 
-    # security
+    # error pages
+    error_page 500 502 503 504 /custom_50x.html;
+        location = /custom_50x.html {
+        root /etc/nginx/html/;
+        internal;
+    }
+
+        # security
     include                 nginxconfig.io/security.conf;
 
     # additional config
     include                 nginxconfig.io/general.conf;
 
     # Add Headers for odoo proxy mode
     proxy_set_header X-Forwarded-Host $host;
```

### Comparing `nginx-set-conf-equitania-0.9.3/nginx_set_conf/nginx_set_conf.py` & `nginx-set-conf-equitania-0.9.4/nginx_set_conf/nginx_set_conf.py`

 * *Files identical despite different names*

### Comparing `nginx-set-conf-equitania-0.9.3/nginx_set_conf/utils.py` & `nginx-set-conf-equitania-0.9.4/nginx_set_conf/utils.py`

 * *Files identical despite different names*

### Comparing `nginx-set-conf-equitania-0.9.3/nginx_set_conf_equitania.egg-info/PKG-INFO` & `nginx-set-conf-equitania-0.9.4/nginx_set_conf_equitania.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nginx-set-conf-equitania
-Version: 0.9.3
+Version: 0.9.4
 Summary: A package to create configurations for nginx for different web applications
 Author: Equitania Software GmbH
 Author-email: info@equitania.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `nginx-set-conf-equitania-0.9.3/setup.py` & `nginx-set-conf-equitania-0.9.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nginx-set-conf-equitania",
-    version="0.9.3",
+    version="0.9.4",
     author="Equitania Software GmbH",
     author_email="info@equitania.de",
     description="A package to create configurations for nginx for different web applications",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=['nginx_set_conf'],
     classifiers=[
```

