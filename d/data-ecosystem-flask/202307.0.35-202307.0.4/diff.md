# Comparing `tmp/data_ecosystem_flask-202307.0.35.tar.gz` & `tmp/data_ecosystem_flask-202307.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_ecosystem_flask-202307.0.35.tar", max compression
+gzip compressed data, was "data_ecosystem_flask-202307.0.4.tar", max compression
```

## Comparing `data_ecosystem_flask-202307.0.35.tar` & `data_ecosystem_flask-202307.0.4.tar`

### file list

```diff
@@ -1,38 +1,17 @@
--rw-r--r--   0        0        0      591 2023-07-31 01:30:10.011105 data_ecosystem_flask-202307.0.35/data_ecosystem_flask/.env
--rw-r--r--   0        0        0      863 2023-07-28 12:14:08.336487 data_ecosystem_flask-202307.0.35/data_ecosystem_flask/Makefile.ps1
--rw-r--r--   0        0        0     1155 2023-07-28 12:14:08.339487 data_ecosystem_flask-202307.0.35/data_ecosystem_flask/__init__.py
--rw-r--r--   0        0        0    44698 2023-07-31 01:23:52.403322 data_ecosystem_flask-202307.0.35/data_ecosystem_flask/app.py
--rw-r--r--   0        0        0    13809 2023-07-31 01:18:04.017924 data_ecosystem_flask-202307.0.35/data_ecosystem_flask/app_startup.py
--rw-r--r--   0        0        0     5341 2023-07-31 01:30:09.997114 data_ecosystem_flask-202307.0.35/data_ecosystem_flask/config/config.dev.json
--rw-r--r--   0        0        0     5071 2023-07-31 01:30:10.000106 data_ecosystem_flask-202307.0.35/data_ecosystem_flask/config/config.prod.json
--rw-r--r--   0        0        0      344 2023-07-31 01:30:10.003103 data_ecosystem_flask-202307.0.35/data_ecosystem_flask/config/manifest.json
--rw-r--r--   0        0        0    59440 2023-07-31 01:30:09.987109 data_ecosystem_flask-202307.0.35/data_ecosystem_flask/excel-manifest-schema.xlsx
--rw-r--r--   0        0        0    24571 2023-07-31 01:30:09.977101 data_ecosystem_flask-202307.0.35/data_ecosystem_flask/excel_manifest_schema_for_schemas_sql.xlsx
--rw-r--r--   0        0        0    12829 2023-07-31 01:30:09.974097 data_ecosystem_flask-202307.0.35/data_ecosystem_flask/excel_manifest_schema_for_schemas_sql_merged.xlsx
--rw-r--r--   0        0        0    27811 2023-07-31 01:30:09.980108 data_ecosystem_flask-202307.0.35/data_ecosystem_flask/excel_manifest_schema_for_tables_sql.xlsx
--rw-r--r--   0        0        0    38559 2023-07-31 01:30:09.984097 data_ecosystem_flask-202307.0.35/data_ecosystem_flask/excel_manifest_schema_valuesets.xlsx
--rw-r--r--   0        0        0    28571 2023-07-28 12:14:08.351488 data_ecosystem_flask-202307.0.35/data_ecosystem_flask/install.py
--rw-r--r--   0        0        0    14945 2023-07-31 01:30:09.963099 data_ecosystem_flask-202307.0.35/data_ecosystem_flask/json-manifest-schema.json
--rw-r--r--   0        0        0      344 2023-07-28 20:05:27.819214 data_ecosystem_flask-202307.0.35/data_ecosystem_flask/manifest.json
--rw-r--r--   0        0        0    14015 2023-07-31 01:30:09.965112 data_ecosystem_flask-202307.0.35/data_ecosystem_flask/manifest.schema.json
--rw-r--r--   0        0        0    11000 2023-07-31 01:30:12.842088 data_ecosystem_flask-202307.0.35/data_ecosystem_flask/requirements.txt
--rw-r--r--   0        0        0     2283 2023-07-28 12:14:08.362487 data_ecosystem_flask-202307.0.35/data_ecosystem_flask/templates/download.html
--rw-r--r--   0        0        0      432 2023-07-28 12:14:08.365485 data_ecosystem_flask-202307.0.35/data_ecosystem_flask/templates/error.html
--rw-r--r--   0        0        0     2723 2023-07-28 12:14:08.367490 data_ecosystem_flask-202307.0.35/data_ecosystem_flask/templates/log_file.html
--rw-r--r--   0        0        0     1905 2023-07-28 12:14:08.370482 data_ecosystem_flask-202307.0.35/data_ecosystem_flask/templates/upload.html
--rw-r--r--   0        0        0    59440 2023-07-27 10:12:39.655773 data_ecosystem_flask-202307.0.35/dev_schema/excel-manifest-schema.xlsx
--rw-r--r--   0        0        0    24571 2023-07-27 10:12:39.658771 data_ecosystem_flask-202307.0.35/dev_schema/excel_manifest_schema_for_schemas_sql.xlsx
--rw-r--r--   0        0        0    12829 2023-07-27 10:12:39.660775 data_ecosystem_flask-202307.0.35/dev_schema/excel_manifest_schema_for_schemas_sql_merged.xlsx
--rw-r--r--   0        0        0    27811 2023-07-27 10:12:39.663772 data_ecosystem_flask-202307.0.35/dev_schema/excel_manifest_schema_for_tables_sql.xlsx
--rw-r--r--   0        0        0    38559 2023-07-27 10:12:39.666775 data_ecosystem_flask-202307.0.35/dev_schema/excel_manifest_schema_valuesets.xlsx
--rw-r--r--   0        0        0    14945 2023-07-27 10:12:39.669778 data_ecosystem_flask-202307.0.35/dev_schema/json-manifest-schema.json
--rw-r--r--   0        0        0    14015 2023-07-27 10:12:39.671783 data_ecosystem_flask-202307.0.35/dev_schema/manifest.schema.json
--rw-r--r--   0        0        0    11368 2023-07-30 21:12:34.051256 data_ecosystem_flask-202307.0.35/license.md
--rw-r--r--   0        0        0     5341 2023-07-31 00:45:49.413323 data_ecosystem_flask-202307.0.35/ocio/ocio_pade_dev/config/config.dev.json
--rw-r--r--   0        0        0     5071 2023-07-30 01:26:52.658842 data_ecosystem_flask-202307.0.35/ocio/ocio_pade_dev/config/config.prod.json
--rw-r--r--   0        0        0      344 2023-07-30 01:26:52.662843 data_ecosystem_flask-202307.0.35/ocio/ocio_pade_dev/config/manifest.json
--rw-r--r--   0        0        0     2895 2023-07-31 01:31:28.631263 data_ecosystem_flask-202307.0.35/pyproject.toml
--rw-r--r--   0        0        0    15040 2023-07-27 10:12:39.687768 data_ecosystem_flask-202307.0.35/readme.md
--rw-r--r--   0        0        0      126 2023-06-30 18:22:06.511392 data_ecosystem_flask-202307.0.35/setup.cfg
--rw-r--r--   0        0        0      127 2023-06-30 18:22:06.514388 data_ecosystem_flask-202307.0.35/setup.py
--rw-r--r--   0        0        0     1889 1970-01-01 00:00:00.000000 data_ecosystem_flask-202307.0.35/PKG-INFO
+-rw-r--r--   0        0        0      863 2023-07-18 10:51:23.854973 data_ecosystem_flask-202307.0.4/data_ecosystem_flask/Makefile.ps1
+-rw-r--r--   0        0        0     1155 2023-07-18 10:51:23.854973 data_ecosystem_flask-202307.0.4/data_ecosystem_flask/__init__.py
+-rw-r--r--   0        0        0    42638 2023-07-18 10:51:23.854973 data_ecosystem_flask-202307.0.4/data_ecosystem_flask/app.py
+-rw-r--r--   0        0        0    13336 2023-07-18 10:51:23.854973 data_ecosystem_flask-202307.0.4/data_ecosystem_flask/app_startup.py
+-rw-r--r--   0        0        0    28571 2023-07-18 10:51:23.854973 data_ecosystem_flask-202307.0.4/data_ecosystem_flask/install.py
+-rw-r--r--   0        0        0     2082 2023-07-18 10:51:23.854973 data_ecosystem_flask-202307.0.4/data_ecosystem_flask/manifest.json
+-rw-r--r--   0        0        0    16945 2023-07-18 10:51:23.854973 data_ecosystem_flask-202307.0.4/data_ecosystem_flask/requirements.txt
+-rw-r--r--   0        0        0     1572 2023-07-18 10:51:23.854973 data_ecosystem_flask-202307.0.4/data_ecosystem_flask/templates/download.html
+-rw-r--r--   0        0        0      432 2023-07-18 10:51:23.854973 data_ecosystem_flask-202307.0.4/data_ecosystem_flask/templates/error.html
+-rw-r--r--   0        0        0     2723 2023-07-18 10:51:23.854973 data_ecosystem_flask-202307.0.4/data_ecosystem_flask/templates/log_file.html
+-rw-r--r--   0        0        0     1905 2023-07-18 10:51:23.854973 data_ecosystem_flask-202307.0.4/data_ecosystem_flask/templates/upload.html
+-rw-r--r--   0        0        0    11357 2023-07-18 10:51:23.906975 data_ecosystem_flask-202307.0.4/license.md
+-rw-r--r--   0        0        0     2559 2023-07-18 10:59:22.927276 data_ecosystem_flask-202307.0.4/pyproject.toml
+-rw-r--r--   0        0        0    15040 2023-07-18 10:51:23.910975 data_ecosystem_flask-202307.0.4/readme.md
+-rw-r--r--   0        0        0      126 2023-07-18 10:51:23.910975 data_ecosystem_flask-202307.0.4/setup.cfg
+-rw-r--r--   0        0        0      127 2023-07-18 10:51:23.910975 data_ecosystem_flask-202307.0.4/setup.py
+-rw-r--r--   0        0        0     1796 1970-01-01 00:00:00.000000 data_ecosystem_flask-202307.0.4/PKG-INFO
```

### Comparing `data_ecosystem_flask-202307.0.35/data_ecosystem_flask/Makefile.ps1` & `data_ecosystem_flask-202307.0.4/data_ecosystem_flask/Makefile.ps1`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.35/data_ecosystem_flask/__init__.py` & `data_ecosystem_flask-202307.0.4/data_ecosystem_flask/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.35/data_ecosystem_flask/app.py` & `data_ecosystem_flask-202307.0.4/data_ecosystem_flask/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,30 +30,15 @@
 from datetime import datetime
 from werkzeug.datastructures import FileStorage
 from requests.exceptions import RequestException
 from flask import redirect, send_file, request, render_template, Blueprint, g, jsonify, make_response, Response
 from flask_restx import Api, Resource, fields, Namespace, reqparse, marshal_with
 from opentelemetry.instrumentation.flask import FlaskInstrumentor
 from azure.monitor.opentelemetry.exporter import AzureMonitorMetricExporter
-
-try:
-    from data_ecosystem_flask.app_startup import create_api, create_app
-except ModuleNotFoundError:
-    try:
-        from .app_startup import create_api, create_app
-    except ModuleNotFoundError:
-        try:
-            from app_startup import create_api, create_app
-        except ModuleNotFoundError:
-            trace_msg = traceback.format_exc()
-            line_number = traceback.extract_tb(ex.__traceback__)[-1].lineno
-            error_message = f"An unexpected error occurred: {ex} at line {line_number}\nCall Stack:{trace_msg}"
-            exc_info = sys.exc_info()
-            # logger_singleton.error_with_exception(error_message, exc_info)
-            raise ModuleNotFoundError
+from data_ecosystem_flask.app_startup import create_api, create_app
 
 from data_ecosystem_services.alation_service import (
     schema as pade_schema
 )
 from data_ecosystem_services.cdc_tech_environment_service import (
     environment_file as pade_env_file
 )
@@ -73,15 +58,14 @@
 
 TIMEOUT_5_SEC = 5
 TIMEOUT_ONE_MIN = 60
 # Get the currently running file name
 SERVICE_NAME = os.path.basename(__file__)
 # Get the parent folder name of the running file
 NAMESPACE_NAME = os.path.basename(os.path.dirname(__file__))
-ENVIRONMENT = 'dev'
 
 print(f"SERVICE_NAME:{SERVICE_NAME}")
 print(f"NAMESPACE_NAME: {NAMESPACE_NAME}")
 sys.path.append(os.getcwd())
 app_dir = os.path.dirname(os.path.abspath(__file__))
 sys.path.append(app_dir)
 
@@ -151,19 +135,17 @@
     return render_template('error.html', error_message=error_message)
 
 
 @cdc_admin_bp.route('/get_log_file_tail/<int:number_of_lines>')
 def get_log_file_tail(number_of_lines):
     """Get the last n lines of the log file"""
 
-    try:
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(calling_namespace_name=NAMESPACE_NAME, calling_service_name=SERVICE_NAME)
-    except TypeError as e:
-        # If a TypeError occurs, retry the call with no parameters
-        logger_singleton = pade_env_logging.LoggerSingleton.instance()
+    logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        NAMESPACE_NAME, SERVICE_NAME)
+    logger = logger_singleton.get_logger()
 
     with tracer.start_as_current_span(f"get_log_file_tail"):
 
         try:
 
             log_data = None
 
@@ -205,38 +187,40 @@
             return render_template('log_file.html', entries=log_entries)
 
         except Exception as ex:
             trace_msg = traceback.format_exc()
             line_number = traceback.extract_tb(ex.__traceback__)[-1].lineno
             error_message = f"An unexpected error occurred: {ex} at line {line_number}\nCall Stack:{trace_msg}"
             exc_info = sys.exc_info()
-            # logger_singleton.error_with_exception(error_message, exc_info)
+            logger_singleton.error_with_exception(error_message, exc_info)
             return render_template('error.html', error_message=error_message)
 
 
 app.register_blueprint(cdc_admin_bp)
 app.register_blueprint(cdc_files_bp)
 
 metric_exporter = AzureMonitorMetricExporter()
 
 logger = app.logger
+logger_singleton = pade_env_logging.LoggerSingleton.instance(
+    NAMESPACE_NAME, SERVICE_NAME)
 tracer = app.tracer
 
 FlaskInstrumentor().instrument_app(app)
 
 API_DESCRIPTION = '''
 <h2>API Documentation</h2>
 <p>The Program Agnostic Data Ecosystem (PADE) provides shared resources,
 practices and guardrails for analysts to discover, access, link, and use
 agency data in a consistent way. PADE improvements in standardized and 
 streamlined workflows reduce the effort required to find, access, and
 trust data.</p>
-<p><a href="files/upload">Upload Page</a></p>
-<p><a href="files/download">Download Page</a></p>
-<p>For detailed logs, please visit the <a href="logs/get_log_file_tail/1000">Log File Page</a>.</p>
+<p><a href="/files/upload">Upload Page</a></p>
+<p><a href="/files/download">Download Page</a></p>
+<p>For detailed logs, please visit the <a href="/logs/get_log_file_tail/1000">Log File Page</a>.</p>
 '''
 
 api, ns_welcome, ns_alation, ns_jira, ns_posit, ns_cdc_admin, ns_cdc_security = create_api(
     app, API_DESCRIPTION)
 
 # Define a model for the metadata
 metadata_model = api.model('Metadata', {
@@ -327,20 +311,14 @@
         Note:
             This method communicates with JIRA to fetch the tasks.
 
         Example: DTEDS
 
         """
 
-        try:
-            logger_singleton = pade_env_logging.LoggerSingleton.instance(calling_namespace_name=NAMESPACE_NAME, calling_service_name=SERVICE_NAME)
-        except TypeError as e:
-            # If a TypeError occurs, retry the call with no parameters
-            logger_singleton = pade_env_logging.LoggerSingleton.instance()
-            
         with tracer.start_as_current_span(f"tasks/{project}"):
             try:
 
                 config = app.cdc_config
 
                 jira_client_secret_key = config.get("jira_client_secret_key")
                 az_kv_jira_env_var = jira_client_secret_key.replace("-", "_")
@@ -393,15 +371,15 @@
                         return {"tasks": tasks}
                     except ValueError:
                         msg = f"Failed to retrieve json tasks from url: {url}."
                         msg = msg + f" parms:{params}"
                         msg = msg + "response_jira_tasks_content:"
                         msg = msg + f"{response_jira_tasks_content}"
                         exc_info = sys.exc_info()
-                        # logger_singleton.error_with_exception(msg, exc_info)
+                        logger_singleton.error_with_exception(msg, exc_info)
                         logger_singleton.force_flush()
                         return {"error": msg}
                 else:
                     msg = f"Failed to retrieve tasks from url:{url}"
                     msg = msg + \
                         f": status_code: {response_jira_tasks.status_code}"
                     msg = msg + ": response_jira_tasks_content:"
@@ -412,21 +390,21 @@
                                 "message"]
                         except ValueError:
                             error_message = "Failed to retrieve json from url:"
                             error_message = error_message + \
                                 f"{url}: params: {params}."
                     msg = msg + ": error_message: " + error_message
                     exc_info = sys.exc_info()
-                    # logger_singleton.error_with_exception(msg, exc_info)
+                    logger_singleton.error_with_exception(msg, exc_info)
                     logger_singleton.force_flush()
                     return {"error": msg}
             except Exception as ex:
                 msg = f"An unexpected error occurred: {str(ex)}"
                 exc_info = sys.exc_info()
-                # logger_singleton.error_with_exception(msg, exc_info)
+                logger_singleton.error_with_exception(msg, exc_info)
                 logger_singleton.force_flush()
                 return {"error": f"An unexpected error occurred: {msg}"}
 
 
 class MetadataJsonFileDownload(Resource):
     """
     A Flask-RESTful resource responsible for downloading metadata JSON files.
@@ -453,21 +431,14 @@
             dict: A dictionary containing the downloaded JSON metadata file.
 
         Example:
             Use schema_id 106788 to test OCIO_PADE_DEV (DataBricks): ocio_pade_dev
             Use schema_id 1464 to test Acme Bookstore (Synapse SQL Warehouse): EDAV.alation
         """
 
-        try:
-            logger_singleton = pade_env_logging.LoggerSingleton.instance(calling_namespace_name=NAMESPACE_NAME, calling_service_name=SERVICE_NAME)
-        except TypeError as e:
-            # If a TypeError occurs, retry the call with no parameters
-            logger_singleton = pade_env_logging.LoggerSingleton.instance()
-
-
         with tracer.start_as_current_span(f"metadata_json_file_download/{schema_id}"):
             try:
 
                 start_time = time.time()  # Record the start time
 
                 config = app.cdc_config
 
@@ -484,15 +455,15 @@
 
                 # Return the file as a response
                 return send_file(manifest_json_file, as_attachment=True, download_name=file_name)
 
             except Exception as ex:
                 msg = f"An unexpected error occurred for download file for schema_id: {schema_id}: {str(ex)}"
                 exc_info = sys.exc_info()
-                # logger_singleton.error_with_exception(msg, exc_info)
+                logger_singleton.error_with_exception(msg, exc_info)
                 logger_singleton.force_flush()
                 response = make_response(jsonify({"error": str(ex)}), 500)
                 return response
 
 
 class MetadataExcelFileDownload(Resource):
     """
@@ -522,38 +493,24 @@
             dict: A dictionary containing the downloaded Excel metadata file.
 
         Example:
             Use schema_id 106788 to test OCIO_PADE_DEV (DataBricks): ocio_pade_dev
             Use schema_id 1464 to test Acme Bookstore (Synapse SQL Warehouse): EDAV.alationn
         """
 
-        try:
-            logger_singleton = pade_env_logging.LoggerSingleton.instance(calling_namespace_name=NAMESPACE_NAME, calling_service_name=SERVICE_NAME)
-        except TypeError as e:
-            # If a TypeError occurs, retry the call with no parameters
-            logger_singleton = pade_env_logging.LoggerSingleton.instance()
-            
         with tracer.start_as_current_span(f"metadata_excel_file_download/{schema_id}"):
             try:
 
                 start_time = time.time()  # Record the start time
 
                 config = app.cdc_config
 
-                obj_file = pade_env_file.EnvironmentFile()
-                app_dir = os.path.dirname(os.path.abspath(__file__))
-                parent_dir = os.path.dirname(app_dir)
-
-                schema_path = parent_dir + "/" + ENVIRONMENT + "_schema/"
-                schema_path = obj_file.convert_to_current_os_dir(schema_path)
-                schema_file = schema_path + "excel_manifest_schema_for_tables_sql.xlsx"
-
                 schema = pade_schema.Schema()
                 manifest_excel_file = schema.download_schema_manifest_excel_file(
-                    schema_id, config, schema_file)
+                    schema_id, config)
 
                 # Return the file as a download
                 file_name = os.path.basename(manifest_excel_file)
                 logger.info(f"file_name:{file_name}")
 
                 end_time = time.time()  # Record the start time
 
@@ -572,15 +529,15 @@
 
                 # Return the file as a response
                 return send_file(manifest_excel_file, as_attachment=True, download_name=file_name)
 
             except Exception as ex:
                 msg = f"An unexpected error occurred for download file for schema_id: {schema_id}: {str(ex)}"
                 exc_info = sys.exc_info()
-                # logger_singleton.error_with_exception(msg, exc_info)
+                logger_singleton.error_with_exception(msg, exc_info)
                 logger_singleton.force_flush()
                 response = make_response(jsonify({"error": str(ex)}), 500)
                 return response
 
 
 class MetadataExcelFileUpload(Resource):
     """
@@ -667,14 +624,15 @@
 
 class ConnectApiKeyVerification(Resource):
     """
     A Flask-RESTful resource for handling the verification of API keys.
 
     """
 
+    @enforce_https
     def get(self):
         """
         Verifies the key stored in key vault based on configuration setting: az_kv_posit_connect_secret_key
 
         Returns:
             tuple: A tuple containing the status code and response from the server.
             The response will be in JSON format if possible, otherwise it will be the raw text response.
@@ -704,14 +662,15 @@
 
 class DeploymentBundle(Resource):
     """
     A Flask-RESTful resource for handling POSIT Deployment Bundle.
 
     """
 
+    @enforce_https
     def get(self, content_id, bundle_id):
         """
         Generates DeploymentBundle
 
         Returns:
             tuple: A tuple containing the status code and response from the server.
             The response will be in JSON format if possible, otherwise it will be the raw text response.
@@ -741,14 +700,15 @@
 
 class PythonInformation(Resource):
     """
     A Flask-RESTful resource for handling POSIT Python Information.
 
     """
 
+    @enforce_https
     def get(self):
         """
         Generates python information about POSIT
 
         Returns:
             tuple: A tuple containing the status code and response from the server.
             The response will be in JSON format if possible, otherwise it will be the raw text response.
@@ -779,14 +739,15 @@
 
 class GeneratedManifest(Resource):
     """
     A Flask-RESTful resource for handling POSIT Manifest Generation
 
     """
 
+    @enforce_https
     def get(self):
         """
         Generates manifest JSON
 
         Returns:
             tuple: A tuple containing the status code and response from the server.
             The response will be in JSON format if possible, otherwise it will be the raw text response.
@@ -899,14 +860,15 @@
 
 class PublishManifest(Resource):
     """
     A Flask-RESTful resource for handling POSIT Manifest Publication
 
     """
 
+    @enforce_https
     def get(self):
         """
         Publishes manifest JSON
 
         Returns:
             tuple: A tuple containing the status code and response from the server.
             The response will be in JSON format if possible, otherwise it will be the raw text response.
@@ -959,14 +921,15 @@
 
 class ContentList(Resource):
     """
     A Flask-RESTful resource for handling POSIT Content Lists
 
     """
 
+    @enforce_https
     def get(self):
         """
         Retrieves the manifest JSON for the content list.
 
         Returns:
             tuple: A tuple containing the status code and response from the server.
                    The response will be in JSON format if possible, otherwise it will be the raw text response.
@@ -994,14 +957,15 @@
 
 class DeploymentBundleList(Resource):
     """
     A Flask-RESTful resource for handling POSIT Bundle Lists
 
     """
 
+    @enforce_https
     def get(self, content_id):
         """
         Publishes manifest JSON
 
         Returns:
             tuple: A tuple containing the status code and response from the server.
             The response will be in JSON format if possible, otherwise it will be the raw text response.
@@ -1031,14 +995,15 @@
 
 class TaskStatus(Resource):
     """
     A Flask-RESTful resource for handling POSIT Bundle Lists
 
     """
 
+    @enforce_https
     def get(self, task_id):
         """
         Gets Task Status
 
         Returns:
             tuple: A tuple containing the status code and response from the server.
             The response will be in JSON format if possible, otherwise it will be the raw text response.
@@ -1148,15 +1113,15 @@
 
                 response = make_response(jsonify(message), 200)
                 return response
 
             except RequestException as ex:
                 msg = f"RequestException occurred: {str(ex)}"
                 exc_info = sys.exc_info()
-                # logger_singleton.error_with_exception(msg, exc_info)
+                logger_singleton.error_with_exception(msg, exc_info)
                 # Create the return message with the start, end, and total time
                 message = {
                     'start_time': start_time,
                     'end_time': end_time,
                     'total_time': total_time,
                     'data': msg
                 }
```

### Comparing `data_ecosystem_flask-202307.0.35/data_ecosystem_flask/app_startup.py` & `data_ecosystem_flask-202307.0.4/data_ecosystem_flask/app_startup.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 
 # Constant indicating if the application is running inside Windows Subsystem for Linux (WSL)
 RUNNING_IN_WSL = False
 # Get the currently running file name
 NAMESPACE_NAME = os.path.basename(os.path.dirname(__file__))
 # Get the parent folder name of the running file
 SERVICE_NAME = os.path.basename(__file__)
- 
+
+
 def change_to_root_directory():
     # Get the absolute path of the current script
     current_script_path = os.path.abspath(__file__)
 
     # Get the project root directory by going up one or more levels
     project_root = os.path.dirname(os.path.dirname(current_script_path))
 
@@ -219,47 +220,33 @@
     """
     # Add your Flask app creation and configuration logic here
 
     # Get the path to the .env file
 
     CURRENT_USER_NAME = os.getenv('USERNAME') or os.getenv('USER')
     API_PATH = "/data-ecosystem-services/data_ecosystem_services"
-    instrumentation_key = "d091b27b-14e0-437f-ae3c-90f3f04ef3dc"
-
-
     dotenv_path = os.path.join(os.path.dirname(__file__), '.env')
+
     # Load the .env file
     load_dotenv(dotenv_path)
-
-    # set_key(dotenv_path, "PYARROW_IGNORE_TIMEZONE",
-    #        "1")
-    # set_key(dotenv_path, "APPLICATIONINSIGHTS_CONNECTION_STRING",
-    #        f"InstrumentationKey={instrumentation_key};IngestionEndpoint=https://eastus-8.in.applicationinsights.azure.com/;LiveEndpoint=https://eastus.livediagnostics.monitor.azure.com/")
-    # set_key(dotenv_path, "APPINSIGHTS_INSTRUMENTATIONKEY",
-    #        instrumentation_key)
+    instrumentation_key = "d091b27b-14e0-437f-ae3c-90f3f04ef3dc"
+    set_key(dotenv_path, "PYARROW_IGNORE_TIMEZONE",
+            "1")
+    set_key(dotenv_path, "APPLICATIONINSIGHTS_CONNECTION_STRING",
+            f"InstrumentationKey={instrumentation_key};IngestionEndpoint=https://eastus-8.in.applicationinsights.azure.com/;LiveEndpoint=https://eastus.livediagnostics.monitor.azure.com/")
+    set_key(dotenv_path, "APPINSIGHTS_INSTRUMENTATIONKEY",
+            instrumentation_key)
     # Reload the updated .env file
-    # load_dotenv(dotenv_path)
+    load_dotenv(dotenv_path)
 
-    
-    try:
-        logger_singleton = pade_env_logging.LoggerSingleton.instance(calling_namespace_name=NAMESPACE_NAME, calling_service_name=SERVICE_NAME)
-    except TypeError as e:
-        # If a TypeError occurs, retry the call with no parameters
-        logger_singleton = pade_env_logging.LoggerSingleton.instance()
-        
+    logger_singleton = pade_env_logging.LoggerSingleton.instance(
+        NAMESPACE_NAME, SERVICE_NAME)
     logger = logger_singleton.get_logger()
-
-
-    try:
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance(calling_namespace_name=NAMESPACE_NAME, calling_service_name=SERVICE_NAME)
-    except TypeError as e:
-        # If a TypeError occurs, retry the call with no parameters
-        tracer_singleton = pade_env_tracing.TracerSingleton.instance()
-    
-    
+    tracer_singleton = pade_env_tracing.TracerSingleton.instance(
+        NAMESPACE_NAME, SERVICE_NAME)
     tracer = tracer_singleton.get_tracer()
     app = None
 
     try:
         with tracer.start_as_current_span("create_app"):
 
             # Get the absolute path of the directory of the current script
@@ -302,35 +289,35 @@
 
             app.env = 'development'
             app.debug = True  # Enable debug mode
 
             app.cdc_config = config
             env_file_path = config.get("env_file_path")
 
-            # shutil.copy(env_file_path, app.root_path)
+            shutil.copy(env_file_path, app.root_path)
             load_dotenv(env_file_path)
 
             az_kv_az_sub_client_secret_key = config.get(
                 "az_kv_az_sub_client_secret_key")
             az_kv_az_sub_client_secret_key = az_kv_az_sub_client_secret_key.replace(
                 "-", "_")
             client_secret = os.getenv(az_kv_az_sub_client_secret_key)
             logger.info(
                 f"az_kv_az_sub_client_secret_key:{az_kv_az_sub_client_secret_key}")
             logger.info(f"client_secret length:{len(client_secret)}")
 
             # Set the new value
-            # set_key(dotenv_path, "FLASK_DEBUG", "1")
-            # set_key(dotenv_path, "PYARROW_IGNORE_TIMEZONE", "1")
+            set_key(dotenv_path, "FLASK_DEBUG", "1")
+            set_key(dotenv_path, "PYARROW_IGNORE_TIMEZONE", "1")
             tenant_id = config.get("tenant_id")
             client_id = config.get("client_id")
             az_kv_key_vault_name = config.get("az_kv_key_vault_name")
 
             # Reload the updated .env file
-            # load_dotenv(dotenv_path)
+            load_dotenv(dotenv_path)
 
             # Trim leading and trailing whitespace from client_secret
             if client_secret is None:
                 logger.warning(f"client_secret is None")
             else:
                 client_secret = client_secret.strip()
```

### Comparing `data_ecosystem_flask-202307.0.35/data_ecosystem_flask/install.py` & `data_ecosystem_flask-202307.0.4/data_ecosystem_flask/install.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.35/data_ecosystem_flask/requirements.txt` & `data_ecosystem_flask-202307.0.4/data_ecosystem_flask/requirements.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,146 +1,228 @@
+adal==1.2.7 ; python_version >= "3.9" and python_version < "4.0"
+alabaster==0.7.13 ; python_version >= "3.9" and python_version < "4.0"
 alation==0.1.14 ; python_version >= "3.9" and python_version < "4.0"
 aniso8601==9.0.1 ; python_version >= "3.9" and python_version < "4.0"
-anyio==3.7.1 ; python_version >= "3.9" and python_version < "4.0"
+anyascii==0.3.2 ; python_version >= "3.9" and python_version < "4.0"
+anyio==3.7.0 ; python_version >= "3.9" and python_version < "4.0"
 appdirs==1.4.4 ; python_version >= "3.9" and python_version < "4.0"
-appnope==0.1.3 ; python_version >= "3.9" and python_version < "4.0" and sys_platform == "darwin" or python_version >= "3.9" and python_version < "4.0" and platform_system == "Darwin"
+appnope==0.1.3 ; python_version >= "3.9" and python_version < "4.0" and (sys_platform == "darwin" or platform_system == "Darwin")
 argon2-cffi-bindings==21.2.0 ; python_version >= "3.9" and python_version < "4.0"
 argon2-cffi==21.3.0 ; python_version >= "3.9" and python_version < "4.0"
 arrow==1.2.3 ; python_version >= "3.9" and python_version < "4.0"
+astroid==2.15.5 ; python_version >= "3.9" and python_version < "4.0"
 asttokens==2.2.1 ; python_version >= "3.9" and python_version < "4.0"
 attrs==23.1.0 ; python_version >= "3.9" and python_version < "4.0"
-azure-core==1.28.0 ; python_version >= "3.9" and python_version < "4.0"
+azure-common==1.1.28 ; python_version >= "3.9" and python_version < "4.0"
+azure-core==1.27.1 ; python_version >= "3.9" and python_version < "4.0"
+azure-identity==1.13.0 ; python_version >= "3.9" and python_version < "4.0"
+azure-keyvault-certificates==4.7.0 ; python_version >= "3.9" and python_version < "4.0"
+azure-keyvault-keys==4.8.0 ; python_version >= "3.9" and python_version < "4.0"
+azure-keyvault-secrets==4.7.0 ; python_version >= "3.9" and python_version < "4.0"
+azure-keyvault==4.2.0 ; python_version >= "3.9" and python_version < "4.0"
+azure-mgmt-core==1.4.0 ; python_version >= "3.9" and python_version < "4.0"
+azure-mgmt-monitor==5.0.1 ; python_version >= "3.9" and python_version < "4.0"
+azure-mgmt-resource==23.0.1 ; python_version >= "3.9" and python_version < "4.0"
 azure-monitor-opentelemetry-exporter==1.0.0b14 ; python_version >= "3.9" and python_version < "4.0"
+azure-storage-blob==12.16.0 ; python_version >= "3.9" and python_version < "4.0"
+azure-storage-file-datalake==12.11.0 ; python_version >= "3.9" and python_version < "4.0"
+azure-storage-queue==12.6.0 ; python_version >= "3.9" and python_version < "4.0"
+babel==2.12.1 ; python_version >= "3.9" and python_version < "4.0"
 backcall==0.2.0 ; python_version >= "3.9" and python_version < "4.0"
 beautifulsoup4==4.12.2 ; python_version >= "3.9" and python_version < "4.0"
 bleach==6.0.0 ; python_version >= "3.9" and python_version < "4.0"
 blinker==1.6.2 ; python_version >= "3.9" and python_version < "4.0"
+boto3==1.21.18 ; python_version >= "3.9" and python_version < "4.0"
+botocore==1.24.18 ; python_version >= "3.9" and python_version < "4.0"
+cachetools==5.3.1 ; python_version >= "3.9" and python_version < "4.0"
 certifi==2023.5.7 ; python_version >= "3.9" and python_version < "4.0"
 cffi==1.15.1 ; python_version >= "3.9" and python_version < "4.0"
-charset-normalizer==3.2.0 ; python_version >= "3.9" and python_version < "4.0"
-click==8.1.6 ; python_version >= "3.9" and python_version < "4.0"
-colorama==0.4.6 ; python_version >= "3.9" and python_version < "4.0" and platform_system == "Windows" or python_version >= "3.9" and python_version < "4.0" and sys_platform == "win32"
+chardet==5.1.0 ; python_version >= "3.9" and python_version < "4.0"
+charset-normalizer==3.1.0 ; python_version >= "3.9" and python_version < "4.0"
+click==8.1.3 ; python_version >= "3.9" and python_version < "4.0"
+colorama==0.4.6 ; python_version >= "3.9" and python_version < "4.0" and (platform_system == "Windows" or sys_platform == "win32")
 comm==0.1.3 ; python_version >= "3.9" and python_version < "4.0"
+cryptography==41.0.1 ; python_version >= "3.9" and python_version < "4.0"
+data-ecosystem-services==202306.0.41 ; python_version >= "3.9" and python_version < "4.0"
+ddlparse==1.10.0 ; python_version >= "3.9" and python_version < "4.0"
 debugpy==1.6.7 ; python_version >= "3.9" and python_version < "4.0"
 decorator==5.1.1 ; python_version >= "3.9" and python_version < "4.0"
 defusedxml==0.7.1 ; python_version >= "3.9" and python_version < "4.0"
 deprecated==1.2.14 ; python_version >= "3.9" and python_version < "4.0"
+docutils==0.17.1 ; python_version >= "3.9" and python_version < "4.0"
 entrypoints==0.4 ; python_version >= "3.9" and python_version < "4.0"
 et-xmlfile==1.1.0 ; python_version >= "3.9" and python_version < "4.0"
-exceptiongroup==1.1.2 ; python_version >= "3.9" and python_version < "3.11"
+exceptiongroup==1.1.1 ; python_version >= "3.9" and python_version < "3.11"
 executing==1.2.0 ; python_version >= "3.9" and python_version < "4.0"
-fastjsonschema==2.18.0 ; python_version >= "3.9" and python_version < "4.0"
+fastjsonschema==2.17.1 ; python_version >= "3.9" and python_version < "4.0"
 fixedint==0.1.6 ; python_version >= "3.9" and python_version < "4.0"
 flake8==4.0.1 ; python_version >= "3.9" and python_version < "4.0"
 flask-restful==0.3.10 ; python_version >= "3.9" and python_version < "4.0"
 flask-restx==1.1.0 ; python_version >= "3.9" and python_version < "4.0"
 flask==2.3.2 ; python_version >= "3.9" and python_version < "4.0"
 fqdn==1.5.1 ; python_version >= "3.9" and python_version < "4"
 fsspec==2023.6.0 ; python_version >= "3.9" and python_version < "4.0"
+google-api-core==2.11.1 ; python_version >= "3.9" and python_version < "4.0"
+google-auth==2.21.0 ; python_version >= "3.9" and python_version < "4.0"
+googleapis-common-protos==1.59.1 ; python_version >= "3.9" and python_version < "4.0"
+html2text==2020.1.16 ; python_version >= "3.9" and python_version < "4.0"
 humanize==4.7.0 ; python_version >= "3.9" and python_version < "4.0"
 idna==3.4 ; python_version >= "3.9" and python_version < "4.0"
+imagesize==1.4.1 ; python_version >= "3.9" and python_version < "4.0"
 importlib-metadata==6.0.1 ; python_version >= "3.9" and python_version < "4.0"
-importlib-resources==6.0.0 ; python_version >= "3.9" and python_version < "4.0"
-ipykernel==6.25.0 ; python_version >= "3.9" and python_version < "4.0"
+importlib-resources==5.12.0 ; python_version >= "3.9" and python_version < "4.0"
+iniconfig==2.0.0 ; python_version >= "3.9" and python_version < "4.0"
+ipykernel==6.23.3 ; python_version >= "3.9" and python_version < "4.0"
 ipython-genutils==0.2.0 ; python_version >= "3.9" and python_version < "4.0"
 ipython==8.14.0 ; python_version >= "3.9" and python_version < "4.0"
 isodate==0.6.1 ; python_version >= "3.9" and python_version < "4.0"
 isoduration==20.11.0 ; python_version >= "3.9" and python_version < "4.0"
 itsdangerous==2.1.2 ; python_version >= "3.9" and python_version < "4.0"
-jedi==0.19.0 ; python_version >= "3.9" and python_version < "4.0"
+jedi==0.18.2 ; python_version >= "3.9" and python_version < "4.0"
 jinja2==3.1.2 ; python_version >= "3.9" and python_version < "4.0"
+jmespath==0.10.0 ; python_version >= "3.9" and python_version < "4.0"
 joblib==1.3.1 ; python_version >= "3.9" and python_version < "4.0"
 jsonpointer==2.4 ; python_version >= "3.9" and python_version < "4.0"
-jsonschema-specifications==2023.7.1 ; python_version >= "3.9" and python_version < "4.0"
-jsonschema==4.18.4 ; python_version >= "3.9" and python_version < "4.0"
-jsonschema[format-nongpl]==4.18.4 ; python_version >= "3.9" and python_version < "4.0"
-jupyter-client==7.4.9 ; python_version >= "3.9" and python_version < "4.0"
+jsonschema==4.17.3 ; python_version >= "3.9" and python_version < "4.0"
+jsonschema[format-nongpl]==4.17.3 ; python_version >= "3.9" and python_version < "4.0"
+jupyter-client==8.3.0 ; python_version >= "3.9" and python_version < "4.0"
 jupyter-core==5.3.1 ; python_version >= "3.9" and python_version < "4.0"
 jupyter-events==0.6.3 ; python_version >= "3.9" and python_version < "4.0"
 jupyter-server-terminals==0.4.4 ; python_version >= "3.9" and python_version < "4.0"
 jupyter-server==2.7.0 ; python_version >= "3.9" and python_version < "4.0"
 jupyterlab-pygments==0.2.2 ; python_version >= "3.9" and python_version < "4.0"
-lxml==4.9.3 ; python_version >= "3.9" and python_version < "4.0"
+lazy-object-proxy==1.9.0 ; python_version >= "3.9" and python_version < "4.0"
+lxml==4.9.2 ; python_version >= "3.9" and python_version < "4.0"
+markdown-it-py==2.2.0 ; python_version >= "3.9" and python_version < "4.0"
+markdown==3.4.3 ; python_version >= "3.9" and python_version < "4.0"
 markupsafe==2.1.3 ; python_version >= "3.9" and python_version < "4.0"
 matplotlib-inline==0.1.6 ; python_version >= "3.9" and python_version < "4.0"
 mccabe==0.6.1 ; python_version >= "3.9" and python_version < "4.0"
+mdit-py-plugins==0.3.5 ; python_version >= "3.9" and python_version < "4.0"
+mdurl==0.1.2 ; python_version >= "3.9" and python_version < "4.0"
 mistune==0.8.4 ; python_version >= "3.9" and python_version < "4.0"
+msal-extensions==1.0.0 ; python_version >= "3.9" and python_version < "4.0"
+msal==1.22.0 ; python_version >= "3.9" and python_version < "4.0"
 msrest==0.7.1 ; python_version >= "3.9" and python_version < "4.0"
+myst-parser==0.18.1 ; python_version >= "3.9" and python_version < "4.0"
 nbclassic==1.0.0 ; python_version >= "3.9" and python_version < "4.0"
 nbclient==0.8.0 ; python_version >= "3.9" and python_version < "4.0"
 nbconvert==6.5.4 ; python_version >= "3.9" and python_version < "4.0"
-nbformat==5.9.1 ; python_version >= "3.9" and python_version < "4.0"
-nest-asyncio==1.5.7 ; python_version >= "3.9" and python_version < "4.0"
+nbformat==5.9.0 ; python_version >= "3.9" and python_version < "4.0"
+nest-asyncio==1.5.6 ; python_version >= "3.9" and python_version < "4.0"
 notebook-shim==0.2.3 ; python_version >= "3.9" and python_version < "4.0"
-notebook==6.5.5 ; python_version >= "3.9" and python_version < "4.0"
-numpy==1.25.1 ; python_version >= "3.9" and python_version < "4.0"
+notebook==6.5.4 ; python_version >= "3.9" and python_version < "4.0"
+numpy==1.25.0 ; python_version >= "3.9" and python_version < "4.0"
 oauthlib==3.2.2 ; python_version >= "3.9" and python_version < "4.0"
+opencensus-context==0.1.3 ; python_version >= "3.9" and python_version < "4.0"
+opencensus-ext-azure==1.1.9 ; python_version >= "3.9" and python_version < "4.0"
+opencensus==0.11.2 ; python_version >= "3.9" and python_version < "4.0"
 openpyxl==3.1.2 ; python_version >= "3.9" and python_version < "4.0"
 opentelemetry-api==1.18.0 ; python_version >= "3.9" and python_version < "4.0"
 opentelemetry-instrumentation-flask==0.39b0 ; python_version >= "3.9" and python_version < "4.0"
 opentelemetry-instrumentation-wsgi==0.39b0 ; python_version >= "3.9" and python_version < "4.0"
 opentelemetry-instrumentation==0.39b0 ; python_version >= "3.9" and python_version < "4.0"
 opentelemetry-sdk==1.18.0 ; python_version >= "3.9" and python_version < "4.0"
 opentelemetry-semantic-conventions==0.39b0 ; python_version >= "3.9" and python_version < "4.0"
 opentelemetry-util-http==0.39b0 ; python_version >= "3.9" and python_version < "4.0"
 overrides==7.3.1 ; python_version >= "3.9" and python_version < "4.0"
 packaging==23.1 ; python_version >= "3.9" and python_version < "4.0"
 pandas==2.0.3 ; python_version >= "3.9" and python_version < "4.0"
 pandocfilters==1.5.0 ; python_version >= "3.9" and python_version < "4.0"
 parso==0.8.3 ; python_version >= "3.9" and python_version < "4.0"
+pathlib==1.0.1 ; python_version >= "3.9" and python_version < "4.0"
+pbr==5.11.1 ; python_version >= "3.9" and python_version < "4.0"
 pexpect==4.8.0 ; python_version >= "3.9" and python_version < "4.0" and sys_platform != "win32"
 pickleshare==0.7.5 ; python_version >= "3.9" and python_version < "4.0"
 pins==0.8.1 ; python_version >= "3.9" and python_version < "4.0"
-pip==23.2.1 ; python_version >= "3.9" and python_version < "4.0"
-platformdirs==3.10.0 ; python_version >= "3.9" and python_version < "4.0"
-prometheus-client==0.17.1 ; python_version >= "3.9" and python_version < "4.0"
-prompt-toolkit==3.0.39 ; python_version >= "3.9" and python_version < "4.0"
+pip-system-certs==4.0 ; python_version >= "3.9" and python_version < "4.0"
+pip==23.1.2 ; python_version >= "3.9" and python_version < "4.0"
+platformdirs==3.8.0 ; python_version >= "3.9" and python_version < "4.0"
+pluggy==1.2.0 ; python_version >= "3.9" and python_version < "4.0"
+portalocker==2.7.0 ; python_version >= "3.9" and python_version < "4.0"
+prometheus-client==0.17.0 ; python_version >= "3.9" and python_version < "4.0"
+prompt-toolkit==3.0.38 ; python_version >= "3.9" and python_version < "4.0"
+protobuf==4.23.3 ; python_version >= "3.9" and python_version < "4.0"
 psutil==5.9.5 ; python_version >= "3.9" and python_version < "4.0"
-ptyprocess==0.7.0 ; python_version >= "3.9" and python_version < "4.0" and sys_platform != "win32" or python_version >= "3.9" and python_version < "4.0" and os_name != "nt"
+ptyprocess==0.7.0 ; python_version >= "3.9" and python_version < "4.0" and (sys_platform != "win32" or os_name != "nt")
 pure-eval==0.2.2 ; python_version >= "3.9" and python_version < "4.0"
-py==1.11.0 ; python_version >= "3.9" and python_version < "4.0" and implementation_name == "pypy"
+pyarrow==10.0.1 ; python_version >= "3.9" and python_version < "4.0"
+pyasn1-modules==0.3.0 ; python_version >= "3.9" and python_version < "4.0"
+pyasn1==0.5.0 ; python_version >= "3.9" and python_version < "4.0"
 pycodestyle==2.8.0 ; python_version >= "3.9" and python_version < "4.0"
 pycparser==2.21 ; python_version >= "3.9" and python_version < "4.0"
+pydash==7.0.4 ; python_version >= "3.9" and python_version < "4.0"
 pyflakes==2.4.0 ; python_version >= "3.9" and python_version < "4.0"
 pygments==2.15.1 ; python_version >= "3.9" and python_version < "4.0"
-pyjwt==2.8.0 ; python_version >= "3.9" and python_version < "4.0"
+pyjwt==2.7.0 ; python_version >= "3.9" and python_version < "4.0"
+pyjwt[crypto]==2.7.0 ; python_version >= "3.9" and python_version < "4.0"
+pyparsing==3.1.0 ; python_version >= "3.9" and python_version < "4.0"
+pyreadstat==1.2.2 ; python_version >= "3.9" and python_version < "4.0"
+pyrsistent==0.19.3 ; python_version >= "3.9" and python_version < "4.0"
+pytest==7.4.0 ; python_version >= "3.9" and python_version < "4.0"
 python-dateutil==2.8.2 ; python_version >= "3.9" and python_version < "4.0"
 python-dotenv==1.0.0 ; python_version >= "3.9" and python_version < "4.0"
 python-json-logger==2.0.7 ; python_version >= "3.9" and python_version < "4.0"
 pytz==2023.3 ; python_version >= "3.9" and python_version < "4.0"
-pywin32==306 ; sys_platform == "win32" and platform_python_implementation != "PyPy" and python_version >= "3.9" and python_version < "4.0"
-pywinpty==2.0.11 ; python_version >= "3.9" and python_version < "4.0" and os_name == "nt"
-pyyaml==6.0.1 ; python_version >= "3.9" and python_version < "4.0"
-pyzmq==24.0.1 ; python_version >= "3.9" and python_version < "4.0"
-referencing==0.30.0 ; python_version >= "3.9" and python_version < "4.0"
+pywin32==306 ; python_version >= "3.9" and (sys_platform == "win32" or platform_system == "Windows") and python_version < "4.0" and (platform_python_implementation != "PyPy" or platform_system == "Windows")
+pywinpty==2.0.10 ; python_version >= "3.9" and python_version < "4.0" and os_name == "nt"
+pyyaml==6.0 ; python_version >= "3.9" and python_version < "4.0"
+pyzmq==25.1.0 ; python_version >= "3.9" and python_version < "4.0"
 requests-oauthlib==1.3.1 ; python_version >= "3.9" and python_version < "4.0"
 requests==2.31.0 ; python_version >= "3.9" and python_version < "4.0"
 rfc3339-validator==0.1.4 ; python_version >= "3.9" and python_version < "4.0"
 rfc3986-validator==0.1.1 ; python_version >= "3.9" and python_version < "4.0"
-rpds-py==0.9.2 ; python_version >= "3.9" and python_version < "4.0"
+rich==13.4.2 ; python_version >= "3.9" and python_version < "4.0"
+rsa==4.9 ; python_version >= "3.9" and python_version < "4"
 rsconnect-jupyter==1.8.0 ; python_version >= "3.9" and python_version < "4.0"
-rsconnect-python==1.19.0 ; python_version >= "3.9" and python_version < "4.0"
+rsconnect-python==1.18.0 ; python_version >= "3.9" and python_version < "4.0"
 rsconnect==0.1.3 ; python_version >= "3.9" and python_version < "4.0"
+s3transfer==0.5.2 ; python_version >= "3.9" and python_version < "4.0"
 semver==2.13.0 ; python_version >= "3.9" and python_version < "4.0"
 send2trash==1.8.2 ; python_version >= "3.9" and python_version < "4.0"
 setuptools==65.6.3 ; python_version >= "3.9" and python_version < "4.0"
 six==1.16.0 ; python_version >= "3.9" and python_version < "4.0"
 sniffio==1.3.0 ; python_version >= "3.9" and python_version < "4.0"
+snowballstemmer==2.2.0 ; python_version >= "3.9" and python_version < "4.0"
 soupsieve==2.4.1 ; python_version >= "3.9" and python_version < "4.0"
+sphinx-autoapi==2.1.1 ; python_version >= "3.9" and python_version < "4.0"
+sphinx-autodoc-typehints==1.23.0 ; python_version >= "3.9" and python_version < "4.0"
+sphinx-markdown-builder==0.5.5 ; python_version >= "3.9" and python_version < "4.0"
+sphinx-markdown-tables==0.0.17 ; python_version >= "3.9" and python_version < "4.0"
+sphinx-rtd-theme==1.2.2 ; python_version >= "3.9" and python_version < "4.0"
+sphinx-sitemap==2.5.0 ; python_version >= "3.9" and python_version < "4.0"
+sphinx-sql==1.3.4 ; python_version >= "3.9" and python_version < "4.0"
+sphinx==5.3.0 ; python_version >= "3.9" and python_version < "4.0"
+sphinxcontrib-applehelp==1.0.4 ; python_version >= "3.9" and python_version < "4.0"
+sphinxcontrib-devhelp==1.0.2 ; python_version >= "3.9" and python_version < "4.0"
+sphinxcontrib-htmlhelp==2.0.1 ; python_version >= "3.9" and python_version < "4.0"
+sphinxcontrib-jquery==4.1 ; python_version >= "3.9" and python_version < "4.0"
+sphinxcontrib-jsmath==1.0.1 ; python_version >= "3.9" and python_version < "4.0"
+sphinxcontrib-mermaid==0.7.1 ; python_version >= "3.9" and python_version < "4.0"
+sphinxcontrib-qthelp==1.0.3 ; python_version >= "3.9" and python_version < "4.0"
+sphinxcontrib-serializinghtml==1.1.5 ; python_version >= "3.9" and python_version < "4.0"
 stack-data==0.6.2 ; python_version >= "3.9" and python_version < "4.0"
+style==1.1.6 ; python_version >= "3.9" and python_version < "4.0"
 terminado==0.17.1 ; python_version >= "3.9" and python_version < "4.0"
+testresources==2.0.1 ; python_version >= "3.9" and python_version < "4.0"
 tinycss2==1.2.1 ; python_version >= "3.9" and python_version < "4.0"
+toml==0.10.2 ; python_version >= "3.9" and python_version < "4.0"
+tomli==2.0.1 ; python_version >= "3.9" and python_version < "4.0"
 tornado==6.3.2 ; python_version >= "3.9" and python_version < "4.0"
 traitlets==5.9.0 ; python_version >= "3.9" and python_version < "4.0"
-typing-extensions==4.7.1 ; python_version >= "3.9" and python_version < "4.0"
+tryceratops==2.3.2 ; python_version >= "3.9" and python_version < "4.0"
+typing-extensions==4.7.0 ; python_version >= "3.9" and python_version < "4.0"
 tzdata==2023.3 ; python_version >= "3.9" and python_version < "4.0"
+unify==0.5 ; python_version >= "3.9" and python_version < "4.0"
+untokenize==0.1.1 ; python_version >= "3.9" and python_version < "4.0"
 uri-template==1.3.0 ; python_version >= "3.9" and python_version < "4.0"
 urllib3==1.26.16 ; python_version >= "3.9" and python_version < "4.0"
 wcwidth==0.2.6 ; python_version >= "3.9" and python_version < "4.0"
 webcolors==1.13 ; python_version >= "3.9" and python_version < "4.0"
 webencodings==0.5.1 ; python_version >= "3.9" and python_version < "4.0"
 websocket-client==1.6.1 ; python_version >= "3.9" and python_version < "4.0"
 werkzeug==2.3.6 ; python_version >= "3.9" and python_version < "4.0"
 wrapt==1.15.0 ; python_version >= "3.9" and python_version < "4.0"
 xlsxwriter==3.1.2 ; python_version >= "3.9" and python_version < "4.0"
-xxhash==3.3.0 ; python_version >= "3.9" and python_version < "4.0"
-zipp==3.16.2 ; python_version >= "3.9" and python_version < "4.0"
+xxhash==3.2.0 ; python_version >= "3.9" and python_version < "4.0"
+yapf==0.33.0 ; python_version >= "3.9" and python_version < "4.0"
+zipp==3.15.0 ; python_version >= "3.9" and python_version < "4.0"
```

### Comparing `data_ecosystem_flask-202307.0.35/data_ecosystem_flask/templates/log_file.html` & `data_ecosystem_flask-202307.0.4/data_ecosystem_flask/templates/log_file.html`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.35/data_ecosystem_flask/templates/upload.html` & `data_ecosystem_flask-202307.0.4/data_ecosystem_flask/templates/upload.html`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.35/license.md` & `data_ecosystem_flask-202307.0.4/license.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# License
-
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
    1. Definitions.
```

### Comparing `data_ecosystem_flask-202307.0.35/pyproject.toml` & `data_ecosystem_flask-202307.0.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "data_ecosystem_flask"
 authors = [{name="John Bowyer", email="zfi4@cdc.gov" }]
 description = "Data Ecosystem Flask (PADE)  - Python "
 readme = "readme.md"
 requires-python = ">=3.9,<4.0"
-version = "202307.0.35"
+version = "202307.0.1"
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.9"
 ]
 
@@ -16,15 +16,15 @@
 [project.urls]
 "Homepage" = "https://test.pypi.org/project/data-ecosystem-services"
 "Documentation" = "https://gift.readthedocs.io"
 "Repository" = "https://github.com/cdcent/data-ecosystem-services"
 
 [tool.poetry]
 name = "data_ecosystem_flask"
-version="202307.0.35"
+version="202307.0.4"
 description = "Program Agnostic Data Ecosystem (PADE) - Flask Web Service"
 authors = ["John Bowyer <zfi4@cdc.gov>"]
 license = "Apache"
 homepage="https://test.pypi.org/project/data-ecosystem-services"
 repository="https://github.com/cdcent/data-ecosystem-services"
 classifiers=[
     "Development Status :: 4 - Beta",
@@ -36,29 +36,20 @@
 ]
 include = [ "readme.md",
             "license.md",
             "setup.cfg",
             "setup.py",
             "pyproject.toml",
             "data_ecosystem_flask/data_ecosystem_flask/**/*.py",
-            "data_ecosystem_flask/**/*.py",
-            "ocio/**/*.json",            
-            "dev_schema/**/*.xlsx",     
-            "dev_schema/**/*.json",
-            "ocio/ocio_pade_dev/config/config.dev.json",
-            "data_ecosystem_flask/config/*.json",
-            "data_ecosystem_flask/*.xlsx",
-            "data_ecosystem_flask/.env"
-        ]
+            "data_ecosystem_flask/**/*.py"]
+
 
 [tool.poetry.dependencies]
 python = "^3.9"
 flask = "^2.0.0"
-numpy = "^1.23.0"
-wrapt = "^1.14.0"
 six = "^1.16.0"
 openpyxl = "^3.1.2"
 oauthlib = "^3.2.2"
 xlsxwriter = "^3.1.0"
 werkzeug = "^2.3.3"
 flask-restx = "^1.1.0"
 flake8 = "^4.0.1"
@@ -69,20 +60,20 @@
 alation = "^0.1.14"
 opentelemetry-sdk = "^1.17.0"
 azure-monitor-opentelemetry-exporter = {version = "^1.0.0b14", allow-prereleases = true}
 opentelemetry-instrumentation-flask = "^0.39b0"
 python-dotenv = "^1.0.0"
 rsconnect = "^0.1.3"
 flask-restful = "^0.3.10"
-data-ecosystem-services = "^202307.0.32"
-
+data-ecosystem-services = "^202306.0.26"
+certifi = "2023.5.7"
+ 
 
 [tool.poetry.dev-dependencies]
 
- 
 [tool.poetry.scripts]
 flaskapp = "data_ecosystem_flask.app:app"
 
 
 [tool.pytest.ini_options]
 minversion="6.0"
 addopts="-ra -q --cov --cov-report html --cov-report term-missing --cov-fail-under 15"
```

### Comparing `data_ecosystem_flask-202307.0.35/readme.md` & `data_ecosystem_flask-202307.0.4/readme.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_flask-202307.0.35/PKG-INFO` & `data_ecosystem_flask-202307.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-ecosystem-flask
-Version: 202307.0.35
+Version: 202307.0.4
 Summary: Program Agnostic Data Ecosystem (PADE) - Flask Web Service
 Home-page: https://test.pypi.org/project/data-ecosystem-services
 License: Apache
 Author: John Bowyer
 Author-email: zfi4@cdc.gov
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -13,31 +13,29 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: alation (>=0.1.14,<0.2.0)
 Requires-Dist: azure-monitor-opentelemetry-exporter (>=1.0.0b14,<2.0.0)
-Requires-Dist: data-ecosystem-services (>=202307.0.32,<202308.0.0)
+Requires-Dist: certifi (==2023.5.7)
+Requires-Dist: data-ecosystem-services (>=202306.0.26,<202307.0.0)
 Requires-Dist: flake8 (>=4.0.1,<5.0.0)
 Requires-Dist: flask (>=2.0.0,<3.0.0)
 Requires-Dist: flask-restful (>=0.3.10,<0.4.0)
 Requires-Dist: flask-restx (>=1.1.0,<2.0.0)
-Requires-Dist: numpy (>=1.23.0,<2.0.0)
 Requires-Dist: oauthlib (>=3.2.2,<4.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: opentelemetry-instrumentation-flask (>=0.39b0,<0.40)
 Requires-Dist: opentelemetry-sdk (>=1.17.0,<2.0.0)
 Requires-Dist: pycodestyle (>=2.8.0,<2.9.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rsconnect (>=0.1.3,<0.2.0)
 Requires-Dist: rsconnect-python (>=1.17.1,<2.0.0)
 Requires-Dist: setuptools (==65.6.3)
 Requires-Dist: six (>=1.16.0,<2.0.0)
 Requires-Dist: werkzeug (>=2.3.3,<3.0.0)
-Requires-Dist: wrapt (>=1.14.0,<2.0.0)
 Requires-Dist: xlsxwriter (>=3.1.0,<4.0.0)
 Project-URL: Repository, https://github.com/cdcent/data-ecosystem-services
```

