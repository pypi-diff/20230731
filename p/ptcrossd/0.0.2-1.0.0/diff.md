# Comparing `tmp/ptcrossd-0.0.2.tar.gz` & `tmp/ptcrossd-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptcrossd-0.0.2.tar", last modified: Mon Mar 28 16:54:20 2022, max compression
+gzip compressed data, was "ptcrossd-1.0.0.tar", last modified: Mon Jul 31 18:51:43 2023, max compression
```

## Comparing `ptcrossd-0.0.2.tar` & `ptcrossd-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2022-03-28 16:54:20.037387 ptcrossd-0.0.2/
--rw-r--r--   0 kali      (1000) kali      (1000)    35823 2021-12-17 14:07:29.000000 ptcrossd-0.0.2/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     2563 2022-03-28 16:54:20.037387 ptcrossd-0.0.2/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     2190 2022-03-28 16:53:55.000000 ptcrossd-0.0.2/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2022-03-28 16:54:20.037387 ptcrossd-0.0.2/ptcrossd/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2021-12-17 14:07:29.000000 ptcrossd-0.0.2/ptcrossd/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)     7049 2022-03-28 16:53:44.000000 ptcrossd-0.0.2/ptcrossd/ptcrossd.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2022-03-28 16:54:20.037387 ptcrossd-0.0.2/ptcrossd.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     2563 2022-03-28 16:54:19.000000 ptcrossd-0.0.2/ptcrossd.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      262 2022-03-28 16:54:19.000000 ptcrossd-0.0.2/ptcrossd.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2022-03-28 16:54:19.000000 ptcrossd-0.0.2/ptcrossd.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       53 2022-03-28 16:54:19.000000 ptcrossd-0.0.2/ptcrossd.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       34 2022-03-28 16:54:19.000000 ptcrossd-0.0.2/ptcrossd.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        9 2022-03-28 16:54:19.000000 ptcrossd-0.0.2/ptcrossd.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2022-03-28 16:54:20.037387 ptcrossd-0.0.2/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)      835 2022-03-28 16:54:04.000000 ptcrossd-0.0.2/setup.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-31 18:51:43.695000 ptcrossd-1.0.0/
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    35823 2023-07-27 11:42:59.000000 ptcrossd-1.0.0/LICENSE
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3090 2023-07-31 18:51:43.695000 ptcrossd-1.0.0/PKG-INFO
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2601 2023-07-31 14:12:20.000000 ptcrossd-1.0.0/README.md
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-31 18:51:43.691000 ptcrossd-1.0.0/ptcrossd/
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-27 11:42:59.000000 ptcrossd-1.0.0/ptcrossd/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       21 2023-07-27 11:42:59.000000 ptcrossd-1.0.0/ptcrossd/_version.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     8901 2023-07-31 13:52:11.000000 ptcrossd-1.0.0/ptcrossd/ptcrossd.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-31 18:51:43.695000 ptcrossd-1.0.0/ptcrossd.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3090 2023-07-31 18:51:43.000000 ptcrossd-1.0.0/ptcrossd.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      283 2023-07-31 18:51:43.000000 ptcrossd-1.0.0/ptcrossd.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-07-31 18:51:43.000000 ptcrossd-1.0.0/ptcrossd.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       52 2023-07-31 18:51:43.000000 ptcrossd-1.0.0/ptcrossd.egg-info/entry_points.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       33 2023-07-31 18:51:43.000000 ptcrossd-1.0.0/ptcrossd.egg-info/requires.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        9 2023-07-31 18:51:43.000000 ptcrossd-1.0.0/ptcrossd.egg-info/top_level.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-07-31 18:51:43.695000 ptcrossd-1.0.0/setup.cfg
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1036 2023-07-27 11:42:59.000000 ptcrossd-1.0.0/setup.py
```

### Comparing `ptcrossd-0.0.2/LICENSE` & `ptcrossd-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ptcrossd-0.0.2/PKG-INFO` & `ptcrossd-1.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,78 +1,98 @@
 Metadata-Version: 2.1
 Name: ptcrossd
-Version: 0.0.2
-Summary: Crossdomain.xml Testing Tool
+Version: 1.0.0
+Summary: crossdomain.xml misconfigurations testing tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3+
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
+Classifier: Topic :: Security
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)
+[![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
+
 
 # PTCROSSD
-> Crossdomain.xml Testing Tool
+
+> crossdomain.xml misconfigurations testing tool
 
 ## Installation
 ```
 pip install ptcrossd
 ```
 
 ## Add to PATH
+If you cannot invoke the script in your terminal, its probably because its not in your PATH. Fix it by running commands below.
+
+> Add to PATH for Bash
 ```bash
-# If you cannot invoke the script in your terminal, its probably because its not in your PATH. Fix it by running commands below.
 echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.bashrc
 source ~/.bashrc
 ```
 
+> Add to PATH for ZSH
+```bash
+echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshhrc
+source ~/.zshhrc
+```
+
+
 ## Usage examples
 ```
-$ ptcrossd.py -u https://www.example.com/crossdomain.xml
-$ ptcrossd.py -u https://www.example.com/
+ptcrossd -u https://www.example.com/crossdomain.xml
+ptcrossd -u https://www.example.com/
 ```
 
 ## Options
+
 ```
 -u   --url         <url>           Connect to URL
 -p   --proxy       <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
+-T   --timeout     <timeout>       Set timeout (default to 10)
 -c   --cookie      <cookie>        Set cookie
--H   --headers     <header:value>  Set custom header(s)
 -ua  --user-agent  <user-agent>    Set User-Agent header
--j   --json                        Output in JSON format
+-H   --headers     <header:value>  Set custom header(s)
+-C   --cache                       Cache requests (load from tmp in future)
 -v   --version                     Show script version and exit
 -h   --help                        Show this help message and exit
+-j   --json                        Output in JSON format
 ```
 
 ## Dependencies
-    - defusedxml
-    - requests
-    - ptlibs
+```
+defusedxml
+requests
+ptlibs
+```
 
 ## Version History
-- 0.0.1 - 0.0.2
-    - Alpha release
-
-## Licence
+```
+1.0.0
+    - updated for ptlibs 1.0.0
+    - code refactorization
+0.0.1 - 0.0.2
+    - Alpha releases
+```
+## License
 
-Copyright (c) 2020 HACKER Consulting s.r.o.
+Copyright (c) 2023 Penterep Security s.r.o.
 
 ptcrossd is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 ptcrossd is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with ptcrossd. If not, see https://www.gnu.org/licenses/.
 
 ## Warning
 
 You are only allowed to run the tool against the websites which
 you have been given permission to pentest. We do not accept any
 responsibility for any damage/harm that this application causes to your
 computer, or your network. Penterep is not responsible for any illegal
 or malicious use of this code. Be Ethical!
-
```

### Comparing `ptcrossd-0.0.2/README.md` & `ptcrossd-1.0.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,54 +1,74 @@
-![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)
+[![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
+
 
 # PTCROSSD
-> Crossdomain.xml Testing Tool
+
+> crossdomain.xml misconfigurations testing tool
 
 ## Installation
 ```
 pip install ptcrossd
 ```
 
 ## Add to PATH
+If you cannot invoke the script in your terminal, its probably because its not in your PATH. Fix it by running commands below.
+
+> Add to PATH for Bash
 ```bash
-# If you cannot invoke the script in your terminal, its probably because its not in your PATH. Fix it by running commands below.
 echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.bashrc
 source ~/.bashrc
 ```
 
+> Add to PATH for ZSH
+```bash
+echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshhrc
+source ~/.zshhrc
+```
+
+
 ## Usage examples
 ```
-$ ptcrossd.py -u https://www.example.com/crossdomain.xml
-$ ptcrossd.py -u https://www.example.com/
+ptcrossd -u https://www.example.com/crossdomain.xml
+ptcrossd -u https://www.example.com/
 ```
 
 ## Options
+
 ```
 -u   --url         <url>           Connect to URL
 -p   --proxy       <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
+-T   --timeout     <timeout>       Set timeout (default to 10)
 -c   --cookie      <cookie>        Set cookie
--H   --headers     <header:value>  Set custom header(s)
 -ua  --user-agent  <user-agent>    Set User-Agent header
--j   --json                        Output in JSON format
+-H   --headers     <header:value>  Set custom header(s)
+-C   --cache                       Cache requests (load from tmp in future)
 -v   --version                     Show script version and exit
 -h   --help                        Show this help message and exit
+-j   --json                        Output in JSON format
 ```
 
 ## Dependencies
-    - defusedxml
-    - requests
-    - ptlibs
+```
+defusedxml
+requests
+ptlibs
+```
 
 ## Version History
-- 0.0.1 - 0.0.2
-    - Alpha release
-
-## Licence
+```
+1.0.0
+    - updated for ptlibs 1.0.0
+    - code refactorization
+0.0.1 - 0.0.2
+    - Alpha releases
+```
+## License
 
-Copyright (c) 2020 HACKER Consulting s.r.o.
+Copyright (c) 2023 Penterep Security s.r.o.
 
 ptcrossd is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 ptcrossd is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with ptcrossd. If not, see https://www.gnu.org/licenses/.
```

### Comparing `ptcrossd-0.0.2/ptcrossd/ptcrossd.py` & `ptcrossd-1.0.0/ptcrossd/ptcrossd.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,158 +1,173 @@
 #!/usr/bin/python3
 """
-    Crossdomain tester
+    Copyright (c) 2023 Penterep Security s.r.o.
 
-    Copyright (c) 2020 HACKER Consulting s.r.o.
+    ptcrossd - crossdomain.xml misconfigurations testing tool
 
-    This program is free software: you can redistribute it and/or modify
+    ptcrossd is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
 
-    This program is distributed in the hope that it will be useful,
+    ptcrossd is distributed in the hope that it will be useful,
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+    along with ptcrossd.  If not, see <https://www.gnu.org/licenses/>.
 """
 
-__version__ = "0.0.2"
-
 import argparse
-import sys
+import re
+import sys; sys.path.append(__file__.rsplit("/", 1)[0])
 import urllib
 
-import defusedxml.ElementTree as ET
-import requests 
-
-import ptlibs.ptjsonlib as ptjsonlib
-import ptlibs.ptmisclib as ptmisclib
+import requests
+import defusedxml.ElementTree as DEFUSED_ET
 
+from _version import __version__
+from ptlibs import ptjsonlib, ptprinthelper, ptmisclib, ptnethelper
 
-class ptcrossd:
+class PtCrossd:
     def __init__(self, args):
-        self.use_json = args.json
-        self.ptjsonlib = ptjsonlib.ptjsonlib(self.use_json)
-        self.json_no = self.ptjsonlib.add_json("ptcrossd")
-
-        self.headers = ptmisclib.get_request_headers(args)
-        self.proxies = {"http": args.proxy, "https": args.proxy}
-        self.url = self.adjust_url(args.url)
-
-    def run(self):
-        ptmisclib.ptprint_(ptmisclib.out_ifnot(f"Testing: {self.url}", "TITLE", self.use_json))
-        response = self.get_response()
-        if response:
-            self.proccess_crossdomain(response)
-        ptmisclib.ptprint_(ptmisclib.out_if(self.ptjsonlib.get_all_json(), condition=self.use_json))
+        self.ptjsonlib  = ptjsonlib.PtJsonLib()
+        self.headers    = ptnethelper.get_request_headers(args)
+        self.use_json   = args.json
+        self.timeout    = args.timeout
+        self.cache      = args.cache
+        self.proxies    = {"http": args.proxy, "https": args.proxy}
+
+    def run(self, args):
+        rel_path, url = self._adjust_url(args.url)
+        ptprinthelper.ptprint(f"Testing: {url}", "TITLE", not self.use_json, colortext=True)
 
-    def get_response(self):
         try:
-            response = requests.get(self.url, headers=self.headers, proxies=self.proxies, verify=False, allow_redirects=False)
-            if response.status_code == 200:
-                data = {"url": self.url, "crossdomain_found": "True", "status_code": response.status_code, "xml_content": response.text}
-                self.ptjsonlib.set_status(self.json_no, "ok")
-                self.ptjsonlib.add_data(self.json_no, data)
-                return response
+            response, response_dump = ptmisclib.load_url_from_web_or_temp(url, method="GET", headers=self.headers, proxies=self.proxies, timeout=self.timeout, redirects=False, verify=False, cache=self.cache, dump_response=True)
+        except requests.RequestException:
+            self.ptjsonlib.end_error(f"Cannot connect to server", self.use_json)
+
+        if response.status_code == 200:
+            if response.headers.get("Access-Control-Allow-Origin"):
+                ptprinthelper.ptprint(f"Response Header: Access-Control-Allow-Origin: {response.headers.get('Access-Control-Allow-Origin')}", "INFO", not self.use_json)
+                if response.headers.get("Access-Control-Allow-Origin") == "*":
+                    self.ptjsonlib.add_vulnerability("PTWV-OPEN-CORS-HEADER", request=response_dump["request"], response=response_dump["response"])
+
+            if response.headers.get("Content-Type") in ["application/xml", "text/plain"]:
+                self.ptjsonlib.add_node(self.ptjsonlib.create_node_object("webpage", properties={"url": url, "name": rel_path[1:] if rel_path.startswith("/") else rel_path, "WebPageType": "crossdomain_xml"}))
+                self._process_crossdomain_xml(response, response_dump)
             else:
-                ptmisclib.end_error(f"crossdomain.xml not found", self.json_no, self.ptjsonlib, self.use_json)
-        except (requests.exceptions.MissingSchema, requests.exceptions.InvalidSchema):
-            ptmisclib.end_error("missing scheme", self.json_no, self.ptjsonlib, self.use_json)
-        except requests.exceptions.Timeout:
-            ptmisclib.end_error("timeout Error", self.json_no, self.ptjsonlib, self.use_json)
-        except Exception as e:
-            ptmisclib.end_error(f"server not reachable {e}", self.json_no, self.ptjsonlib, self.use_json)
+                self.ptjsonlib.end_error(f"Expected Content-Type is application/xml, got {response.headers.get('Content-Type')}", self.use_json)
+        else:
+            self.ptjsonlib.end_error(f"crossdomain.xml not found", self.use_json)
 
-    def proccess_crossdomain(self, response):
-        """Parse crossdomain file, check if vulnerable and set corresponding JSON"""
-        try:
-            tree = ET.fromstring(response.text)
-        except ET.ParseError:
-            ptmisclib.end_error("error Parsing XML", self.json_no, self.ptjsonlib, self.use_json)
-        except ET.EntitiesForbidden:
-            ptmisclib.end_error("forbidden entities found, quitting", self.json_no, self.ptjsonlib, self.use_json)
-
-        ptmisclib.ptprint_(ptmisclib.out_ifnot("File contents:\n", "TITLE", self.use_json))
-        ptmisclib.ptprint_(ptmisclib.out_ifnot(ptmisclib.get_colored_text(response.text, "ADDITIONS"), "", self.use_json))
-        vulnerable = None
+        if self.use_json:
+            ptprinthelper.ptprint(self.ptjsonlib.get_result_json())
 
+    def _process_crossdomain_xml(self, response, response_dump) -> None:
+        try:
+            tree = DEFUSED_ET.fromstring(response.text)
+        except DEFUSED_ET.ParseError:
+            self.ptjsonlib.end_error("Error parsing provided XML file", self.use_json)
+        except DEFUSED_ET.EntitiesForbidden:
+            self.ptjsonlib.end_error("Forbidden entities found, program will exit", self.use_json)
+
+        if not self.use_json:
+            import xml.etree.ElementTree as ET
+            element = ET.XML(response.text); ET.indent(element)
+            ptprinthelper.ptprint("XML content:", "TITLE", not self.use_json)
+            ptprinthelper.ptprint(ptprinthelper.get_colored_text(ET.tostring(element, encoding='unicode'), "INFO"), newline_above=True)
+
+        self._allow_access_from_test(tree, response_dump)
+
+    def _allow_access_from_test(self, tree, response_dump) -> None:
+        has_open_cors = False
+        has_non_secure_communication = False
         acf_elements = tree.findall("allow-access-from")
         if acf_elements:
-            for acf in acf_elements:
-                if acf.attrib["domain"] and acf.attrib["domain"] == "*":
-                    vulnerable = True
-            if vulnerable:
-                ptmisclib.ptprint_(ptmisclib.out_ifnot("file is vulnerable to open policy", "VULN", self.use_json))
-                self.ptjsonlib.set_vulnerable(self.json_no, "True")
-            else:
-                ptmisclib.ptprint_(ptmisclib.out_ifnot("no vulnerabilities found", "NOTVULN", self.use_json))
-                self.ptjsonlib.set_vulnerable(self.json_no, "False")
+            for acf_element in acf_elements:
+                if "domain" in acf_element.keys() and acf_element.attrib["domain"] == "*":
+                    has_open_cors = True
+                if "secure" in acf_element.keys() and not acf_element.attrib["secure"]:
+                    has_non_secure_communication = True
+            if has_open_cors:
+                ptprinthelper.ptprint("Open CORS vulnerability detected", "VULN", not self.use_json, newline_above=True)
+                self.ptjsonlib.add_vulnerability("PTWV-OPEN-CORS", request=response_dump["request"], response=response_dump["response"])
+            if has_non_secure_communication:
+                ptprinthelper.ptprint("Non-secure communication detected", "VULN", not self.use_json, newline_above=True)
+                self.ptjsonlib.add_vulnerability("PTWV-NON-SECURE-CORS", request=response_dump["request"], response=response_dump["response"])
         else:
-            ptmisclib.ptprint_(ptmisclib.out_ifnot("allow-access-from element not found", "INFO", self.use_json))
-            self.ptjsonlib.set_vulnerable(self.json_no, "False")
+            self.ptjsonlib.end_error("No allow-access-from elements were found", self.use_json)
 
-    def adjust_url(self, url):
-        ext = urllib.parse.urlparse(url)
-        path = ext.path
-        if not ext.path.endswith("/crossdomain.xml"):
-            if not ext.path.endswith("/"):
-                path = path + "/"
-            path = path + "crossdomain.xml"
-        return ext.scheme + "://" + ext.netloc + path
+
+    def _adjust_url(self, url: str) -> tuple[str, str]:
+        parsed_url = urllib.parse.urlparse(url)
+        if not re.match("https?$", parsed_url.scheme):
+            self.ptjsonlib.end_error("Missing or wrong scheme - only HTTP/HTTPS schemas are supported", self.use_json)
+        if not parsed_url.netloc:
+            self.ptjsonlib.end_error("Invalid URL provided", self.use_json)
+
+        if not parsed_url.path.endswith("/crossdomain.xml"):
+            if parsed_url.path in ["/", ""]:
+                parsed_url = parsed_url._replace(path="/crossdomain.xml")
+            else:
+                parsed_url = parsed_url._replace(path='/'.join([i for i in parsed_url.path.split("/") if i]) + "/crossdomain.xml")
+        return (parsed_url.path, urllib.parse.urlunparse((parsed_url.scheme, parsed_url.netloc, parsed_url.path, "", "", "")))
 
 
 def get_help():
     return [
-        {"description": ["Crossdomain.xml Testing Tool"]},
+        {"description": ["crossdomain.xml misconfigurations testing tool"]},
         {"usage": ["ptcrossd <options>"]},
         {"usage_example": [
             "ptcrossd -u https://www.example.com/crossdomain.xml",
             "ptcrossd -u https://www.example.com/"
         ]},
         {"options": [
             ["-u",  "--url",                    "<url>",            "Connect to URL"],
             ["-p",  "--proxy",                  "<proxy>",          "Set proxy (e.g. http://127.0.0.1:8080)"],
+            ["-T",  "--timeout",                "<timeout>",        "Set timeout (default to 10)"],
             ["-c",  "--cookie",                 "<cookie>",         "Set cookie"],
+            ["-ua", "--user-agent",             "<user-agent>",     "Set User-Agent header"],
             ["-H",  "--headers",                "<header:value>",   "Set custom header(s)"],
-            ["-ua",  "--user-agent",            "<user-agent>",     "Set User-Agent header"],
-            ["-j",  "--json",                   "",                 "Output in JSON format"],
+            ["-C",  "--cache",                  "",                 "Cache requests (load from tmp in future)"],
             ["-v",  "--version",                "",                 "Show script version and exit"],
-            ["-h",  "--help",                   "",                 "Show this help message and exit"]
+            ["-h",  "--help",                   "",                 "Show this help message and exit"],
+            ["-j",  "--json",                   "",                 "Output in JSON format"],
         ]
-        }]                                                 
+        }]
 
 
 def parse_args():
     parser = argparse.ArgumentParser(add_help="False")
-    parser.add_argument("-u", "--url", type=str, required=True)
-    parser.add_argument("-p", "--proxy", type=str)
-    parser.add_argument("-c", "--cookie", type=str)
-    parser.add_argument("-H", "--headers", type=ptmisclib.pairs, nargs="+")
-    parser.add_argument("-ua", "--user-agent", type=str, default="Penterep Tools")
-    parser.add_argument("-j", "--json", action="store_true")
-    parser.add_argument("-v", "--version", action="version", version=f"{SCRIPTNAME} {__version__}")
-    
+    parser.add_argument("-u",  "--url",         type=str, required=True)
+    parser.add_argument("-p",  "--proxy",       type=str)
+    parser.add_argument("-c",  "--cookie",      type=str)
+    parser.add_argument("-ua", "--user-agent",  type=str, default="Penterep Tools")
+    parser.add_argument("-T",  "--timeout",     type=int, default=10)
+    parser.add_argument("-H",  "--headers",     type=ptmisclib.pairs, nargs="+")
+    parser.add_argument("-j",  "--json",        action="store_true")
+    parser.add_argument("-C",  "--cache",       action="store_true")
+    parser.add_argument("-v",  "--version",     action="version", version=f"{SCRIPTNAME} {__version__}")
+
     if len(sys.argv) == 1 or "-h" in sys.argv or "--help" in sys.argv:
-        ptmisclib.help_print(get_help(), SCRIPTNAME, __version__)
+        ptprinthelper.help_print(get_help(), SCRIPTNAME, __version__)
         sys.exit(0)
 
     args = parser.parse_args()
-    ptmisclib.print_banner(SCRIPTNAME, __version__, args.json)
+    ptprinthelper.print_banner(SCRIPTNAME, __version__, args.json)
     return args
 
 
 def main():
     global SCRIPTNAME
     SCRIPTNAME = "ptcrossd"
     requests.packages.urllib3.disable_warnings()
     requests.packages.urllib3.util.ssl_.DEFAULT_CIPHERS += ':HIGH:!DH:!aNULL'
-
     args = parse_args()
-    script = ptcrossd(args)
-    script.run()
+    script = PtCrossd(args)
+    script.run(args)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ptcrossd-0.0.2/ptcrossd.egg-info/PKG-INFO` & `ptcrossd-1.0.0/ptcrossd.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,78 +1,98 @@
 Metadata-Version: 2.1
 Name: ptcrossd
-Version: 0.0.2
-Summary: Crossdomain.xml Testing Tool
+Version: 1.0.0
+Summary: crossdomain.xml misconfigurations testing tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3+
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
+Classifier: Topic :: Security
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)
+[![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
+
 
 # PTCROSSD
-> Crossdomain.xml Testing Tool
+
+> crossdomain.xml misconfigurations testing tool
 
 ## Installation
 ```
 pip install ptcrossd
 ```
 
 ## Add to PATH
+If you cannot invoke the script in your terminal, its probably because its not in your PATH. Fix it by running commands below.
+
+> Add to PATH for Bash
 ```bash
-# If you cannot invoke the script in your terminal, its probably because its not in your PATH. Fix it by running commands below.
 echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.bashrc
 source ~/.bashrc
 ```
 
+> Add to PATH for ZSH
+```bash
+echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshhrc
+source ~/.zshhrc
+```
+
+
 ## Usage examples
 ```
-$ ptcrossd.py -u https://www.example.com/crossdomain.xml
-$ ptcrossd.py -u https://www.example.com/
+ptcrossd -u https://www.example.com/crossdomain.xml
+ptcrossd -u https://www.example.com/
 ```
 
 ## Options
+
 ```
 -u   --url         <url>           Connect to URL
 -p   --proxy       <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
+-T   --timeout     <timeout>       Set timeout (default to 10)
 -c   --cookie      <cookie>        Set cookie
--H   --headers     <header:value>  Set custom header(s)
 -ua  --user-agent  <user-agent>    Set User-Agent header
--j   --json                        Output in JSON format
+-H   --headers     <header:value>  Set custom header(s)
+-C   --cache                       Cache requests (load from tmp in future)
 -v   --version                     Show script version and exit
 -h   --help                        Show this help message and exit
+-j   --json                        Output in JSON format
 ```
 
 ## Dependencies
-    - defusedxml
-    - requests
-    - ptlibs
+```
+defusedxml
+requests
+ptlibs
+```
 
 ## Version History
-- 0.0.1 - 0.0.2
-    - Alpha release
-
-## Licence
+```
+1.0.0
+    - updated for ptlibs 1.0.0
+    - code refactorization
+0.0.1 - 0.0.2
+    - Alpha releases
+```
+## License
 
-Copyright (c) 2020 HACKER Consulting s.r.o.
+Copyright (c) 2023 Penterep Security s.r.o.
 
 ptcrossd is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 ptcrossd is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with ptcrossd. If not, see https://www.gnu.org/licenses/.
 
 ## Warning
 
 You are only allowed to run the tool against the websites which
 you have been given permission to pentest. We do not accept any
 responsibility for any damage/harm that this application causes to your
 computer, or your network. Penterep is not responsible for any illegal
 or malicious use of this code. Be Ethical!
-
```

### Comparing `ptcrossd-0.0.2/setup.py` & `ptcrossd-1.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import setuptools
+from ptcrossd._version import __version__
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ptcrossd",
-    version="0.0.2",
-    description="Crossdomain.xml Testing Tool",
+    description="crossdomain.xml misconfigurations testing tool",
+    version=__version__,
     author="Penterep",
     author_email="info@penterep.com",
     url="https://www.penterep.com/",
     license="GPLv3+",
     packages=setuptools.find_packages(),
     classifiers=[
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Environment :: Console"
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: Implementation :: CPython",
+        "Environment :: Console",
+        "Topic :: Security",
+        "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)"
     ],
     python_requires='>=3.6',
-    install_requires=["ptlibs>=0.0.6", "requests", "defusedxml"],
+    install_requires=["ptlibs>=1,<2", "requests", "defusedxml"],
     entry_points = {'console_scripts': ['ptcrossd = ptcrossd.ptcrossd:main']},
     include_package_data= True,
     long_description=long_description,
     long_description_content_type="text/markdown",
 )
```

