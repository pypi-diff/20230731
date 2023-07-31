# Comparing `tmp/pypus-1.3.0.tar.gz` & `tmp/pypus-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypus-1.3.0.tar", max compression
+gzip compressed data, was "pypus-1.4.0.tar", max compression
```

## Comparing `pypus-1.3.0.tar` & `pypus-1.4.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1073 2021-05-28 19:35:21.744187 pypus-1.3.0/LICENSE
--rw-r--r--   0        0        0      114 2021-05-28 19:36:19.806135 pypus-1.3.0/README.md
--rw-r--r--   0        0        0      569 2023-07-29 16:34:00.874249 pypus-1.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2021-05-11 19:37:09.641525 pypus-1.3.0/src/pypus/__init__.py
--rw-r--r--   0        0        0    24713 2023-07-29 16:33:09.561695 pypus-1.3.0/src/pypus/cli.py
--rw-r--r--   0        0        0      392 2023-07-28 22:05:17.330425 pypus-1.3.0/src/pypus/shelf.py
--rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 pypus-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2021-05-28 19:35:21.744187 pypus-1.4.0/LICENSE
+-rw-r--r--   0        0        0      114 2021-05-28 19:36:19.806135 pypus-1.4.0/README.md
+-rw-r--r--   0        0        0      587 2023-07-31 20:24:50.000783 pypus-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      937 2023-07-31 18:46:58.056574 pypus-1.4.0/src/pypus/Octo.py
+-rw-r--r--   0        0        0        0 2021-05-11 19:37:09.641525 pypus-1.4.0/src/pypus/__init__.py
+-rw-r--r--   0        0        0    30814 2023-07-31 20:16:54.250552 pypus-1.4.0/src/pypus/cli.py
+-rw-r--r--   0        0        0      601 2023-07-31 14:50:20.344572 pypus-1.4.0/src/pypus/shelf.py
+-rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 pypus-1.4.0/PKG-INFO
```

### Comparing `pypus-1.3.0/LICENSE` & `pypus-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypus-1.3.0/pyproject.toml` & `pypus-1.4.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "pypus"
-version = "1.3.0"
+version = "1.4.0"
 description = "Octopus cli toolkit"
 authors = ["Michael MacKenna <mmackenna@unitedfiregroup.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.25.1"
 click = "^8.0.0"
 termcolor = "^1.1.0"
+pyyaml = "^6.0.1"
 
 [tool.poetry.dev-dependencies]
 keyring = "^23.0.1"
 mdv = "^1.7.4"
 pylint = "^2.8.2"
 
 [tool.poetry.scripts]
```

### Comparing `pypus-1.3.0/src/pypus/cli.py` & `pypus-1.4.0/src/pypus/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """ Core module with cli """
 import click
 import json
 import os
 import requests
+import yaml
 from pypus import shelf
+from pypus import Octo
 from termcolor import cprint
 from pprint import pprint
 from requests.api import get, head
 from urllib3.exceptions import InsecureRequestWarning
 # Suppress only the single warning from urllib3 needed.
 requests.packages.urllib3.disable_warnings(category=InsecureRequestWarning)
 # Set `verify=False` on `requests.post`.
@@ -126,14 +128,15 @@
     filename = filename.split('.', 1)[0]
     with open(json_file) as f:
         data = json.load(f)
         shelf.shelf_add_item(filename, 'Variables', data['Variables'])
         shelf.shelf_add_item(filename, 'ScopeValues', data['ScopeValues'])
 
 
+
 @main.command('get-vars', short_help='Get a list of vars for a project in a space')
 @click.argument("space")
 @click.argument("project")
 def get_vars(space, project):
     """ Get a list of vars for a project within a space
 
     Arguments:
@@ -176,20 +179,21 @@
     uri = '{0}/{1}/projects'.format(octopus_server_uri, space['Id'])
     projects = get_octopus_resource(uri, headers)
     project = next((x for x in projects if x['Name'] == project_name), None)
     if project != None:
         uri = '{0}/{1}/variables/{2}'.format(octopus_server_uri, space['Id'], project['VariableSetId'])
         project_variables = get_octopus_resource(uri, headers)
         for var in project_variables['Variables']:
-            print(f"Found a variable with the ID of {var['Id']}, a name of {var['Name']}, and a value of {var['Value']}")
+            print(f"ID: {var['Id']} Name: {var['Name']} Value: {var['Value']} Scope: {var['Scope']}")
         return project_variables
     else:
         return None
 
 
+
 @main.command('set-var', short_help='Set a variable for a project in a space')
 @click.argument("space")
 @click.argument("project")
 @click.argument("variable-name")
 @click.argument("variable-value")
 @click.argument("variable-scope")
 @click.option('--sensitive', is_flag=True)
@@ -588,11 +592,166 @@
                 publish_object = create_publish_object(project_id, runbook_id, info['next_name'])
                 print(f" This is the publish_object {publish_object}")
                 publish_result = post_octopus_resource('{0}/{1}/runbookSnapshots?publish=true'.format(octopus_server_uri, space['Id']), publish_object)
                 print(publish_result)
             else:
                 cprint('No publishing needed', 'green')
 
+
+@main.command('read-yaml', short_help='Read a yaml file')
+@click.argument('yaml-file', type=click.Path(exists=True))
+def import_yaml(yaml_file):
+    with open(yaml_file, "r") as stream:
+        try:
+            print(yaml.safe_load(stream))
+        except yaml.YAMLError as exc:
+            print(exc)
+
+
 @main.command("list-shelf-data", short_help="Print data in a shelf")
 @click.argument("shelf_name")
 def list_shelf_data(shelf_name):
     contents = shelf.shelf_list_contents(shelf_name)
+
+
+@main.command("get-shelf-key", short_help="Print data for a key in a shelf")
+@click.argument("shelf_name")
+@click.argument("key_name")
+def get_shelf_key(shelf_name, key_name):
+    contents = shelf.get_shelf_item(shelf_name, key_name)
+    for var in contents:
+        print(f"{var['Name']} {var['Value']} {var['Scope']}")
+
+
+@main.command('transpose-from-shelf', short_help='Transpose varaibles from shelf')
+@click.argument('shelf-name')
+@click.argument('key-name')
+@click.argument('yaml-map-file', type=click.Path(exists=True))
+@click.argument('new-shelf')
+def transpose_from_shelf(shelf_name, key_name, yaml_map_file, new_shelf):
+    """ Takes variables from a shelf and transposes Scope Values
+    based on a provided map from a yaml file. New values are written
+    to a new shelf file.
+
+    Arguments:
+        shelf-name: The current shelf that holds the variables
+        key-name: The key that holds the variables to transpose
+        yaml-map: The yaml file with the mapped values
+        new-shelf: The new shelf created with the transposed values
+
+    """
+    object_list = []
+    var_dicts = []
+    contents = shelf.get_shelf_item(shelf_name, key_name)
+    with open(yaml_map_file, 'r') as stream:
+        try:
+            map_values = yaml.safe_load(stream)
+        except yaml.YAMLError as e:
+            print(e)
+
+    for var in contents:
+        obj = Octo.OctoVar(var['Name'], var['Value'], var['Scope'])
+        scopes = obj.getScope()
+        if 'Environment' in scopes:
+            env_list = scopes['Environment']
+            for env in env_list:
+                if env in map_values['env_map']:
+                    env_list.remove(env)
+                    env_list.append(map_values['env_map'][env])
+                    print(f"Replaced item {env} with item {map_values['env_map'][env]}")
+            obj.setScopeEnvironment(env_list)
+        object_list.append(obj)
+    for obj in object_list:
+        vdict = obj.getVarAsDict()
+        var_dicts.append(vdict)
+    shelf.shelf_add_item(new_shelf, 'Variables', var_dicts)
+
+
+@main.command('set-vars-from-shelf', short_help='Set project variables from values stored in shelf')
+@click.argument("space")
+@click.argument("project")
+@click.argument("shelf-name")
+def set_vars_from_shelf(space, project, shelf_name):
+    """ Sets project variables from values stored in shelf.
+
+    Arguments:
+        space: The space where the project resides
+        project: The project where the variable is created
+        shelf-name: Name of the shelf where values are stored
+
+        note: Only string variable types are currently supported
+
+        Example: pypus set-var-from-shelf SQLDBA SSIS_BONDDB transposed-vars-for-space1-project1'
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
+    def get_shelf_key(shelf_name, key_name):
+        var_list = []
+        contents = shelf.get_shelf_item(shelf_name, key_name)
+        for var in contents:
+            var_list.append(var)
+        return var_list
+    octopus_api_key = os.getenv('OCTOPUS_API_KEY')
+    octopus_server_uri = os.getenv('OCTOPUS_SERVER_URI')
+    headers = {'X-Octopus-ApiKey': octopus_api_key}
+    project_name = project
+    space_name = space
+    var_list = get_shelf_key(shelf_name, 'Variables')
+    uri = '{0}/spaces'.format(octopus_server_uri)
+    spaces = get_octopus_resource(uri, headers)
+    space = next((x for x in spaces if x['Name'] == space_name), None)
+    uri = '{0}/{1}/projects'.format(octopus_server_uri, space['Id'])
+    projects = get_octopus_resource(uri, headers)
+    project = next((x for x in projects if x['Name'] == project_name), None)
+    if project != None:
+        uri = '{0}/{1}/variables/{2}'.format(octopus_server_uri, space['Id'], project['VariableSetId'])
+        project_variables = get_octopus_resource(uri, headers)
+    else:
+        print(f"Project {project_name} was not found")
+        sys.exit(1)
+    for var in var_list:
+        variable_name = var['Name']
+        variable_scope = var['Scope']
+        variable_value = var['Value']
+        sensitive = False
+        variable = {
+                'Name': variable_name,
+                'Value': variable_value,
+                'Type': 'String',
+                'Scope': variable_scope,
+                'IsSensitive': sensitive
+        }
+        project_variable = next((x for x in project_variables['Variables'] if (x['Name'] == variable['Name']) and
+            (x['Scope'] == variable['Scope'])), None)
+
+        if project_variable == None:
+            project_variables['Variables'].append(variable)
+        else:
+            project_variable['Value'] = variable['Value']
+            project_variable['Type'] = variable['Type']
+            project_variable['Scope'] = variable['Scope']
+            project_variable['IsSensitive'] = variable['IsSensitive']
+    response = requests.put(uri, headers=headers, json=project_variables, verify=False)
+    response.raise_for_status
+    print(response)
```

### Comparing `pypus-1.3.0/PKG-INFO` & `pypus-1.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pypus
-Version: 1.3.0
+Version: 1.4.0
 Summary: Octopus cli toolkit
 License: MIT
 Author: Michael MacKenna
 Author-email: mmackenna@unitedfiregroup.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.0.0,<9.0.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Requires-Dist: termcolor (>=1.1.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Pypus
 
 Pypus is a cli tool for publishing Octopus Deploy Runbooks.
```

