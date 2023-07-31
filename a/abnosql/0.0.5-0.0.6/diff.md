# Comparing `tmp/abnosql-0.0.5.tar.gz` & `tmp/abnosql-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abnosql-0.0.5.tar", last modified: Thu Jul 20 17:24:57 2023, max compression
+gzip compressed data, was "abnosql-0.0.6.tar", last modified: Mon Jul 31 17:37:48 2023, max compression
```

## Comparing `abnosql-0.0.5.tar` & `abnosql-0.0.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:24:57.727913 abnosql-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-20 17:24:39.000000 abnosql-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16918 2023-07-20 17:24:57.727913 abnosql-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15790 2023-07-20 17:24:39.000000 abnosql-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:24:57.727913 abnosql-0.0.5/abnosql/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4095 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/kms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:24:57.727913 abnosql-0.0.5/abnosql/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/mocks/mock_azure_kms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/mocks/mock_cosmos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/mocks/mock_dynamodbx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:24:57.727913 abnosql-0.0.5/abnosql/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:24:57.727913 abnosql-0.0.5/abnosql/plugins/kms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/plugins/kms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/plugins/kms/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/plugins/kms/azure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:24:57.727913 abnosql-0.0.5/abnosql/plugins/table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/plugins/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/plugins/table/cosmos.py
--rw-r--r--   0 runner    (1001) docker     (123)     9793 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/plugins/table/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/plugins/table/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    15395 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/table.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:24:57.727913 abnosql-0.0.5/abnosql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16918 2023-07-20 17:24:57.000000 abnosql-0.0.5/abnosql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-20 17:24:57.000000 abnosql-0.0.5/abnosql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 17:24:57.000000 abnosql-0.0.5/abnosql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-20 17:24:57.000000 abnosql-0.0.5/abnosql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-20 17:24:57.000000 abnosql-0.0.5/abnosql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 17:24:57.000000 abnosql-0.0.5/abnosql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-20 17:24:57.727913 abnosql-0.0.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2818 2023-07-20 17:24:39.000000 abnosql-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:37:48.860376 abnosql-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-31 17:37:28.000000 abnosql-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16918 2023-07-31 17:37:48.860376 abnosql-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15790 2023-07-31 17:37:28.000000 abnosql-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:37:48.856377 abnosql-0.0.6/abnosql/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4128 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/kms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:37:48.856377 abnosql-0.0.6/abnosql/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/mocks/mock_azure_kms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/mocks/mock_cosmos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/mocks/mock_dynamodbx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:37:48.856377 abnosql-0.0.6/abnosql/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:37:48.860376 abnosql-0.0.6/abnosql/plugins/kms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/plugins/kms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/plugins/kms/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/plugins/kms/azure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:37:48.860376 abnosql-0.0.6/abnosql/plugins/table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/plugins/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/plugins/table/cosmos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/plugins/table/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/plugins/table/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15395 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-31 17:37:28.000000 abnosql-0.0.6/abnosql/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:37:48.856377 abnosql-0.0.6/abnosql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16918 2023-07-31 17:37:48.000000 abnosql-0.0.6/abnosql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-31 17:37:48.000000 abnosql-0.0.6/abnosql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 17:37:48.000000 abnosql-0.0.6/abnosql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-31 17:37:48.000000 abnosql-0.0.6/abnosql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-31 17:37:48.000000 abnosql-0.0.6/abnosql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-31 17:37:48.000000 abnosql-0.0.6/abnosql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-31 17:37:48.860376 abnosql-0.0.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2818 2023-07-31 17:37:28.000000 abnosql-0.0.6/setup.py
```

### Comparing `abnosql-0.0.5/LICENSE` & `abnosql-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.5/PKG-INFO` & `abnosql-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abnosql
-Version: 0.0.5
+Version: 0.0.6
 Summary: NoSQL Abstraction Library
 Home-page: https://github.com/rog555/abnosql
 Download-URL: http://pypi.python.org/pypi/abnosql
 Author: Roger Foskett
 Author-email: r_foskett@hotmail.com
 Maintainer: Roger Foskett
 Maintainer-email: r_foskett@hotmail.com
```

### Comparing `abnosql-0.0.5/README.md` & `abnosql-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.5/abnosql/cli.py` & `abnosql-0.0.6/abnosql/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -114,23 +114,23 @@
     tb = _table(table, get_config(config), database=database)
     tb.delete_item(**get_key(partition_key, id_key))
     print('deleted')
 
 
 @click.command()
 @click.argument('table')
-@click.argument('partition-key')
+@click.option('--partition-key', '-p')
 @click.option('--id-key', '-k')
 @click.option('--filters', '-f')
 @click.option('--database', '-d')
 @click.option('--config', '-c')
 def query(table, partition_key, id_key, filters, database, config):
     tb = _table(table, get_config(config), database=database)
     dump(tb.query(
-        key=get_key(partition_key, id_key),
+        key=get_key(partition_key, id_key) if partition_key else None,
         filters=parse_dict_arg(filters)
     )['items'])
 
 
 @click.command()
 @click.argument('table')
 @click.argument('statement')
```

### Comparing `abnosql-0.0.5/abnosql/kms.py` & `abnosql-0.0.6/abnosql/kms.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.5/abnosql/mocks/mock_azure_kms.py` & `abnosql-0.0.6/abnosql/mocks/mock_azure_kms.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.5/abnosql/mocks/mock_cosmos.py` & `abnosql-0.0.6/abnosql/mocks/mock_cosmos.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.5/abnosql/mocks/mock_dynamodbx.py` & `abnosql-0.0.6/abnosql/mocks/mock_dynamodbx.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.5/abnosql/plugin.py` & `abnosql-0.0.6/abnosql/plugin.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.5/abnosql/plugins/kms/aws.py` & `abnosql-0.0.6/abnosql/plugins/kms/aws.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.5/abnosql/plugins/kms/azure.py` & `abnosql-0.0.6/abnosql/plugins/kms/azure.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.5/abnosql/plugins/table/cosmos.py` & `abnosql-0.0.6/abnosql/plugins/table/cosmos.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import functools
+import logging
 import os
+
 import typing as t
 
 import pluggy  # type: ignore
 
 import abnosql.exceptions as ex
 from abnosql.plugin import PM
 from abnosql.table import add_audit
@@ -199,22 +201,24 @@
         filters = filters or {}
         key = key or {}
         validate_query_attrs(key, filters)
         parameters = {
             f'@{k}': v
             for k, v in filters.items()
         }
+        # cosmos doesnt like hyphens in table names
+        table_alias = 'c' if '-' in self.name else self.name
         parameters.update({
             f'@{k}': v
             for k, v in key.items()
         })
-        statement = f'SELECT * FROM {self.name}'
+        statement = f'SELECT * FROM {table_alias}'
         op = 'WHERE'
         for param in parameters.keys():
-            statement += f' {op} {self.name}.{param[1:]} = {param}'
+            statement += f' {op} {table_alias}.{param[1:]} = {param}'
             op = 'AND'
 
         resp = self.query_sql(
             statement,
             parameters,
             limit=limit,
             next=next
@@ -254,14 +258,15 @@
         # for cross-partition queries - see limitations https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos  # noqa
         # so add OFFSET and LIMIT if not already present
         if (
             ' OFFSET ' not in statement.upper()
             and ' LIMIT ' not in statement.upper()
         ):
             kwargs['query'] += f' OFFSET {next} LIMIT {limit}'
+        logging.debug(f'query_sql() table: {self.name}, kwargs: {kwargs}')
         container = self._container(self.name)
         items = list(container.query_items(**kwargs))
         headers = container.client_connection.last_response_headers
         # continuation = headers.get('x-ms-continuation')
         # total size in 'x-ms-resource-usage' eg ;documentsCount=3
         resource_usage = {
             _.split('=', 1)[0]: _.split('=', 1)[1]
```

### Comparing `abnosql-0.0.5/abnosql/plugins/table/dynamodb.py` & `abnosql-0.0.6/abnosql/plugins/table/dynamodb.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from base64 import b64decode
 from base64 import b64encode
 from datetime import datetime
 import functools
 import json
+import logging
 import os
 import typing as t
 
 import pluggy  # type: ignore
 
 import abnosql.exceptions as ex
 from abnosql.plugin import PM
@@ -251,16 +252,18 @@
         )
         if next is not None:
             kwargs['ExclusiveStartKey'] = json.loads(b64decode(next).decode())
         if limit is not None:
             kwargs['Limit'] = limit
         response = None
         if key is not None:
+            logging.debug(f'query() table: {self.name}, query kwargs: {kwargs}')
             response = self.table.query(**kwargs)
         else:
+            logging.debug(f'query() table: {self.name}, scan kwargs: {kwargs}')
             response = self.table.scan(**kwargs)
         items = response.get('Items', [])
         items = kms_process_query_items(self.config, items)
         last = response.get('LastEvaluatedKey')
         if last is not None:
             last = b64encode(json.dumps(last).encode()).decode()
         return {
@@ -287,14 +290,15 @@
         if next is not None:
             kwargs['NextToken'] = next
         if limit is not None:
             kwargs['Limit'] = limit
         if len(params):
             kwargs['Parameters'] = params
 
+        logging.debug(f'query_sql() table: {self.name}, kwargs: {kwargs}')
         response = client.execute_statement(**kwargs)
         items = []
         _items = response.get('Items', [])
         _items = kms_process_query_items(self.config, _items)
         for item in _items:
             items.append(json_util.loads(json.dumps(item)))
```

### Comparing `abnosql-0.0.5/abnosql/plugins/table/memory.py` & `abnosql-0.0.6/abnosql/plugins/table/memory.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.5/abnosql/table.py` & `abnosql-0.0.6/abnosql/table.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.5/abnosql.egg-info/PKG-INFO` & `abnosql-0.0.6/abnosql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abnosql
-Version: 0.0.5
+Version: 0.0.6
 Summary: NoSQL Abstraction Library
 Home-page: https://github.com/rog555/abnosql
 Download-URL: http://pypi.python.org/pypi/abnosql
 Author: Roger Foskett
 Author-email: r_foskett@hotmail.com
 Maintainer: Roger Foskett
 Maintainer-email: r_foskett@hotmail.com
```

### Comparing `abnosql-0.0.5/abnosql.egg-info/SOURCES.txt` & `abnosql-0.0.6/abnosql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.5/abnosql.egg-info/requires.txt` & `abnosql-0.0.6/abnosql.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.5/setup.py` & `abnosql-0.0.6/setup.py`

 * *Files identical despite different names*

