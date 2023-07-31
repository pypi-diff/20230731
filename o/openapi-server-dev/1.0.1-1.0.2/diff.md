# Comparing `tmp/openapi-server-dev-1.0.1.tar.gz` & `tmp/openapi-server-dev-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openapi-server-dev-1.0.1.tar", last modified: Mon Jul 31 06:35:50 2023, max compression
+gzip compressed data, was "dist/openapi-server-dev-1.0.2.tar", last modified: Mon Jul 31 06:49:36 2023, max compression
```

## Comparing `openapi-server-dev-1.0.1.tar` & `openapi-server-dev-1.0.2.tar`

### file list

```diff
@@ -1,95 +1,94 @@
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-31 06:35:50.260121 openapi-server-dev-1.0.1/
--rw-r--r--   0 jialening   (501) staff       (20)       44 2023-07-14 22:13:36.000000 openapi-server-dev-1.0.1/MANIFEST.in
--rw-r--r--   0 jialening   (501) staff       (20)      322 2023-07-31 06:35:50.259852 openapi-server-dev-1.0.1/PKG-INFO
--rw-r--r--   0 jialening   (501) staff       (20)      902 2023-07-18 18:22:05.000000 openapi-server-dev-1.0.1/README.md
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-31 06:35:50.224904 openapi-server-dev-1.0.1/openapi_server/
--rw-r--r--   0 jialening   (501) staff       (20)     6148 2023-07-14 22:13:36.000000 openapi-server-dev-1.0.1/openapi_server/.DS_Store
--rw-r--r--   0 jialening   (501) staff       (20)        0 2023-07-14 22:07:36.000000 openapi-server-dev-1.0.1/openapi_server/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)      393 2023-07-14 22:07:36.000000 openapi-server-dev-1.0.1/openapi_server/__main__.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-31 06:35:50.226639 openapi-server-dev-1.0.1/openapi_server/controllers/
--rw-r--r--   0 jialening   (501) staff       (20)        0 2023-07-14 22:07:36.000000 openapi-server-dev-1.0.1/openapi_server/controllers/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)     5687 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/controllers/deploy_resources_controller.py
--rw-r--r--   0 jialening   (501) staff       (20)      552 2023-07-14 22:07:36.000000 openapi-server-dev-1.0.1/openapi_server/controllers/security_controller_.py
--rw-r--r--   0 jialening   (501) staff       (20)      608 2023-07-14 22:07:36.000000 openapi-server-dev-1.0.1/openapi_server/encoder.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-31 06:35:50.255120 openapi-server-dev-1.0.1/openapi_server/models/
--rw-r--r--   0 jialening   (501) staff       (20)     4146 2023-07-25 23:32:32.000000 openapi-server-dev-1.0.1/openapi_server/models/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)     3753 2023-07-14 22:07:34.000000 openapi-server-dev-1.0.1/openapi_server/models/affinity.py
--rw-r--r--   0 jialening   (501) staff       (20)     1913 2023-07-14 22:07:36.000000 openapi-server-dev-1.0.1/openapi_server/models/base_model_.py
--rw-r--r--   0 jialening   (501) staff       (20)     4907 2023-07-14 22:07:34.000000 openapi-server-dev-1.0.1/openapi_server/models/config.py
--rw-r--r--   0 jialening   (501) staff       (20)     2503 2023-07-14 22:07:34.000000 openapi-server-dev-1.0.1/openapi_server/models/config_templates_inner.py
--rw-r--r--   0 jialening   (501) staff       (20)    16535 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/container.py
--rw-r--r--   0 jialening   (501) staff       (20)     2639 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/container_life_cycle.py
--rw-r--r--   0 jialening   (501) staff       (20)     3654 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/container_port.py
--rw-r--r--   0 jialening   (501) staff       (20)     3936 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/container_sec_context.py
--rw-r--r--   0 jialening   (501) staff       (20)     2568 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/container_sec_context_capabilities.py
--rw-r--r--   0 jialening   (501) staff       (20)    10247 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/deploy_platform_resource.py
--rw-r--r--   0 jialening   (501) staff       (20)     9794 2023-07-25 23:32:32.000000 openapi-server-dev-1.0.1/openapi_server/models/deploy_resources.py
--rw-r--r--   0 jialening   (501) staff       (20)     3963 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/dingman_error.py
--rw-r--r--   0 jialening   (501) staff       (20)     2425 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/dingman_response.py
--rw-r--r--   0 jialening   (501) staff       (20)    10477 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/endpoint.py
--rw-r--r--   0 jialening   (501) staff       (20)     3192 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/env_from_source.py
--rw-r--r--   0 jialening   (501) staff       (20)     2961 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/env_var.py
--rw-r--r--   0 jialening   (501) staff       (20)     1827 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/env_var_source.py
--rw-r--r--   0 jialening   (501) staff       (20)     4682 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/http_get.py
--rw-r--r--   0 jialening   (501) staff       (20)     4413 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/http_ingress_path.py
--rw-r--r--   0 jialening   (501) staff       (20)     5643 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/ingress.py
--rw-r--r--   0 jialening   (501) staff       (20)     1821 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/ingress_backend.py
--rw-r--r--   0 jialening   (501) staff       (20)     2446 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/ingress_backend_service.py
--rw-r--r--   0 jialening   (501) staff       (20)     3082 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/ingress_rule.py
--rw-r--r--   0 jialening   (501) staff       (20)     3211 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/ingress_tls.py
--rw-r--r--   0 jialening   (501) staff       (20)     3561 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/life_cycle_handler.py
--rw-r--r--   0 jialening   (501) staff       (20)     4613 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/node_affinity.py
--rw-r--r--   0 jialening   (501) staff       (20)     2047 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/node_selector.py
--rw-r--r--   0 jialening   (501) staff       (20)     3199 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/node_selector_term.py
--rw-r--r--   0 jialening   (501) staff       (20)     2827 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/object_field_selector.py
--rw-r--r--   0 jialening   (501) staff       (20)     9740 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/persistent_volume_claim.py
--rw-r--r--   0 jialening   (501) staff       (20)    12357 2023-07-20 23:40:33.000000 openapi-server-dev-1.0.1/openapi_server/models/pod.py
--rw-r--r--   0 jialening   (501) staff       (20)     4649 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/pod_affinity.py
--rw-r--r--   0 jialening   (501) staff       (20)     3664 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/pod_affinity_term.py
--rw-r--r--   0 jialening   (501) staff       (20)     4713 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/pod_anti_affinity.py
--rw-r--r--   0 jialening   (501) staff       (20)     3682 2023-07-14 22:13:36.000000 openapi-server-dev-1.0.1/openapi_server/models/pod_sec_context.py
--rw-r--r--   0 jialening   (501) staff       (20)     2623 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/preferred_scheduling_term.py
--rw-r--r--   0 jialening   (501) staff       (20)     7480 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/probe.py
--rw-r--r--   0 jialening   (501) staff       (20)     3138 2023-07-20 23:38:35.000000 openapi-server-dev-1.0.1/openapi_server/models/rbac_role_ref.py
--rw-r--r--   0 jialening   (501) staff       (20)     3577 2023-07-20 23:38:35.000000 openapi-server-dev-1.0.1/openapi_server/models/rbac_rule.py
--rw-r--r--   0 jialening   (501) staff       (20)     3598 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/ref_volume_source.py
--rw-r--r--   0 jialening   (501) staff       (20)     6245 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/relabel_config.py
--rw-r--r--   0 jialening   (501) staff       (20)     2787 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/resource_requirements.py
--rw-r--r--   0 jialening   (501) staff       (20)     4812 2023-07-20 23:38:35.000000 openapi-server-dev-1.0.1/openapi_server/models/role.py
--rw-r--r--   0 jialening   (501) staff       (20)     6130 2023-07-20 23:38:35.000000 openapi-server-dev-1.0.1/openapi_server/models/role_binding.py
--rw-r--r--   0 jialening   (501) staff       (20)     2365 2023-07-20 23:38:35.000000 openapi-server-dev-1.0.1/openapi_server/models/role_binding_subject.py
--rw-r--r--   0 jialening   (501) staff       (20)     4141 2023-07-25 23:32:32.000000 openapi-server-dev-1.0.1/openapi_server/models/secret.py
--rw-r--r--   0 jialening   (501) staff       (20)     8819 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/service.py
--rw-r--r--   0 jialening   (501) staff       (20)     7583 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/service_monitor.py
--rw-r--r--   0 jialening   (501) staff       (20)     3055 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/service_monitor_namespace_selector.py
--rw-r--r--   0 jialening   (501) staff       (20)     5386 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/service_port.py
--rw-r--r--   0 jialening   (501) staff       (20)     2189 2023-07-14 22:13:36.000000 openapi-server-dev-1.0.1/openapi_server/models/sysctl.py
--rw-r--r--   0 jialening   (501) staff       (20)     2413 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/tcp_socket.py
--rw-r--r--   0 jialening   (501) staff       (20)     5905 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/topology_spread_constraint.py
--rw-r--r--   0 jialening   (501) staff       (20)     3521 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/update_strategy.py
--rw-r--r--   0 jialening   (501) staff       (20)     4965 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/update_strategy_rolling_update_config.py
--rw-r--r--   0 jialening   (501) staff       (20)     6189 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/volume.py
--rw-r--r--   0 jialening   (501) staff       (20)     3553 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/volume_device.py
--rw-r--r--   0 jialening   (501) staff       (20)     2767 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/volume_empty_dir.py
--rw-r--r--   0 jialening   (501) staff       (20)     2585 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/volume_host_path.py
--rw-r--r--   0 jialening   (501) staff       (20)     4139 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/volume_mount.py
--rw-r--r--   0 jialening   (501) staff       (20)     2938 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/volume_persistent_volume_claim.py
--rw-r--r--   0 jialening   (501) staff       (20)     2769 2023-07-14 22:07:35.000000 openapi-server-dev-1.0.1/openapi_server/models/weighted_pod_affinity_term.py
--rw-r--r--   0 jialening   (501) staff       (20)    13077 2023-07-20 23:40:33.000000 openapi-server-dev-1.0.1/openapi_server/models/workload.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-31 06:35:50.255427 openapi-server-dev-1.0.1/openapi_server/openapi/
--rw-r--r--   0 jialening   (501) staff       (20)   186818 2023-07-25 23:32:32.000000 openapi-server-dev-1.0.1/openapi_server/openapi/openapi.yaml
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-31 06:35:50.257065 openapi-server-dev-1.0.1/openapi_server/test/
--rw-r--r--   0 jialening   (501) staff       (20)      437 2023-07-14 22:07:36.000000 openapi-server-dev-1.0.1/openapi_server/test/__init__.py
--rw-r--r--   0 jialening   (501) staff       (20)   138979 2023-07-25 23:32:32.000000 openapi-server-dev-1.0.1/openapi_server/test/test_deploy_resources_controller.py
--rw-r--r--   0 jialening   (501) staff       (20)      809 2023-07-14 22:07:36.000000 openapi-server-dev-1.0.1/openapi_server/typing_utils.py
--rw-r--r--   0 jialening   (501) staff       (20)     3533 2023-07-14 22:07:36.000000 openapi-server-dev-1.0.1/openapi_server/util.py
-drwxr-xr-x   0 jialening   (501) staff       (20)        0 2023-07-31 06:35:50.259402 openapi-server-dev-1.0.1/openapi_server_dev.egg-info/
--rw-r--r--   0 jialening   (501) staff       (20)      322 2023-07-31 06:35:50.000000 openapi-server-dev-1.0.1/openapi_server_dev.egg-info/PKG-INFO
--rw-r--r--   0 jialening   (501) staff       (20)     3332 2023-07-31 06:35:50.000000 openapi-server-dev-1.0.1/openapi_server_dev.egg-info/SOURCES.txt
--rw-r--r--   0 jialening   (501) staff       (20)        1 2023-07-31 06:35:50.000000 openapi-server-dev-1.0.1/openapi_server_dev.egg-info/dependency_links.txt
--rw-r--r--   0 jialening   (501) staff       (20)       20 2023-07-31 06:35:50.000000 openapi-server-dev-1.0.1/openapi_server_dev.egg-info/requires.txt
--rw-r--r--   0 jialening   (501) staff       (20)       15 2023-07-31 06:35:50.000000 openapi-server-dev-1.0.1/openapi_server_dev.egg-info/top_level.txt
--rw-r--r--   0 jialening   (501) staff       (20)        6 2023-07-31 06:27:58.000000 openapi-server-dev-1.0.1/openapi_version
--rw-r--r--   0 jialening   (501) staff       (20)       38 2023-07-31 06:35:50.260227 openapi-server-dev-1.0.1/setup.cfg
--rw-r--r--   0 jialening   (501) staff       (20)      903 2023-07-31 06:27:06.000000 openapi-server-dev-1.0.1/setup.py
--rw-r--r--   0 jialening   (501) staff       (20)     1278 2023-07-31 06:35:46.000000 openapi-server-dev-1.0.1/update_dev_pkg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 06:49:36.000000 openapi-server-dev-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      266 2023-07-31 06:49:36.000000 openapi-server-dev-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      902 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 06:49:36.000000 openapi-server-dev-1.0.2/openapi_server/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      393 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 06:49:36.000000 openapi-server-dev-1.0.2/openapi_server/controllers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5687 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/controllers/deploy_resources_controller.py
+-rw-r--r--   0 root         (0) root         (0)      552 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/controllers/security_controller_.py
+-rw-r--r--   0 root         (0) root         (0)      608 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/encoder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 06:49:36.000000 openapi-server-dev-1.0.2/openapi_server/models/
+-rw-r--r--   0 root         (0) root         (0)     4146 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3753 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/affinity.py
+-rw-r--r--   0 root         (0) root         (0)     1913 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/base_model_.py
+-rw-r--r--   0 root         (0) root         (0)     4907 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/config.py
+-rw-r--r--   0 root         (0) root         (0)     2503 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/config_templates_inner.py
+-rw-r--r--   0 root         (0) root         (0)    16535 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/container.py
+-rw-r--r--   0 root         (0) root         (0)     2639 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/container_life_cycle.py
+-rw-r--r--   0 root         (0) root         (0)     3654 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/container_port.py
+-rw-r--r--   0 root         (0) root         (0)     3936 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/container_sec_context.py
+-rw-r--r--   0 root         (0) root         (0)     2568 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/container_sec_context_capabilities.py
+-rw-r--r--   0 root         (0) root         (0)    10247 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/deploy_platform_resource.py
+-rw-r--r--   0 root         (0) root         (0)     9794 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/deploy_resources.py
+-rw-r--r--   0 root         (0) root         (0)     3963 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/dingman_error.py
+-rw-r--r--   0 root         (0) root         (0)     2425 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/dingman_response.py
+-rw-r--r--   0 root         (0) root         (0)    10477 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/endpoint.py
+-rw-r--r--   0 root         (0) root         (0)     3192 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/env_from_source.py
+-rw-r--r--   0 root         (0) root         (0)     2961 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/env_var.py
+-rw-r--r--   0 root         (0) root         (0)     1827 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/env_var_source.py
+-rw-r--r--   0 root         (0) root         (0)     4682 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/http_get.py
+-rw-r--r--   0 root         (0) root         (0)     4413 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/http_ingress_path.py
+-rw-r--r--   0 root         (0) root         (0)     5643 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/ingress.py
+-rw-r--r--   0 root         (0) root         (0)     1821 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/ingress_backend.py
+-rw-r--r--   0 root         (0) root         (0)     2446 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/ingress_backend_service.py
+-rw-r--r--   0 root         (0) root         (0)     3082 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/ingress_rule.py
+-rw-r--r--   0 root         (0) root         (0)     3211 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/ingress_tls.py
+-rw-r--r--   0 root         (0) root         (0)     3561 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/life_cycle_handler.py
+-rw-r--r--   0 root         (0) root         (0)     4613 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/node_affinity.py
+-rw-r--r--   0 root         (0) root         (0)     2047 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/node_selector.py
+-rw-r--r--   0 root         (0) root         (0)     3199 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/node_selector_term.py
+-rw-r--r--   0 root         (0) root         (0)     2827 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/object_field_selector.py
+-rw-r--r--   0 root         (0) root         (0)     9740 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/persistent_volume_claim.py
+-rw-r--r--   0 root         (0) root         (0)    12357 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/pod.py
+-rw-r--r--   0 root         (0) root         (0)     4649 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/pod_affinity.py
+-rw-r--r--   0 root         (0) root         (0)     3664 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/pod_affinity_term.py
+-rw-r--r--   0 root         (0) root         (0)     4713 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/pod_anti_affinity.py
+-rw-r--r--   0 root         (0) root         (0)     3682 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/pod_sec_context.py
+-rw-r--r--   0 root         (0) root         (0)     2623 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/preferred_scheduling_term.py
+-rw-r--r--   0 root         (0) root         (0)     7480 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/probe.py
+-rw-r--r--   0 root         (0) root         (0)     3138 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/rbac_role_ref.py
+-rw-r--r--   0 root         (0) root         (0)     3577 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/rbac_rule.py
+-rw-r--r--   0 root         (0) root         (0)     3598 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/ref_volume_source.py
+-rw-r--r--   0 root         (0) root         (0)     6245 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/relabel_config.py
+-rw-r--r--   0 root         (0) root         (0)     2787 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/resource_requirements.py
+-rw-r--r--   0 root         (0) root         (0)     4812 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/role.py
+-rw-r--r--   0 root         (0) root         (0)     6130 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/role_binding.py
+-rw-r--r--   0 root         (0) root         (0)     2365 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/role_binding_subject.py
+-rw-r--r--   0 root         (0) root         (0)     4141 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/secret.py
+-rw-r--r--   0 root         (0) root         (0)     8819 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/service.py
+-rw-r--r--   0 root         (0) root         (0)     7583 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/service_monitor.py
+-rw-r--r--   0 root         (0) root         (0)     3055 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/service_monitor_namespace_selector.py
+-rw-r--r--   0 root         (0) root         (0)     5386 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/service_port.py
+-rw-r--r--   0 root         (0) root         (0)     2189 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/sysctl.py
+-rw-r--r--   0 root         (0) root         (0)     2413 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/tcp_socket.py
+-rw-r--r--   0 root         (0) root         (0)     5905 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/topology_spread_constraint.py
+-rw-r--r--   0 root         (0) root         (0)     3521 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/update_strategy.py
+-rw-r--r--   0 root         (0) root         (0)     4965 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/update_strategy_rolling_update_config.py
+-rw-r--r--   0 root         (0) root         (0)     6189 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/volume.py
+-rw-r--r--   0 root         (0) root         (0)     3553 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/volume_device.py
+-rw-r--r--   0 root         (0) root         (0)     2767 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/volume_empty_dir.py
+-rw-r--r--   0 root         (0) root         (0)     2585 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/volume_host_path.py
+-rw-r--r--   0 root         (0) root         (0)     4139 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/volume_mount.py
+-rw-r--r--   0 root         (0) root         (0)     2938 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/volume_persistent_volume_claim.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/weighted_pod_affinity_term.py
+-rw-r--r--   0 root         (0) root         (0)    13077 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/models/workload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 06:49:36.000000 openapi-server-dev-1.0.2/openapi_server/openapi/
+-rw-r--r--   0 root         (0) root         (0)   186818 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/openapi/openapi.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 06:49:36.000000 openapi-server-dev-1.0.2/openapi_server/test/
+-rw-r--r--   0 root         (0) root         (0)      437 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   138979 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/test/test_deploy_resources_controller.py
+-rw-r--r--   0 root         (0) root         (0)      809 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/typing_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3533 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_server/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 06:49:36.000000 openapi-server-dev-1.0.2/openapi_server_dev.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      266 2023-07-31 06:49:36.000000 openapi-server-dev-1.0.2/openapi_server_dev.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3307 2023-07-31 06:49:36.000000 openapi-server-dev-1.0.2/openapi_server_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 06:49:36.000000 openapi-server-dev-1.0.2/openapi_server_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-31 06:49:36.000000 openapi-server-dev-1.0.2/openapi_server_dev.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-31 06:49:36.000000 openapi-server-dev-1.0.2/openapi_server_dev.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/openapi_version
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 06:49:36.000000 openapi-server-dev-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      903 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-07-31 06:49:28.000000 openapi-server-dev-1.0.2/update_dev_pkg.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `openapi-server-dev-1.0.1/README.md` & `openapi-server-dev-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/controllers/deploy_resources_controller.py` & `openapi-server-dev-1.0.2/openapi_server/controllers/deploy_resources_controller.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/controllers/security_controller_.py` & `openapi-server-dev-1.0.2/openapi_server/controllers/security_controller_.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/encoder.py` & `openapi-server-dev-1.0.2/openapi_server/encoder.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/__init__.py` & `openapi-server-dev-1.0.2/openapi_server/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/affinity.py` & `openapi-server-dev-1.0.2/openapi_server/models/affinity.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/base_model_.py` & `openapi-server-dev-1.0.2/openapi_server/models/base_model_.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/config.py` & `openapi-server-dev-1.0.2/openapi_server/models/config.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/config_templates_inner.py` & `openapi-server-dev-1.0.2/openapi_server/models/config_templates_inner.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/container.py` & `openapi-server-dev-1.0.2/openapi_server/models/container.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/container_life_cycle.py` & `openapi-server-dev-1.0.2/openapi_server/models/container_life_cycle.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/container_port.py` & `openapi-server-dev-1.0.2/openapi_server/models/container_port.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/container_sec_context.py` & `openapi-server-dev-1.0.2/openapi_server/models/container_sec_context.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/container_sec_context_capabilities.py` & `openapi-server-dev-1.0.2/openapi_server/models/container_sec_context_capabilities.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/deploy_platform_resource.py` & `openapi-server-dev-1.0.2/openapi_server/models/deploy_platform_resource.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/deploy_resources.py` & `openapi-server-dev-1.0.2/openapi_server/models/deploy_resources.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/dingman_error.py` & `openapi-server-dev-1.0.2/openapi_server/models/dingman_error.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/dingman_response.py` & `openapi-server-dev-1.0.2/openapi_server/models/dingman_response.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/endpoint.py` & `openapi-server-dev-1.0.2/openapi_server/models/endpoint.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/env_from_source.py` & `openapi-server-dev-1.0.2/openapi_server/models/env_from_source.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/env_var.py` & `openapi-server-dev-1.0.2/openapi_server/models/env_var.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/env_var_source.py` & `openapi-server-dev-1.0.2/openapi_server/models/env_var_source.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/http_get.py` & `openapi-server-dev-1.0.2/openapi_server/models/http_get.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/http_ingress_path.py` & `openapi-server-dev-1.0.2/openapi_server/models/http_ingress_path.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/ingress.py` & `openapi-server-dev-1.0.2/openapi_server/models/ingress.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/ingress_backend.py` & `openapi-server-dev-1.0.2/openapi_server/models/ingress_backend.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/ingress_backend_service.py` & `openapi-server-dev-1.0.2/openapi_server/models/ingress_backend_service.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/ingress_rule.py` & `openapi-server-dev-1.0.2/openapi_server/models/ingress_rule.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/ingress_tls.py` & `openapi-server-dev-1.0.2/openapi_server/models/ingress_tls.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/life_cycle_handler.py` & `openapi-server-dev-1.0.2/openapi_server/models/life_cycle_handler.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/node_affinity.py` & `openapi-server-dev-1.0.2/openapi_server/models/node_affinity.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/node_selector.py` & `openapi-server-dev-1.0.2/openapi_server/models/node_selector.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/node_selector_term.py` & `openapi-server-dev-1.0.2/openapi_server/models/node_selector_term.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/object_field_selector.py` & `openapi-server-dev-1.0.2/openapi_server/models/object_field_selector.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/persistent_volume_claim.py` & `openapi-server-dev-1.0.2/openapi_server/models/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/pod.py` & `openapi-server-dev-1.0.2/openapi_server/models/pod.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/pod_affinity.py` & `openapi-server-dev-1.0.2/openapi_server/models/pod_affinity.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/pod_affinity_term.py` & `openapi-server-dev-1.0.2/openapi_server/models/pod_affinity_term.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/pod_anti_affinity.py` & `openapi-server-dev-1.0.2/openapi_server/models/pod_anti_affinity.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/pod_sec_context.py` & `openapi-server-dev-1.0.2/openapi_server/models/pod_sec_context.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/preferred_scheduling_term.py` & `openapi-server-dev-1.0.2/openapi_server/models/preferred_scheduling_term.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/probe.py` & `openapi-server-dev-1.0.2/openapi_server/models/probe.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/rbac_role_ref.py` & `openapi-server-dev-1.0.2/openapi_server/models/rbac_role_ref.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/rbac_rule.py` & `openapi-server-dev-1.0.2/openapi_server/models/rbac_rule.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/ref_volume_source.py` & `openapi-server-dev-1.0.2/openapi_server/models/ref_volume_source.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/relabel_config.py` & `openapi-server-dev-1.0.2/openapi_server/models/relabel_config.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/resource_requirements.py` & `openapi-server-dev-1.0.2/openapi_server/models/resource_requirements.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/role.py` & `openapi-server-dev-1.0.2/openapi_server/models/role.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/role_binding.py` & `openapi-server-dev-1.0.2/openapi_server/models/role_binding.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/role_binding_subject.py` & `openapi-server-dev-1.0.2/openapi_server/models/role_binding_subject.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/secret.py` & `openapi-server-dev-1.0.2/openapi_server/models/secret.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/service.py` & `openapi-server-dev-1.0.2/openapi_server/models/service.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/service_monitor.py` & `openapi-server-dev-1.0.2/openapi_server/models/service_monitor.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/service_monitor_namespace_selector.py` & `openapi-server-dev-1.0.2/openapi_server/models/service_monitor_namespace_selector.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/service_port.py` & `openapi-server-dev-1.0.2/openapi_server/models/service_port.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/sysctl.py` & `openapi-server-dev-1.0.2/openapi_server/models/sysctl.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/tcp_socket.py` & `openapi-server-dev-1.0.2/openapi_server/models/tcp_socket.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/topology_spread_constraint.py` & `openapi-server-dev-1.0.2/openapi_server/models/topology_spread_constraint.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/update_strategy.py` & `openapi-server-dev-1.0.2/openapi_server/models/update_strategy.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/update_strategy_rolling_update_config.py` & `openapi-server-dev-1.0.2/openapi_server/models/update_strategy_rolling_update_config.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/volume.py` & `openapi-server-dev-1.0.2/openapi_server/models/volume.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/volume_device.py` & `openapi-server-dev-1.0.2/openapi_server/models/volume_device.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/volume_empty_dir.py` & `openapi-server-dev-1.0.2/openapi_server/models/volume_empty_dir.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/volume_host_path.py` & `openapi-server-dev-1.0.2/openapi_server/models/volume_host_path.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/volume_mount.py` & `openapi-server-dev-1.0.2/openapi_server/models/volume_mount.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/volume_persistent_volume_claim.py` & `openapi-server-dev-1.0.2/openapi_server/models/volume_persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/weighted_pod_affinity_term.py` & `openapi-server-dev-1.0.2/openapi_server/models/weighted_pod_affinity_term.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/models/workload.py` & `openapi-server-dev-1.0.2/openapi_server/models/workload.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/openapi/openapi.yaml` & `openapi-server-dev-1.0.2/openapi_server/openapi/openapi.yaml`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/test/test_deploy_resources_controller.py` & `openapi-server-dev-1.0.2/openapi_server/test/test_deploy_resources_controller.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/typing_utils.py` & `openapi-server-dev-1.0.2/openapi_server/typing_utils.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server/util.py` & `openapi-server-dev-1.0.2/openapi_server/util.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/openapi_server_dev.egg-info/SOURCES.txt` & `openapi-server-dev-1.0.2/openapi_server_dev.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 MANIFEST.in
 README.md
 openapi_version
 setup.py
 update_dev_pkg.py
-openapi_server/.DS_Store
 openapi_server/__init__.py
 openapi_server/__main__.py
 openapi_server/encoder.py
 openapi_server/typing_utils.py
 openapi_server/util.py
 openapi_server/controllers/__init__.py
 openapi_server/controllers/deploy_resources_controller.py
```

### Comparing `openapi-server-dev-1.0.1/setup.py` & `openapi-server-dev-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `openapi-server-dev-1.0.1/update_dev_pkg.py` & `openapi-server-dev-1.0.2/update_dev_pkg.py`

 * *Files identical despite different names*

