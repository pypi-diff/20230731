# Comparing `tmp/pbipy-2.4.5.tar.gz` & `tmp/pbipy-2.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbipy-2.4.5.tar", last modified: Sat Jul  8 17:45:28 2023, max compression
+gzip compressed data, was "pbipy-2.5.6.tar", last modified: Mon Jul 31 09:38:20 2023, max compression
```

## Comparing `pbipy-2.4.5.tar` & `pbipy-2.5.6.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 17:45:28.953789 pbipy-2.4.5/
--rw-rw-rw-   0        0        0    11523 2022-10-28 08:16:15.000000 pbipy-2.4.5/LICENSE
--rw-rw-rw-   0        0        0    11056 2023-07-08 17:45:28.953789 pbipy-2.4.5/PKG-INFO
--rw-rw-rw-   0        0        0    10272 2023-07-08 17:41:53.000000 pbipy-2.4.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 17:45:28.945788 pbipy-2.4.5/pbipy/
--rw-rw-rw-   0        0        0       29 2022-10-28 07:52:32.000000 pbipy-2.4.5/pbipy/__init__.py
--rw-rw-rw-   0        0        0      335 2023-07-08 17:44:27.000000 pbipy-2.4.5/pbipy/__version__.py
--rw-rw-rw-   0        0        0     4932 2023-07-03 17:56:42.000000 pbipy-2.4.5/pbipy/apps.py
--rw-rw-rw-   0        0        0     1630 2023-07-03 09:18:23.000000 pbipy-2.4.5/pbipy/dashboards.py
--rw-rw-rw-   0        0        0     5782 2023-07-08 17:35:27.000000 pbipy-2.4.5/pbipy/dataflows.py
--rw-rw-rw-   0        0        0    19984 2023-07-08 17:28:25.000000 pbipy-2.4.5/pbipy/datasets.py
--rw-rw-rw-   0        0        0     5861 2023-06-20 20:12:45.000000 pbipy-2.4.5/pbipy/groups.py
--rw-rw-rw-   0        0        0    16707 2023-07-08 17:29:44.000000 pbipy-2.4.5/pbipy/powerbi.py
--rw-rw-rw-   0        0        0    12848 2023-06-30 01:50:56.000000 pbipy-2.4.5/pbipy/reports.py
--rw-rw-rw-   0        0        0     1367 2023-07-06 17:22:30.000000 pbipy-2.4.5/pbipy/resources.py
--rw-rw-rw-   0        0        0      110 2023-06-18 05:21:13.000000 pbipy-2.4.5/pbipy/settings.py
--rw-rw-rw-   0        0        0    11724 2023-07-08 01:16:07.000000 pbipy-2.4.5/pbipy/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:45:28.953789 pbipy-2.4.5/pbipy.egg-info/
--rw-rw-rw-   0        0        0    11056 2023-07-08 17:45:28.000000 pbipy-2.4.5/pbipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      382 2023-07-08 17:45:28.000000 pbipy-2.4.5/pbipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 17:45:28.000000 pbipy-2.4.5/pbipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-07-08 17:45:28.000000 pbipy-2.4.5/pbipy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-08 17:45:28.000000 pbipy-2.4.5/pbipy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 17:45:28.953789 pbipy-2.4.5/setup.cfg
--rw-rw-rw-   0        0        0     3594 2022-12-05 03:27:44.000000 pbipy-2.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:38:20.356694 pbipy-2.5.6/
+-rw-rw-rw-   0        0        0    11523 2022-10-28 08:16:15.000000 pbipy-2.5.6/LICENSE
+-rw-rw-rw-   0        0        0    13075 2023-07-31 09:38:20.354693 pbipy-2.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0    12291 2023-07-31 09:34:59.000000 pbipy-2.5.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 09:38:20.340691 pbipy-2.5.6/pbipy/
+-rw-rw-rw-   0        0        0       29 2022-10-28 07:52:32.000000 pbipy-2.5.6/pbipy/__init__.py
+-rw-rw-rw-   0        0        0      335 2023-07-31 09:35:34.000000 pbipy-2.5.6/pbipy/__version__.py
+-rw-rw-rw-   0        0        0    32566 2023-07-30 20:29:36.000000 pbipy-2.5.6/pbipy/admin.py
+-rw-rw-rw-   0        0        0     4932 2023-07-16 09:54:12.000000 pbipy-2.5.6/pbipy/apps.py
+-rw-rw-rw-   0        0        0     1630 2023-07-16 09:54:35.000000 pbipy-2.5.6/pbipy/dashboards.py
+-rw-rw-rw-   0        0        0     5782 2023-07-16 09:54:35.000000 pbipy-2.5.6/pbipy/dataflows.py
+-rw-rw-rw-   0        0        0    19984 2023-07-16 09:54:35.000000 pbipy-2.5.6/pbipy/datasets.py
+-rw-rw-rw-   0        0        0     5861 2023-07-16 09:54:35.000000 pbipy-2.5.6/pbipy/groups.py
+-rw-rw-rw-   0        0        0    17012 2023-07-10 19:43:47.000000 pbipy-2.5.6/pbipy/powerbi.py
+-rw-rw-rw-   0        0        0    12848 2023-07-16 09:54:35.000000 pbipy-2.5.6/pbipy/reports.py
+-rw-rw-rw-   0        0        0     1367 2023-07-16 17:37:42.000000 pbipy-2.5.6/pbipy/resources.py
+-rw-rw-rw-   0        0        0      110 2023-06-18 05:21:13.000000 pbipy-2.5.6/pbipy/settings.py
+-rw-rw-rw-   0        0        0    12712 2023-07-30 18:09:57.000000 pbipy-2.5.6/pbipy/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:38:20.352692 pbipy-2.5.6/pbipy.egg-info/
+-rw-rw-rw-   0        0        0    13075 2023-07-31 09:38:20.000000 pbipy-2.5.6/pbipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      397 2023-07-31 09:38:20.000000 pbipy-2.5.6/pbipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 09:38:20.000000 pbipy-2.5.6/pbipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-07-31 09:38:20.000000 pbipy-2.5.6/pbipy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-31 09:38:20.000000 pbipy-2.5.6/pbipy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 09:38:20.356694 pbipy-2.5.6/setup.cfg
+-rw-rw-rw-   0        0        0     3594 2023-07-30 18:10:32.000000 pbipy-2.5.6/setup.py
```

### Comparing `pbipy-2.4.5/LICENSE` & `pbipy-2.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pbipy-2.4.5/PKG-INFO` & `pbipy-2.5.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbipy
-Version: 2.4.5
+Version: 2.5.6
 Summary: A Python Library for interacting with the Power BI Rest API.
 Home-page: https://github.com/andrewvillazon/pbipy
 Author: Andrew Villazon
 Author-email: andrew.villazon@gmail.com
 License: Apache 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -43,37 +43,31 @@
 
 ## Getting Started: Authentication
 
 To use `pbipy` you'll first need to acquire a `bearer_token`.
 
 *How do I get a `bearer_token`?*
 
-To acquire a `bearer_token` you'll need to authenticate against your [Registered Azure Power BI App](https://learn.microsoft.com/en-us/power-bi/developer/embedded/register-app?tabs=customers). Registering is the first step in turning on the Power BI Rest API, so from this point on it's assumed your Power BI Rest API is up and running.
+To acquire a `bearer_token` you'll need to authenticate against your [Registered Azure Power BI App](https://learn.microsoft.com/en-us/power-bi/developer/embedded/register-app?tabs=customers). Registering is the first step in turning on the Power BI Rest API, so from here on it's assumed your Power BI Rest API is up and running.
 
-To authenticate against the Registered App, Microsoft provides the `MSAL` and `azure-identity` python libraries. These libraries support many different ways of acquiring a `bearer_token`.
+To authenticate against the Registered App, Microsoft provides the `MSAL` and `azure-identity` python libraries. These libraries support different ways of acquiring a `bearer_token` and which to use will depend on how your cloud/tenant is configured.
 
-Because there are multiple ways to acquire the token, `pbipy` assumes you'll do this in the way that suits, rather than directly handling authentication (of course, this might change in future).
+Because there are multiple ways to acquire the token, `pbipy` leaves it up to do this in the way that suits, rather than directly handling authentication (of course, this might change in future).
 
-This `README` doesn't cover Authentication in detail, however, these are some helpful resources that look at acquiring a `bearer_token` in the context of Power BI:
+This `README` doesn't cover authentication in detail, however, these are some helpful resources that look at acquiring a `bearer_token` in the context of Power BI:
 
 * [Power BI REST API with Python and MSAL. Part II.](https://www.datalineo.com/post/power-bi-rest-api-with-python-and-msal-part-ii)
 * [Power BI REST API with Python Part III, azure-identity](https://www.datalineo.com/post/power-bi-rest-api-with-python-part-iii-azure-identity)
 * [Monitoring Power BI using REST APIs from Python](https://data-goblins.com/power-bi/power-bi-api-python)
 
-The example below uses the `msal` library to to get a `bearer_token`.
-
-## Useage
-
-Start by creating the `PowerBI()` client. All interactions with the Power BI Rest API go through this object. 
+The example below uses the `msal` library to to get a bearer_token.
 
 ```python
 import msal
 
-from pbipy import PowerBI
-
 
 #  msal auth setup
 def acquire_bearer_token(username, password, azure_tenant_id, client_id, scopes):
     app = msal.PublicClientApplication(client_id, authority=azure_tenant_id)
     result = app.acquire_token_by_username_password(username, password, scopes)
     return result["access_token"]
 
@@ -81,16 +75,25 @@
 bearer_token = acquire_bearer_token(
     username="your-username",
     password="your-password",
     azure_tenant_id="https://login.microsoftonline.com/your-azure-tenant-id",
     client_id="your-pbi-client-id",
     scopes=["https://analysis.windows.net/powerbi/api/.default"],
 )
+```
+
+The code that follows assumes you've authenticated and acquired your `bearer_token`.
+
+## Useage
+
+Start by creating the `PowerBI()` client. Interactions with the Power BI Rest API go through this object. 
+
+```python
+from pbipy import PowerBI
 
-# Create Client
 pbi = PowerBI(bearer_token)
 ```
 
 To interact with the API, simply call the relevant method from the client.
 
 ```python
 # Grab the datasets from a workspace
@@ -109,23 +112,29 @@
 # <class 'pbipy.resources.Dataset'>
 # True
 ```
 
 Most methods take in an object id...
 
 ```python
-dataset = pbi.dataset("cfafbeb1-8037-4d0c-896e-a46fb27ff229", group="a2f89923-421a-464e-bf4c-25eab39bb09f")
+dataset = pbi.dataset(
+    id="cfafbeb1-8037-4d0c-896e-a46fb27ff229",
+    group="a2f89923-421a-464e-bf4c-25eab39bb09f"
+)
 ```
 
 ... or just pass in the object itself.
 
 ```python
 group = pbi.group("a2f89923-421a-464e-bf4c-25eab39bb09f")
 
-dataset = pbi.dataset("cfafbeb1-8037-4d0c-896e-a46fb27ff229", group=group)
+dataset = pbi.dataset(
+    "cfafbeb1-8037-4d0c-896e-a46fb27ff229"
+    ,group=group
+)
 ```
 
 If you need to access the raw json representation, this is supported to.
 
 ```python
 sales = pbi.dataset("cfafbeb1-8037-4d0c-896e-a46fb27ff229")
 
@@ -140,65 +149,65 @@
 # }
 ```
 
 ## Example: Working with Datasets
 
 Let's see how `pbipy` works by performing some operations on a Dataset.
 
-First, we need to load the Dataset from the API. To do this, we call the `dataset()` method from the `pbi` client we created above. 
-
-The Power BI Rest API will look for the Dataset in the current user's workspace if we don't provide a `group` argument.
+First, we initialize our client.
 
 ```python
-sales = pbi.dataset(id="cfafbeb1-8037-4d0c-896e-a46fb27ff229")
-print(sales)
+from pbipy import PowerBI
 
-# <Dataset id='cfafbeb1-8037-4d0c-896e-a46fb27ff229', name='SalesMarketing', ...>
+pbi = PowerBI(bearer_token)
 ```
 
-But we likely want to target a Dataset in a *Workspace*. To do this, we provide the Workspace Id as the `group` argument when we call the `dataset()` method.
+Now that we've got a client, we can load a Dataset from the API. To load a Dataset, we call the `dataset()` method with an `id` and `group` argument. In the Power BI Rest API, a **Group** and **Workspace** are synonymous and used interchangeably.
 
 ```python
 sales = pbi.dataset(
-    "cfafbeb1-8037-4d0c-896e-a46fb27ff229",
+    id="cfafbeb1-8037-4d0c-896e-a46fb27ff229",
     group="f089354e-8366-4e18-aea3-4cb4a3a50b48",
 )
+
+print(sales)
+
+# <Dataset id='cfafbeb1-8037-4d0c-896e-a46fb27ff229', name='SalesMarketing', ...>
 ```
 
-Now that we've got our target Dataset let's look at its Refresh History. We call the `refresh_history()` method on our Dataset. Easy.
+Dataset not updating? Let's look at the Refresh History. 
 
-```python
-dataset = pbi.dataset(
-    "cfafbeb1-8037-4d0c-896e-a46fb27ff229",
-    group="f089354e-8366-4e18-aea3-4cb4a3a50b48",
-)
+We call the `refresh_history()` method on our Dataset. Easy.
 
-refresh_history = dataset.refresh_history()
+```python
+refresh_history = sales.refresh_history()
 
 for entry in refresh_history:
     print(entry)
 
 # {"refreshType":"ViaApi", "startTime":"2017-06-13T09:25:43.153Z", "status": "Completed" ...}
 ```
 
-How about adding some user permissions to our Dataset? That's easy too. Just call the `add_user()` method with the User's details and permissions.
+Need to kick off a refresh? That's easy too.
 
 ```python
-sales_ds = pbi.dataset( "cfafbeb1-8037-4d0c-896e-a46fb27ff229")
+sales.refresh()
+```
+
+How about adding some user permissions to our Dataset? Just call the `add_user()` method with the User's details and permissions.
 
+```python
 # Give John 'Read' access on the dataset
-sales_ds.add_user("john@contoso.com", "User", "Read")
+sales.add_user("john@contoso.com", "User", "Read")
 ```
 
 Lastly, if we're feeling adventurous, we can execute DAX against a Dataset and use the results in Python.
 
 ```python
-dataset = pbi.dataset( "cfafbeb1-8037-4d0c-896e-a46fb27ff229")
-
-dxq_result = dataset.execute_queries("EVALUATE VALUES(MyTable)")
+dxq_result = sales.execute_queries("EVALUATE VALUES(MyTable)")
 print(dxq_result)
 
 # {
 #   "results": [
 #     {
 #       "tables": [
 #         {
@@ -207,14 +216,64 @@
 #               "MyTable[Year]": 2010,
 #               "MyTable[Quarter]": "Q1"
 #             },
 # ...
 # }
 ```
 
+## Example: Working with the Admin object
+
+`pbypi` also supports [Administrator Operations](https://learn.microsoft.com/en-us/rest/api/power-bi/admin), specialized operations available to users with Power BI Admin rights. Let's see how we can use these.
+
+First, we need to initialize our client. Then we call the `admin` method and initialize an `Admin` object.
+
+```python
+from pbipy import PowerBI
+
+pbi = PowerBI(bearer_token)
+admin = pbi.admin()
+```
+
+Need to review some access on some reports? We can call the `report_users` method.
+
+```python
+users = admin.report_users("5b218778-e7a5-4d73-8187-f10824047715")
+print(users[0])
+
+# {"displayName": "John Nick", "emailAddress": "john@contoso.com", ...}
+```
+
+What about understanding User activity on your Power BI tenant?
+
+```python
+from datetime import datetime
+
+start_dtm = datetime(2019, 8, 31, 0, 0, 0)
+end_dtm = datetime(2019, 8, 31, 23, 59, 59)
+
+activity_events = admin.activity_events(start_dtm, end_dtm)
+
+print(activity_events)
+
+# [
+#   {
+#       "Id": "41ce06d1", 
+#       "CreationTime": "2019-08-13T07:55:15", 
+#       "Operation": "ViewReport", 
+#       ...
+#   },
+#   {
+#       "Id": "c632aa64", 
+#       "CreationTime": "2019-08-13T07:55:10", 
+#       "Operation": "GetSnapshots", 
+#       ...
+#   }
+# ]
+```
+
 ## More examples
 
 ### Datasets in a Workspace
 
 ```python
 datasets = pbi.datasets(group="f089354e-8366-4e18-aea3-4cb4a3a50b48")
 
@@ -262,28 +321,30 @@
 ## Power BI Rest API Operations
 
 `pbipy` methods wrap around the Operations described in the Power BI Rest API Reference:
 
 [Power BI REST APIs for embedded analytics and automation - Power BI REST API](https://learn.microsoft.com/en-us/rest/api/power-bi/)
 
 
-## Development Progress
+## What's implemented?
+
+Most of the core operations on Datasets, Workspaces (Groups), Reports, Apps, and Dataflows are implemented. Given the many available endpoints, not everything is covered by `pbipy`, so expect a few features to be missing.
 
-`pbipy` is in development so expect a few features to be missing. The aim is to cover off most of the core stuff like Datasets, Workspaces (Groups), Reports, Apps, etc., and the rest later on. Check back regularly to see what's been added or still in the pipeline.
+If an operation is missing and you think it'd be useful, feel free to suggest it on the [Issues tab](https://github.com/andrewvillazon/pbipy/issues).
 
-| PowerBI Component   	| Progress 	| Notes 	|
-|---------------------	|----------	|-------	|
-| Datasets            	| Done     	|       	|
-| Groups (Workspaces) 	| Done    	|       	|
-| Reports             	| Done      |       	|
-| Apps                	| Done   	|       	|
-| Dataflows           	| Done    	|       	|
-| Admin Operations     	| Doing    	|       	|
-| Dashboards          	| Todo     	|       	|
-| Everything else     	| Backlog  	|       	|
+| PowerBI Component   	| Progress 	| Notes 	                                                                            |
+|---------------------	|----------	|-------------------------------------------------------------------------------------- |
+| Datasets            	| Done     	|       	                                                                            |
+| Groups (Workspaces) 	| Done    	|       	                                                                            |
+| Reports             	| Done      |       	                                                                            |
+| Apps                	| Done   	|       	                                                                            |
+| Dataflows           	| Done    	|       	                                                                            |
+| Admin Operations     	| Done    	| Implements operations related to Datasets, Groups, Reports, Apps, and Dataflows only. |
+| Dashboards          	| Todo     	|       	                                                                            |
+| Everything else     	| Backlog  	|       	                                                                            |
 
 ## Contributing
 
 Contributions such as bug reports, fixes, documentation or docstrings, enhancements, and ideas are welcome. `pbipy` uses github to host code, track issues, record feature requests, and accept pull requests.
 
 A `contributing.md` is in the works, but in the meantime below is a general guide.
```

### Comparing `pbipy-2.4.5/README.md` & `pbipy-2.5.6/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -23,37 +23,31 @@
 
 ## Getting Started: Authentication
 
 To use `pbipy` you'll first need to acquire a `bearer_token`.
 
 *How do I get a `bearer_token`?*
 
-To acquire a `bearer_token` you'll need to authenticate against your [Registered Azure Power BI App](https://learn.microsoft.com/en-us/power-bi/developer/embedded/register-app?tabs=customers). Registering is the first step in turning on the Power BI Rest API, so from this point on it's assumed your Power BI Rest API is up and running.
+To acquire a `bearer_token` you'll need to authenticate against your [Registered Azure Power BI App](https://learn.microsoft.com/en-us/power-bi/developer/embedded/register-app?tabs=customers). Registering is the first step in turning on the Power BI Rest API, so from here on it's assumed your Power BI Rest API is up and running.
 
-To authenticate against the Registered App, Microsoft provides the `MSAL` and `azure-identity` python libraries. These libraries support many different ways of acquiring a `bearer_token`.
+To authenticate against the Registered App, Microsoft provides the `MSAL` and `azure-identity` python libraries. These libraries support different ways of acquiring a `bearer_token` and which to use will depend on how your cloud/tenant is configured.
 
-Because there are multiple ways to acquire the token, `pbipy` assumes you'll do this in the way that suits, rather than directly handling authentication (of course, this might change in future).
+Because there are multiple ways to acquire the token, `pbipy` leaves it up to do this in the way that suits, rather than directly handling authentication (of course, this might change in future).
 
-This `README` doesn't cover Authentication in detail, however, these are some helpful resources that look at acquiring a `bearer_token` in the context of Power BI:
+This `README` doesn't cover authentication in detail, however, these are some helpful resources that look at acquiring a `bearer_token` in the context of Power BI:
 
 * [Power BI REST API with Python and MSAL. Part II.](https://www.datalineo.com/post/power-bi-rest-api-with-python-and-msal-part-ii)
 * [Power BI REST API with Python Part III, azure-identity](https://www.datalineo.com/post/power-bi-rest-api-with-python-part-iii-azure-identity)
 * [Monitoring Power BI using REST APIs from Python](https://data-goblins.com/power-bi/power-bi-api-python)
 
-The example below uses the `msal` library to to get a `bearer_token`.
-
-## Useage
-
-Start by creating the `PowerBI()` client. All interactions with the Power BI Rest API go through this object. 
+The example below uses the `msal` library to to get a bearer_token.
 
 ```python
 import msal
 
-from pbipy import PowerBI
-
 
 #  msal auth setup
 def acquire_bearer_token(username, password, azure_tenant_id, client_id, scopes):
     app = msal.PublicClientApplication(client_id, authority=azure_tenant_id)
     result = app.acquire_token_by_username_password(username, password, scopes)
     return result["access_token"]
 
@@ -61,16 +55,25 @@
 bearer_token = acquire_bearer_token(
     username="your-username",
     password="your-password",
     azure_tenant_id="https://login.microsoftonline.com/your-azure-tenant-id",
     client_id="your-pbi-client-id",
     scopes=["https://analysis.windows.net/powerbi/api/.default"],
 )
+```
+
+The code that follows assumes you've authenticated and acquired your `bearer_token`.
+
+## Useage
+
+Start by creating the `PowerBI()` client. Interactions with the Power BI Rest API go through this object. 
+
+```python
+from pbipy import PowerBI
 
-# Create Client
 pbi = PowerBI(bearer_token)
 ```
 
 To interact with the API, simply call the relevant method from the client.
 
 ```python
 # Grab the datasets from a workspace
@@ -89,23 +92,29 @@
 # <class 'pbipy.resources.Dataset'>
 # True
 ```
 
 Most methods take in an object id...
 
 ```python
-dataset = pbi.dataset("cfafbeb1-8037-4d0c-896e-a46fb27ff229", group="a2f89923-421a-464e-bf4c-25eab39bb09f")
+dataset = pbi.dataset(
+    id="cfafbeb1-8037-4d0c-896e-a46fb27ff229",
+    group="a2f89923-421a-464e-bf4c-25eab39bb09f"
+)
 ```
 
 ... or just pass in the object itself.
 
 ```python
 group = pbi.group("a2f89923-421a-464e-bf4c-25eab39bb09f")
 
-dataset = pbi.dataset("cfafbeb1-8037-4d0c-896e-a46fb27ff229", group=group)
+dataset = pbi.dataset(
+    "cfafbeb1-8037-4d0c-896e-a46fb27ff229"
+    ,group=group
+)
 ```
 
 If you need to access the raw json representation, this is supported to.
 
 ```python
 sales = pbi.dataset("cfafbeb1-8037-4d0c-896e-a46fb27ff229")
 
@@ -120,65 +129,65 @@
 # }
 ```
 
 ## Example: Working with Datasets
 
 Let's see how `pbipy` works by performing some operations on a Dataset.
 
-First, we need to load the Dataset from the API. To do this, we call the `dataset()` method from the `pbi` client we created above. 
-
-The Power BI Rest API will look for the Dataset in the current user's workspace if we don't provide a `group` argument.
+First, we initialize our client.
 
 ```python
-sales = pbi.dataset(id="cfafbeb1-8037-4d0c-896e-a46fb27ff229")
-print(sales)
+from pbipy import PowerBI
 
-# <Dataset id='cfafbeb1-8037-4d0c-896e-a46fb27ff229', name='SalesMarketing', ...>
+pbi = PowerBI(bearer_token)
 ```
 
-But we likely want to target a Dataset in a *Workspace*. To do this, we provide the Workspace Id as the `group` argument when we call the `dataset()` method.
+Now that we've got a client, we can load a Dataset from the API. To load a Dataset, we call the `dataset()` method with an `id` and `group` argument. In the Power BI Rest API, a **Group** and **Workspace** are synonymous and used interchangeably.
 
 ```python
 sales = pbi.dataset(
-    "cfafbeb1-8037-4d0c-896e-a46fb27ff229",
+    id="cfafbeb1-8037-4d0c-896e-a46fb27ff229",
     group="f089354e-8366-4e18-aea3-4cb4a3a50b48",
 )
+
+print(sales)
+
+# <Dataset id='cfafbeb1-8037-4d0c-896e-a46fb27ff229', name='SalesMarketing', ...>
 ```
 
-Now that we've got our target Dataset let's look at its Refresh History. We call the `refresh_history()` method on our Dataset. Easy.
+Dataset not updating? Let's look at the Refresh History. 
 
-```python
-dataset = pbi.dataset(
-    "cfafbeb1-8037-4d0c-896e-a46fb27ff229",
-    group="f089354e-8366-4e18-aea3-4cb4a3a50b48",
-)
+We call the `refresh_history()` method on our Dataset. Easy.
 
-refresh_history = dataset.refresh_history()
+```python
+refresh_history = sales.refresh_history()
 
 for entry in refresh_history:
     print(entry)
 
 # {"refreshType":"ViaApi", "startTime":"2017-06-13T09:25:43.153Z", "status": "Completed" ...}
 ```
 
-How about adding some user permissions to our Dataset? That's easy too. Just call the `add_user()` method with the User's details and permissions.
+Need to kick off a refresh? That's easy too.
 
 ```python
-sales_ds = pbi.dataset( "cfafbeb1-8037-4d0c-896e-a46fb27ff229")
+sales.refresh()
+```
+
+How about adding some user permissions to our Dataset? Just call the `add_user()` method with the User's details and permissions.
 
+```python
 # Give John 'Read' access on the dataset
-sales_ds.add_user("john@contoso.com", "User", "Read")
+sales.add_user("john@contoso.com", "User", "Read")
 ```
 
 Lastly, if we're feeling adventurous, we can execute DAX against a Dataset and use the results in Python.
 
 ```python
-dataset = pbi.dataset( "cfafbeb1-8037-4d0c-896e-a46fb27ff229")
-
-dxq_result = dataset.execute_queries("EVALUATE VALUES(MyTable)")
+dxq_result = sales.execute_queries("EVALUATE VALUES(MyTable)")
 print(dxq_result)
 
 # {
 #   "results": [
 #     {
 #       "tables": [
 #         {
@@ -187,14 +196,64 @@
 #               "MyTable[Year]": 2010,
 #               "MyTable[Quarter]": "Q1"
 #             },
 # ...
 # }
 ```
 
+## Example: Working with the Admin object
+
+`pbypi` also supports [Administrator Operations](https://learn.microsoft.com/en-us/rest/api/power-bi/admin), specialized operations available to users with Power BI Admin rights. Let's see how we can use these.
+
+First, we need to initialize our client. Then we call the `admin` method and initialize an `Admin` object.
+
+```python
+from pbipy import PowerBI
+
+pbi = PowerBI(bearer_token)
+admin = pbi.admin()
+```
+
+Need to review some access on some reports? We can call the `report_users` method.
+
+```python
+users = admin.report_users("5b218778-e7a5-4d73-8187-f10824047715")
+print(users[0])
+
+# {"displayName": "John Nick", "emailAddress": "john@contoso.com", ...}
+```
+
+What about understanding User activity on your Power BI tenant?
+
+```python
+from datetime import datetime
+
+start_dtm = datetime(2019, 8, 31, 0, 0, 0)
+end_dtm = datetime(2019, 8, 31, 23, 59, 59)
+
+activity_events = admin.activity_events(start_dtm, end_dtm)
+
+print(activity_events)
+
+# [
+#   {
+#       "Id": "41ce06d1", 
+#       "CreationTime": "2019-08-13T07:55:15", 
+#       "Operation": "ViewReport", 
+#       ...
+#   },
+#   {
+#       "Id": "c632aa64", 
+#       "CreationTime": "2019-08-13T07:55:10", 
+#       "Operation": "GetSnapshots", 
+#       ...
+#   }
+# ]
+```
+
 ## More examples
 
 ### Datasets in a Workspace
 
 ```python
 datasets = pbi.datasets(group="f089354e-8366-4e18-aea3-4cb4a3a50b48")
 
@@ -242,28 +301,30 @@
 ## Power BI Rest API Operations
 
 `pbipy` methods wrap around the Operations described in the Power BI Rest API Reference:
 
 [Power BI REST APIs for embedded analytics and automation - Power BI REST API](https://learn.microsoft.com/en-us/rest/api/power-bi/)
 
 
-## Development Progress
+## What's implemented?
+
+Most of the core operations on Datasets, Workspaces (Groups), Reports, Apps, and Dataflows are implemented. Given the many available endpoints, not everything is covered by `pbipy`, so expect a few features to be missing.
 
-`pbipy` is in development so expect a few features to be missing. The aim is to cover off most of the core stuff like Datasets, Workspaces (Groups), Reports, Apps, etc., and the rest later on. Check back regularly to see what's been added or still in the pipeline.
+If an operation is missing and you think it'd be useful, feel free to suggest it on the [Issues tab](https://github.com/andrewvillazon/pbipy/issues).
 
-| PowerBI Component   	| Progress 	| Notes 	|
-|---------------------	|----------	|-------	|
-| Datasets            	| Done     	|       	|
-| Groups (Workspaces) 	| Done    	|       	|
-| Reports             	| Done      |       	|
-| Apps                	| Done   	|       	|
-| Dataflows           	| Done    	|       	|
-| Admin Operations     	| Doing    	|       	|
-| Dashboards          	| Todo     	|       	|
-| Everything else     	| Backlog  	|       	|
+| PowerBI Component   	| Progress 	| Notes 	                                                                            |
+|---------------------	|----------	|-------------------------------------------------------------------------------------- |
+| Datasets            	| Done     	|       	                                                                            |
+| Groups (Workspaces) 	| Done    	|       	                                                                            |
+| Reports             	| Done      |       	                                                                            |
+| Apps                	| Done   	|       	                                                                            |
+| Dataflows           	| Done    	|       	                                                                            |
+| Admin Operations     	| Done    	| Implements operations related to Datasets, Groups, Reports, Apps, and Dataflows only. |
+| Dashboards          	| Todo     	|       	                                                                            |
+| Everything else     	| Backlog  	|       	                                                                            |
 
 ## Contributing
 
 Contributions such as bug reports, fixes, documentation or docstrings, enhancements, and ideas are welcome. `pbipy` uses github to host code, track issues, record feature requests, and accept pull requests.
 
 A `contributing.md` is in the works, but in the meantime below is a general guide.
```

### Comparing `pbipy-2.4.5/pbipy/apps.py` & `pbipy-2.5.6/pbipy/apps.py`

 * *Files identical despite different names*

### Comparing `pbipy-2.4.5/pbipy/dashboards.py` & `pbipy-2.5.6/pbipy/dashboards.py`

 * *Files identical despite different names*

### Comparing `pbipy-2.4.5/pbipy/dataflows.py` & `pbipy-2.5.6/pbipy/dataflows.py`

 * *Files identical despite different names*

### Comparing `pbipy-2.4.5/pbipy/datasets.py` & `pbipy-2.5.6/pbipy/datasets.py`

 * *Files identical despite different names*

### Comparing `pbipy-2.4.5/pbipy/groups.py` & `pbipy-2.5.6/pbipy/groups.py`

 * *Files identical despite different names*

### Comparing `pbipy-2.4.5/pbipy/powerbi.py` & `pbipy-2.5.6/pbipy/powerbi.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 
 Full API documentation can be found at:
 
 https://learn.microsoft.com/en-us/rest/api/power-bi/
 """
 
 import requests
-from requests.exceptions import HTTPError
 
 from pbipy import settings
+from pbipy.admin import Admin
 from pbipy.apps import App
 from pbipy.dataflows import Dataflow
-from pbipy.groups import Group
 from pbipy.datasets import Dataset
+from pbipy.groups import Group
 from pbipy.reports import Report
 from pbipy.utils import RequestsMixin, remove_no_values
 
 
 class PowerBI(RequestsMixin):
     """
     User Interface into Power BI Rest Api.
@@ -54,14 +54,30 @@
         self.bearer_token = bearer_token
 
         if not session:
             self.session = requests.Session()
 
         self.session.headers.update({"Authorization": f"Bearer {self.bearer_token}"})
 
+    def admin(
+        self,
+    ) -> Admin:
+        """
+        Initialize and return an `Admin` object. The `Admin` object is used
+        to access admin-only functionality.
+
+        Returns
+        -------
+        `Admin`
+            The initialized `Admin` object.
+        
+        """
+
+        return Admin(self.session)
+
     def app(
         self,
         app: str,
     ) -> App:
         """
         Return the specified installed app.
 
@@ -111,16 +127,16 @@
         Attempt to cancel the specified Dataflow Transaction.
 
         Parameters
         ----------
         `transaction_id` : `str`
             Id of the Transaction to cancel.
         `group` : `str | Group`
-            Group Id or `Group` object where the Transaction originated. 
-            Should match the Group of the Dataflow that generated the 
+            Group Id or `Group` object where the Transaction originated.
+            Should match the Group of the Dataflow that generated the
             transaction.
 
         Returns
         -------
         `dict`
             Dataflow transaction status.
 
@@ -229,36 +245,36 @@
 
     def delete_dataflow(
         self,
         dataflow: str | Dataflow,
         group: str | Group,
     ) -> None:
         """
-        Deletes a dataflow from Power BI data prep storage, including its 
+        Deletes a dataflow from Power BI data prep storage, including its
         definition file and model.
 
         Parameters
         ----------
         `dataflow` : `str | Dataflow`
             Dataflow Id or `Dataflow` object to delete.
         `group` : `str | Group`
             Group Id or `Group` object where the Dataflow resides.
-        
+
         """
 
         if isinstance(dataflow, Dataflow):
             dataflow_id = dataflow.id
         else:
             dataflow_id = dataflow
-        
+
         if isinstance(group, Group):
             group_id = group.id
         else:
             group_id = group
-        
+
         resource = self.BASE_URL + f"/groups/{group_id}/dataflows/{dataflow_id}"
 
         self.delete(resource, self.session)
 
     # TODO: Add support for passing in a group obj
     def dataset(
         self,
```

### Comparing `pbipy-2.4.5/pbipy/reports.py` & `pbipy-2.5.6/pbipy/reports.py`

 * *Files identical despite different names*

### Comparing `pbipy-2.4.5/pbipy/resources.py` & `pbipy-2.5.6/pbipy/resources.py`

 * *Files identical despite different names*

### Comparing `pbipy-2.4.5/pbipy/utils.py` & `pbipy-2.5.6/pbipy/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,55 @@
 """Utility functions and classes used internally by pybi."""
 
 import json
 from pathlib import Path
 import re
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from pbipy.resources import Resource
 
 from requests import Response, Session
 from requests.exceptions import HTTPError
 
 
+def build_path(
+    path_format: str,
+    *identifiers: "str | Resource",
+) -> str:
+    """
+    Build a path to a resource from the supplied components.
+
+    Parameters
+    ----------
+    `path_format` : `str`
+        The resource format with bracketed placeholders, e.g., `reports/{}/datasources`
+    `*identifiers` : `str | Resource`
+        Ids or Resource Objects with an `id` attribute. The provided Ids
+        will be added to the path according `path_format`.
+
+    Returns
+    -------
+    `str`
+        Path to a resource.
+    
+    """
+    
+    ids = []
+
+    for identifier in identifiers:
+        try:
+            ids.append(identifier.id)
+        except AttributeError:
+            ids.append(identifier)
+    
+    path = path_format.format(*ids)
+
+    return path
+
+
 def to_snake_case(s):
     pattern = re.compile("((?<=[a-z0-9])[A-Z]|(?!^)[A-Z](?=[a-z]))")
     return pattern.sub(r"_\1", s).lower()
 
 
 def to_camel_case(text):
     s = text.replace("-", " ").replace("_", " ")
@@ -131,14 +169,15 @@
     Mostly requests lib boilerplate with a sprinkling of json parsing.
     """
 
     def delete(
         self,
         resource: str,
         session: Session,
+        params: dict = None,
         success_codes: list[int] = [200, 201],
     ) -> None:
         """
         Make a delete request to an api endpoint.
 
         Parameters
         ----------
@@ -152,15 +191,18 @@
 
         Raises
         ------
         `HTTPError`
             If the response status code was not found in `success_codes`.
         """
 
-        response = session.delete(resource)
+        response = session.delete(
+            resource,
+            params=params,
+        )
 
         if response.status_code not in success_codes:
             raise HTTPError(
                 f"""Encountered api error. Response: 
                 
                 {json.dumps(response.json(), indent=True)})"""
             )
```

### Comparing `pbipy-2.4.5/pbipy.egg-info/PKG-INFO` & `pbipy-2.5.6/pbipy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbipy
-Version: 2.4.5
+Version: 2.5.6
 Summary: A Python Library for interacting with the Power BI Rest API.
 Home-page: https://github.com/andrewvillazon/pbipy
 Author: Andrew Villazon
 Author-email: andrew.villazon@gmail.com
 License: Apache 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -43,37 +43,31 @@
 
 ## Getting Started: Authentication
 
 To use `pbipy` you'll first need to acquire a `bearer_token`.
 
 *How do I get a `bearer_token`?*
 
-To acquire a `bearer_token` you'll need to authenticate against your [Registered Azure Power BI App](https://learn.microsoft.com/en-us/power-bi/developer/embedded/register-app?tabs=customers). Registering is the first step in turning on the Power BI Rest API, so from this point on it's assumed your Power BI Rest API is up and running.
+To acquire a `bearer_token` you'll need to authenticate against your [Registered Azure Power BI App](https://learn.microsoft.com/en-us/power-bi/developer/embedded/register-app?tabs=customers). Registering is the first step in turning on the Power BI Rest API, so from here on it's assumed your Power BI Rest API is up and running.
 
-To authenticate against the Registered App, Microsoft provides the `MSAL` and `azure-identity` python libraries. These libraries support many different ways of acquiring a `bearer_token`.
+To authenticate against the Registered App, Microsoft provides the `MSAL` and `azure-identity` python libraries. These libraries support different ways of acquiring a `bearer_token` and which to use will depend on how your cloud/tenant is configured.
 
-Because there are multiple ways to acquire the token, `pbipy` assumes you'll do this in the way that suits, rather than directly handling authentication (of course, this might change in future).
+Because there are multiple ways to acquire the token, `pbipy` leaves it up to do this in the way that suits, rather than directly handling authentication (of course, this might change in future).
 
-This `README` doesn't cover Authentication in detail, however, these are some helpful resources that look at acquiring a `bearer_token` in the context of Power BI:
+This `README` doesn't cover authentication in detail, however, these are some helpful resources that look at acquiring a `bearer_token` in the context of Power BI:
 
 * [Power BI REST API with Python and MSAL. Part II.](https://www.datalineo.com/post/power-bi-rest-api-with-python-and-msal-part-ii)
 * [Power BI REST API with Python Part III, azure-identity](https://www.datalineo.com/post/power-bi-rest-api-with-python-part-iii-azure-identity)
 * [Monitoring Power BI using REST APIs from Python](https://data-goblins.com/power-bi/power-bi-api-python)
 
-The example below uses the `msal` library to to get a `bearer_token`.
-
-## Useage
-
-Start by creating the `PowerBI()` client. All interactions with the Power BI Rest API go through this object. 
+The example below uses the `msal` library to to get a bearer_token.
 
 ```python
 import msal
 
-from pbipy import PowerBI
-
 
 #  msal auth setup
 def acquire_bearer_token(username, password, azure_tenant_id, client_id, scopes):
     app = msal.PublicClientApplication(client_id, authority=azure_tenant_id)
     result = app.acquire_token_by_username_password(username, password, scopes)
     return result["access_token"]
 
@@ -81,16 +75,25 @@
 bearer_token = acquire_bearer_token(
     username="your-username",
     password="your-password",
     azure_tenant_id="https://login.microsoftonline.com/your-azure-tenant-id",
     client_id="your-pbi-client-id",
     scopes=["https://analysis.windows.net/powerbi/api/.default"],
 )
+```
+
+The code that follows assumes you've authenticated and acquired your `bearer_token`.
+
+## Useage
+
+Start by creating the `PowerBI()` client. Interactions with the Power BI Rest API go through this object. 
+
+```python
+from pbipy import PowerBI
 
-# Create Client
 pbi = PowerBI(bearer_token)
 ```
 
 To interact with the API, simply call the relevant method from the client.
 
 ```python
 # Grab the datasets from a workspace
@@ -109,23 +112,29 @@
 # <class 'pbipy.resources.Dataset'>
 # True
 ```
 
 Most methods take in an object id...
 
 ```python
-dataset = pbi.dataset("cfafbeb1-8037-4d0c-896e-a46fb27ff229", group="a2f89923-421a-464e-bf4c-25eab39bb09f")
+dataset = pbi.dataset(
+    id="cfafbeb1-8037-4d0c-896e-a46fb27ff229",
+    group="a2f89923-421a-464e-bf4c-25eab39bb09f"
+)
 ```
 
 ... or just pass in the object itself.
 
 ```python
 group = pbi.group("a2f89923-421a-464e-bf4c-25eab39bb09f")
 
-dataset = pbi.dataset("cfafbeb1-8037-4d0c-896e-a46fb27ff229", group=group)
+dataset = pbi.dataset(
+    "cfafbeb1-8037-4d0c-896e-a46fb27ff229"
+    ,group=group
+)
 ```
 
 If you need to access the raw json representation, this is supported to.
 
 ```python
 sales = pbi.dataset("cfafbeb1-8037-4d0c-896e-a46fb27ff229")
 
@@ -140,65 +149,65 @@
 # }
 ```
 
 ## Example: Working with Datasets
 
 Let's see how `pbipy` works by performing some operations on a Dataset.
 
-First, we need to load the Dataset from the API. To do this, we call the `dataset()` method from the `pbi` client we created above. 
-
-The Power BI Rest API will look for the Dataset in the current user's workspace if we don't provide a `group` argument.
+First, we initialize our client.
 
 ```python
-sales = pbi.dataset(id="cfafbeb1-8037-4d0c-896e-a46fb27ff229")
-print(sales)
+from pbipy import PowerBI
 
-# <Dataset id='cfafbeb1-8037-4d0c-896e-a46fb27ff229', name='SalesMarketing', ...>
+pbi = PowerBI(bearer_token)
 ```
 
-But we likely want to target a Dataset in a *Workspace*. To do this, we provide the Workspace Id as the `group` argument when we call the `dataset()` method.
+Now that we've got a client, we can load a Dataset from the API. To load a Dataset, we call the `dataset()` method with an `id` and `group` argument. In the Power BI Rest API, a **Group** and **Workspace** are synonymous and used interchangeably.
 
 ```python
 sales = pbi.dataset(
-    "cfafbeb1-8037-4d0c-896e-a46fb27ff229",
+    id="cfafbeb1-8037-4d0c-896e-a46fb27ff229",
     group="f089354e-8366-4e18-aea3-4cb4a3a50b48",
 )
+
+print(sales)
+
+# <Dataset id='cfafbeb1-8037-4d0c-896e-a46fb27ff229', name='SalesMarketing', ...>
 ```
 
-Now that we've got our target Dataset let's look at its Refresh History. We call the `refresh_history()` method on our Dataset. Easy.
+Dataset not updating? Let's look at the Refresh History. 
 
-```python
-dataset = pbi.dataset(
-    "cfafbeb1-8037-4d0c-896e-a46fb27ff229",
-    group="f089354e-8366-4e18-aea3-4cb4a3a50b48",
-)
+We call the `refresh_history()` method on our Dataset. Easy.
 
-refresh_history = dataset.refresh_history()
+```python
+refresh_history = sales.refresh_history()
 
 for entry in refresh_history:
     print(entry)
 
 # {"refreshType":"ViaApi", "startTime":"2017-06-13T09:25:43.153Z", "status": "Completed" ...}
 ```
 
-How about adding some user permissions to our Dataset? That's easy too. Just call the `add_user()` method with the User's details and permissions.
+Need to kick off a refresh? That's easy too.
 
 ```python
-sales_ds = pbi.dataset( "cfafbeb1-8037-4d0c-896e-a46fb27ff229")
+sales.refresh()
+```
+
+How about adding some user permissions to our Dataset? Just call the `add_user()` method with the User's details and permissions.
 
+```python
 # Give John 'Read' access on the dataset
-sales_ds.add_user("john@contoso.com", "User", "Read")
+sales.add_user("john@contoso.com", "User", "Read")
 ```
 
 Lastly, if we're feeling adventurous, we can execute DAX against a Dataset and use the results in Python.
 
 ```python
-dataset = pbi.dataset( "cfafbeb1-8037-4d0c-896e-a46fb27ff229")
-
-dxq_result = dataset.execute_queries("EVALUATE VALUES(MyTable)")
+dxq_result = sales.execute_queries("EVALUATE VALUES(MyTable)")
 print(dxq_result)
 
 # {
 #   "results": [
 #     {
 #       "tables": [
 #         {
@@ -207,14 +216,64 @@
 #               "MyTable[Year]": 2010,
 #               "MyTable[Quarter]": "Q1"
 #             },
 # ...
 # }
 ```
 
+## Example: Working with the Admin object
+
+`pbypi` also supports [Administrator Operations](https://learn.microsoft.com/en-us/rest/api/power-bi/admin), specialized operations available to users with Power BI Admin rights. Let's see how we can use these.
+
+First, we need to initialize our client. Then we call the `admin` method and initialize an `Admin` object.
+
+```python
+from pbipy import PowerBI
+
+pbi = PowerBI(bearer_token)
+admin = pbi.admin()
+```
+
+Need to review some access on some reports? We can call the `report_users` method.
+
+```python
+users = admin.report_users("5b218778-e7a5-4d73-8187-f10824047715")
+print(users[0])
+
+# {"displayName": "John Nick", "emailAddress": "john@contoso.com", ...}
+```
+
+What about understanding User activity on your Power BI tenant?
+
+```python
+from datetime import datetime
+
+start_dtm = datetime(2019, 8, 31, 0, 0, 0)
+end_dtm = datetime(2019, 8, 31, 23, 59, 59)
+
+activity_events = admin.activity_events(start_dtm, end_dtm)
+
+print(activity_events)
+
+# [
+#   {
+#       "Id": "41ce06d1", 
+#       "CreationTime": "2019-08-13T07:55:15", 
+#       "Operation": "ViewReport", 
+#       ...
+#   },
+#   {
+#       "Id": "c632aa64", 
+#       "CreationTime": "2019-08-13T07:55:10", 
+#       "Operation": "GetSnapshots", 
+#       ...
+#   }
+# ]
+```
+
 ## More examples
 
 ### Datasets in a Workspace
 
 ```python
 datasets = pbi.datasets(group="f089354e-8366-4e18-aea3-4cb4a3a50b48")
 
@@ -262,28 +321,30 @@
 ## Power BI Rest API Operations
 
 `pbipy` methods wrap around the Operations described in the Power BI Rest API Reference:
 
 [Power BI REST APIs for embedded analytics and automation - Power BI REST API](https://learn.microsoft.com/en-us/rest/api/power-bi/)
 
 
-## Development Progress
+## What's implemented?
+
+Most of the core operations on Datasets, Workspaces (Groups), Reports, Apps, and Dataflows are implemented. Given the many available endpoints, not everything is covered by `pbipy`, so expect a few features to be missing.
 
-`pbipy` is in development so expect a few features to be missing. The aim is to cover off most of the core stuff like Datasets, Workspaces (Groups), Reports, Apps, etc., and the rest later on. Check back regularly to see what's been added or still in the pipeline.
+If an operation is missing and you think it'd be useful, feel free to suggest it on the [Issues tab](https://github.com/andrewvillazon/pbipy/issues).
 
-| PowerBI Component   	| Progress 	| Notes 	|
-|---------------------	|----------	|-------	|
-| Datasets            	| Done     	|       	|
-| Groups (Workspaces) 	| Done    	|       	|
-| Reports             	| Done      |       	|
-| Apps                	| Done   	|       	|
-| Dataflows           	| Done    	|       	|
-| Admin Operations     	| Doing    	|       	|
-| Dashboards          	| Todo     	|       	|
-| Everything else     	| Backlog  	|       	|
+| PowerBI Component   	| Progress 	| Notes 	                                                                            |
+|---------------------	|----------	|-------------------------------------------------------------------------------------- |
+| Datasets            	| Done     	|       	                                                                            |
+| Groups (Workspaces) 	| Done    	|       	                                                                            |
+| Reports             	| Done      |       	                                                                            |
+| Apps                	| Done   	|       	                                                                            |
+| Dataflows           	| Done    	|       	                                                                            |
+| Admin Operations     	| Done    	| Implements operations related to Datasets, Groups, Reports, Apps, and Dataflows only. |
+| Dashboards          	| Todo     	|       	                                                                            |
+| Everything else     	| Backlog  	|       	                                                                            |
 
 ## Contributing
 
 Contributions such as bug reports, fixes, documentation or docstrings, enhancements, and ideas are welcome. `pbipy` uses github to host code, track issues, record feature requests, and accept pull requests.
 
 A `contributing.md` is in the works, but in the meantime below is a general guide.
```

### Comparing `pbipy-2.4.5/setup.py` & `pbipy-2.5.6/setup.py`

 * *Files identical despite different names*

