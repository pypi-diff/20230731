# Comparing `tmp/offat-0.3.0.tar.gz` & `tmp/offat-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "offat-0.3.0.tar", max compression
+gzip compressed data, was "offat-0.4.0.tar", max compression
```

## Comparing `offat-0.3.0.tar` & `offat-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-07-15 11:22:03.008874 offat-0.3.0/LICENSE
--rw-r--r--   0        0        0     5632 2023-07-15 11:22:03.008874 offat-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-07-15 11:22:03.008874 offat-0.3.0/offat/__init__.py
--rw-r--r--   0        0        0      662 2023-07-15 11:22:03.008874 offat-0.3.0/offat/__main__.py
--rw-r--r--   0        0        0     4327 2023-07-15 11:22:03.008874 offat-0.3.0/offat/http.py
--rw-r--r--   0        0        0     1122 2023-07-15 11:22:03.008874 offat-0.3.0/offat/logger.py
--rw-r--r--   0        0        0     3767 2023-07-15 11:22:03.008874 offat-0.3.0/offat/openapi.py
--rw-r--r--   0        0        0        0 2023-07-15 11:22:03.008874 offat-0.3.0/offat/tester/__init__.py
--rw-r--r--   0        0        0     3158 2023-07-15 11:22:03.008874 offat-0.3.0/offat/tester/fuzzer.py
--rw-r--r--   0        0        0    11990 2023-07-15 11:22:03.008874 offat-0.3.0/offat/tester/test_generator.py
--rw-r--r--   0        0        0     1274 2023-07-15 11:22:03.008874 offat-0.3.0/offat/tester/test_results.py
--rw-r--r--   0        0        0     3903 2023-07-15 11:22:03.008874 offat-0.3.0/offat/tester/test_runner.py
--rw-r--r--   0        0        0     1403 2023-07-15 11:22:03.008874 offat-0.3.0/offat/tester/tester_utils.py
--rw-r--r--   0        0        0     2021 2023-07-15 11:22:03.008874 offat-0.3.0/offat/utils.py
--rw-r--r--   0        0        0      873 2023-07-15 11:22:03.008874 offat-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6600 1970-01-01 00:00:00.000000 offat-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-31 18:36:18.784892 offat-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5781 2023-07-31 18:36:18.784892 offat-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-31 18:36:18.784892 offat-0.4.0/offat/__init__.py
+-rw-r--r--   0        0        0     1027 2023-07-31 18:36:18.788892 offat-0.4.0/offat/__main__.py
+-rw-r--r--   0        0        0     4327 2023-07-31 18:36:18.788892 offat-0.4.0/offat/http.py
+-rw-r--r--   0        0        0     1122 2023-07-31 18:36:18.788892 offat-0.4.0/offat/logger.py
+-rw-r--r--   0        0        0     3767 2023-07-31 18:36:18.788892 offat-0.4.0/offat/openapi.py
+-rw-r--r--   0        0        0        0 2023-07-31 18:36:18.788892 offat-0.4.0/offat/tester/__init__.py
+-rw-r--r--   0        0        0     1567 2023-07-31 18:36:18.788892 offat-0.4.0/offat/tester/data_exposure.py
+-rw-r--r--   0        0        0     3158 2023-07-31 18:36:18.788892 offat-0.4.0/offat/tester/fuzzer.py
+-rw-r--r--   0        0        0     1617 2023-07-31 18:36:18.788892 offat-0.4.0/offat/tester/regexs.py
+-rw-r--r--   0        0        0    12039 2023-07-31 18:36:18.788892 offat-0.4.0/offat/tester/test_generator.py
+-rw-r--r--   0        0        0     1537 2023-07-31 18:36:18.788892 offat-0.4.0/offat/tester/test_results.py
+-rw-r--r--   0        0        0     4720 2023-07-31 18:36:18.788892 offat-0.4.0/offat/tester/test_runner.py
+-rw-r--r--   0        0        0     2175 2023-07-31 18:36:18.788892 offat-0.4.0/offat/tester/tester_utils.py
+-rw-r--r--   0        0        0     3051 2023-07-31 18:36:18.788892 offat-0.4.0/offat/utils.py
+-rw-r--r--   0        0        0      873 2023-07-31 18:36:18.788892 offat-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6749 1970-01-01 00:00:00.000000 offat-0.4.0/PKG-INFO
```

### Comparing `offat-0.3.0/LICENSE` & `offat-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `offat-0.3.0/README.md` & `offat-0.4.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ![UnDocumented petstore API endpoint HTTP method results](./.images/tests/offat-test-undocumented-api-endpoint-http-method.png)
 
 ## Features
 
 - [X] Restricted HTTP Methods
 - [X] SQLi
 - [X] BOLA (Might need few bug fixes)
+- [X] Data Exposure (Detects Common Data Exposures)
 - [ ] Broken Authentication
 - [ ] Mass Assignment
-- [ ] Data Exposure
 
 ## Demo
 
 [![asciicast](https://asciinema.org/a/9MSwl7UafIVT3iJn13OcvWXeF.svg)](https://asciinema.org/a/9MSwl7UafIVT3iJn13OcvWXeF)
 
 ## PyPi Downloads
 
@@ -82,24 +82,30 @@
   ```bash
   # without options
   poetry install
   ```
 
 ## Start OffAT
 
-- run offat
+- Run offat
 
   ```bash
-  python3 -m offat
+  offat -f swagger_file.json
   ```
 
-- to get all the commands use `help`
+- To get all the commands use `help`
 
   ```bash
-  python3 -m offat -h
+  offat -h
+  ```
+
+- Run tests only for endpoint paths matching regex pattern
+
+  ```bash
+  offat -f swagger_file.json -pr '/user'
   ```
 
 > If you're using Termux or windows, then use `pip` instead of `pip3`.  
 > Few features are only for linux os, hence they might not work on windows and require admin priviliges.
 
 ### Open In Google Cloud Shell
```

### Comparing `offat-0.3.0/offat/__main__.py` & `offat-0.4.0/offat/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 
 
 def start():
     '''Starts cli tool'''
     parser = ArgumentParser(prog='offat')
     parser.add_argument('-f','--file', dest='fpath', type=str, help='path of openapi/swagger specification file', required=True)
     parser.add_argument('-v','--version', action='version', version=f'%(prog)s {get_package_version()}')
+    parser.add_argument('-pr','--path-regex', dest='path_regex_pattern', type=str, help='run tests for paths matching given regex pattern', required=False, default=None)
+    parser.add_argument('-o', '--output', dest='output_file', type=str, help='path to store test results in json format', required=False, default=None)
     args = parser.parse_args()
 
     # parse and run tests
     api_parser = OpenAPIParser(args.fpath)
-    generate_and_run_tests(api_parser)
+    generate_and_run_tests(api_parser, args.path_regex_pattern, args.output_file)
 
 if __name__ == '__main__':
     start()
```

### Comparing `offat-0.3.0/offat/http.py` & `offat-0.4.0/offat/http.py`

 * *Files identical despite different names*

### Comparing `offat-0.3.0/offat/logger.py` & `offat-0.4.0/offat/logger.py`

 * *Files identical despite different names*

### Comparing `offat-0.3.0/offat/openapi.py` & `offat-0.4.0/offat/openapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         paths = self._spec.get('paths',{})
 
         # extract endpoints and supported params
         for path in paths.keys():
             path_params = paths[path].get('parameters',[])
 
             for http_method in paths.get(path,{}).keys():
-                # confider only http methods
+                # consider only http methods
                 if http_method not in ['get', 'put', 'post', 'delete', 'options']:
                     continue
                 
 
                 body_parameters = paths[path][http_method].get('parameters',[])
                 response_params = self._get_response_definition_schema(paths[path][http_method].get('responses',{}))
```

### Comparing `offat-0.3.0/offat/tester/fuzzer.py` & `offat-0.4.0/offat/tester/fuzzer.py`

 * *Files identical despite different names*

### Comparing `offat-0.3.0/offat/tester/test_generator.py` & `offat-0.4.0/offat/tester/test_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from copy import deepcopy
-from random import randint
+from .fuzzer import fill_params
 from .test_runner import TestRunnerFiltersEnum
 from ..openapi import OpenAPIParser
-from .fuzzer import fill_params
 
 
 class TestGenerator:
     """
     Class to generate API test checks.
 
     This class provides methods to generate API test checks for various scenarios.
@@ -82,15 +81,15 @@
                     'kwargs': kwargs,
                     'result_details':{
                         True: 'Endpoint does not perform any HTTP method which is not documented', # passed
                         False: 'Endpoint performs HTTP method which is not documented', # failed
                     },
                     'body_params':[],
                     'success_codes':success_codes,
-                    'response_filter': TestRunnerFiltersEnum.STATUS_CODE_FILTER
+                    'response_filter': TestRunnerFiltersEnum.STATUS_CODE_FILTER.name
                 })
 
         return tasks
     
 
     def __get_request_params_list(self, request_params:list[dict]):
         '''Get list of request parameters
@@ -207,15 +206,15 @@
                     'args': args,
                     'kwargs': kwargs,
                     'result_details':{
                         True:'Parameters are not vulnerable to SQLi Payload', # passed
                         False:'One or more parameter is vulnerable to SQL Injection Attack', # failed
                     },
                     'success_codes':success_codes,
-                    'response_filter': TestRunnerFiltersEnum.STATUS_CODE_FILTER
+                    'response_filter': TestRunnerFiltersEnum.STATUS_CODE_FILTER.name
                 })
 
         return tasks
     
 
     def bola_path_test(
             self,
@@ -229,15 +228,15 @@
         Args:
             openapi_parser (OpenAPIParser): An instance of the OpenAPIParser class containing the parsed OpenAPI specification.
             success_codes (list[int], optional): A list of HTTP success codes to consider as successful BOLA responses. Defaults to [200, 201, 301].
             *args: Variable-length positional arguments.
             **kwargs: Arbitrary keyword arguments.
         
         Returns:
-            None
+            list[dict]: list of dict containing test case for endpoint
         
         Raises:
             Any exceptions raised during the execution.
         '''
         base_url:str = openapi_parser.base_url
         request_response_params:list[dict] = openapi_parser.request_response_params
 
@@ -288,11 +287,13 @@
                 'args': args,
                 'kwargs': kwargs,
                 'result_details':{
                     True:'Endpoint is not vulnerable to BOLA', # passed
                     False:'Endpoint might be vulnerable to BOLA', # failed
                 },
                 'success_codes':success_codes,
-                'response_filter': TestRunnerFiltersEnum.STATUS_CODE_FILTER
+                'response_filter': TestRunnerFiltersEnum.STATUS_CODE_FILTER.name
             })
 
-        return tasks
+        return tasks
+    
+
```

### Comparing `offat-0.3.0/offat/tester/test_results.py` & `offat-0.4.0/offat/tester/test_results.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,25 +6,32 @@
         self.headers = headers
         self.args = args
         self.kwargs = kwargs
 
     def generate_result_table(self, results:list, filter_passed_results:bool=True):
         return tabulate(self._sanitize_results(results, filter_passed_results), headers=self.headers, tablefmt=self.tablefmt, *self.args, **self.kwargs)
     
-    def _sanitize_results(self, results:list, filter_passed_results:bool=True):
+    def _sanitize_results(self, results:list, filter_passed_results:bool=True, is_leaking_data:bool=False):
         if filter_passed_results:
-            results = list(filter(lambda x: not x.get('result'), results))
+            results = list(filter(lambda x: not x.get('result') or x.get('data_leak'), results))
 
         # remove args, kwargs and other unrequired keys for results
         for result in results:
             if result['result']:
                 result['result'] = u"\u2713"
             else:
                 result['result'] = u"\u00d7"
 
+            if not is_leaking_data:
+                del result['response_headers']
+                del result['response_body']
+
+            if not result.get('data_leak'):
+                del result['data_leak']
+
             del result['url']
             del result['args']
             del result['kwargs']
             del result['test_name']
             del result['response_filter']
             del result['success_codes']
             del result['body_params']
```

### Comparing `offat-0.3.0/offat/utils.py` & `offat-0.4.0/offat/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,15 @@
-from json import loads as json_load, JSONDecodeError
-from os.path import isfile
-from yaml import safe_load, YAMLError
+from json import loads as json_load, dumps as json_dumps, JSONDecodeError
 from pkg_resources import get_distribution
+from yaml import safe_load, YAMLError
+from os.path import isfile
+from .logger import create_logger
+
+
+logger = create_logger(__name__)
 
 
 def get_package_version():
     '''Returns package current version
     
     Args:
         None
@@ -73,7 +77,40 @@
     match file_ext:
         case 'json':
             return read_json(file_path)
         case 'yaml':
             return read_yaml(file_path)
         case _:
             return {"error":"Invalid file extension"}
+
+
+def write_json_to_file(json_data:dict, file_path:str):
+    '''Writes dict obj to file as json
+
+    Args:
+        json_data (dict): JSON payload to be written into file
+        file_path (str): path of output json file
+
+    Returns:
+        bool: True is `json_data` is written into `file_path` else
+        returns False (in case of any exception) 
+
+    Raises:
+        Any exception occurred during operation
+    '''
+    if isfile(file_path):
+       logger.info(f'{file_path} file will be overwritten.')
+
+    logger.info(f'Writing data to file: {file_path}')
+    try:
+        with open(file_path, 'w') as f:
+            f.write(json_dumps(json_data))
+            logger.info(f'Completed writing data to file: {file_path}')
+            return True
+
+    except JSONDecodeError:
+        logger.error(f'Invalid JSON data, error while writing to {file_path} file.')
+
+    except Exception as e:
+        logger.error(repr(e))
+
+    return False
```

### Comparing `offat-0.3.0/pyproject.toml` & `offat-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "offat"
-version = "0.3.0"
+version = "0.4.0"
 description = "Offensive API tester tool automates checks for common API vulnerabilities"
 authors = ["Dhrumil Mistry <56185972+dmdhrumilmistry@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `offat-0.3.0/PKG-INFO` & `offat-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: offat
-Version: 0.3.0
+Version: 0.4.0
 Summary: Offensive API tester tool automates checks for common API vulnerabilities
 License: MIT
 Author: Dhrumil Mistry
 Author-email: 56185972+dmdhrumilmistry@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -28,17 +28,17 @@
 ![UnDocumented petstore API endpoint HTTP method results](./.images/tests/offat-test-undocumented-api-endpoint-http-method.png)
 
 ## Features
 
 - [X] Restricted HTTP Methods
 - [X] SQLi
 - [X] BOLA (Might need few bug fixes)
+- [X] Data Exposure (Detects Common Data Exposures)
 - [ ] Broken Authentication
 - [ ] Mass Assignment
-- [ ] Data Exposure
 
 ## Demo
 
 [![asciicast](https://asciinema.org/a/9MSwl7UafIVT3iJn13OcvWXeF.svg)](https://asciinema.org/a/9MSwl7UafIVT3iJn13OcvWXeF)
 
 ## PyPi Downloads
 
@@ -105,24 +105,30 @@
   ```bash
   # without options
   poetry install
   ```
 
 ## Start OffAT
 
-- run offat
+- Run offat
 
   ```bash
-  python3 -m offat
+  offat -f swagger_file.json
   ```
 
-- to get all the commands use `help`
+- To get all the commands use `help`
 
   ```bash
-  python3 -m offat -h
+  offat -h
+  ```
+
+- Run tests only for endpoint paths matching regex pattern
+
+  ```bash
+  offat -f swagger_file.json -pr '/user'
   ```
 
 > If you're using Termux or windows, then use `pip` instead of `pip3`.  
 > Few features are only for linux os, hence they might not work on windows and require admin priviliges.
 
 ### Open In Google Cloud Shell
```

