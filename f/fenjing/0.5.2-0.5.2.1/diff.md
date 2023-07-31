# Comparing `tmp/fenjing-0.5.2.tar.gz` & `tmp/fenjing-0.5.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenjing-0.5.2.tar", last modified: Mon Jul 31 12:23:17 2023, max compression
+gzip compressed data, was "fenjing-0.5.2.1.tar", last modified: Mon Jul 31 12:29:31 2023, max compression
```

## Comparing `fenjing-0.5.2.tar` & `fenjing-0.5.2.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:23:17.824095 fenjing-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-31 12:23:04.000000 fenjing-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-31 12:23:04.000000 fenjing-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-07-31 12:23:17.824095 fenjing-0.5.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     9413 2023-07-31 12:23:04.000000 fenjing-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 12:23:04.000000 fenjing-0.5.2/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:23:17.824095 fenjing-0.5.2/fenjing/
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-31 12:23:04.000000 fenjing-0.5.2/fenjing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-31 12:23:04.000000 fenjing-0.5.2/fenjing/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15737 2023-07-31 12:23:04.000000 fenjing-0.5.2/fenjing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-31 12:23:04.000000 fenjing-0.5.2/fenjing/colorize.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-31 12:23:04.000000 fenjing-0.5.2/fenjing/config_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-31 12:23:04.000000 fenjing-0.5.2/fenjing/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-31 12:23:04.000000 fenjing-0.5.2/fenjing/context_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-07-31 12:23:04.000000 fenjing-0.5.2/fenjing/cracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-31 12:23:04.000000 fenjing-0.5.2/fenjing/form.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7619 2023-07-31 12:23:04.000000 fenjing-0.5.2/fenjing/full_payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    46622 2023-07-31 12:23:04.000000 fenjing-0.5.2/fenjing/payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-31 12:23:04.000000 fenjing-0.5.2/fenjing/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-31 12:23:04.000000 fenjing-0.5.2/fenjing/scan_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-31 12:23:04.000000 fenjing-0.5.2/fenjing/shell_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-07-31 12:23:04.000000 fenjing-0.5.2/fenjing/submitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:23:17.824095 fenjing-0.5.2/fenjing/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-31 12:23:04.000000 fenjing-0.5.2/fenjing/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-07-31 12:23:04.000000 fenjing-0.5.2/fenjing/waf_func_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    10187 2023-07-31 12:23:04.000000 fenjing-0.5.2/fenjing/webui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:23:17.824095 fenjing-0.5.2/fenjing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-07-31 12:23:17.000000 fenjing-0.5.2/fenjing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-31 12:23:17.000000 fenjing-0.5.2/fenjing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 12:23:17.000000 fenjing-0.5.2/fenjing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-31 12:23:17.000000 fenjing-0.5.2/fenjing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-31 12:23:17.000000 fenjing-0.5.2/fenjing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-31 12:23:04.000000 fenjing-0.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 12:23:17.824095 fenjing-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-31 12:23:04.000000 fenjing-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:23:17.824095 fenjing-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-07-31 12:23:04.000000 fenjing-0.5.2/tests/test_cracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-07-31 12:23:04.000000 fenjing-0.5.2/tests/test_full_payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-07-31 12:23:04.000000 fenjing-0.5.2/tests/test_payload_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:29:31.487445 fenjing-0.5.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-31 12:29:19.000000 fenjing-0.5.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-31 12:29:19.000000 fenjing-0.5.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-07-31 12:29:31.487445 fenjing-0.5.2.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9413 2023-07-31 12:29:19.000000 fenjing-0.5.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-31 12:29:19.000000 fenjing-0.5.2.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:29:31.483445 fenjing-0.5.2.1/fenjing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-31 12:29:19.000000 fenjing-0.5.2.1/fenjing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-31 12:29:19.000000 fenjing-0.5.2.1/fenjing/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15737 2023-07-31 12:29:19.000000 fenjing-0.5.2.1/fenjing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-31 12:29:19.000000 fenjing-0.5.2.1/fenjing/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-31 12:29:19.000000 fenjing-0.5.2.1/fenjing/config_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-31 12:29:19.000000 fenjing-0.5.2.1/fenjing/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-31 12:29:19.000000 fenjing-0.5.2.1/fenjing/context_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-07-31 12:29:19.000000 fenjing-0.5.2.1/fenjing/cracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-31 12:29:19.000000 fenjing-0.5.2.1/fenjing/form.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7619 2023-07-31 12:29:19.000000 fenjing-0.5.2.1/fenjing/full_payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46622 2023-07-31 12:29:19.000000 fenjing-0.5.2.1/fenjing/payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-31 12:29:19.000000 fenjing-0.5.2.1/fenjing/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-31 12:29:19.000000 fenjing-0.5.2.1/fenjing/scan_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-31 12:29:19.000000 fenjing-0.5.2.1/fenjing/shell_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-07-31 12:29:19.000000 fenjing-0.5.2.1/fenjing/submitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:29:31.487445 fenjing-0.5.2.1/fenjing/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-31 12:29:19.000000 fenjing-0.5.2.1/fenjing/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-07-31 12:29:19.000000 fenjing-0.5.2.1/fenjing/waf_func_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10187 2023-07-31 12:29:19.000000 fenjing-0.5.2.1/fenjing/webui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:29:31.487445 fenjing-0.5.2.1/fenjing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-07-31 12:29:31.000000 fenjing-0.5.2.1/fenjing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-31 12:29:31.000000 fenjing-0.5.2.1/fenjing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 12:29:31.000000 fenjing-0.5.2.1/fenjing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-31 12:29:31.000000 fenjing-0.5.2.1/fenjing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-31 12:29:31.000000 fenjing-0.5.2.1/fenjing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-31 12:29:19.000000 fenjing-0.5.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 12:29:31.487445 fenjing-0.5.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-31 12:29:19.000000 fenjing-0.5.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:29:31.487445 fenjing-0.5.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-07-31 12:29:19.000000 fenjing-0.5.2.1/tests/test_cracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-07-31 12:29:19.000000 fenjing-0.5.2.1/tests/test_full_payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-07-31 12:29:19.000000 fenjing-0.5.2.1/tests/test_payload_gen.py
```

### Comparing `fenjing-0.5.2/LICENSE` & `fenjing-0.5.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.2/PKG-INFO` & `fenjing-0.5.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.5.2
+Version: 0.5.2.1
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.5.2/README.md` & `fenjing-0.5.2.1/README.md`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.2/fenjing/cli.py` & `fenjing-0.5.2.1/fenjing/cli.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.2/fenjing/colorize.py` & `fenjing-0.5.2.1/fenjing/colorize.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.2/fenjing/config_payload.py` & `fenjing-0.5.2.1/fenjing/config_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.2/fenjing/const.py` & `fenjing-0.5.2.1/fenjing/const.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.2/fenjing/context_vars.py` & `fenjing-0.5.2.1/fenjing/context_vars.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.2/fenjing/cracker.py` & `fenjing-0.5.2.1/fenjing/cracker.py`

 * *Files 8% similar despite different names*

```diff
@@ -173,22 +173,24 @@
         )
         if payload is None:
             return None
         assert will_print is not None, "It just shouldn't! when payload is not None!"
         payload_dict = {self.subm.target_field: payload}
         method = self.subm.form["method"]
         assert isinstance(method, str)
+        payload_param = random_fill(self.subm.form)
+        payload_param.update(payload_dict)
         new_subm = RequestSubmitter(
             url=self.subm.url,
             method=method,
             target_field=args_target_field,
-            params=random_fill(self.subm.form) | payload_dict
+            params=payload_param
             if method == "GET"
             else {},
-            data=random_fill(self.subm.form) | payload_dict if method != "GET" else {},
+            data=payload_param if method != "GET" else {},
             requester=self.subm.req,
         )
         if self.subm.tamperers:
             for tamperer in self.subm.tamperers:
                 new_subm.add_tamperer(tamperer)
         if will_print:
             if self.test_payload_eval_args(self.test_eval, new_subm):
```

### Comparing `fenjing-0.5.2/fenjing/form.py` & `fenjing-0.5.2.1/fenjing/form.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.2/fenjing/full_payload_gen.py` & `fenjing-0.5.2.1/fenjing/full_payload_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.2/fenjing/payload_gen.py` & `fenjing-0.5.2.1/fenjing/payload_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.2/fenjing/requester.py` & `fenjing-0.5.2.1/fenjing/requester.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.2/fenjing/scan_url.py` & `fenjing-0.5.2.1/fenjing/scan_url.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.2/fenjing/shell_payload.py` & `fenjing-0.5.2.1/fenjing/shell_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.2/fenjing/submitter.py` & `fenjing-0.5.2.1/fenjing/submitter.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.2/fenjing/templates/index.html` & `fenjing-0.5.2.1/fenjing/templates/index.html`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.2/fenjing/waf_func_gen.py` & `fenjing-0.5.2.1/fenjing/waf_func_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.2/fenjing/webui.py` & `fenjing-0.5.2.1/fenjing/webui.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.2/fenjing.egg-info/PKG-INFO` & `fenjing-0.5.2.1/fenjing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.5.2
+Version: 0.5.2.1
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.5.2/fenjing.egg-info/SOURCES.txt` & `fenjing-0.5.2.1/fenjing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.2/setup.py` & `fenjing-0.5.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.2/tests/test_cracker.py` & `fenjing-0.5.2.1/tests/test_cracker.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.2/tests/test_full_payload_gen.py` & `fenjing-0.5.2.1/tests/test_full_payload_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.2/tests/test_payload_gen.py` & `fenjing-0.5.2.1/tests/test_payload_gen.py`

 * *Files identical despite different names*

