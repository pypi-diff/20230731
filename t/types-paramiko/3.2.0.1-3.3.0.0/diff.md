# Comparing `tmp/types-paramiko-3.2.0.1.tar.gz` & `tmp/types-paramiko-3.3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-paramiko-3.2.0.1.tar", last modified: Thu Jul 20 15:20:44 2023, max compression
+gzip compressed data, was "types-paramiko-3.3.0.0.tar", last modified: Mon Jul 31 09:15:39 2023, max compression
```

## Comparing `types-paramiko-3.2.0.1.tar` & `types-paramiko-3.3.0.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:44.240465 types-paramiko-3.2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     6230 2023-07-20 15:20:43.000000 types-paramiko-3.2.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:20:43.000000 types-paramiko-3.2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-20 15:20:44.240465 types-paramiko-3.2.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:44.240465 types-paramiko-3.2.0.1/paramiko-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-20 15:20:43.000000 types-paramiko-3.2.0.1/paramiko-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/_version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/_winapi.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/agent.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/auth_handler.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/auth_strategy.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/ber.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/buffered_pipe.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/channel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/common.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/compress.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/dsskey.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/ecdsakey.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/ed25519key.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/file.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/hostkeys.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/kex_curve25519.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/kex_ecdh_nist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/kex_gex.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/kex_group1.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/kex_group14.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/kex_group16.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/kex_gss.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/message.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/packet.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/pipe.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/pkey.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/primes.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/proxy.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/rsakey.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/server.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/sftp.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/sftp_attr.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/sftp_client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/sftp_file.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/sftp_handle.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/sftp_server.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/sftp_si.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/ssh_exception.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/ssh_gss.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/transport.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/win_openssh.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-20 15:15:13.000000 types-paramiko-3.2.0.1/paramiko-stubs/win_pageant.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:20:44.240465 types-paramiko-3.2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-20 15:20:43.000000 types-paramiko-3.2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:44.240465 types-paramiko-3.2.0.1/types_paramiko.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-20 15:20:44.000000 types-paramiko-3.2.0.1/types_paramiko.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-20 15:20:44.000000 types-paramiko-3.2.0.1/types_paramiko.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:20:44.000000 types-paramiko-3.2.0.1/types_paramiko.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:20:44.000000 types-paramiko-3.2.0.1/types_paramiko.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 15:20:44.000000 types-paramiko-3.2.0.1/types_paramiko.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:15:39.772252 types-paramiko-3.3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-07-31 09:15:39.000000 types-paramiko-3.3.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-31 09:15:39.000000 types-paramiko-3.3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-31 09:15:39.772252 types-paramiko-3.3.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:15:39.772252 types-paramiko-3.3.0.0/paramiko-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-31 09:15:39.000000 types-paramiko-3.3.0.0/paramiko-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/_winapi.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/agent.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/auth_handler.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/auth_strategy.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/ber.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/buffered_pipe.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/channel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/common.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/compress.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/dsskey.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/ecdsakey.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/ed25519key.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/file.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/hostkeys.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/kex_curve25519.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/kex_ecdh_nist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/kex_gex.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/kex_group1.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/kex_group14.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/kex_group16.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/kex_gss.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/message.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/packet.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/pipe.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/pkey.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/primes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/proxy.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/rsakey.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/server.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/sftp.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/sftp_attr.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/sftp_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/sftp_file.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/sftp_handle.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/sftp_server.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/sftp_si.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/ssh_exception.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/ssh_gss.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/transport.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/win_openssh.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-31 09:15:19.000000 types-paramiko-3.3.0.0/paramiko-stubs/win_pageant.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 09:15:39.772252 types-paramiko-3.3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-31 09:15:39.000000 types-paramiko-3.3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:15:39.772252 types-paramiko-3.3.0.0/types_paramiko.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-31 09:15:39.000000 types-paramiko-3.3.0.0/types_paramiko.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-31 09:15:39.000000 types-paramiko-3.3.0.0/types_paramiko.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 09:15:39.000000 types-paramiko-3.3.0.0/types_paramiko.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-31 09:15:39.000000 types-paramiko-3.3.0.0/types_paramiko.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-31 09:15:39.000000 types-paramiko-3.3.0.0/types_paramiko.egg-info/top_level.txt
```

### Comparing `types-paramiko-3.2.0.1/CHANGELOG.md` & `types-paramiko-3.3.0.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 3.3.0.0 (2023-07-31)
+
+Bump paramiko to 3.3.* (#10522)
+
 ## 3.2.0.1 (2023-07-20)
 
 Add an upstream_repository field to METADATA.toml (#10487)
 
 Closes: #10478
 
 ## 3.2.0.0 (2023-06-01)
```

### Comparing `types-paramiko-3.2.0.1/PKG-INFO` & `types-paramiko-3.3.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-paramiko
-Version: 3.2.0.1
+Version: 3.3.0.0
 Summary: Typing stubs for paramiko
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/paramiko.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -26,10 +26,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
-with mypy 1.4.1, pyright 1.1.318, and
-pytype 2023.6.16.
+This package was generated from typeshed commit `fe2ebd69af14d376825f21182d415223bd037485` and was tested
+with mypy 1.4.1, pyright 1.1.319, and
+pytype 2023.7.21.
```

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/__init__.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/_winapi.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/_winapi.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/agent.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/agent.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/auth_handler.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/auth_handler.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/auth_strategy.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/auth_strategy.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/ber.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/ber.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/channel.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/channel.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/client.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/client.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/common.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/common.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/config.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/config.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/dsskey.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/dsskey.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/ecdsakey.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/ecdsakey.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/ed25519key.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/ed25519key.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/file.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/file.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/hostkeys.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/hostkeys.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/kex_curve25519.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/kex_curve25519.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/kex_ecdh_nist.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/kex_ecdh_nist.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/kex_gex.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/kex_gex.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/kex_group1.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/kex_group1.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/kex_gss.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/kex_gss.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/message.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/message.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/packet.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/packet.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/pipe.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/pipe.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/pkey.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/pkey.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/proxy.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/proxy.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/rsakey.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/rsakey.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/server.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/server.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/sftp.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/sftp.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/sftp_attr.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/sftp_attr.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/sftp_client.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/sftp_client.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -49,13 +49,25 @@
     def getcwd(self) -> str | None: ...
     def putfo(
         self, fl: IO[bytes], remotepath: bytes | str, file_size: int = 0, callback: _Callback | None = None, confirm: bool = True
     ) -> SFTPAttributes: ...
     def put(
         self, localpath: StrOrBytesPath, remotepath: bytes | str, callback: _Callback | None = None, confirm: bool = True
     ) -> SFTPAttributes: ...
-    def getfo(self, remotepath: bytes | str, fl: IO[bytes], callback: _Callback | None = None, prefetch: bool = True) -> int: ...
+    def getfo(
+        self,
+        remotepath: bytes | str,
+        fl: IO[bytes],
+        callback: _Callback | None = None,
+        prefetch: bool = True,
+        max_concurrent_prefetch_requests: int | None = None,
+    ) -> int: ...
     def get(
-        self, remotepath: bytes | str, localpath: StrOrBytesPath, callback: _Callback | None = None, prefetch: bool = True
+        self,
+        remotepath: bytes | str,
+        localpath: StrOrBytesPath,
+        callback: _Callback | None = None,
+        prefetch: bool = True,
+        max_concurrent_prefetch_requests: int | None = None,
     ) -> None: ...
 
 class SFTP(SFTPClient): ...
```

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/sftp_file.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/sftp_file.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -23,9 +23,11 @@
     def stat(self) -> SFTPAttributes: ...
     def chmod(self, mode: int) -> None: ...
     def chown(self, uid: int, gid: int) -> None: ...
     def utime(self, times: tuple[float, float] | None) -> None: ...
     def truncate(self, size: int) -> None: ...
     def check(self, hash_algorithm: str, offset: int = 0, length: int = 0, block_size: int = 0) -> bytes: ...
     def set_pipelined(self, pipelined: bool = True) -> None: ...
-    def prefetch(self, file_size: int | None = None) -> None: ...
-    def readv(self, chunks: Sequence[tuple[int, int]]) -> Iterator[bytes]: ...
+    def prefetch(self, file_size: int | None = None, max_concurrent_requests: int | None = None) -> None: ...
+    def readv(
+        self, chunks: Sequence[tuple[int, int]], max_concurrent_prefetch_requests: int | None = None
+    ) -> Iterator[bytes]: ...
```

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/sftp_server.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/sftp_server.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/sftp_si.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/sftp_si.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/ssh_exception.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/ssh_exception.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/ssh_gss.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/ssh_gss.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/transport.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/transport.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.2.0.1/paramiko-stubs/util.pyi` & `types-paramiko-3.3.0.0/paramiko-stubs/util.pyi`

 * *Files identical despite different names*

### Comparing `types-paramiko-3.2.0.1/setup.py` & `types-paramiko-3.3.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
-with mypy 1.4.1, pyright 1.1.318, and
-pytype 2023.6.16.
+This package was generated from typeshed commit `fe2ebd69af14d376825f21182d415223bd037485` and was tested
+with mypy 1.4.1, pyright 1.1.319, and
+pytype 2023.7.21.
 '''.lstrip()
 
 setup(name=name,
-      version="3.2.0.1",
+      version="3.3.0.0",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/paramiko.md",
```

### Comparing `types-paramiko-3.2.0.1/types_paramiko.egg-info/PKG-INFO` & `types-paramiko-3.3.0.0/types_paramiko.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-paramiko
-Version: 3.2.0.1
+Version: 3.3.0.0
 Summary: Typing stubs for paramiko
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/paramiko.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -26,10 +26,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
-with mypy 1.4.1, pyright 1.1.318, and
-pytype 2023.6.16.
+This package was generated from typeshed commit `fe2ebd69af14d376825f21182d415223bd037485` and was tested
+with mypy 1.4.1, pyright 1.1.319, and
+pytype 2023.7.21.
```

### Comparing `types-paramiko-3.2.0.1/types_paramiko.egg-info/SOURCES.txt` & `types-paramiko-3.3.0.0/types_paramiko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

