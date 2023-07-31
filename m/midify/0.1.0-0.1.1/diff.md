# Comparing `tmp/Midify-0.1.0.tar.gz` & `tmp/midify-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Midify-0.1.0.tar", last modified: Mon Jul 31 05:07:28 2023, max compression
+gzip compressed data, was "midify-0.1.1.tar", last modified: Mon Jul 31 05:12:15 2023, max compression
```

## Comparing `Midify-0.1.0.tar` & `midify-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
-drwxrwxr-x   0 danielsan  (1000) danielsan  (1000)        0 2023-07-31 05:07:28.531724 Midify-0.1.0/
--rw-rw-r--   0 danielsan  (1000) danielsan  (1000)      321 2023-07-31 05:07:28.531724 Midify-0.1.0/PKG-INFO
-drwxrwxr-x   0 danielsan  (1000) danielsan  (1000)        0 2023-07-31 05:07:28.531724 Midify-0.1.0/midify/
--rwxrwxr-x   0 danielsan  (1000) danielsan  (1000)       71 2023-07-31 05:04:35.739031 Midify-0.1.0/midify/midify
--rw-rw-r--   0 danielsan  (1000) danielsan  (1000)      414 2023-07-31 05:07:17.163668 Midify-0.1.0/setup.py
+drwxrwxr-x   0 danielsan  (1000) danielsan  (1000)        0 2023-07-31 05:12:15.757517 midify-0.1.1/
+-rw-rw-r--   0 danielsan  (1000) danielsan  (1000)      321 2023-07-31 05:12:15.757517 midify-0.1.1/PKG-INFO
+drwxrwxr-x   0 danielsan  (1000) danielsan  (1000)        0 2023-07-31 05:12:15.757517 midify-0.1.1/midify/
+-rwxrwxr-x   0 danielsan  (1000) danielsan  (1000)       71 2023-07-31 05:04:35.739031 midify-0.1.1/midify/midify
+-rw-rw-r--   0 danielsan  (1000) danielsan  (1000)      414 2023-07-31 05:12:11.605487 midify-0.1.1/setup.py
```

