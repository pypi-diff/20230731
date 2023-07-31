# Comparing `tmp/config_server_client-0.0.3.tar.gz` & `tmp/config_server_client-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/config_server_client-0.0.3.tar", last modified: Mon Jul 31 11:56:23 2023, max compression
+gzip compressed data, was "dist/config_server_client-0.0.4.tar", last modified: Mon Jul 31 12:33:14 2023, max compression
```

## Comparing `config_server_client-0.0.3.tar` & `config_server_client-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 jayant     (501) staff       (20)        0 2023-07-31 11:56:23.000000 config_server_client-0.0.3/
--rw-r--r--   0 jayant     (501) staff       (20)      224 2023-07-31 11:56:23.000000 config_server_client-0.0.3/PKG-INFO
-drwxr-xr-x   0 jayant     (501) staff       (20)        0 2023-07-31 11:56:23.000000 config_server_client-0.0.3/config_server_client.egg-info/
--rw-r--r--   0 jayant     (501) staff       (20)      224 2023-07-31 11:56:23.000000 config_server_client-0.0.3/config_server_client.egg-info/PKG-INFO
--rw-r--r--   0 jayant     (501) staff       (20)      184 2023-07-31 11:56:23.000000 config_server_client-0.0.3/config_server_client.egg-info/SOURCES.txt
--rw-r--r--   0 jayant     (501) staff       (20)        1 2023-07-31 11:56:23.000000 config_server_client-0.0.3/config_server_client.egg-info/dependency_links.txt
--rw-r--r--   0 jayant     (501) staff       (20)        1 2023-07-31 11:56:23.000000 config_server_client-0.0.3/config_server_client.egg-info/top_level.txt
--rw-r--r--   0 jayant     (501) staff       (20)       38 2023-07-31 11:56:23.000000 config_server_client-0.0.3/setup.cfg
--rw-r--r--   0 jayant     (501) staff       (20)      253 2023-07-31 11:56:18.000000 config_server_client-0.0.3/setup.py
+drwxr-xr-x   0 jayant     (501) staff       (20)        0 2023-07-31 12:33:14.000000 config_server_client-0.0.4/
+-rw-r--r--   0 jayant     (501) staff       (20)      213 2023-07-31 12:33:14.000000 config_server_client-0.0.4/PKG-INFO
+drwxr-xr-x   0 jayant     (501) staff       (20)        0 2023-07-31 12:33:14.000000 config_server_client-0.0.4/config_server_client.egg-info/
+-rw-r--r--   0 jayant     (501) staff       (20)      213 2023-07-31 12:33:14.000000 config_server_client-0.0.4/config_server_client.egg-info/PKG-INFO
+-rw-r--r--   0 jayant     (501) staff       (20)      184 2023-07-31 12:33:14.000000 config_server_client-0.0.4/config_server_client.egg-info/SOURCES.txt
+-rw-r--r--   0 jayant     (501) staff       (20)        1 2023-07-31 12:33:14.000000 config_server_client-0.0.4/config_server_client.egg-info/top_level.txt
+-rw-r--r--   0 jayant     (501) staff       (20)        1 2023-07-31 12:33:14.000000 config_server_client-0.0.4/config_server_client.egg-info/dependency_links.txt
+-rw-r--r--   0 jayant     (501) staff       (20)      253 2023-07-31 12:31:20.000000 config_server_client-0.0.4/setup.py
+-rw-r--r--   0 jayant     (501) staff       (20)       38 2023-07-31 12:33:14.000000 config_server_client-0.0.4/setup.cfg
```

