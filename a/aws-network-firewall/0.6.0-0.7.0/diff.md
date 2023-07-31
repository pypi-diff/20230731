# Comparing `tmp/aws_network_firewall-0.6.0.tar.gz` & `tmp/aws_network_firewall-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_network_firewall-0.6.0.tar", max compression
+gzip compressed data, was "aws_network_firewall-0.7.0.tar", max compression
```

## Comparing `aws_network_firewall-0.6.0.tar` & `aws_network_firewall-0.7.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11335 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0      800 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/README.md
--rw-r--r--   0        0        0       22 2023-07-28 17:35:51.650500 aws_network_firewall-0.6.0/aws_network_firewall/__init__.py
--rw-r--r--   0        0        0     1776 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/account.py
--rw-r--r--   0        0        0      175 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/cidr_range.py
--rw-r--r--   0        0        0      387 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/cidr_ranges.py
--rw-r--r--   0        0        0      505 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/cli/commands/__init__.py
--rw-r--r--   0        0        0     1365 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/cli/commands/check.py
--rw-r--r--   0        0        0      374 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/cli/commands/docs.py
--rw-r--r--   0        0        0     1191 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/cli/commands/update.py
--rw-r--r--   0        0        0      744 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/cli/handler.py
--rw-r--r--   0        0        0      318 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/destination.py
--rw-r--r--   0        0        0     1130 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/documentation_generator.py
--rw-r--r--   0        0        0     3501 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/rule.py
--rw-r--r--   0        0        0      708 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/rule_set.py
--rw-r--r--   0        0        0     1992 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/schemas/__init__.py
--rw-r--r--   0        0        0     2673 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/schemas/environment.yaml
--rw-r--r--   0        0        0      211 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/source.py
--rw-r--r--   0        0        0      210 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/suricata/__init__.py
--rw-r--r--   0        0        0      457 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/suricata/host.py
--rw-r--r--   0        0        0      473 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/suricata/option.py
--rw-r--r--   0        0        0     1812 2023-07-28 17:35:50.874461 aws_network_firewall-0.6.0/aws_network_firewall/suricata/rule.py
--rw-r--r--   0        0        0     1202 2023-07-28 17:35:51.650500 aws_network_firewall-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1565 1970-01-01 00:00:00.000000 aws_network_firewall-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11335 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0      800 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/README.md
+-rw-r--r--   0        0        0       22 2023-07-31 12:29:04.254158 aws_network_firewall-0.7.0/aws_network_firewall/__init__.py
+-rw-r--r--   0        0        0     1776 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/account.py
+-rw-r--r--   0        0        0      175 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/cidr_range.py
+-rw-r--r--   0        0        0      387 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/cidr_ranges.py
+-rw-r--r--   0        0        0      505 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1365 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/cli/commands/check.py
+-rw-r--r--   0        0        0      374 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/cli/commands/docs.py
+-rw-r--r--   0        0        0     1191 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/cli/commands/update.py
+-rw-r--r--   0        0        0      744 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/cli/handler.py
+-rw-r--r--   0        0        0      352 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/destination.py
+-rw-r--r--   0        0        0     1130 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/documentation_generator.py
+-rw-r--r--   0        0        0     5277 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/rule.py
+-rw-r--r--   0        0        0      708 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/rule_set.py
+-rw-r--r--   0        0        0     2043 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/schemas/__init__.py
+-rw-r--r--   0        0        0     2723 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/schemas/environment.yaml
+-rw-r--r--   0        0        0      211 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/source.py
+-rw-r--r--   0        0        0      210 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/suricata/__init__.py
+-rw-r--r--   0        0        0      457 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/suricata/host.py
+-rw-r--r--   0        0        0      473 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/suricata/option.py
+-rw-r--r--   0        0        0     1812 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/suricata/rule.py
+-rw-r--r--   0        0        0     1202 2023-07-31 12:29:04.254158 aws_network_firewall-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1565 1970-01-01 00:00:00.000000 aws_network_firewall-0.7.0/PKG-INFO
```

### Comparing `aws_network_firewall-0.6.0/LICENSE.txt` & `aws_network_firewall-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.6.0/README.md` & `aws_network_firewall-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.6.0/aws_network_firewall/account.py` & `aws_network_firewall-0.7.0/aws_network_firewall/account.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.6.0/aws_network_firewall/cli/commands/check.py` & `aws_network_firewall-0.7.0/aws_network_firewall/cli/commands/check.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.6.0/aws_network_firewall/cli/commands/update.py` & `aws_network_firewall-0.7.0/aws_network_firewall/cli/commands/update.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.6.0/aws_network_firewall/cli/handler.py` & `aws_network_firewall-0.7.0/aws_network_firewall/cli/handler.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.6.0/aws_network_firewall/documentation_generator.py` & `aws_network_firewall-0.7.0/aws_network_firewall/documentation_generator.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.6.0/aws_network_firewall/rule.py` & `aws_network_firewall-0.7.0/aws_network_firewall/rule.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import itertools
 from dataclasses import dataclass
 from typing import List, Optional, ClassVar
 
 from aws_network_firewall.source import Source
 from aws_network_firewall.destination import Destination
 from aws_network_firewall.suricata import SuricataRule, SuricataHost, SuricataOption
 
@@ -37,70 +38,118 @@
     def __suricata_source(self) -> List[SuricataHost]:
         def convert_source(source: Source) -> Optional[SuricataHost]:
             return SuricataHost(address=source.cidr, port=0) if source.cidr else None
 
         return list(filter(None, map(convert_source, self.sources)))
 
     @staticmethod
-    def __tls_endpoint_options(endpoint: str) -> List[SuricataOption]:
+    def __resolve_tls_options(
+        destination: Destination, tls_version: Optional[str]
+    ) -> List[SuricataOption]:
         options = [
             SuricataOption(name="tls.sni"),
-            SuricataOption(name="tls.version", value="1.2", quoted_value=False),
-            # When using multiple tls versions you need 2 rules
-            # openssl 1.1.1 is needed for tls1.3
-            # SuricataOption(name="tls.version", value="1.3", quoted_value=False),
         ]
+        if tls_version:
+            options.append(
+                SuricataOption(
+                    name="tls.version", value=tls_version, quoted_value=False
+                )
+            )
 
-        if endpoint.startswith("*"):
+        if destination.endpoint.startswith("*"):  # type: ignore
             options += [
                 SuricataOption(name="dotprefix"),
-                SuricataOption(name="content", value=endpoint[1:]),
+                SuricataOption(name="content", value=destination.endpoint[1:]),  # type: ignore
                 SuricataOption(name="nocase"),
                 SuricataOption(name="endswith"),
             ]
         else:
             options += [
-                SuricataOption(name="content", value=endpoint),
+                SuricataOption(name="content", value=destination.endpoint),
                 SuricataOption(name="nocase"),
                 SuricataOption(name="startswith"),
                 SuricataOption(name="endswith"),
             ]
 
         return options
 
     def __resolve_options(self, destination: Destination) -> List[SuricataOption]:
-        options = []
-
-        if destination.protocol == "TLS" and destination.endpoint:
-            options = self.__tls_endpoint_options(destination.endpoint)
-
         message = (
             f"{destination.message} | {self.workload} | {self.name}"
             if destination.message
             else f"{self.workload} | {self.name}"
         )
 
-        return options + [
+        return [
             SuricataOption(name="msg", value=message),
             SuricataOption(name="rev", value="1", quoted_value=False),
             SuricataOption(name="sid", value="XXX", quoted_value=False),
         ]
 
-    def __resolve_rule(self, destination: Destination) -> SuricataRule:
-        return SuricataRule(
-            action="pass",
-            protocol=destination.protocol,
-            sources=self.__suricata_source,
-            destination=SuricataHost(
-                address=destination.cidr if destination.cidr else "",
-                port=destination.port if destination.port else 0,
-            ),
-            options=self.__resolve_options(destination),
-        )
+    def __resolve_tls_version_rules(
+        self, destination: Destination
+    ) -> List[SuricataRule]:
+        rules = []
+
+        for tls_version in destination.tls_versions:
+            rules.append(
+                SuricataRule(
+                    action="pass",
+                    protocol=destination.protocol,
+                    sources=self.__suricata_source,
+                    destination=SuricataHost(
+                        address=destination.cidr if destination.cidr else "",
+                        port=destination.port if destination.port else 0,
+                    ),
+                    options=self.__resolve_tls_options(
+                        destination=destination, tls_version=tls_version
+                    )
+                    + self.__resolve_options(destination=destination),
+                )
+            )
+
+        return rules
+
+    def __resolve_tls_rules(self, destination: Destination) -> List[SuricataRule]:
+        if destination.tls_versions:
+            return self.__resolve_tls_version_rules(destination)
+
+        return [
+            SuricataRule(
+                action="pass",
+                protocol=destination.protocol,
+                sources=self.__suricata_source,
+                destination=SuricataHost(
+                    address=destination.cidr if destination.cidr else "",
+                    port=destination.port if destination.port else 0,
+                ),
+                options=self.__resolve_tls_options(
+                    destination=destination, tls_version=None
+                )
+                + self.__resolve_options(destination=destination),
+            )
+        ]
+
+    def __resolve_rule(self, destination: Destination) -> List[SuricataRule]:
+        if destination.protocol == "TLS" and destination.endpoint:
+            return self.__resolve_tls_rules(destination=destination)
+
+        return [
+            SuricataRule(
+                action="pass",
+                protocol=destination.protocol,
+                sources=self.__suricata_source,
+                destination=SuricataHost(
+                    address=destination.cidr if destination.cidr else "",
+                    port=destination.port if destination.port else 0,
+                ),
+                options=self.__resolve_options(destination),
+            )
+        ]
 
     @property
     def suricata_rules(self) -> List[SuricataRule]:
         rules = list(filter(None, map(self.__resolve_rule, self.destinations)))
-        return rules
+        return list(itertools.chain.from_iterable(rules))
 
     def __str__(self) -> str:
         return "\n".join(map(str, self.suricata_rules))
```

### Comparing `aws_network_firewall-0.6.0/aws_network_firewall/rule_set.py` & `aws_network_firewall-0.7.0/aws_network_firewall/rule_set.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.6.0/aws_network_firewall/schemas/__init__.py` & `aws_network_firewall-0.7.0/aws_network_firewall/schemas/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     return Destination(
         description=entry["Description"],
         protocol=entry["Protocol"],
         port=entry.get("Port"),
         endpoint=entry.get("Endpoint"),
         cidr=entry.get("Cidr"),
         message=entry.get("Message"),
+        tls_versions=entry.get("TLSVersions", []),
     )
 
 
 def rule_resolver(workload: str, entry: dict) -> Rule:
     return Rule(
         workload=workload,
         type=entry["Type"],
```

### Comparing `aws_network_firewall-0.6.0/aws_network_firewall/schemas/environment.yaml` & `aws_network_firewall-0.7.0/aws_network_firewall/schemas/environment.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -111,14 +111,16 @@
         type: string
       Protocol:
         enum: [ "TCP", "TLS", "ICMP" ]
       Port:
         type: integer
       Message:
         type: string
+      TLSVersions:
+        enum: [ "1.2", "1.3" ]
     examples:
       - Description: Website of Xebia
         Protocol: TLS
         Endpoint: xebia.com
         Region: eu-central-1
         Port: 443
```

### Comparing `aws_network_firewall-0.6.0/aws_network_firewall/suricata/rule.py` & `aws_network_firewall-0.7.0/aws_network_firewall/suricata/rule.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.6.0/pyproject.toml` & `aws_network_firewall-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-network-firewall"
-version = "0.6.0"
+version = "0.7.0"
 description = ""
 authors = ["Joris Conijn <Joris.Conijn@xebia.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "aws_network_firewall"}]
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `aws_network_firewall-0.6.0/PKG-INFO` & `aws_network_firewall-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-network-firewall
-Version: 0.6.0
+Version: 0.7.0
 Summary: 
 License: MIT
 Author: Joris Conijn
 Author-email: Joris.Conijn@xebia.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

