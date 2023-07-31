# Comparing `tmp/sas-airflow-provider-0.0.6.tar.gz` & `tmp/sas-airflow-provider-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/sas-airflow-provider/sas-airflow-provider/dist/.tmp-gmcu142n/sas-airflow-provider-0.0.6.tar", last modified: Fri Jul 28 17:39:23 2023, max compression
+gzip compressed data, was "/home/runner/work/sas-airflow-provider/sas-airflow-provider/dist/.tmp-fwdlq0ld/sas-airflow-provider-0.0.7.tar", last modified: Mon Jul 31 16:06:24 2023, max compression
```

## Comparing `sas-airflow-provider-0.0.6.tar` & `sas-airflow-provider-0.0.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:39:23.000000 sas-airflow-provider-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-28 17:39:10.000000 sas-airflow-provider-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-07-28 17:39:23.000000 sas-airflow-provider-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-28 17:39:10.000000 sas-airflow-provider-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-28 17:39:10.000000 sas-airflow-provider-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-28 17:39:23.000000 sas-airflow-provider-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:39:23.000000 sas-airflow-provider-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:39:23.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-28 17:39:10.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:39:23.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/example_dags/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-28 17:39:10.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/example_dags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-28 17:39:10.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/example_dags/example_sas_jobexecution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-28 17:39:10.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/example_dags/example_sas_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-28 17:39:10.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/example_dags/example_studio_advanced.py
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-07-28 17:39:10.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/example_dags/example_templating.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:39:23.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-28 17:39:10.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-28 17:39:10.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/hooks/sas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:39:23.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/operators/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-28 17:39:10.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-07-28 17:39:10.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/operators/sas_create_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-28 17:39:10.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/operators/sas_jobexecution.py
--rw-r--r--   0 runner    (1001) docker     (123)    12577 2023-07-28 17:39:10.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/operators/sas_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)    10380 2023-07-28 17:39:10.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/operators/sas_studioflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:39:23.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/util/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-28 17:39:10.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-07-28 17:39:10.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider/util/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:39:23.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-07-28 17:39:23.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-28 17:39:23.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 17:39:23.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-28 17:39:23.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 17:39:23.000000 sas-airflow-provider-0.0.6/src/sas_airflow_provider.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:06:24.000000 sas-airflow-provider-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-31 16:05:56.000000 sas-airflow-provider-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-07-31 16:06:24.000000 sas-airflow-provider-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-31 16:05:56.000000 sas-airflow-provider-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-31 16:05:56.000000 sas-airflow-provider-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-31 16:06:24.000000 sas-airflow-provider-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:06:24.000000 sas-airflow-provider-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:06:24.000000 sas-airflow-provider-0.0.7/src/sas_airflow_provider/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-31 16:05:56.000000 sas-airflow-provider-0.0.7/src/sas_airflow_provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:06:24.000000 sas-airflow-provider-0.0.7/src/sas_airflow_provider/example_dags/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-31 16:05:56.000000 sas-airflow-provider-0.0.7/src/sas_airflow_provider/example_dags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-31 16:05:56.000000 sas-airflow-provider-0.0.7/src/sas_airflow_provider/example_dags/example_sas_jobexecution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-31 16:05:56.000000 sas-airflow-provider-0.0.7/src/sas_airflow_provider/example_dags/example_sas_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-31 16:05:56.000000 sas-airflow-provider-0.0.7/src/sas_airflow_provider/example_dags/example_studio_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-07-31 16:05:56.000000 sas-airflow-provider-0.0.7/src/sas_airflow_provider/example_dags/example_templating.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:06:24.000000 sas-airflow-provider-0.0.7/src/sas_airflow_provider/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-31 16:05:56.000000 sas-airflow-provider-0.0.7/src/sas_airflow_provider/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-31 16:05:56.000000 sas-airflow-provider-0.0.7/src/sas_airflow_provider/hooks/sas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:06:24.000000 sas-airflow-provider-0.0.7/src/sas_airflow_provider/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-31 16:05:56.000000 sas-airflow-provider-0.0.7/src/sas_airflow_provider/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-07-31 16:05:56.000000 sas-airflow-provider-0.0.7/src/sas_airflow_provider/operators/sas_create_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-07-31 16:05:56.000000 sas-airflow-provider-0.0.7/src/sas_airflow_provider/operators/sas_jobexecution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12577 2023-07-31 16:05:56.000000 sas-airflow-provider-0.0.7/src/sas_airflow_provider/operators/sas_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10380 2023-07-31 16:05:56.000000 sas-airflow-provider-0.0.7/src/sas_airflow_provider/operators/sas_studioflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:06:24.000000 sas-airflow-provider-0.0.7/src/sas_airflow_provider/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-31 16:05:56.000000 sas-airflow-provider-0.0.7/src/sas_airflow_provider/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-07-31 16:05:56.000000 sas-airflow-provider-0.0.7/src/sas_airflow_provider/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:06:24.000000 sas-airflow-provider-0.0.7/src/sas_airflow_provider.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-07-31 16:06:24.000000 sas-airflow-provider-0.0.7/src/sas_airflow_provider.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-31 16:06:24.000000 sas-airflow-provider-0.0.7/src/sas_airflow_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 16:06:24.000000 sas-airflow-provider-0.0.7/src/sas_airflow_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-31 16:06:24.000000 sas-airflow-provider-0.0.7/src/sas_airflow_provider.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-31 16:06:24.000000 sas-airflow-provider-0.0.7/src/sas_airflow_provider.egg-info/top_level.txt
```

### Comparing `sas-airflow-provider-0.0.6/LICENSE` & `sas-airflow-provider-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.6/PKG-INFO` & `sas-airflow-provider-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sas-airflow-provider
-Version: 0.0.6
+Version: 0.0.7
 Summary: Enables execution of Studio Flows and Jobs from Airflow
 Home-page: https://github.com/sassoftware/sas-airflow-provider
 Author: SAS
 Author-email: andrew.shakinovsky@sas.com
 Project-URL: Bug Tracker, https://github.com/sassoftware
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `sas-airflow-provider-0.0.6/README.md` & `sas-airflow-provider-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.6/setup.cfg` & `sas-airflow-provider-0.0.7/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sas-airflow-provider
-version = 0.0.6
+version = 0.0.7
 author = SAS
 author_email = andrew.shakinovsky@sas.com
 description = Enables execution of Studio Flows and Jobs from Airflow
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sassoftware/sas-airflow-provider
 project_urls =
```

### Comparing `sas-airflow-provider-0.0.6/src/sas_airflow_provider/example_dags/__init__.py` & `sas-airflow-provider-0.0.7/src/sas_airflow_provider/example_dags/__init__.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.6/src/sas_airflow_provider/example_dags/example_sas_jobexecution.py` & `sas-airflow-provider-0.0.7/src/sas_airflow_provider/example_dags/example_sas_jobexecution.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.6/src/sas_airflow_provider/example_dags/example_sas_studio.py` & `sas-airflow-provider-0.0.7/src/sas_airflow_provider/example_dags/example_sas_studio.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.6/src/sas_airflow_provider/example_dags/example_studio_advanced.py` & `sas-airflow-provider-0.0.7/src/sas_airflow_provider/example_dags/example_studio_advanced.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.6/src/sas_airflow_provider/example_dags/example_templating.py` & `sas-airflow-provider-0.0.7/src/sas_airflow_provider/example_dags/example_templating.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.6/src/sas_airflow_provider/hooks/__init__.py` & `sas-airflow-provider-0.0.7/src/sas_airflow_provider/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.6/src/sas_airflow_provider/hooks/sas.py` & `sas-airflow-provider-0.0.7/src/sas_airflow_provider/hooks/sas.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.6/src/sas_airflow_provider/operators/__init__.py` & `sas-airflow-provider-0.0.7/src/sas_airflow_provider/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.6/src/sas_airflow_provider/operators/sas_create_session.py` & `sas-airflow-provider-0.0.7/src/sas_airflow_provider/operators/sas_create_session.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.6/src/sas_airflow_provider/operators/sas_jobexecution.py` & `sas-airflow-provider-0.0.7/src/sas_airflow_provider/operators/sas_jobexecution.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 
 from __future__ import annotations
 
+import os
 import urllib.parse
 
 from airflow.exceptions import AirflowFailException
 from airflow.models import BaseOperator
 from sas_airflow_provider.hooks.sas import SasHook
 from sas_airflow_provider.util.util import dump_logs
 
@@ -32,35 +33,54 @@
     The specific endpoint /SASJobExecution is documented here:
     https://go.documentation.sas.com/doc/en/pgmsascdc/default/jobexecug/n06tcybrt9wdeun1ko9bkjn0ko0b.htm
 
     :param connection_name: Name of the SAS Viya connection stored as an Airflow HTTP connection
     :param job_name: Name of the SAS Job to be run
     :param parameters Dictionary of all the parameters that should be passed to the
         SAS Job as SAS Macro variables
-    :param job_exec_log: boolean. whether or not to dump out the log
+    :param job_exec_log: boolean. whether or not to dump out the log (default is false)
+    :param add_airflow_vars: boolean. whether or not to add airflow environment variables as macro variables
+       (default is false)
     """
 
     template_fields: Sequence[str] = ("parameters",)
 
     def __init__(self,
                  job_name: str,
                  parameters: dict,
                  connection_name: str = None,
                  job_exec_log: bool = False,
+                 add_airflow_vars: bool = False,
                  **kwargs) -> None:
         super().__init__(**kwargs)
         self.connection_name = connection_name
         self.job_name = job_name
         self.parameters = parameters
         self.job_exec_log = job_exec_log
+        self.add_airflow_vars = add_airflow_vars
+
+    def _add_airflow_env_vars(self):
+        for x in ['AIRFLOW_CTX_DAG_OWNER',
+                  'AIRFLOW_CTX_DAG_ID',
+                  'AIRFLOW_CTX_TASK_ID',
+                  'AIRFLOW_CTX_EXECUTION_DATE',
+                  'AIRFLOW_CTX_TRY_NUMBER',
+                  'AIRFLOW_CTX_DAG_RUN_ID', ]:
+            v = os.getenv(x)
+            if v:
+                self.parameters[x] = v
 
     def execute(self, context):
         h = SasHook(self.connection_name)
         session = h.get_conn()
 
+        if self.add_airflow_vars:
+            print(f"Add Airflow variables as parameters")
+            self._add_airflow_env_vars()
+
         print(f"Executing SAS job: {self.job_name}")
         # url escape the program name
         program_name = urllib.parse.quote(self.job_name)
         url_string = ""
         for key, value in self.parameters.items():
             url_string += f"&{key}={urllib.parse.quote(value)}"
```

### Comparing `sas-airflow-provider-0.0.6/src/sas_airflow_provider/operators/sas_studio.py` & `sas-airflow-provider-0.0.7/src/sas_airflow_provider/operators/sas_studio.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.6/src/sas_airflow_provider/operators/sas_studioflow.py` & `sas-airflow-provider-0.0.7/src/sas_airflow_provider/operators/sas_studioflow.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.6/src/sas_airflow_provider/util/__init__.py` & `sas-airflow-provider-0.0.7/src/sas_airflow_provider/util/__init__.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.6/src/sas_airflow_provider/util/util.py` & `sas-airflow-provider-0.0.7/src/sas_airflow_provider/util/util.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.6/src/sas_airflow_provider.egg-info/PKG-INFO` & `sas-airflow-provider-0.0.7/src/sas_airflow_provider.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sas-airflow-provider
-Version: 0.0.6
+Version: 0.0.7
 Summary: Enables execution of Studio Flows and Jobs from Airflow
 Home-page: https://github.com/sassoftware/sas-airflow-provider
 Author: SAS
 Author-email: andrew.shakinovsky@sas.com
 Project-URL: Bug Tracker, https://github.com/sassoftware
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `sas-airflow-provider-0.0.6/src/sas_airflow_provider.egg-info/SOURCES.txt` & `sas-airflow-provider-0.0.7/src/sas_airflow_provider.egg-info/SOURCES.txt`

 * *Files identical despite different names*

