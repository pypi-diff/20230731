# Comparing `tmp/pyautomail-1.5.1.1.tar.gz` & `tmp/pyautomail-1.5.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyautomail-1.5.1.1.tar", last modified: Mon Jul 31 02:56:13 2023, max compression
+gzip compressed data, was "pyautomail-1.5.1.2.tar", last modified: Mon Jul 31 04:05:07 2023, max compression
```

## Comparing `pyautomail-1.5.1.1.tar` & `pyautomail-1.5.1.2.tar`

### file list

```diff
@@ -1,63 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:56:13.492852 pyautomail-1.5.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:56:13.484851 pyautomail-1.5.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:56:13.488851 pyautomail-1.5.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-31 02:56:13.492852 pyautomail-1.5.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:56:13.488851 pyautomail-1.5.1.1/automail/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/automail/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:56:13.488851 pyautomail-1.5.1.1/automail/config/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/automail/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/automail/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/automail/emailsender.py
--rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/automail/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:56:13.488851 pyautomail-1.5.1.1/automail/storage/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/automail/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/automail/storage/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/automail/storage/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/automail/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/config.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/contact.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:56:13.488851 pyautomail-1.5.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:56:13.488851 pyautomail-1.5.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   191926 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/docs/_static/automail-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:56:13.488851 pyautomail-1.5.1.1/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:56:13.492852 pyautomail-1.5.1.1/docs/_templates/apidoc/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/docs/_templates/apidoc/module.rst_t
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/docs/_templates/apidoc/package.rst_t
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/docs/_templates/apidoc/toc.rst_t
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:56:13.492852 pyautomail-1.5.1.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/docs/api/automail.config.rst
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/docs/api/automail.rst
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/docs/api/automail.storage.rst
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/docs/getting-started.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:56:13.492852 pyautomail-1.5.1.1/docs/tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/docs/tutorial/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/docs/tutorial/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)    36379 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/document.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:56:13.492852 pyautomail-1.5.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/examples/base-usage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:56:13.492852 pyautomail-1.5.1.1/pyautomail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-31 02:56:13.000000 pyautomail-1.5.1.1/pyautomail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 02:56:13.000000 pyautomail-1.5.1.1/pyautomail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 02:56:13.000000 pyautomail-1.5.1.1/pyautomail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-31 02:56:13.000000 pyautomail-1.5.1.1/pyautomail.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-31 02:56:13.000000 pyautomail-1.5.1.1/pyautomail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-31 02:56:13.000000 pyautomail-1.5.1.1/pyautomail.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/sending_gmail.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-31 02:56:13.492852 pyautomail-1.5.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/sub.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:56:13.492852 pyautomail-1.5.1.1/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/templates/body.txt
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-31 02:56:05.000000 pyautomail-1.5.1.1/templates/html.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:05:07.103667 pyautomail-1.5.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:05:07.095667 pyautomail-1.5.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:05:07.099667 pyautomail-1.5.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-07-31 04:05:07.103667 pyautomail-1.5.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:05:07.099667 pyautomail-1.5.1.2/automail/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/automail/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:05:07.099667 pyautomail-1.5.1.2/automail/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/automail/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/automail/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/automail/emailsender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/automail/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:05:07.099667 pyautomail-1.5.1.2/automail/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/automail/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/automail/storage/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/automail/storage/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/automail/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/config.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/contact.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:05:07.099667 pyautomail-1.5.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:05:07.099667 pyautomail-1.5.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   191926 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/docs/_static/automail-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:05:07.095667 pyautomail-1.5.1.2/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:05:07.099667 pyautomail-1.5.1.2/docs/_templates/apidoc/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/docs/_templates/apidoc/module.rst_t
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/docs/_templates/apidoc/package.rst_t
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/docs/_templates/apidoc/toc.rst_t
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:05:07.099667 pyautomail-1.5.1.2/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/docs/api/automail.config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/docs/api/automail.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/docs/api/automail.storage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/docs/getting-started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:05:07.099667 pyautomail-1.5.1.2/docs/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/docs/tutorial/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    36379 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/document.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:05:07.103667 pyautomail-1.5.1.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/examples/base-usage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:05:07.103667 pyautomail-1.5.1.2/pyautomail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-07-31 04:05:07.000000 pyautomail-1.5.1.2/pyautomail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-31 04:05:07.000000 pyautomail-1.5.1.2/pyautomail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 04:05:07.000000 pyautomail-1.5.1.2/pyautomail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-31 04:05:07.000000 pyautomail-1.5.1.2/pyautomail.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-31 04:05:07.000000 pyautomail-1.5.1.2/pyautomail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-31 04:05:07.000000 pyautomail-1.5.1.2/pyautomail.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/sending_gmail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-31 04:05:07.103667 pyautomail-1.5.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/sub.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:05:07.103667 pyautomail-1.5.1.2/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/templates/body.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-31 04:04:59.000000 pyautomail-1.5.1.2/templates/html.html
```

### Comparing `pyautomail-1.5.1.1/.readthedocs.yaml` & `pyautomail-1.5.1.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.1/automail/config/config.py` & `pyautomail-1.5.1.2/automail/config/config.py`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.1/automail/emailsender.py` & `pyautomail-1.5.1.2/automail/emailsender.py`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.1/automail/manager.py` & `pyautomail-1.5.1.2/automail/manager.py`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.1/automail/storage/model.py` & `pyautomail-1.5.1.2/automail/storage/model.py`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.1/automail/storage/util.py` & `pyautomail-1.5.1.2/automail/storage/util.py`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.1/automail/utils.py` & `pyautomail-1.5.1.2/automail/utils.py`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.1/docs/Makefile` & `pyautomail-1.5.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.1/docs/_static/automail-logo.png` & `pyautomail-1.5.1.2/docs/_static/automail-logo.png`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.1/docs/_templates/apidoc/package.rst_t` & `pyautomail-1.5.1.2/docs/_templates/apidoc/package.rst_t`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.1/docs/api/automail.rst` & `pyautomail-1.5.1.2/docs/api/automail.rst`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.1/docs/conf.py` & `pyautomail-1.5.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.1/docs/getting-started.rst` & `pyautomail-1.5.1.2/docs/getting-started.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Quickstart with automail
+Quickstart with pyautomail
 =============================
 
 Welcome to automail! This guide will help you get up and running with the automated
 email sending Python package in no time.
 
 .. note::
     This guide assumes that you have some basic knowledge of Python and the command line.
@@ -22,16 +22,22 @@
 
     **Additionally a user interface will be provided in the future.**
 
 .. _install:
 
 Installation
 ------------
+To install pyautomail, you can use pip to install the package directly from PyPI:
 
-To install automail, you can use pip and git to install the package directly from GitHub:
+.. code-block:: bash
+
+    $ pip install pyautomail
+
+
+Or you can use pip and git to install the latest version directly from GitHub:
 
 .. code-block:: bash
 
     $ pip install git+https://github.com/msinamsina/automail.git
 
 
 This will download and install the latest version of automail along with its dependencies.
@@ -44,26 +50,26 @@
     $ cd automail
     $ pip install .
 
 .. _htu:
 
 How to Use
 ----------
-There are two ways to use automail to send emails. You can either use the most powerful
+There are two ways to use pyautomail to send emails. You can either use the most powerful
 command-line interface (CLI) tool without writing any Python code, or you can use the
 Python package in your custom scripts. We'll cover a quick overview of both of these
 options in this guide. For more details, please refer to :doc:`the Tutorial section <tutorial/index>`
 and the :doc:`API reference <api/index>`.
 
 .. _cli:
 
 1. Automail command-line interface (CLI) tool
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-When you install automail, you will also get a command-line interface (CLI) tool called `automail`.
+When you install pyautomail, you will also get a command-line interface (CLI) tool called `automail`.
 This tool can be used to send emails from the command line, without writing any Python code.
 So if you want to send a quick email without writing a script, you can use the CLI tool.
 
 To use the CLI tool, you will need to provide your contact list in a CSV file.
 The CSV file should contain the following columns: `name`, `email` and other
 columns can be added as contact information which will be used in the email template.
 
@@ -116,15 +122,15 @@
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 If you want to automate your email sending process, you can also use the Python package in your custom scripts.
 This will give you more flexibility and control over the email sending process.
 You can use the Python package to send emails to multiple recipients, use custom email templates,
 and customize other settings according to your needs.
 
-You can also use automail in your custom Python scripts to send emails.
+You can also use pyautomail in your custom Python scripts to send emails.
 Here's two basic examples of sending an email to a single recipient:
 
 - **First example**
     .. code-block:: python
 
         from automail import EmailSender
```

### Comparing `pyautomail-1.5.1.1/docs/index.rst` & `pyautomail-1.5.1.2/docs/index.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,117 +1,56 @@
-.. Automail documentation master file, created by
+.. Pyautomail documentation master file, created by
    sphinx-quickstart on Tue Jul 25 17:21:33 2023.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
-**AUTOMAIL: Automated Email Sending for Large Scale Email and Gmail Automation**
+**PYAUTOMAIL: Automated Email Sending for Large Scale Email and Gmail Automation**
 ================================================================================
 
 .. figure:: _static/automail-logo.png
    :align: center
    :alt: automail logo
    :width: 100%
 
 .. raw:: html
 
    <br>
 
-
-Welcome to the documentation for **automail**, a powerful Python package designed
+Welcome to the documentation for **pyautomail**, a powerful Python package designed
 for automated email sending, especially tailored for large scale Email or Gmail automation.
 In today's fast-paced digital world, effective communication is a vital aspect of many
 businesses and projects which rely on email as a primary means of communication.
 However, manually sending individual emails or even managing bulk
 email campaigns can be time-consuming and error-prone.
 
-**Automail** comes to the rescue by providing a seamless and efficient solution for
+**Pyautomail** comes to the rescue by providing a seamless and efficient solution for
 automating email communication. Whether you need to send personalized emails to
 a vast audience, conduct email marketing campaigns, or automate routine email
 tasks, this package is your go-to tool. Its user-friendly interface
 and versatile features make it suitable for a wide range of applications, from
 startups to enterprises, professionals, and developers.
 
 Whether you need to send bulk emails, automate Gmail tasks, or
-improve your email communication efficiency, **automail** is here to streamline
+improve your email communication efficiency, **PYautomail** is here to streamline
 your workflow and enhance productivity.
 
 .. note::
-   For more information about **automail**
+   For more information about **pyautomail**
    and its capabilities, please explore our documentation.
 
-   - You can see a short overview and features of ``automail`` in the :doc:`Introduction <introduction>` section.
-   - If you are new to ``automail``, you can get started with our :doc:`Getting Started <getting-started>` guide.
+   - You can see a short overview and features of ``pyautomail`` in the :doc:`Introduction <introduction>` section.
+   - If you are new to ``pyautomail``, you can get started with our :doc:`Getting Started <getting-started>` guide.
    - For a quick reference, you can check out the :doc:`API Reference <api/index>` section.
-   - If you want to learn more about ``automail`` and best practices, you can read our :doc:`Tutorial <tutorial/index>` section.
+   - If you want to learn more about ``pyautomail`` and best practices, you can read our :doc:`Tutorial <tutorial/index>` section.
 
 The documentation is organized into the following sections:
 
-
 .. toctree::
    :maxdepth: 2
    :caption: Contents
 
    introduction
    getting-started
    tutorial/index
    api/index
 
-
-
 **Keywords**: Email, Gmail, Automation, Large Scale Email Sending, Python Package, Bulk Email, Email Automation, Email Automation Python, Gmail Integration, Automated Email Communication, Email Automation Tool, Mass Email Sending, Python Email Automation.
-
-
-
-1. **Introduction**
-
-   - Overview
-   - Features
-   - Installation
-
-2. **Getting Started**
-
-   - Quickstart Guide
-   - Configuration
-
-3. **Sending Emails**
-
-   - Single Recipient
-   - Multiple Recipients
-   - Customizing Templates
-
-4. **Gmail Automation**
-
-   - Setting Up Gmail Integration
-   - Managing Labels
-   - Searching and Filtering Emails
-
-5. **Advanced Usage**
-
-   - Email Attachments
-   - Error Handling
-   - Throttling and Rate Limiting
-
-6. **Best Practices**
-
-   - Bulk Email Tips
-   - Avoiding Spam Filters
-   - Performance Optimization
-
-7. **FAQs**
-
-   - Frequently Asked Questions
-
-8. **API Reference**
-
-   - automail Module
-
-9. **Contributing**
-
-   - How to Contribute
-   - Code Guidelines
-   - Issue Tracker
-
-10. **Changelog**
-
-    - Version History
-
-
```

### Comparing `pyautomail-1.5.1.1/docs/introduction.rst` & `pyautomail-1.5.1.2/docs/introduction.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,66 +1,64 @@
 Introduction
 ============
 
 Overview
 --------
 
-Automail is a dynamic Python package that enhances automated email sending.
+Pyautomail is a dynamic Python package that enhances automated email sending.
 Utilizing the built-in smtplib module, it ensures reliable communication.
 With the flexibility to send personalized emails using HTML or plain text templates,
-Automail adds a personal touch to each message. Boosted by Jinja2, it enables the
+Pyautomail adds a personal touch to each message. Boosted by Jinja2, it enables the
 creation of captivating and visually appealing email templates. Moreover, you can
 effortlessly attach global or personalized PDF files to enrich your emails.
 The package also offers the convenience of scheduling emails for timely delivery.
-Simplify your email campaigns and elevate your communication with **Automail**'s creative features and efficiency.
+Simplify your email campaigns and elevate your communication with **Pyautomail**'s creative features and efficiency.
 
 .. warning::
 
-   Automail is currently in alpha. It is not yet ready for production use.
+   Pyautomail is currently in alpha. It is not yet ready for production use.
 
 Key Features
 ------------
 - **Automated Email Sending**:
-    Automail enables you to automate the entire email sending process, saving
+    Pyautomail enables you to automate the entire email sending process, saving
     you valuable time and effort. With just a few lines of code, you can send
     personalized emails to individuals or even conduct large-scale email campaigns.
 
 - **Customizable Email Templates**:
-    Personalization is key to effective communication. With automail, you can
+    Personalization is key to effective communication. With pyautomail, you can
     create dynamic email templates using Jinja2 or simple HTML, allowing you to
     tailor each email's content to suit the recipient.
 
 - **Attachment Support**:
-    Want to include additional content with your emails? Automail makes it easy
+    Want to include additional content with your emails? Pyautomail makes it easy
     to attach global PDFs or personalized PDFs to each email, providing a seamless
     experience for your recipients.
 
 - **HTML or Plain Text**:
     Whether you prefer richly formatted HTML emails or simple plain text messages,
-    automail caters to your needs. The package supports both HTML (Jinja2 or standard)
+    pyautomail caters to your needs. The package supports both HTML (Jinja2 or standard)
     and plain text templates for versatile email communication.
 
 - **Scheduled Emails**:
-    Need to send emails at specific times? Automail allows you to schedule your
+    Need to send emails at specific times? Pyautomail allows you to schedule your
     emails for future delivery, ensuring your messages reach recipients at the
     most opportune moments.
 
-Whether you're a marketer, developer, or business owner, automail is a valuable addition
+Whether you're a marketer, developer, or business owner, pyautomail is a valuable addition
 to your toolkit. Experience the ease of automated email communication while reaching a
 wider audience and driving your projects towards success. So if you're ready to start
-see the :doc:`Getting Started <getting-started>` to learn how to use automail.
-
-
+see the :doc:`Getting Started <getting-started>` to learn how to use pyautomail.
 
 .. note::
 
    If you encounter any issues or have suggestions for improvements, please feel free to report them on our
    `GitHub issue tracker <https://github.com/msinamsina/automail/issues>`_.
 
 
 Github
 ------
-The source code for automail is available on GitHub at the following link:
+The source code for pyautomail is available on GitHub at the following link:
 
 https://github.com/msinamsina/automail.git
 
-Please see the :ref:`how to use <how to use>` for a quick introduction on how to use Automail.
+Please see the :ref:`how to use <how to use>` for a quick introduction on how to use Pyautomail.
```

### Comparing `pyautomail-1.5.1.1/docs/make.bat` & `pyautomail-1.5.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.1/docs/tutorial/tutorial.rst` & `pyautomail-1.5.1.2/docs/tutorial/index.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-.. Automail documentation master file, created by
-   sphinx-quickstart on Tue Jul 25 17:21:33 2023.
-   You can adapt this file completely to your liking, but it should at least
-   contain the root `toctree` directive.
-
 Tutorial
 ========
 
 .. note::
    To install automail please see :ref:`installation <installation>`
 
 Base usage
```

### Comparing `pyautomail-1.5.1.1/document.pdf` & `pyautomail-1.5.1.2/document.pdf`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.1/pyautomail.egg-info/SOURCES.txt` & `pyautomail-1.5.1.2/pyautomail.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 docs/_templates/apidoc/package.rst_t
 docs/_templates/apidoc/toc.rst_t
 docs/api/automail.config.rst
 docs/api/automail.rst
 docs/api/automail.storage.rst
 docs/api/index.rst
 docs/tutorial/index.rst
-docs/tutorial/tutorial.rst
 examples/base-usage.py
 pyautomail.egg-info/PKG-INFO
 pyautomail.egg-info/SOURCES.txt
 pyautomail.egg-info/dependency_links.txt
 pyautomail.egg-info/entry_points.txt
 pyautomail.egg-info/requires.txt
 pyautomail.egg-info/top_level.txt
```

### Comparing `pyautomail-1.5.1.1/sending_gmail.py` & `pyautomail-1.5.1.2/sending_gmail.py`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.1/setup.cfg` & `pyautomail-1.5.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyautomail-1.5.1.1/setup.py` & `pyautomail-1.5.1.2/setup.py`

 * *Files identical despite different names*

