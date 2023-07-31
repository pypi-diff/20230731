# Comparing `tmp/pierskarsenbarg_pulumi_sdm-1.3.0.tar.gz` & `tmp/pierskarsenbarg_pulumi_sdm-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pierskarsenbarg_pulumi_sdm-1.3.0.tar", last modified: Tue Jul 18 13:47:17 2023, max compression
+gzip compressed data, was "dist/pierskarsenbarg_pulumi_sdm-1.4.0.tar", last modified: Mon Jul 31 20:32:42 2023, max compression
```

## Comparing `pierskarsenbarg_pulumi_sdm-1.3.0.tar` & `pierskarsenbarg_pulumi_sdm-1.4.0.tar`

### file list

```diff
@@ -1,39 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:47:17.000000 pierskarsenbarg_pulumi_sdm-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-18 13:47:17.000000 pierskarsenbarg_pulumi_sdm-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:47:17.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   756526 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/account_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:47:17.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    10341 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/get_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/get_account_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/get_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/get_remote_identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/get_remote_identity_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/get_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/get_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/get_secret_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/get_ssh_ca_pubkey.py
--rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/node.py
--rw-r--r--   0 runner    (1001) docker     (123)  1293623 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10592 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/remote_identity.py
--rw-r--r--   0 runner    (1001) docker     (123)   154776 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12954 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    23146 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/secret_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:47:17.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-18 13:47:17.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-18 13:47:17.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:47:17.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:47:17.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-18 13:47:17.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-18 13:47:17.000000 pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 13:47:17.000000 pierskarsenbarg_pulumi_sdm-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-18 13:47:16.000000 pierskarsenbarg_pulumi_sdm-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:32:42.000000 pierskarsenbarg_pulumi_sdm-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-31 20:32:42.000000 pierskarsenbarg_pulumi_sdm-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:32:42.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   755154 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/account_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:32:42.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10341 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_account_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_peering_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_peering_group_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_peering_group_peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_peering_group_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_remote_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_remote_identity_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_secret_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_ssh_ca_pubkey.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1296574 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/peering_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8025 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/peering_group_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/peering_group_peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8337 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/peering_group_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10592 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/remote_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)   154776 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12954 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23146 2023-07-31 20:32:41.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/secret_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:32:42.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-31 20:32:42.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-31 20:32:42.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 20:32:42.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 20:32:42.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-31 20:32:42.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-31 20:32:42.000000 pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 20:32:42.000000 pierskarsenbarg_pulumi_sdm-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-31 20:32:42.000000 pierskarsenbarg_pulumi_sdm-1.4.0/setup.py
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.3.0/PKG-INFO` & `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pierskarsenbarg_pulumi_sdm
-Version: 1.3.0
+Name: pierskarsenbarg-pulumi-sdm
+Version: 1.4.0
 Summary: A Pulumi package for creating and managing StrongDM cloud resources.
 Home-page: https://github.com/pierskarsenbarg/pulumi-sdm
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pierskarsenbarg/pulumi-sdm
 Description: # StrongDM Resource Provider
         
         The StrongDM Resource Provider lets you manage [StrongDM](http://strongdm.com) resources.
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.3.0/README.md` & `pierskarsenbarg_pulumi_sdm-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/_inputs.py` & `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -308,40 +308,36 @@
 
 
 @pulumi.input_type
 class NodeGatewayArgs:
     def __init__(__self__, *,
                  listen_address: pulumi.Input[str],
                  bind_address: Optional[pulumi.Input[str]] = None,
-                 connects_to: Optional[pulumi.Input[str]] = None,
                  device: Optional[pulumi.Input[str]] = None,
                  gateway_filter: Optional[pulumi.Input[str]] = None,
                  location: Optional[pulumi.Input[str]] = None,
                  maintenance_windows: Optional[pulumi.Input[Sequence[pulumi.Input['NodeGatewayMaintenanceWindowArgs']]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  token: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] listen_address: The public hostname/port tuple at which the gateway will be accessible to clients.
         :param pulumi.Input[str] bind_address: The hostname/port tuple which the gateway daemon will bind to. If not provided on create, set to "0.0.0.0:listen_address_port".
-        :param pulumi.Input[str] connects_to: ConnectsTo can be used to restrict the peering between relays and gateways.
         :param pulumi.Input[str] device: Device is a read only device name uploaded by the gateway process when it comes online.
         :param pulumi.Input[str] gateway_filter: GatewayFilter can be used to restrict the peering between relays and gateways. Deprecated.
         :param pulumi.Input[str] location: Location is a read only network location uploaded by the gateway process when it comes online.
         :param pulumi.Input[Sequence[pulumi.Input['NodeGatewayMaintenanceWindowArgs']]] maintenance_windows: Maintenance Windows define when this node is allowed to restart. If a node is requested to restart, it will check each window to determine if any of them permit it to restart, and if any do, it will. This check is repeated per window until the restart is successfully completed.  If not set here, may be set on the command line or via an environment variable on the process itself; any server setting will take precedence over local settings. This setting is ineffective for nodes below version 38.44.0.  If this setting is not applied via this remote configuration or via local configuration, the default setting is used: always allow restarts if serving no connections, and allow a restart even if serving connections between 7-8 UTC, any day.
         :param pulumi.Input[str] name: Unique human-readable name of the Relay. Node names must include only letters, numbers, and hyphens (no spaces, underscores, or other special characters). Generated if not provided on create.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         :param pulumi.Input[str] version: Version is a read only sdm binary version uploaded by the gateway process when it comes online.
         """
         pulumi.set(__self__, "listen_address", listen_address)
         if bind_address is not None:
             pulumi.set(__self__, "bind_address", bind_address)
-        if connects_to is not None:
-            pulumi.set(__self__, "connects_to", connects_to)
         if device is not None:
             pulumi.set(__self__, "device", device)
         if gateway_filter is not None:
             pulumi.set(__self__, "gateway_filter", gateway_filter)
         if location is not None:
             pulumi.set(__self__, "location", location)
         if maintenance_windows is not None:
@@ -376,26 +372,14 @@
         return pulumi.get(self, "bind_address")
 
     @bind_address.setter
     def bind_address(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "bind_address", value)
 
     @property
-    @pulumi.getter(name="connectsTo")
-    def connects_to(self) -> Optional[pulumi.Input[str]]:
-        """
-        ConnectsTo can be used to restrict the peering between relays and gateways.
-        """
-        return pulumi.get(self, "connects_to")
-
-    @connects_to.setter
-    def connects_to(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "connects_to", value)
-
-    @property
     @pulumi.getter
     def device(self) -> Optional[pulumi.Input[str]]:
         """
         Device is a read only device name uploaded by the gateway process when it comes online.
         """
         return pulumi.get(self, "device")
 
@@ -511,35 +495,31 @@
     def require_idleness(self, value: pulumi.Input[bool]):
         pulumi.set(self, "require_idleness", value)
 
 
 @pulumi.input_type
 class NodeRelayArgs:
     def __init__(__self__, *,
-                 connects_to: Optional[pulumi.Input[str]] = None,
                  device: Optional[pulumi.Input[str]] = None,
                  gateway_filter: Optional[pulumi.Input[str]] = None,
                  location: Optional[pulumi.Input[str]] = None,
                  maintenance_windows: Optional[pulumi.Input[Sequence[pulumi.Input['NodeRelayMaintenanceWindowArgs']]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  token: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] connects_to: ConnectsTo can be used to restrict the peering between relays and gateways.
         :param pulumi.Input[str] device: Device is a read only device name uploaded by the gateway process when it comes online.
         :param pulumi.Input[str] gateway_filter: GatewayFilter can be used to restrict the peering between relays and gateways. Deprecated.
         :param pulumi.Input[str] location: Location is a read only network location uploaded by the gateway process when it comes online.
         :param pulumi.Input[Sequence[pulumi.Input['NodeRelayMaintenanceWindowArgs']]] maintenance_windows: Maintenance Windows define when this node is allowed to restart. If a node is requested to restart, it will check each window to determine if any of them permit it to restart, and if any do, it will. This check is repeated per window until the restart is successfully completed.  If not set here, may be set on the command line or via an environment variable on the process itself; any server setting will take precedence over local settings. This setting is ineffective for nodes below version 38.44.0.  If this setting is not applied via this remote configuration or via local configuration, the default setting is used: always allow restarts if serving no connections, and allow a restart even if serving connections between 7-8 UTC, any day.
         :param pulumi.Input[str] name: Unique human-readable name of the Relay. Node names must include only letters, numbers, and hyphens (no spaces, underscores, or other special characters). Generated if not provided on create.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         :param pulumi.Input[str] version: Version is a read only sdm binary version uploaded by the gateway process when it comes online.
         """
-        if connects_to is not None:
-            pulumi.set(__self__, "connects_to", connects_to)
         if device is not None:
             pulumi.set(__self__, "device", device)
         if gateway_filter is not None:
             pulumi.set(__self__, "gateway_filter", gateway_filter)
         if location is not None:
             pulumi.set(__self__, "location", location)
         if maintenance_windows is not None:
@@ -550,26 +530,14 @@
             pulumi.set(__self__, "tags", tags)
         if token is not None:
             pulumi.set(__self__, "token", token)
         if version is not None:
             pulumi.set(__self__, "version", version)
 
     @property
-    @pulumi.getter(name="connectsTo")
-    def connects_to(self) -> Optional[pulumi.Input[str]]:
-        """
-        ConnectsTo can be used to restrict the peering between relays and gateways.
-        """
-        return pulumi.get(self, "connects_to")
-
-    @connects_to.setter
-    def connects_to(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "connects_to", value)
-
-    @property
     @pulumi.getter
     def device(self) -> Optional[pulumi.Input[str]]:
         """
         Device is a read only device name uploaded by the gateway process when it comes online.
         """
         return pulumi.get(self, "device")
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/_utilities.py` & `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/_utilities.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/account.py` & `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/account.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/account_attachment.py` & `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/account_attachment.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/config/vars.py` & `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/config/vars.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/get_account.py` & `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_account.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/get_account_attachment.py` & `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_account_attachment.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/get_node.py` & `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_node.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/get_remote_identity.py` & `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_remote_identity.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/get_remote_identity_group.py` & `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_remote_identity_group.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/get_resource.py` & `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_resource.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/get_role.py` & `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_role.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/get_secret_store.py` & `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_secret_store.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/get_ssh_ca_pubkey.py` & `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/get_ssh_ca_pubkey.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/node.py` & `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/node.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/outputs.py` & `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,14 +113,18 @@
     'GetAccountAccountUserResult',
     'GetAccountAttachmentAccountAttachmentResult',
     'GetNodeNodeResult',
     'GetNodeNodeGatewayResult',
     'GetNodeNodeGatewayMaintenanceWindowResult',
     'GetNodeNodeRelayResult',
     'GetNodeNodeRelayMaintenanceWindowResult',
+    'GetPeeringGroupNodePeeringGroupNodeResult',
+    'GetPeeringGroupPeerPeeringGroupPeerResult',
+    'GetPeeringGroupPeeringGroupResult',
+    'GetPeeringGroupResourcePeeringGroupResourceResult',
     'GetRemoteIdentityGroupRemoteIdentityGroupResult',
     'GetRemoteIdentityRemoteIdentityResult',
     'GetResourceResourceResult',
     'GetResourceResourceAkResult',
     'GetResourceResourceAksBasicAuthResult',
     'GetResourceResourceAksServiceAccountResult',
     'GetResourceResourceAksServiceAccountUserImpersonationResult',
@@ -395,16 +399,14 @@
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "listenAddress":
             suggest = "listen_address"
         elif key == "bindAddress":
             suggest = "bind_address"
-        elif key == "connectsTo":
-            suggest = "connects_to"
         elif key == "gatewayFilter":
             suggest = "gateway_filter"
         elif key == "maintenanceWindows":
             suggest = "maintenance_windows"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in NodeGateway. Access the value via the '{suggest}' property getter instead.")
@@ -416,40 +418,36 @@
     def get(self, key: str, default = None) -> Any:
         NodeGateway.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  listen_address: str,
                  bind_address: Optional[str] = None,
-                 connects_to: Optional[str] = None,
                  device: Optional[str] = None,
                  gateway_filter: Optional[str] = None,
                  location: Optional[str] = None,
                  maintenance_windows: Optional[Sequence['outputs.NodeGatewayMaintenanceWindow']] = None,
                  name: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  token: Optional[str] = None,
                  version: Optional[str] = None):
         """
         :param str listen_address: The public hostname/port tuple at which the gateway will be accessible to clients.
         :param str bind_address: The hostname/port tuple which the gateway daemon will bind to. If not provided on create, set to "0.0.0.0:listen_address_port".
-        :param str connects_to: ConnectsTo can be used to restrict the peering between relays and gateways.
         :param str device: Device is a read only device name uploaded by the gateway process when it comes online.
         :param str gateway_filter: GatewayFilter can be used to restrict the peering between relays and gateways. Deprecated.
         :param str location: Location is a read only network location uploaded by the gateway process when it comes online.
         :param Sequence['NodeGatewayMaintenanceWindowArgs'] maintenance_windows: Maintenance Windows define when this node is allowed to restart. If a node is requested to restart, it will check each window to determine if any of them permit it to restart, and if any do, it will. This check is repeated per window until the restart is successfully completed.  If not set here, may be set on the command line or via an environment variable on the process itself; any server setting will take precedence over local settings. This setting is ineffective for nodes below version 38.44.0.  If this setting is not applied via this remote configuration or via local configuration, the default setting is used: always allow restarts if serving no connections, and allow a restart even if serving connections between 7-8 UTC, any day.
         :param str name: Unique human-readable name of the Relay. Node names must include only letters, numbers, and hyphens (no spaces, underscores, or other special characters). Generated if not provided on create.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         :param str version: Version is a read only sdm binary version uploaded by the gateway process when it comes online.
         """
         pulumi.set(__self__, "listen_address", listen_address)
         if bind_address is not None:
             pulumi.set(__self__, "bind_address", bind_address)
-        if connects_to is not None:
-            pulumi.set(__self__, "connects_to", connects_to)
         if device is not None:
             pulumi.set(__self__, "device", device)
         if gateway_filter is not None:
             pulumi.set(__self__, "gateway_filter", gateway_filter)
         if location is not None:
             pulumi.set(__self__, "location", location)
         if maintenance_windows is not None:
@@ -476,22 +474,14 @@
     def bind_address(self) -> Optional[str]:
         """
         The hostname/port tuple which the gateway daemon will bind to. If not provided on create, set to "0.0.0.0:listen_address_port".
         """
         return pulumi.get(self, "bind_address")
 
     @property
-    @pulumi.getter(name="connectsTo")
-    def connects_to(self) -> Optional[str]:
-        """
-        ConnectsTo can be used to restrict the peering between relays and gateways.
-        """
-        return pulumi.get(self, "connects_to")
-
-    @property
     @pulumi.getter
     def device(self) -> Optional[str]:
         """
         Device is a read only device name uploaded by the gateway process when it comes online.
         """
         return pulumi.get(self, "device")
 
@@ -588,17 +578,15 @@
 
 
 @pulumi.output_type
 class NodeRelay(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
-        if key == "connectsTo":
-            suggest = "connects_to"
-        elif key == "gatewayFilter":
+        if key == "gatewayFilter":
             suggest = "gateway_filter"
         elif key == "maintenanceWindows":
             suggest = "maintenance_windows"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in NodeRelay. Access the value via the '{suggest}' property getter instead.")
 
@@ -607,35 +595,31 @@
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         NodeRelay.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
-                 connects_to: Optional[str] = None,
                  device: Optional[str] = None,
                  gateway_filter: Optional[str] = None,
                  location: Optional[str] = None,
                  maintenance_windows: Optional[Sequence['outputs.NodeRelayMaintenanceWindow']] = None,
                  name: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  token: Optional[str] = None,
                  version: Optional[str] = None):
         """
-        :param str connects_to: ConnectsTo can be used to restrict the peering between relays and gateways.
         :param str device: Device is a read only device name uploaded by the gateway process when it comes online.
         :param str gateway_filter: GatewayFilter can be used to restrict the peering between relays and gateways. Deprecated.
         :param str location: Location is a read only network location uploaded by the gateway process when it comes online.
         :param Sequence['NodeRelayMaintenanceWindowArgs'] maintenance_windows: Maintenance Windows define when this node is allowed to restart. If a node is requested to restart, it will check each window to determine if any of them permit it to restart, and if any do, it will. This check is repeated per window until the restart is successfully completed.  If not set here, may be set on the command line or via an environment variable on the process itself; any server setting will take precedence over local settings. This setting is ineffective for nodes below version 38.44.0.  If this setting is not applied via this remote configuration or via local configuration, the default setting is used: always allow restarts if serving no connections, and allow a restart even if serving connections between 7-8 UTC, any day.
         :param str name: Unique human-readable name of the Relay. Node names must include only letters, numbers, and hyphens (no spaces, underscores, or other special characters). Generated if not provided on create.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         :param str version: Version is a read only sdm binary version uploaded by the gateway process when it comes online.
         """
-        if connects_to is not None:
-            pulumi.set(__self__, "connects_to", connects_to)
         if device is not None:
             pulumi.set(__self__, "device", device)
         if gateway_filter is not None:
             pulumi.set(__self__, "gateway_filter", gateway_filter)
         if location is not None:
             pulumi.set(__self__, "location", location)
         if maintenance_windows is not None:
@@ -646,22 +630,14 @@
             pulumi.set(__self__, "tags", tags)
         if token is not None:
             pulumi.set(__self__, "token", token)
         if version is not None:
             pulumi.set(__self__, "version", version)
 
     @property
-    @pulumi.getter(name="connectsTo")
-    def connects_to(self) -> Optional[str]:
-        """
-        ConnectsTo can be used to restrict the peering between relays and gateways.
-        """
-        return pulumi.get(self, "connects_to")
-
-    @property
     @pulumi.getter
     def device(self) -> Optional[str]:
         """
         Device is a read only device name uploaded by the gateway process when it comes online.
         """
         return pulumi.get(self, "device")
 
@@ -16817,41 +16793,37 @@
 @pulumi.output_type
 class GetNodeNodeGatewayResult(dict):
     def __init__(__self__, *,
                  device: str,
                  location: str,
                  version: str,
                  bind_address: Optional[str] = None,
-                 connects_to: Optional[str] = None,
                  gateway_filter: Optional[str] = None,
                  id: Optional[str] = None,
                  listen_address: Optional[str] = None,
                  maintenance_windows: Optional[Sequence['outputs.GetNodeNodeGatewayMaintenanceWindowResult']] = None,
                  name: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str device: Device is a read only device name uploaded by the gateway process when it comes online.
         :param str location: Location is a read only network location uploaded by the gateway process when it comes online.
         :param str version: Version is a read only sdm binary version uploaded by the gateway process when it comes online.
         :param str bind_address: The hostname/port tuple which the gateway daemon will bind to. If not provided on create, set to "0.0.0.0:listen_address_port".
-        :param str connects_to: ConnectsTo can be used to restrict the peering between relays and gateways.
         :param str gateway_filter: GatewayFilter can be used to restrict the peering between relays and gateways. Deprecated.
         :param str id: Unique identifier of the Relay.
         :param str listen_address: The public hostname/port tuple at which the gateway will be accessible to clients.
         :param Sequence['GetNodeNodeGatewayMaintenanceWindowArgs'] maintenance_windows: Maintenance Windows define when this node is allowed to restart. If a node is requested to restart, it will check each window to determine if any of them permit it to restart, and if any do, it will. This check is repeated per window until the restart is successfully completed.  If not set here, may be set on the command line or via an environment variable on the process itself; any server setting will take precedence over local settings. This setting is ineffective for nodes below version 38.44.0.  If this setting is not applied via this remote configuration or via local configuration, the default setting is used: always allow restarts if serving no connections, and allow a restart even if serving connections between 7-8 UTC, any day.
         :param str name: Unique human-readable name of the Relay. Node names must include only letters, numbers, and hyphens (no spaces, underscores, or other special characters). Generated if not provided on create.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "device", device)
         pulumi.set(__self__, "location", location)
         pulumi.set(__self__, "version", version)
         if bind_address is not None:
             pulumi.set(__self__, "bind_address", bind_address)
-        if connects_to is not None:
-            pulumi.set(__self__, "connects_to", connects_to)
         if gateway_filter is not None:
             pulumi.set(__self__, "gateway_filter", gateway_filter)
         if id is not None:
             pulumi.set(__self__, "id", id)
         if listen_address is not None:
             pulumi.set(__self__, "listen_address", listen_address)
         if maintenance_windows is not None:
@@ -16890,22 +16862,14 @@
     def bind_address(self) -> Optional[str]:
         """
         The hostname/port tuple which the gateway daemon will bind to. If not provided on create, set to "0.0.0.0:listen_address_port".
         """
         return pulumi.get(self, "bind_address")
 
     @property
-    @pulumi.getter(name="connectsTo")
-    def connects_to(self) -> Optional[str]:
-        """
-        ConnectsTo can be used to restrict the peering between relays and gateways.
-        """
-        return pulumi.get(self, "connects_to")
-
-    @property
     @pulumi.getter(name="gatewayFilter")
     def gateway_filter(self) -> Optional[str]:
         """
         GatewayFilter can be used to restrict the peering between relays and gateways. Deprecated.
         """
         return pulumi.get(self, "gateway_filter")
 
@@ -16971,36 +16935,32 @@
 
 @pulumi.output_type
 class GetNodeNodeRelayResult(dict):
     def __init__(__self__, *,
                  device: str,
                  location: str,
                  version: str,
-                 connects_to: Optional[str] = None,
                  gateway_filter: Optional[str] = None,
                  id: Optional[str] = None,
                  maintenance_windows: Optional[Sequence['outputs.GetNodeNodeRelayMaintenanceWindowResult']] = None,
                  name: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str device: Device is a read only device name uploaded by the gateway process when it comes online.
         :param str location: Location is a read only network location uploaded by the gateway process when it comes online.
         :param str version: Version is a read only sdm binary version uploaded by the gateway process when it comes online.
-        :param str connects_to: ConnectsTo can be used to restrict the peering between relays and gateways.
         :param str gateway_filter: GatewayFilter can be used to restrict the peering between relays and gateways. Deprecated.
         :param str id: Unique identifier of the Relay.
         :param Sequence['GetNodeNodeRelayMaintenanceWindowArgs'] maintenance_windows: Maintenance Windows define when this node is allowed to restart. If a node is requested to restart, it will check each window to determine if any of them permit it to restart, and if any do, it will. This check is repeated per window until the restart is successfully completed.  If not set here, may be set on the command line or via an environment variable on the process itself; any server setting will take precedence over local settings. This setting is ineffective for nodes below version 38.44.0.  If this setting is not applied via this remote configuration or via local configuration, the default setting is used: always allow restarts if serving no connections, and allow a restart even if serving connections between 7-8 UTC, any day.
         :param str name: Unique human-readable name of the Relay. Node names must include only letters, numbers, and hyphens (no spaces, underscores, or other special characters). Generated if not provided on create.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "device", device)
         pulumi.set(__self__, "location", location)
         pulumi.set(__self__, "version", version)
-        if connects_to is not None:
-            pulumi.set(__self__, "connects_to", connects_to)
         if gateway_filter is not None:
             pulumi.set(__self__, "gateway_filter", gateway_filter)
         if id is not None:
             pulumi.set(__self__, "id", id)
         if maintenance_windows is not None:
             pulumi.set(__self__, "maintenance_windows", maintenance_windows)
         if name is not None:
@@ -17029,22 +16989,14 @@
     def version(self) -> str:
         """
         Version is a read only sdm binary version uploaded by the gateway process when it comes online.
         """
         return pulumi.get(self, "version")
 
     @property
-    @pulumi.getter(name="connectsTo")
-    def connects_to(self) -> Optional[str]:
-        """
-        ConnectsTo can be used to restrict the peering between relays and gateways.
-        """
-        return pulumi.get(self, "connects_to")
-
-    @property
     @pulumi.getter(name="gatewayFilter")
     def gateway_filter(self) -> Optional[str]:
         """
         GatewayFilter can be used to restrict the peering between relays and gateways. Deprecated.
         """
         return pulumi.get(self, "gateway_filter")
 
@@ -17097,14 +17049,174 @@
     @property
     @pulumi.getter(name="requireIdleness")
     def require_idleness(self) -> bool:
         return pulumi.get(self, "require_idleness")
 
 
 @pulumi.output_type
+class GetPeeringGroupNodePeeringGroupNodeResult(dict):
+    def __init__(__self__, *,
+                 group_id: Optional[str] = None,
+                 id: Optional[str] = None,
+                 node_id: Optional[str] = None):
+        """
+        :param str group_id: Peering Group ID to which the node will be attached to.
+        :param str id: Unique identifier of the Attachment.
+        :param str node_id: Node ID to be attached.
+        """
+        if group_id is not None:
+            pulumi.set(__self__, "group_id", group_id)
+        if id is not None:
+            pulumi.set(__self__, "id", id)
+        if node_id is not None:
+            pulumi.set(__self__, "node_id", node_id)
+
+    @property
+    @pulumi.getter(name="groupId")
+    def group_id(self) -> Optional[str]:
+        """
+        Peering Group ID to which the node will be attached to.
+        """
+        return pulumi.get(self, "group_id")
+
+    @property
+    @pulumi.getter
+    def id(self) -> Optional[str]:
+        """
+        Unique identifier of the Attachment.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter(name="nodeId")
+    def node_id(self) -> Optional[str]:
+        """
+        Node ID to be attached.
+        """
+        return pulumi.get(self, "node_id")
+
+
+@pulumi.output_type
+class GetPeeringGroupPeerPeeringGroupPeerResult(dict):
+    def __init__(__self__, *,
+                 group_id: Optional[str] = None,
+                 id: Optional[str] = None,
+                 peers_with_group_id: Optional[str] = None):
+        """
+        :param str group_id: Group ID from which the link will originate.
+        :param str id: Unique identifier of the Attachment.
+        :param str peers_with_group_id: Peering Group ID to which Group ID will link.
+        """
+        if group_id is not None:
+            pulumi.set(__self__, "group_id", group_id)
+        if id is not None:
+            pulumi.set(__self__, "id", id)
+        if peers_with_group_id is not None:
+            pulumi.set(__self__, "peers_with_group_id", peers_with_group_id)
+
+    @property
+    @pulumi.getter(name="groupId")
+    def group_id(self) -> Optional[str]:
+        """
+        Group ID from which the link will originate.
+        """
+        return pulumi.get(self, "group_id")
+
+    @property
+    @pulumi.getter
+    def id(self) -> Optional[str]:
+        """
+        Unique identifier of the Attachment.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter(name="peersWithGroupId")
+    def peers_with_group_id(self) -> Optional[str]:
+        """
+        Peering Group ID to which Group ID will link.
+        """
+        return pulumi.get(self, "peers_with_group_id")
+
+
+@pulumi.output_type
+class GetPeeringGroupPeeringGroupResult(dict):
+    def __init__(__self__, *,
+                 id: Optional[str] = None,
+                 name: Optional[str] = None):
+        """
+        :param str id: Unique identifier of the PeeringGroup.
+        :param str name: Unique human-readable name of the PeeringGroup.
+        """
+        if id is not None:
+            pulumi.set(__self__, "id", id)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+
+    @property
+    @pulumi.getter
+    def id(self) -> Optional[str]:
+        """
+        Unique identifier of the PeeringGroup.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[str]:
+        """
+        Unique human-readable name of the PeeringGroup.
+        """
+        return pulumi.get(self, "name")
+
+
+@pulumi.output_type
+class GetPeeringGroupResourcePeeringGroupResourceResult(dict):
+    def __init__(__self__, *,
+                 group_id: Optional[str] = None,
+                 id: Optional[str] = None,
+                 resource_id: Optional[str] = None):
+        """
+        :param str group_id: Peering Group ID to which the resource will be attached to.
+        :param str id: Unique identifier of the Attachment.
+        :param str resource_id: Resource ID to be attached.
+        """
+        if group_id is not None:
+            pulumi.set(__self__, "group_id", group_id)
+        if id is not None:
+            pulumi.set(__self__, "id", id)
+        if resource_id is not None:
+            pulumi.set(__self__, "resource_id", resource_id)
+
+    @property
+    @pulumi.getter(name="groupId")
+    def group_id(self) -> Optional[str]:
+        """
+        Peering Group ID to which the resource will be attached to.
+        """
+        return pulumi.get(self, "group_id")
+
+    @property
+    @pulumi.getter
+    def id(self) -> Optional[str]:
+        """
+        Unique identifier of the Attachment.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter(name="resourceId")
+    def resource_id(self) -> Optional[str]:
+        """
+        Resource ID to be attached.
+        """
+        return pulumi.get(self, "resource_id")
+
+
+@pulumi.output_type
 class GetRemoteIdentityGroupRemoteIdentityGroupResult(dict):
     def __init__(__self__, *,
                  id: Optional[str] = None,
                  name: Optional[str] = None):
         """
         :param str id: Unique identifier of the RemoteIdentityGroup.
         :param str name: Unique human-readable name of the RemoteIdentityGroup.
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/provider.py` & `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/provider.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/remote_identity.py` & `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/remote_identity.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/resource.py` & `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/resource.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/role.py` & `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/role.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm/secret_store.py` & `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm/secret_store.py`

 * *Files identical despite different names*

### Comparing `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm.egg-info/PKG-INFO` & `pierskarsenbarg_pulumi_sdm-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pierskarsenbarg-pulumi-sdm
-Version: 1.3.0
+Name: pierskarsenbarg_pulumi_sdm
+Version: 1.4.0
 Summary: A Pulumi package for creating and managing StrongDM cloud resources.
 Home-page: https://github.com/pierskarsenbarg/pulumi-sdm
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pierskarsenbarg/pulumi-sdm
 Description: # StrongDM Resource Provider
         
         The StrongDM Resource Provider lets you manage [StrongDM](http://strongdm.com) resources.
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.3.0/pierskarsenbarg_pulumi_sdm.egg-info/SOURCES.txt` & `pierskarsenbarg_pulumi_sdm-1.4.0/pierskarsenbarg_pulumi_sdm.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -4,22 +4,30 @@
 pierskarsenbarg_pulumi_sdm/_inputs.py
 pierskarsenbarg_pulumi_sdm/_utilities.py
 pierskarsenbarg_pulumi_sdm/account.py
 pierskarsenbarg_pulumi_sdm/account_attachment.py
 pierskarsenbarg_pulumi_sdm/get_account.py
 pierskarsenbarg_pulumi_sdm/get_account_attachment.py
 pierskarsenbarg_pulumi_sdm/get_node.py
+pierskarsenbarg_pulumi_sdm/get_peering_group.py
+pierskarsenbarg_pulumi_sdm/get_peering_group_node.py
+pierskarsenbarg_pulumi_sdm/get_peering_group_peer.py
+pierskarsenbarg_pulumi_sdm/get_peering_group_resource.py
 pierskarsenbarg_pulumi_sdm/get_remote_identity.py
 pierskarsenbarg_pulumi_sdm/get_remote_identity_group.py
 pierskarsenbarg_pulumi_sdm/get_resource.py
 pierskarsenbarg_pulumi_sdm/get_role.py
 pierskarsenbarg_pulumi_sdm/get_secret_store.py
 pierskarsenbarg_pulumi_sdm/get_ssh_ca_pubkey.py
 pierskarsenbarg_pulumi_sdm/node.py
 pierskarsenbarg_pulumi_sdm/outputs.py
+pierskarsenbarg_pulumi_sdm/peering_group.py
+pierskarsenbarg_pulumi_sdm/peering_group_node.py
+pierskarsenbarg_pulumi_sdm/peering_group_peer.py
+pierskarsenbarg_pulumi_sdm/peering_group_resource.py
 pierskarsenbarg_pulumi_sdm/provider.py
 pierskarsenbarg_pulumi_sdm/pulumi-plugin.json
 pierskarsenbarg_pulumi_sdm/py.typed
 pierskarsenbarg_pulumi_sdm/remote_identity.py
 pierskarsenbarg_pulumi_sdm/resource.py
 pierskarsenbarg_pulumi_sdm/role.py
 pierskarsenbarg_pulumi_sdm/secret_store.py
```

### Comparing `pierskarsenbarg_pulumi_sdm-1.3.0/setup.py` & `pierskarsenbarg_pulumi_sdm-1.4.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.3.0"
-PLUGIN_VERSION = "1.3.0"
+VERSION = "1.4.0"
+PLUGIN_VERSION = "1.4.0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'sdm', PLUGIN_VERSION, '--server', 'github://api.github.com/pierskarsenbarg/pulumi-sdm'])
         except OSError as error:
```

