# Comparing `tmp/aws_network_firewall-0.7.0.tar.gz` & `tmp/aws_network_firewall-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_network_firewall-0.7.0.tar", max compression
+gzip compressed data, was "aws_network_firewall-0.7.1.tar", max compression
```

## Comparing `aws_network_firewall-0.7.0.tar` & `aws_network_firewall-0.7.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11335 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0      800 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/README.md
--rw-r--r--   0        0        0       22 2023-07-31 12:29:04.254158 aws_network_firewall-0.7.0/aws_network_firewall/__init__.py
--rw-r--r--   0        0        0     1776 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/account.py
--rw-r--r--   0        0        0      175 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/cidr_range.py
--rw-r--r--   0        0        0      387 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/cidr_ranges.py
--rw-r--r--   0        0        0      505 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/cli/commands/__init__.py
--rw-r--r--   0        0        0     1365 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/cli/commands/check.py
--rw-r--r--   0        0        0      374 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/cli/commands/docs.py
--rw-r--r--   0        0        0     1191 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/cli/commands/update.py
--rw-r--r--   0        0        0      744 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/cli/handler.py
--rw-r--r--   0        0        0      352 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/destination.py
--rw-r--r--   0        0        0     1130 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/documentation_generator.py
--rw-r--r--   0        0        0     5277 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/rule.py
--rw-r--r--   0        0        0      708 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/rule_set.py
--rw-r--r--   0        0        0     2043 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/schemas/__init__.py
--rw-r--r--   0        0        0     2723 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/schemas/environment.yaml
--rw-r--r--   0        0        0      211 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/source.py
--rw-r--r--   0        0        0      210 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/suricata/__init__.py
--rw-r--r--   0        0        0      457 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/suricata/host.py
--rw-r--r--   0        0        0      473 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/suricata/option.py
--rw-r--r--   0        0        0     1812 2023-07-31 12:29:03.562112 aws_network_firewall-0.7.0/aws_network_firewall/suricata/rule.py
--rw-r--r--   0        0        0     1202 2023-07-31 12:29:04.254158 aws_network_firewall-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     1565 1970-01-01 00:00:00.000000 aws_network_firewall-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11335 2023-07-31 13:25:53.044341 aws_network_firewall-0.7.1/LICENSE.txt
+-rw-r--r--   0        0        0      800 2023-07-31 13:25:53.044341 aws_network_firewall-0.7.1/README.md
+-rw-r--r--   0        0        0       22 2023-07-31 13:25:53.756348 aws_network_firewall-0.7.1/aws_network_firewall/__init__.py
+-rw-r--r--   0        0        0     1776 2023-07-31 13:25:53.044341 aws_network_firewall-0.7.1/aws_network_firewall/account.py
+-rw-r--r--   0        0        0      175 2023-07-31 13:25:53.044341 aws_network_firewall-0.7.1/aws_network_firewall/cidr_range.py
+-rw-r--r--   0        0        0      387 2023-07-31 13:25:53.044341 aws_network_firewall-0.7.1/aws_network_firewall/cidr_ranges.py
+-rw-r--r--   0        0        0      505 2023-07-31 13:25:53.044341 aws_network_firewall-0.7.1/aws_network_firewall/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 13:25:53.044341 aws_network_firewall-0.7.1/aws_network_firewall/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1365 2023-07-31 13:25:53.044341 aws_network_firewall-0.7.1/aws_network_firewall/cli/commands/check.py
+-rw-r--r--   0        0        0      374 2023-07-31 13:25:53.044341 aws_network_firewall-0.7.1/aws_network_firewall/cli/commands/docs.py
+-rw-r--r--   0        0        0     1191 2023-07-31 13:25:53.044341 aws_network_firewall-0.7.1/aws_network_firewall/cli/commands/update.py
+-rw-r--r--   0        0        0      744 2023-07-31 13:25:53.044341 aws_network_firewall-0.7.1/aws_network_firewall/cli/handler.py
+-rw-r--r--   0        0        0      352 2023-07-31 13:25:53.044341 aws_network_firewall-0.7.1/aws_network_firewall/destination.py
+-rw-r--r--   0        0        0     1130 2023-07-31 13:25:53.044341 aws_network_firewall-0.7.1/aws_network_firewall/documentation_generator.py
+-rw-r--r--   0        0        0     6088 2023-07-31 13:25:53.044341 aws_network_firewall-0.7.1/aws_network_firewall/rule.py
+-rw-r--r--   0        0        0      708 2023-07-31 13:25:53.044341 aws_network_firewall-0.7.1/aws_network_firewall/rule_set.py
+-rw-r--r--   0        0        0     2043 2023-07-31 13:25:53.044341 aws_network_firewall-0.7.1/aws_network_firewall/schemas/__init__.py
+-rw-r--r--   0        0        0     2766 2023-07-31 13:25:53.044341 aws_network_firewall-0.7.1/aws_network_firewall/schemas/environment.yaml
+-rw-r--r--   0        0        0      211 2023-07-31 13:25:53.044341 aws_network_firewall-0.7.1/aws_network_firewall/source.py
+-rw-r--r--   0        0        0      210 2023-07-31 13:25:53.048341 aws_network_firewall-0.7.1/aws_network_firewall/suricata/__init__.py
+-rw-r--r--   0        0        0      457 2023-07-31 13:25:53.048341 aws_network_firewall-0.7.1/aws_network_firewall/suricata/host.py
+-rw-r--r--   0        0        0      473 2023-07-31 13:25:53.048341 aws_network_firewall-0.7.1/aws_network_firewall/suricata/option.py
+-rw-r--r--   0        0        0     1283 2023-07-31 13:25:53.048341 aws_network_firewall-0.7.1/aws_network_firewall/suricata/rule.py
+-rw-r--r--   0        0        0     1202 2023-07-31 13:25:53.756348 aws_network_firewall-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     1565 1970-01-01 00:00:00.000000 aws_network_firewall-0.7.1/PKG-INFO
```

### Comparing `aws_network_firewall-0.7.0/LICENSE.txt` & `aws_network_firewall-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.7.0/README.md` & `aws_network_firewall-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.7.0/aws_network_firewall/account.py` & `aws_network_firewall-0.7.1/aws_network_firewall/account.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.7.0/aws_network_firewall/cli/commands/check.py` & `aws_network_firewall-0.7.1/aws_network_firewall/cli/commands/check.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.7.0/aws_network_firewall/cli/commands/update.py` & `aws_network_firewall-0.7.1/aws_network_firewall/cli/commands/update.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.7.0/aws_network_firewall/cli/handler.py` & `aws_network_firewall-0.7.1/aws_network_firewall/cli/handler.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.7.0/aws_network_firewall/documentation_generator.py` & `aws_network_firewall-0.7.1/aws_network_firewall/documentation_generator.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.7.0/aws_network_firewall/rule.py` & `aws_network_firewall-0.7.1/aws_network_firewall/rule.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,23 +39,23 @@
         def convert_source(source: Source) -> Optional[SuricataHost]:
             return SuricataHost(address=source.cidr, port=0) if source.cidr else None
 
         return list(filter(None, map(convert_source, self.sources)))
 
     @staticmethod
     def __resolve_tls_options(
-        destination: Destination, tls_version: Optional[str]
+        destination: Destination, ssl_version: Optional[str]
     ) -> List[SuricataOption]:
         options = [
             SuricataOption(name="tls.sni"),
         ]
-        if tls_version:
+        if ssl_version:
             options.append(
                 SuricataOption(
-                    name="tls.version", value=tls_version, quoted_value=False
+                    name="ssl_version", value=ssl_version, quoted_value=False
                 )
             )
 
         if destination.endpoint.startswith("*"):  # type: ignore
             options += [
                 SuricataOption(name="dotprefix"),
                 SuricataOption(name="content", value=destination.endpoint[1:]),  # type: ignore
@@ -84,55 +84,77 @@
             SuricataOption(name="rev", value="1", quoted_value=False),
             SuricataOption(name="sid", value="XXX", quoted_value=False),
         ]
 
     def __resolve_tls_version_rules(
         self, destination: Destination
     ) -> List[SuricataRule]:
-        rules = []
+        ssl_version = ",".join(destination.tls_versions)
 
-        for tls_version in destination.tls_versions:
-            rules.append(
-                SuricataRule(
-                    action="pass",
-                    protocol=destination.protocol,
-                    sources=self.__suricata_source,
-                    destination=SuricataHost(
-                        address=destination.cidr if destination.cidr else "",
-                        port=destination.port if destination.port else 0,
-                    ),
-                    options=self.__resolve_tls_options(
-                        destination=destination, tls_version=tls_version
-                    )
-                    + self.__resolve_options(destination=destination),
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
+                    destination=destination, ssl_version=ssl_version
                 )
+                + self.__resolve_options(destination=destination),
             )
+        ]
 
-        return rules
+    def __resolve_tls_handshake(self, destination: Destination) -> SuricataRule:
+        if not destination.message:
+            destination.message = "Pass non-established TCP for 3-way handshake"
+        else:
+            destination.message += " | Pass non-established TCP for 3-way handshake"
+
+        rule = SuricataRule(
+            action="pass",
+            protocol="TCP",
+            sources=self.__suricata_source,
+            destination=SuricataHost(
+                address=destination.cidr if destination.cidr else "",
+                port=destination.port if destination.port else 0,
+            ),
+            options=[SuricataOption(name="flow", value="not_established")]
+            + self.__resolve_options(destination),
+        )
+
+        return rule
 
     def __resolve_tls_rules(self, destination: Destination) -> List[SuricataRule]:
         if destination.tls_versions:
             return self.__resolve_tls_version_rules(destination)
 
-        return [
+        rules = [
             SuricataRule(
                 action="pass",
                 protocol=destination.protocol,
                 sources=self.__suricata_source,
                 destination=SuricataHost(
                     address=destination.cidr if destination.cidr else "",
                     port=destination.port if destination.port else 0,
                 ),
                 options=self.__resolve_tls_options(
-                    destination=destination, tls_version=None
+                    destination=destination, ssl_version=None
                 )
                 + self.__resolve_options(destination=destination),
             )
         ]
 
+        if destination.port != 443:
+            rules.append(self.__resolve_tls_handshake(destination=destination))
+
+        return rules
+
     def __resolve_rule(self, destination: Destination) -> List[SuricataRule]:
         if destination.protocol == "TLS" and destination.endpoint:
             return self.__resolve_tls_rules(destination=destination)
 
         return [
             SuricataRule(
                 action="pass",
```

### Comparing `aws_network_firewall-0.7.0/aws_network_firewall/rule_set.py` & `aws_network_firewall-0.7.1/aws_network_firewall/rule_set.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.7.0/aws_network_firewall/schemas/__init__.py` & `aws_network_firewall-0.7.1/aws_network_firewall/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.7.0/aws_network_firewall/schemas/environment.yaml` & `aws_network_firewall-0.7.1/aws_network_firewall/schemas/environment.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,17 @@
       Protocol:
         enum: [ "TCP", "TLS", "ICMP" ]
       Port:
         type: integer
       Message:
         type: string
       TLSVersions:
-        enum: [ "1.2", "1.3" ]
+        type: array
+        items:
+          enum: [ "tls1.2", "tls1.3" ]
     examples:
       - Description: Website of Xebia
         Protocol: TLS
         Endpoint: xebia.com
         Region: eu-central-1
         Port: 443
```

### Comparing `aws_network_firewall-0.7.0/aws_network_firewall/suricata/rule.py` & `aws_network_firewall-0.7.1/aws_network_firewall/suricata/rule.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import List
+from typing import List, Optional
 
 from aws_network_firewall.suricata.host import Host
 from aws_network_firewall.suricata.option import Option
 
 
 @dataclass
 class Rule:
@@ -20,36 +20,28 @@
     options: List[Option]
 
     def __post_init__(self):
         self.protocol = self.protocol.lower()
 
     @property
     def direction(self) -> str:
-        return "<>" if self.protocol == "icmp" else "->"
+        message = next(
+            filter(lambda option: option.name == "msg", self.options),
+            Option(name="msg"),
+        )
+        if (
+            "Pass non-established TCP for 3-way handshake" in str(message.value)
+            or self.protocol == "icmp"
+        ):
+            return "<>"
+
+        return "->"
 
     @property
     def source(self) -> str:
         addresses = list(map(lambda host: host.address, self.sources))
         sources = ",".join(addresses)
         return f"[{sources}] any" if len(addresses) > 1 else f"{sources} any"
 
     def __str__(self) -> str:
-        post_rule = ""
         options = "; ".join(list(map(str, self.options)))
-
-        if self.protocol == "tls" and self.destination.port != 443:
-            message = next(
-                filter(lambda option: option.name == "msg", self.options),
-                Option(name="msg", value="Unknown"),
-            )
-            message.value = (
-                f"{message.value} | Pass non-established TCP for 3-way handshake"
-            )
-            flow = Option(name="flow", value="not_established")  # No quotes
-            sid = Option(name="sid", value="XXX", quoted_value=False)
-            rev = Option(name="rev", value="1", quoted_value=False)
-
-            handshake_options = "; ".join(list(map(str, [message, flow, rev, sid])))
-
-            post_rule = f"\n{self.action} tcp {self.source} <> {self.destination} ({handshake_options};)"
-
-        return f"{self.action} {self.protocol} {self.source} {self.direction} {self.destination} ({options};){post_rule}"
+        return f"{self.action} {self.protocol} {self.source} {self.direction} {self.destination} ({options};)"
```

### Comparing `aws_network_firewall-0.7.0/pyproject.toml` & `aws_network_firewall-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-network-firewall"
-version = "0.7.0"
+version = "0.7.1"
 description = ""
 authors = ["Joris Conijn <Joris.Conijn@xebia.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "aws_network_firewall"}]
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `aws_network_firewall-0.7.0/PKG-INFO` & `aws_network_firewall-0.7.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-network-firewall
-Version: 0.7.0
+Version: 0.7.1
 Summary: 
 License: MIT
 Author: Joris Conijn
 Author-email: Joris.Conijn@xebia.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

