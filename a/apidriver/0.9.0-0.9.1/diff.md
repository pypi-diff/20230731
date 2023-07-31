# Comparing `tmp/apidriver-0.9.0.tar.gz` & `tmp/apidriver-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apidriver-0.9.0.tar", last modified: Mon Jul 24 07:11:21 2023, max compression
+gzip compressed data, was "apidriver-0.9.1.tar", last modified: Mon Jul 31 14:18:42 2023, max compression
```

## Comparing `apidriver-0.9.0.tar` & `apidriver-0.9.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 chnjx      (501) staff       (20)        0 2023-07-24 07:11:21.031938 apidriver-0.9.0/
--rw-r--r--   0 chnjx      (501) staff       (20)     1068 2023-02-07 12:22:16.000000 apidriver-0.9.0/LICENSE.txt
--rw-r--r--   0 chnjx      (501) staff       (20)       84 2023-03-15 15:32:00.000000 apidriver-0.9.0/MANIFEST.in
--rw-r--r--   0 chnjx      (501) staff       (20)      209 2023-07-24 07:11:21.030928 apidriver-0.9.0/PKG-INFO
--rw-r--r--   0 chnjx      (501) staff       (20)     3340 2023-04-13 12:44:49.000000 apidriver-0.9.0/README.md
-drwxr-xr-x   0 chnjx      (501) staff       (20)        0 2023-07-24 07:11:21.001855 apidriver-0.9.0/api_driver/
--rw-r--r--   0 chnjx      (501) staff       (20)       64 2023-03-14 14:16:04.000000 apidriver-0.9.0/api_driver/__init__.py
--rw-r--r--   0 chnjx      (501) staff       (20)      120 2023-03-15 15:01:02.000000 apidriver-0.9.0/api_driver/__main__.py
--rw-r--r--   0 chnjx      (501) staff       (20)      127 2023-07-24 07:06:07.000000 apidriver-0.9.0/api_driver/_version.py
--rw-r--r--   0 chnjx      (501) staff       (20)     2712 2023-07-04 01:36:23.000000 apidriver-0.9.0/api_driver/ad_utils.py
--rw-r--r--   0 chnjx      (501) staff       (20)     3483 2023-07-24 07:00:48.000000 apidriver-0.9.0/api_driver/api_driver.py
--rw-r--r--   0 chnjx      (501) staff       (20)     2971 2023-03-15 15:08:27.000000 apidriver-0.9.0/api_driver/command.py
--rw-r--r--   0 chnjx      (501) staff       (20)    14714 2023-04-13 12:44:49.000000 apidriver-0.9.0/api_driver/har_parser.py
--rw-r--r--   0 chnjx      (501) staff       (20)     2278 2023-04-13 12:44:49.000000 apidriver-0.9.0/api_driver/loader_swagger.py
--rw-r--r--   0 chnjx      (501) staff       (20)     4417 2023-04-13 12:44:49.000000 apidriver-0.9.0/api_driver/project_generator.py
--rw-r--r--   0 chnjx      (501) staff       (20)     8018 2023-04-13 12:44:49.000000 apidriver-0.9.0/api_driver/swagger_generate.py
--rw-r--r--   0 chnjx      (501) staff       (20)      485 2023-04-13 12:44:49.000000 apidriver-0.9.0/api_driver/template.py
-drwxr-xr-x   0 chnjx      (501) staff       (20)        0 2023-07-24 07:11:21.013247 apidriver-0.9.0/api_driver/templates/
--rw-r--r--   0 chnjx      (501) staff       (20)     2121 2023-04-13 12:44:49.000000 apidriver-0.9.0/api_driver/templates/api.tpl
--rw-r--r--   0 chnjx      (501) staff       (20)      374 2023-03-15 15:46:44.000000 apidriver-0.9.0/api_driver/templates/api_demo.tpl
--rw-r--r--   0 chnjx      (501) staff       (20)      398 2023-03-15 15:08:27.000000 apidriver-0.9.0/api_driver/templates/base_testcase.tpl
--rw-r--r--   0 chnjx      (501) staff       (20)     2879 2023-03-15 15:12:01.000000 apidriver-0.9.0/api_driver/templates/har2api_case.tpl
--rw-r--r--   0 chnjx      (501) staff       (20)     2242 2023-03-15 15:12:01.000000 apidriver-0.9.0/api_driver/templates/har2case.tpl
--rw-r--r--   0 chnjx      (501) staff       (20)     5224 2023-04-13 12:44:49.000000 apidriver-0.9.0/api_driver/templates/http.tpl
--rw-r--r--   0 chnjx      (501) staff       (20)    15328 2023-07-24 07:03:03.000000 apidriver-0.9.0/api_driver/templates/report_template.html
--rw-r--r--   0 chnjx      (501) staff       (20)      355 2023-03-15 13:14:27.000000 apidriver-0.9.0/api_driver/templates/testcase_demo.tpl
--rw-r--r--   0 chnjx      (501) staff       (20)     2933 2023-04-13 12:44:49.000000 apidriver-0.9.0/api_driver/testcase_mixin.py
-drwxr-xr-x   0 chnjx      (501) staff       (20)        0 2023-07-24 07:11:21.019937 apidriver-0.9.0/api_driver/utils/
--rw-r--r--   0 chnjx      (501) staff       (20)        0 2023-02-07 12:22:16.000000 apidriver-0.9.0/api_driver/utils/__init__.py
--rw-r--r--   0 chnjx      (501) staff       (20)     1043 2023-03-15 15:08:27.000000 apidriver-0.9.0/api_driver/utils/custom_str_utils.py
--rw-r--r--   0 chnjx      (501) staff       (20)     1882 2023-03-14 13:52:12.000000 apidriver-0.9.0/api_driver/utils/database_conn.py
--rw-r--r--   0 chnjx      (501) staff       (20)     3322 2023-03-14 13:52:12.000000 apidriver-0.9.0/api_driver/utils/fake.py
--rw-r--r--   0 chnjx      (501) staff       (20)     2172 2023-03-15 15:08:27.000000 apidriver-0.9.0/api_driver/utils/placeholder.py
--rw-r--r--   0 chnjx      (501) staff       (20)     1283 2023-02-17 12:48:23.000000 apidriver-0.9.0/api_driver/utils/service_logger.py
-drwxr-xr-x   0 chnjx      (501) staff       (20)        0 2023-07-24 07:11:21.027824 apidriver-0.9.0/apidriver.egg-info/
--rw-r--r--   0 chnjx      (501) staff       (20)      209 2023-07-24 07:11:20.000000 apidriver-0.9.0/apidriver.egg-info/PKG-INFO
--rw-r--r--   0 chnjx      (501) staff       (20)     1061 2023-07-24 07:11:20.000000 apidriver-0.9.0/apidriver.egg-info/SOURCES.txt
--rw-r--r--   0 chnjx      (501) staff       (20)        1 2023-07-24 07:11:20.000000 apidriver-0.9.0/apidriver.egg-info/dependency_links.txt
--rw-r--r--   0 chnjx      (501) staff       (20)       39 2023-07-24 07:11:20.000000 apidriver-0.9.0/apidriver.egg-info/entry_points.txt
--rw-r--r--   0 chnjx      (501) staff       (20)      171 2023-07-24 07:11:20.000000 apidriver-0.9.0/apidriver.egg-info/requires.txt
--rw-r--r--   0 chnjx      (501) staff       (20)       11 2023-07-24 07:11:20.000000 apidriver-0.9.0/apidriver.egg-info/top_level.txt
--rw-r--r--   0 chnjx      (501) staff       (20)      170 2023-04-13 12:44:49.000000 apidriver-0.9.0/requirements.txt
--rw-r--r--   0 chnjx      (501) staff       (20)       38 2023-07-24 07:11:21.032253 apidriver-0.9.0/setup.cfg
--rw-r--r--   0 chnjx      (501) staff       (20)      903 2023-04-13 12:44:49.000000 apidriver-0.9.0/setup.py
-drwxr-xr-x   0 chnjx      (501) staff       (20)        0 2023-07-24 07:11:21.029474 apidriver-0.9.0/test/
--rw-r--r--   0 chnjx      (501) staff       (20)     1105 2023-04-13 12:44:49.000000 apidriver-0.9.0/test/test_cli.py
+drwxr-xr-x   0 chnjx      (501) staff       (20)        0 2023-07-31 14:18:42.025158 apidriver-0.9.1/
+-rw-r--r--   0 chnjx      (501) staff       (20)     1068 2023-02-07 12:22:16.000000 apidriver-0.9.1/LICENSE.txt
+-rw-r--r--   0 chnjx      (501) staff       (20)       84 2023-03-15 15:32:00.000000 apidriver-0.9.1/MANIFEST.in
+-rw-r--r--   0 chnjx      (501) staff       (20)      209 2023-07-31 14:18:42.024726 apidriver-0.9.1/PKG-INFO
+-rw-r--r--   0 chnjx      (501) staff       (20)     3340 2023-04-13 12:44:49.000000 apidriver-0.9.1/README.md
+drwxr-xr-x   0 chnjx      (501) staff       (20)        0 2023-07-31 14:18:42.008100 apidriver-0.9.1/api_driver/
+-rw-r--r--   0 chnjx      (501) staff       (20)       64 2023-03-14 14:16:04.000000 apidriver-0.9.1/api_driver/__init__.py
+-rw-r--r--   0 chnjx      (501) staff       (20)      120 2023-03-15 15:01:02.000000 apidriver-0.9.1/api_driver/__main__.py
+-rw-r--r--   0 chnjx      (501) staff       (20)      127 2023-07-31 14:17:48.000000 apidriver-0.9.1/api_driver/_version.py
+-rw-r--r--   0 chnjx      (501) staff       (20)     2712 2023-07-04 01:36:23.000000 apidriver-0.9.1/api_driver/ad_utils.py
+-rw-r--r--   0 chnjx      (501) staff       (20)     3857 2023-07-30 03:50:13.000000 apidriver-0.9.1/api_driver/api_driver.py
+-rw-r--r--   0 chnjx      (501) staff       (20)     2971 2023-03-15 15:08:27.000000 apidriver-0.9.1/api_driver/command.py
+-rw-r--r--   0 chnjx      (501) staff       (20)    14714 2023-04-13 12:44:49.000000 apidriver-0.9.1/api_driver/har_parser.py
+-rw-r--r--   0 chnjx      (501) staff       (20)     2278 2023-04-13 12:44:49.000000 apidriver-0.9.1/api_driver/loader_swagger.py
+-rw-r--r--   0 chnjx      (501) staff       (20)     4417 2023-04-13 12:44:49.000000 apidriver-0.9.1/api_driver/project_generator.py
+-rw-r--r--   0 chnjx      (501) staff       (20)     8018 2023-04-13 12:44:49.000000 apidriver-0.9.1/api_driver/swagger_generate.py
+-rw-r--r--   0 chnjx      (501) staff       (20)      485 2023-04-13 12:44:49.000000 apidriver-0.9.1/api_driver/template.py
+drwxr-xr-x   0 chnjx      (501) staff       (20)        0 2023-07-31 14:18:42.015825 apidriver-0.9.1/api_driver/templates/
+-rw-r--r--   0 chnjx      (501) staff       (20)     2121 2023-04-13 12:44:49.000000 apidriver-0.9.1/api_driver/templates/api.tpl
+-rw-r--r--   0 chnjx      (501) staff       (20)      374 2023-03-15 15:46:44.000000 apidriver-0.9.1/api_driver/templates/api_demo.tpl
+-rw-r--r--   0 chnjx      (501) staff       (20)      398 2023-03-15 15:08:27.000000 apidriver-0.9.1/api_driver/templates/base_testcase.tpl
+-rw-r--r--   0 chnjx      (501) staff       (20)     2879 2023-03-15 15:12:01.000000 apidriver-0.9.1/api_driver/templates/har2api_case.tpl
+-rw-r--r--   0 chnjx      (501) staff       (20)     2242 2023-03-15 15:12:01.000000 apidriver-0.9.1/api_driver/templates/har2case.tpl
+-rw-r--r--   0 chnjx      (501) staff       (20)     5224 2023-04-13 12:44:49.000000 apidriver-0.9.1/api_driver/templates/http.tpl
+-rw-r--r--   0 chnjx      (501) staff       (20)    15517 2023-07-31 14:13:10.000000 apidriver-0.9.1/api_driver/templates/report_template.html
+-rw-r--r--   0 chnjx      (501) staff       (20)      355 2023-03-15 13:14:27.000000 apidriver-0.9.1/api_driver/templates/testcase_demo.tpl
+-rw-r--r--   0 chnjx      (501) staff       (20)     2933 2023-04-13 12:44:49.000000 apidriver-0.9.1/api_driver/testcase_mixin.py
+drwxr-xr-x   0 chnjx      (501) staff       (20)        0 2023-07-31 14:18:42.020912 apidriver-0.9.1/api_driver/utils/
+-rw-r--r--   0 chnjx      (501) staff       (20)        0 2023-02-07 12:22:16.000000 apidriver-0.9.1/api_driver/utils/__init__.py
+-rw-r--r--   0 chnjx      (501) staff       (20)     1043 2023-03-15 15:08:27.000000 apidriver-0.9.1/api_driver/utils/custom_str_utils.py
+-rw-r--r--   0 chnjx      (501) staff       (20)     1882 2023-03-14 13:52:12.000000 apidriver-0.9.1/api_driver/utils/database_conn.py
+-rw-r--r--   0 chnjx      (501) staff       (20)     3322 2023-03-14 13:52:12.000000 apidriver-0.9.1/api_driver/utils/fake.py
+-rw-r--r--   0 chnjx      (501) staff       (20)     2172 2023-03-15 15:08:27.000000 apidriver-0.9.1/api_driver/utils/placeholder.py
+-rw-r--r--   0 chnjx      (501) staff       (20)     1283 2023-02-17 12:48:23.000000 apidriver-0.9.1/api_driver/utils/service_logger.py
+drwxr-xr-x   0 chnjx      (501) staff       (20)        0 2023-07-31 14:18:42.023610 apidriver-0.9.1/apidriver.egg-info/
+-rw-r--r--   0 chnjx      (501) staff       (20)      209 2023-07-31 14:18:41.000000 apidriver-0.9.1/apidriver.egg-info/PKG-INFO
+-rw-r--r--   0 chnjx      (501) staff       (20)     1061 2023-07-31 14:18:41.000000 apidriver-0.9.1/apidriver.egg-info/SOURCES.txt
+-rw-r--r--   0 chnjx      (501) staff       (20)        1 2023-07-31 14:18:41.000000 apidriver-0.9.1/apidriver.egg-info/dependency_links.txt
+-rw-r--r--   0 chnjx      (501) staff       (20)       39 2023-07-31 14:18:41.000000 apidriver-0.9.1/apidriver.egg-info/entry_points.txt
+-rw-r--r--   0 chnjx      (501) staff       (20)      171 2023-07-31 14:18:41.000000 apidriver-0.9.1/apidriver.egg-info/requires.txt
+-rw-r--r--   0 chnjx      (501) staff       (20)       11 2023-07-31 14:18:41.000000 apidriver-0.9.1/apidriver.egg-info/top_level.txt
+-rw-r--r--   0 chnjx      (501) staff       (20)      170 2023-04-13 12:44:49.000000 apidriver-0.9.1/requirements.txt
+-rw-r--r--   0 chnjx      (501) staff       (20)       38 2023-07-31 14:18:42.025287 apidriver-0.9.1/setup.cfg
+-rw-r--r--   0 chnjx      (501) staff       (20)      903 2023-04-13 12:44:49.000000 apidriver-0.9.1/setup.py
+drwxr-xr-x   0 chnjx      (501) staff       (20)        0 2023-07-31 14:18:42.024006 apidriver-0.9.1/test/
+-rw-r--r--   0 chnjx      (501) staff       (20)     1105 2023-04-13 12:44:49.000000 apidriver-0.9.1/test/test_cli.py
```

### Comparing `apidriver-0.9.0/LICENSE.txt` & `apidriver-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apidriver-0.9.0/README.md` & `apidriver-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `apidriver-0.9.0/api_driver/ad_utils.py` & `apidriver-0.9.1/api_driver/ad_utils.py`

 * *Files identical despite different names*

### Comparing `apidriver-0.9.0/api_driver/api_driver.py` & `apidriver-0.9.1/api_driver/api_driver.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding:utf-8 -*-
 # @Time     :2023/7/10 15:04
 # @Author   :CHNJX
 # @File     :api_driver.py
 # @Desc     :
+import logging
 import subprocess
 import time
 from datetime import datetime
 
 import pytest
 from jinja2 import Environment, FileSystemLoader
 
@@ -48,33 +49,46 @@
                 'test_model': test_suite,
                 'test_class': test_class,
                 'test_name': test_name,
                 'result': report.outcome,
                 'details': str(report.longrepr),
             }
 
+            # 获取测试用例方法的日志信息
+            logs = report.caplog if hasattr(report, 'caplog') else None
+            # 将测试用例方法的日志添加到results中
+            result['logs'] = logs
+
             if test_suite not in self.results:
                 self.results[test_suite] = {}
             if test_class not in self.results[test_suite]:
                 self.results[test_suite][test_class] = []
             self.results[test_suite][test_class].append(result)
 
+
+
     def get_results(self) -> dict:
         return {
             'test_count': self.test_count,
             'pass_count': self.pass_count,
             'fail_count': self.fail_count,
             'skip_count': self.skip_count,
             'error_count': self.error_count,
             'results': self.results
         }
 
 
 class ApiDriver:
 
+    def __init__(self):
+        self.setup_logging()
+
+    def setup_logging(self):
+        logging.basicConfig(level=logging.INFO)
+
     def run_tests(self, testcases: str, report_file: str = None):
         plugin = TestResultPlugin()
         start_time = time.time()
         pytest.main([testcases, '-v', '-s'], plugins=[plugin])
         end_time = time.time()
         execution_time = "{:.2f}s".format(end_time - start_time)
         res = plugin.get_results()
```

### Comparing `apidriver-0.9.0/api_driver/command.py` & `apidriver-0.9.1/api_driver/command.py`

 * *Files identical despite different names*

### Comparing `apidriver-0.9.0/api_driver/har_parser.py` & `apidriver-0.9.1/api_driver/har_parser.py`

 * *Files identical despite different names*

### Comparing `apidriver-0.9.0/api_driver/loader_swagger.py` & `apidriver-0.9.1/api_driver/loader_swagger.py`

 * *Files identical despite different names*

### Comparing `apidriver-0.9.0/api_driver/project_generator.py` & `apidriver-0.9.1/api_driver/project_generator.py`

 * *Files identical despite different names*

### Comparing `apidriver-0.9.0/api_driver/swagger_generate.py` & `apidriver-0.9.1/api_driver/swagger_generate.py`

 * *Files identical despite different names*

### Comparing `apidriver-0.9.0/api_driver/templates/api.tpl` & `apidriver-0.9.1/api_driver/templates/api.tpl`

 * *Files identical despite different names*

### Comparing `apidriver-0.9.0/api_driver/templates/har2api_case.tpl` & `apidriver-0.9.1/api_driver/templates/har2api_case.tpl`

 * *Files identical despite different names*

### Comparing `apidriver-0.9.0/api_driver/templates/har2case.tpl` & `apidriver-0.9.1/api_driver/templates/har2case.tpl`

 * *Files identical despite different names*

### Comparing `apidriver-0.9.0/api_driver/templates/http.tpl` & `apidriver-0.9.1/api_driver/templates/http.tpl`

 * *Files identical despite different names*

### Comparing `apidriver-0.9.0/api_driver/templates/report_template.html` & `apidriver-0.9.1/api_driver/templates/report_template.html`

 * *Files 2% similar despite different names*

```diff
@@ -475,14 +475,15 @@
        onChange="filterTable(this)"
        type="checkbox"/><span class="xfailed">0 expected failures</span>,
 <input
         checked="true" class="filter" data-test-result="xpassed" disabled="true" hidden="true" name="filter_checkbox"
         onChange="filterTable(this)" type="checkbox"/><span class="xpassed">0 unexpected passes</span>
 <h2>Results</h2>
 <table id="results-table">
+
     <thead id="results-table-head">
     <tr>
         <th class="sortable result initial-sort" col="result">Test Model</th>
         <th class="sortable" col="name">Test Class</th>
         <th class="sortable" col="duration">Case Name</th>
         <th class="sortable links" col="links">Result</th>
     </tr>
@@ -499,15 +500,20 @@
         <td class="col-result">{{ test.test_model }}</td>
         <td class="col-name">{{ test.test_class }}</td>
         <td class="col-duration">{{ test.test_name }}</td>
         <td class="col-links">{{ test.result }}</td>
     </tr>
     <tr>
         <td class="extra" colspan="4">
-            <div class="log">{{ test.details }}</div>
+                <!-- 折叠面板开始 -->
+                <details>
+                    <summary>Show Log</summary>
+                    <pre>{{ test.logs }}</pre>
+                </details>
+                <!-- 折叠面板结束 -->
         </td>
     </tr>
     </tbody>
     {% endfor %}
     {% endfor %}
     {% endfor %}
 </table>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -7,8 +7,10 @@
 {results.fail_count}} failed, * {{results.error_count}} errors, *0 expected
 failures, *0 unexpected passes
 ***** Results *****
 Test Model         Test Class            Case Name            Result
 No results found. Try to check the filters
 {{ test.test_model {{ test.test_class }} {{ test.test_name }} {{ test.result }}
 }}
-{{ test.details }}
+  Show Log
+{{ test.logs }}
+
```

### Comparing `apidriver-0.9.0/api_driver/testcase_mixin.py` & `apidriver-0.9.1/api_driver/testcase_mixin.py`

 * *Files identical despite different names*

### Comparing `apidriver-0.9.0/api_driver/utils/custom_str_utils.py` & `apidriver-0.9.1/api_driver/utils/custom_str_utils.py`

 * *Files identical despite different names*

### Comparing `apidriver-0.9.0/api_driver/utils/database_conn.py` & `apidriver-0.9.1/api_driver/utils/database_conn.py`

 * *Files identical despite different names*

### Comparing `apidriver-0.9.0/api_driver/utils/fake.py` & `apidriver-0.9.1/api_driver/utils/fake.py`

 * *Files identical despite different names*

### Comparing `apidriver-0.9.0/api_driver/utils/placeholder.py` & `apidriver-0.9.1/api_driver/utils/placeholder.py`

 * *Files identical despite different names*

### Comparing `apidriver-0.9.0/api_driver/utils/service_logger.py` & `apidriver-0.9.1/api_driver/utils/service_logger.py`

 * *Files identical despite different names*

### Comparing `apidriver-0.9.0/apidriver.egg-info/SOURCES.txt` & `apidriver-0.9.1/apidriver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apidriver-0.9.0/setup.py` & `apidriver-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `apidriver-0.9.0/test/test_cli.py` & `apidriver-0.9.1/test/test_cli.py`

 * *Files identical despite different names*

