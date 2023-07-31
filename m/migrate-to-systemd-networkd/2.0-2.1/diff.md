# Comparing `tmp/migrate_to_systemd_networkd-2.0.tar.gz` & `tmp/migrate_to_systemd_networkd-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "migrate_to_systemd_networkd-2.0.tar", max compression
+gzip compressed data, was "migrate_to_systemd_networkd-2.1.tar", max compression
```

## Comparing `migrate_to_systemd_networkd-2.0.tar` & `migrate_to_systemd_networkd-2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-07-31 00:51:37.191347 migrate_to_systemd_networkd-2.0/migrate_to_systemd_networkd/__init__.py
--rw-r--r--   0        0        0    14811 2023-07-31 00:51:37.191347 migrate_to_systemd_networkd-2.0/migrate_to_systemd_networkd/ifupdown.py
--rw-r--r--   0        0        0     1430 2023-07-31 00:51:37.191347 migrate_to_systemd_networkd-2.0/migrate_to_systemd_networkd/utils.py
--rw-r--r--   0        0        0      403 2023-07-31 00:51:37.191347 migrate_to_systemd_networkd-2.0/pyproject.toml
--rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 migrate_to_systemd_networkd-2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-31 00:51:37.191347 migrate_to_systemd_networkd-2.1/migrate_to_systemd_networkd/__init__.py
+-rw-r--r--   0        0        0    15434 2023-07-31 01:22:03.272552 migrate_to_systemd_networkd-2.1/migrate_to_systemd_networkd/ifupdown.py
+-rw-r--r--   0        0        0     1430 2023-07-31 00:51:37.191347 migrate_to_systemd_networkd-2.1/migrate_to_systemd_networkd/utils.py
+-rw-r--r--   0        0        0      452 2023-07-31 01:25:33.746386 migrate_to_systemd_networkd-2.1/pyproject.toml
+-rw-r--r--   0        0        0      587 1970-01-01 00:00:00.000000 migrate_to_systemd_networkd-2.1/PKG-INFO
```

### Comparing `migrate_to_systemd_networkd-2.0/migrate_to_systemd_networkd/ifupdown.py` & `migrate_to_systemd_networkd-2.1/migrate_to_systemd_networkd/ifupdown.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,48 +59,66 @@
     ):
         network = "{}.network".format(name)
         netdev = "{}.netdev".format(name)
         # Match Block
         result[network]["Match"]["Name"] = name
 
         # Configs
-        if "address" in config and "netmask" in config:
-            # address and netmask
-            netmask = ipaddress.IPv4Network("0.0.0.0/{}".format(config["netmask"][0]))
-            result[network]["Address"]["Address"] = "{}/{}".format(
-                config["address"][0], netmask.prefixlen
-            )
-        elif "address" in config:
-            # only address
-            result[network]["Address"]["Address"] = config["address"][0]
-
-        if method == "static":
-            if "scope" in config:
-                result[network]["Address"]["Scope"] = config["scope"][0]
-            if "pointopoint" in config:
-                result[network]["Address"]["Peer"] = config["pointopoint"][0]
-            if "metric" in config:
-                result[network]["Address"]["RouteMetric"] = config["metric"][0]
+        if "address" in config:
+            address_config = AutoVivification()
+            if "netmask" in config:
+                # address and netmask
+                netmask = ipaddress.IPv4Network(
+                    "0.0.0.0/{}".format(config["netmask"][0]))
+                address = "{}/{}".format(
+                    config["address"][0], netmask.prefixlen
+                )
+            else:
+                # only address
+                address = config["address"][0]
+            address_config["Address"] = address
+
+            if method == "static":
+                if "scope" in config:
+                    address_config["Scope"] = config["scope"][0]
+                if "pointopoint" in config:
+                    address_config["Peer"] = config["pointopoint"][0]
+                if "metric" in config:
+                    address_config["RouteMetric"] = config["metric"][0]
+
+            if "Address" in result[network]:
+                result[network]["Address"].append(address_config)
+            else:
+                result[network]["Address"] = [address_config]
+
+        if method == "static" and not is_ipv4:
+            # inet6 static
+            result[network]["Network"]["IPv6AcceptRA"] = "no"
 
         if "gateway" in config:
-            result[network]["Network"]["Gateway"] = config["gateway"][0]
+            gateway = config["gateway"][0]
+            if "Gateway" in result[network]["Network"]:
+                result[network]["Network"]["Gateway"].append(gateway)
+            else:
+                result[network]["Network"]["Gateway"] = [gateway]
+
         if "hwaddress" in config:
             value = config["hwaddress"][0]
             parts = value.split(" ")
             # hwaddress ether
             if parts[0] == "ether":
                 result[network]["Link"]["MACAddress"] = parts[1]
         if "mtu" in config:
             result[network]["Link"]["MTUBytes"] = config["mtu"][0]
 
         # VLAN:
         if "." in name:
             index = name.rfind(".")
             device = name[:index]
-            vlan_id = int(name[index + 1 :])
+            vlan_id = int(name[index + 1:])
 
             result[netdev]["NetDev"]["Name"] = name
             result[netdev]["NetDev"]["Kind"] = "vlan"
             result[netdev]["VLAN"]["Id"] = vlan_id
 
             raw_network = "{}.network".format(device)
 
@@ -135,15 +153,16 @@
                 "active-backup",
                 "balance-xor",
                 "broadcast",
                 "802.3ad",
                 "balance-tlb",
                 "balance-alb",
             ]
-            result[netdev]["Bond"]["Mode"] = policy[int(config["bond-mode"][0])]
+            result[netdev]["Bond"]["Mode"] = policy[int(
+                config["bond-mode"][0])]
         if "bond-miimon" in config:
             result[netdev]["Bond"]["MIIMonitorSec"] = (
                 float(config["bond-miimon"][0]) / 1000
             )
         if "bond-lacp-rate" in config:
             rate = {"30": "slow", "1": "fast"}
             result[netdev]["Bond"]["LACPTransmitRate"] = rate[
@@ -397,15 +416,16 @@
     )
     parser.add_argument(
         "--config",
         required=False,
         help="output config for systemd-networkd service config, default to /etc/systemd/networkd.conf.d/tables.conf",
         default="/etc/systemd/networkd.conf.d/tables.conf",
     )
-    parser.add_argument("--systemd-version", required=False, help="systemd version")
+    parser.add_argument("--systemd-version", required=False,
+                        help="systemd version")
     args = parser.parse_args()
 
     converter = Converter(
         args.interfaces, args.tables, args.output, args.config, args.systemd_version
     )
     converter.work()
```

### Comparing `migrate_to_systemd_networkd-2.0/migrate_to_systemd_networkd/utils.py` & `migrate_to_systemd_networkd-2.1/migrate_to_systemd_networkd/utils.py`

 * *Files identical despite different names*

### Comparing `migrate_to_systemd_networkd-2.0/PKG-INFO` & `migrate_to_systemd_networkd-2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: migrate-to-systemd-networkd
-Version: 2.0
-Summary: 
+Version: 2.1
+Summary: Migrate network configuration to systemd networkd
 Author: Jiajie Chen
 Author-email: c@jia.je
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

