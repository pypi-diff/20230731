# Comparing `tmp/gitlab_sdk-0.1.0.tar.gz` & `tmp/gitlab_sdk-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab_sdk-0.1.0.tar", last modified: Mon Jul 31 08:30:46 2023, max compression
+gzip compressed data, was "gitlab_sdk-0.2.0.tar", last modified: Mon Jul 31 13:20:14 2023, max compression
```

## Comparing `gitlab_sdk-0.1.0.tar` & `gitlab_sdk-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ankit      (501) staff       (20)        0 2023-07-31 08:30:46.228842 gitlab_sdk-0.1.0/
--rw-r--r--   0 ankit      (501) staff       (20)      277 2023-07-31 08:30:46.228703 gitlab_sdk-0.1.0/PKG-INFO
--rw-r--r--   0 ankit      (501) staff       (20)     2714 2023-07-31 08:21:16.000000 gitlab_sdk-0.1.0/README.md
-drwxr-xr-x   0 ankit      (501) staff       (20)        0 2023-07-31 08:30:46.227420 gitlab_sdk-0.1.0/gitlab_sdk/
--rw-r--r--   0 ankit      (501) staff       (20)       81 2023-07-31 08:21:16.000000 gitlab_sdk-0.1.0/gitlab_sdk/__init__.py
--rw-r--r--   0 ankit      (501) staff       (20)      123 2023-07-31 08:21:16.000000 gitlab_sdk-0.1.0/gitlab_sdk/_version.py
--rw-r--r--   0 ankit      (501) staff       (20)     1838 2023-07-31 08:21:16.000000 gitlab_sdk-0.1.0/gitlab_sdk/client.py
-drwxr-xr-x   0 ankit      (501) staff       (20)        0 2023-07-31 08:30:46.228244 gitlab_sdk-0.1.0/gitlab_sdk.egg-info/
--rw-r--r--   0 ankit      (501) staff       (20)      277 2023-07-31 08:30:46.000000 gitlab_sdk-0.1.0/gitlab_sdk.egg-info/PKG-INFO
--rw-r--r--   0 ankit      (501) staff       (20)      293 2023-07-31 08:30:46.000000 gitlab_sdk-0.1.0/gitlab_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 ankit      (501) staff       (20)        1 2023-07-31 08:30:46.000000 gitlab_sdk-0.1.0/gitlab_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 ankit      (501) staff       (20)       24 2023-07-31 08:30:46.000000 gitlab_sdk-0.1.0/gitlab_sdk.egg-info/requires.txt
--rw-r--r--   0 ankit      (501) staff       (20)       17 2023-07-31 08:30:46.000000 gitlab_sdk-0.1.0/gitlab_sdk.egg-info/top_level.txt
--rw-r--r--   0 ankit      (501) staff       (20)       38 2023-07-31 08:30:46.228885 gitlab_sdk-0.1.0/setup.cfg
--rw-r--r--   0 ankit      (501) staff       (20)      438 2023-07-31 08:21:16.000000 gitlab_sdk-0.1.0/setup.py
-drwxr-xr-x   0 ankit      (501) staff       (20)        0 2023-07-31 08:30:46.228516 gitlab_sdk-0.1.0/tests/
--rw-r--r--   0 ankit      (501) staff       (20)        0 2023-07-31 08:21:16.000000 gitlab_sdk-0.1.0/tests/__init__.py
--rw-r--r--   0 ankit      (501) staff       (20)     2424 2023-07-31 08:21:16.000000 gitlab_sdk-0.1.0/tests/test_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 13:20:14.299667 gitlab_sdk-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)      322 2023-07-31 13:20:14.298667 gitlab_sdk-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3214 2023-07-31 13:20:01.000000 gitlab_sdk-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 13:20:14.297666 gitlab_sdk-0.2.0/gitlab_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-07-31 13:20:01.000000 gitlab_sdk-0.2.0/gitlab_sdk/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-07-31 13:20:01.000000 gitlab_sdk-0.2.0/gitlab_sdk/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     1838 2023-07-31 13:20:01.000000 gitlab_sdk-0.2.0/gitlab_sdk/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 13:20:14.298667 gitlab_sdk-0.2.0/gitlab_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      322 2023-07-31 13:20:14.000000 gitlab_sdk-0.2.0/gitlab_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      293 2023-07-31 13:20:14.000000 gitlab_sdk-0.2.0/gitlab_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 13:20:14.000000 gitlab_sdk-0.2.0/gitlab_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-31 13:20:14.000000 gitlab_sdk-0.2.0/gitlab_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-31 13:20:14.000000 gitlab_sdk-0.2.0/gitlab_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 13:20:14.299667 gitlab_sdk-0.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      438 2023-07-31 13:20:01.000000 gitlab_sdk-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 13:20:14.298667 gitlab_sdk-0.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-31 13:20:01.000000 gitlab_sdk-0.2.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2424 2023-07-31 13:20:01.000000 gitlab_sdk-0.2.0/tests/test_client.py
```

### Comparing `gitlab_sdk-0.1.0/README.md` & `gitlab_sdk-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -20,58 +20,59 @@
 from gitlab_sdk import Client
 
 client = Client(app_id='YOUR_APP_ID', host='YOUR_HOST')
 ```
 
 ## Client initialization options
 
-| Option          | Description                                                                                                                               |
-|:----------------|:------------------------------------------------------------------------------------------------------------------------------------------|
+| Option   | Description                                                                                                            |
+| :------- | :--------------------------------------------------------------------------------------------------------------------- |
 | `app_id` | The ID specified in the GitLab Project Analytics setup guide. It ensures your data is sent to your analytics instance. |
-| `host`          | The GitLab Project Analytics instance specified in the setup guide.                                                           |
+| `host`   | The GitLab Project Analytics instance specified in the setup guide.                                                    |
 
 ## Methods
 
 ### `identify`
 
 Used to associate a user and their attributes with the session and tracking events.
 
 ```python
 client.identify(user_id='123abc', user_attributes={ "user_name": "Matthew" })
 ```
 
-| Property         | Type     | Description                                                                   |
-|:-----------------|:---------|:------------------------------------------------------------------------------|
-| `user_id`         | `String` | The ID of the user.      |
+| Property          | Type         | Description                                                              |
+| :---------------- | :----------- | :----------------------------------------------------------------------- |
+| `user_id`         | `String`     | The ID of the user.                                                      |
 | `user_attributes` | `Dictionary` | Optional. The user attributes to add to the session and tracking events. |
 
 ### `track`
 
 Used to trigger a custom event.
 
 ```python
 client.track(event_name=event_name, event_payload=event_payload)
 ```
 
-| Property          | Type      | Description                                                      |
-|:------------------|:----------|:-----------------------------------------------------------------|
-| `event_name`       | `String` | The name of the event.                                           |
-| `event_payload`    | `Dictionary`   | The event attributes to add to the tracked event. |
+| Property        | Type         | Description                                       |
+| :-------------- | :----------- | :------------------------------------------------ |
+| `event_name`    | `String`     | The name of the event.                            |
+| `event_payload` | `Dictionary` | The event attributes to add to the tracked event. |
 
 ## Developing with the devkit
 
 To develop with a local Snowplow pipeline, use Analytics devkit's [Snowplow setup](https://gitlab.com/gitlab-org/analytics-section/product-analytics/devkit/-/tree/main#setup).
 
-
 To run development libraries, run:
+
 ```bash
 pip install -r requirements-dev.txt
 ```
 
 and run:
+
 ```bash
 make -i python-linter
 
 # for help, run:
 # make help
 ```
 
@@ -80,10 +81,35 @@
 To run the test suite, first install the required packages:
 
 ```bash
 pip install -r requirements-test.txt
 ```
 
 And then, execute the tests:
+
 ```bash
 pytest
 ```
+
+### Developer guidelines
+
+##### Releasing New Versions:
+
+When you want your changes to trigger a new release upon being merged to `master`, your commit message should include specific keywords:
+
+1. Major Release: For backward-incompatible changes that require a major version bump.
+
+   ```
+   [major] Description of the change.
+   ```
+
+2. Minor Release: For backward-compatible new features.
+
+   ```
+   [minor] Description of the new feature.
+   ```
+
+3. Patch Release: For backward-compatible bug fixes.
+
+   ```
+   [patch] Description of the bug fix.
+   ```
```

### Comparing `gitlab_sdk-0.1.0/gitlab_sdk/client.py` & `gitlab_sdk-0.2.0/gitlab_sdk/client.py`

 * *Files identical despite different names*

### Comparing `gitlab_sdk-0.1.0/tests/test_client.py` & `gitlab_sdk-0.2.0/tests/test_client.py`

 * *Files identical despite different names*

