# Comparing `tmp/fluxoperator-0.0.31.tar.gz` & `tmp/fluxoperator-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluxoperator-0.0.31.tar", last modified: Sat Jul  1 08:16:07 2023, max compression
+gzip compressed data, was "fluxoperator-0.1.0.tar", last modified: Mon Jul 31 01:49:13 2023, max compression
```

## Comparing `fluxoperator-0.0.31.tar` & `fluxoperator-0.1.0.tar`

### file list

```diff
@@ -1,79 +1,81 @@
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 08:16:07.120089 fluxoperator-0.0.31/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2840 2023-07-01 08:16:07.120089 fluxoperator-0.0.31/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      391 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/README.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 08:16:07.116089 fluxoperator-0.0.31/fluxoperator/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2219 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/__init__.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 08:16:07.116089 fluxoperator-0.0.31/fluxoperator/api/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       87 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/api/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    27361 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/api_client.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13767 2023-06-28 02:00:02.000000 fluxoperator-0.0.31/fluxoperator/client.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16066 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/configuration.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      756 2023-04-07 19:58:49.000000 fluxoperator-0.0.31/fluxoperator/decorator.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       75 2023-04-07 19:58:49.000000 fluxoperator-0.0.31/fluxoperator/defaults.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5061 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/exceptions.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 08:16:07.120089 fluxoperator-0.0.31/fluxoperator/models/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1743 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4552 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/bursted_cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4674 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/bursting.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8452 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/commands.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4338 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/container_resources.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4322 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/container_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6193 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/flux_broker.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6774 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/flux_restful.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13103 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/flux_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4119 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/flux_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4402 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/life_cycle.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6622 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/logging_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7375 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/mini_cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3612 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/mini_cluster_archive.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    24483 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/mini_cluster_container.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8150 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/mini_cluster_existing_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6969 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/mini_cluster_list.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16961 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/mini_cluster_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7727 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/mini_cluster_status.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4434 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/mini_cluster_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13029 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/mini_cluster_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3714 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/network.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7124 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/pod_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4440 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/secret.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3683 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/models/security_context.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 08:16:07.120089 fluxoperator-0.0.31/fluxoperator/resource/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-04-07 19:58:49.000000 fluxoperator-0.0.31/fluxoperator/resource/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1910 2023-04-07 19:58:49.000000 fluxoperator-0.0.31/fluxoperator/resource/network.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6890 2023-06-25 05:43:00.000000 fluxoperator-0.0.31/fluxoperator/resource/pods.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12590 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/fluxoperator/rest.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 08:16:07.116089 fluxoperator-0.0.31/fluxoperator.egg-info/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2840 2023-07-01 08:16:07.000000 fluxoperator-0.0.31/fluxoperator.egg-info/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2207 2023-07-01 08:16:07.000000 fluxoperator-0.0.31/fluxoperator.egg-info/SOURCES.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-07-01 08:16:07.000000 fluxoperator-0.0.31/fluxoperator.egg-info/dependency_links.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-02-25 05:06:19.000000 fluxoperator-0.0.31/fluxoperator.egg-info/not-zip-safe
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       20 2023-07-01 08:16:07.000000 fluxoperator-0.0.31/fluxoperator.egg-info/requires.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       18 2023-07-01 08:16:07.000000 fluxoperator-0.0.31/fluxoperator.egg-info/top_level.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       69 2023-07-01 08:16:07.120089 fluxoperator-0.0.31/setup.cfg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2153 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/setup.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 08:16:07.120089 fluxoperator-0.0.31/test/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 08:12:31.000000 fluxoperator-0.0.31/test/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1352 2023-06-25 05:43:00.000000 fluxoperator-0.0.31/test/test_bursted_cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1831 2023-06-25 05:43:00.000000 fluxoperator-0.0.31/test/test_bursting.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1224 2023-04-07 19:58:49.000000 fluxoperator-0.0.31/test/test_commands.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1351 2023-04-07 19:58:49.000000 fluxoperator-0.0.31/test/test_container_resources.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1335 2023-04-07 19:58:49.000000 fluxoperator-0.0.31/test/test_container_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1341 2023-06-25 05:43:00.000000 fluxoperator-0.0.31/test/test_flux_broker.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1271 2023-04-07 19:58:49.000000 fluxoperator-0.0.31/test/test_flux_restful.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1234 2023-06-25 05:43:00.000000 fluxoperator-0.0.31/test/test_flux_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1212 2023-04-07 19:58:49.000000 fluxoperator-0.0.31/test/test_flux_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1226 2023-04-07 19:58:49.000000 fluxoperator-0.0.31/test/test_life_cycle.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1277 2023-04-07 19:58:49.000000 fluxoperator-0.0.31/test/test_logging_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7553 2023-06-25 05:43:00.000000 fluxoperator-0.0.31/test/test_mini_cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1316 2023-06-25 05:43:00.000000 fluxoperator-0.0.31/test/test_mini_cluster_archive.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3352 2023-06-25 05:43:00.000000 fluxoperator-0.0.31/test/test_mini_cluster_container.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1504 2023-06-25 05:43:00.000000 fluxoperator-0.0.31/test/test_mini_cluster_existing_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16512 2023-06-25 05:43:00.000000 fluxoperator-0.0.31/test/test_mini_cluster_list.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    11270 2023-06-25 05:43:00.000000 fluxoperator-0.0.31/test/test_mini_cluster_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1414 2023-06-25 05:43:00.000000 fluxoperator-0.0.31/test/test_mini_cluster_status.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1334 2023-06-25 05:43:00.000000 fluxoperator-0.0.31/test/test_mini_cluster_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1773 2023-06-25 05:43:00.000000 fluxoperator-0.0.31/test/test_mini_cluster_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1212 2023-06-25 05:43:00.000000 fluxoperator-0.0.31/test/test_network.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1284 2023-04-07 19:58:49.000000 fluxoperator-0.0.31/test/test_pod_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1314 2023-07-01 07:43:43.000000 fluxoperator-0.0.31/test/test_secret.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1289 2023-04-07 19:58:49.000000 fluxoperator-0.0.31/test/test_security_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:49:13.958217 fluxoperator-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-31 01:49:13.958217 fluxoperator-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:49:13.950217 fluxoperator-0.1.0/fluxoperator/
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:49:13.950217 fluxoperator-0.1.0/fluxoperator/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27361 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13767 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16066 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:49:13.954217 fluxoperator-0.1.0/fluxoperator/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/models/bursted_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/models/bursting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8452 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/models/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/models/container_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/models/container_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/models/flux_broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/models/flux_restful.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/models/flux_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13804 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/models/flux_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/models/flux_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/models/life_cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/models/logging_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/models/mini_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/models/mini_cluster_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23117 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/models/mini_cluster_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/models/mini_cluster_existing_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/models/mini_cluster_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18050 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/models/mini_cluster_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7727 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/models/mini_cluster_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/models/mini_cluster_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13029 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/models/mini_cluster_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/models/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/models/pod_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/models/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/models/security_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:49:13.954217 fluxoperator-0.1.0/fluxoperator/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/resource/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/resource/pods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12590 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/fluxoperator/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:49:13.950217 fluxoperator-0.1.0/fluxoperator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-31 01:49:13.000000 fluxoperator-0.1.0/fluxoperator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-31 01:49:13.000000 fluxoperator-0.1.0/fluxoperator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 01:49:13.000000 fluxoperator-0.1.0/fluxoperator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 01:49:13.000000 fluxoperator-0.1.0/fluxoperator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-31 01:49:13.000000 fluxoperator-0.1.0/fluxoperator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-31 01:49:13.000000 fluxoperator-0.1.0/fluxoperator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-31 01:49:13.958217 fluxoperator-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:49:13.958217 fluxoperator-0.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/test/test_bursted_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/test/test_bursting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/test/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/test/test_container_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/test/test_container_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/test/test_flux_broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/test/test_flux_restful.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/test/test_flux_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/test/test_flux_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/test/test_flux_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/test/test_life_cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/test/test_logging_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9923 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/test/test_mini_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/test/test_mini_cluster_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/test/test_mini_cluster_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/test/test_mini_cluster_existing_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21823 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/test/test_mini_cluster_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15021 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/test/test_mini_cluster_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/test/test_mini_cluster_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/test/test_mini_cluster_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/test/test_mini_cluster_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/test/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/test/test_pod_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/test/test_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-31 01:48:45.000000 fluxoperator-0.1.0/test/test_security_context.py
```

### Comparing `fluxoperator-0.0.31/PKG-INFO` & `fluxoperator-0.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: fluxoperator
-Version: 0.0.31
+Version: 0.1.0
 Summary: Python SDK for the Flux Operator
 Home-page: https://github.com/flux-framework/flux-operator/tree/main/python-sdk/v1alpha1
 Author: Vanessasaurus
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessasaurus
 License: Apache 2.0
 Keywords: flux-operator,flux-framework,kubernetes,workflows,jobs-api
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
@@ -79,16 +78,17 @@
 ## Documentation For Models
 
  - [BurstedCluster](BurstedCluster.md)
  - [Bursting](Bursting.md)
  - [Commands](Commands.md)
  - [ContainerResources](dContainerResources.md)
  - [ContainerVolume](ContainerVolume.md)
- - [FluxBroker](FluxBrokerl.md)
+ - [FluxBroker](FluxBroker.md)
  - [FluxRestful](FluxRestful.md)
+ - [FluxScheduler](FluxScheduler.md)
  - [FluxSpec](FluxSpec.md)
  - [FluxUser](FluxUser.md)
  - [LifeCycle](LifeCycle.md)
  - [LoggingSpec](LoggingSpec.md)
  - [MiniCluster](MiniCluster.md)
  - [MiniClusterArchive](MiniClusterArchive.md)
  - [MiniClusterContainer](MiniClusterContainer.md)
@@ -106,9 +106,7 @@
 ## Documentation For Authorization
 
  All endpoints do not require authorization (but they do require you have permission via your kubernetes config)
 
 ## Author
 
 - [@vsoch](https://github.com/vsoch)
-
-
```

### Comparing `fluxoperator-0.0.31/fluxoperator/__init__.py` & `fluxoperator-0.1.0/fluxoperator/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 from fluxoperator.models.bursted_cluster import BurstedCluster
 from fluxoperator.models.bursting import Bursting
 from fluxoperator.models.commands import Commands
 from fluxoperator.models.container_resources import ContainerResources
 from fluxoperator.models.container_volume import ContainerVolume
 from fluxoperator.models.flux_broker import FluxBroker
 from fluxoperator.models.flux_restful import FluxRestful
+from fluxoperator.models.flux_scheduler import FluxScheduler
 from fluxoperator.models.flux_spec import FluxSpec
 from fluxoperator.models.flux_user import FluxUser
 from fluxoperator.models.life_cycle import LifeCycle
 from fluxoperator.models.logging_spec import LoggingSpec
 from fluxoperator.models.mini_cluster import MiniCluster
 from fluxoperator.models.mini_cluster_archive import MiniClusterArchive
 from fluxoperator.models.mini_cluster_container import MiniClusterContainer
```

### Comparing `fluxoperator-0.0.31/fluxoperator/api_client.py` & `fluxoperator-0.1.0/fluxoperator/api_client.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/fluxoperator/client.py` & `fluxoperator-0.1.0/fluxoperator/client.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/fluxoperator/configuration.py` & `fluxoperator-0.1.0/fluxoperator/configuration.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/fluxoperator/decorator.py` & `fluxoperator-0.1.0/fluxoperator/decorator.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/fluxoperator/exceptions.py` & `fluxoperator-0.1.0/fluxoperator/exceptions.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/fluxoperator/models/__init__.py` & `fluxoperator-0.1.0/fluxoperator/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from fluxoperator.models.bursted_cluster import BurstedCluster
 from fluxoperator.models.bursting import Bursting
 from fluxoperator.models.commands import Commands
 from fluxoperator.models.container_resources import ContainerResources
 from fluxoperator.models.container_volume import ContainerVolume
 from fluxoperator.models.flux_broker import FluxBroker
 from fluxoperator.models.flux_restful import FluxRestful
+from fluxoperator.models.flux_scheduler import FluxScheduler
 from fluxoperator.models.flux_spec import FluxSpec
 from fluxoperator.models.flux_user import FluxUser
 from fluxoperator.models.life_cycle import LifeCycle
 from fluxoperator.models.logging_spec import LoggingSpec
 from fluxoperator.models.mini_cluster import MiniCluster
 from fluxoperator.models.mini_cluster_archive import MiniClusterArchive
 from fluxoperator.models.mini_cluster_container import MiniClusterContainer
```

### Comparing `fluxoperator-0.0.31/fluxoperator/models/bursted_cluster.py` & `fluxoperator-0.1.0/fluxoperator/models/bursted_cluster.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/fluxoperator/models/bursting.py` & `fluxoperator-0.1.0/fluxoperator/models/flux_user.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,97 +14,98 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from fluxoperator.configuration import Configuration
 
 
-class Bursting(object):
+class FluxUser(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'clusters': 'list[BurstedCluster]',
-        'lead_broker': 'FluxBroker'
+        'name': 'str',
+        'uid': 'int'
     }
 
     attribute_map = {
-        'clusters': 'clusters',
-        'lead_broker': 'leadBroker'
+        'name': 'name',
+        'uid': 'uid'
     }
 
-    def __init__(self, clusters=None, lead_broker=None, local_vars_configuration=None):  # noqa: E501
-        """Bursting - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, name='flux', uid=1000, local_vars_configuration=None):  # noqa: E501
+        """FluxUser - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._clusters = None
-        self._lead_broker = None
+        self._name = None
+        self._uid = None
         self.discriminator = None
 
-        self.clusters = clusters
-        if lead_broker is not None:
-            self.lead_broker = lead_broker
+        if name is not None:
+            self.name = name
+        if uid is not None:
+            self.uid = uid
 
     @property
-    def clusters(self):
-        """Gets the clusters of this Bursting.  # noqa: E501
+    def name(self):
+        """Gets the name of this FluxUser.  # noqa: E501
 
-        External clusters to burst to. Each external cluster must share the same listing to align ranks  # noqa: E501
+        Flux user name  # noqa: E501
 
-        :return: The clusters of this Bursting.  # noqa: E501
-        :rtype: list[BurstedCluster]
+        :return: The name of this FluxUser.  # noqa: E501
+        :rtype: str
         """
-        return self._clusters
+        return self._name
 
-    @clusters.setter
-    def clusters(self, clusters):
-        """Sets the clusters of this Bursting.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this FluxUser.
 
-        External clusters to burst to. Each external cluster must share the same listing to align ranks  # noqa: E501
+        Flux user name  # noqa: E501
 
-        :param clusters: The clusters of this Bursting.  # noqa: E501
-        :type clusters: list[BurstedCluster]
+        :param name: The name of this FluxUser.  # noqa: E501
+        :type name: str
         """
-        if self.local_vars_configuration.client_side_validation and clusters is None:  # noqa: E501
-            raise ValueError("Invalid value for `clusters`, must not be `None`")  # noqa: E501
 
-        self._clusters = clusters
+        self._name = name
 
     @property
-    def lead_broker(self):
-        """Gets the lead_broker of this Bursting.  # noqa: E501
+    def uid(self):
+        """Gets the uid of this FluxUser.  # noqa: E501
 
+        UID for the FluxUser  # noqa: E501
 
-        :return: The lead_broker of this Bursting.  # noqa: E501
-        :rtype: FluxBroker
+        :return: The uid of this FluxUser.  # noqa: E501
+        :rtype: int
         """
-        return self._lead_broker
+        return self._uid
 
-    @lead_broker.setter
-    def lead_broker(self, lead_broker):
-        """Sets the lead_broker of this Bursting.
+    @uid.setter
+    def uid(self, uid):
+        """Sets the uid of this FluxUser.
 
+        UID for the FluxUser  # noqa: E501
 
-        :param lead_broker: The lead_broker of this Bursting.  # noqa: E501
-        :type lead_broker: FluxBroker
+        :param uid: The uid of this FluxUser.  # noqa: E501
+        :type uid: int
         """
 
-        self._lead_broker = lead_broker
+        self._uid = uid
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -140,18 +141,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Bursting):
+        if not isinstance(other, FluxUser):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Bursting):
+        if not isinstance(other, FluxUser):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `fluxoperator-0.0.31/fluxoperator/models/commands.py` & `fluxoperator-0.1.0/fluxoperator/models/commands.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/fluxoperator/models/container_resources.py` & `fluxoperator-0.1.0/fluxoperator/models/container_resources.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/fluxoperator/models/container_volume.py` & `fluxoperator-0.1.0/fluxoperator/models/container_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/fluxoperator/models/flux_broker.py` & `fluxoperator-0.1.0/fluxoperator/models/flux_broker.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/fluxoperator/models/flux_restful.py` & `fluxoperator-0.1.0/fluxoperator/models/flux_restful.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/fluxoperator/models/flux_spec.py` & `fluxoperator-0.1.0/fluxoperator/models/flux_spec.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,32 +39,34 @@
         'curve_cert': 'str',
         'curve_cert_secret': 'str',
         'install_root': 'str',
         'log_level': 'int',
         'minimal_service': 'bool',
         'munge_secret': 'str',
         'option_flags': 'str',
+        'scheduler': 'FluxScheduler',
         'wrap': 'str'
     }
 
     attribute_map = {
         'broker_config': 'brokerConfig',
         'bursting': 'bursting',
         'connect_timeout': 'connectTimeout',
         'curve_cert': 'curveCert',
         'curve_cert_secret': 'curveCertSecret',
         'install_root': 'installRoot',
         'log_level': 'logLevel',
         'minimal_service': 'minimalService',
         'munge_secret': 'mungeSecret',
         'option_flags': 'optionFlags',
+        'scheduler': 'scheduler',
         'wrap': 'wrap'
     }
 
-    def __init__(self, broker_config='', bursting=None, connect_timeout='5s', curve_cert='', curve_cert_secret='', install_root='/usr', log_level=6, minimal_service=False, munge_secret='', option_flags='', wrap=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, broker_config='', bursting=None, connect_timeout='5s', curve_cert='', curve_cert_secret='', install_root='/usr', log_level=6, minimal_service=False, munge_secret='', option_flags='', scheduler=None, wrap=None, local_vars_configuration=None):  # noqa: E501
         """FluxSpec - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._broker_config = None
         self._bursting = None
@@ -72,14 +74,15 @@
         self._curve_cert = None
         self._curve_cert_secret = None
         self._install_root = None
         self._log_level = None
         self._minimal_service = None
         self._munge_secret = None
         self._option_flags = None
+        self._scheduler = None
         self._wrap = None
         self.discriminator = None
 
         if broker_config is not None:
             self.broker_config = broker_config
         if bursting is not None:
             self.bursting = bursting
@@ -95,14 +98,16 @@
             self.log_level = log_level
         if minimal_service is not None:
             self.minimal_service = minimal_service
         if munge_secret is not None:
             self.munge_secret = munge_secret
         if option_flags is not None:
             self.option_flags = option_flags
+        if scheduler is not None:
+            self.scheduler = scheduler
         if wrap is not None:
             self.wrap = wrap
 
     @property
     def broker_config(self):
         """Gets the broker_config of this FluxSpec.  # noqa: E501
 
@@ -327,14 +332,35 @@
         :param option_flags: The option_flags of this FluxSpec.  # noqa: E501
         :type option_flags: str
         """
 
         self._option_flags = option_flags
 
     @property
+    def scheduler(self):
+        """Gets the scheduler of this FluxSpec.  # noqa: E501
+
+
+        :return: The scheduler of this FluxSpec.  # noqa: E501
+        :rtype: FluxScheduler
+        """
+        return self._scheduler
+
+    @scheduler.setter
+    def scheduler(self, scheduler):
+        """Sets the scheduler of this FluxSpec.
+
+
+        :param scheduler: The scheduler of this FluxSpec.  # noqa: E501
+        :type scheduler: FluxScheduler
+        """
+
+        self._scheduler = scheduler
+
+    @property
     def wrap(self):
         """Gets the wrap of this FluxSpec.  # noqa: E501
 
         Commands for flux start --wrap  # noqa: E501
 
         :return: The wrap of this FluxSpec.  # noqa: E501
         :rtype: str
```

### Comparing `fluxoperator-0.0.31/fluxoperator/models/flux_user.py` & `fluxoperator-0.1.0/fluxoperator/models/secret.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,98 +14,100 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from fluxoperator.configuration import Configuration
 
 
-class FluxUser(object):
+class Secret(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'name': 'str',
-        'uid': 'int'
+        'key': 'str',
+        'name': 'str'
     }
 
     attribute_map = {
-        'name': 'name',
-        'uid': 'uid'
+        'key': 'key',
+        'name': 'name'
     }
 
-    def __init__(self, name='flux', uid=1000, local_vars_configuration=None):  # noqa: E501
-        """FluxUser - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, key='', name='', local_vars_configuration=None):  # noqa: E501
+        """Secret - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
+        self._key = None
         self._name = None
-        self._uid = None
         self.discriminator = None
 
-        if name is not None:
-            self.name = name
-        if uid is not None:
-            self.uid = uid
+        self.key = key
+        self.name = name
 
     @property
-    def name(self):
-        """Gets the name of this FluxUser.  # noqa: E501
+    def key(self):
+        """Gets the key of this Secret.  # noqa: E501
 
-        Flux user name  # noqa: E501
+        Key under secretKeyRef->Key  # noqa: E501
 
-        :return: The name of this FluxUser.  # noqa: E501
+        :return: The key of this Secret.  # noqa: E501
         :rtype: str
         """
-        return self._name
+        return self._key
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this FluxUser.
+    @key.setter
+    def key(self, key):
+        """Sets the key of this Secret.
 
-        Flux user name  # noqa: E501
+        Key under secretKeyRef->Key  # noqa: E501
 
-        :param name: The name of this FluxUser.  # noqa: E501
-        :type name: str
+        :param key: The key of this Secret.  # noqa: E501
+        :type key: str
         """
+        if self.local_vars_configuration.client_side_validation and key is None:  # noqa: E501
+            raise ValueError("Invalid value for `key`, must not be `None`")  # noqa: E501
 
-        self._name = name
+        self._key = key
 
     @property
-    def uid(self):
-        """Gets the uid of this FluxUser.  # noqa: E501
+    def name(self):
+        """Gets the name of this Secret.  # noqa: E501
 
-        UID for the FluxUser  # noqa: E501
+        Name under secretKeyRef->Name  # noqa: E501
 
-        :return: The uid of this FluxUser.  # noqa: E501
-        :rtype: int
+        :return: The name of this Secret.  # noqa: E501
+        :rtype: str
         """
-        return self._uid
+        return self._name
 
-    @uid.setter
-    def uid(self, uid):
-        """Sets the uid of this FluxUser.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this Secret.
 
-        UID for the FluxUser  # noqa: E501
+        Name under secretKeyRef->Name  # noqa: E501
 
-        :param uid: The uid of this FluxUser.  # noqa: E501
-        :type uid: int
+        :param name: The name of this Secret.  # noqa: E501
+        :type name: str
         """
+        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
-        self._uid = uid
+        self._name = name
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -141,18 +143,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, FluxUser):
+        if not isinstance(other, Secret):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, FluxUser):
+        if not isinstance(other, Secret):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `fluxoperator-0.0.31/fluxoperator/models/life_cycle.py` & `fluxoperator-0.1.0/fluxoperator/models/life_cycle.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/fluxoperator/models/logging_spec.py` & `fluxoperator-0.1.0/fluxoperator/models/logging_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/fluxoperator/models/mini_cluster.py` & `fluxoperator-0.1.0/fluxoperator/models/mini_cluster.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/fluxoperator/models/mini_cluster_archive.py` & `fluxoperator-0.1.0/fluxoperator/models/mini_cluster_archive.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/fluxoperator/models/mini_cluster_container.py` & `fluxoperator-0.1.0/fluxoperator/models/mini_cluster_container.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,15 +45,14 @@
         'image': 'str',
         'image_pull_secret': 'str',
         'launcher': 'bool',
         'life_cycle': 'LifeCycle',
         'logs': 'str',
         'name': 'str',
         'ports': 'list[int]',
-        'pre_command': 'str',
         'pull_always': 'bool',
         'resources': 'ContainerResources',
         'run_flux': 'bool',
         'secrets': 'dict(str, Secret)',
         'security_context': 'SecurityContext',
         'volumes': 'dict(str, ContainerVolume)',
         'working_dir': 'str'
@@ -72,25 +71,24 @@
         'image': 'image',
         'image_pull_secret': 'imagePullSecret',
         'launcher': 'launcher',
         'life_cycle': 'lifeCycle',
         'logs': 'logs',
         'name': 'name',
         'ports': 'ports',
-        'pre_command': 'preCommand',
         'pull_always': 'pullAlways',
         'resources': 'resources',
         'run_flux': 'runFlux',
         'secrets': 'secrets',
         'security_context': 'securityContext',
         'volumes': 'volumes',
         'working_dir': 'workingDir'
     }
 
-    def __init__(self, batch=False, batch_raw=False, command='', commands=None, cores=0, diagnostics=False, environment=None, existing_volumes=None, flux_user=None, image='ghcr.io/rse-ops/accounting:app-latest', image_pull_secret='', launcher=False, life_cycle=None, logs='', name='', ports=None, pre_command='', pull_always=False, resources=None, run_flux=False, secrets=None, security_context=None, volumes=None, working_dir='', local_vars_configuration=None):  # noqa: E501
+    def __init__(self, batch=False, batch_raw=False, command='', commands=None, cores=0, diagnostics=False, environment=None, existing_volumes=None, flux_user=None, image='ghcr.io/rse-ops/accounting:app-latest', image_pull_secret='', launcher=False, life_cycle=None, logs='', name='', ports=None, pull_always=False, resources=None, run_flux=False, secrets=None, security_context=None, volumes=None, working_dir='', local_vars_configuration=None):  # noqa: E501
         """MiniClusterContainer - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._batch = None
         self._batch_raw = None
@@ -104,15 +102,14 @@
         self._image = None
         self._image_pull_secret = None
         self._launcher = None
         self._life_cycle = None
         self._logs = None
         self._name = None
         self._ports = None
-        self._pre_command = None
         self._pull_always = None
         self._resources = None
         self._run_flux = None
         self._secrets = None
         self._security_context = None
         self._volumes = None
         self._working_dir = None
@@ -146,16 +143,14 @@
             self.life_cycle = life_cycle
         if logs is not None:
             self.logs = logs
         if name is not None:
             self.name = name
         if ports is not None:
             self.ports = ports
-        if pre_command is not None:
-            self.pre_command = pre_command
         if pull_always is not None:
             self.pull_always = pull_always
         if resources is not None:
             self.resources = resources
         if run_flux is not None:
             self.run_flux = run_flux
         if secrets is not None:
@@ -526,37 +521,14 @@
         :param ports: The ports of this MiniClusterContainer.  # noqa: E501
         :type ports: list[int]
         """
 
         self._ports = ports
 
     @property
-    def pre_command(self):
-        """Gets the pre_command of this MiniClusterContainer.  # noqa: E501
-
-        Special command to run at beginning of script, directly after asFlux is defined as sudo -u flux -E (so you can change that if desired.) This is only valid if FluxRunner is set (that writes a wait.sh script) This is for the indexed job pods and the certificate generation container.  # noqa: E501
-
-        :return: The pre_command of this MiniClusterContainer.  # noqa: E501
-        :rtype: str
-        """
-        return self._pre_command
-
-    @pre_command.setter
-    def pre_command(self, pre_command):
-        """Sets the pre_command of this MiniClusterContainer.
-
-        Special command to run at beginning of script, directly after asFlux is defined as sudo -u flux -E (so you can change that if desired.) This is only valid if FluxRunner is set (that writes a wait.sh script) This is for the indexed job pods and the certificate generation container.  # noqa: E501
-
-        :param pre_command: The pre_command of this MiniClusterContainer.  # noqa: E501
-        :type pre_command: str
-        """
-
-        self._pre_command = pre_command
-
-    @property
     def pull_always(self):
         """Gets the pull_always of this MiniClusterContainer.  # noqa: E501
 
         Allow the user to dictate pulling By default we pull if not present. Setting this to true will indicate to pull always  # noqa: E501
 
         :return: The pull_always of this MiniClusterContainer.  # noqa: E501
         :rtype: bool
```

### Comparing `fluxoperator-0.0.31/fluxoperator/models/mini_cluster_existing_volume.py` & `fluxoperator-0.1.0/fluxoperator/models/mini_cluster_existing_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/fluxoperator/models/mini_cluster_list.py` & `fluxoperator-0.1.0/fluxoperator/models/mini_cluster_list.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/fluxoperator/models/mini_cluster_spec.py` & `fluxoperator-0.1.0/fluxoperator/models/mini_cluster_spec.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         'interactive': 'bool',
         'job_labels': 'dict(str, str)',
         'logging': 'LoggingSpec',
         'max_size': 'int',
         'network': 'Network',
         'pod': 'PodSpec',
         'services': 'list[MiniClusterContainer]',
+        'share_process_namespace': 'bool',
         'size': 'int',
         'tasks': 'int',
         'users': 'list[MiniClusterUser]',
         'volumes': 'dict(str, MiniClusterVolume)'
     }
 
     attribute_map = {
@@ -62,21 +63,22 @@
         'interactive': 'interactive',
         'job_labels': 'jobLabels',
         'logging': 'logging',
         'max_size': 'maxSize',
         'network': 'network',
         'pod': 'pod',
         'services': 'services',
+        'share_process_namespace': 'shareProcessNamespace',
         'size': 'size',
         'tasks': 'tasks',
         'users': 'users',
         'volumes': 'volumes'
     }
 
-    def __init__(self, archive=None, cleanup=False, containers=None, deadline_seconds=31500000, flux=None, flux_restful=None, interactive=False, job_labels=None, logging=None, max_size=None, network=None, pod=None, services=None, size=1, tasks=1, users=None, volumes=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, archive=None, cleanup=False, containers=None, deadline_seconds=31500000, flux=None, flux_restful=None, interactive=False, job_labels=None, logging=None, max_size=None, network=None, pod=None, services=None, share_process_namespace=False, size=1, tasks=1, users=None, volumes=None, local_vars_configuration=None):  # noqa: E501
         """MiniClusterSpec - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._archive = None
         self._cleanup = None
@@ -87,14 +89,15 @@
         self._interactive = None
         self._job_labels = None
         self._logging = None
         self._max_size = None
         self._network = None
         self._pod = None
         self._services = None
+        self._share_process_namespace = None
         self._size = None
         self._tasks = None
         self._users = None
         self._volumes = None
         self.discriminator = None
 
         if archive is not None:
@@ -118,14 +121,16 @@
             self.max_size = max_size
         if network is not None:
             self.network = network
         if pod is not None:
             self.pod = pod
         if services is not None:
             self.services = services
+        if share_process_namespace is not None:
+            self.share_process_namespace = share_process_namespace
         if size is not None:
             self.size = size
         if tasks is not None:
             self.tasks = tasks
         if users is not None:
             self.users = users
         if volumes is not None:
@@ -417,14 +422,37 @@
         :param services: The services of this MiniClusterSpec.  # noqa: E501
         :type services: list[MiniClusterContainer]
         """
 
         self._services = services
 
     @property
+    def share_process_namespace(self):
+        """Gets the share_process_namespace of this MiniClusterSpec.  # noqa: E501
+
+        Share process namespace?  # noqa: E501
+
+        :return: The share_process_namespace of this MiniClusterSpec.  # noqa: E501
+        :rtype: bool
+        """
+        return self._share_process_namespace
+
+    @share_process_namespace.setter
+    def share_process_namespace(self, share_process_namespace):
+        """Sets the share_process_namespace of this MiniClusterSpec.
+
+        Share process namespace?  # noqa: E501
+
+        :param share_process_namespace: The share_process_namespace of this MiniClusterSpec.  # noqa: E501
+        :type share_process_namespace: bool
+        """
+
+        self._share_process_namespace = share_process_namespace
+
+    @property
     def size(self):
         """Gets the size of this MiniClusterSpec.  # noqa: E501
 
         Size (number of job pods to run, size of minicluster in pods) This is also the minimum number required to start Flux  # noqa: E501
 
         :return: The size of this MiniClusterSpec.  # noqa: E501
         :rtype: int
```

### Comparing `fluxoperator-0.0.31/fluxoperator/models/mini_cluster_status.py` & `fluxoperator-0.1.0/fluxoperator/models/mini_cluster_status.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/fluxoperator/models/mini_cluster_user.py` & `fluxoperator-0.1.0/fluxoperator/models/mini_cluster_user.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/fluxoperator/models/mini_cluster_volume.py` & `fluxoperator-0.1.0/fluxoperator/models/mini_cluster_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/fluxoperator/models/network.py` & `fluxoperator-0.1.0/fluxoperator/models/network.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/fluxoperator/models/pod_spec.py` & `fluxoperator-0.1.0/fluxoperator/models/pod_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/fluxoperator/models/security_context.py` & `fluxoperator-0.1.0/fluxoperator/models/flux_scheduler.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,70 +14,70 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from fluxoperator.configuration import Configuration
 
 
-class SecurityContext(object):
+class FluxScheduler(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'privileged': 'bool'
+        'queue_policy': 'str'
     }
 
     attribute_map = {
-        'privileged': 'privileged'
+        'queue_policy': 'queuePolicy'
     }
 
-    def __init__(self, privileged=None, local_vars_configuration=None):  # noqa: E501
-        """SecurityContext - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, queue_policy='', local_vars_configuration=None):  # noqa: E501
+        """FluxScheduler - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._privileged = None
+        self._queue_policy = None
         self.discriminator = None
 
-        if privileged is not None:
-            self.privileged = privileged
+        if queue_policy is not None:
+            self.queue_policy = queue_policy
 
     @property
-    def privileged(self):
-        """Gets the privileged of this SecurityContext.  # noqa: E501
+    def queue_policy(self):
+        """Gets the queue_policy of this FluxScheduler.  # noqa: E501
 
-        Privileged container  # noqa: E501
+        Scheduler queue policy, defaults to \"fcfs\" can also be \"easy\"  # noqa: E501
 
-        :return: The privileged of this SecurityContext.  # noqa: E501
-        :rtype: bool
+        :return: The queue_policy of this FluxScheduler.  # noqa: E501
+        :rtype: str
         """
-        return self._privileged
+        return self._queue_policy
 
-    @privileged.setter
-    def privileged(self, privileged):
-        """Sets the privileged of this SecurityContext.
+    @queue_policy.setter
+    def queue_policy(self, queue_policy):
+        """Sets the queue_policy of this FluxScheduler.
 
-        Privileged container  # noqa: E501
+        Scheduler queue policy, defaults to \"fcfs\" can also be \"easy\"  # noqa: E501
 
-        :param privileged: The privileged of this SecurityContext.  # noqa: E501
-        :type privileged: bool
+        :param queue_policy: The queue_policy of this FluxScheduler.  # noqa: E501
+        :type queue_policy: str
         """
 
-        self._privileged = privileged
+        self._queue_policy = queue_policy
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -113,18 +113,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SecurityContext):
+        if not isinstance(other, FluxScheduler):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, SecurityContext):
+        if not isinstance(other, FluxScheduler):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `fluxoperator-0.0.31/fluxoperator/resource/network.py` & `fluxoperator-0.1.0/fluxoperator/resource/network.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/fluxoperator/resource/pods.py` & `fluxoperator-0.1.0/fluxoperator/resource/pods.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/fluxoperator/rest.py` & `fluxoperator-0.1.0/fluxoperator/rest.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/fluxoperator.egg-info/PKG-INFO` & `fluxoperator-0.1.0/fluxoperator.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: fluxoperator
-Version: 0.0.31
+Version: 0.1.0
 Summary: Python SDK for the Flux Operator
 Home-page: https://github.com/flux-framework/flux-operator/tree/main/python-sdk/v1alpha1
 Author: Vanessasaurus
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessasaurus
 License: Apache 2.0
 Keywords: flux-operator,flux-framework,kubernetes,workflows,jobs-api
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
@@ -79,16 +78,17 @@
 ## Documentation For Models
 
  - [BurstedCluster](BurstedCluster.md)
  - [Bursting](Bursting.md)
  - [Commands](Commands.md)
  - [ContainerResources](dContainerResources.md)
  - [ContainerVolume](ContainerVolume.md)
- - [FluxBroker](FluxBrokerl.md)
+ - [FluxBroker](FluxBroker.md)
  - [FluxRestful](FluxRestful.md)
+ - [FluxScheduler](FluxScheduler.md)
  - [FluxSpec](FluxSpec.md)
  - [FluxUser](FluxUser.md)
  - [LifeCycle](LifeCycle.md)
  - [LoggingSpec](LoggingSpec.md)
  - [MiniCluster](MiniCluster.md)
  - [MiniClusterArchive](MiniClusterArchive.md)
  - [MiniClusterContainer](MiniClusterContainer.md)
@@ -106,9 +106,7 @@
 ## Documentation For Authorization
 
  All endpoints do not require authorization (but they do require you have permission via your kubernetes config)
 
 ## Author
 
 - [@vsoch](https://github.com/vsoch)
-
-
```

### Comparing `fluxoperator-0.0.31/fluxoperator.egg-info/SOURCES.txt` & `fluxoperator-0.1.0/fluxoperator.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 fluxoperator/models/bursted_cluster.py
 fluxoperator/models/bursting.py
 fluxoperator/models/commands.py
 fluxoperator/models/container_resources.py
 fluxoperator/models/container_volume.py
 fluxoperator/models/flux_broker.py
 fluxoperator/models/flux_restful.py
+fluxoperator/models/flux_scheduler.py
 fluxoperator/models/flux_spec.py
 fluxoperator/models/flux_user.py
 fluxoperator/models/life_cycle.py
 fluxoperator/models/logging_spec.py
 fluxoperator/models/mini_cluster.py
 fluxoperator/models/mini_cluster_archive.py
 fluxoperator/models/mini_cluster_container.py
@@ -48,14 +49,15 @@
 test/test_bursted_cluster.py
 test/test_bursting.py
 test/test_commands.py
 test/test_container_resources.py
 test/test_container_volume.py
 test/test_flux_broker.py
 test/test_flux_restful.py
+test/test_flux_scheduler.py
 test/test_flux_spec.py
 test/test_flux_user.py
 test/test_life_cycle.py
 test/test_logging_spec.py
 test/test_mini_cluster.py
 test/test_mini_cluster_archive.py
 test/test_mini_cluster_container.py
```

### Comparing `fluxoperator-0.0.31/setup.py` & `fluxoperator-0.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ################################################################################
 # MAIN #########################################################################
 ################################################################################
 
 if __name__ == "__main__":
     setup(
         name="fluxoperator",
-        version="0.0.31",
+        version="0.1.0",
         author="Vanessasaurus",
         author_email="vsoch@users.noreply.github.com",
         maintainer="Vanessasaurus",
         packages=find_packages(),
         include_package_data=True,
         zip_safe=False,
         url="https://github.com/flux-framework/flux-operator/tree/main/python-sdk/v1alpha1",
```

### Comparing `fluxoperator-0.0.31/test/test_bursted_cluster.py` & `fluxoperator-0.1.0/test/test_bursted_cluster.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/test/test_bursting.py` & `fluxoperator-0.1.0/test/test_bursting.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/test/test_commands.py` & `fluxoperator-0.1.0/test/test_commands.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/test/test_container_resources.py` & `fluxoperator-0.1.0/test/test_container_resources.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/test/test_container_volume.py` & `fluxoperator-0.1.0/test/test_container_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/test/test_flux_broker.py` & `fluxoperator-0.1.0/test/test_flux_broker.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/test/test_flux_restful.py` & `fluxoperator-0.1.0/test/test_flux_restful.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/test/test_flux_spec.py` & `fluxoperator-0.1.0/test/test_flux_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/test/test_flux_user.py` & `fluxoperator-0.1.0/test/test_flux_user.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/test/test_life_cycle.py` & `fluxoperator-0.1.0/test/test_life_cycle.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/test/test_logging_spec.py` & `fluxoperator-0.1.0/test/test_logging_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/test/test_mini_cluster_archive.py` & `fluxoperator-0.1.0/test/test_mini_cluster_user.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,39 +12,42 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import fluxoperator
-from fluxoperator.models.mini_cluster_archive import MiniClusterArchive  # noqa: E501
+from fluxoperator.models.mini_cluster_user import MiniClusterUser  # noqa: E501
 from fluxoperator.rest import ApiException
 
-
-class TestMiniClusterArchive(unittest.TestCase):
-    """MiniClusterArchive unit test stubs"""
+class TestMiniClusterUser(unittest.TestCase):
+    """MiniClusterUser unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test MiniClusterArchive
-        include_option is a boolean, when False only required
-        params are included, when True both required and
-        optional params are included"""
-        # model = fluxoperator.models.mini_cluster_archive.MiniClusterArchive()  # noqa: E501
-        if include_optional:
-            return MiniClusterArchive(path="")
-        else:
-            return MiniClusterArchive()
+        """Test MiniClusterUser
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # model = fluxoperator.models.mini_cluster_user.MiniClusterUser()  # noqa: E501
+        if include_optional :
+            return MiniClusterUser(
+                name = '', 
+                password = ''
+            )
+        else :
+            return MiniClusterUser(
+                name = '',
+        )
 
-    def testMiniClusterArchive(self):
-        """Test MiniClusterArchive"""
+    def testMiniClusterUser(self):
+        """Test MiniClusterUser"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
-
-if __name__ == "__main__":
+if __name__ == '__main__':
     unittest.main()
```

### Comparing `fluxoperator-0.0.31/test/test_mini_cluster_existing_volume.py` & `fluxoperator-0.1.0/test/test_mini_cluster_existing_volume.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,44 +12,47 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import fluxoperator
-from fluxoperator.models.mini_cluster_existing_volume import (
-    MiniClusterExistingVolume,
-)  # noqa: E501
+from fluxoperator.models.mini_cluster_existing_volume import MiniClusterExistingVolume  # noqa: E501
 from fluxoperator.rest import ApiException
 
-
 class TestMiniClusterExistingVolume(unittest.TestCase):
     """MiniClusterExistingVolume unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
         """Test MiniClusterExistingVolume
-        include_option is a boolean, when False only required
-        params are included, when True both required and
-        optional params are included"""
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
         # model = fluxoperator.models.mini_cluster_existing_volume.MiniClusterExistingVolume()  # noqa: E501
-        if include_optional:
-            return MiniClusterExistingVolume(claim_name="", path="", read_only=True)
-        else:
+        if include_optional :
             return MiniClusterExistingVolume(
-                claim_name="",
-                path="",
+                claim_name = '', 
+                config_map_name = '', 
+                items = {
+                    'key' : ''
+                    }, 
+                path = '', 
+                read_only = True, 
+                secret_name = ''
             )
+        else :
+            return MiniClusterExistingVolume(
+        )
 
     def testMiniClusterExistingVolume(self):
         """Test MiniClusterExistingVolume"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
-
-if __name__ == "__main__":
+if __name__ == '__main__':
     unittest.main()
```

### Comparing `fluxoperator-0.0.31/test/test_mini_cluster_status.py` & `fluxoperator-0.1.0/test/test_mini_cluster_status.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,39 +15,47 @@
 import unittest
 import datetime
 
 import fluxoperator
 from fluxoperator.models.mini_cluster_status import MiniClusterStatus  # noqa: E501
 from fluxoperator.rest import ApiException
 
-
 class TestMiniClusterStatus(unittest.TestCase):
     """MiniClusterStatus unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
         """Test MiniClusterStatus
-        include_option is a boolean, when False only required
-        params are included, when True both required and
-        optional params are included"""
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
         # model = fluxoperator.models.mini_cluster_status.MiniClusterStatus()  # noqa: E501
-        if include_optional:
-            return MiniClusterStatus(conditions=[None], jobid="", maximum_size=56)
-        else:
+        if include_optional :
             return MiniClusterStatus(
-                jobid="",
-                maximum_size=56,
+                conditions = [
+                    None
+                    ], 
+                jobid = '', 
+                maximum_size = 56, 
+                selector = '', 
+                size = 56
             )
+        else :
+            return MiniClusterStatus(
+                jobid = '',
+                maximum_size = 56,
+                selector = '',
+                size = 56,
+        )
 
     def testMiniClusterStatus(self):
         """Test MiniClusterStatus"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
-
-if __name__ == "__main__":
+if __name__ == '__main__':
     unittest.main()
```

### Comparing `fluxoperator-0.0.31/test/test_mini_cluster_volume.py` & `fluxoperator-0.1.0/test/test_mini_cluster_volume.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,51 +15,57 @@
 import unittest
 import datetime
 
 import fluxoperator
 from fluxoperator.models.mini_cluster_volume import MiniClusterVolume  # noqa: E501
 from fluxoperator.rest import ApiException
 
-
 class TestMiniClusterVolume(unittest.TestCase):
     """MiniClusterVolume unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
         """Test MiniClusterVolume
-        include_option is a boolean, when False only required
-        params are included, when True both required and
-        optional params are included"""
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
         # model = fluxoperator.models.mini_cluster_volume.MiniClusterVolume()  # noqa: E501
-        if include_optional:
+        if include_optional :
             return MiniClusterVolume(
-                annotations={"key": ""},
-                attributes={"key": ""},
-                capacity="5Gi",
-                claim_annotations={"key": ""},
-                delete=True,
-                driver="",
-                labels={"key": ""},
-                path="",
-                secret="",
-                secret_namespace="default",
-                storage_class="hostpath",
-                volume_handle="",
+                annotations = {
+                    'key' : ''
+                    }, 
+                attributes = {
+                    'key' : ''
+                    }, 
+                capacity = '5Gi', 
+                claim_annotations = {
+                    'key' : ''
+                    }, 
+                delete = True, 
+                driver = '', 
+                labels = {
+                    'key' : ''
+                    }, 
+                path = '', 
+                secret = '', 
+                secret_namespace = 'default', 
+                storage_class = 'hostpath', 
+                volume_handle = ''
             )
-        else:
+        else :
             return MiniClusterVolume(
-                path="",
-            )
+                path = '',
+        )
 
     def testMiniClusterVolume(self):
         """Test MiniClusterVolume"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
-
-if __name__ == "__main__":
+if __name__ == '__main__':
     unittest.main()
```

### Comparing `fluxoperator-0.0.31/test/test_network.py` & `fluxoperator-0.1.0/test/test_network.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/test/test_pod_spec.py` & `fluxoperator-0.1.0/test/test_pod_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/test/test_secret.py` & `fluxoperator-0.1.0/test/test_secret.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.31/test/test_security_context.py` & `fluxoperator-0.1.0/test/test_security_context.py`

 * *Files identical despite different names*

