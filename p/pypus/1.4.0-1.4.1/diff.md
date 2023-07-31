# Comparing `tmp/pypus-1.4.0.tar.gz` & `tmp/pypus-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypus-1.4.0.tar", max compression
+gzip compressed data, was "pypus-1.4.1.tar", max compression
```

## Comparing `pypus-1.4.0.tar` & `pypus-1.4.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2021-05-28 19:35:21.744187 pypus-1.4.0/LICENSE
--rw-r--r--   0        0        0      114 2021-05-28 19:36:19.806135 pypus-1.4.0/README.md
--rw-r--r--   0        0        0      587 2023-07-31 20:24:50.000783 pypus-1.4.0/pyproject.toml
--rw-r--r--   0        0        0      937 2023-07-31 18:46:58.056574 pypus-1.4.0/src/pypus/Octo.py
--rw-r--r--   0        0        0        0 2021-05-11 19:37:09.641525 pypus-1.4.0/src/pypus/__init__.py
--rw-r--r--   0        0        0    30814 2023-07-31 20:16:54.250552 pypus-1.4.0/src/pypus/cli.py
--rw-r--r--   0        0        0      601 2023-07-31 14:50:20.344572 pypus-1.4.0/src/pypus/shelf.py
--rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 pypus-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2021-05-28 19:35:21.744187 pypus-1.4.1/LICENSE
+-rw-r--r--   0        0        0      114 2021-05-28 19:36:19.806135 pypus-1.4.1/README.md
+-rw-r--r--   0        0        0      587 2023-07-31 21:48:29.015431 pypus-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0      937 2023-07-31 18:46:58.056574 pypus-1.4.1/src/pypus/Octo.py
+-rw-r--r--   0        0        0        0 2021-05-11 19:37:09.641525 pypus-1.4.1/src/pypus/__init__.py
+-rw-r--r--   0        0        0    33139 2023-07-31 21:36:32.576802 pypus-1.4.1/src/pypus/cli.py
+-rw-r--r--   0        0        0      601 2023-07-31 21:09:19.484807 pypus-1.4.1/src/pypus/shelf.py
+-rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 pypus-1.4.1/PKG-INFO
```

### Comparing `pypus-1.4.0/LICENSE` & `pypus-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypus-1.4.0/pyproject.toml` & `pypus-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pypus"
-version = "1.4.0"
+version = "1.4.1"
 description = "Octopus cli toolkit"
 authors = ["Michael MacKenna <mmackenna@unitedfiregroup.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `pypus-1.4.0/src/pypus/Octo.py` & `pypus-1.4.1/src/pypus/Octo.py`

 * *Files identical despite different names*

### Comparing `pypus-1.4.0/src/pypus/cli.py` & `pypus-1.4.1/src/pypus/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,14 +185,68 @@
         for var in project_variables['Variables']:
             print(f"ID: {var['Id']} Name: {var['Name']} Value: {var['Value']} Scope: {var['Scope']}")
         return project_variables
     else:
         return None
 
 
+@main.command('get-vars-add-toshelf', short_help='Get a list of vars for a project in a space and add to shelf')
+@click.argument("space")
+@click.argument("project")
+@click.argument("shelf-name")
+def get_vars(space, project, shelf_name):
+    """ Get a list of vars for a project within a space
+
+    Arguments:
+        space: The space where the project resides
+        project: The project from which to get variables
+        shelf-name: The name of the shelf to create
+
+    """
+    def get_octopus_resource(uri, headers, skip_count = 0):
+        """ Gets a resource from the API
+
+        Arguments:
+            uri: The base url of the Octopus Deploy API
+        """
+        items = []
+        response = requests.get((uri + "?skip=" + str(skip_count)), headers=headers, verify=False)
+        response.raise_for_status()
+        # Get results of API call
+        results = json.loads(response.content.decode('utf-8'))
+        # Store results
+        if 'Items' in results.keys():
+            items += results['Items']
+
+            # Check to see if there are more results
+            if (len(results['Items']) > 0) and (len(results['Items']) == results['ItemsPerPage']):
+                skip_count += results['ItemsPerPage']
+                items += get_octopus_resource(uri, headers, skip_count)
+
+        else:
+            return results
+        # return results
+        return items
+    octopus_api_key = os.getenv('OCTOPUS_API_KEY')
+    octopus_server_uri = os.getenv('OCTOPUS_SERVER_URI')
+    headers = {'X-Octopus-ApiKey': octopus_api_key}
+    project_name = project
+    space_name = space
+    uri = '{0}/spaces'.format(octopus_server_uri)
+    spaces = get_octopus_resource(uri, headers)
+    space = next((x for x in spaces if x['Name'] == space_name), None)
+    uri = '{0}/{1}/projects'.format(octopus_server_uri, space['Id'])
+    projects = get_octopus_resource(uri, headers)
+    project = next((x for x in projects if x['Name'] == project_name), None)
+    if project != None:
+        uri = '{0}/{1}/variables/{2}'.format(octopus_server_uri, space['Id'], project['VariableSetId'])
+        project_variables = get_octopus_resource(uri, headers)
+        new_shelf = shelf.shelf_add_item(shelf_name, 'Variables', project_variables)
+    else:
+        print(f"Unable to locate project {project}")
 
 @main.command('set-var', short_help='Set a variable for a project in a space')
 @click.argument("space")
 @click.argument("project")
 @click.argument("variable-name")
 @click.argument("variable-value")
 @click.argument("variable-scope")
@@ -614,15 +668,15 @@
 
 
 @main.command("get-shelf-key", short_help="Print data for a key in a shelf")
 @click.argument("shelf_name")
 @click.argument("key_name")
 def get_shelf_key(shelf_name, key_name):
     contents = shelf.get_shelf_item(shelf_name, key_name)
-    for var in contents:
+    for var in contents['Variables']:
         print(f"{var['Name']} {var['Value']} {var['Scope']}")
 
 
 @main.command('transpose-from-shelf', short_help='Transpose varaibles from shelf')
 @click.argument('shelf-name')
 @click.argument('key-name')
 @click.argument('yaml-map-file', type=click.Path(exists=True))
@@ -644,15 +698,15 @@
     contents = shelf.get_shelf_item(shelf_name, key_name)
     with open(yaml_map_file, 'r') as stream:
         try:
             map_values = yaml.safe_load(stream)
         except yaml.YAMLError as e:
             print(e)
 
-    for var in contents:
+    for var in contents['Variables']:
         obj = Octo.OctoVar(var['Name'], var['Value'], var['Scope'])
         scopes = obj.getScope()
         if 'Environment' in scopes:
             env_list = scopes['Environment']
             for env in env_list:
                 if env in map_values['env_map']:
                     env_list.remove(env)
```

### Comparing `pypus-1.4.0/src/pypus/shelf.py` & `pypus-1.4.1/src/pypus/shelf.py`

 * *Files identical despite different names*

