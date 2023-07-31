# Comparing `tmp/dingman-openapi-server-dev-1.0.0.tar.gz` & `tmp/dingman-openapi-server-dev-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dingman-openapi-server-dev-1.0.0.tar", last modified: Mon Jul 31 21:04:44 2023, max compression
+gzip compressed data, was "dist/dingman-openapi-server-dev-1.0.1.tar", last modified: Mon Jul 31 21:05:06 2023, max compression
```

## Comparing `dingman-openapi-server-dev-1.0.0.tar` & `dingman-openapi-server-dev-1.0.1.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-31 21:04:44.875650 dingman-openapi-server-dev-1.0.0/
--rw-r--r--   0 jialening   (501) staff       (20)       44 2023-07-14 22:13:36.000000 dingman-openapi-server-dev-1.0.0/MANIFEST.in
--rw-r--r--   0 jialening   (501) staff       (20)      330 2023-07-31 21:04:44.875385 dingman-openapi-server-dev-1.0.0/PKG-INFO
--rw-r--r--   0 jialening   (501) staff       (20)      902 2023-07-18 18:22:05.000000 dingman-openapi-server-dev-1.0.0/README.md
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-31 21:04:44.850281 dingman-openapi-server-dev-1.0.0/dingman_openapi_server_dev.egg-info/
--rw-r--r--   0 jialening   (501) staff       (20)      330 2023-07-31 21:04:44.000000 dingman-openapi-server-dev-1.0.0/dingman_openapi_server_dev.egg-info/PKG-INFO
--rw-r--r--   0 jialening   (501) staff       (20)     3372 2023-07-31 21:04:44.000000 dingman-openapi-server-dev-1.0.0/dingman_openapi_server_dev.egg-info/SOURCES.txt
--rw-r--r--   0 jialening   (501) staff       (20)        1 2023-07-31 21:04:44.000000 dingman-openapi-server-dev-1.0.0/dingman_openapi_server_dev.egg-info/dependency_links.txt
--rw-r--r--   0 jialening   (501) staff       (20)       20 2023-07-31 21:04:44.000000 dingman-openapi-server-dev-1.0.0/dingman_openapi_server_dev.egg-info/requires.txt
--rw-r--r--   0 jialening   (501) staff       (20)       15 2023-07-31 21:04:44.000000 dingman-openapi-server-dev-1.0.0/dingman_openapi_server_dev.egg-info/top_level.txt
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-31 21:04:44.852473 dingman-openapi-server-dev-1.0.0/openapi_server/
--rw-r--r--   0 jialening   (501) staff       (20)     6148 2023-07-14 22:13:36.000000 dingman-openapi-server-dev-1.0.0/openapi_server/.DS_Store
--rw-r--r--   0 jialening   (501) staff       (20)        0 2023-07-14 22:07:36.000000 dingman-openapi-server-dev-1.0.0/openapi_server/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)      393 2023-07-14 22:07:36.000000 dingman-openapi-server-dev-1.0.0/openapi_server/__main__.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-31 21:04:44.853541 dingman-openapi-server-dev-1.0.0/openapi_server/controllers/
--rw-r--r--   0 jialening   (501) staff       (20)        0 2023-07-14 22:07:36.000000 dingman-openapi-server-dev-1.0.0/openapi_server/controllers/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)     5687 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/controllers/deploy_resources_controller.py
--rw-r--r--   0 jialening   (501) staff       (20)      552 2023-07-14 22:07:36.000000 dingman-openapi-server-dev-1.0.0/openapi_server/controllers/security_controller_.py
--rw-r--r--   0 jialening   (501) staff       (20)      608 2023-07-14 22:07:36.000000 dingman-openapi-server-dev-1.0.0/openapi_server/encoder.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-31 21:04:44.873252 dingman-openapi-server-dev-1.0.0/openapi_server/models/
--rw-r--r--   0 jialening   (501) staff       (20)     4146 2023-07-25 23:32:32.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)     3753 2023-07-14 22:07:34.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/affinity.py
--rw-r--r--   0 jialening   (501) staff       (20)     1913 2023-07-14 22:07:36.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/base_model_.py
--rw-r--r--   0 jialening   (501) staff       (20)     4907 2023-07-14 22:07:34.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/config.py
--rw-r--r--   0 jialening   (501) staff       (20)     2503 2023-07-14 22:07:34.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/config_templates_inner.py
--rw-r--r--   0 jialening   (501) staff       (20)    16535 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/container.py
--rw-r--r--   0 jialening   (501) staff       (20)     2639 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/container_life_cycle.py
--rw-r--r--   0 jialening   (501) staff       (20)     3654 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/container_port.py
--rw-r--r--   0 jialening   (501) staff       (20)     3936 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/container_sec_context.py
--rw-r--r--   0 jialening   (501) staff       (20)     2568 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/container_sec_context_capabilities.py
--rw-r--r--   0 jialening   (501) staff       (20)    10247 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/deploy_platform_resource.py
--rw-r--r--   0 jialening   (501) staff       (20)     9794 2023-07-25 23:32:32.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/deploy_resources.py
--rw-r--r--   0 jialening   (501) staff       (20)     3963 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/dingman_error.py
--rw-r--r--   0 jialening   (501) staff       (20)     2425 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/dingman_response.py
--rw-r--r--   0 jialening   (501) staff       (20)    10477 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/endpoint.py
--rw-r--r--   0 jialening   (501) staff       (20)     3192 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/env_from_source.py
--rw-r--r--   0 jialening   (501) staff       (20)     2961 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/env_var.py
--rw-r--r--   0 jialening   (501) staff       (20)     1827 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/env_var_source.py
--rw-r--r--   0 jialening   (501) staff       (20)     4682 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/http_get.py
--rw-r--r--   0 jialening   (501) staff       (20)     4413 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/http_ingress_path.py
--rw-r--r--   0 jialening   (501) staff       (20)     5643 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/ingress.py
--rw-r--r--   0 jialening   (501) staff       (20)     1821 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/ingress_backend.py
--rw-r--r--   0 jialening   (501) staff       (20)     2446 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/ingress_backend_service.py
--rw-r--r--   0 jialening   (501) staff       (20)     3082 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/ingress_rule.py
--rw-r--r--   0 jialening   (501) staff       (20)     3211 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/ingress_tls.py
--rw-r--r--   0 jialening   (501) staff       (20)     3561 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/life_cycle_handler.py
--rw-r--r--   0 jialening   (501) staff       (20)     4613 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/node_affinity.py
--rw-r--r--   0 jialening   (501) staff       (20)     2047 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/node_selector.py
--rw-r--r--   0 jialening   (501) staff       (20)     3199 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/node_selector_term.py
--rw-r--r--   0 jialening   (501) staff       (20)     2827 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/object_field_selector.py
--rw-r--r--   0 jialening   (501) staff       (20)     9740 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/persistent_volume_claim.py
--rw-r--r--   0 jialening   (501) staff       (20)    12357 2023-07-20 23:40:33.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/pod.py
--rw-r--r--   0 jialening   (501) staff       (20)     4649 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/pod_affinity.py
--rw-r--r--   0 jialening   (501) staff       (20)     3664 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/pod_affinity_term.py
--rw-r--r--   0 jialening   (501) staff       (20)     4713 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/pod_anti_affinity.py
--rw-r--r--   0 jialening   (501) staff       (20)     3682 2023-07-14 22:13:36.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/pod_sec_context.py
--rw-r--r--   0 jialening   (501) staff       (20)     2623 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/preferred_scheduling_term.py
--rw-r--r--   0 jialening   (501) staff       (20)     7480 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/probe.py
--rw-r--r--   0 jialening   (501) staff       (20)     3138 2023-07-20 23:38:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/rbac_role_ref.py
--rw-r--r--   0 jialening   (501) staff       (20)     3577 2023-07-20 23:38:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/rbac_rule.py
--rw-r--r--   0 jialening   (501) staff       (20)     3598 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/ref_volume_source.py
--rw-r--r--   0 jialening   (501) staff       (20)     6245 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/relabel_config.py
--rw-r--r--   0 jialening   (501) staff       (20)     2787 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/resource_requirements.py
--rw-r--r--   0 jialening   (501) staff       (20)     4812 2023-07-20 23:38:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/role.py
--rw-r--r--   0 jialening   (501) staff       (20)     6130 2023-07-20 23:38:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/role_binding.py
--rw-r--r--   0 jialening   (501) staff       (20)     2365 2023-07-20 23:38:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/role_binding_subject.py
--rw-r--r--   0 jialening   (501) staff       (20)     4141 2023-07-25 23:32:32.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/secret.py
--rw-r--r--   0 jialening   (501) staff       (20)     8819 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/service.py
--rw-r--r--   0 jialening   (501) staff       (20)     7583 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/service_monitor.py
--rw-r--r--   0 jialening   (501) staff       (20)     3055 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/service_monitor_namespace_selector.py
--rw-r--r--   0 jialening   (501) staff       (20)     5386 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/service_port.py
--rw-r--r--   0 jialening   (501) staff       (20)     2189 2023-07-14 22:13:36.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/sysctl.py
--rw-r--r--   0 jialening   (501) staff       (20)     2413 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/tcp_socket.py
--rw-r--r--   0 jialening   (501) staff       (20)     5905 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/topology_spread_constraint.py
--rw-r--r--   0 jialening   (501) staff       (20)     3521 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/update_strategy.py
--rw-r--r--   0 jialening   (501) staff       (20)     4965 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/update_strategy_rolling_update_config.py
--rw-r--r--   0 jialening   (501) staff       (20)     6189 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/volume.py
--rw-r--r--   0 jialening   (501) staff       (20)     3553 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/volume_device.py
--rw-r--r--   0 jialening   (501) staff       (20)     2767 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/volume_empty_dir.py
--rw-r--r--   0 jialening   (501) staff       (20)     2585 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/volume_host_path.py
--rw-r--r--   0 jialening   (501) staff       (20)     4139 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/volume_mount.py
--rw-r--r--   0 jialening   (501) staff       (20)     2938 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/volume_persistent_volume_claim.py
--rw-r--r--   0 jialening   (501) staff       (20)     2769 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/weighted_pod_affinity_term.py
--rw-r--r--   0 jialening   (501) staff       (20)    13077 2023-07-20 23:40:33.000000 dingman-openapi-server-dev-1.0.0/openapi_server/models/workload.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-31 21:04:44.873554 dingman-openapi-server-dev-1.0.0/openapi_server/openapi/
--rw-r--r--   0 jialening   (501) staff       (20)   186818 2023-07-25 23:32:32.000000 dingman-openapi-server-dev-1.0.0/openapi_server/openapi/openapi.yaml
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-31 21:04:44.874774 dingman-openapi-server-dev-1.0.0/openapi_server/test/
--rw-r--r--   0 jialening   (501) staff       (20)      437 2023-07-14 22:07:36.000000 dingman-openapi-server-dev-1.0.0/openapi_server/test/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)   138979 2023-07-25 23:32:32.000000 dingman-openapi-server-dev-1.0.0/openapi_server/test/test_deploy_resources_controller.py
--rw-r--r--   0 jialening   (501) staff       (20)      809 2023-07-14 22:07:36.000000 dingman-openapi-server-dev-1.0.0/openapi_server/typing_utils.py
--rw-r--r--   0 jialening   (501) staff       (20)     3533 2023-07-14 22:07:36.000000 dingman-openapi-server-dev-1.0.0/openapi_server/util.py
--rw-r--r--   0 jialening   (501) staff       (20)        7 2023-07-31 06:45:53.000000 dingman-openapi-server-dev-1.0.0/openapi_version
--rw-r--r--   0 jialening   (501) staff       (20)       38 2023-07-31 21:04:44.875744 dingman-openapi-server-dev-1.0.0/setup.cfg
--rw-r--r--   0 jialening   (501) staff       (20)      903 2023-07-31 06:42:45.000000 dingman-openapi-server-dev-1.0.0/setup.py
--rw-r--r--   0 jialening   (501) staff       (20)     1328 2023-07-31 21:03:25.000000 dingman-openapi-server-dev-1.0.0/update_dev_pkg.py
+drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-31 21:05:06.185230 dingman-openapi-server-dev-1.0.1/
+-rw-r--r--   0 jialening   (501) staff       (20)       44 2023-07-14 22:13:36.000000 dingman-openapi-server-dev-1.0.1/MANIFEST.in
+-rw-r--r--   0 jialening   (501) staff       (20)      330 2023-07-31 21:05:06.184896 dingman-openapi-server-dev-1.0.1/PKG-INFO
+-rw-r--r--   0 jialening   (501) staff       (20)      902 2023-07-18 18:22:05.000000 dingman-openapi-server-dev-1.0.1/README.md
+drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-31 21:05:06.163522 dingman-openapi-server-dev-1.0.1/dingman_openapi_server_dev.egg-info/
+-rw-r--r--   0 jialening   (501) staff       (20)      330 2023-07-31 21:05:06.000000 dingman-openapi-server-dev-1.0.1/dingman_openapi_server_dev.egg-info/PKG-INFO
+-rw-r--r--   0 jialening   (501) staff       (20)     3372 2023-07-31 21:05:06.000000 dingman-openapi-server-dev-1.0.1/dingman_openapi_server_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 jialening   (501) staff       (20)        1 2023-07-31 21:05:06.000000 dingman-openapi-server-dev-1.0.1/dingman_openapi_server_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 jialening   (501) staff       (20)       20 2023-07-31 21:05:06.000000 dingman-openapi-server-dev-1.0.1/dingman_openapi_server_dev.egg-info/requires.txt
+-rw-r--r--   0 jialening   (501) staff       (20)       15 2023-07-31 21:05:06.000000 dingman-openapi-server-dev-1.0.1/dingman_openapi_server_dev.egg-info/top_level.txt
+drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-31 21:05:06.165009 dingman-openapi-server-dev-1.0.1/openapi_server/
+-rw-r--r--   0 jialening   (501) staff       (20)     6148 2023-07-14 22:13:36.000000 dingman-openapi-server-dev-1.0.1/openapi_server/.DS_Store
+-rw-r--r--   0 jialening   (501) staff       (20)        0 2023-07-14 22:07:36.000000 dingman-openapi-server-dev-1.0.1/openapi_server/__init__.py
+-rw-r--r--   0 jialening   (501) staff       (20)      393 2023-07-14 22:07:36.000000 dingman-openapi-server-dev-1.0.1/openapi_server/__main__.py
+drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-31 21:05:06.165723 dingman-openapi-server-dev-1.0.1/openapi_server/controllers/
+-rw-r--r--   0 jialening   (501) staff       (20)        0 2023-07-14 22:07:36.000000 dingman-openapi-server-dev-1.0.1/openapi_server/controllers/__init__.py
+-rw-r--r--   0 jialening   (501) staff       (20)     5687 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/controllers/deploy_resources_controller.py
+-rw-r--r--   0 jialening   (501) staff       (20)      552 2023-07-14 22:07:36.000000 dingman-openapi-server-dev-1.0.1/openapi_server/controllers/security_controller_.py
+-rw-r--r--   0 jialening   (501) staff       (20)      608 2023-07-14 22:07:36.000000 dingman-openapi-server-dev-1.0.1/openapi_server/encoder.py
+drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-31 21:05:06.183288 dingman-openapi-server-dev-1.0.1/openapi_server/models/
+-rw-r--r--   0 jialening   (501) staff       (20)     4146 2023-07-25 23:32:32.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/__init__.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3753 2023-07-14 22:07:34.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/affinity.py
+-rw-r--r--   0 jialening   (501) staff       (20)     1913 2023-07-14 22:07:36.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/base_model_.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4907 2023-07-14 22:07:34.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/config.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2503 2023-07-14 22:07:34.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/config_templates_inner.py
+-rw-r--r--   0 jialening   (501) staff       (20)    16535 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/container.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2639 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/container_life_cycle.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3654 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/container_port.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3936 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/container_sec_context.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2568 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/container_sec_context_capabilities.py
+-rw-r--r--   0 jialening   (501) staff       (20)    10247 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/deploy_platform_resource.py
+-rw-r--r--   0 jialening   (501) staff       (20)     9794 2023-07-25 23:32:32.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/deploy_resources.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3963 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/dingman_error.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2425 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/dingman_response.py
+-rw-r--r--   0 jialening   (501) staff       (20)    10477 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/endpoint.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3192 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/env_from_source.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2961 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/env_var.py
+-rw-r--r--   0 jialening   (501) staff       (20)     1827 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/env_var_source.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4682 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/http_get.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4413 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/http_ingress_path.py
+-rw-r--r--   0 jialening   (501) staff       (20)     5643 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/ingress.py
+-rw-r--r--   0 jialening   (501) staff       (20)     1821 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/ingress_backend.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2446 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/ingress_backend_service.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3082 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/ingress_rule.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3211 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/ingress_tls.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3561 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/life_cycle_handler.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4613 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/node_affinity.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2047 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/node_selector.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3199 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/node_selector_term.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2827 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/object_field_selector.py
+-rw-r--r--   0 jialening   (501) staff       (20)     9740 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/persistent_volume_claim.py
+-rw-r--r--   0 jialening   (501) staff       (20)    12357 2023-07-20 23:40:33.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/pod.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4649 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/pod_affinity.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3664 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/pod_affinity_term.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4713 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/pod_anti_affinity.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3682 2023-07-14 22:13:36.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/pod_sec_context.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2623 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/preferred_scheduling_term.py
+-rw-r--r--   0 jialening   (501) staff       (20)     7480 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/probe.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3138 2023-07-20 23:38:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/rbac_role_ref.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3577 2023-07-20 23:38:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/rbac_rule.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3598 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/ref_volume_source.py
+-rw-r--r--   0 jialening   (501) staff       (20)     6245 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/relabel_config.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2787 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/resource_requirements.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4812 2023-07-20 23:38:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/role.py
+-rw-r--r--   0 jialening   (501) staff       (20)     6130 2023-07-20 23:38:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/role_binding.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2365 2023-07-20 23:38:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/role_binding_subject.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4141 2023-07-25 23:32:32.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/secret.py
+-rw-r--r--   0 jialening   (501) staff       (20)     8819 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/service.py
+-rw-r--r--   0 jialening   (501) staff       (20)     7583 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/service_monitor.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3055 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/service_monitor_namespace_selector.py
+-rw-r--r--   0 jialening   (501) staff       (20)     5386 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/service_port.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2189 2023-07-14 22:13:36.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/sysctl.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2413 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/tcp_socket.py
+-rw-r--r--   0 jialening   (501) staff       (20)     5905 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/topology_spread_constraint.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3521 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/update_strategy.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4965 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/update_strategy_rolling_update_config.py
+-rw-r--r--   0 jialening   (501) staff       (20)     6189 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/volume.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3553 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/volume_device.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2767 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/volume_empty_dir.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2585 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/volume_host_path.py
+-rw-r--r--   0 jialening   (501) staff       (20)     4139 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/volume_mount.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2938 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/volume_persistent_volume_claim.py
+-rw-r--r--   0 jialening   (501) staff       (20)     2769 2023-07-14 22:07:35.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/weighted_pod_affinity_term.py
+-rw-r--r--   0 jialening   (501) staff       (20)    13077 2023-07-20 23:40:33.000000 dingman-openapi-server-dev-1.0.1/openapi_server/models/workload.py
+drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-31 21:05:06.183597 dingman-openapi-server-dev-1.0.1/openapi_server/openapi/
+-rw-r--r--   0 jialening   (501) staff       (20)   186818 2023-07-25 23:32:32.000000 dingman-openapi-server-dev-1.0.1/openapi_server/openapi/openapi.yaml
+drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-31 21:05:06.184353 dingman-openapi-server-dev-1.0.1/openapi_server/test/
+-rw-r--r--   0 jialening   (501) staff       (20)      437 2023-07-14 22:07:36.000000 dingman-openapi-server-dev-1.0.1/openapi_server/test/__init__.py
+-rw-r--r--   0 jialening   (501) staff       (20)   138979 2023-07-25 23:32:32.000000 dingman-openapi-server-dev-1.0.1/openapi_server/test/test_deploy_resources_controller.py
+-rw-r--r--   0 jialening   (501) staff       (20)      809 2023-07-14 22:07:36.000000 dingman-openapi-server-dev-1.0.1/openapi_server/typing_utils.py
+-rw-r--r--   0 jialening   (501) staff       (20)     3533 2023-07-14 22:07:36.000000 dingman-openapi-server-dev-1.0.1/openapi_server/util.py
+-rw-r--r--   0 jialening   (501) staff       (20)        7 2023-07-31 06:45:53.000000 dingman-openapi-server-dev-1.0.1/openapi_version
+-rw-r--r--   0 jialening   (501) staff       (20)       38 2023-07-31 21:05:06.185337 dingman-openapi-server-dev-1.0.1/setup.cfg
+-rw-r--r--   0 jialening   (501) staff       (20)      903 2023-07-31 06:42:45.000000 dingman-openapi-server-dev-1.0.1/setup.py
+-rw-r--r--   0 jialening   (501) staff       (20)     1286 2023-07-31 21:05:01.000000 dingman-openapi-server-dev-1.0.1/update_dev_pkg.py
```

### Comparing `dingman-openapi-server-dev-1.0.0/README.md` & `dingman-openapi-server-dev-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/dingman_openapi_server_dev.egg-info/SOURCES.txt` & `dingman-openapi-server-dev-1.0.1/dingman_openapi_server_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/.DS_Store` & `dingman-openapi-server-dev-1.0.1/openapi_server/.DS_Store`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/controllers/deploy_resources_controller.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/controllers/deploy_resources_controller.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/controllers/security_controller_.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/controllers/security_controller_.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/encoder.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/encoder.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/__init__.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/affinity.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/affinity.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/base_model_.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/base_model_.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/config.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/config.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/config_templates_inner.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/config_templates_inner.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/container.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/container.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/container_life_cycle.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/container_life_cycle.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/container_port.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/container_port.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/container_sec_context.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/container_sec_context.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/container_sec_context_capabilities.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/container_sec_context_capabilities.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/deploy_platform_resource.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/deploy_platform_resource.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/deploy_resources.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/deploy_resources.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/dingman_error.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/dingman_error.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/dingman_response.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/dingman_response.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/endpoint.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/endpoint.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/env_from_source.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/env_from_source.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/env_var.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/env_var.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/env_var_source.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/env_var_source.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/http_get.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/http_get.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/http_ingress_path.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/http_ingress_path.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/ingress.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/ingress.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/ingress_backend.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/ingress_backend.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/ingress_backend_service.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/ingress_backend_service.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/ingress_rule.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/ingress_rule.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/ingress_tls.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/ingress_tls.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/life_cycle_handler.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/life_cycle_handler.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/node_affinity.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/node_affinity.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/node_selector.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/node_selector.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/node_selector_term.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/node_selector_term.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/object_field_selector.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/object_field_selector.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/persistent_volume_claim.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/pod.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/pod.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/pod_affinity.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/pod_affinity.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/pod_affinity_term.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/pod_affinity_term.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/pod_anti_affinity.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/pod_anti_affinity.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/pod_sec_context.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/pod_sec_context.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/preferred_scheduling_term.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/preferred_scheduling_term.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/probe.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/probe.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/rbac_role_ref.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/rbac_role_ref.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/rbac_rule.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/rbac_rule.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/ref_volume_source.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/ref_volume_source.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/relabel_config.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/relabel_config.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/resource_requirements.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/resource_requirements.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/role.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/role.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/role_binding.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/role_binding.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/role_binding_subject.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/role_binding_subject.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/secret.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/secret.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/service.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/service.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/service_monitor.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/service_monitor.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/service_monitor_namespace_selector.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/service_monitor_namespace_selector.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/service_port.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/service_port.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/sysctl.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/sysctl.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/tcp_socket.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/tcp_socket.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/topology_spread_constraint.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/topology_spread_constraint.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/update_strategy.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/update_strategy.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/update_strategy_rolling_update_config.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/update_strategy_rolling_update_config.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/volume.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/volume.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/volume_device.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/volume_device.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/volume_empty_dir.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/volume_empty_dir.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/volume_host_path.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/volume_host_path.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/volume_mount.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/volume_mount.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/volume_persistent_volume_claim.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/volume_persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/weighted_pod_affinity_term.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/weighted_pod_affinity_term.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/models/workload.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/models/workload.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/openapi/openapi.yaml` & `dingman-openapi-server-dev-1.0.1/openapi_server/openapi/openapi.yaml`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/test/test_deploy_resources_controller.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/test/test_deploy_resources_controller.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/typing_utils.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/typing_utils.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/openapi_server/util.py` & `dingman-openapi-server-dev-1.0.1/openapi_server/util.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/setup.py` & `dingman-openapi-server-dev-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.0/update_dev_pkg.py` & `dingman-openapi-server-dev-1.0.1/update_dev_pkg.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import requests
 import setuptools
 import sys, os
 dev_pkg_name = "dingman-openapi-server-dev"
-# data = requests.get(f"https://pypi.org/pypi/{dev_pkg_name}/json").json()
-# latest_version = [1, 0, 0]
-# for version in data["releases"]:
-#     version_lst = [int(num) for num in version.split(".")]
-#     if version_lst > latest_version:
-#         latest_version = version_lst
-# new_version = latest_version
-# new_version[2] += 1
-# new_version = [str(num) for num in new_version]
-# new_version = ".".join(new_version)
-new_version = "1.0.0"
+data = requests.get(f"https://pypi.org/pypi/{dev_pkg_name}/json").json()
+latest_version = [1, 0, 0]
+for version in data["releases"]:
+    version_lst = [int(num) for num in version.split(".")]
+    if version_lst > latest_version:
+        latest_version = version_lst
+new_version = latest_version
+new_version[2] += 1
+new_version = [str(num) for num in new_version]
+new_version = ".".join(new_version)
 openapi_modules = setuptools.find_packages("openapi_server")
 # provide full path for the modules
 openapi_modules = ["openapi_server." + module for module in openapi_modules]
 openapi_modules.append("openapi_server")
 # to protect the version number printed as the program output
 sys.stdout = open(os.devnull, 'w')
 setuptools.setup(
```

