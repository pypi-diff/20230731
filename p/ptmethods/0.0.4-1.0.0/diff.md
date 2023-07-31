# Comparing `tmp/ptmethods-0.0.4.tar.gz` & `tmp/ptmethods-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptmethods-0.0.4.tar", last modified: Mon Mar 28 16:38:37 2022, max compression
+gzip compressed data, was "ptmethods-1.0.0.tar", last modified: Mon Jul 31 19:00:18 2023, max compression
```

## Comparing `ptmethods-0.0.4.tar` & `ptmethods-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2022-03-28 16:38:37.199471 ptmethods-0.0.4/
--rw-r--r--   0 kali      (1000) kali      (1000)    35823 2021-12-17 14:07:30.000000 ptmethods-0.0.4/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     3582 2022-03-28 16:38:37.199471 ptmethods-0.0.4/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     3236 2022-03-28 16:38:15.000000 ptmethods-0.0.4/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2022-03-28 16:38:37.199471 ptmethods-0.0.4/ptmethods/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2021-12-17 14:07:30.000000 ptmethods-0.0.4/ptmethods/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)    13444 2022-03-28 16:37:55.000000 ptmethods-0.0.4/ptmethods/ptmethods.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2022-03-28 16:38:37.199471 ptmethods-0.0.4/ptmethods.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     3582 2022-03-28 16:38:37.000000 ptmethods-0.0.4/ptmethods.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      271 2022-03-28 16:38:37.000000 ptmethods-0.0.4/ptmethods.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2022-03-28 16:38:37.000000 ptmethods-0.0.4/ptmethods.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       56 2022-03-28 16:38:37.000000 ptmethods-0.0.4/ptmethods.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       16 2022-03-28 16:38:37.000000 ptmethods-0.0.4/ptmethods.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       10 2022-03-28 16:38:37.000000 ptmethods-0.0.4/ptmethods.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2022-03-28 16:38:37.199471 ptmethods-0.0.4/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)      782 2022-03-28 16:37:44.000000 ptmethods-0.0.4/setup.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-31 19:00:18.162987 ptmethods-1.0.0/
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    35823 2023-02-16 20:42:08.000000 ptmethods-1.0.0/LICENSE
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3909 2023-07-31 19:00:18.162987 ptmethods-1.0.0/PKG-INFO
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3453 2023-07-31 18:59:07.000000 ptmethods-1.0.0/README.md
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-31 19:00:18.158987 ptmethods-1.0.0/ptmethods/
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-02-16 20:42:08.000000 ptmethods-1.0.0/ptmethods/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       21 2023-04-14 08:08:26.000000 ptmethods-1.0.0/ptmethods/_version.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    14643 2023-07-31 18:56:57.000000 ptmethods-1.0.0/ptmethods/ptmethods.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-31 19:00:18.162987 ptmethods-1.0.0/ptmethods.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3909 2023-07-31 19:00:18.000000 ptmethods-1.0.0/ptmethods.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      293 2023-07-31 19:00:18.000000 ptmethods-1.0.0/ptmethods.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-07-31 19:00:18.000000 ptmethods-1.0.0/ptmethods.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       55 2023-07-31 19:00:18.000000 ptmethods-1.0.0/ptmethods.egg-info/entry_points.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       22 2023-07-31 19:00:18.000000 ptmethods-1.0.0/ptmethods.egg-info/requires.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       10 2023-07-31 19:00:18.000000 ptmethods-1.0.0/ptmethods.egg-info/top_level.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-07-31 19:00:18.162987 ptmethods-1.0.0/setup.cfg
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)      973 2023-04-17 09:01:26.000000 ptmethods-1.0.0/setup.py
```

### Comparing `ptmethods-0.0.4/LICENSE` & `ptmethods-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ptmethods-0.0.4/PKG-INFO` & `ptmethods-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,103 +1,111 @@
 Metadata-Version: 2.1
 Name: ptmethods
-Version: 0.0.4
-Summary: HTTP Methods Testing Tool
+Version: 1.0.0
+Summary: HTTP methods testing tool
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
 
 # PTMETHODS
-> HTTP Methods Testing Tool
+> HTTP methods testing tool
 
-- Script retrieves methods offered by server from *OPTIONS* request
-- Script sends GET, POST, PUT, PATCH, DELETE, OPTIONS, HEAD, TRACE, DEBUG headers and retrieves it's response.
-- Script tests CONNECT method by connecting to url at ports 80, 443
-- Script tests if domain can be used as proxy.
+- Script retrieves methods offered by server from OPTIONS request
+- Script sends GET, POST, PUT, PATCH, DELETE, OPTIONS, HEAD, TRACE, DEBUG, FOO headers and returns server response
+- Script tests CONNECT method by connecting to URL at ports 80, 443
+- Script tests if domain can be used as a proxy
 
 ## Installation
-
 ```
 pip install ptmethods
 ```
 
-### Add to PATH
+## Add to PATH
 If you cannot invoke the script in your terminal, its probably because its not in your PATH. Fix it by running commands below.
 
-Add to path for BASH
+> Add to PATH for Bash
 ```bash
 echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.bashrc
 source ~/.bashrc
 ```
-Add to path for ZSH
+
+> Add to PATH for ZSH
 ```bash
 echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshhrc
 source ~/.zshhrc
 ```
 
 ## Usage examples
 Optimally use this script against homepage, any image and sources protected by HTTP authentication
 ```
 ptmethods -u https://www.example.com/
 ptmethods -u https://www.example.com/ -r
 ptmethods -u https://www.example.com/index.php -sr -sh
-ptmethods -u https://www.example.com/index.php -c PHPSESSID
+ptmethods -u https://www.example.com/index.php -c PHPSESSID=abcdef
 ptmethods -f URL_list.txt
 ```
 
 ## Options
 ```
 -u   --url            <url>           Test specified URL
--f   --file           <file>          Load list of URLs from file
+-f   --file           <file>          Load URLs from file
 -sh  --show-headers                   Show response headers
 -sr  --show-response                  Show response text
 -p   --proxy          <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
+-T   --timeout                        Set timeout (default 10)
+-c   --cookie         <cookie>        Set cookie
 -ua  --user-agent     <ua>            Set User-Agent header
 -H   --headers        <header:value>  Set custom header(s)
--c   --cookie         <cookie>        Set cookie(s)
 -r   --redirects                      Follow redirects (default False)
--j   --json                           Output in JSON format
+-c   --cache                          Cache requests (load from tmp in future)
 -v   --version                        Show script version and exit
 -h   --help                           Show this help message and exit
+-j   --json                           Output in JSON format
 ```
 
 ## Dependencies
 ```
 requests
 ptlibs
 ```
 
 ## Version History
-    0.0.2 - 0.0.4
-        - Implemented proxy test
-        - Implemented CONNECT tests
-    0.0.1 - 0.0.3
-        Alpha releases
+```
+1.0.0
+    - Support for ptlibs v1.0.0
+    - Code refactorization
+0.0.2 - 0.0.4
+    - Implemented proxy and connect tests
+0.0.1 - 0.0.3
+    Alpha releases
+```
 
-## Licence
 
-Copyright (c) 2020 HACKER Consulting s.r.o.
+## License
+
+Copyright (c) 2023 Penterep Security s.r.o.
 
 ptmethods is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 ptmethods is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with ptmethods. If not, see https://www.gnu.org/licenses/.
 
 ## Warning
 
 You are only allowed to run the tool against the websites which
 you have been given permission to pentest. We do not accept any
 responsibility for any damage/harm that this application causes to your
 computer, or your network. Penterep is not responsible for any illegal
 or malicious use of this code. Be Ethical!
-
```

### Comparing `ptmethods-0.0.4/README.md` & `ptmethods-1.0.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,79 +1,87 @@
-![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)
+[![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
+
 
 # PTMETHODS
-> HTTP Methods Testing Tool
+> HTTP methods testing tool
 
-- Script retrieves methods offered by server from *OPTIONS* request
-- Script sends GET, POST, PUT, PATCH, DELETE, OPTIONS, HEAD, TRACE, DEBUG headers and retrieves it's response.
-- Script tests CONNECT method by connecting to url at ports 80, 443
-- Script tests if domain can be used as proxy.
+- Script retrieves methods offered by server from OPTIONS request
+- Script sends GET, POST, PUT, PATCH, DELETE, OPTIONS, HEAD, TRACE, DEBUG, FOO headers and returns server response
+- Script tests CONNECT method by connecting to URL at ports 80, 443
+- Script tests if domain can be used as a proxy
 
 ## Installation
-
 ```
 pip install ptmethods
 ```
 
-### Add to PATH
+## Add to PATH
 If you cannot invoke the script in your terminal, its probably because its not in your PATH. Fix it by running commands below.
 
-Add to path for BASH
+> Add to PATH for Bash
 ```bash
 echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.bashrc
 source ~/.bashrc
 ```
-Add to path for ZSH
+
+> Add to PATH for ZSH
 ```bash
 echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshhrc
 source ~/.zshhrc
 ```
 
 ## Usage examples
 Optimally use this script against homepage, any image and sources protected by HTTP authentication
 ```
 ptmethods -u https://www.example.com/
 ptmethods -u https://www.example.com/ -r
 ptmethods -u https://www.example.com/index.php -sr -sh
-ptmethods -u https://www.example.com/index.php -c PHPSESSID
+ptmethods -u https://www.example.com/index.php -c PHPSESSID=abcdef
 ptmethods -f URL_list.txt
 ```
 
 ## Options
 ```
 -u   --url            <url>           Test specified URL
--f   --file           <file>          Load list of URLs from file
+-f   --file           <file>          Load URLs from file
 -sh  --show-headers                   Show response headers
 -sr  --show-response                  Show response text
 -p   --proxy          <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
+-T   --timeout                        Set timeout (default 10)
+-c   --cookie         <cookie>        Set cookie
 -ua  --user-agent     <ua>            Set User-Agent header
 -H   --headers        <header:value>  Set custom header(s)
--c   --cookie         <cookie>        Set cookie(s)
 -r   --redirects                      Follow redirects (default False)
--j   --json                           Output in JSON format
+-c   --cache                          Cache requests (load from tmp in future)
 -v   --version                        Show script version and exit
 -h   --help                           Show this help message and exit
+-j   --json                           Output in JSON format
 ```
 
 ## Dependencies
 ```
 requests
 ptlibs
 ```
 
 ## Version History
-    0.0.2 - 0.0.4
-        - Implemented proxy test
-        - Implemented CONNECT tests
-    0.0.1 - 0.0.3
-        Alpha releases
+```
+1.0.0
+    - Support for ptlibs v1.0.0
+    - Code refactorization
+0.0.2 - 0.0.4
+    - Implemented proxy and connect tests
+0.0.1 - 0.0.3
+    Alpha releases
+```
+
 
-## Licence
+## License
 
-Copyright (c) 2020 HACKER Consulting s.r.o.
+Copyright (c) 2023 Penterep Security s.r.o.
 
 ptmethods is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 ptmethods is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with ptmethods. If not, see https://www.gnu.org/licenses/.
```

### Comparing `ptmethods-0.0.4/ptmethods/ptmethods.py` & `ptmethods-1.0.0/ptmethods/ptmethods.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,268 +1,280 @@
 #!/usr/bin/python3
 """
-    ptmethods - HTTP Methods Testing Tool
+    Copyright (c) 2023 Penterep Security s.r.o.
 
-    Copyright (c) 2020 HACKER Consulting s.r.o.
+    ptmethod - HTTP methods testing tool
 
-    This program is free software: you can redistribute it and/or modify
+    ptmethods is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
 
-    This program is distributed in the hope that it will be useful,
+    ptmethods is distributed in the hope that it will be useful,
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+    along with ptmethods.  If not, see <https://www.gnu.org/licenses/>.
 """
 
-__version__ = "0.0.4"
 
 import argparse
 import re
-import sys
+import sys; sys.path.append(__file__.rsplit("/", 1)[0])
 import urllib
 
 import requests
-from ptlibs import ptjsonlib, ptmisclib
 
+from _version import __version__
+from ptlibs import ptjsonlib, ptmisclib, ptnethelper, ptprinthelper
 
-class ptmethods:
+
+class PtMethods:
     def __init__(self, args):
-        self.use_json = args.json
-        self.ptjsonlib = ptjsonlib.ptjsonlib(self.use_json)
-        self.json_no = self.ptjsonlib.add_json(SCRIPTNAME)
-        self.ptjsonlib.add_data(self.json_no, {"urls": []})
-        self.headers = ptmisclib.get_request_headers(args)
-        self.proxy = {"http": args.proxy, "https": args.proxy}
-        self.redirects = args.redirects
-        self.show_headers = args.show_headers
-        self.show_response = args.show_response
-
-        if not (args.file or args.url):
-            ptmisclib.end_error("--url or --file parameter required", self.json_no, self.ptjsonlib, self.use_json)
-        elif args.url and args.file:
-            ptmisclib.end_error("Cannot use both --url and --file parameters together", self.json_no, self.ptjsonlib, self.use_json)
+        self.ptjsonlib          = ptjsonlib.PtJsonLib()
+        self.headers            = ptnethelper.get_request_headers(args)
+        self.proxies            = {"http": args.proxy, "https": args.proxy}
+        self.use_json           = args.json
+        self.redirects          = args.redirects
+        self.cache              = args.cache
+        self.timeout            = args.timeout
+        self.show_headers       = args.show_headers
+        self.show_response      = args.show_response
+
         try:
             self.url_list = ptmisclib.read_file(args.file) if args.file else args.url
         except FileNotFoundError:
-            ptmisclib.end_error("File not found", self.json_no, self.ptjsonlib, self.use_json)
-        ptmisclib.check_connectivity()
+            self.ptjsonlib.end_error("File not found", self.use_json)
 
-    def parse_url(self, url):
-        o = urllib.parse.urlparse(url)
-        if o.scheme not in ["http", "https"]:
-             raise Exception("Missing or unsupported scheme")
-        if ":" in o.netloc:
-            split_obj = o.netloc.split(":")
-            port = split_obj[-1]
-            o = o._replace(netloc=split_obj[0])
-        else:
-            port = "443" if o.scheme == "https" else "80"
-        return port, urllib.parse.urlunparse(o)
+        if len(self.url_list) > 1 and self.use_json:
+                self.ptjsonlib.end_error("Cannot test more than 1 URL while --json parameter is present", self.use_json)
 
     def run(self):
-        """Main function"""
-        for url in self.url_list:
-            ptmisclib.ptprint_(ptmisclib.out_title_ifnot(f"Testing: {url}", self.use_json), end="\n")
-            self.data = {"url": url, "status": "null", "vulnerable:": "null", "options": {}, "methods": {}}
+        """Main method"""
+        for index, url in enumerate(self.url_list):
+            ptprinthelper.ptprint(f"Testing: {url}", "TITLE", not self.use_json, colortext=True)
             try:
-                port, url = self.parse_url(url)
-                self.port = port
-                options = self.get_options(url)
-                methods = self.check_methods(url)
-                connect_test = self.test_connect_method(url)
-                proxy_test = self.check_proxy_method(url)
-                localhost_connect_test = self.test_connect_method_localhost(url) if connect_test else None
-                localhost_proxy_test = self.check_proxy_localhost(url) if proxy_test else None
-                self.print_result(options, methods, proxy_test, connect_test, localhost_proxy_test, localhost_connect_test)
-                self.data.update({
-                    "status": "ok",
-                    "options": options,
-                    "methods": methods,
-                    "proxy_test": proxy_test,
-                    "connect_test": connect_test,
-                    "localhost_proxy_test": localhost_proxy_test,
-                    "localhost_connect_test": localhost_connect_test,
-                    })
-                if self.use_json:
-                    self.ptjsonlib.json_list[self.json_no]["data"]["urls"].append(self.data)
-            except Exception as e:
+                self.port, url = self._parse_url(url)
+                self._run_tests(url)
+            except (ValueError, requests.exceptions.RequestException) as e:
                 if len(self.url_list) > 1:
-                    self.data.update({"status": "error", "message": str(e)})
-                    if self.use_json:
-                        self.ptjsonlib.json_list[self.json_no]["data"]["urls"].append(self.data)
-                    ptmisclib.ptprint_(ptmisclib.out_ifnot(f"Error: {e}, skipping. \n", "ERROR", self.use_json))
+                    ptprinthelper.ptprint(f"Error: {e}", "ERROR", not self.use_json, end="\n\n" if not index+1 == len(self.url_list) else "\n")
                     continue
                 else:
-                    ptmisclib.end_error(str(e), self.json_no, self.ptjsonlib, self.use_json)
-        ptmisclib.ptprint_(ptmisclib.out_if(self.ptjsonlib.get_all_json(), "", self.use_json))
+                    self.ptjsonlib.end_error(f"{e}", self.use_json)
 
-    def get_response(self, url, method, proxy=None):
-        if proxy is None:
-            proxy = self.proxy
-        r = requests.request(method, url, allow_redirects=self.redirects, headers=self.headers, proxies=proxy, verify=False, timeout=3)
-        return r
+        if self.use_json:
+            self.ptjsonlib.set_status("ok")
+            ptprinthelper.ptprint(self.ptjsonlib.get_result_json(), "", self.use_json)
 
-    def test_connect_method(self, url):
+    def _run_tests(self, url: str):
+        """Runs all the tests"""
         try:
-            r = self.get_response("https://www.example.com", "GET", {"https": url+":"+str(self.port)})
-            if re.search(r"<title>Example Domain</title>", r.text):
-                return True
-        except:
-            pass
-        return False
-
-    def test_connect_method_localhost(self, url):
-        r_localhost = self.get_response("https://127.0.0.1", "GET", {"https": url+":"+str(self.port)})
-        print(r_localhost, r_localhost.text)
-        title = re.search(r"<title.*?>([\s\S]*?)</title>", r_localhost.text)
-        print(title)
-        if title:
-            return title[1]
-        else:
-            return 'No title'
+            options       = self._get_options(url)
+            methods       = self._check_methods(url)
+            connect_test  = self._test_connect_method(url)
+            proxy_test    = self._check_proxy_method(url)
+            self._print_results(url, options, methods, proxy_test, connect_test)
+        except requests.exceptions.RequestException as e:
+            raise e
 
-    def check_proxy_localhost(self, url):
-        r_localhost = self.get_response("http://127.0.0.1", "GET", {"http": url+":"+str(self.port)})
-        title = re.search(r"<title.*?>([\s\S]*?)</title>", r_localhost.text)
-        if title:
-            return title[1]
-        else:
-            return 'No title'
+    def _test_connect_method(self, url):
+        try:
+            response = self._get_response("https://www.example.com", "GET", proxies={"https": url+":"+self.port})
+        except requests.RequestException as e:
+            return False
+        if re.search(r"<title>Example Domain</title>", response.text):
+            try:
+                response_localhost = self._get_response("https://127.0.0.1", "GET", {"https": url+":"+self.port})
+            except requests.RequestException as e:
+                title = "Error retrieving title from localhost"
+                return title
+            title = re.search(r"<title.*?>([\s\S]*?)</title>", response_localhost.text)
+            if title:
+                title = title.groups()[0]
+            return title
 
-    def check_proxy_method(self, url):
-        r = self.get_response("http://www.example.com", "GET", {"http": url+":"+str(self.port)})
-        if re.search(r"<title>Example Domain</title>", r.text):
-            return True
-        else:
+    def _check_proxy_method(self, url):
+        try:
+            r, response_dump = self._get_response("http://www.example.com", "GET", {"http": url+":"+self.port}, dump_response=True)
+        except requests.RequestException as e:
             return False
+        if re.search(r"<title>Example Domain</title>", r.text):
+            try:
+                response_localhost = self._get_response("http://127.0.0.1", "GET", {"http": url+":"+self.port})
+            except requests.RequestException as e:
+                title = "Error retrieving title from localhost"
+                return title
+            title = re.search(r"<title.*?>([\s\S]*?)</title>", response_localhost.text)
+            if title:
+                title = title.groups()[0]
+            self.ptjsonlib.add_vulnerability("PTWVPROXY", request=response_dump["request"], response=response_dump["response"], note=f"Title of localhost when proxy is used: {title}")
+            return title
 
-    def get_options(self, url):
-        response = self.get_response(url, "OPTIONS")
-        if "allow" in response.headers:
-            allowed_methods = response.raw.headers.getlist('allow')
-            allowed_methods = "".join(allowed_methods).split(",")
-            return allowed_methods
-        else:
-            return ["None"]
+    def _get_options(self, url):
+        try:
+            response = self._get_response(url, "OPTIONS")
+            if "Allow" in response.headers:
+                allowed_methods = response.headers["Allow"].split(", ")
+                return allowed_methods
+            else:
+                return ["None"]
+        except requests.exceptions.RequestException as e:
+            return ["error"]
 
-    def check_methods(self, url):
-        METHOD_LIST = ["GET", "POST", "PUT", "PATCH", "DELETE", "OPTIONS", "HEAD", "TRACE", "DEBUG", "FOO"]
+    def _check_methods(self, url):
+        """Check url for available methods"""
         methods_result = {"available_methods": [], "not_available_methods": []}
-        for method in METHOD_LIST:
+        for method in ["GET", "POST", "PUT", "PATCH", "DELETE", "OPTIONS", "HEAD", "TRACE", "DEBUG", "FOO"]:
+            ptprinthelper.ptprint(f"Testing method: {method} {' '*10}", "TITLE", self.use_json == False, end="\r")
             try:
-                response = self.get_response(url, method)
-            except Exception as e:
-                methods_result["not_available_methods"].append({"method": method, "status": 'error', "headers": [], "response": []})
+                response, response_dump = self._get_response(url, method, dump_response=True)
+            except requests.RequestException as e:
+                methods_result["not_available_methods"].append({"method": method, "status": 'error', "location": None, "headers": [], "response": []})
                 continue
-            json_data = {"method": method, "status": response.status_code, "headers": [], "response": []}
+            method_data = {"method": method, "status": response.status_code, "location": None, "headers": [], "response": []}
+            if response.headers.get("location"):
+                method_data.update({"location": response.headers.get("location")})
             if self.show_headers:
-                json_data["headers"].append(dict(response.headers))
+                method_data["headers"].append(dict(response.headers))
             if self.show_response:
-                json_data["response"].append(response.text)
+                method_data["response"].append(response.text)
             if response.status_code < 400:
-                methods_result["available_methods"].append(json_data)
+                methods_result["available_methods"].append(method_data)
+                self.ptjsonlib.add_node(self.ptjsonlib.create_node_object("httpMethod", properties={"name": method, "httpMethodType": method}))
+                if method in ["TRACE"]:
+                    self.ptjsonlib.add_vulnerability("PTWVHTTPTRACE", request=response_dump["request"], response=response_dump["response"])
             else:
-                methods_result["not_available_methods"].append(json_data)
+                methods_result["not_available_methods"].append(method_data)
+        ptprinthelper.ptprint(f"{' '*30}", "", self.use_json == False, end="\r")
+
         return methods_result
 
-    def print_result(self, options, methods, proxy_method, connect_method, localhost_proxy_test, localhost_connect_test):
-        ptmisclib.ptprint_(ptmisclib.out_ifnot(f"Response for OPTIONS: {', '.join(options)}", "INFO", self.use_json))
+    def _print_results(self, url, options, methods, proxy_method, connect_method):
+        ptprinthelper.ptprint(f"Response for OPTIONS: {', '.join(options)}", "INFO", self.use_json == False)
 
-        for key, value in methods.items(): #
-            ptmisclib.ptprint_(ptmisclib.out_ifnot(f" ", "", self.use_json))
-            ptmisclib.ptprint_(ptmisclib.out_ifnot(f"{key.capitalize().replace('_',' ')}:", "INFO", self.use_json))
+        for key, value in methods.items():
+            ptprinthelper.ptprint(f"{key.capitalize().replace('_',' ')}:", "INFO", self.use_json == False, newline_above=True)
             if not value:
-                ptmisclib.ptprint_(ptmisclib.out_ifnot(f"    None", "", self.use_json))
-            for idx, dictionary in enumerate(value):
-                ptmisclib.ptprint_(ptmisclib.out_ifnot(f"    {dictionary['method']}{' '*(9-len(dictionary['method']))}[{dictionary['status']}]", "", self.use_json))
-                """
-                if not self.show_headers:
-                    ptmisclib.ptprint_(ptmisclib.out_ifnot(f" ", "", self.use_json))
-                """
+                ptprinthelper.ptprint(f"    None", "", self.use_json == False)
+            for dictionary in value:
+                ptprinthelper.ptprint(f"    {dictionary['method']}{' '*(9-len(dictionary['method']))}[{dictionary['status']}]", "", self.use_json == False, "")
+                if dictionary["location"]:
+                    ptprinthelper.ptprint(f"        -> {dictionary['location']}", "", self.use_json == False)
+                else:
+                    ptprinthelper.ptprint(f" ", "", self.use_json == False, end="\n")
                 if self.show_headers:
                     for header, value in dictionary["headers"][0].items():
-                        ptmisclib.ptprint_(ptmisclib.out_ifnot(ptmisclib.get_colored_text(f'      {header} : {value}', 'ADDITIONS'), "", self.use_json))
+                        ptprinthelper.ptprint(f'      {header} : {value}', 'ADDITIONS', self.use_json == False, colortext=True)
                 if self.show_headers and self.show_response:
-                    ptmisclib.ptprint_(ptmisclib.out_ifnot(f" ", "", self.use_json))
+                    ptprinthelper.ptprint(f" ", "", self.use_json == False)
                 if self.show_response:
-                    ptmisclib.ptprint_(ptmisclib.out_ifnot(ptmisclib.get_colored_text(f'{"".join(dictionary["response"])}', 'ADDITIONS'), "", self.use_json))
-        ptmisclib.ptprint_(ptmisclib.out_ifnot(f" ", "", self.use_json))
+                    ptprinthelper.ptprint(f'{"".join(dictionary["response"])}', 'ADDITIONS', self.use_json == False, colortext=True)
+
+        ptprinthelper.ptprint(f" ", "", self.use_json == False)
         if proxy_method:
-            ptmisclib.ptprint_(ptmisclib.out_ifnot(f"Proxy mode is allowed", "VULN", self.use_json))
-            ptmisclib.ptprint_(ptmisclib.out_ifnot(f"Title of localhost via proxy: {localhost_proxy_test}", "VULN", self.use_json))
+            ptprinthelper.ptprint(f"Proxy mode is allowed", "VULN", self.use_json == False)
+            ptprinthelper.ptprint(f"Title of localhost via proxy: {proxy_method}", "VULN", self.use_json == False)
         else:
-            ptmisclib.ptprint_(ptmisclib.out_ifnot(f"Proxy mode is not allowed", "NOTVULN", self.use_json))
+            ptprinthelper.ptprint(f"Proxy mode is not allowed", "NOTVULN", self.use_json == False)
+
         if connect_method:
-            ptmisclib.ptprint_(ptmisclib.out_ifnot(f"CONNECT method at port {self.port} is allowed", "VULN", self.use_json))
-            ptmisclib.ptprint_(ptmisclib.out_ifnot(f"Title of localhost via CONNECT method: {localhost_connect_test}", "VULN", self.use_json))
+            ptprinthelper.ptprint(f"CONNECT method at port {self.port} is allowed", "VULN", self.use_json == False)
+            ptprinthelper.ptprint(f"Title of localhost via CONNECT method: {connect_method}", "VULN", self.use_json == False)
         else:
-            ptmisclib.ptprint_(ptmisclib.out_ifnot(f"CONNECT method at port {self.port} is not allowed", "NOTVULN", self.use_json))
+            ptprinthelper.ptprint(f"CONNECT method at port {self.port} is not allowed", "NOTVULN", self.use_json == False)
+
+        if next((method for method in methods["available_methods"] if method['method'] == "TRACE"), None):
+            ptprinthelper.ptprint(f"TRACE method is allowed", "VULN", self.use_json == False)
 
+        if len(self.url_list) > 1 and not url == self.url_list[-1]:
+            ptprinthelper.ptprint(f" ", "", self.use_json == False)
+
+    def _get_response(self, url, method, proxies=None, dump_response=False):
+        """Retrieve response"""
+        if proxies is None:
+            proxies = self.proxies
+        return ptmisclib.load_url_from_web_or_temp(url, method=method, headers=self.headers, proxies=proxies, timeout=self.timeout, redirects=self.redirects, verify=False, cache=self.cache, dump_response=dump_response)
+
+    def _parse_url(self, url):
+        """Validates url, returns port and url"""
+        o = urllib.parse.urlparse(url)
+        if o.scheme not in ["http", "https"]:
+            raise ValueError("Missing or unsupported schema")
+        if ":" in o.netloc:
+            split_obj = o.netloc.split(":")
+            port = split_obj[-1]
+            o = o._replace(netloc=split_obj[0])
+        else:
+            port = "443" if o.scheme == "https" else "80"
+        return port, urllib.parse.urlunparse(o)
 
 
 def get_help():
     return [
-        {"description": ["Allowed HTTP Methods Testing Tool"]},
+        {"description": ["HTTP methods testing tool"]},
         {"usage": ["ptmethods <options>"]},
         {"Tip": ["Optimally use this script against homepage, any image and sources protected by HTTP authentication"]},
         {"usage_example": [
-            "ptmethods -u https://www.example.com/image.jpg",
+            "ptmethods -u https://www.example.com/image.png",
             "ptmethods -u https://www.example.com/index.php",
             "ptmethods -u https://www.example.com/index.php -c PHPSESSID=abcdef",
             "ptmethods -f URL_list.txt",
         ]},
         {"options": [
             ["-u",  "--url",                    "<url>",            "Test specified URL"],
-            ["-f",  "--file",                   "<file>",           "Load list of URLs from file"],
+            ["-f",  "--file",                   "<file>",           "Load URLs from file"],
             ["-sh", "--show-headers",           "",                 "Show response headers"],
             ["-sr", "--show-response",          "",                 "Show response text"],
+            ["-T",  "--timeout",                "",                 "Set timeout (default 10)"],
             ["-p",  "--proxy",                  "<proxy>",          "Set proxy (e.g. http://127.0.0.1:8080)"],
             ["-ua", "--user-agent",             "<ua>",             "Set User-Agent header"],
+            ["-c",  "--cookie",                 "<cookie>",         "Set cookie"],
             ["-H",  "--headers",                "<header:value>",   "Set custom header(s)"],
-            ["-c",  "--cookie",                 "<cookie>",         "Set cookie(s)"],
             ["-r",  "--redirects",              "",                 "Follow redirects (default False)"],
-            ["-j",  "--json",                   "",                 "Output in JSON format"],
+            ["-c",  "--cache",                  "",                 "Cache requests (load from tmp in future)"],
             ["-v",  "--version",                "",                 "Show script version and exit"],
-            ["-h",  "--help",                   "",                 "Show this help message and exit"]
+            ["-h",  "--help",                   "",                 "Show this help message and exit"],
+            ["-j",  "--json",                   "",                 "Output in JSON format"],
         ]
         }]
 
 
 def parse_args():
     parser = argparse.ArgumentParser(add_help=False, usage="ptmethods <options>")
-    parser.add_argument("-u", "--url", type=str, nargs="+")
-    parser.add_argument("-f", "--file", type=str)
-    parser.add_argument("-p", "--proxy", type=str)
-    parser.add_argument("-ua", "--user-agent", type=str, default="Penterep Tools")
-    parser.add_argument("-c", "--cookie", type=str, nargs="+")
-    parser.add_argument("-H", "--headers", type=ptmisclib.pairs, nargs="+")
-    parser.add_argument("-j", "--json", action="store_true")
-    parser.add_argument("-r", "--redirects", action="store_true")
-    parser.add_argument("-sr", "--show-response", action="store_true")
-    parser.add_argument("-sh", "--show-headers", action="store_true")
-    parser.add_argument("-v", "--version", action="version", version=f"{SCRIPTNAME} {__version__}")
+    exclusive_group = parser.add_mutually_exclusive_group(required=True)
+    exclusive_group.add_argument("-u", "--url",    type=str, nargs="+")
+    exclusive_group.add_argument("-f", "--file",   type=str)
+    parser.add_argument("-p",  "--proxy",          type=str)
+    parser.add_argument("-ua", "--user-agent",     type=str, default="Penterep Tools")
+    parser.add_argument("-c",  "--cookie",         type=str, nargs="+")
+    parser.add_argument("-T",  "--timeout",        type=int, default=6)
+    parser.add_argument("-H",  "--headers",        type=ptmisclib.pairs, nargs="+")
+    parser.add_argument("-j",  "--json",           action="store_true")
+    parser.add_argument("-r",  "--redirects",      action="store_true")
+    parser.add_argument("-C",  "--cache",          action="store_true")
+    parser.add_argument("-sr", "--show-response",  action="store_true")
+    parser.add_argument("-sh", "--show-headers",   action="store_true")
+    parser.add_argument("-v",  "--version",        action="version", version=f"{SCRIPTNAME} {__version__}")
 
     if len(sys.argv) == 1 or "-h" in sys.argv or "--help" in sys.argv:
-        ptmisclib.help_print(get_help(), SCRIPTNAME, __version__)
+        ptprinthelper.help_print(get_help(), SCRIPTNAME, __version__)
         sys.exit(0)
     args = parser.parse_args()
-    ptmisclib.print_banner(SCRIPTNAME, __version__, args.json, space=0)
+    ptprinthelper.print_banner(SCRIPTNAME, __version__, args.json, space=0)
     return args
 
 
 def main():
     global SCRIPTNAME
     SCRIPTNAME = "ptmethods"
     requests.packages.urllib3.disable_warnings()
     requests.packages.urllib3.util.ssl_.DEFAULT_CIPHERS += ':HIGH:!DH:!aNULL'
     args = parse_args()
-    script = ptmethods(args)
+    script = PtMethods(args)
     script.run()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ptmethods-0.0.4/ptmethods.egg-info/PKG-INFO` & `ptmethods-1.0.0/ptmethods.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,103 +1,111 @@
 Metadata-Version: 2.1
 Name: ptmethods
-Version: 0.0.4
-Summary: HTTP Methods Testing Tool
+Version: 1.0.0
+Summary: HTTP methods testing tool
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
 
 # PTMETHODS
-> HTTP Methods Testing Tool
+> HTTP methods testing tool
 
-- Script retrieves methods offered by server from *OPTIONS* request
-- Script sends GET, POST, PUT, PATCH, DELETE, OPTIONS, HEAD, TRACE, DEBUG headers and retrieves it's response.
-- Script tests CONNECT method by connecting to url at ports 80, 443
-- Script tests if domain can be used as proxy.
+- Script retrieves methods offered by server from OPTIONS request
+- Script sends GET, POST, PUT, PATCH, DELETE, OPTIONS, HEAD, TRACE, DEBUG, FOO headers and returns server response
+- Script tests CONNECT method by connecting to URL at ports 80, 443
+- Script tests if domain can be used as a proxy
 
 ## Installation
-
 ```
 pip install ptmethods
 ```
 
-### Add to PATH
+## Add to PATH
 If you cannot invoke the script in your terminal, its probably because its not in your PATH. Fix it by running commands below.
 
-Add to path for BASH
+> Add to PATH for Bash
 ```bash
 echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.bashrc
 source ~/.bashrc
 ```
-Add to path for ZSH
+
+> Add to PATH for ZSH
 ```bash
 echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshhrc
 source ~/.zshhrc
 ```
 
 ## Usage examples
 Optimally use this script against homepage, any image and sources protected by HTTP authentication
 ```
 ptmethods -u https://www.example.com/
 ptmethods -u https://www.example.com/ -r
 ptmethods -u https://www.example.com/index.php -sr -sh
-ptmethods -u https://www.example.com/index.php -c PHPSESSID
+ptmethods -u https://www.example.com/index.php -c PHPSESSID=abcdef
 ptmethods -f URL_list.txt
 ```
 
 ## Options
 ```
 -u   --url            <url>           Test specified URL
--f   --file           <file>          Load list of URLs from file
+-f   --file           <file>          Load URLs from file
 -sh  --show-headers                   Show response headers
 -sr  --show-response                  Show response text
 -p   --proxy          <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
+-T   --timeout                        Set timeout (default 10)
+-c   --cookie         <cookie>        Set cookie
 -ua  --user-agent     <ua>            Set User-Agent header
 -H   --headers        <header:value>  Set custom header(s)
--c   --cookie         <cookie>        Set cookie(s)
 -r   --redirects                      Follow redirects (default False)
--j   --json                           Output in JSON format
+-c   --cache                          Cache requests (load from tmp in future)
 -v   --version                        Show script version and exit
 -h   --help                           Show this help message and exit
+-j   --json                           Output in JSON format
 ```
 
 ## Dependencies
 ```
 requests
 ptlibs
 ```
 
 ## Version History
-    0.0.2 - 0.0.4
-        - Implemented proxy test
-        - Implemented CONNECT tests
-    0.0.1 - 0.0.3
-        Alpha releases
+```
+1.0.0
+    - Support for ptlibs v1.0.0
+    - Code refactorization
+0.0.2 - 0.0.4
+    - Implemented proxy and connect tests
+0.0.1 - 0.0.3
+    Alpha releases
+```
 
-## Licence
 
-Copyright (c) 2020 HACKER Consulting s.r.o.
+## License
+
+Copyright (c) 2023 Penterep Security s.r.o.
 
 ptmethods is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 ptmethods is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with ptmethods. If not, see https://www.gnu.org/licenses/.
 
 ## Warning
 
 You are only allowed to run the tool against the websites which
 you have been given permission to pentest. We do not accept any
 responsibility for any damage/harm that this application causes to your
 computer, or your network. Penterep is not responsible for any illegal
 or malicious use of this code. Be Ethical!
-
```

### Comparing `ptmethods-0.0.4/setup.py` & `ptmethods-1.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import setuptools
+from ptmethods._version import __version__
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ptmethods",
-    version="0.0.4",
-    description="HTTP Methods Testing Tool",
+    version=__version__,
+    description="HTTP methods testing tool",
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
-    install_requires=["ptlibs", "requests"],
+    install_requires=["ptlibs>=1,<2", "requests"],
     entry_points = {'console_scripts': ['ptmethods = ptmethods.ptmethods:main']},
     long_description=long_description,
     long_description_content_type="text/markdown",
 )
```

