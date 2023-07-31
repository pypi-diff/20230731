# Comparing `tmp/python-aap-0.0.6.tar.gz` & `tmp/python-aap-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-aap-0.0.6.tar", last modified: Mon Jul 31 09:26:53 2023, max compression
+gzip compressed data, was "python-aap-0.0.7.tar", last modified: Mon Jul 31 09:27:57 2023, max compression
```

## Comparing `python-aap-0.0.6.tar` & `python-aap-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 gitlab-runner   (991) gitlab-runner   (985)        0 2023-07-31 09:26:53.049655 python-aap-0.0.6/
--rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)     2735 2023-07-28 10:55:52.000000 python-aap-0.0.6/.gitignore
--rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)     1963 2023-07-31 09:26:37.000000 python-aap-0.0.6/.gitlab-ci.yml
--rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)    18020 2023-07-28 10:55:52.000000 python-aap-0.0.6/LICENSE
--rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)     3914 2023-07-31 09:26:53.048655 python-aap-0.0.6/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)     3321 2023-07-31 09:26:37.000000 python-aap-0.0.6/README.md
--rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)      817 2023-07-31 09:26:37.000000 python-aap-0.0.6/pyproject.toml
--rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)       17 2023-07-28 10:55:52.000000 python-aap-0.0.6/requirements.txt
--rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)       38 2023-07-31 09:26:53.049655 python-aap-0.0.6/setup.cfg
-drwxrwxr-x   0 gitlab-runner   (991) gitlab-runner   (985)        0 2023-07-31 09:26:53.042655 python-aap-0.0.6/src/
-drwxrwxr-x   0 gitlab-runner   (991) gitlab-runner   (985)        0 2023-07-31 09:26:53.046655 python-aap-0.0.6/src/aap/
--rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)      265 2023-07-31 09:26:37.000000 python-aap-0.0.6/src/aap/__init__.py
--rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)     4037 2023-07-31 09:26:37.000000 python-aap-0.0.6/src/aap/__main__.py
--rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)     5364 2023-07-31 09:26:37.000000 python-aap-0.0.6/src/aap/base.py
--rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)     3090 2023-07-31 09:26:37.000000 python-aap-0.0.6/src/aap/endpoints.py
--rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)     1901 2023-07-31 09:26:37.000000 python-aap-0.0.6/src/aap/mixins.py
-drwxrwxr-x   0 gitlab-runner   (991) gitlab-runner   (985)        0 2023-07-31 09:26:53.048655 python-aap-0.0.6/src/python_aap.egg-info/
--rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)     3914 2023-07-31 09:26:53.000000 python-aap-0.0.6/src/python_aap.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)      400 2023-07-31 09:26:53.000000 python-aap-0.0.6/src/python_aap.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)        1 2023-07-31 09:26:53.000000 python-aap-0.0.6/src/python_aap.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)       40 2023-07-31 09:26:53.000000 python-aap-0.0.6/src/python_aap.egg-info/entry_points.txt
--rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)       18 2023-07-31 09:26:53.000000 python-aap-0.0.6/src/python_aap.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner   (991) gitlab-runner   (985)        4 2023-07-31 09:26:53.000000 python-aap-0.0.6/src/python_aap.egg-info/top_level.txt
+drwxrwxr-x   0 gitlab-runner   (988) gitlab-runner   (982)        0 2023-07-31 09:27:57.246124 python-aap-0.0.7/
+-rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)     2735 2023-07-28 10:54:04.000000 python-aap-0.0.7/.gitignore
+-rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)     1963 2023-07-28 12:41:45.000000 python-aap-0.0.7/.gitlab-ci.yml
+-rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)    18020 2023-07-26 20:23:00.000000 python-aap-0.0.7/LICENSE
+-rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)     5310 2023-07-31 09:27:57.245124 python-aap-0.0.7/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)     4717 2023-07-31 09:27:45.000000 python-aap-0.0.7/README.md
+-rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)      817 2023-07-31 09:27:45.000000 python-aap-0.0.7/pyproject.toml
+-rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)       17 2023-07-28 10:54:04.000000 python-aap-0.0.7/requirements.txt
+-rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)       38 2023-07-31 09:27:57.246124 python-aap-0.0.7/setup.cfg
+drwxrwxr-x   0 gitlab-runner   (988) gitlab-runner   (982)        0 2023-07-31 09:27:57.239123 python-aap-0.0.7/src/
+drwxrwxr-x   0 gitlab-runner   (988) gitlab-runner   (982)        0 2023-07-31 09:27:57.244124 python-aap-0.0.7/src/aap/
+-rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)      265 2023-07-28 12:41:45.000000 python-aap-0.0.7/src/aap/__init__.py
+-rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)     4037 2023-07-31 09:26:15.000000 python-aap-0.0.7/src/aap/__main__.py
+-rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)     5364 2023-07-28 12:41:45.000000 python-aap-0.0.7/src/aap/base.py
+-rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)     3090 2023-07-28 12:41:45.000000 python-aap-0.0.7/src/aap/endpoints.py
+-rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)     1901 2023-07-28 12:41:45.000000 python-aap-0.0.7/src/aap/mixins.py
+drwxrwxr-x   0 gitlab-runner   (988) gitlab-runner   (982)        0 2023-07-31 09:27:57.245124 python-aap-0.0.7/src/python_aap.egg-info/
+-rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)     5310 2023-07-31 09:27:57.000000 python-aap-0.0.7/src/python_aap.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)      400 2023-07-31 09:27:57.000000 python-aap-0.0.7/src/python_aap.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)        1 2023-07-31 09:27:57.000000 python-aap-0.0.7/src/python_aap.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)       40 2023-07-31 09:27:57.000000 python-aap-0.0.7/src/python_aap.egg-info/entry_points.txt
+-rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)       18 2023-07-31 09:27:57.000000 python-aap-0.0.7/src/python_aap.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner   (988) gitlab-runner   (982)        4 2023-07-31 09:27:57.000000 python-aap-0.0.7/src/python_aap.egg-info/top_level.txt
```

### Comparing `python-aap-0.0.6/.gitignore` & `python-aap-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `python-aap-0.0.6/.gitlab-ci.yml` & `python-aap-0.0.7/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `python-aap-0.0.6/LICENSE` & `python-aap-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `python-aap-0.0.6/PKG-INFO` & `python-aap-0.0.7/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,55 @@
-Metadata-Version: 2.1
-Name: python-aap
-Version: 0.0.6
-Summary: Unofficial python wrapper over Ansible Automation Platform REST API
-Author-email: Ivan Mitruk <imitruk@redhat.com>
-Project-URL: Homepage, https://gitlab.corp.redhat.com/network/python-aap/
-Project-URL: Bug Tracker, https://gitlab.corp.redhat.com/network/python-aap/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Ansible Automation Platform Python Module
 
 This is unofficial wrapper for Ansible Automation Platform (AAP) API.
 
 To see an example how this module can be used please view [__main__.py](./src/aap/__main__.py)
 
 ## Executing jobs from CLI
 
-Python module can be invoked directly to execute job in aap and report status to terminal.
+Python module can be invoked directly to execute job in aap and report status to terminal. AAP Credentials need to be specified either via CLI arguments or env variables
+
 
+
+Usage:
 ```
-python3 -m aap run-job --id <job-id> -f
+usage: python3 -m aap [-h] -i ID [-f] [-p PASSWORD] [-u USERNAME] [-s URL]
+                      [--insecure] [-l LIMIT] [-e EXTRA] [-r RETRIES]
+                      [-t TIMEOUT] [--ignore-fail]
+                      {run-job}
+
+Trigger jobs and workflows from terminal
+
+positional arguments:
+  {run-job}
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -i ID, --id ID        ID of job to run
+  -f, --follow          Wait for job to finish execution and report its status
+  -p PASSWORD, --password PASSWORD
+                        Password used for authentication to AAP API (env:
+                        AAP_PASSWORD)
+  -u USERNAME, --username USERNAME
+                        Username used for authentication to AAP API (env:
+                        AAP_USERNAME)
+  -s URL, --url URL     URL of AAP instance (env: AAP_URL)
+  --insecure            Dont verify ssl certificate
+  -l LIMIT, --limit LIMIT
+                        Limit as comma separated list
+  -e EXTRA, --extra-vars EXTRA
+                        json formatted extra variables
+  -r RETRIES, --retries RETRIES
+                        Number of retries on API error
+  -t TIMEOUT, --poll-timeout TIMEOUT
+                        Number of seconds between 2 polling requests to aap
+  --ignore-fail         Program will return successfull even if job fails
 ```
 
+
 Example run
 ```
 $ python3 -m aap --id 7848 -l sw01-dist.itdev --insecure run-job -f
 Searching job 7848
 Job: Juniper - gather facts
         limit: ['sw01-dist.itdev']
         extra variables: {}
```

### Comparing `python-aap-0.0.6/pyproject.toml` & `python-aap-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "python-aap"
-version = "0.0.6"
+version = "0.0.7"
 dependencies = [
   'requests',
   'datetime'
 ]
 authors = [
   { name="Ivan Mitruk", email="imitruk@redhat.com" },
 ]
```

### Comparing `python-aap-0.0.6/src/aap/__main__.py` & `python-aap-0.0.7/src/aap/__main__.py`

 * *Files identical despite different names*

### Comparing `python-aap-0.0.6/src/aap/base.py` & `python-aap-0.0.7/src/aap/base.py`

 * *Files identical despite different names*

### Comparing `python-aap-0.0.6/src/aap/endpoints.py` & `python-aap-0.0.7/src/aap/endpoints.py`

 * *Files identical despite different names*

### Comparing `python-aap-0.0.6/src/aap/mixins.py` & `python-aap-0.0.7/src/aap/mixins.py`

 * *Files identical despite different names*

