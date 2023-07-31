# Comparing `tmp/midify-0.1.1.tar.gz` & `tmp/midify-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midify-0.1.1.tar", last modified: Mon Jul 31 05:12:15 2023, max compression
+gzip compressed data, was "midify-0.2.0.tar", last modified: Mon Jul 31 06:14:06 2023, max compression
```

## Comparing `midify-0.1.1.tar` & `midify-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,9 @@
-drwxrwxr-x   0 danielsan  (1000) danielsan  (1000)        0 2023-07-31 05:12:15.757517 midify-0.1.1/
--rw-rw-r--   0 danielsan  (1000) danielsan  (1000)      321 2023-07-31 05:12:15.757517 midify-0.1.1/PKG-INFO
-drwxrwxr-x   0 danielsan  (1000) danielsan  (1000)        0 2023-07-31 05:12:15.757517 midify-0.1.1/midify/
--rwxrwxr-x   0 danielsan  (1000) danielsan  (1000)       71 2023-07-31 05:04:35.739031 midify-0.1.1/midify/midify
--rw-rw-r--   0 danielsan  (1000) danielsan  (1000)      414 2023-07-31 05:12:11.605487 midify-0.1.1/setup.py
+drwxrwxr-x   0 danielsan  (1000) danielsan  (1000)        0 2023-07-31 06:14:06.030673 midify-0.2.0/
+-rw-rw-r--   0 danielsan  (1000) danielsan  (1000)      321 2023-07-31 06:14:06.030673 midify-0.2.0/PKG-INFO
+drwxrwxr-x   0 danielsan  (1000) danielsan  (1000)        0 2023-07-31 06:14:06.030673 midify-0.2.0/midify/
+-rw-rw-r--   0 danielsan  (1000) danielsan  (1000)      129 2023-07-31 06:09:04.831996 midify-0.2.0/midify/__init__.py
+-rw-rw-r--   0 danielsan  (1000) danielsan  (1000)      586 2023-07-31 05:48:39.789372 midify-0.2.0/midify/find_peaks.py
+-rwxrwxr-x   0 danielsan  (1000) danielsan  (1000)     2468 2023-07-31 06:08:54.479905 midify-0.2.0/midify/midify
+-rw-rw-r--   0 danielsan  (1000) danielsan  (1000)     1124 2023-07-31 05:55:36.224896 midify-0.2.0/midify/notes.py
+-rw-rw-r--   0 danielsan  (1000) danielsan  (1000)      132 2023-07-31 05:36:39.471361 midify-0.2.0/midify/resample.py
+-rw-rw-r--   0 danielsan  (1000) danielsan  (1000)      551 2023-07-31 06:13:54.010566 midify-0.2.0/setup.py
```

