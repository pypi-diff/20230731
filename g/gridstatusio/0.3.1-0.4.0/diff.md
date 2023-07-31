# Comparing `tmp/gridstatusio-0.3.1.tar.gz` & `tmp/gridstatusio-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/github/workspace/dist/.tmp-miq3ax9h/gridstatusio-0.3.1.tar", last modified: Thu Jul 27 18:03:18 2023, max compression
+gzip compressed data, was "/github/workspace/dist/.tmp-yt4f9maj/gridstatusio-0.4.0.tar", last modified: Mon Jul 31 21:21:26 2023, max compression
```

## Comparing `gridstatusio-0.3.1.tar` & `gridstatusio-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 18:03:18.000000 gridstatusio-0.3.1/
--rw-r--r--   0 root         (0) root         (0)     1461 2023-07-27 18:02:59.000000 gridstatusio-0.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3293 2023-07-27 18:03:18.000000 gridstatusio-0.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      883 2023-07-27 18:02:59.000000 gridstatusio-0.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 18:03:18.000000 gridstatusio-0.3.1/gridstatusio/
--rw-r--r--   0 root         (0) root         (0)       98 2023-07-27 18:02:59.000000 gridstatusio-0.3.1/gridstatusio/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10649 2023-07-27 18:02:59.000000 gridstatusio-0.3.1/gridstatusio/gs_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 18:03:18.000000 gridstatusio-0.3.1/gridstatusio/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 18:02:59.000000 gridstatusio-0.3.1/gridstatusio/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6714 2023-07-27 18:02:59.000000 gridstatusio-0.3.1/gridstatusio/tests/test_api.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-27 18:02:59.000000 gridstatusio-0.3.1/gridstatusio/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 18:03:18.000000 gridstatusio-0.3.1/gridstatusio.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3293 2023-07-27 18:03:18.000000 gridstatusio-0.3.1/gridstatusio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      348 2023-07-27 18:03:18.000000 gridstatusio-0.3.1/gridstatusio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 18:03:18.000000 gridstatusio-0.3.1/gridstatusio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      237 2023-07-27 18:03:18.000000 gridstatusio-0.3.1/gridstatusio.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-27 18:03:18.000000 gridstatusio-0.3.1/gridstatusio.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2319 2023-07-27 18:02:59.000000 gridstatusio-0.3.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 18:03:18.000000 gridstatusio-0.3.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 21:21:26.000000 gridstatusio-0.4.0/
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-07-31 21:21:10.000000 gridstatusio-0.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3293 2023-07-31 21:21:26.000000 gridstatusio-0.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      883 2023-07-31 21:21:10.000000 gridstatusio-0.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 21:21:26.000000 gridstatusio-0.4.0/gridstatusio/
+-rw-r--r--   0 root         (0) root         (0)       98 2023-07-31 21:21:10.000000 gridstatusio-0.4.0/gridstatusio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11530 2023-07-31 21:21:10.000000 gridstatusio-0.4.0/gridstatusio/gs_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 21:21:26.000000 gridstatusio-0.4.0/gridstatusio/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 21:21:10.000000 gridstatusio-0.4.0/gridstatusio/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6714 2023-07-31 21:21:10.000000 gridstatusio-0.4.0/gridstatusio/tests/test_api.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-31 21:21:10.000000 gridstatusio-0.4.0/gridstatusio/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 21:21:26.000000 gridstatusio-0.4.0/gridstatusio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3293 2023-07-31 21:21:26.000000 gridstatusio-0.4.0/gridstatusio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      348 2023-07-31 21:21:26.000000 gridstatusio-0.4.0/gridstatusio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 21:21:26.000000 gridstatusio-0.4.0/gridstatusio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      237 2023-07-31 21:21:26.000000 gridstatusio-0.4.0/gridstatusio.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-31 21:21:26.000000 gridstatusio-0.4.0/gridstatusio.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2319 2023-07-31 21:21:10.000000 gridstatusio-0.4.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 21:21:26.000000 gridstatusio-0.4.0/setup.cfg
```

### Comparing `gridstatusio-0.3.1/LICENSE` & `gridstatusio-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gridstatusio-0.3.1/PKG-INFO` & `gridstatusio-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridstatusio
-Version: 0.3.1
+Version: 0.4.0
 Summary: Python Client for GridStatus.io API
 Author-email: Max Kanter <kmax12@gmail.com>
 Maintainer-email: Max Kanter <kmax12@gmail.com>
 License: Copyright 2022 James Max Kanter
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
```

### Comparing `gridstatusio-0.3.1/README.md` & `gridstatusio-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `gridstatusio-0.3.1/gridstatusio/gs_client.py` & `gridstatusio-0.4.0/gridstatusio/gs_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,23 +19,31 @@
     if verbose == "debug":
         print(msg, end=end)
     elif verbose == "info" and level == "info":
         print(msg, end=end)
 
 
 class GridStatusClient:
-    def __init__(self, api_key=None, host="https://api.gridstatus.io/v1"):
+    def __init__(
+        self,
+        api_key=None,
+        host="https://api.gridstatus.io/v1",
+        request_format="json",
+    ):
         """Create a GridStatus.io API client
 
         Parameters:
             api_key (str): The API key to use for authentication.
             If not provided, the GRIDSTATUS_API_KEY environment variable will be used.
 
             host (str): The host to use for the API.
                 Defaults to https://api.gridstatus.io
+
+            request_format (str): The format to use for requests. Options are "json"
+                or "csv". Defaults to "json".
         """
 
         if api_key is None:
             import os
 
             api_key = os.environ.get("GRIDSTATUS_API_KEY")
 
@@ -44,34 +52,60 @@
                 "No API key provided. Either pass an api_key to the \
                 GridStatusClient constructor or set the \
                 GRIDSTATUS_API_KEY environment variable.",
             )
 
         self.api_key = api_key
         self.host = host
+        self.request_format = request_format
+
+        assert self.request_format in [
+            "json",
+            "csv",
+        ], "request_format must be 'json' or 'csv'"
 
     def __repr__(self) -> str:
         return f"GridStatusClient(host={self.host})"
 
     def get(self, url, params=None, verbose=False):
+        if params is None:
+            params = {}
+
         headers = {
             "x-api-key": self.api_key,
             # set client and version
             "x-client": "gridstatusio-python",
             "x-client-version": __version__,
         }
 
+        # note
+        # parameter name different for API
+        # than for python client
+        if "return_format" not in params:
+            params["return_format"] = self.request_format
+
+            if self.request_format == "json":
+                params["json_schema"] = "array-of-arrays"
+
         log(f"\nGET {url}", verbose=verbose, level="debug")
         log(f"Params: {params}", verbose=verbose, level="debug")
         response = requests.get(url, params=params, headers=headers)
 
         if response.status_code != 200:
             raise Exception(f"Error {response.status_code}: {response.text}")
 
-        return response
+        if self.request_format == "json":
+            data = response.json()
+            df = pd.DataFrame(data["data"][1:], columns=data["data"][0])
+        elif self.request_format == "csv":
+            df = pd.read_csv(io.StringIO(response.text), low_memory=False)
+
+        has_next_page = response.headers["x-has-next-page"] == "true"
+
+        return df, has_next_page
 
     def list_datasets(self, filter_term=None, return_list=False):
         """List available datasets from the API,
         with optional filter and return list option.
 
         Parameters:
             filter_term (str, optional): The term to match against
@@ -81,21 +115,19 @@
 
         Returns:
             list, None: The filtered datasets as a list if
                 return_list is set to True, otherwise None.
         """
         url = f"{self.host}/datasets/"
 
-        response = self.get(url)
-
-        data = response.json()
+        df, has_next_page = self.get(url)
 
         matched_datasets = []
 
-        for dataset in data["data"]:
+        for dataset in df.to_dict("records"):
             dataset_description = dataset.get("description", "")
             if dataset_description is None:
                 dataset_description = ""
             if filter_term is None or (
                 filter_term.lower() in dataset["id"].lower()
                 or filter_term.lower() in dataset["name"].lower()
                 or filter_term.lower() in dataset_description.lower()
@@ -208,15 +240,14 @@
         while has_next_page:
             start_time = time.time()
 
             params = {
                 "start_time": start,
                 "end_time": end,
                 "limit": limit,
-                "return_format": "csv",
                 "page": page,
                 "max_rows": max_rows,
             }
             url = f"{self.host}/datasets/{dataset}/query/"
             if filter_column is not None:
                 if isinstance(filter_value, list) and filter_operator == "in":
                     filter_value = ",".join(filter_value)
@@ -227,20 +258,18 @@
 
             if columns is not None:
                 params["columns"] = ",".join(columns)
 
             # Log the fetching message
             log(f"Fetching Page {page}...", verbose, end="")
 
-            response = self.get(url, params=params, verbose=verbose)
+            df, has_next_page = self.get(url, params=params, verbose=verbose)
 
-            df = pd.read_csv(io.StringIO(response.text))
             dfs.append(df)
 
-            has_next_page = response.headers["x-has-next-page"] == "true"
             response_time = time.time() - start_time
             total_time += response_time
             avg_time_per_page = total_time / page
 
             # Update the fetching message with the done message
             if page == 1:
                 log(
@@ -275,15 +304,15 @@
         # convert to datetime for any columns that end in _utc
         # or are of type object
         for col in df.columns:
             if df[col].dtype == "object" or col.endswith("_utc"):
                 try:
                     df[col] = pd.to_datetime(
                         df[col],
-                        format="%Y-%m-%d %H:%M:%S%z",
+                        format="ISO8601",
                         utc=True,
                     )
 
                     if tz != "UTC":
                         df[col] = df[col].dt.tz_convert(tz)
                         # rename with _utc suffix
                         df = df.rename(
```

### Comparing `gridstatusio-0.3.1/gridstatusio/tests/test_api.py` & `gridstatusio-0.4.0/gridstatusio/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `gridstatusio-0.3.1/gridstatusio.egg-info/PKG-INFO` & `gridstatusio-0.4.0/gridstatusio.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridstatusio
-Version: 0.3.1
+Version: 0.4.0
 Summary: Python Client for GridStatus.io API
 Author-email: Max Kanter <kmax12@gmail.com>
 Maintainer-email: Max Kanter <kmax12@gmail.com>
 License: Copyright 2022 James Max Kanter
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
```

### Comparing `gridstatusio-0.3.1/pyproject.toml` & `gridstatusio-0.4.0/pyproject.toml`

 * *Files identical despite different names*

