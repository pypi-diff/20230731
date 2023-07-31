# Comparing `tmp/clean_workspace-0.2.0.tar.gz` & `tmp/clean_workspace-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clean_workspace-0.2.0.tar", max compression
+gzip compressed data, was "clean_workspace-0.3.0.tar", max compression
```

## Comparing `clean_workspace-0.2.0.tar` & `clean_workspace-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1071 2023-07-07 14:11:37.204209 clean_workspace-0.2.0/LICENSE
--rw-r--r--   0        0        0     1945 2023-07-07 14:11:37.204505 clean_workspace-0.2.0/README.md
--rw-r--r--   0        0        0     7639 2023-07-07 14:11:37.205823 clean_workspace-0.2.0/clean_workspace/__init__.py
--rw-r--r--   0        0        0      762 2023-07-07 14:13:03.605335 clean_workspace-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2736 1970-01-01 00:00:00.000000 clean_workspace-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-31 16:31:03.677692 clean_workspace-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2387 2023-07-31 16:31:03.761129 clean_workspace-0.3.0/README.md
+-rw-r--r--   0        0        0     7864 2023-07-31 16:31:03.925908 clean_workspace-0.3.0/clean_workspace/__init__.py
+-rw-r--r--   0        0        0      762 2023-07-31 16:35:11.892773 clean_workspace-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3178 1970-01-01 00:00:00.000000 clean_workspace-0.3.0/PKG-INFO
```

### Comparing `clean_workspace-0.2.0/LICENSE` & `clean_workspace-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clean_workspace-0.2.0/README.md` & `clean_workspace-0.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -8,23 +8,41 @@
 This is simple utility to automate this process. It will close all your tabs (in both Safari & Chrome), and send them to [todoist](https://mikebian.co/todoist) (and output) them to the terminal.
 
 We'll see if this actually helps!
 
 ## Installation
 
 ```shell
+pip install clean-workspace
+clean-workspace
+```
+
+## Development
+
+```shell
 poetry install
 poetry run clean-workspace
 ```
 
 ## Usage
 
 - Add your todoist token to `.envrc` and `direnv allow .`
 - Customize the url and domain blacklist
 
+```shell
+❯ clean-workspace --help
+Usage: clean-workspace [OPTIONS]
+
+Options:
+  --blacklist-domains PATH
+  --blacklist-urls PATH
+  --tab-description TEXT    Description for tab
+  --help                    Show this message and exit.
+```
+
 ### Collecting Tab Description Via AppleScript
 
 Here's a quick script you can use to collect a description of what you were working on via applescript:
 
 ```shell
 dialogResult=$(
 osascript <<EOT
@@ -41,7 +59,9 @@
 - https://gist.github.com/aleks-mariusz/cc27b21f2c5b91fbd285
 - https://github.com/tominsam/shelf-python/blob/f357d9b147fa651034b71501edabf65f59d5befa/extractors/ComAppleSafari.py#L11
 
 ## TODO
 
 - [ ] Indicate in python config that this is macOS only in poetry config?
 - [ ] move blacklist files into example area of repo
+- [ ] look at previous tasks and see if links are contained there before including them again
+- [ ] support google chrome canary
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `clean_workspace-0.2.0/clean_workspace/__init__.py` & `clean_workspace-0.3.0/clean_workspace/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import plistlib
 import sys
 import typing as t
-import click
 
 import chrome_bookmarks
+import click
 from ScriptingBridge import SBApplication
 
 
 def todoist_client():
     # extract todoist api key from environment without throwing an exception
     todoist_api_key = os.environ.get("TODOIST_API_KEY", None)
 
@@ -118,15 +118,19 @@
 
 
 def quit_browsers():
     os.system("osascript -e 'quit app \"Safari\"'")
     os.system("osascript -e 'quit app \"Chrome\"'")
 
 
-def clean_workspace(tab_description, blacklist_domains, blacklist_urls):
+# the syntax we use is starting and ending with `/`, like sed
+def _is_regex_entry(entry: str):
+    return entry.startswith("/") and entry.endswith("/")
+
+def clean_workspace(tab_description, blacklist_domains_file_path, blacklist_urls_file_path):
     browser_urls = get_browser_urls()
 
     # if page is blank, there is no url or string does not contain http
     browser_urls = [x for x in browser_urls if x[0] is not None and "http" in x[0]]
 
     # remove duplicates
     browser_urls = list(set(browser_urls))
@@ -137,23 +141,24 @@
     # strip all anchors from the urls
     browser_urls = [(url.split("#")[0], name) for url, name in browser_urls]
 
     # TODO load these files from a home config file
 
     # user configurable blacklist for urls you don't want to archive
     url_blacklist = []
-    with open(blacklist_urls, "r") as f:
+    with open(blacklist_urls_file_path, "r") as f:
         url_blacklist = f.read().splitlines()
 
     domain_blacklist = []
-    with open(blacklist_domains, "r") as f:
+    with open(blacklist_domains_file_path, "r") as f:
         domain_blacklist = f.read().splitlines()
+
         # add a `www.` prefix to each domain in the blacklist and merge it with the existing list
         domain_blacklist = domain_blacklist + [
-            "www." + domain for domain in domain_blacklist
+            "www." + domain for domain in domain_blacklist if not _is_regex_entry(domain)
         ]
 
     bookmark_urls = get_bookmarks_urls()
 
     # TODO output skipped domains
     # TODO support wildcard subdomains, *.sentry.io
```

### Comparing `clean_workspace-0.2.0/pyproject.toml` & `clean_workspace-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clean-workspace"
-version = "0.2.0"
+version = "0.3.0"
 description = "Collect all browser URLs, output to terminal, and archive to todoist"
 authors = ["Michael Bianco <mike@mikebian.co>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/iloveitaly/clean-workspace"
 
 [tool.poetry.dependencies]
```

### Comparing `clean_workspace-0.2.0/PKG-INFO` & `clean_workspace-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean-workspace
-Version: 0.2.0
+Version: 0.3.0
 Summary: Collect all browser URLs, output to terminal, and archive to todoist
 Home-page: https://github.com/iloveitaly/clean-workspace
 License: MIT
 Author: Michael Bianco
 Author-email: mike@mikebian.co
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -28,23 +28,41 @@
 This is simple utility to automate this process. It will close all your tabs (in both Safari & Chrome), and send them to [todoist](https://mikebian.co/todoist) (and output) them to the terminal.
 
 We'll see if this actually helps!
 
 ## Installation
 
 ```shell
+pip install clean-workspace
+clean-workspace
+```
+
+## Development
+
+```shell
 poetry install
 poetry run clean-workspace
 ```
 
 ## Usage
 
 - Add your todoist token to `.envrc` and `direnv allow .`
 - Customize the url and domain blacklist
 
+```shell
+❯ clean-workspace --help
+Usage: clean-workspace [OPTIONS]
+
+Options:
+  --blacklist-domains PATH
+  --blacklist-urls PATH
+  --tab-description TEXT    Description for tab
+  --help                    Show this message and exit.
+```
+
 ### Collecting Tab Description Via AppleScript
 
 Here's a quick script you can use to collect a description of what you were working on via applescript:
 
 ```shell
 dialogResult=$(
 osascript <<EOT
@@ -61,8 +79,10 @@
 - https://gist.github.com/aleks-mariusz/cc27b21f2c5b91fbd285
 - https://github.com/tominsam/shelf-python/blob/f357d9b147fa651034b71501edabf65f59d5befa/extractors/ComAppleSafari.py#L11
 
 ## TODO
 
 - [ ] Indicate in python config that this is macOS only in poetry config?
 - [ ] move blacklist files into example area of repo
+- [ ] look at previous tasks and see if links are contained there before including them again
+- [ ] support google chrome canary
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

