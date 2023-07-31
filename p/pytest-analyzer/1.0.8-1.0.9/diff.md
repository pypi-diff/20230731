# Comparing `tmp/pytest-analyzer-1.0.8.tar.gz` & `tmp/pytest-analyzer-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-analyzer-1.0.8.tar", last modified: Fri Jul 28 17:21:25 2023, max compression
+gzip compressed data, was "pytest-analyzer-1.0.9.tar", last modified: Mon Jul 31 10:01:29 2023, max compression
```

## Comparing `pytest-analyzer-1.0.8.tar` & `pytest-analyzer-1.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 17:21:25.338924 pytest-analyzer-1.0.8/
--rw-rw-rw-   0        0        0     1091 2023-05-04 18:48:32.000000 pytest-analyzer-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     3528 2023-07-28 17:21:25.338924 pytest-analyzer-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2848 2023-07-28 14:05:19.000000 pytest-analyzer-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 17:21:25.331925 pytest-analyzer-1.0.8/analyzer/
--rw-rw-rw-   0        0        0        0 2023-07-28 12:45:20.000000 pytest-analyzer-1.0.8/analyzer/__init__.py
--rw-rw-rw-   0        0        0     6868 2023-07-28 17:08:49.000000 pytest-analyzer-1.0.8/analyzer/analyzer.py
--rw-rw-rw-   0        0        0      702 2023-07-28 13:54:36.000000 pytest-analyzer-1.0.8/analyzer/code_collector.py
--rw-rw-rw-   0        0        0     5536 2023-07-28 13:59:23.000000 pytest-analyzer-1.0.8/analyzer/connector.py
--rw-rw-rw-   0        0        0     3149 2023-07-28 13:54:36.000000 pytest-analyzer-1.0.8/analyzer/decorator_updater.py
--rw-rw-rw-   0        0        0     1750 2023-07-28 09:36:45.000000 pytest-analyzer-1.0.8/analyzer/testItem.py
--rw-rw-rw-   0        0        0      731 2023-07-28 10:25:11.000000 pytest-analyzer-1.0.8/analyzer/testRunConfig.py
--rw-rw-rw-   0        0        0     1360 2023-07-28 13:54:36.000000 pytest-analyzer-1.0.8/analyzer/testomat_item.py
--rw-rw-rw-   0        0        0      957 2023-07-28 17:19:40.000000 pytest-analyzer-1.0.8/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-28 17:21:25.335924 pytest-analyzer-1.0.8/pytest_analyzer.egg-info/
--rw-rw-rw-   0        0        0     3528 2023-07-28 17:21:25.000000 pytest-analyzer-1.0.8/pytest_analyzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      506 2023-07-28 17:21:25.000000 pytest-analyzer-1.0.8/pytest_analyzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 17:21:25.000000 pytest-analyzer-1.0.8/pytest_analyzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-28 17:21:25.000000 pytest-analyzer-1.0.8/pytest_analyzer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       47 2023-07-28 17:21:25.000000 pytest-analyzer-1.0.8/pytest_analyzer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-28 17:21:25.000000 pytest-analyzer-1.0.8/pytest_analyzer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 17:21:25.338924 pytest-analyzer-1.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-28 17:21:25.337924 pytest-analyzer-1.0.8/tests/
--rw-rw-rw-   0        0        0      320 2023-07-28 11:32:13.000000 pytest-analyzer-1.0.8/tests/test_class_root.py
--rw-rw-rw-   0        0        0      546 2023-07-28 11:32:13.000000 pytest-analyzer-1.0.8/tests/test_root.py
+drwxrwxrwx   0        0        0        0 2023-07-31 10:01:29.066019 pytest-analyzer-1.0.9/
+-rw-rw-rw-   0        0        0     1091 2023-05-04 18:48:32.000000 pytest-analyzer-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     2985 2023-07-31 10:01:29.065019 pytest-analyzer-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2305 2023-07-31 10:00:47.000000 pytest-analyzer-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 10:01:29.059019 pytest-analyzer-1.0.9/analyzer/
+-rw-rw-rw-   0        0        0        0 2023-07-28 12:45:20.000000 pytest-analyzer-1.0.9/analyzer/__init__.py
+-rw-rw-rw-   0        0        0     7115 2023-07-31 09:55:50.000000 pytest-analyzer-1.0.9/analyzer/analyzer.py
+-rw-rw-rw-   0        0        0      702 2023-07-28 13:54:36.000000 pytest-analyzer-1.0.9/analyzer/code_collector.py
+-rw-rw-rw-   0        0        0     5536 2023-07-28 13:59:23.000000 pytest-analyzer-1.0.9/analyzer/connector.py
+-rw-rw-rw-   0        0        0     3149 2023-07-28 13:54:36.000000 pytest-analyzer-1.0.9/analyzer/decorator_updater.py
+-rw-rw-rw-   0        0        0     1750 2023-07-28 09:36:45.000000 pytest-analyzer-1.0.9/analyzer/testItem.py
+-rw-rw-rw-   0        0        0      731 2023-07-28 10:25:11.000000 pytest-analyzer-1.0.9/analyzer/testRunConfig.py
+-rw-rw-rw-   0        0        0     1360 2023-07-28 13:54:36.000000 pytest-analyzer-1.0.9/analyzer/testomat_item.py
+-rw-rw-rw-   0        0        0      957 2023-07-31 09:54:12.000000 pytest-analyzer-1.0.9/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-31 10:01:29.063019 pytest-analyzer-1.0.9/pytest_analyzer.egg-info/
+-rw-rw-rw-   0        0        0     2985 2023-07-31 10:01:29.000000 pytest-analyzer-1.0.9/pytest_analyzer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      506 2023-07-31 10:01:29.000000 pytest-analyzer-1.0.9/pytest_analyzer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 10:01:29.000000 pytest-analyzer-1.0.9/pytest_analyzer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-31 10:01:29.000000 pytest-analyzer-1.0.9/pytest_analyzer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       47 2023-07-31 10:01:29.000000 pytest-analyzer-1.0.9/pytest_analyzer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-31 10:01:29.000000 pytest-analyzer-1.0.9/pytest_analyzer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 10:01:29.066019 pytest-analyzer-1.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-31 10:01:29.065019 pytest-analyzer-1.0.9/tests/
+-rw-rw-rw-   0        0        0      320 2023-07-28 11:32:13.000000 pytest-analyzer-1.0.9/tests/test_class_root.py
+-rw-rw-rw-   0        0        0      546 2023-07-28 11:32:13.000000 pytest-analyzer-1.0.9/tests/test_root.py
```

### Comparing `pytest-analyzer-1.0.8/LICENSE` & `pytest-analyzer-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-analyzer-1.0.8/PKG-INFO` & `pytest-analyzer-1.0.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-analyzer
-Version: 1.0.8
+Version: 1.0.9
 Summary: this plugin allows to analyze tests in pytest project, collect test metadata and sync it with testomat.io TCM system
 Author: Oleksii Ostapov
 Project-URL: Author's Blog, https://qamania.org
 Project-URL: Homepage, https://github.com/Ypurek/pytest-analyzer
 Project-URL: Bug Tracker, https://github.com/Ypurek/pytest-analyzer/issues
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 3
@@ -50,53 +50,39 @@
 
 Run pytest with analyzer remove parameter to remove all test ids from your tests. Tests will not be executed
 
 ```bash
 pytest --analyzer remove
 ```
 
-Run pytest with analyzer sync parameter to execute tests and send the execution status to testomat.io
+Run pytest with analyzer sync parameter to execute tests and send the execution status to testomat.io.  
+Sync can be executed even without marking tests with ids. If testomat.io failed to match tests by title, it will create new tests for the run
 
 ```bash
 pytest --analyzer sync
 ```
 
 Run pytest with analyzer debug parameter to get test data collected in metadata.json file
 
 ```bash
 pytest --analyzer debug
 ```
 
 ### Advanced usage
 
-to configure additional test run parameters call `analyzer_test_config` fixture.  
-This fixture return `TestRunConfig` object with next parameters:
+to configure test environment, you can use additional option:
 
-- **test_run_id** - do not modify. this parameter is set automatically
-- **title** - test run title. Leave empty to have generic run title like "pytest run at 2020-01-01 00:00:00"
-- **environment** - test environment. Empty by default. Set any suitable: "staging", "production", "test", "Winddows
-  11", "Chrome 115", etc
-- **group_title** - Empty by default. Creates folder in testomat.io for test runs with specified name
-- **parallel** - False by default. Set to True if you run tests in parallel
-
-Example:
-
-```python
-import pytest
-
-
-@pytest.fixture(scope="session")
-def get_web_browser(playwright_fixture, analyzer_test_config):
-    browser = playwright_fixture.chromium.launch()
-    analyzer_test_config.environment = 'chromium'
-    yield browser
-    browser.close()
+```bash
+pytest --analyzer sync --testRunEnv windows11,chrome,1920x1080
 ```
 
+Eny environments used in test run. Should be placed in comma separated list, NO SPACES ALLOWED.
+
 ### Clarifications
+
 - tests can be synced even without `@mark.testomatio('@T96c700e6')` decorator.
 - test title in testomat.io == test name in pytest
 - test suit title in testomat.io == test file name in pytest
 
 ## Example of test
 
 To make analyzer experience more consistent, it uses standard pytest markers.  
@@ -111,8 +97,8 @@
     assert 2 + 2 == 4
 ```
 
 ## Roadmap
 
 - handle REST API exceptions
 - support screenshot attachments
-- 
+- improve logging
```

### Comparing `pytest-analyzer-1.0.8/README.md` & `pytest-analyzer-1.0.9/pytest_analyzer.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: pytest-analyzer
+Version: 1.0.9
+Summary: this plugin allows to analyze tests in pytest project, collect test metadata and sync it with testomat.io TCM system
+Author: Oleksii Ostapov
+Project-URL: Author's Blog, https://qamania.org
+Project-URL: Homepage, https://github.com/Ypurek/pytest-analyzer
+Project-URL: Bug Tracker, https://github.com/Ypurek/pytest-analyzer/issues
+Classifier: Framework :: Pytest
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Testomat.io plugin for pytest
 
 ## uses Testomat.io API:
 
 - https://testomatio.github.io/check-tests/
 - https://testomatio.github.io/reporter/
 
@@ -34,53 +50,39 @@
 
 Run pytest with analyzer remove parameter to remove all test ids from your tests. Tests will not be executed
 
 ```bash
 pytest --analyzer remove
 ```
 
-Run pytest with analyzer sync parameter to execute tests and send the execution status to testomat.io
+Run pytest with analyzer sync parameter to execute tests and send the execution status to testomat.io.  
+Sync can be executed even without marking tests with ids. If testomat.io failed to match tests by title, it will create new tests for the run
 
 ```bash
 pytest --analyzer sync
 ```
 
 Run pytest with analyzer debug parameter to get test data collected in metadata.json file
 
 ```bash
 pytest --analyzer debug
 ```
 
 ### Advanced usage
 
-to configure additional test run parameters call `analyzer_test_config` fixture.  
-This fixture return `TestRunConfig` object with next parameters:
-
-- **test_run_id** - do not modify. this parameter is set automatically
-- **title** - test run title. Leave empty to have generic run title like "pytest run at 2020-01-01 00:00:00"
-- **environment** - test environment. Empty by default. Set any suitable: "staging", "production", "test", "Winddows
-  11", "Chrome 115", etc
-- **group_title** - Empty by default. Creates folder in testomat.io for test runs with specified name
-- **parallel** - False by default. Set to True if you run tests in parallel
-
-Example:
-
-```python
-import pytest
+to configure test environment, you can use additional option:
 
-
-@pytest.fixture(scope="session")
-def get_web_browser(playwright_fixture, analyzer_test_config):
-    browser = playwright_fixture.chromium.launch()
-    analyzer_test_config.environment = 'chromium'
-    yield browser
-    browser.close()
+```bash
+pytest --analyzer sync --testRunEnv windows11,chrome,1920x1080
 ```
 
+Eny environments used in test run. Should be placed in comma separated list, NO SPACES ALLOWED.
+
 ### Clarifications
+
 - tests can be synced even without `@mark.testomatio('@T96c700e6')` decorator.
 - test title in testomat.io == test name in pytest
 - test suit title in testomat.io == test file name in pytest
 
 ## Example of test
 
 To make analyzer experience more consistent, it uses standard pytest markers.  
@@ -95,8 +97,8 @@
     assert 2 + 2 == 4
 ```
 
 ## Roadmap
 
 - handle REST API exceptions
 - support screenshot attachments
-- 
+- improve logging
```

### Comparing `pytest-analyzer-1.0.8/analyzer/analyzer.py` & `pytest-analyzer-1.0.9/analyzer/analyzer.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,44 +22,45 @@
             'debug - saves analyzed test metadata to the json in the test project root\n'
 
 
 def pytest_addoption(parser: Parser) -> None:
     parser.addoption(f'--{analyzer_option}',
                      action='store',
                      help=help_text)
+    parser.addoption(f'--testRunEnv',
+                     action='store',
+                     help='specify test run environment for testomat.io. Works only with --analyzer sync')
 
     parser.addini('testomatio_url', 'testomat.io base url', default='https://app.testomat.io')
     parser.addini('testomatio_project', 'testomat.io project api key')
     parser.addini('testomatio_email', 'testomat.io user email')
     parser.addini('testomatio_password', 'testomat.io user password')
 
 
 def pytest_configure(config: Config):
     config.addinivalue_line(
         "markers", "testomatio(arg): built in marker to connect test case with testomat.io by unique id"
     )
 
     pytest.analyzer_test_run_config = TestRunConfig()
 
+
     if config.getoption(analyzer_option):
         url = config.getini('testomatio_url')
         project = config.getini('testomatio_project')
         email = config.getini('testomatio_email')
         password = config.getini('testomatio_password')
         connector = Connector(email, password, url, project)
         connector.connect()
         pytest.connector = connector
+        if config.getoption('testRunEnv'):
+            pytest.analyzer_test_run_config.environment = config.getoption('testRunEnv')
 
 
 
-@pytest.fixture(scope='session')
-def analyzer_test_config():
-    yield pytest.analyzer_test_run_config
-
-
 def collect_tests(items: list[Item]):
     meta: list[TestItem] = list()
     test_files: set = set()
     test_names: list = list()
     parameter_filter: set[Item] = set()
     for item in items:
         if item.function not in parameter_filter:
@@ -128,15 +129,15 @@
     test_item = TestItem(item)
     request = {
         'status': None,
         'title': test_item.title,
         'run_time': call.duration,
         'suite_title': test_item.file_name,
         'suite_id': None,
-        'test_id': test_item.id[2:],  # remove @T
+        'test_id': test_item.id[2:] if test_item.id else None,  # remove @T if exists
         'message': None,
         'stack': None,
         'example': None,
         'artifacts': None,
         'steps': None,
         'code': None,
     }
```

### Comparing `pytest-analyzer-1.0.8/analyzer/code_collector.py` & `pytest-analyzer-1.0.9/analyzer/code_collector.py`

 * *Files identical despite different names*

### Comparing `pytest-analyzer-1.0.8/analyzer/connector.py` & `pytest-analyzer-1.0.9/analyzer/connector.py`

 * *Files identical despite different names*

### Comparing `pytest-analyzer-1.0.8/analyzer/decorator_updater.py` & `pytest-analyzer-1.0.9/analyzer/decorator_updater.py`

 * *Files identical despite different names*

### Comparing `pytest-analyzer-1.0.8/analyzer/testItem.py` & `pytest-analyzer-1.0.9/analyzer/testItem.py`

 * *Files identical despite different names*

### Comparing `pytest-analyzer-1.0.8/analyzer/testRunConfig.py` & `pytest-analyzer-1.0.9/analyzer/testRunConfig.py`

 * *Files identical despite different names*

### Comparing `pytest-analyzer-1.0.8/analyzer/testomat_item.py` & `pytest-analyzer-1.0.9/analyzer/testomat_item.py`

 * *Files identical despite different names*

### Comparing `pytest-analyzer-1.0.8/pyproject.toml` & `pytest-analyzer-1.0.9/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.5.1", "requests>=2.29.0", "autopep8>=2.0.2", "pytest>=7.3.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytest-analyzer"
-version = "1.0.8"
+version = "1.0.9"
 
 dependencies = [
   "requests>=2.29.0",
   "autopep8>=2.0.2",
   "pytest>=7.3.1",]
 
 authors = [
```

### Comparing `pytest-analyzer-1.0.8/tests/test_root.py` & `pytest-analyzer-1.0.9/tests/test_root.py`

 * *Files identical despite different names*

