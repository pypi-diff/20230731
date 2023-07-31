# Comparing `tmp/config_server_client-0.0.5.tar.gz` & `tmp/config_server_client-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/config_server_client-0.0.5.tar", last modified: Mon Jul 31 12:38:27 2023, max compression
+gzip compressed data, was "dist/config_server_client-0.0.6.tar", last modified: Mon Jul 31 13:13:36 2023, max compression
```

## Comparing `config_server_client-0.0.5.tar` & `config_server_client-0.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 jayant     (501) staff       (20)        0 2023-07-31 12:38:27.000000 config_server_client-0.0.5/
--rw-r--r--   0 jayant     (501) staff       (20)      213 2023-07-31 12:38:27.000000 config_server_client-0.0.5/PKG-INFO
-drwxr-xr-x   0 jayant     (501) staff       (20)        0 2023-07-31 12:38:27.000000 config_server_client-0.0.5/config_server_client.egg-info/
--rw-r--r--   0 jayant     (501) staff       (20)      213 2023-07-31 12:38:27.000000 config_server_client-0.0.5/config_server_client.egg-info/PKG-INFO
--rw-r--r--   0 jayant     (501) staff       (20)      184 2023-07-31 12:38:27.000000 config_server_client-0.0.5/config_server_client.egg-info/SOURCES.txt
--rw-r--r--   0 jayant     (501) staff       (20)        1 2023-07-31 12:38:27.000000 config_server_client-0.0.5/config_server_client.egg-info/top_level.txt
--rw-r--r--   0 jayant     (501) staff       (20)        1 2023-07-31 12:38:27.000000 config_server_client-0.0.5/config_server_client.egg-info/dependency_links.txt
--rw-r--r--   0 jayant     (501) staff       (20)      253 2023-07-31 12:37:21.000000 config_server_client-0.0.5/setup.py
--rw-r--r--   0 jayant     (501) staff       (20)       38 2023-07-31 12:38:27.000000 config_server_client-0.0.5/setup.cfg
+drwxr-xr-x   0 jayant     (501) staff       (20)        0 2023-07-31 13:13:36.000000 config_server_client-0.0.6/
+-rw-r--r--   0 jayant     (501) staff       (20)      213 2023-07-31 13:13:36.000000 config_server_client-0.0.6/PKG-INFO
+drwxr-xr-x   0 jayant     (501) staff       (20)        0 2023-07-31 13:13:36.000000 config_server_client-0.0.6/config_server_client.egg-info/
+-rw-r--r--   0 jayant     (501) staff       (20)      213 2023-07-31 13:13:36.000000 config_server_client-0.0.6/config_server_client.egg-info/PKG-INFO
+-rw-r--r--   0 jayant     (501) staff       (20)      184 2023-07-31 13:13:36.000000 config_server_client-0.0.6/config_server_client.egg-info/SOURCES.txt
+-rw-r--r--   0 jayant     (501) staff       (20)        1 2023-07-31 13:13:36.000000 config_server_client-0.0.6/config_server_client.egg-info/top_level.txt
+-rw-r--r--   0 jayant     (501) staff       (20)        1 2023-07-31 13:13:36.000000 config_server_client-0.0.6/config_server_client.egg-info/dependency_links.txt
+-rw-r--r--   0 jayant     (501) staff       (20)      253 2023-07-31 13:13:25.000000 config_server_client-0.0.6/setup.py
+-rw-r--r--   0 jayant     (501) staff       (20)       38 2023-07-31 13:13:36.000000 config_server_client-0.0.6/setup.cfg
```

