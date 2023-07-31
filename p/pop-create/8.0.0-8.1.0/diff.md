# Comparing `tmp/pop_create-8.0.0.tar.gz` & `tmp/pop_create-8.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pop_create-8.0.0.tar", last modified: Mon Jul 17 13:35:07 2023, max compression
+gzip compressed data, was "pop_create-8.1.0.tar", last modified: Mon Jul 31 18:19:13 2023, max compression
```

## Comparing `pop_create-8.0.0.tar` & `pop_create-8.1.0.tar`

### file list

```diff
@@ -1,86 +1,87 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.980431 pop_create-8.0.0/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-07-17 13:34:53.000000 pop_create-8.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       56 2023-07-17 13:34:53.000000 pop_create-8.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4372 2023-07-17 13:35:07.980431 pop_create-8.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3278 2023-07-17 13:34:53.000000 pop_create-8.0.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.976431 pop_create-8.0.0/pop_create/
--rw-r--r--   0 root         (0) root         (0)     2280 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.976431 pop_create-8.0.0/pop_create/pop_create/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.972431 pop_create-8.0.0/pop_create/pop_create/cicd/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.976431 pop_create-8.0.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/
--rw-r--r--   0 root         (0) root         (0)      653 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.coveragerc
--rw-r--r--   0 root         (0) root         (0)     1066 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)     5546 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)       69 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/build.conf
--rw-r--r--   0 root         (0) root         (0)     7978 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/noxfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.976431 pop_create-8.0.0/pop_create/pop_create/docs/
--rw-r--r--   0 root         (0) root         (0)      220 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/docs/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.976431 pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/
--rw-r--r--   0 root         (0) root         (0)       37 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/.rstcheck.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.976431 pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/
--rw-r--r--   0 root         (0) root         (0)     9591 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)      781 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.976431 pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/releases/
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/releases/index.rst
--rw-r--r--   0 root         (0) root         (0)      175 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/releases/{{cookiecutter.version_number}}.rst
--rw-r--r--   0 root         (0) root         (0)       64 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/sitevars.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.976431 pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/topics/
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/topics/contributing.rst
--rw-r--r--   0 root         (0) root         (0)      227 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/topics/license.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.976431 pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/tutorial/
--rw-r--r--   0 root         (0) root         (0)      143 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/tutorial/example.rst
--rw-r--r--   0 root         (0) root         (0)       76 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/tutorial/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.976431 pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/requirements/
--rw-r--r--   0 root         (0) root         (0)      125 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/requirements/docs.txt
--rw-r--r--   0 root         (0) root         (0)     4737 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.976431 pop_create-8.0.0/pop_create/pop_create/seed/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.976431 pop_create-8.0.0/pop_create/pop_create/seed/hooks/
--rw-r--r--   0 root         (0) root         (0)      473 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/seed/hooks/post_gen_project.py
--rw-r--r--   0 root         (0) root         (0)      374 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/seed/hooks/pre_gen_project.py
--rw-r--r--   0 root         (0) root         (0)      301 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/seed/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.976431 pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/
--rw-r--r--   0 root         (0) root         (0)     2390 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/.gitignore
--rw-r--r--   0 root         (0) root         (0)      366 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/.pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     8748 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/CONTRIBUTING.rst
--rw-r--r--   0 root         (0) root         (0)    11375 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3425 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.976431 pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/requirements/
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/requirements/base.txt
--rw-r--r--   0 root         (0) root         (0)      118 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/run.py
--rw-r--r--   0 root         (0) root         (0)       34 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2928 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.976431 pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
--rw-r--r--   0 root         (0) root         (0)     1243 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/conf.py
--rw-r--r--   0 root         (0) root         (0)      188 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/scripts.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.976431 pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/{{cookiecutter.clean_name}}/
--rw-r--r--   0 root         (0) root         (0)      908 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/{{cookiecutter.clean_name}}/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.972431 pop_create-8.0.0/pop_create/pop_create/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.980431 pop_create-8.0.0/pop_create/pop_create/tests/hooks/
--rw-r--r--   0 root         (0) root         (0)      899 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/tests/hooks/post_gen_project.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.980431 pop_create-8.0.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/
--rw-r--r--   0 root         (0) root         (0)       49 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/pytest.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.980431 pop_create-8.0.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/requirements/
--rw-r--r--   0 root         (0) root         (0)       67 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/requirements/tests.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.976431 pop_create-8.0.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.980431 pop_create-8.0.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/integration/
--rw-r--r--   0 root         (0) root         (0)      881 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/integration/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.980431 pop_create-8.0.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/integration/{{cookiecutter.clean_name}}/
--rw-r--r--   0 root         (0) root         (0)      166 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/integration/{{cookiecutter.clean_name}}/test_init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.980431 pop_create-8.0.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/unit/
--rw-r--r--   0 root         (0) root         (0)      766 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/unit/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.980431 pop_create-8.0.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/unit/{{cookiecutter.clean_name}}/
--rw-r--r--   0 root         (0) root         (0)      305 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/unit/{{cookiecutter.clean_name}}/test_init.py
--rw-r--r--   0 root         (0) root         (0)      151 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/scripts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.980431 pop_create-8.0.0/pop_create/tool/
--rw-r--r--   0 root         (0) root         (0)     2119 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/tool/path.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-17 13:35:07.000000 pop_create-8.0.0/pop_create/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.976431 pop_create-8.0.0/pop_create.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4372 2023-07-17 13:35:07.000000 pop_create-8.0.0/pop_create.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3280 2023-07-17 13:35:07.000000 pop_create-8.0.0/pop_create.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 13:35:07.000000 pop_create-8.0.0/pop_create.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-07-17 13:35:07.000000 pop_create-8.0.0/pop_create.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-07-17 13:35:07.000000 pop_create-8.0.0/pop_create.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-17 13:35:07.000000 pop_create-8.0.0/pop_create.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-17 13:35:07.980431 pop_create-8.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2814 2023-07-17 13:34:53.000000 pop_create-8.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-07-31 18:18:58.000000 pop_create-8.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       56 2023-07-31 18:18:58.000000 pop_create-8.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4372 2023-07-31 18:19:13.567263 pop_create-8.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3278 2023-07-31 18:18:58.000000 pop_create-8.1.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/
+-rw-r--r--   0 root         (0) root         (0)     2334 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.559263 pop_create-8.1.0/pop_create/pop_create/cicd/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/
+-rw-r--r--   0 root         (0) root         (0)      653 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)     5546 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)       69 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/build.conf
+-rw-r--r--   0 root         (0) root         (0)    13448 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/noxfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/docs/
+-rw-r--r--   0 root         (0) root         (0)      220 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/docs/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/
+-rw-r--r--   0 root         (0) root         (0)       37 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/.rstcheck.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/_includes/
+-rw-r--r--   0 root         (0) root         (0)      117 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/_includes/modindex-note.rst
+-rw-r--r--   0 root         (0) root         (0)      112 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/_includes/reference-toc-template.rst
+-rw-r--r--   0 root         (0) root         (0)    11003 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)      881 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      194 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/py-modindex.rst
+-rw-r--r--   0 root         (0) root         (0)       64 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/sitevars.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/topics/
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/topics/contributing.rst
+-rw-r--r--   0 root         (0) root         (0)      227 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/topics/license.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/tutorial/
+-rw-r--r--   0 root         (0) root         (0)      204 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/tutorial/example.rst
+-rw-r--r--   0 root         (0) root         (0)       76 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/tutorial/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/requirements/
+-rw-r--r--   0 root         (0) root         (0)      139 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/requirements/docs.txt
+-rw-r--r--   0 root         (0) root         (0)     4809 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/seed/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/seed/hooks/
+-rw-r--r--   0 root         (0) root         (0)      473 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/seed/hooks/post_gen_project.py
+-rw-r--r--   0 root         (0) root         (0)      374 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/seed/hooks/pre_gen_project.py
+-rw-r--r--   0 root         (0) root         (0)      301 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/seed/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/
+-rw-r--r--   0 root         (0) root         (0)     2459 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      366 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/.pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)    10301 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/CONTRIBUTING.rst
+-rw-r--r--   0 root         (0) root         (0)    11375 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3425 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/requirements/
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/requirements/base.txt
+-rw-r--r--   0 root         (0) root         (0)      118 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/run.py
+-rw-r--r--   0 root         (0) root         (0)       34 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2928 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
+-rw-r--r--   0 root         (0) root         (0)     1243 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/conf.py
+-rw-r--r--   0 root         (0) root         (0)      188 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/scripts.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/{{cookiecutter.clean_name}}/
+-rw-r--r--   0 root         (0) root         (0)      908 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/{{cookiecutter.clean_name}}/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.559263 pop_create-8.1.0/pop_create/pop_create/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/tests/hooks/
+-rw-r--r--   0 root         (0) root         (0)      899 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/tests/hooks/post_gen_project.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/
+-rw-r--r--   0 root         (0) root         (0)       49 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/pytest.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/requirements/
+-rw-r--r--   0 root         (0) root         (0)       67 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/requirements/tests.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.559263 pop_create-8.1.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)      881 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/integration/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/integration/{{cookiecutter.clean_name}}/
+-rw-r--r--   0 root         (0) root         (0)      166 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/integration/{{cookiecutter.clean_name}}/test_init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)      766 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/unit/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/unit/{{cookiecutter.clean_name}}/
+-rw-r--r--   0 root         (0) root         (0)      305 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/unit/{{cookiecutter.clean_name}}/test_init.py
+-rw-r--r--   0 root         (0) root         (0)      151 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/scripts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create/tool/
+-rw-r--r--   0 root         (0) root         (0)     2119 2023-07-31 18:18:58.000000 pop_create-8.1.0/pop_create/tool/path.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-31 18:19:13.000000 pop_create-8.1.0/pop_create/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:19:13.563264 pop_create-8.1.0/pop_create.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4372 2023-07-31 18:19:13.000000 pop_create-8.1.0/pop_create.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3355 2023-07-31 18:19:13.000000 pop_create-8.1.0/pop_create.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 18:19:13.000000 pop_create-8.1.0/pop_create.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-07-31 18:19:13.000000 pop_create-8.1.0/pop_create.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-07-31 18:19:13.000000 pop_create-8.1.0/pop_create.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-31 18:19:13.000000 pop_create-8.1.0/pop_create.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-31 18:19:13.567263 pop_create-8.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2814 2023-07-31 18:18:58.000000 pop_create-8.1.0/setup.py
```

### Comparing `pop_create-8.0.0/LICENSE` & `pop_create-8.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pop_create-8.0.0/PKG-INFO` & `pop_create-8.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop_create
-Version: 8.0.0
+Version: 8.1.0
 Summary: Create new pop projects
 Home-page: https://vmware.gitlab.io/pop/pop-create/en/latest/index.html
 Author: VMware, Inc.
 Author-email: idemproject@vmware.com
 License: Apache Software License 2.0
 Project-URL: Code, https://gitlab.com/vmware/pop/pop-create
 Project-URL: Issue tracker, https://gitlab.com/vmware/pop/pop-create/issues
```

### Comparing `pop_create-8.0.0/README.rst` & `pop_create-8.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `pop_create-8.0.0/pop_create/conf.py` & `pop_create-8.1.0/pop_create/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 CLI_CONFIG = {
     "config": {"options": ["-c"], "subcommands": ["_global_"]},
-    "author": {},
-    "author_email": {},
+    "author": {"subcommands": ["_global_"]},
+    "author_email": {"subcommands": ["_global_"]},
     "project_name": {
         "subcommands": ["_global_"],
         "options": ["-n", "--name"],
     },
     "dyne": {"subcommands": ["_global_"], "options": ["-d"]},
     "overwrite_existing": {
         "options": ["--overwrite", "-o"],
```

### Comparing `pop_create-8.0.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.coveragerc` & `pop_create-8.1.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.coveragerc`

 * *Files identical despite different names*

### Comparing `pop_create-8.0.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.gitlab-ci.yml` & `pop_create-8.1.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.gitlab-ci.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 ---
 stages:
   - pre-commit
   - test-suite
+  - pkg
   - pop-release
 
 include:
   - project: saltstack/pop/cicd/ci-templates
     file: /lint/pre-commit-run-all.yml
   - project: saltstack/pop/cicd/ci-templates
     file: /release/pop_release.yml
@@ -45,7 +46,20 @@
 tests-3.10:
   extends: .test-suite
   image: python:3.10
 
 tests-3.11:
   extends: .test-suite
   image: python:3.11
+
+build-docs-html:
+  stage: test-suite
+
+pages:
+  variables:
+    CICD_DOCS_VERSION_LATEST: latest
+  stage: pkg
+
+publish-docs:
+  variables:
+    # TODO: Set this variable to the location where generated docs will be published
+    CICD_S3_DEST_PATH: ""
```

### Comparing `pop_create-8.0.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.pre-commit-config.yaml` & `pop_create-8.1.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/conf.py` & `pop_create-8.1.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 # full list see the documentation:
 # http://www.sphinx-doc.org/en/master/config
 # -- Path setup --------------------------------------------------------------
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
-# import os
-# import sys
-# sys.path.insert(0, os.path.abspath('.'))
 import datetime
+import os
+import sys
 from pathlib import Path
 
+# Required for autodoc
+sys.path.insert(0, os.path.abspath(".."))
+
 # -- Project information -----------------------------------------------------
 this_year = datetime.datetime.today().year
 if this_year == {{cookiecutter.this_year}}:
     copyright_year = {{cookiecutter.this_year}}
 else:
     copyright_year = f"{{cookiecutter.this_year}} - {this_year}"
 project = "{{cookiecutter.project_name}}"
@@ -49,15 +51,17 @@
 #
 needs_sphinx = "5.2.3"
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
+    "notfound.extension",
     "sphinx_copybutton",
+    "sphinx_design",
     "sphinx.ext.autodoc",
     "sphinx.ext.autosummary",
     "sphinx.ext.napoleon",
     "sphinx.ext.intersphinx",
     "sphinx.ext.viewcode",
     "sphinx.ext.todo",
     "sphinx.ext.coverage",
@@ -79,44 +83,57 @@
 
 # The master toctree document.
 master_doc = "index"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
+
 exclude_patterns = [
     "_build",
     "Thumbs.db",
     ".DS_Store",
     ".vscode",
     ".venv",
     ".git",
     ".gitlab-ci",
     ".gitignore",
     "sitevars.rst",
+    "_includes/reference-toc.rst",
+    "_includes/reference-toc-template.rst",
+    "_includes/modindex-note.rst",
+    "_includes/ref/exec/index",
+    "_includes/ref/states/index",
+    "redirector.html",
 ]
 
-autosummary_generate = True
+# ----- autosectionlabel Config ----------------------------------------------
+# autosectionlabel_prefix_document = True
+# autosectionlabel_maxdepth = 1
+nitpick_ignore_regex = [("py:class", r"types\..*")]
 
 # ----- Napolean Config ------------------------------------------------------
 # For using Google-style docstrings in Python code as a standard, which is
 # highly recommended. This improves tooling by expecting a standard way of
 # using docstrings in your project.
 # https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html
 napoleon_google_docstring = True
 napoleon_numpy_docstring = False
-napoleon_include_init_with_doc = True
+napoleon_include_init_with_doc = False
 napoleon_include_private_with_doc = False
 napoleon_include_special_with_doc = True
 napoleon_use_admonition_for_examples = False
-napoleon_use_admonition_for_notes = False
-napoleon_use_admonition_for_references = False
+napoleon_use_admonition_for_notes = True
+napoleon_use_admonition_for_references = True
 napoleon_use_ivar = False
 napoleon_use_param = True
 napoleon_use_rtype = True
+napoleon_preprocess_types = False
+napoleon_type_aliases = None
+napoleon_attr_annotations = True
 
 # ----- Intersphinx Config ---------------------------------------------------
 # This extension can generate automatic links to the documentation of objects
 # in other projects, such as the official Python or POP docs.
 # https://www.sphinx-doc.org/en/master/usage/extensions/intersphinx.html
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
@@ -134,131 +151,111 @@
 # This extension generates function/method/attribute summary lists, similar to
 # those output e.g. by Epydoc and other API doc generation tools. This is
 # especially useful when your docstrings are long and detailed, and putting
 # each one of them on a separate page makes them easier to read.
 # https://www.sphinx-doc.org/en/master/usage/extensions/autosummary.html
 autosummary_generate = True
 
+# If true, autosummary overwrites existing files by generated stub pages.
+# Defaults to true (enabled).
+autosummary_generate_overwrite = False
+
+# Automatically extract typehints when specified and place them in
+# descriptions of the relevant function/method.
+# autodoc_typehints = "description"
+
+# Don't show class signature with the class' name.
+# autodoc_class_signature = "separated"
+
+# A list of prefixes that are ignored for sorting the Python module index
+# (e.g., if this is set to ['foo.'], then foo.bar is shown under B, not F).
+# This can be handy if you document a project that consists of a single package.
+# Works only for the HTML builder currently.
+# Generates HTML page at <html-root>/py-modindex.html
+# Default is [].
+# We only care about {{cookiecutter.docs_modindex_common_prefix}} module directories
+modindex_common_prefix = {{cookiecutter.docs_modindex_common_prefix}}
+
+# Sphinx autoapi settings
+# autoapi_dirs = ['../idem_posix']
+# autoapi_type = "python"
+# autoapi_template_dir = "_templates/autoapi"
+
+# https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#confval-autodoc_typehints
+# 'signature' – Show typehints in the signature (default)
+# 'description' – Show typehints as content of the function or method The typehints of overloaded functions or methods will still be represented in the signature.
+# 'none' – Do not show typehints
+# 'both' – Show typehints in the signature and as content of the function or method
+autodoc_typehints = "signature"
+
+# Keep the AutoAPI generated files on the filesystem after the run.
+# Useful for debugging or transitioning to manual documentation.
+# https://sphinx-autoapi.readthedocs.io/en/latest/reference/config.html#confval-autoapi_keep_files
+autoapi_keep_files = True
+
+# For information on available options
+# https://sphinx-autoapi.readthedocs.io/en/latest/reference/config.html#confval-autoapi_options
+autoapi_options = [
+    "members",  # Display children of an object
+    "undoc-members",  # Display objects that have no docstring
+    "show-inheritance",  # Display a list of base classes below the class signature.
+    "show-module-summary",  # Whether to include autosummary directives in generated module documentation
+    "imported-members",  # Display objects imported from the same top level package or module. The default module template does not include imported objects, even with this option enabled. The default package template does.
+]
+
+# In case building docs throws import errors, please add the top level package name below
+autodoc_mock_imports = ["dict_tools"]
+
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
 html_theme = "furo"
-html_title = f"{project} Documentation"
+html_title = f"{{cookiecutter.project_name}}"
 html_show_sourcelink = True  # False on private repos; True on public repos
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
+# TODO: Add logo and favicon images to the /docs/_static folder and enable this line
 # html_static_path = ["_static"]
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
 # For example, official Salt Project docs use images from the salt-branding-guide
 # https://gitlab.com/saltstack/open/salt-branding-guide/
 #
 # Example for >=4.0.0 of Sphinx (support for favicon via URL)
 # html_logo = "https://gitlab.com/saltstack/open/salt-branding-guide/-/raw/master/logos/SaltProject_altlogo_teal.png?inline=true"
 # Example for <4.0.0 of Sphinx, if added into _static/img/ and html_static_path is valid
+# TODO: Add logo image to /docs/_static folder and enable this line
 # html_logo = "_static/img/SaltProject_altlogo_teal.png"
 
 # The name of an image file (within the static path) to use as favicon of the
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large. Favicons can be up to at least 228x228. PNG
 # format is supported as well, not just .ico'
 # For example, official Salt Project docs use images from the salt-branding-guide
 # https://gitlab.com/saltstack/open/salt-branding-guide/
 #
 # Example for >=4.0.0 of Sphinx (support for favicon via URL)
 # html_favicon = "https://gitlab.com/saltstack/open/salt-branding-guide/-/raw/master/logos/SaltProject_Logomark_teal.png?inline=true"
 # Example for <4.0.0 of Sphinx, if added into _static/img/ and html_static_path is valid
+# TODO: Add favicon image to /docs/_static folder and enable this line
 # html_favicon = "_static/img/SaltProject_Logomark_teal.png"
 
 # Custom sidebar templates, must be a dictionary that maps document names
 # to template names.
 #
 # The default sidebars (for documents that don't match any pattern) are
 # defined by theme itself.  Builtin themes are using these templates by
 # default: ``['localtoc.html', 'relations.html', 'sourcelink.html',
 # 'searchbox.html']``.
 #
 # html_sidebars = {}
-
-
-# -- Options for HTMLHelp output ---------------------------------------------
-
-# Output file base name for HTML help builder.
-htmlhelp_basename = "{{cookiecutter.clean_name}}doc"
-
-
-# -- Options for LaTeX output ------------------------------------------------
-
-latex_elements = {
-    # The paper size ('letterpaper' or 'a4paper').
-    #
-    # 'papersize': 'letterpaper',
-    # The font size ('10pt', '11pt' or '12pt').
-    #
-    # 'pointsize': '10pt',
-    # Additional stuff for the LaTeX preamble.
-    #
-    # 'preamble': '',
-    # Latex figure (float) alignment
-    #
-    # 'figure_align': 'htbp',
-}
-
-# Grouping the document tree into LaTeX files. List of tuples
-# (source start file, target name, title,
-#  author, documentclass [howto, manual, or own class]).
-latex_documents = [
-    (
-        master_doc,
-        "{{cookiecutter.clean_name}}.tex",
-        "{{cookiecutter.project_name}} Documentation",
-        "{{cookiecutter.author}}",
-        "manual",
-    ),
-]
-
-
-# -- Options for manual page output ------------------------------------------
-
-# One entry per manual page. List of tuples
-# (source start file, name, description, authors, manual section).
-man_pages = [
-    (
-        master_doc,
-        "{{cookiecutter.clean_name}}",
-        "{{cookiecutter.project_name}} Documentation",
-        [author],
-        1,
-    )
-]
-
-
-# -- Options for Texinfo output ----------------------------------------------
-
-# Grouping the document tree into Texinfo files. List of tuples
-# (source start file, target name, title, author,
-#  dir menu entry, description, category)
-texinfo_documents = [
-    (
-        master_doc,
-        "{{cookiecutter.clean_name}}",
-        "{{cookiecutter.project_name}} Documentation",
-        author,
-        "{{cookiecutter.clean_name}}",
-        "One line description of project.",
-        "Miscellaneous",
-    ),
-]
-
-
-# -- Extension configuration -------------------------------------------------
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pop_create-8.0.0/pop_create/pop_create/init.py` & `pop_create-8.1.0/pop_create/pop_create/init.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,14 +96,16 @@
         author_email=author_email,
         clean_name=clean_name,
         dyne_list=dyne_list,
         project_name=project_name,
         short_dyne_list=short_dyne_list,
         this_year=str(datetime.datetime.today().year),
         target_directory=str(directory),
+        docs_modindex_common_prefix=[],
+        docs_autogen_config=[],
     )
 
     for key, value in hub.OPT.pop_create.items():
         # Don't overwrite any values we already sanitized
         if key in ("project_name", "directory", "author", "author_email"):
             continue
         ctx[key] = value
```

### Comparing `pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/.gitignore` & `pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/.gitignore`

 * *Files 13% similar despite different names*

```diff
@@ -68,14 +68,17 @@
 .webassets-cache
 
 # Scrapy stuff:
 .scrapy
 
 # Sphinx documentation
 docs/_build/
+# Sphinx docs autogen path
+docs/ref
+docs/_includes/reference-toc.rst
 
 # PyBuilder
 .pybuilder/
 target/
 
 # Jupyter Notebook
 .ipynb_checkpoints
```

### Comparing `pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/CONTRIBUTING.rst` & `pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/CONTRIBUTING.rst`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ================
 
 #. Have pre-requisites completed:
 
    * ``git``
    * ``nox``
    * ``pre-commit``
-   * Python 3.6+
+   * Python 3.7+
 
 #. Fork the project
 #. ``git clone`` your fork locally
 #. Create your feature branch (ex. ``git checkout -b amazing-feature``)
 #. Setup your local development environment
 
    .. code-block:: bash
@@ -70,15 +70,15 @@
 
 Prerequisites
 =============
 
 For local development, the following prerequisites are needed:
 
 * `git <https://git-scm.com/book/en/v2/Getting-Started-Installing-Git>`__
-* `Python 3.6+ <https://realpython.com/installing-python/>`__
+* `Python 3.7+ <https://realpython.com/installing-python/>`__
 * `Ability to create python venv <https://realpython.com/python-virtual-environments-a-primer/>`__
 
 Windows 10 users
 ----------------
 
 For the best experience, when contributing from a Windows OS to projects using
 Python-based tools like ``pre-commit``, we recommend setting up `Windows Subsystem
@@ -156,15 +156,15 @@
 
 From within your local copy of the forked repo:
 
 .. code-block:: bash
 
     # Setup venv
     python3 -m venv .venv
-    # If Python 3.6+ is in path as 'python', use the following instead:
+    # If Python 3.7+ is in path as 'python', use the following instead:
     # python -m venv .venv
 
     # Activate venv
     source .venv/bin/activate
     # On Windows, use instead:
     # .venv/Scripts/activate
 
@@ -249,14 +249,40 @@
     firefox docs/_build/html/index.html
 
 .. note::
 
     If you encounter an error, Sphinx may be pointing out formatting errors
     that need to be resolved in order for ``nox`` to properly generate the docs.
 
+
+URL validation with brok
+========================
+
+`brok <https://github.com/smallhadroncollider/brok>`__ is used in the testing pipeline as a way to verify URLs.
+
+We went with ``brok`` instead of the built-in Sphinx link validator because ``brok`` can scan files of
+any kind across a repository to do validations, as opposed to only files within scope of Sphinx docs. This
+makes the tool more versatile across our repositories.
+
+The output in the CI/CD logs should show which URLs are causing any problems. The links can be verified
+in your personal browser, and links can then be updated in the appropriate files if they have become
+out-dated.
+
+* If a URL or IP address is being used to provide an example, refer to the Google Style Guide on best
+  practices (ex. use ``example.com``, ``example.org``, IP addresses that don't exist on the internet, etc.).
+  This ensures that URL validation is simplified, with less exceptions, and isn't hitting an actual endpoint.
+  For more information: `Google Style Guide: Example domains and names <https://developers.google.com/style/examples>`__
+* If a URL is valid, but can't be easily verified (due to requiring login, or the site is preventing automated link
+  calls, or the link is an example dummy link, etc.), then the link should be added to the ``.brokignore``
+  file at the root of the repo.
+
+It is recommended that ``brok`` isn't ran locally, and is only done via pipeline, as otherwise
+your personal IP address will be reaching out to websites in a way that may be seen as behavior to be
+blocked.
+
 Testing a ``pop`` project
 =========================
 
 .. code-block:: bash
 
     # View all nox targets
     nox -l
```

### Comparing `pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/LICENSE` & `pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/LICENSE`

 * *Files identical despite different names*

### Comparing `pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/README.rst` & `pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/README.rst`

 * *Files identical despite different names*

### Comparing `pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/setup.py` & `pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/setup.py`

 * *Files identical despite different names*

### Comparing `pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/conf.py` & `pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/conf.py`

 * *Files identical despite different names*

### Comparing `pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/{{cookiecutter.clean_name}}/init.py` & `pop_create-8.1.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/{{cookiecutter.clean_name}}/init.py`

 * *Files identical despite different names*

### Comparing `pop_create-8.0.0/pop_create/pop_create/tests/hooks/post_gen_project.py` & `pop_create-8.1.0/pop_create/pop_create/tests/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `pop_create-8.0.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/integration/conftest.py` & `pop_create-8.1.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `pop_create-8.0.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/unit/conftest.py` & `pop_create-8.1.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `pop_create-8.0.0/pop_create/tool/path.py` & `pop_create-8.1.0/pop_create/tool/path.py`

 * *Files identical despite different names*

### Comparing `pop_create-8.0.0/pop_create.egg-info/PKG-INFO` & `pop_create-8.1.0/pop_create.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-create
-Version: 8.0.0
+Version: 8.1.0
 Summary: Create new pop projects
 Home-page: https://vmware.gitlab.io/pop/pop-create/en/latest/index.html
 Author: VMware, Inc.
 Author-email: idemproject@vmware.com
 License: Apache Software License 2.0
 Project-URL: Code, https://gitlab.com/vmware/pop/pop-create
 Project-URL: Issue tracker, https://gitlab.com/vmware/pop/pop-create/issues
```

### Comparing `pop_create-8.0.0/pop_create.egg-info/SOURCES.txt` & `pop_create-8.1.0/pop_create.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,18 @@
 pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.pre-commit-config.yaml
 pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/build.conf
 pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/noxfile.py
 pop_create/pop_create/docs/init.py
 pop_create/pop_create/docs/{{cookiecutter.root_dir}}/.rstcheck.cfg
 pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/conf.py
 pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/index.rst
+pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/py-modindex.rst
 pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/sitevars.rst
-pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/releases/index.rst
-pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/releases/{{cookiecutter.version_number}}.rst
+pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/_includes/modindex-note.rst
+pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/_includes/reference-toc-template.rst
 pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/topics/contributing.rst
 pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/topics/license.rst
 pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/tutorial/example.rst
 pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/tutorial/index.rst
 pop_create/pop_create/docs/{{cookiecutter.root_dir}}/requirements/docs.txt
 pop_create/pop_create/seed/init.py
 pop_create/pop_create/seed/hooks/post_gen_project.py
```

### Comparing `pop_create-8.0.0/setup.py` & `pop_create-8.1.0/setup.py`

 * *Files identical despite different names*

