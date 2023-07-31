# Comparing `tmp/looper-1.4.1.tar.gz` & `tmp/looper-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "looper-1.4.1.tar", last modified: Fri Jul 14 21:11:25 2023, max compression
+gzip compressed data, was "looper-1.4.2.tar", last modified: Mon Jul 31 21:18:56 2023, max compression
```

## Comparing `looper-1.4.1.tar` & `looper-1.4.2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:11:25.014073 looper-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-14 21:11:09.000000 looper-1.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-14 21:11:09.000000 looper-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-14 21:11:25.014073 looper-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-14 21:11:09.000000 looper-1.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-14 21:11:09.000000 looper-1.4.1/logo_looper.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:11:25.002073 looper-1.4.1/looper/
--rw-r--r--   0 runner    (1001) docker     (123)    15711 2023-07-14 21:11:09.000000 looper-1.4.1/looper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-14 21:11:09.000000 looper-1.4.1/looper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-14 21:11:09.000000 looper-1.4.1/looper/_devtools.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 21:11:09.000000 looper-1.4.1/looper/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    35283 2023-07-14 21:11:09.000000 looper-1.4.1/looper/conductor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-07-14 21:11:09.000000 looper-1.4.1/looper/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-07-14 21:11:09.000000 looper-1.4.1/looper/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    43820 2023-07-14 21:11:09.000000 looper-1.4.1/looper/html_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)    35130 2023-07-14 21:11:09.000000 looper-1.4.1/looper/html_reports_pipestat.py
--rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-07-14 21:11:09.000000 looper-1.4.1/looper/html_reports_project_pipestat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:11:25.010073 looper-1.4.1/looper/jinja_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates/footer_index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates/head.html
--rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates/logo.html
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates/navbar.html
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates/navbar_links.html
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates/navbar_list_parent.html
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates/object.html
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates/project_object.html
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates/sample.html
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates/status.html
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates/status_table.html
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates/status_table_no_links.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:11:25.014073 looper-1.4.1/looper/jinja_templates_old/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates_old/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates_old/footer_index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates_old/head.html
--rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates_old/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates_old/logo.html
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates_old/navbar.html
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates_old/navbar_links.html
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates_old/navbar_list_parent.html
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates_old/object.html
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates_old/project_object.html
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates_old/sample.html
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates_old/status.html
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates_old/status_table.html
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-14 21:11:09.000000 looper-1.4.1/looper/jinja_templates_old/status_table_no_links.html
--rwxr-xr-x   0 runner    (1001) docker     (123)    45072 2023-07-14 21:11:09.000000 looper-1.4.1/looper/looper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-14 21:11:09.000000 looper-1.4.1/looper/parser_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    14876 2023-07-14 21:11:09.000000 looper-1.4.1/looper/pipeline_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-07-14 21:11:09.000000 looper-1.4.1/looper/processed_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    30954 2023-07-14 21:11:09.000000 looper-1.4.1/looper/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:11:25.014073 looper-1.4.1/looper/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-14 21:11:09.000000 looper-1.4.1/looper/schemas/pipeline_interface_schema_generic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-14 21:11:09.000000 looper-1.4.1/looper/schemas/pipeline_interface_schema_project.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-14 21:11:09.000000 looper-1.4.1/looper/schemas/pipeline_interface_schema_sample.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20474 2023-07-14 21:11:09.000000 looper-1.4.1/looper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:11:25.006073 looper-1.4.1/looper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-14 21:11:24.000000 looper-1.4.1/looper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-14 21:11:24.000000 looper-1.4.1/looper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 21:11:24.000000 looper-1.4.1/looper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-14 21:11:24.000000 looper-1.4.1/looper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-14 21:11:24.000000 looper-1.4.1/looper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 21:11:24.000000 looper-1.4.1/looper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:11:25.014073 looper-1.4.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-14 21:11:09.000000 looper-1.4.1/requirements/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-14 21:11:09.000000 looper-1.4.1/requirements/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-14 21:11:09.000000 looper-1.4.1/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-14 21:11:25.018073 looper-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-14 21:11:09.000000 looper-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:18:56.345370 looper-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-31 21:18:47.000000 looper-1.4.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-31 21:18:47.000000 looper-1.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-31 21:18:56.345370 looper-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-31 21:18:47.000000 looper-1.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-31 21:18:47.000000 looper-1.4.2/logo_looper.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:18:56.341370 looper-1.4.2/looper/
+-rw-r--r--   0 runner    (1001) docker     (123)    15711 2023-07-31 21:18:47.000000 looper-1.4.2/looper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-31 21:18:47.000000 looper-1.4.2/looper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-31 21:18:47.000000 looper-1.4.2/looper/_devtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-31 21:18:47.000000 looper-1.4.2/looper/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35449 2023-07-31 21:18:47.000000 looper-1.4.2/looper/conductor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-07-31 21:18:47.000000 looper-1.4.2/looper/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-07-31 21:18:47.000000 looper-1.4.2/looper/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43820 2023-07-31 21:18:47.000000 looper-1.4.2/looper/html_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35130 2023-07-31 21:18:47.000000 looper-1.4.2/looper/html_reports_pipestat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-07-31 21:18:47.000000 looper-1.4.2/looper/html_reports_project_pipestat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:18:56.345370 looper-1.4.2/looper/jinja_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-31 21:18:47.000000 looper-1.4.2/looper/jinja_templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-07-31 21:18:47.000000 looper-1.4.2/looper/jinja_templates/footer_index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-07-31 21:18:47.000000 looper-1.4.2/looper/jinja_templates/head.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-07-31 21:18:47.000000 looper-1.4.2/looper/jinja_templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-07-31 21:18:47.000000 looper-1.4.2/looper/jinja_templates/logo.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-31 21:18:47.000000 looper-1.4.2/looper/jinja_templates/navbar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-31 21:18:47.000000 looper-1.4.2/looper/jinja_templates/navbar_links.html
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-31 21:18:47.000000 looper-1.4.2/looper/jinja_templates/navbar_list_parent.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-31 21:18:47.000000 looper-1.4.2/looper/jinja_templates/object.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-31 21:18:47.000000 looper-1.4.2/looper/jinja_templates/project_object.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-07-31 21:18:47.000000 looper-1.4.2/looper/jinja_templates/sample.html
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-31 21:18:47.000000 looper-1.4.2/looper/jinja_templates/status.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-07-31 21:18:47.000000 looper-1.4.2/looper/jinja_templates/status_table.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-31 21:18:47.000000 looper-1.4.2/looper/jinja_templates/status_table_no_links.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:18:56.345370 looper-1.4.2/looper/jinja_templates_old/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-31 21:18:47.000000 looper-1.4.2/looper/jinja_templates_old/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-31 21:18:47.000000 looper-1.4.2/looper/jinja_templates_old/footer_index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-07-31 21:18:47.000000 looper-1.4.2/looper/jinja_templates_old/head.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-07-31 21:18:47.000000 looper-1.4.2/looper/jinja_templates_old/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-07-31 21:18:47.000000 looper-1.4.2/looper/jinja_templates_old/logo.html
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-31 21:18:47.000000 looper-1.4.2/looper/jinja_templates_old/navbar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-07-31 21:18:47.000000 looper-1.4.2/looper/jinja_templates_old/navbar_links.html
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-31 21:18:47.000000 looper-1.4.2/looper/jinja_templates_old/navbar_list_parent.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-31 21:18:47.000000 looper-1.4.2/looper/jinja_templates_old/object.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-31 21:18:47.000000 looper-1.4.2/looper/jinja_templates_old/project_object.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-31 21:18:47.000000 looper-1.4.2/looper/jinja_templates_old/sample.html
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-31 21:18:47.000000 looper-1.4.2/looper/jinja_templates_old/status.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-31 21:18:47.000000 looper-1.4.2/looper/jinja_templates_old/status_table.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-31 21:18:47.000000 looper-1.4.2/looper/jinja_templates_old/status_table_no_links.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45072 2023-07-31 21:18:47.000000 looper-1.4.2/looper/looper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-31 21:18:47.000000 looper-1.4.2/looper/parser_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14876 2023-07-31 21:18:47.000000 looper-1.4.2/looper/pipeline_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-07-31 21:18:47.000000 looper-1.4.2/looper/processed_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30954 2023-07-31 21:18:47.000000 looper-1.4.2/looper/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:18:56.345370 looper-1.4.2/looper/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-31 21:18:47.000000 looper-1.4.2/looper/schemas/pipeline_interface_schema_generic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-31 21:18:47.000000 looper-1.4.2/looper/schemas/pipeline_interface_schema_project.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-31 21:18:47.000000 looper-1.4.2/looper/schemas/pipeline_interface_schema_sample.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20474 2023-07-31 21:18:47.000000 looper-1.4.2/looper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:18:56.341370 looper-1.4.2/looper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-31 21:18:56.000000 looper-1.4.2/looper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-31 21:18:56.000000 looper-1.4.2/looper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 21:18:56.000000 looper-1.4.2/looper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-31 21:18:56.000000 looper-1.4.2/looper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-31 21:18:56.000000 looper-1.4.2/looper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-31 21:18:56.000000 looper-1.4.2/looper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:18:56.345370 looper-1.4.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-31 21:18:47.000000 looper-1.4.2/requirements/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-31 21:18:47.000000 looper-1.4.2/requirements/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-31 21:18:47.000000 looper-1.4.2/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-31 21:18:56.345370 looper-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-31 21:18:47.000000 looper-1.4.2/setup.py
```

### Comparing `looper-1.4.1/LICENSE.txt` & `looper-1.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/PKG-INFO` & `looper-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: looper
-Version: 1.4.1
+Version: 1.4.2
 Summary: A pipeline submission engine that parses sample inputs and submits pipelines for each sample.
 Home-page: https://github.com/pepkit/looper
 Author: Nathan Sheffield, Vince Reuter, Michal Stolarczyk, Johanna Klughammer, Andre Rendeiro
 License: BSD2
 Keywords: bioinformatics,sequencing,ngs
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `looper-1.4.1/README.md` & `looper-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/logo_looper.svg` & `looper-1.4.2/logo_looper.svg`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/__init__.py` & `looper-1.4.2/looper/__init__.py`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/_devtools.py` & `looper-1.4.2/looper/_devtools.py`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/conductor.py` & `looper-1.4.2/looper/conductor.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from jinja2.exceptions import UndefinedError
 
 from peppy.const import CONFIG_KEY, SAMPLE_NAME_ATTR, SAMPLE_YAML_EXT
 from peppy.exceptions import RemoteYAMLError
 from pipestat import PipestatError
 from ubiquerg import expandpath
 from yaml import dump
-from yacman import YAMLConfigManager
+from yacman import YAMLConfigManager, expandpath as expath
 
 from .const import *
 from .exceptions import JobSubmissionException
 from .processed_project import populate_sample_paths
 from .utils import fetch_sample_flags, jinja_render_template_strictly
 
 _LOGGER = logging.getLogger(__name__)
@@ -726,14 +726,16 @@
             pl_iface = {}
             pl_iface.update(self.pl_iface)
             pl_iface[VAR_TEMPL_KEY] = self.pl_iface.render_var_templates(
                 namespaces=namespaces
             )
             _LOGGER.debug(f"namespace pipelines: { pl_iface }")
             namespaces["pipeline"]["var_templates"] = pl_iface[VAR_TEMPL_KEY]
+            for k, v in namespaces["pipeline"]["var_templates"].items():
+                namespaces["pipeline"]["var_templates"][k] = expath(v)
             # pre_submit hook namespace updates
             namespaces = _exec_pre_submit(pl_iface, namespaces)
             self._rendered_ok = False
             try:
                 argstring = jinja_render_template_strictly(
                     template=templ, namespaces=namespaces
                 )
```

### Comparing `looper-1.4.1/looper/const.py` & `looper-1.4.2/looper/const.py`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/exceptions.py` & `looper-1.4.2/looper/exceptions.py`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/html_reports.py` & `looper-1.4.2/looper/html_reports.py`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/html_reports_pipestat.py` & `looper-1.4.2/looper/html_reports_pipestat.py`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/html_reports_project_pipestat.py` & `looper-1.4.2/looper/html_reports_project_pipestat.py`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/jinja_templates/footer_index.html` & `looper-1.4.2/looper/jinja_templates/footer_index.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/jinja_templates/head.html` & `looper-1.4.2/looper/jinja_templates/head.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/jinja_templates/index.html` & `looper-1.4.2/looper/jinja_templates/index.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/jinja_templates/logo.html` & `looper-1.4.2/looper/jinja_templates/logo.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/jinja_templates/navbar.html` & `looper-1.4.2/looper/jinja_templates/navbar.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/jinja_templates/navbar_links.html` & `looper-1.4.2/looper/jinja_templates/navbar_links.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/jinja_templates/navbar_list_parent.html` & `looper-1.4.2/looper/jinja_templates/navbar_list_parent.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/jinja_templates/object.html` & `looper-1.4.2/looper/jinja_templates/object.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/jinja_templates/project_object.html` & `looper-1.4.2/looper/jinja_templates/project_object.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/jinja_templates/sample.html` & `looper-1.4.2/looper/jinja_templates/sample.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/jinja_templates/status_table.html` & `looper-1.4.2/looper/jinja_templates/status_table.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/jinja_templates/status_table_no_links.html` & `looper-1.4.2/looper/jinja_templates/status_table_no_links.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/jinja_templates_old/footer_index.html` & `looper-1.4.2/looper/jinja_templates_old/footer_index.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/jinja_templates_old/head.html` & `looper-1.4.2/looper/jinja_templates_old/head.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/jinja_templates_old/index.html` & `looper-1.4.2/looper/jinja_templates_old/index.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/jinja_templates_old/logo.html` & `looper-1.4.2/looper/jinja_templates_old/logo.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/jinja_templates_old/navbar.html` & `looper-1.4.2/looper/jinja_templates_old/navbar.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/jinja_templates_old/navbar_links.html` & `looper-1.4.2/looper/jinja_templates_old/navbar_links.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/jinja_templates_old/navbar_list_parent.html` & `looper-1.4.2/looper/jinja_templates_old/navbar_list_parent.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/jinja_templates_old/object.html` & `looper-1.4.2/looper/jinja_templates_old/object.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/jinja_templates_old/project_object.html` & `looper-1.4.2/looper/jinja_templates_old/project_object.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/jinja_templates_old/sample.html` & `looper-1.4.2/looper/jinja_templates_old/sample.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/jinja_templates_old/status_table.html` & `looper-1.4.2/looper/jinja_templates_old/status_table.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/jinja_templates_old/status_table_no_links.html` & `looper-1.4.2/looper/jinja_templates_old/status_table_no_links.html`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/looper.py` & `looper-1.4.2/looper/looper.py`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/parser_types.py` & `looper-1.4.2/looper/parser_types.py`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/pipeline_interface.py` & `looper-1.4.2/looper/pipeline_interface.py`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/processed_project.py` & `looper-1.4.2/looper/processed_project.py`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/project.py` & `looper-1.4.2/looper/project.py`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/schemas/pipeline_interface_schema_generic.yaml` & `looper-1.4.2/looper/schemas/pipeline_interface_schema_generic.yaml`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/schemas/pipeline_interface_schema_project.yaml` & `looper-1.4.2/looper/schemas/pipeline_interface_schema_project.yaml`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/schemas/pipeline_interface_schema_sample.yaml` & `looper-1.4.2/looper/schemas/pipeline_interface_schema_sample.yaml`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper/utils.py` & `looper-1.4.2/looper/utils.py`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/looper.egg-info/PKG-INFO` & `looper-1.4.2/looper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: looper
-Version: 1.4.1
+Version: 1.4.2
 Summary: A pipeline submission engine that parses sample inputs and submits pipelines for each sample.
 Home-page: https://github.com/pepkit/looper
 Author: Nathan Sheffield, Vince Reuter, Michal Stolarczyk, Johanna Klughammer, Andre Rendeiro
 License: BSD2
 Keywords: bioinformatics,sequencing,ngs
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `looper-1.4.1/looper.egg-info/SOURCES.txt` & `looper-1.4.2/looper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `looper-1.4.1/setup.py` & `looper-1.4.2/setup.py`

 * *Files identical despite different names*

