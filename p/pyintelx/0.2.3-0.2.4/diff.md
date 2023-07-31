# Comparing `tmp/pyintelx-0.2.3.tar.gz` & `tmp/pyintelx-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyintelx-0.2.3.tar", last modified: Fri Jul 28 20:04:38 2023, max compression
+gzip compressed data, was "pyintelx-0.2.4.tar", last modified: Mon Jul 31 14:26:58 2023, max compression
```

## Comparing `pyintelx-0.2.3.tar` & `pyintelx-0.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:04:38.294822 pyintelx-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-28 20:04:38.294822 pyintelx-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-07-28 20:04:28.000000 pyintelx-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:04:38.294822 pyintelx-0.2.3/pyintelx/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-28 20:04:28.000000 pyintelx-0.2.3/pyintelx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:04:38.294822 pyintelx-0.2.3/pyintelx/cli/
--rw-r--r--   0 runner    (1001) docker     (123)    10502 2023-07-28 20:04:28.000000 pyintelx-0.2.3/pyintelx/cli/pyintelx
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-28 20:04:28.000000 pyintelx-0.2.3/pyintelx/pyintelx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:04:38.294822 pyintelx-0.2.3/pyintelx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-28 20:04:38.000000 pyintelx-0.2.3/pyintelx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-28 20:04:38.000000 pyintelx-0.2.3/pyintelx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:04:38.000000 pyintelx-0.2.3/pyintelx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-28 20:04:38.000000 pyintelx-0.2.3/pyintelx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:04:38.294822 pyintelx-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-28 20:04:28.000000 pyintelx-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:26:58.676174 pyintelx-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-07-31 14:26:58.676174 pyintelx-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-31 14:26:48.000000 pyintelx-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:26:58.676174 pyintelx-0.2.4/pyintelx/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-31 14:26:48.000000 pyintelx-0.2.4/pyintelx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:26:58.676174 pyintelx-0.2.4/pyintelx/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)    11448 2023-07-31 14:26:48.000000 pyintelx-0.2.4/pyintelx/cli/pyintelx
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-07-31 14:26:48.000000 pyintelx-0.2.4/pyintelx/pyintelx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:26:58.676174 pyintelx-0.2.4/pyintelx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-07-31 14:26:58.000000 pyintelx-0.2.4/pyintelx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-31 14:26:58.000000 pyintelx-0.2.4/pyintelx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 14:26:58.000000 pyintelx-0.2.4/pyintelx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-31 14:26:58.000000 pyintelx-0.2.4/pyintelx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 14:26:58.676174 pyintelx-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-31 14:26:48.000000 pyintelx-0.2.4/setup.py
```

### Comparing `pyintelx-0.2.3/PKG-INFO` & `pyintelx-0.2.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyintelx
-Version: 0.2.3
+Version: 0.2.4
 Summary: This lib add support to use the Identity API from Intelx.io
 Home-page: https://github.com/csirtamericas/pyintelxio
 Author: Fermin Baudino, Einar Lanfranco, Federico Carrilao
 License: MIT
 Keywords: python, package, distribution
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -36,30 +36,39 @@
 
 ```bash 
 
 pyintelx -apikey {API_KEY} -search {search_term} -limit 10 
 
 pyintelx -apikey {API_KEY} -search {search_term} -limit 10 --identityenabled
 
+pyintelx -apikey {API_KEY} -search {search_term} -limit 10 --identityenabled --accounts
+
 ```
 
 SEARCH EXAMPLES
 ---------------
 
 * Query for 10 leaks containing pepe@example.com in intelx.io API
 
 ```bash
 pyintelx -apikey {API_KEY} search -search pepe@example.com -limit 10
 ```
 
 * Query for 10 leaks of accounts and passwords for domain example.com in identity.intelx.io API
 
 ```bash
+pyintelx -apikey {API_KEY} -search example.com -limit 10 --identityenabled --accounts
+```
+
+* Query for 10 data leaks for domain example.com in identity.intelx.io API
+
+```bash
 pyintelx -apikey {API_KEY} -search example.com -limit 10 --identityenabled
 ```
+
 * Download some leak file identied by SYSTEM_ID from some previous search
 
 ```bash
 pyintelx -apikey {API_KEY} -download {SYSTEM_ID} -name {FILE_NAME} -bucket {BUCKET_NAME}
 ```
 
 
@@ -84,25 +93,36 @@
 from pyintelx import intelx
 API_KEY = "your api key"
 
 intelx_service = intelx(API_KEY)
 intelx_service.search("example@example.com", maxresults=max_results, datefrom=date_from, dateto=date_to, buckets=[])
 ```
 
-* Search for using identity service
+* Search for using identity Search Data Leaks service
 
 ```python
 from pyintelx import IdentityService
 API_KEY = "your api key"
 
 identity_service = IdentityService(API_KEY)
 
 identity_service.search("example@example.com", maxresults=max_results, datefrom=date_from, dateto=date_to, buckets=[])
 ```
 
+* Search for using identity export accounts service
+
+```python
+from pyintelx import IdentityService
+API_KEY = "your api key"
+
+identity_service = IdentityService(API_KEY)
+
+identity_service.export_accounts("example.com", maxresults=max_results, datefrom=date_from, dateto=date_to, buckets=[])
+```
+
 
 ## Buckets list
 - darknet.tor
 - darknet.i2p
 - documents.public.scihub
 - dumpster
 - leaks.private.general
```

### Comparing `pyintelx-0.2.3/README.md` & `pyintelx-0.2.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,30 +20,39 @@
 
 ```bash 
 
 pyintelx -apikey {API_KEY} -search {search_term} -limit 10 
 
 pyintelx -apikey {API_KEY} -search {search_term} -limit 10 --identityenabled
 
+pyintelx -apikey {API_KEY} -search {search_term} -limit 10 --identityenabled --accounts
+
 ```
 
 SEARCH EXAMPLES
 ---------------
 
 * Query for 10 leaks containing pepe@example.com in intelx.io API
 
 ```bash
 pyintelx -apikey {API_KEY} search -search pepe@example.com -limit 10
 ```
 
 * Query for 10 leaks of accounts and passwords for domain example.com in identity.intelx.io API
 
 ```bash
+pyintelx -apikey {API_KEY} -search example.com -limit 10 --identityenabled --accounts
+```
+
+* Query for 10 data leaks for domain example.com in identity.intelx.io API
+
+```bash
 pyintelx -apikey {API_KEY} -search example.com -limit 10 --identityenabled
 ```
+
 * Download some leak file identied by SYSTEM_ID from some previous search
 
 ```bash
 pyintelx -apikey {API_KEY} -download {SYSTEM_ID} -name {FILE_NAME} -bucket {BUCKET_NAME}
 ```
 
 
@@ -68,25 +77,36 @@
 from pyintelx import intelx
 API_KEY = "your api key"
 
 intelx_service = intelx(API_KEY)
 intelx_service.search("example@example.com", maxresults=max_results, datefrom=date_from, dateto=date_to, buckets=[])
 ```
 
-* Search for using identity service
+* Search for using identity Search Data Leaks service
 
 ```python
 from pyintelx import IdentityService
 API_KEY = "your api key"
 
 identity_service = IdentityService(API_KEY)
 
 identity_service.search("example@example.com", maxresults=max_results, datefrom=date_from, dateto=date_to, buckets=[])
 ```
 
+* Search for using identity export accounts service
+
+```python
+from pyintelx import IdentityService
+API_KEY = "your api key"
+
+identity_service = IdentityService(API_KEY)
+
+identity_service.export_accounts("example.com", maxresults=max_results, datefrom=date_from, dateto=date_to, buckets=[])
+```
+
 
 ## Buckets list
 - darknet.tor
 - darknet.i2p
 - documents.public.scihub
 - dumpster
 - leaks.private.general
```

### Comparing `pyintelx-0.2.3/pyintelx/cli/pyintelx` & `pyintelx-0.2.4/pyintelx/cli/pyintelx`

 * *Files 3% similar despite different names*

```diff
@@ -52,14 +52,20 @@
 
 def idsearch(identity_ix, query, maxresults=100, buckets=[], timeout=5, datefrom="", dateto="", terminate=[]):
     if not args.raw:
         print(colored(f"[{rightnow()}] Starting search of \"{args.search}\".", 'green'))
     s = identity_ix.search(term=query, maxresults=maxresults, buckets=buckets, timeout=timeout, datefrom=datefrom, dateto=dateto,  terminate=terminate)
     return s
 
+def export_accounts(identity_ix, query, maxresults=100, buckets=[], timeout=5, datefrom="", dateto="", terminate=[]):
+    if not args.raw:
+        print(colored(f"[{rightnow()}] Starting search of \"{args.search}\".", 'green'))
+    s = identity_ix.export_accounts(term=query, maxresults=maxresults, buckets=buckets, datefrom=datefrom, dateto=dateto,  terminate=terminate)
+    return s
+
 def get_stats(stats):
     if not args.raw:
         print(colored(f"[{rightnow()}] Gathering stats from search.\n", 'green'))
         stats = json.dumps(ix.stats(search), indent=4, sort_keys=True)
         print(stats)
 
 
@@ -134,14 +140,15 @@
     parser.add_argument('--view', help="show full contents of search results", action="store_true")
     parser.add_argument('--phonebook', help="set the search type to a phonebook search")
     parser.add_argument('--emails', help="show only emails from phonebook results", action="store_true")
     parser.add_argument('--capabilities', help="show your account's capabilities", action="store_true")
     parser.add_argument('--stats', help="show stats of search results", action="store_true")
     parser.add_argument('--raw', help="show raw json", action="store_true")
     parser.add_argument('--identityenabled', help="enable identity api search (requires api key)", action="store_true")
+    parser.add_argument('--accounts', help="search only leaked accounts on identity service", action="store_true")
     args = parser.parse_args()
 
     # configure IX & the API key
     if 'INTELX_KEY' in os.environ:
         ix = intelx(os.environ['INTELX_KEY'])
         if 'IDENTITY_ENABLED' in os.environ:
             ix_identity = IdentityService(os.environ['INTELX_KEY'])
@@ -226,24 +233,36 @@
                 dateto=dateto,
                 sort=sort,
                 media=media,
                 terminate=terminate,
                 target=targetval
             )
         elif args.identityenabled:
-            search = idsearch(
-                ix_identity,
-                args.search,
-                maxresults=maxresults,
-                buckets=buckets,
-                timeout=timeout,
-                datefrom=datefrom,
-                dateto=dateto,
-                terminate=terminate
-            )
+            if args.accounts:
+                search = export_accounts(
+                    ix_identity,
+                    args.search,
+                    maxresults=maxresults,
+                    buckets=buckets,
+                    timeout=timeout,
+                    datefrom=datefrom,
+                    dateto=dateto,
+                    terminate=terminate
+                )
+            else:
+                search = idsearch(
+                    ix_identity,
+                    args.search,
+                    maxresults=maxresults,
+                    buckets=buckets,
+                    timeout=timeout,
+                    datefrom=datefrom,
+                    dateto=dateto,
+                    terminate=terminate
+                )
 
         if args.raw or args.identityenabled:
             print(json.dumps(search))
 
         if args.stats:
             get_stats(search)
```

### Comparing `pyintelx-0.2.3/pyintelx/pyintelx.py` & `pyintelx-0.2.4/pyintelx/pyintelx.py`

 * *Files 15% similar despite different names*

```diff
@@ -62,22 +62,39 @@
         r = requests.get(self.API_ROOT + '/live/search/internal',
                          headers=self.HEADERS, params=p)
         if r.status_code == 204:
             return (r.status_code, r.text)
         else:
             return (r.status_code, r.text)
 
-    def export_csv(self, selector, date_from=None, date_to=None, limit=10, bucket_filter=[], terminate=None):
+    def export_accounts(self, term, datefrom=None, dateto=None, maxresults=10, buckets=[], terminate=None):
         p = {
-            "selector": selector,
-            "bucket": bucket_filter,
-            "limit": limit,
-            "datefrom": date_from,  # "YYYY-MM-DD HH:MM:SS",
-            "dateto": date_to,  # "YYYY-MM-DD HH:MM:SS"
+            "selector": term,
+            "bucket": buckets,
+            "limit": maxresults,
+            "datefrom": datefrom,  # "YYYY-MM-DD HH:MM:SS",
+            "dateto": dateto,  # "YYYY-MM-DD HH:MM:SS"
             "terminate": terminate,
         }
+        done = False
+        results = []
         r = requests.get(self.API_ROOT + '/accounts/csv',
                          headers=self.HEADERS, params=p)
         if r.status_code == 200:
-            return r.json()['id']
+            search_id = r.json()['id']
+            if (len(str(search_id)) <= 3):
+                print(
+                    f"[!] intelx.IDENTITY_EXPORT() Received {self.get_error(search_id)}")
+            while not done:
+                time.sleep(1)
+                r = self.get_search_results(search_id, maxresults=maxresults)
+                if (r["status"] == 0 and r["records"]):
+                    for a in r['records']:
+                        results.append(a)
+                    maxresults -= len(r['records'])
+                if (r['status'] == 1 or r['status'] == 2 or maxresults <= 0):
+                    if (maxresults <= 0):
+                        self.terminate_search(search_id)
+                    done = True
+            return {'records': results}
         else:
             return (r.status_code, r.text)
```

### Comparing `pyintelx-0.2.3/pyintelx.egg-info/PKG-INFO` & `pyintelx-0.2.4/pyintelx.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyintelx
-Version: 0.2.3
+Version: 0.2.4
 Summary: This lib add support to use the Identity API from Intelx.io
 Home-page: https://github.com/csirtamericas/pyintelxio
 Author: Fermin Baudino, Einar Lanfranco, Federico Carrilao
 License: MIT
 Keywords: python, package, distribution
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -36,30 +36,39 @@
 
 ```bash 
 
 pyintelx -apikey {API_KEY} -search {search_term} -limit 10 
 
 pyintelx -apikey {API_KEY} -search {search_term} -limit 10 --identityenabled
 
+pyintelx -apikey {API_KEY} -search {search_term} -limit 10 --identityenabled --accounts
+
 ```
 
 SEARCH EXAMPLES
 ---------------
 
 * Query for 10 leaks containing pepe@example.com in intelx.io API
 
 ```bash
 pyintelx -apikey {API_KEY} search -search pepe@example.com -limit 10
 ```
 
 * Query for 10 leaks of accounts and passwords for domain example.com in identity.intelx.io API
 
 ```bash
+pyintelx -apikey {API_KEY} -search example.com -limit 10 --identityenabled --accounts
+```
+
+* Query for 10 data leaks for domain example.com in identity.intelx.io API
+
+```bash
 pyintelx -apikey {API_KEY} -search example.com -limit 10 --identityenabled
 ```
+
 * Download some leak file identied by SYSTEM_ID from some previous search
 
 ```bash
 pyintelx -apikey {API_KEY} -download {SYSTEM_ID} -name {FILE_NAME} -bucket {BUCKET_NAME}
 ```
 
 
@@ -84,25 +93,36 @@
 from pyintelx import intelx
 API_KEY = "your api key"
 
 intelx_service = intelx(API_KEY)
 intelx_service.search("example@example.com", maxresults=max_results, datefrom=date_from, dateto=date_to, buckets=[])
 ```
 
-* Search for using identity service
+* Search for using identity Search Data Leaks service
 
 ```python
 from pyintelx import IdentityService
 API_KEY = "your api key"
 
 identity_service = IdentityService(API_KEY)
 
 identity_service.search("example@example.com", maxresults=max_results, datefrom=date_from, dateto=date_to, buckets=[])
 ```
 
+* Search for using identity export accounts service
+
+```python
+from pyintelx import IdentityService
+API_KEY = "your api key"
+
+identity_service = IdentityService(API_KEY)
+
+identity_service.export_accounts("example.com", maxresults=max_results, datefrom=date_from, dateto=date_to, buckets=[])
+```
+
 
 ## Buckets list
 - darknet.tor
 - darknet.i2p
 - documents.public.scihub
 - dumpster
 - leaks.private.general
```

### Comparing `pyintelx-0.2.3/setup.py` & `pyintelx-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 
 setup(
     name='pyintelx',
-    version='0.2.3',
+    version='0.2.4',
     description='This lib add support to use the Identity API from Intelx.io',
     license='MIT',
     keywords=['python, package, distribution'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Fermin Baudino, Einar Lanfranco, Federico Carrilao',
     url='https://github.com/csirtamericas/pyintelxio',
```

