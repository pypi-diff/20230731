# Comparing `tmp/aws_network_firewall-0.7.1.tar.gz` & `tmp/aws_network_firewall-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_network_firewall-0.7.1.tar", max compression
+gzip compressed data, was "aws_network_firewall-0.7.2.tar", max compression
```

## Comparing `aws_network_firewall-0.7.1.tar` & `aws_network_firewall-0.7.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11335 2023-07-31 13:25:53.044341 aws_network_firewall-0.7.1/LICENSE.txt
--rw-r--r--   0        0        0      800 2023-07-31 13:25:53.044341 aws_network_firewall-0.7.1/README.md
--rw-r--r--   0        0        0       22 2023-07-31 13:25:53.756348 aws_network_firewall-0.7.1/aws_network_firewall/__init__.py
--rw-r--r--   0        0        0     1776 2023-07-31 13:25:53.044341 aws_network_firewall-0.7.1/aws_network_firewall/account.py
--rw-r--r--   0        0        0      175 2023-07-31 13:25:53.044341 aws_network_firewall-0.7.1/aws_network_firewall/cidr_range.py
--rw-r--r--   0        0        0      387 2023-07-31 13:25:53.044341 aws_network_firewall-0.7.1/aws_network_firewall/cidr_ranges.py
--rw-r--r--   0        0        0      505 2023-07-31 13:25:53.044341 aws_network_firewall-0.7.1/aws_network_firewall/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 13:25:53.044341 aws_network_firewall-0.7.1/aws_network_firewall/cli/commands/__init__.py
--rw-r--r--   0        0        0     1365 2023-07-31 13:25:53.044341 aws_network_firewall-0.7.1/aws_network_firewall/cli/commands/check.py
--rw-r--r--   0        0        0      374 2023-07-31 13:25:53.044341 aws_network_firewall-0.7.1/aws_network_firewall/cli/commands/docs.py
--rw-r--r--   0        0        0     1191 2023-07-31 13:25:53.044341 aws_network_firewall-0.7.1/aws_network_firewall/cli/commands/update.py
--rw-r--r--   0        0        0      744 2023-07-31 13:25:53.044341 aws_network_firewall-0.7.1/aws_network_firewall/cli/handler.py
--rw-r--r--   0        0        0      352 2023-07-31 13:25:53.044341 aws_network_firewall-0.7.1/aws_network_firewall/destination.py
--rw-r--r--   0        0        0     1130 2023-07-31 13:25:53.044341 aws_network_firewall-0.7.1/aws_network_firewall/documentation_generator.py
--rw-r--r--   0        0        0     6088 2023-07-31 13:25:53.044341 aws_network_firewall-0.7.1/aws_network_firewall/rule.py
--rw-r--r--   0        0        0      708 2023-07-31 13:25:53.044341 aws_network_firewall-0.7.1/aws_network_firewall/rule_set.py
--rw-r--r--   0        0        0     2043 2023-07-31 13:25:53.044341 aws_network_firewall-0.7.1/aws_network_firewall/schemas/__init__.py
--rw-r--r--   0        0        0     2766 2023-07-31 13:25:53.044341 aws_network_firewall-0.7.1/aws_network_firewall/schemas/environment.yaml
--rw-r--r--   0        0        0      211 2023-07-31 13:25:53.044341 aws_network_firewall-0.7.1/aws_network_firewall/source.py
--rw-r--r--   0        0        0      210 2023-07-31 13:25:53.048341 aws_network_firewall-0.7.1/aws_network_firewall/suricata/__init__.py
--rw-r--r--   0        0        0      457 2023-07-31 13:25:53.048341 aws_network_firewall-0.7.1/aws_network_firewall/suricata/host.py
--rw-r--r--   0        0        0      473 2023-07-31 13:25:53.048341 aws_network_firewall-0.7.1/aws_network_firewall/suricata/option.py
--rw-r--r--   0        0        0     1283 2023-07-31 13:25:53.048341 aws_network_firewall-0.7.1/aws_network_firewall/suricata/rule.py
--rw-r--r--   0        0        0     1202 2023-07-31 13:25:53.756348 aws_network_firewall-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     1565 1970-01-01 00:00:00.000000 aws_network_firewall-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    11335 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/LICENSE.txt
+-rw-r--r--   0        0        0      800 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/README.md
+-rw-r--r--   0        0        0       22 2023-07-31 14:39:01.500255 aws_network_firewall-0.7.2/aws_network_firewall/__init__.py
+-rw-r--r--   0        0        0     1776 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/account.py
+-rw-r--r--   0        0        0      175 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/cidr_range.py
+-rw-r--r--   0        0        0      387 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/cidr_ranges.py
+-rw-r--r--   0        0        0      505 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1365 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/cli/commands/check.py
+-rw-r--r--   0        0        0      374 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/cli/commands/docs.py
+-rw-r--r--   0        0        0     1191 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/cli/commands/update.py
+-rw-r--r--   0        0        0      744 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/cli/handler.py
+-rw-r--r--   0        0        0      352 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/destination.py
+-rw-r--r--   0        0        0     1130 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/documentation_generator.py
+-rw-r--r--   0        0        0     6089 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/rule.py
+-rw-r--r--   0        0        0      708 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/rule_set.py
+-rw-r--r--   0        0        0     2043 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/schemas/__init__.py
+-rw-r--r--   0        0        0     2766 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/schemas/environment.yaml
+-rw-r--r--   0        0        0      211 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/source.py
+-rw-r--r--   0        0        0      210 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/suricata/__init__.py
+-rw-r--r--   0        0        0      457 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/suricata/host.py
+-rw-r--r--   0        0        0      473 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/suricata/option.py
+-rw-r--r--   0        0        0     1283 2023-07-31 14:39:00.540249 aws_network_firewall-0.7.2/aws_network_firewall/suricata/rule.py
+-rw-r--r--   0        0        0     1202 2023-07-31 14:39:01.504255 aws_network_firewall-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     1565 1970-01-01 00:00:00.000000 aws_network_firewall-0.7.2/PKG-INFO
```

### Comparing `aws_network_firewall-0.7.1/LICENSE.txt` & `aws_network_firewall-0.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.7.1/README.md` & `aws_network_firewall-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.7.1/aws_network_firewall/account.py` & `aws_network_firewall-0.7.2/aws_network_firewall/account.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.7.1/aws_network_firewall/cli/commands/check.py` & `aws_network_firewall-0.7.2/aws_network_firewall/cli/commands/check.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.7.1/aws_network_firewall/cli/commands/update.py` & `aws_network_firewall-0.7.2/aws_network_firewall/cli/commands/update.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.7.1/aws_network_firewall/cli/handler.py` & `aws_network_firewall-0.7.2/aws_network_firewall/cli/handler.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.7.1/aws_network_firewall/documentation_generator.py` & `aws_network_firewall-0.7.2/aws_network_firewall/documentation_generator.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.7.1/aws_network_firewall/rule.py` & `aws_network_firewall-0.7.2/aws_network_firewall/rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,17 +123,14 @@
             options=[SuricataOption(name="flow", value="not_established")]
             + self.__resolve_options(destination),
         )
 
         return rule
 
     def __resolve_tls_rules(self, destination: Destination) -> List[SuricataRule]:
-        if destination.tls_versions:
-            return self.__resolve_tls_version_rules(destination)
-
         rules = [
             SuricataRule(
                 action="pass",
                 protocol=destination.protocol,
                 sources=self.__suricata_source,
                 destination=SuricataHost(
                     address=destination.cidr if destination.cidr else "",
@@ -142,14 +139,17 @@
                 options=self.__resolve_tls_options(
                     destination=destination, ssl_version=None
                 )
                 + self.__resolve_options(destination=destination),
             )
         ]
 
+        if destination.tls_versions:
+            rules = self.__resolve_tls_version_rules(destination)
+
         if destination.port != 443:
             rules.append(self.__resolve_tls_handshake(destination=destination))
 
         return rules
 
     def __resolve_rule(self, destination: Destination) -> List[SuricataRule]:
         if destination.protocol == "TLS" and destination.endpoint:
```

### Comparing `aws_network_firewall-0.7.1/aws_network_firewall/rule_set.py` & `aws_network_firewall-0.7.2/aws_network_firewall/rule_set.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.7.1/aws_network_firewall/schemas/__init__.py` & `aws_network_firewall-0.7.2/aws_network_firewall/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.7.1/aws_network_firewall/schemas/environment.yaml` & `aws_network_firewall-0.7.2/aws_network_firewall/schemas/environment.yaml`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.7.1/aws_network_firewall/suricata/rule.py` & `aws_network_firewall-0.7.2/aws_network_firewall/suricata/rule.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.7.1/pyproject.toml` & `aws_network_firewall-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-network-firewall"
-version = "0.7.1"
+version = "0.7.2"
 description = ""
 authors = ["Joris Conijn <Joris.Conijn@xebia.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "aws_network_firewall"}]
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `aws_network_firewall-0.7.1/PKG-INFO` & `aws_network_firewall-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-network-firewall
-Version: 0.7.1
+Version: 0.7.2
 Summary: 
 License: MIT
 Author: Joris Conijn
 Author-email: Joris.Conijn@xebia.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

