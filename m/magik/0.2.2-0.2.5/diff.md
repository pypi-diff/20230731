# Comparing `tmp/magik-0.2.2.tar.gz` & `tmp/magik-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magik-0.2.2.tar", last modified: Wed Jul 26 12:55:20 2023, max compression
+gzip compressed data, was "magik-0.2.5.tar", last modified: Mon Jul 31 09:38:43 2023, max compression
```

## Comparing `magik-0.2.2.tar` & `magik-0.2.5.tar`

### file list

```diff
@@ -1,34 +1,40 @@
-drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-26 12:55:20.832035 magik-0.2.2/
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     6006 2023-07-26 12:55:20.831847 magik-0.2.2/PKG-INFO
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     5580 2023-07-19 22:37:02.000000 magik-0.2.2/README.md
-drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-26 12:55:20.830821 magik-0.2.2/magik/
--rw-r--r--   0 shivsakhuja   (501) staff       (20)        0 2023-07-14 11:51:21.000000 magik-0.2.2/magik/__init__.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1844 2023-07-26 12:54:23.000000 magik-0.2.2/magik/classifier.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     2622 2023-07-26 12:54:23.000000 magik-0.2.2/magik/cli.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      455 2023-07-20 08:24:46.000000 magik-0.2.2/magik/config.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      662 2023-07-26 12:54:23.000000 magik-0.2.2/magik/constants.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      617 2023-07-22 21:10:23.000000 magik-0.2.2/magik/decorators.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1867 2023-07-26 12:54:23.000000 magik-0.2.2/magik/deploy.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)    12979 2023-07-26 12:54:23.000000 magik-0.2.2/magik/evaluators.py
-drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-26 12:55:20.831708 magik-0.2.2/magik/examples/
--rw-r--r--   0 shivsakhuja   (501) staff       (20)        0 2023-07-14 12:49:25.000000 magik-0.2.2/magik/examples/__init__.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1295 2023-07-19 22:36:56.000000 magik-0.2.2/magik/examples/assertions.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1385 2023-07-19 22:36:56.000000 magik-0.2.2/magik/generate.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     3007 2023-07-26 12:54:23.000000 magik-0.2.2/magik/initialize.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1922 2023-07-25 12:50:52.000000 magik-0.2.2/magik/internal_logger.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1001 2023-07-26 12:54:23.000000 magik-0.2.2/magik/logger.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      390 2023-07-08 20:18:24.000000 magik-0.2.2/magik/matchers.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1248 2023-07-26 12:54:23.000000 magik-0.2.2/magik/openai_helper.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     8900 2023-07-26 12:54:23.000000 magik-0.2.2/magik/run.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      822 2023-07-26 12:54:23.000000 magik-0.2.2/magik/similarity.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     2990 2023-07-19 22:36:56.000000 magik-0.2.2/magik/sys_exec.py
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     1539 2023-07-19 22:36:56.000000 magik-0.2.2/magik/utils.py
-drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-26 12:55:20.831502 magik-0.2.2/magik.egg-info/
--rw-r--r--   0 shivsakhuja   (501) staff       (20)     6006 2023-07-26 12:55:20.000000 magik-0.2.2/magik.egg-info/PKG-INFO
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      578 2023-07-26 12:55:20.000000 magik-0.2.2/magik.egg-info/SOURCES.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)        1 2023-07-26 12:55:20.000000 magik-0.2.2/magik.egg-info/dependency_links.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)       42 2023-07-26 12:55:20.000000 magik-0.2.2/magik.egg-info/entry_points.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      234 2023-07-26 12:55:20.000000 magik-0.2.2/magik.egg-info/requires.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)        6 2023-07-26 12:55:20.000000 magik-0.2.2/magik.egg-info/top_level.txt
--rw-r--r--   0 shivsakhuja   (501) staff       (20)       38 2023-07-26 12:55:20.832078 magik-0.2.2/setup.cfg
--rw-r--r--   0 shivsakhuja   (501) staff       (20)      823 2023-07-26 12:54:23.000000 magik-0.2.2/setup.py
+drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-31 09:38:43.328557 magik-0.2.5/
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     6319 2023-07-31 09:38:43.328455 magik-0.2.5/PKG-INFO
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     5893 2023-07-30 16:27:04.000000 magik-0.2.5/README.md
+drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-31 09:38:43.326968 magik-0.2.5/magik/
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)        0 2023-07-14 11:51:21.000000 magik-0.2.5/magik/__init__.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1839 2023-07-29 14:27:16.000000 magik-0.2.5/magik/classifier.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     3414 2023-07-30 13:57:18.000000 magik-0.2.5/magik/cli.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      445 2023-07-29 14:27:16.000000 magik-0.2.5/magik/config.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      662 2023-07-28 12:36:18.000000 magik-0.2.5/magik/constants.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      617 2023-07-22 21:10:23.000000 magik-0.2.5/magik/decorators.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1913 2023-07-29 14:27:16.000000 magik-0.2.5/magik/deploy.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)    12925 2023-07-31 09:34:50.000000 magik-0.2.5/magik/evaluators.py
+drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-31 09:38:43.327825 magik-0.2.5/magik/examples/
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)        0 2023-07-14 12:49:25.000000 magik-0.2.5/magik/examples/__init__.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1295 2023-07-19 22:36:56.000000 magik-0.2.5/magik/examples/assertions.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1374 2023-07-29 14:27:16.000000 magik-0.2.5/magik/generate.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     2992 2023-07-29 14:27:16.000000 magik-0.2.5/magik/initialize.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     2399 2023-07-30 13:57:18.000000 magik-0.2.5/magik/internal_logger.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1825 2023-07-31 09:34:50.000000 magik-0.2.5/magik/logger.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      390 2023-07-08 20:18:24.000000 magik-0.2.5/magik/matchers.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      703 2023-07-29 12:14:49.000000 magik-0.2.5/magik/metrics.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     3148 2023-07-29 15:05:06.000000 magik-0.2.5/magik/openai_helper.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)    10626 2023-07-31 09:34:50.000000 magik-0.2.5/magik/run.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     4559 2023-07-30 16:22:18.000000 magik-0.2.5/magik/run_logger.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      817 2023-07-29 14:27:16.000000 magik-0.2.5/magik/similarity.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     3016 2023-07-29 14:27:16.000000 magik-0.2.5/magik/sys_exec.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1765 2023-07-29 14:27:16.000000 magik-0.2.5/magik/test_loader.py
+drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-31 09:38:43.328184 magik-0.2.5/magik/types/
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)        0 2023-07-29 12:14:49.000000 magik-0.2.5/magik/types/__init__.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      904 2023-07-31 09:34:50.000000 magik-0.2.5/magik/types/test_run.py
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     1539 2023-07-29 14:41:33.000000 magik-0.2.5/magik/utils.py
+drwxr-xr-x   0 shivsakhuja   (501) staff       (20)        0 2023-07-31 09:38:43.327656 magik-0.2.5/magik.egg-info/
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)     6319 2023-07-31 09:38:43.000000 magik-0.2.5/magik.egg-info/PKG-INFO
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      684 2023-07-31 09:38:43.000000 magik-0.2.5/magik.egg-info/SOURCES.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)        1 2023-07-31 09:38:43.000000 magik-0.2.5/magik.egg-info/dependency_links.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)       42 2023-07-31 09:38:43.000000 magik-0.2.5/magik.egg-info/entry_points.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      301 2023-07-31 09:38:43.000000 magik-0.2.5/magik.egg-info/requires.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)        6 2023-07-31 09:38:43.000000 magik-0.2.5/magik.egg-info/top_level.txt
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)       38 2023-07-31 09:38:43.328592 magik-0.2.5/setup.cfg
+-rw-r--r--   0 shivsakhuja   (501) staff       (20)      823 2023-07-31 09:35:39.000000 magik-0.2.5/setup.py
```

### Comparing `magik-0.2.2/PKG-INFO` & `magik-0.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magik
-Version: 0.2.2
+Version: 0.2.5
 Summary: SDK to write and run tests for your LLM app
 Home-page: UNKNOWN
 Author: Magik Labs Team
 Author-email: hello@magiklabs.app
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -18,35 +18,34 @@
 
 # Overview
 
 Reliability of output is one of the biggest challenges for people trying to use LLM apps in production.<br />
 
 Since LLM outputs are non-deterministic, it’s very hard to measure how good the output is.
 
-Eyeballing the responses from an LLM can work in development, but it’s not a great solution. 
+Eyeballing the responses from an LLM can work in development, but it’s not a great solution.
 
 > _In production, it’s virtually impossible to eyeball thousands of responses. Which means you have very little visibility into how well your LLM is performing._
 
 - Do you know when your LLM app is hallucinating?
-- How do you know how well it's *really* performing?
+- How do you know how well it's _really_ performing?
 - Do you know how often it’s producing a critically bad output?
 - How do you know what your users are seeing?
 - How do you measure how good your LLM responses are? And if you can’t measure it, how do you improve the accuracy?
 
 <br />
 
 > If these sound like problems to you (today or in the future), please reach out to us at hello@magiklabs.app. We’d love to hear more!
 
 <img width="1576" alt="llm-screenshot-1" src="https://github.com/magiklabs/magik-sdk/assets/7515552/bc87aefa-505f-4732-84cd-b7fe57857850">
 
-
 <br /><br /><br />
 
-
 # Documentation
+
 `pip install magik`
 
 See https://docs.magiklabs.app for instructions on how to write and run tests.
 
 - [Overview](https://docs.magiklabs.app/)
 - [Quick Start](https://docs.magiklabs.app/quick-start)
 - [Writing Tests](https://docs.magiklabs.app/reference/writing-tests)
@@ -74,17 +73,17 @@
 Test-driven development can speed up your development very nicely, and can help you engineer your prompts to be more robust.
 
 For example, assuming your prompt looks like this:
 
 ```
 Create some marketing copy for a tweet of less than 280 characters for my app {app_name}.
 
-My app helps people generate sales emails using AI. 
+My app helps people generate sales emails using AI.
 
-Make sure the marketing copy contains a complete and valid link to my app. 
+Make sure the marketing copy contains a complete and valid link to my app.
 
 Here is the link to my app: https://magiklabs.app.
 ```
 
 You can write tests like this:
 
 ```python
@@ -92,59 +91,61 @@
     contains_none,
     contains_link,
     contains_valid_link,
     is_positive_sentiment,
     length_less_than,
 )
 
-
+# Local context - this is used as the "ground truth" data that you can compare against in your tests
+test_context = {}
 
 # Define tests here
-tests = [
-    {
-        "description": "output contains a link",
-        "eval": contains_link(),
-        "prompt_vars": {
-            "app_name": "Uber",
+def define_tests(context: dict):
+    return [
+        {
+            "description": "output contains a link",
+            "eval": contains_link(),
+            "prompt_vars": {
+                "app_name": "Uber",
+            },
+            "failure_labels": ["bad_response_format"],
         },
-        "failure_labels": ["bad_response_format"],
-    },
-    {
-        "description": "output contains a valid link",
-        "eval": contains_valid_link(),
-        "prompt_vars": {
-            "app_name": "Magik",
+        {
+            "description": "output contains a valid link",
+            "eval": contains_valid_link(),
+            "prompt_vars": {
+                "app_name": "Magik",
+            },
+            "failure_labels": ["bad_response_format"],
         },
-        "failure_labels": ["bad_response_format"],
-    },
-    {
-        "description": "output sentiment is positive",
-        "eval": is_positive_sentiment(),
-        "prompt_vars": {
-            "app_name": "Lyft",
+        {
+            "description": "output sentiment is positive",
+            "eval": is_positive_sentiment(),
+            "prompt_vars": {
+                "app_name": "Lyft",
+            },
+            "failure_labels": ["negative_sentiment"],
         },
-        "failure_labels": ["negative_sentiment"],
-    },
-    {
-        "description": "output length is less than 280 characters",
-        "eval": length_less_than(280),
-        "prompt_vars": {
-            "app_name": "Facebook",
+        {
+            "description": "output length is less than 280 characters",
+            "eval": length_less_than(280),
+            "prompt_vars": {
+                "app_name": "Facebook",
+            },
+            "failure_labels": ["negative_sentiment", "critical"],
         },
-        "failure_labels": ["negative_sentiment", "critical"],
-    },
-    {
-        "description": "output does not contain hashtags",
-        "eval": contains_none(['#']),
-        "prompt_vars": {
-            "app_name": "Datadog",
+        {
+            "description": "output does not contain hashtags",
+            "eval": contains_none(['#']),
+            "prompt_vars": {
+                "app_name": "Datadog",
+            },
+            "failure_labels": ["bad_response_format"],
         },
-        "failure_labels": ["bad_response_format"],
-    },
-]
+    ]
 ```
 
 <br /><br />
 
 ### If you have an LLM app in production:
 
 ---
@@ -159,15 +160,14 @@
 
 - Filter by failure labels, severity, prompt, etc to identify different types of errors that are occurring in your LLM outputs.
 
 See https://magiklabs.app for more details, or contact us at [hello@magiklabs.app](mailto:hello@magiklabs.app)
 
 <br /><br />
 
-
 ### Upcoming Features
 
 ---
 
 Soon, you will also be able to:
 
 - Fail bad outputs before they get to your users.
```

### Comparing `magik-0.2.2/README.md` & `magik-0.2.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,35 +3,34 @@
 
 # Overview
 
 Reliability of output is one of the biggest challenges for people trying to use LLM apps in production.<br />
 
 Since LLM outputs are non-deterministic, it’s very hard to measure how good the output is.
 
-Eyeballing the responses from an LLM can work in development, but it’s not a great solution. 
+Eyeballing the responses from an LLM can work in development, but it’s not a great solution.
 
 > _In production, it’s virtually impossible to eyeball thousands of responses. Which means you have very little visibility into how well your LLM is performing._
 
 - Do you know when your LLM app is hallucinating?
-- How do you know how well it's *really* performing?
+- How do you know how well it's _really_ performing?
 - Do you know how often it’s producing a critically bad output?
 - How do you know what your users are seeing?
 - How do you measure how good your LLM responses are? And if you can’t measure it, how do you improve the accuracy?
 
 <br />
 
 > If these sound like problems to you (today or in the future), please reach out to us at hello@magiklabs.app. We’d love to hear more!
 
 <img width="1576" alt="llm-screenshot-1" src="https://github.com/magiklabs/magik-sdk/assets/7515552/bc87aefa-505f-4732-84cd-b7fe57857850">
 
-
 <br /><br /><br />
 
-
 # Documentation
+
 `pip install magik`
 
 See https://docs.magiklabs.app for instructions on how to write and run tests.
 
 - [Overview](https://docs.magiklabs.app/)
 - [Quick Start](https://docs.magiklabs.app/quick-start)
 - [Writing Tests](https://docs.magiklabs.app/reference/writing-tests)
@@ -59,17 +58,17 @@
 Test-driven development can speed up your development very nicely, and can help you engineer your prompts to be more robust.
 
 For example, assuming your prompt looks like this:
 
 ```
 Create some marketing copy for a tweet of less than 280 characters for my app {app_name}.
 
-My app helps people generate sales emails using AI. 
+My app helps people generate sales emails using AI.
 
-Make sure the marketing copy contains a complete and valid link to my app. 
+Make sure the marketing copy contains a complete and valid link to my app.
 
 Here is the link to my app: https://magiklabs.app.
 ```
 
 You can write tests like this:
 
 ```python
@@ -77,59 +76,61 @@
     contains_none,
     contains_link,
     contains_valid_link,
     is_positive_sentiment,
     length_less_than,
 )
 
-
+# Local context - this is used as the "ground truth" data that you can compare against in your tests
+test_context = {}
 
 # Define tests here
-tests = [
-    {
-        "description": "output contains a link",
-        "eval": contains_link(),
-        "prompt_vars": {
-            "app_name": "Uber",
+def define_tests(context: dict):
+    return [
+        {
+            "description": "output contains a link",
+            "eval": contains_link(),
+            "prompt_vars": {
+                "app_name": "Uber",
+            },
+            "failure_labels": ["bad_response_format"],
         },
-        "failure_labels": ["bad_response_format"],
-    },
-    {
-        "description": "output contains a valid link",
-        "eval": contains_valid_link(),
-        "prompt_vars": {
-            "app_name": "Magik",
+        {
+            "description": "output contains a valid link",
+            "eval": contains_valid_link(),
+            "prompt_vars": {
+                "app_name": "Magik",
+            },
+            "failure_labels": ["bad_response_format"],
         },
-        "failure_labels": ["bad_response_format"],
-    },
-    {
-        "description": "output sentiment is positive",
-        "eval": is_positive_sentiment(),
-        "prompt_vars": {
-            "app_name": "Lyft",
+        {
+            "description": "output sentiment is positive",
+            "eval": is_positive_sentiment(),
+            "prompt_vars": {
+                "app_name": "Lyft",
+            },
+            "failure_labels": ["negative_sentiment"],
         },
-        "failure_labels": ["negative_sentiment"],
-    },
-    {
-        "description": "output length is less than 280 characters",
-        "eval": length_less_than(280),
-        "prompt_vars": {
-            "app_name": "Facebook",
+        {
+            "description": "output length is less than 280 characters",
+            "eval": length_less_than(280),
+            "prompt_vars": {
+                "app_name": "Facebook",
+            },
+            "failure_labels": ["negative_sentiment", "critical"],
         },
-        "failure_labels": ["negative_sentiment", "critical"],
-    },
-    {
-        "description": "output does not contain hashtags",
-        "eval": contains_none(['#']),
-        "prompt_vars": {
-            "app_name": "Datadog",
+        {
+            "description": "output does not contain hashtags",
+            "eval": contains_none(['#']),
+            "prompt_vars": {
+                "app_name": "Datadog",
+            },
+            "failure_labels": ["bad_response_format"],
         },
-        "failure_labels": ["bad_response_format"],
-    },
-]
+    ]
 ```
 
 <br /><br />
 
 ### If you have an LLM app in production:
 
 ---
@@ -144,15 +145,14 @@
 
 - Filter by failure labels, severity, prompt, etc to identify different types of errors that are occurring in your LLM outputs.
 
 See https://magiklabs.app for more details, or contact us at [hello@magiklabs.app](mailto:hello@magiklabs.app)
 
 <br /><br />
 
-
 ### Upcoming Features
 
 ---
 
 Soon, you will also be able to:
 
 - Fail bad outputs before they get to your users.
```

### Comparing `magik-0.2.2/magik/classifier.py` & `magik-0.2.5/magik/classifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from magik.openai_helper import OpenAI
+from .openai_helper import OpenAI
 
 classifier_prompt = """
 You are acting as a classifier. 
 I want you to classify this output into one of the classification labels I am describing.
 I am giving you the classification labels along with a description of the label.
 
 Use the description to understand what each label means.
```

### Comparing `magik-0.2.2/magik/cli.py` & `magik-0.2.5/magik/cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python3
 
 import argparse
-from magik.initialize import initialize
-from magik.generate import generate_test
-from magik.deploy import deploy_test
-from magik.internal_logger import logger
-from magik.constants import TEST_DIR, TEST_RUNS_DIR
-from magik.run import Run
+from .initialize import initialize
+from .generate import generate_test
+from .deploy import deploy_test
+from .internal_logger import logger
+from .constants import TEST_DIR, TEST_RUNS_DIR
+from .run import Run
 
 
 def main():
     parser = argparse.ArgumentParser(
         prog="magik", description="Magik testing suite CLI tool"
     )
 
@@ -24,14 +24,24 @@
     parser_generate = subparsers.add_parser("generate", help="Generate a new test")
     parser_generate.add_argument("test_name", help="Name of the test")
     parser_generate.set_defaults(func=generate)
 
     # magik run <test-name>
     parser_run = subparsers.add_parser("run", help="Run a test")
     parser_run.add_argument("test_name", help="Name of the test")
+    parser_run.add_argument("--model", dest="model", help="Name of the LLM")
+    parser_run.add_argument(
+        "--response", dest="response", help="prompt response generated by the llm"
+    )
+    parser_run.add_argument(
+        "--n", dest="number_of_runs", help="number of times to run each test run"
+    )
+    parser_run.add_argument(
+        "--csv", dest="csv_file_path", help="CSV file to store results in"
+    )
     parser_run.set_defaults(func=run)
 
     # magik deploy <test-name>
     parser_deploy = subparsers.add_parser("deploy", help="Deploy a test")
     parser_deploy.add_argument("test_name", help="Name of the test")
     parser_deploy.set_defaults(func=deploy)
 
@@ -59,15 +69,25 @@
 
 def generate(args):
     generate_test(args.test_name)
 
 
 def run(args):
     test_runner = Run(test_dir=TEST_DIR, test_runs_dir=TEST_RUNS_DIR)
-    test_runner.run_tests(args.test_name)
+    number_of_runs = int(args.number_of_runs) if args.number_of_runs else 1
+    model = args.model if args.model else "gpt-3.5-turbo"
+    response = args.response if args.response else None
+    csv_file_path = args.csv_file_path if args.csv_file_path else None
+    test_runner.run_tests(
+        args.test_name,
+        model=model,
+        response=response,
+        number_of_runs=number_of_runs,
+        csv_file_path=csv_file_path,
+    )
 
 
 def deploy(args):
     deploy_test(args.test_name)
 
 
 def run_prod(args):
```

### Comparing `magik-0.2.2/magik/constants.py` & `magik-0.2.5/magik/constants.py`

 * *Files identical despite different names*

### Comparing `magik-0.2.2/magik/decorators.py` & `magik-0.2.5/magik/decorators.py`

 * *Files identical despite different names*

### Comparing `magik-0.2.2/magik/deploy.py` & `magik-0.2.5/magik/deploy.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import json
 import os
 import requests
-from magik.internal_logger import logger
-from magik.constants import CONFIG_FILE_PATH, DEPLOY_URL, TEST_DIR, TEST_RUNS_DIR
-from magik.run import Run
-from magik.config import get_magik_api_key
+from .internal_logger import logger
+from .constants import CONFIG_FILE_PATH, DEPLOY_URL, TEST_DIR, TEST_RUNS_DIR
+from .run import Run
+from .config import get_magik_api_key
 
 
 def deploy_test(test_name: str):
     api_key = get_magik_api_key()
     if api_key == None:
-        logger.error(f"No API key found. Please add your API key to {CONFIG_FILE_PATH}")
+        logger.error(
+            f"No API key found. Please add your API key to {CONFIG_FILE_PATH}")
 
     # construct the file path
     file_path = f"{TEST_DIR}/{test_name}/assertions.py"
 
     # check if the file exists
     if not os.path.isfile(file_path):
         logger.info(f"No assertions.py file found for test_name {test_name}")
@@ -23,19 +24,23 @@
     # read file
     with open(file_path, "rb") as f:
         file_content = f.read()
 
     # prepare data for API request
     test_runner = Run(test_dir=TEST_DIR, test_runs_dir=TEST_RUNS_DIR)
     test_context = test_runner._load_context(test_name)
-    tests = test_runner._load_tests(test_name=test_name, test_context=test_context)
-    tests = list(map(lambda test: {**test, "eval": test["eval"].__name__}, tests))
+    test_suite = test_runner._load_test_suite(
+        test_name=test_name, test_context=test_context
+    )
+    test_suite = list(
+        map(lambda test: {**test, "eval": test["eval"].__name__}, test_suite)
+    )
 
     headers = {"magik-api-key": api_key}
-    data = {"test_slug": test_name, "test_data": tests}
+    data = {"test_slug": test_name, "test_data": test_suite}
     files = {
         "file": ("assertions.py", file_content, "application/octet-stream"),
         "json": (None, json.dumps(data), "application/json"),
     }
 
     # make a POST request to the API
     response = requests.post(DEPLOY_URL, files=files, headers=headers)
```

### Comparing `magik-0.2.2/magik/evaluators.py` & `magik-0.2.5/magik/evaluators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Contains functions to evaluate assertions.
 import requests
 import json
 import re
 import ast
 import numpy as np
-from magik.openai_helper import OpenAI
-from magik.utils import standardize_url, generate_grading_prompt
-from magik.constants import OPEN_AI_DEFAULT_MODEL
-from magik.decorators import magik_eval
-from magik.similarity import similarity_score
-from magik.classifier import classify_output
+from .openai_helper import OpenAI
+from .utils import standardize_url, generate_grading_prompt
+from .constants import OPEN_AI_DEFAULT_MODEL
+from .decorators import magik_eval
+from .similarity import similarity_score
+from .classifier import classify_output
 
 
 @magik_eval
 def equals(expected_output, case_sensitive=False, output_to_test=None):
     if case_sensitive == False:
         output_to_test = output_to_test.lower()
         expected_output = expected_output.lower()
@@ -214,26 +214,26 @@
         If the string has a negative sentiment, then the test passed. Otherwise, the test failed.
     """
     return grade_using_llm(sentiment_grading_prompt)(output_to_test)
 
 
 @magik_eval
 def contains_pii(output_to_test=None):
-    sentiment_grading_prompt = """
+    pii_grading_prompt = """
         If the string contains information that looks like personally identifiable information, then the test passed. Otherwise, the test failed.
     """
-    return grade_using_llm(sentiment_grading_prompt)(output_to_test)
+    return grade_using_llm(pii_grading_prompt)(output_to_test)
 
 
 @magik_eval
 def not_contains_pii(output_to_test=None):
-    sentiment_grading_prompt = """
+    pii_grading_prompt = """
         If the string contains information that looks like personally identifiable information, then the test failed. Otherwise, the test passed.
     """
-    return grade_using_llm(sentiment_grading_prompt)(output_to_test)
+    return grade_using_llm(pii_grading_prompt)(output_to_test)
 
 
 @magik_eval
 def contains_link(output_to_test=None):
     pattern = r"(?!.*@)(?:https?://)?(?:www\.)?\S+\.\S+"
     result = bool(re.search(pattern, output_to_test))
     if result:
```

### Comparing `magik-0.2.2/magik/examples/assertions.py` & `magik-0.2.5/magik/examples/assertions.py`

 * *Files identical despite different names*

### Comparing `magik-0.2.2/magik/generate.py` & `magik-0.2.5/magik/generate.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from magik.internal_logger import logger
-from magik.constants import TEST_DIR
-from magik.sys_exec import read_from_file, write_to_file
-from magik.constants import EXAMPLES_DIR
+from .internal_logger import logger
+from .constants import TEST_DIR
+from .sys_exec import read_from_file, write_to_file
+from .constants import EXAMPLES_DIR
 import inspect
 
 
 # Get the path of the file within the module
 def _get_module_file_path(file_name):
     module = inspect.getmodule(_get_module_file_path)
     module_file_path = inspect.getfile(module)
-    module_dir = module_file_path.rpartition("/")[0]  # Extract the directory path
+    module_dir = module_file_path.rpartition(
+        "/")[0]  # Extract the directory path
     file_path = module_dir + "/" + file_name  # Combine with the file name
     return file_path
 
 
 def _generate_example_prompt(test_path):
     example_prompt = (
         "Write a tweet about my new app named {app_name}. Make sure to include a link."
```

### Comparing `magik-0.2.2/magik/initialize.py` & `magik-0.2.5/magik/initialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
-from magik.internal_logger import logger
-from magik.sys_exec import write_to_file
-from magik.constants import (
+from .internal_logger import logger
+from .sys_exec import write_to_file
+from .constants import (
     TEST_RUNS_DIR,
     TEST_DIR,
     CONFIG_FILE_PATH,
     SCHEDULE_CONFIG_FILE_PATH,
 )
```

### Comparing `magik-0.2.2/magik/internal_logger.py` & `magik-0.2.5/magik/internal_logger.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 import colorlog
+from typing import Dict, Any
 
 
 class Singleton(type):
-    _instances = {}
+    _instances: Dict[Any, Any] = {}
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
             cls._instances[cls] = super(Singleton, cls).__call__(*args, **kwargs)
         return cls._instances[cls]
 
 
@@ -52,14 +53,27 @@
             "white": "37",
         }
 
         color_code = colors.get(color.lower(), "37")
         formatted_message = f"\033[{color_code}m{message}\033[0m"
         print(formatted_message, *args, **kwargs)
 
+    def to_file(self, output: str, log_file):
+        if log_file is not None:
+            log_file.write(output + "\n")
+            log_file.flush()  # Ensure immediate writing to the file
+
+    def to_file_and_console(self, output: str, log_file=None, color=None):
+        self.to_file(output, log_file)
+
+        if color is not None:
+            logger.log_with_color(output, color)
+        else:
+            logger.info(output)
+
 
 def setup_logger():
     logger = CLIAppLogger("cli_logger", level=logging.INFO)
     return logger
 
 
 # Create a default logger instance
```

### Comparing `magik-0.2.2/magik/logger.py` & `magik-0.2.5/magik/logger.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,61 @@
 import requests
-from magik.constants import API_BASE_URL
-from magik.config import get_magik_api_key
+from .constants import API_BASE_URL
+from .config import get_magik_api_key
 
 
 # Log the request and response from OpenAI chat completion to Magik API
 #
 # prompt_slug: name of the prompt for analytics and grouping
 # messages: "messages" json array sent to OpenAI chat completion
 # model: string id of the language model used
 # chat_completion: "choices" json response from OpenAI chat completion
 def log_open_ai_chat_response(
-    prompt_slug, messages, model, chat_completion, response_time, context
+    prompt_slug, messages, model, chat_completion, response_time=None, context=None
 ):
     """
     Track the request and response.
     """
+    payload = {
+        "prompt_slug": prompt_slug,
+        "prompt_data": messages,
+        "language_model_id": model,
+        "completion": chat_completion,
+        "response_time": response_time,
+        "context": context,
+    }
+    # Remove None fields from the payload
+    payload = {k: v for k, v in payload.items() if v is not None}
     requests.post(
         f"{API_BASE_URL}/api/v1/savePromptAndResponse",
-        json={
-            "prompt_slug": prompt_slug,
-            "prompt_data": messages,
-            "language_model_id": model,
-            "completion": chat_completion,
-            "response_time": response_time,
-            "context": context,
+        json=payload,
+        headers={
+            "magik-api-key": get_magik_api_key(),
+        },
+    )
+
+
+def log_open_ai_completion_response(
+    prompt_slug, message, model, completion, response_time=None, context=None
+):
+    """
+    Track the request and response.
+    """
+    payload = {
+        "prompt_slug": prompt_slug,
+        "prompt_data": {
+            "text": message
         },
+        "language_model_id": model,
+        "completion": completion,
+        "response_time": response_time,
+        "context": context,
+    }
+    # Remove None fields from the payload
+    payload = {k: v for k, v in payload.items() if v is not None}
+    requests.post(
+        f"{API_BASE_URL}/api/v1/savePromptAndResponse",
+        json=payload,
         headers={
             "magik-api-key": get_magik_api_key(),
         },
     )
```

### Comparing `magik-0.2.2/magik/similarity.py` & `magik-0.2.5/magik/similarity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from magik.openai_helper import OpenAI
+from .openai_helper import OpenAI
 
 
 # Similarity score
 def _cosine_similarity_from_embeddings(e1: list[float], e2: list[float]) -> float:
     # Convert the embedding lists to numpy arrays
     v1 = np.array(e1)
     v2 = np.array(e2)
```

### Comparing `magik-0.2.2/magik/sys_exec.py` & `magik-0.2.5/magik/sys_exec.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import asyncio
 import os
 import json
 import subprocess
-from magik.internal_logger import logger
+from .internal_logger import logger
 
 
 def execute_command(command, confirm=True, log=True):
     if confirm:
         confirmation = input(f"Run '{command}'? (y/n)")
         if confirmation != "y":
             return
 
-    result = subprocess.run(command, shell=True, capture_output=True, text=True)
+    result = subprocess.run(command, shell=True,
+                            capture_output=True, text=True)
 
     if result.returncode == 0:
         if log:
             logger.info(command)
         output = result.stdout
         if log:
             logger.info(output)
@@ -65,15 +66,16 @@
 
 
 def create_file(filepath):
     directory = os.path.dirname(filepath)
     os.makedirs(
         directory, exist_ok=True
     )  # Create parent directories if they don't exist
-    open(filepath, "a").close()  # Create an empty file at the specified filepath
+    # Create an empty file at the specified filepath
+    open(filepath, "a").close()
 
 
 def touch(file_path, confirm=False):
     execute_command(f"touch {file_path}", confirm=confirm)
 
 
 def write_to_file(file_path, content):
```

### Comparing `magik-0.2.2/magik/utils.py` & `magik-0.2.5/magik/utils.py`

 * *Files identical despite different names*

### Comparing `magik-0.2.2/magik.egg-info/PKG-INFO` & `magik-0.2.5/magik.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magik
-Version: 0.2.2
+Version: 0.2.5
 Summary: SDK to write and run tests for your LLM app
 Home-page: UNKNOWN
 Author: Magik Labs Team
 Author-email: hello@magiklabs.app
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -18,35 +18,34 @@
 
 # Overview
 
 Reliability of output is one of the biggest challenges for people trying to use LLM apps in production.<br />
 
 Since LLM outputs are non-deterministic, it’s very hard to measure how good the output is.
 
-Eyeballing the responses from an LLM can work in development, but it’s not a great solution. 
+Eyeballing the responses from an LLM can work in development, but it’s not a great solution.
 
 > _In production, it’s virtually impossible to eyeball thousands of responses. Which means you have very little visibility into how well your LLM is performing._
 
 - Do you know when your LLM app is hallucinating?
-- How do you know how well it's *really* performing?
+- How do you know how well it's _really_ performing?
 - Do you know how often it’s producing a critically bad output?
 - How do you know what your users are seeing?
 - How do you measure how good your LLM responses are? And if you can’t measure it, how do you improve the accuracy?
 
 <br />
 
 > If these sound like problems to you (today or in the future), please reach out to us at hello@magiklabs.app. We’d love to hear more!
 
 <img width="1576" alt="llm-screenshot-1" src="https://github.com/magiklabs/magik-sdk/assets/7515552/bc87aefa-505f-4732-84cd-b7fe57857850">
 
-
 <br /><br /><br />
 
-
 # Documentation
+
 `pip install magik`
 
 See https://docs.magiklabs.app for instructions on how to write and run tests.
 
 - [Overview](https://docs.magiklabs.app/)
 - [Quick Start](https://docs.magiklabs.app/quick-start)
 - [Writing Tests](https://docs.magiklabs.app/reference/writing-tests)
@@ -74,17 +73,17 @@
 Test-driven development can speed up your development very nicely, and can help you engineer your prompts to be more robust.
 
 For example, assuming your prompt looks like this:
 
 ```
 Create some marketing copy for a tweet of less than 280 characters for my app {app_name}.
 
-My app helps people generate sales emails using AI. 
+My app helps people generate sales emails using AI.
 
-Make sure the marketing copy contains a complete and valid link to my app. 
+Make sure the marketing copy contains a complete and valid link to my app.
 
 Here is the link to my app: https://magiklabs.app.
 ```
 
 You can write tests like this:
 
 ```python
@@ -92,59 +91,61 @@
     contains_none,
     contains_link,
     contains_valid_link,
     is_positive_sentiment,
     length_less_than,
 )
 
-
+# Local context - this is used as the "ground truth" data that you can compare against in your tests
+test_context = {}
 
 # Define tests here
-tests = [
-    {
-        "description": "output contains a link",
-        "eval": contains_link(),
-        "prompt_vars": {
-            "app_name": "Uber",
+def define_tests(context: dict):
+    return [
+        {
+            "description": "output contains a link",
+            "eval": contains_link(),
+            "prompt_vars": {
+                "app_name": "Uber",
+            },
+            "failure_labels": ["bad_response_format"],
         },
-        "failure_labels": ["bad_response_format"],
-    },
-    {
-        "description": "output contains a valid link",
-        "eval": contains_valid_link(),
-        "prompt_vars": {
-            "app_name": "Magik",
+        {
+            "description": "output contains a valid link",
+            "eval": contains_valid_link(),
+            "prompt_vars": {
+                "app_name": "Magik",
+            },
+            "failure_labels": ["bad_response_format"],
         },
-        "failure_labels": ["bad_response_format"],
-    },
-    {
-        "description": "output sentiment is positive",
-        "eval": is_positive_sentiment(),
-        "prompt_vars": {
-            "app_name": "Lyft",
+        {
+            "description": "output sentiment is positive",
+            "eval": is_positive_sentiment(),
+            "prompt_vars": {
+                "app_name": "Lyft",
+            },
+            "failure_labels": ["negative_sentiment"],
         },
-        "failure_labels": ["negative_sentiment"],
-    },
-    {
-        "description": "output length is less than 280 characters",
-        "eval": length_less_than(280),
-        "prompt_vars": {
-            "app_name": "Facebook",
+        {
+            "description": "output length is less than 280 characters",
+            "eval": length_less_than(280),
+            "prompt_vars": {
+                "app_name": "Facebook",
+            },
+            "failure_labels": ["negative_sentiment", "critical"],
         },
-        "failure_labels": ["negative_sentiment", "critical"],
-    },
-    {
-        "description": "output does not contain hashtags",
-        "eval": contains_none(['#']),
-        "prompt_vars": {
-            "app_name": "Datadog",
+        {
+            "description": "output does not contain hashtags",
+            "eval": contains_none(['#']),
+            "prompt_vars": {
+                "app_name": "Datadog",
+            },
+            "failure_labels": ["bad_response_format"],
         },
-        "failure_labels": ["bad_response_format"],
-    },
-]
+    ]
 ```
 
 <br /><br />
 
 ### If you have an LLM app in production:
 
 ---
@@ -159,15 +160,14 @@
 
 - Filter by failure labels, severity, prompt, etc to identify different types of errors that are occurring in your LLM outputs.
 
 See https://magiklabs.app for more details, or contact us at [hello@magiklabs.app](mailto:hello@magiklabs.app)
 
 <br /><br />
 
-
 ### Upcoming Features
 
 ---
 
 Soon, you will also be able to:
 
 - Fail bad outputs before they get to your users.
```

### Comparing `magik-0.2.2/magik.egg-info/SOURCES.txt` & `magik-0.2.5/magik.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -9,20 +9,25 @@
 magik/deploy.py
 magik/evaluators.py
 magik/generate.py
 magik/initialize.py
 magik/internal_logger.py
 magik/logger.py
 magik/matchers.py
+magik/metrics.py
 magik/openai_helper.py
 magik/run.py
+magik/run_logger.py
 magik/similarity.py
 magik/sys_exec.py
+magik/test_loader.py
 magik/utils.py
 magik.egg-info/PKG-INFO
 magik.egg-info/SOURCES.txt
 magik.egg-info/dependency_links.txt
 magik.egg-info/entry_points.txt
 magik.egg-info/requires.txt
 magik.egg-info/top_level.txt
 magik/examples/__init__.py
-magik/examples/assertions.py
+magik/examples/assertions.py
+magik/types/__init__.py
+magik/types/test_run.py
```

### Comparing `magik-0.2.2/setup.py` & `magik-0.2.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="magik",
-    version="0.2.2",
+    version="0.2.5",
     author="Magik Labs Team",
     author_email="hello@magiklabs.app",
     description="SDK to write and run tests for your LLM app",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=requirements,
```

