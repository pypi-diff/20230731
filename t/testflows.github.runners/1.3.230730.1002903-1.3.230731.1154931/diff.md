# Comparing `tmp/testflows.github.runners-1.3.230730.1002903.tar.gz` & `tmp/testflows.github.runners-1.3.230731.1154931.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.3.230730.1002903.tar", last modified: Sun Jul 30 00:29:03 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.3.230731.1154931.tar", last modified: Mon Jul 31 15:49:31 2023, max compression
```

## Comparing `testflows.github.runners-1.3.230730.1002903.tar` & `testflows.github.runners-1.3.230731.1154931.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-30 00:29:03.262535 testflows.github.runners-1.3.230730.1002903/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230730.1002903/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    47832 2023-07-30 00:29:03.262535 testflows.github.runners-1.3.230730.1002903/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    47240 2023-07-30 00:22:54.000000 testflows.github.runners-1.3.230730.1002903/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-30 00:29:03.262535 testflows.github.runners-1.3.230730.1002903/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-30 00:29:03.000000 testflows.github.runners-1.3.230730.1002903/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-30 00:29:03.258535 testflows.github.runners-1.3.230730.1002903/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-30 00:29:03.258535 testflows.github.runners-1.3.230730.1002903/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-30 00:29:03.262535 testflows.github.runners-1.3.230730.1002903/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-30 00:29:03.000000 testflows.github.runners-1.3.230730.1002903/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1615 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230730.1002903/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     2491 2023-07-29 22:10:17.000000 testflows.github.runners-1.3.230730.1002903/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-30 00:29:03.262535 testflows.github.runners-1.3.230730.1002903/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    23217 2023-07-29 23:28:28.000000 testflows.github.runners-1.3.230730.1002903/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)    13607 2023-07-29 23:57:40.000000 testflows.github.runners-1.3.230730.1002903/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     4008 2023-07-29 23:57:15.000000 testflows.github.runners-1.3.230730.1002903/testflows/github/runners/config.py
--rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.3.230730.1002903/testflows/github/runners/delete.py
--rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230730.1002903/testflows/github/runners/logger.py
--rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.3.230730.1002903/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)    10814 2023-07-29 23:14:39.000000 testflows.github.runners-1.3.230730.1002903/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    16705 2023-07-29 20:55:15.000000 testflows.github.runners-1.3.230730.1002903/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-30 00:29:03.262535 testflows.github.runners-1.3.230730.1002903/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230730.1002903/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-30 00:29:03.262535 testflows.github.runners-1.3.230730.1002903/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230730.1002903/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230730.1002903/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230730.1002903/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230730.1002903/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230730.1002903/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2522 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230730.1002903/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     5122 2023-07-29 20:55:15.000000 testflows.github.runners-1.3.230730.1002903/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230730.1002903/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-30 00:29:03.258535 testflows.github.runners-1.3.230730.1002903/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    47832 2023-07-30 00:29:03.000000 testflows.github.runners-1.3.230730.1002903/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1105 2023-07-30 00:29:03.000000 testflows.github.runners-1.3.230730.1002903/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-30 00:29:03.000000 testflows.github.runners-1.3.230730.1002903/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.3.230730.1002903/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-30 00:29:03.000000 testflows.github.runners-1.3.230730.1002903/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-30 00:29:03.000000 testflows.github.runners-1.3.230730.1002903/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 15:49:31.399552 testflows.github.runners-1.3.230731.1154931/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1154931/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    49039 2023-07-31 15:49:31.399552 testflows.github.runners-1.3.230731.1154931/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    48447 2023-07-31 15:49:25.000000 testflows.github.runners-1.3.230731.1154931/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-31 15:49:31.399552 testflows.github.runners-1.3.230731.1154931/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-31 15:49:31.000000 testflows.github.runners-1.3.230731.1154931/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 15:49:31.395552 testflows.github.runners-1.3.230731.1154931/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 15:49:31.395552 testflows.github.runners-1.3.230731.1154931/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 15:49:31.399552 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-31 15:49:31.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1615 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2599 2023-07-31 15:05:55.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 15:49:31.399552 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    23381 2023-07-31 15:15:18.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)    13607 2023-07-29 23:57:40.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4164 2023-07-31 15:16:54.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/config.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/delete.py
+-rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/logger.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10814 2023-07-29 23:14:39.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16903 2023-07-31 15:02:38.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 15:49:31.399552 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 15:49:31.399552 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scripts/setup_docker.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2522 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5122 2023-07-29 20:55:15.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 15:49:31.395552 testflows.github.runners-1.3.230731.1154931/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    49039 2023-07-31 15:49:31.000000 testflows.github.runners-1.3.230731.1154931/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1154 2023-07-31 15:49:31.000000 testflows.github.runners-1.3.230731.1154931/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-31 15:49:31.000000 testflows.github.runners-1.3.230731.1154931/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.3.230731.1154931/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-31 15:49:31.000000 testflows.github.runners-1.3.230731.1154931/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-31 15:49:31.000000 testflows.github.runners-1.3.230731.1154931/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.3.230730.1002903/LICENSE` & `testflows.github.runners-1.3.230731.1154931/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230730.1002903/PKG-INFO` & `testflows.github.runners-1.3.230731.1154931/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.3.230730.1002903
+Version: 1.3.230731.1154931
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -12,16 +12,16 @@
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
 .. image:: https://raw.githubusercontent.com/testflows/TestFlows-ArtWork/master/images/logo.png
-   :width: 20%
-   :align: left
+   :width: 300px
+   :align: center
    :target: https://testflows.com
    :alt: TestFlows Open-source Testing Framework
 
 ----
 
 :PyPi:
    `Versions <https://pypi.org/project/testflows.github.runners/>`_
@@ -34,15 +34,21 @@
 
 A simple alternative to Github's `Recommended autoscaling solutions <https://docs.github.com/en/actions/hosting-your-own-runners/managing-self-hosted-runners/autoscaling-with-self-hosted-runners#recommended-autoscaling-solutions>`_.
 
 The **github-runners** service program starts and monitors queued up jobs for GitHub Actions workflows.
 When a new job is queued up, it creates a new Hetzner Cloud server instance
 that provides an ephemeral GitHub Actions runner. Each server instance is automatically
 powered off when job completes and then powered off servers are
-automatically deleted. Both **x64** and **arm64** runners are supported.
+automatically deleted. Both **x64** (*x86*) and **arm64** (*arm*) runners are supported.
+See `Features`_ and `Limitations`_ for more details.
+
+.. image:: https://raw.githubusercontent.com/testflows/TestFlows-GitHub-Runners/master/intro.gif
+   :align: center
+   :alt: TestFlows GitHub Runners
+
 
 :❗Warning:
    This program is provided on "AS IS" basis without warranties or conditions of any kind. See LICENSE.
    Use it at your own risk. Manual monitoring is required to make sure server instances are cleaned up properly
    and costs are kept under control.
 
 Costs depend on the server type, number of jobs and execution time. For each job a new server instance is created
@@ -65,15 +71,18 @@
 Features
 --------
 
 * cost efficient on-demand runners using `Hetzner Cloud <https://www.hetzner.com/cloud>`_
 * simple configuration, no Webhooks, no need for AWS lambdas, and no need to setup any GitHub application
 * supports specifying custom runner server types, images, and locations using job labels
 * self-contained program that you can use to deploy, redeploy, and manage the service on a cloud instance
-* supports both x64 and ARM64 runners
+* supports x64 (x86) and ARM64 (arm) runners
+* supports using any Hetzner Cloud server types
+* supports runners with pre-installed Docker
+* supports using any standard Hetzner Cloud images and applications
 * supports auto-replenishable fixed standby runner pools for jobs to be picked up immediately
 * simpler alternative to what GitHub lists in `Recommended autoscaling solutions <https://docs.github.com/en/actions/hosting-your-own-runners/managing-self-hosted-runners/autoscaling-with-self-hosted-runners#recommended-autoscaling-solutions>`_
 
 ----
 
 -----------
 Limitations
@@ -184,14 +193,39 @@
 
 .. code-block:: bash
 
    github-runners --max-runners 40
 
 ----
 
+-------------------------------
+Jobs That Require Docker Engine
+-------------------------------
+
+For jobs that require Docker to be installed, you can use the standard `Hetzner Docker CE application <https://docs.hetzner.com/cloud/apps/list/docker-ce/>`_
+which can be specified using the **image-** label. See `Specifying Runner Image`_ for more details about specifying custom runner images.
+
+For example
+
+:x64:
+
+   .. code-block:: yaml
+
+      job-name:
+         runs-on: [self-hosted, type-cx11, image-x86-app-docker-ce]
+
+:ARM64:
+
+   .. code-block:: yaml
+
+      job-name:
+         runs-on: [self-hosted, type-cax11, image-arm-app-docker-ce]
+
+----
+
 ----------------------
 Specifying Runner Type
 ----------------------
 
 x64 Runners
 ============
 
@@ -254,44 +288,48 @@
 -----------------------
 Specifying Runner Image
 -----------------------
 
 By default, the default image of the server for the runner is **ubuntu-22.04**. You can use the **--default-image**
 option to force specific default server image.
 
-You can also use the **image-{type}-{name}** runner label to specify server image for a specific job. Where the **{name}** must be a valid
-Hetzner Cloud image such as *ubuntu-22.04* or *ubuntu-20.04*, and the **{type}** is either *system*, *snapshot*, *backup*, or *app*.
+You can also use the **image-{architecture}-{type}-{name}** runner label to specify server image for a specific job.
+
+Where,
+
+* **{architecture}** is either *x86* or *arm*
+* **{type}** is either *system*, *snapshot*, *backup*, or *app*
+* **{name}** must be a valid Hetzner Cloud image name, for *system* or *app* type, such as *ubuntu-22.04*,
+  or a description, for *backup* or *snapshot* type.
 
 For example,
 
 :ubuntu-20.04:
 
    .. code-block:: yaml
 
       job-name:
-         runs-on: [self-hosted, type-cx11, in-ash, image-system-ubuntu-20.04]
+         runs-on: [self-hosted, type-cx11, in-ash, image-x86-system-ubuntu-20.04]
 
 
 :docker-ce app:
-   :✋ Note:
-      Currently Docker CE application does not support ARM64 architecture.
 
    .. code-block:: yaml
 
       job-name:
-         runs-on: [self-hosted, type-cx11, in-ash, image-app-docker-ce]
+         runs-on: [self-hosted, type-cx11, in-ash, image-x86-app-docker-ce]
 
 :snapshot:
    For snapshots, specify **description** as the name. Snapshot descriptions
    must be unique.
 
    .. code-block:: yaml
 
       job-name:
-         runs-on: [self-hosted, type-cx11, in-ash, image-snapshot-snapshot_description]
+         runs-on: [self-hosted, type-cx11, in-ash, image-x86-snapshot-snapshot_description]
 
 ----
 
 --------------------------------------------
 Specifying Custom Runner Server Setup Script
 --------------------------------------------
 
@@ -484,15 +522,15 @@
 
 You can sanity check your configuration file by executing it directly:
 
 .. code-block:: bash
 
    python3 config.py
 
-You can pass your custom configuration file using the *-c path, --config path** command line option.
+You can pass your custom configuration file using the **-c path, --config path** command line option.
 
 .. code-block:: bash
 
    github-runners -c config.py
 
 Configuration Schema
 =====================
@@ -1064,29 +1102,29 @@
 ------------------
 
 The program scales up runners by looking for any jobs that have **queued** status.
 For each such job, a corresponding Hetzner Cloud server instance is created with the following name:
 
 ::
 
-   github-runner-{job.run_id}-{job.id}
+   github-runner-{job.id}
 
 The server is configured using default **setup** and **startup** scripts. The runner name is set
 to be the same as the server name so that servers can be deleted for any unused runner that for some reason
 does not pick up a job for which it was created within the **max-unused-runner-time** period.
 
 :Note:
-   Given that the server name is fixed and specific for each *job.run_id, job.id* tuple, if multiple `github-runners` are running in parallel then
+   Given that the server name is fixed and specific for each *job.id*, if multiple `github-runners` are running in parallel then
    only 1 server will be created for a given `job` and any other attempts to create a server with the same name will be rejected
    by the Hetzner Cloud.
 
 Also,
 
 :Note:
-   There is no guarantee that a given runner will pick the job with the exact **run_id, job.id** tuple that caused it to be created.
+   There is no guarantee that a given runner will pick the job with the exact **job.id** that caused it to be created.
    This is expected and because for each **queued** job a unique runner will be created the number of runners will be
    equal the number of jobs and therefore under normal conditions all jobs will be executed as expected.
 
 ----
 
 Maximum Number of Runners
 =========================
@@ -1125,15 +1163,15 @@
 :Server Location:
 
    The server location can bespecified by using the **--default-location** option or the **in-<name>** runner label.
    By default, location is not set as some server types are not available in some locations.
 
 :Image:
 
-   The server is configured to have the image specified by the **--default-image** option or the **image-{type}-{name}** runner label.
+   The server is configured to have the image specified by the **--default-image** option or the **image-{architecture}-{type}-{name}** runner label.
 
 :SSH Access:
 
    The server is configured to be accessed using *ssh* utility and the SSH public key path is specified using the **--ssh-key**
    option.
 
 :Image Configuration:
@@ -1303,17 +1341,18 @@
 
 * **--default-type name**
   default runner server type name, default: *cx11*
 
 * **--default-location name**
   default runner server location name, default: not specified
 
-* **--default-image type:name_or_description**
+* **--default-image architecture:type:name_or_description**
   default runner server image type and name or description,
-  where type is either: 'system','snapshot','backup','app',
+  where the architecture is either: 'x86' or 'arm',
+  and type is either: 'system','snapshot','backup','app',
   default: *system:ubuntu-22.04*
 
 * **-m count, --max-runners count**
   maximum number of active runners, default: *10*
 
 * **-w count, --workers count**
   number of concurrent workers, default: *10*
@@ -1373,17 +1412,18 @@
 
         * **-l name, --location name**
           deployment server location, default: *ash*
 
         * **-t name, --type name**
           deployment server type, default: *cpx11*
 
-        * **-i type:name_or_description, --image type:name_or_description**
+        * **-i architecture:type:name_or_description, --image architecture:type:name_or_description**
           deployment server image type and name or description,
-          where the type is either: 'system','snapshot','backup','app',
+          where the architecture is either: 'x86' or 'arm',
+          and the type is either: 'system','snapshot','backup','app',
           default: *system:ubuntu-22.04*
 
         * **--setup-script path**
           path to custom deployment server setup script
 
       * **redeploy**
         redeploy on the same cloud service server
```

### Comparing `testflows.github.runners-1.3.230730.1002903/README.rst` & `testflows.github.runners-1.3.230731.1154931/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .. image:: https://raw.githubusercontent.com/testflows/TestFlows-ArtWork/master/images/logo.png
-   :width: 20%
-   :align: left
+   :width: 300px
+   :align: center
    :target: https://testflows.com
    :alt: TestFlows Open-source Testing Framework
 
 ----
 
 :PyPi:
    `Versions <https://pypi.org/project/testflows.github.runners/>`_
@@ -17,15 +17,21 @@
 
 A simple alternative to Github's `Recommended autoscaling solutions <https://docs.github.com/en/actions/hosting-your-own-runners/managing-self-hosted-runners/autoscaling-with-self-hosted-runners#recommended-autoscaling-solutions>`_.
 
 The **github-runners** service program starts and monitors queued up jobs for GitHub Actions workflows.
 When a new job is queued up, it creates a new Hetzner Cloud server instance
 that provides an ephemeral GitHub Actions runner. Each server instance is automatically
 powered off when job completes and then powered off servers are
-automatically deleted. Both **x64** and **arm64** runners are supported.
+automatically deleted. Both **x64** (*x86*) and **arm64** (*arm*) runners are supported.
+See `Features`_ and `Limitations`_ for more details.
+
+.. image:: https://raw.githubusercontent.com/testflows/TestFlows-GitHub-Runners/master/intro.gif
+   :align: center
+   :alt: TestFlows GitHub Runners
+
 
 :❗Warning:
    This program is provided on "AS IS" basis without warranties or conditions of any kind. See LICENSE.
    Use it at your own risk. Manual monitoring is required to make sure server instances are cleaned up properly
    and costs are kept under control.
 
 Costs depend on the server type, number of jobs and execution time. For each job a new server instance is created
@@ -48,15 +54,18 @@
 Features
 --------
 
 * cost efficient on-demand runners using `Hetzner Cloud <https://www.hetzner.com/cloud>`_
 * simple configuration, no Webhooks, no need for AWS lambdas, and no need to setup any GitHub application
 * supports specifying custom runner server types, images, and locations using job labels
 * self-contained program that you can use to deploy, redeploy, and manage the service on a cloud instance
-* supports both x64 and ARM64 runners
+* supports x64 (x86) and ARM64 (arm) runners
+* supports using any Hetzner Cloud server types
+* supports runners with pre-installed Docker
+* supports using any standard Hetzner Cloud images and applications
 * supports auto-replenishable fixed standby runner pools for jobs to be picked up immediately
 * simpler alternative to what GitHub lists in `Recommended autoscaling solutions <https://docs.github.com/en/actions/hosting-your-own-runners/managing-self-hosted-runners/autoscaling-with-self-hosted-runners#recommended-autoscaling-solutions>`_
 
 ----
 
 -----------
 Limitations
@@ -167,14 +176,39 @@
 
 .. code-block:: bash
 
    github-runners --max-runners 40
 
 ----
 
+-------------------------------
+Jobs That Require Docker Engine
+-------------------------------
+
+For jobs that require Docker to be installed, you can use the standard `Hetzner Docker CE application <https://docs.hetzner.com/cloud/apps/list/docker-ce/>`_
+which can be specified using the **image-** label. See `Specifying Runner Image`_ for more details about specifying custom runner images.
+
+For example
+
+:x64:
+
+   .. code-block:: yaml
+
+      job-name:
+         runs-on: [self-hosted, type-cx11, image-x86-app-docker-ce]
+
+:ARM64:
+
+   .. code-block:: yaml
+
+      job-name:
+         runs-on: [self-hosted, type-cax11, image-arm-app-docker-ce]
+
+----
+
 ----------------------
 Specifying Runner Type
 ----------------------
 
 x64 Runners
 ============
 
@@ -237,44 +271,48 @@
 -----------------------
 Specifying Runner Image
 -----------------------
 
 By default, the default image of the server for the runner is **ubuntu-22.04**. You can use the **--default-image**
 option to force specific default server image.
 
-You can also use the **image-{type}-{name}** runner label to specify server image for a specific job. Where the **{name}** must be a valid
-Hetzner Cloud image such as *ubuntu-22.04* or *ubuntu-20.04*, and the **{type}** is either *system*, *snapshot*, *backup*, or *app*.
+You can also use the **image-{architecture}-{type}-{name}** runner label to specify server image for a specific job.
+
+Where,
+
+* **{architecture}** is either *x86* or *arm*
+* **{type}** is either *system*, *snapshot*, *backup*, or *app*
+* **{name}** must be a valid Hetzner Cloud image name, for *system* or *app* type, such as *ubuntu-22.04*,
+  or a description, for *backup* or *snapshot* type.
 
 For example,
 
 :ubuntu-20.04:
 
    .. code-block:: yaml
 
       job-name:
-         runs-on: [self-hosted, type-cx11, in-ash, image-system-ubuntu-20.04]
+         runs-on: [self-hosted, type-cx11, in-ash, image-x86-system-ubuntu-20.04]
 
 
 :docker-ce app:
-   :✋ Note:
-      Currently Docker CE application does not support ARM64 architecture.
 
    .. code-block:: yaml
 
       job-name:
-         runs-on: [self-hosted, type-cx11, in-ash, image-app-docker-ce]
+         runs-on: [self-hosted, type-cx11, in-ash, image-x86-app-docker-ce]
 
 :snapshot:
    For snapshots, specify **description** as the name. Snapshot descriptions
    must be unique.
 
    .. code-block:: yaml
 
       job-name:
-         runs-on: [self-hosted, type-cx11, in-ash, image-snapshot-snapshot_description]
+         runs-on: [self-hosted, type-cx11, in-ash, image-x86-snapshot-snapshot_description]
 
 ----
 
 --------------------------------------------
 Specifying Custom Runner Server Setup Script
 --------------------------------------------
 
@@ -467,15 +505,15 @@
 
 You can sanity check your configuration file by executing it directly:
 
 .. code-block:: bash
 
    python3 config.py
 
-You can pass your custom configuration file using the *-c path, --config path** command line option.
+You can pass your custom configuration file using the **-c path, --config path** command line option.
 
 .. code-block:: bash
 
    github-runners -c config.py
 
 Configuration Schema
 =====================
@@ -1047,29 +1085,29 @@
 ------------------
 
 The program scales up runners by looking for any jobs that have **queued** status.
 For each such job, a corresponding Hetzner Cloud server instance is created with the following name:
 
 ::
 
-   github-runner-{job.run_id}-{job.id}
+   github-runner-{job.id}
 
 The server is configured using default **setup** and **startup** scripts. The runner name is set
 to be the same as the server name so that servers can be deleted for any unused runner that for some reason
 does not pick up a job for which it was created within the **max-unused-runner-time** period.
 
 :Note:
-   Given that the server name is fixed and specific for each *job.run_id, job.id* tuple, if multiple `github-runners` are running in parallel then
+   Given that the server name is fixed and specific for each *job.id*, if multiple `github-runners` are running in parallel then
    only 1 server will be created for a given `job` and any other attempts to create a server with the same name will be rejected
    by the Hetzner Cloud.
 
 Also,
 
 :Note:
-   There is no guarantee that a given runner will pick the job with the exact **run_id, job.id** tuple that caused it to be created.
+   There is no guarantee that a given runner will pick the job with the exact **job.id** that caused it to be created.
    This is expected and because for each **queued** job a unique runner will be created the number of runners will be
    equal the number of jobs and therefore under normal conditions all jobs will be executed as expected.
 
 ----
 
 Maximum Number of Runners
 =========================
@@ -1108,15 +1146,15 @@
 :Server Location:
 
    The server location can bespecified by using the **--default-location** option or the **in-<name>** runner label.
    By default, location is not set as some server types are not available in some locations.
 
 :Image:
 
-   The server is configured to have the image specified by the **--default-image** option or the **image-{type}-{name}** runner label.
+   The server is configured to have the image specified by the **--default-image** option or the **image-{architecture}-{type}-{name}** runner label.
 
 :SSH Access:
 
    The server is configured to be accessed using *ssh* utility and the SSH public key path is specified using the **--ssh-key**
    option.
 
 :Image Configuration:
@@ -1286,17 +1324,18 @@
 
 * **--default-type name**
   default runner server type name, default: *cx11*
 
 * **--default-location name**
   default runner server location name, default: not specified
 
-* **--default-image type:name_or_description**
+* **--default-image architecture:type:name_or_description**
   default runner server image type and name or description,
-  where type is either: 'system','snapshot','backup','app',
+  where the architecture is either: 'x86' or 'arm',
+  and type is either: 'system','snapshot','backup','app',
   default: *system:ubuntu-22.04*
 
 * **-m count, --max-runners count**
   maximum number of active runners, default: *10*
 
 * **-w count, --workers count**
   number of concurrent workers, default: *10*
@@ -1356,17 +1395,18 @@
 
         * **-l name, --location name**
           deployment server location, default: *ash*
 
         * **-t name, --type name**
           deployment server type, default: *cpx11*
 
-        * **-i type:name_or_description, --image type:name_or_description**
+        * **-i architecture:type:name_or_description, --image architecture:type:name_or_description**
           deployment server image type and name or description,
-          where the type is either: 'system','snapshot','backup','app',
+          where the architecture is either: 'x86' or 'arm',
+          and the type is either: 'system','snapshot','backup','app',
           default: *system:ubuntu-22.04*
 
         * **--setup-script path**
           path to custom deployment server setup script
 
       * **redeploy**
         redeploy on the same cloud service server
```

### Comparing `testflows.github.runners-1.3.230730.1002903/setup.py` & `testflows.github.runners-1.3.230731.1154931/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.3.230730.1002903",
+    version="1.3.230731.1154931",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.3.230730.1002903/testflows/github/runners/__init__.py` & `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.3.230730.1002903"
+__version__ = "1.3.230731.1154931"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.3.230730.1002903/testflows/github/runners/actions.py` & `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230730.1002903/testflows/github/runners/args.py` & `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/args.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,24 +40,26 @@
         raise ArgumentTypeError(f"{v} must be >= 0")
     return v
 
 
 def image_type(v, separator=":"):
     """Image type argument. Example: system:ubuntu-22.04"""
     try:
-        image_type, image_name = v.split(separator, 1)
+        image_architecture, image_type, image_name = v.split(separator, 2)
         assert image_type in ("system", "snapshot", "backup", "app")
     except:
         raise ArgumentTypeError(f"invalid image {v}")
 
     if image_type in ("system", "app"):
-        return Image(type=image_type, name=image_name)
+        return Image(type=image_type, architecture=image_architecture, name=image_name)
     else:
         # backup or snapshot uses description
-        return Image(type=image_type, description=image_name)
+        return Image(
+            type=image_type, architecture=image_architecture, description=image_name
+        )
 
 
 def location_type(v):
     """Location type argument. Example: ash"""
     if v is not None:
         return Location(name=v)
     return None
```

### Comparing `testflows.github.runners-1.3.230730.1002903/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/bin/github-runners`

 * *Files 1% similar despite different names*

```diff
@@ -117,20 +117,21 @@
         metavar="count",
         type=args.count_type,
         help="maximum number of active runners, default: 10",
     )
 
     parser.add_argument(
         "--default-image",
-        metavar="type:name_or_description",
+        metavar="architecture:type:name_or_description",
         type=args.image_type,
         help=(
             "default runner server image type and name or description,\n"
-            "where the type is either: 'system','snapshot','backup','app',\n"
-            "default: system:ubuntu-22.04"
+            "where the architecture is either: 'x86' or 'arm' and\n"
+            "the type is either: 'system','snapshot','backup','app',\n"
+            "default: x86:system:ubuntu-22.04"
         ),
     )
 
     parser.add_argument(
         "--default-type",
         dest="default_server_type",
         metavar="name",
@@ -302,21 +303,22 @@
         type=args.server_type,
         help="deployment server type, default: cpx11",
     )
 
     deploy_cloud_parser.add_argument(
         "-i",
         "--image",
-        metavar="type:name_or_description",
+        metavar="architecture:type:name_or_description",
         dest="cloud_deploy_image",
         type=args.image_type,
         help=(
             "deployment server image type and name or description,\n"
-            "where the type is either: 'system','snapshot','backup','app',\n"
-            "default: system:ubuntu-22.04"
+            "where the architecture is either: 'x86' or 'arm' and\n"
+            "and the type is either: 'system','snapshot','backup','app',\n"
+            "default: x86:system:ubuntu-22.04"
         ),
     )
 
     deploy_cloud_parser.add_argument(
         "--setup-script",
         metavar="path",
         dest="cloud_deploy_setup_script",
```

### Comparing `testflows.github.runners-1.3.230730.1002903/testflows/github/runners/cloud.py` & `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/cloud.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230730.1002903/testflows/github/runners/config.py` & `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     count: count = 1
     replenish_immediately: bool = True
 
 
 @dataclass
 class deploy:
     server_type: server_type = server_type("cpx11")
-    image: image = image("system:ubuntu-22.04")
+    image: image = image("x86:system:ubuntu-22.04")
     location: location = None
     setup_script: path = None
 
 
 @dataclass
 class cloud:
     server_name: str = "github-runners"
@@ -46,15 +46,15 @@
     """Program configuration class."""
 
     github_token: str = os.getenv("GITHUB_TOKEN")
     github_repository: str = os.getenv("GITHUB_REPOSITORY")
     hetzner_token: str = os.getenv("HETZNER_TOKEN")
     ssh_key: str = os.path.expanduser("~/.ssh/id_rsa.pub")
     max_runners: count = 10
-    default_image: image = image("system:ubuntu-22.04")
+    default_image: image = image("x86:system:ubuntu-22.04")
     default_server_type: server_type = server_type("cx11")
     default_location: location = None
     workers: count = 10
     setup_script: path = None
     startup_x64_script: path = None
     startup_arm64_script: path = None
     max_powered_off_time: count = 60
@@ -119,18 +119,22 @@
 
 def check_image(client: Client, image: Image):
     """Check if image exists.
     If image type is not 'system' then use image description to find it.
     """
 
     if image.type in ("system", "app"):
-        return client.images.get_by_name(image.name)
+        return client.images.get_by_name_and_architecture(
+            name=image.name, architecture=image.architecture
+        )
     else:
         # backup or snapshot
         try:
             return [
                 i
-                for i in client.images.get_all(type=image.type)
+                for i in client.images.get_all(
+                    type=image.type, architecture=image.architecture
+                )
                 if i.description == image.description
             ][0]
         except IndexError:
             raise ImageNotFoundError(f"{image.type}:{image.description} not found")
```

### Comparing `testflows.github.runners-1.3.230730.1002903/testflows/github/runners/delete.py` & `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/delete.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230730.1002903/testflows/github/runners/logger.py` & `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/logger.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230730.1002903/testflows/github/runners/request.py` & `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230730.1002903/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230730.1002903/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scale_up.py`

 * *Files 1% similar despite different names*

```diff
@@ -404,38 +404,41 @@
                                             setup_worker_pool=setup_worker_pool,
                                             futures=futures,
                                             servers=servers,
                                         )
                     except StopIteration:
                         pass
 
-                with Action("Checking standby runner pool"):
-                    for standby_runner in standby_runners:
-                        labels = set(standby_runner.labels)
-                        replenish_immediately = standby_runner.replenish_immediately
-                        if replenish_immediately:
-                            available = count_available(servers=servers, labels=labels)
-                        else:
-                            available = count_present(server=servers, labels=labels)
+                if standby_runners:
+                    with Action("Checking standby runner pool"):
+                        for standby_runner in standby_runners:
+                            labels = set(standby_runner.labels)
+                            replenish_immediately = standby_runner.replenish_immediately
+                            if replenish_immediately:
+                                available = count_available(
+                                    servers=servers, labels=labels
+                                )
+                            else:
+                                available = count_present(server=servers, labels=labels)
 
-                        if available < standby_runner.count:
-                            for _ in range(standby_runner.count - available):
-                                try:
-                                    with Action(
-                                        f"Replenishing{' immediately' if replenish_immediately else ''} standby server with {labels}"
-                                    ):
-                                        create_runner_server(
-                                            name=f"{standby_server_name_prefix}{str(uuid.uuid1()).replace('-','')}",
-                                            labels=labels,
-                                            setup_worker_pool=setup_worker_pool,
-                                            futures=futures,
-                                            servers=servers,
-                                        )
-                                except StopIteration:
-                                    break
+                            if available < standby_runner.count:
+                                for _ in range(standby_runner.count - available):
+                                    try:
+                                        with Action(
+                                            f"Replenishing{' immediately' if replenish_immediately else ''} standby server with {labels}"
+                                        ):
+                                            create_runner_server(
+                                                name=f"{standby_server_name_prefix}{str(uuid.uuid1()).replace('-','')}",
+                                                labels=labels,
+                                                setup_worker_pool=setup_worker_pool,
+                                                futures=futures,
+                                                servers=servers,
+                                            )
+                                    except StopIteration:
+                                        break
 
                 for future in futures:
                     with Action(
                         f"Waiting to finish creating server {future.server_name}",
                         ignore_fail=True,
                     ):
                         future.result()
```

### Comparing `testflows.github.runners-1.3.230730.1002903/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230730.1002903/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230730.1002903/testflows/github/runners/scripts/deploy/setup.sh` & `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scripts/deploy/setup.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230730.1002903/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230730.1002903/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230730.1002903/testflows/github/runners/server.py` & `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230730.1002903/testflows/github/runners/service.py` & `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/service.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230730.1002903/testflows/github/runners/shell.py` & `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230730.1002903/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.3.230731.1154931/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.3.230730.1002903
+Version: 1.3.230731.1154931
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -12,16 +12,16 @@
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
 .. image:: https://raw.githubusercontent.com/testflows/TestFlows-ArtWork/master/images/logo.png
-   :width: 20%
-   :align: left
+   :width: 300px
+   :align: center
    :target: https://testflows.com
    :alt: TestFlows Open-source Testing Framework
 
 ----
 
 :PyPi:
    `Versions <https://pypi.org/project/testflows.github.runners/>`_
@@ -34,15 +34,21 @@
 
 A simple alternative to Github's `Recommended autoscaling solutions <https://docs.github.com/en/actions/hosting-your-own-runners/managing-self-hosted-runners/autoscaling-with-self-hosted-runners#recommended-autoscaling-solutions>`_.
 
 The **github-runners** service program starts and monitors queued up jobs for GitHub Actions workflows.
 When a new job is queued up, it creates a new Hetzner Cloud server instance
 that provides an ephemeral GitHub Actions runner. Each server instance is automatically
 powered off when job completes and then powered off servers are
-automatically deleted. Both **x64** and **arm64** runners are supported.
+automatically deleted. Both **x64** (*x86*) and **arm64** (*arm*) runners are supported.
+See `Features`_ and `Limitations`_ for more details.
+
+.. image:: https://raw.githubusercontent.com/testflows/TestFlows-GitHub-Runners/master/intro.gif
+   :align: center
+   :alt: TestFlows GitHub Runners
+
 
 :❗Warning:
    This program is provided on "AS IS" basis without warranties or conditions of any kind. See LICENSE.
    Use it at your own risk. Manual monitoring is required to make sure server instances are cleaned up properly
    and costs are kept under control.
 
 Costs depend on the server type, number of jobs and execution time. For each job a new server instance is created
@@ -65,15 +71,18 @@
 Features
 --------
 
 * cost efficient on-demand runners using `Hetzner Cloud <https://www.hetzner.com/cloud>`_
 * simple configuration, no Webhooks, no need for AWS lambdas, and no need to setup any GitHub application
 * supports specifying custom runner server types, images, and locations using job labels
 * self-contained program that you can use to deploy, redeploy, and manage the service on a cloud instance
-* supports both x64 and ARM64 runners
+* supports x64 (x86) and ARM64 (arm) runners
+* supports using any Hetzner Cloud server types
+* supports runners with pre-installed Docker
+* supports using any standard Hetzner Cloud images and applications
 * supports auto-replenishable fixed standby runner pools for jobs to be picked up immediately
 * simpler alternative to what GitHub lists in `Recommended autoscaling solutions <https://docs.github.com/en/actions/hosting-your-own-runners/managing-self-hosted-runners/autoscaling-with-self-hosted-runners#recommended-autoscaling-solutions>`_
 
 ----
 
 -----------
 Limitations
@@ -184,14 +193,39 @@
 
 .. code-block:: bash
 
    github-runners --max-runners 40
 
 ----
 
+-------------------------------
+Jobs That Require Docker Engine
+-------------------------------
+
+For jobs that require Docker to be installed, you can use the standard `Hetzner Docker CE application <https://docs.hetzner.com/cloud/apps/list/docker-ce/>`_
+which can be specified using the **image-** label. See `Specifying Runner Image`_ for more details about specifying custom runner images.
+
+For example
+
+:x64:
+
+   .. code-block:: yaml
+
+      job-name:
+         runs-on: [self-hosted, type-cx11, image-x86-app-docker-ce]
+
+:ARM64:
+
+   .. code-block:: yaml
+
+      job-name:
+         runs-on: [self-hosted, type-cax11, image-arm-app-docker-ce]
+
+----
+
 ----------------------
 Specifying Runner Type
 ----------------------
 
 x64 Runners
 ============
 
@@ -254,44 +288,48 @@
 -----------------------
 Specifying Runner Image
 -----------------------
 
 By default, the default image of the server for the runner is **ubuntu-22.04**. You can use the **--default-image**
 option to force specific default server image.
 
-You can also use the **image-{type}-{name}** runner label to specify server image for a specific job. Where the **{name}** must be a valid
-Hetzner Cloud image such as *ubuntu-22.04* or *ubuntu-20.04*, and the **{type}** is either *system*, *snapshot*, *backup*, or *app*.
+You can also use the **image-{architecture}-{type}-{name}** runner label to specify server image for a specific job.
+
+Where,
+
+* **{architecture}** is either *x86* or *arm*
+* **{type}** is either *system*, *snapshot*, *backup*, or *app*
+* **{name}** must be a valid Hetzner Cloud image name, for *system* or *app* type, such as *ubuntu-22.04*,
+  or a description, for *backup* or *snapshot* type.
 
 For example,
 
 :ubuntu-20.04:
 
    .. code-block:: yaml
 
       job-name:
-         runs-on: [self-hosted, type-cx11, in-ash, image-system-ubuntu-20.04]
+         runs-on: [self-hosted, type-cx11, in-ash, image-x86-system-ubuntu-20.04]
 
 
 :docker-ce app:
-   :✋ Note:
-      Currently Docker CE application does not support ARM64 architecture.
 
    .. code-block:: yaml
 
       job-name:
-         runs-on: [self-hosted, type-cx11, in-ash, image-app-docker-ce]
+         runs-on: [self-hosted, type-cx11, in-ash, image-x86-app-docker-ce]
 
 :snapshot:
    For snapshots, specify **description** as the name. Snapshot descriptions
    must be unique.
 
    .. code-block:: yaml
 
       job-name:
-         runs-on: [self-hosted, type-cx11, in-ash, image-snapshot-snapshot_description]
+         runs-on: [self-hosted, type-cx11, in-ash, image-x86-snapshot-snapshot_description]
 
 ----
 
 --------------------------------------------
 Specifying Custom Runner Server Setup Script
 --------------------------------------------
 
@@ -484,15 +522,15 @@
 
 You can sanity check your configuration file by executing it directly:
 
 .. code-block:: bash
 
    python3 config.py
 
-You can pass your custom configuration file using the *-c path, --config path** command line option.
+You can pass your custom configuration file using the **-c path, --config path** command line option.
 
 .. code-block:: bash
 
    github-runners -c config.py
 
 Configuration Schema
 =====================
@@ -1064,29 +1102,29 @@
 ------------------
 
 The program scales up runners by looking for any jobs that have **queued** status.
 For each such job, a corresponding Hetzner Cloud server instance is created with the following name:
 
 ::
 
-   github-runner-{job.run_id}-{job.id}
+   github-runner-{job.id}
 
 The server is configured using default **setup** and **startup** scripts. The runner name is set
 to be the same as the server name so that servers can be deleted for any unused runner that for some reason
 does not pick up a job for which it was created within the **max-unused-runner-time** period.
 
 :Note:
-   Given that the server name is fixed and specific for each *job.run_id, job.id* tuple, if multiple `github-runners` are running in parallel then
+   Given that the server name is fixed and specific for each *job.id*, if multiple `github-runners` are running in parallel then
    only 1 server will be created for a given `job` and any other attempts to create a server with the same name will be rejected
    by the Hetzner Cloud.
 
 Also,
 
 :Note:
-   There is no guarantee that a given runner will pick the job with the exact **run_id, job.id** tuple that caused it to be created.
+   There is no guarantee that a given runner will pick the job with the exact **job.id** that caused it to be created.
    This is expected and because for each **queued** job a unique runner will be created the number of runners will be
    equal the number of jobs and therefore under normal conditions all jobs will be executed as expected.
 
 ----
 
 Maximum Number of Runners
 =========================
@@ -1125,15 +1163,15 @@
 :Server Location:
 
    The server location can bespecified by using the **--default-location** option or the **in-<name>** runner label.
    By default, location is not set as some server types are not available in some locations.
 
 :Image:
 
-   The server is configured to have the image specified by the **--default-image** option or the **image-{type}-{name}** runner label.
+   The server is configured to have the image specified by the **--default-image** option or the **image-{architecture}-{type}-{name}** runner label.
 
 :SSH Access:
 
    The server is configured to be accessed using *ssh* utility and the SSH public key path is specified using the **--ssh-key**
    option.
 
 :Image Configuration:
@@ -1303,17 +1341,18 @@
 
 * **--default-type name**
   default runner server type name, default: *cx11*
 
 * **--default-location name**
   default runner server location name, default: not specified
 
-* **--default-image type:name_or_description**
+* **--default-image architecture:type:name_or_description**
   default runner server image type and name or description,
-  where type is either: 'system','snapshot','backup','app',
+  where the architecture is either: 'x86' or 'arm',
+  and type is either: 'system','snapshot','backup','app',
   default: *system:ubuntu-22.04*
 
 * **-m count, --max-runners count**
   maximum number of active runners, default: *10*
 
 * **-w count, --workers count**
   number of concurrent workers, default: *10*
@@ -1373,17 +1412,18 @@
 
         * **-l name, --location name**
           deployment server location, default: *ash*
 
         * **-t name, --type name**
           deployment server type, default: *cpx11*
 
-        * **-i type:name_or_description, --image type:name_or_description**
+        * **-i architecture:type:name_or_description, --image architecture:type:name_or_description**
           deployment server image type and name or description,
-          where the type is either: 'system','snapshot','backup','app',
+          where the architecture is either: 'x86' or 'arm',
+          and the type is either: 'system','snapshot','backup','app',
           default: *system:ubuntu-22.04*
 
         * **--setup-script path**
           path to custom deployment server setup script
 
       * **redeploy**
         redeploy on the same cloud service server
```

### Comparing `testflows.github.runners-1.3.230730.1002903/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.3.230731.1154931/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -19,11 +19,12 @@
 testflows/github/runners/scale_up.py
 testflows/github/runners/server.py
 testflows/github/runners/service.py
 testflows/github/runners/shell.py
 testflows/github/runners/bin/github-runners
 testflows/github/runners/scripts/__init__.py
 testflows/github/runners/scripts/setup.sh
+testflows/github/runners/scripts/setup_docker.sh
 testflows/github/runners/scripts/startup_arm64.sh
 testflows/github/runners/scripts/startup_x64.sh
 testflows/github/runners/scripts/deploy/__init__.py
 testflows/github/runners/scripts/deploy/setup.sh
```

