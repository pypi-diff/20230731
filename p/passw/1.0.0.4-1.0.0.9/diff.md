# Comparing `tmp/passw-1.0.0.4.tar.gz` & `tmp/passw-1.0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passw-1.0.0.4.tar", last modified: Fri Jul 28 10:04:30 2023, max compression
+gzip compressed data, was "passw-1.0.0.9.tar", last modified: Mon Jul 31 06:56:00 2023, max compression
```

## Comparing `passw-1.0.0.4.tar` & `passw-1.0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:04:30.858371 passw-1.0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-28 10:04:30.858371 passw-1.0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 10:04:18.000000 passw-1.0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:04:30.858371 passw-1.0.0.4/passw/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-28 10:04:18.000000 passw-1.0.0.4/passw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-28 10:04:18.000000 passw-1.0.0.4/passw/generate_pass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:04:30.858371 passw-1.0.0.4/passw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-28 10:04:30.000000 passw-1.0.0.4/passw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-28 10:04:30.000000 passw-1.0.0.4/passw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:04:30.000000 passw-1.0.0.4/passw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-28 10:04:30.000000 passw-1.0.0.4/passw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 10:04:30.858371 passw-1.0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-28 10:04:18.000000 passw-1.0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:56:00.918005 passw-1.0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-31 06:56:00.918005 passw-1.0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-31 06:55:52.000000 passw-1.0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:56:00.918005 passw-1.0.0.9/passw/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-31 06:55:52.000000 passw-1.0.0.9/passw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-31 06:55:52.000000 passw-1.0.0.9/passw/generate_pass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:56:00.918005 passw-1.0.0.9/passw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-31 06:56:00.000000 passw-1.0.0.9/passw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-31 06:56:00.000000 passw-1.0.0.9/passw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 06:56:00.000000 passw-1.0.0.9/passw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 06:56:00.000000 passw-1.0.0.9/passw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 06:56:00.918005 passw-1.0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-31 06:56:00.000000 passw-1.0.0.9/setup.py
```

### Comparing `passw-1.0.0.4/passw/generate_pass.py` & `passw-1.0.0.9/passw/generate_pass.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,11 +16,11 @@
             any(c.isdigit() for c in password)):
             break
 
     return password
 
 
 def gen_pass():
-    pass_len = random.randint(6,10)
+    pass_len = random.randint(6,11)
     passw = generate_random_password(pass_len)
     return passw
```

