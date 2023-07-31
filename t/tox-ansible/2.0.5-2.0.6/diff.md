# Comparing `tmp/tox-ansible-2.0.5.tar.gz` & `tmp/tox-ansible-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tox-ansible-2.0.5.tar", last modified: Tue May 16 12:09:11 2023, max compression
+gzip compressed data, was "tox-ansible-2.0.6.tar", last modified: Mon Jul 31 21:01:46 2023, max compression
```

## Comparing `tox-ansible-2.0.5.tar` & `tox-ansible-2.0.6.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:09:11.565381 tox-ansible-2.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:09:11.557381 tox-ansible-2.0.5/.config/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/.config/dictionary.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/.config/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/.config/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/.config/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/.darglint
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:09:11.557381 tox-ansible-2.0.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:09:11.557381 tox-ansible-2.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/.github/workflows/run.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-05-16 12:09:11.565381 tox-ansible-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/cspell.config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:09:11.561381 tox-ansible-2.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/docs/galaxy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/docs/integration.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/docs/sanity.ini
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/docs/tox-ansible.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/docs/unit.ini
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 12:09:11.565381 tox-ansible-2.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:09:11.549381 tox-ansible-2.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:09:11.561381 tox-ansible-2.0.5/src/tox_ansible/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/src/tox_ansible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-16 12:09:11.000000 tox-ansible-2.0.5/src/tox_ansible/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16200 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/src/tox_ansible/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:09:11.561381 tox-ansible-2.0.5/src/tox_ansible.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-05-16 12:09:11.000000 tox-ansible-2.0.5/src/tox_ansible.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-16 12:09:11.000000 tox-ansible-2.0.5/src/tox_ansible.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 12:09:11.000000 tox-ansible-2.0.5/src/tox_ansible.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-16 12:09:11.000000 tox-ansible-2.0.5/src/tox_ansible.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-16 12:09:11.000000 tox-ansible-2.0.5/src/tox_ansible.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 12:09:11.000000 tox-ansible-2.0.5/src/tox_ansible.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:09:11.565381 tox-ansible-2.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:09:11.549381 tox-ansible-2.0.5/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:09:11.549381 tox-ansible-2.0.5/tests/fixtures/integration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:09:11.565381 tox-ansible-2.0.5/tests/fixtures/integration/test_basic/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/tests/fixtures/integration/test_basic/galaxy.yml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/tests/fixtures/integration/test_basic/tox-ansible.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:09:11.565381 tox-ansible-2.0.5/tests/fixtures/integration/test_user_provided/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/tests/fixtures/integration/test_user_provided/galaxy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/tests/fixtures/integration/test_user_provided/tox-ansible.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:09:11.565381 tox-ansible-2.0.5/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/tests/integration/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/tests/integration/test_user_provided.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-16 12:08:56.000000 tox-ansible-2.0.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:01:46.475579 tox-ansible-2.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:01:46.459579 tox-ansible-2.0.6/.config/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/.config/dictionary.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/.config/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/.config/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/.config/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/.darglint
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:01:46.459579 tox-ansible-2.0.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:01:46.463579 tox-ansible-2.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/.github/workflows/run.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-07-31 21:01:46.471579 tox-ansible-2.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/cspell.config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:01:46.463579 tox-ansible-2.0.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/docs/galaxy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/docs/integration.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/docs/sanity.ini
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/docs/tox-ansible.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/docs/unit.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 21:01:46.475579 tox-ansible-2.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:01:46.455579 tox-ansible-2.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:01:46.467579 tox-ansible-2.0.6/src/tox_ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/src/tox_ansible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-31 21:01:46.000000 tox-ansible-2.0.6/src/tox_ansible/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16194 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/src/tox_ansible/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:01:46.467579 tox-ansible-2.0.6/src/tox_ansible.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-07-31 21:01:46.000000 tox-ansible-2.0.6/src/tox_ansible.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-31 21:01:46.000000 tox-ansible-2.0.6/src/tox_ansible.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 21:01:46.000000 tox-ansible-2.0.6/src/tox_ansible.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-31 21:01:46.000000 tox-ansible-2.0.6/src/tox_ansible.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-31 21:01:46.000000 tox-ansible-2.0.6/src/tox_ansible.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-31 21:01:46.000000 tox-ansible-2.0.6/src/tox_ansible.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:01:46.471579 tox-ansible-2.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:01:46.455579 tox-ansible-2.0.6/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:01:46.455579 tox-ansible-2.0.6/tests/fixtures/integration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:01:46.471579 tox-ansible-2.0.6/tests/fixtures/integration/test_basic/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/tests/fixtures/integration/test_basic/galaxy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/tests/fixtures/integration/test_basic/tox-ansible.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:01:46.471579 tox-ansible-2.0.6/tests/fixtures/integration/test_user_provided/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/tests/fixtures/integration/test_user_provided/galaxy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/tests/fixtures/integration/test_user_provided/tox-ansible.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:01:46.471579 tox-ansible-2.0.6/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/tests/integration/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/tests/integration/test_user_provided.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-31 21:01:26.000000 tox-ansible-2.0.6/tox.ini
```

### Comparing `tox-ansible-2.0.5/.flake8` & `tox-ansible-2.0.6/.flake8`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.5/.github/workflows/release.yml` & `tox-ansible-2.0.6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.5/.github/workflows/run.yml` & `tox-ansible-2.0.6/.github/workflows/run.yml`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.5/.github/workflows/tox.yml` & `tox-ansible-2.0.6/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.5/.gitignore` & `tox-ansible-2.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.5/.pre-commit-config.yaml` & `tox-ansible-2.0.6/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -8,62 +8,62 @@
       - id: debug-statements
       - id: end-of-file-fixer
       - id: no-commit-to-branch
         args: [--branch, main]
       - id: trailing-whitespace
 
   - repo: https://github.com/asottile/add-trailing-comma.git
-    rev: v2.4.0
+    rev: v3.0.1
     hooks:
       - id: add-trailing-comma
         args:
           - --py36-plus
 
   - repo: https://github.com/Lucas-C/pre-commit-hooks.git
     rev: v1.5.1
     hooks:
       - id: remove-tabs
 
   - repo: https://github.com/pre-commit/mirrors-prettier
     # keep it before yamllint
-    rev: v3.0.0-alpha.9-for-vscode
+    rev: v3.0.0
     hooks:
       - id: prettier
         always_run: true
         additional_dependencies:
           - prettier
           - prettier-plugin-toml
           - prettier-plugin-sort-json
 
   - repo: https://github.com/psf/black
-    rev: 23.3.0
+    rev: 23.7.0
     hooks:
       - id: black
 
   - repo: https://github.com/tox-dev/tox-ini-fmt
-    rev: "1.3.0"
+    rev: "1.3.1"
     hooks:
       - id: tox-ini-fmt
 
-  - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.0.267"
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: "v0.0.280"
     hooks:
       - id: ruff
         args:
           - "--exit-non-zero-on-fix"
 
   - repo: https://github.com/streetsidesoftware/cspell-cli
-    rev: v6.31.0
+    rev: v6.31.1
     hooks:
       - id: cspell
         name: Spell check with cspell
 
   # untill ruff has parity with darglint
   - repo: https://github.com/PyCQA/flake8.git
-    rev: 6.0.0
+    rev: 6.1.0
     hooks:
       - id: flake8
         language_version: python3
         additional_dependencies:
           - darglint
           - flake8-docstrings
 
@@ -75,15 +75,15 @@
           - --output-format=colorized
         additional_dependencies:
           - pytest
           - tox
           - pyyaml
 
   - repo: https://github.com/pre-commit/mirrors-mypy.git
-    rev: v1.3.0
+    rev: v1.4.1
     hooks:
       - id: mypy
         additional_dependencies:
           - pytest
           - tox
           - types-PyYAML
         args:
```

### Comparing `tox-ansible-2.0.5/LICENSE` & `tox-ansible-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.5/PKG-INFO` & `tox-ansible-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tox-ansible
-Version: 2.0.5
+Version: 2.0.6
 Summary: A radical approach to testing ansible content
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: MIT
 Keywords: ansible,collections,tox
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -226,15 +226,15 @@
 ]
 ```
 
 ## How does it work?
 
 `tox` will, by default, create a python virtual environment for a given environment. `tox-ansible` adds ansible collection specific build and test logic to tox. The collection is copied into the virtual environment created by tox, built, and installed into the virtual environment. The installation of the collection will include the collection's collection dependencies. `tox-ansible` will also install any python dependencies from a `test-requirements.txt` and `requirements.txt` file. The virtual environment's temporary directory is used, so the copy, build and install steps are performed with each test run ensuring the current collection code is used.
 
-`tox-ansible` also sets the `ANSIBLE_COLLECTIONS_PATHS` environment variable to point to the virtual environment's temporary directory. This ensures that the collection under test is used when running tests. The `pytest-ansible-units` pytest plugin injects the `ANSIBLE_COLLECTIONS_PATHS` environment variable into the collection loader so ansible-core can locate the collection.
+`tox-ansible` also sets the `ANSIBLE_COLLECTIONS_PATH` environment variable to point to the virtual environment's temporary directory. This ensures that the collection under test is used when running tests. The `pytest-ansible-units` pytest plugin injects the `ANSIBLE_COLLECTIONS_PATH` environment variable into the collection loader so ansible-core can locate the collection.
 
 `pytest` is ued to run both the `unit` and `integration tests`.
 `ansible-test sanity` is used to run the `sanity` tests.
 
 For a full configuration examples for each of the sanity, integration, and unit tests including the commands being run and the environments variables being set and passed, see the following:
 
 - [integration](docs/integration.ini)
```

### Comparing `tox-ansible-2.0.5/README.md` & `tox-ansible-2.0.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
 ]
 ```
 
 ## How does it work?
 
 `tox` will, by default, create a python virtual environment for a given environment. `tox-ansible` adds ansible collection specific build and test logic to tox. The collection is copied into the virtual environment created by tox, built, and installed into the virtual environment. The installation of the collection will include the collection's collection dependencies. `tox-ansible` will also install any python dependencies from a `test-requirements.txt` and `requirements.txt` file. The virtual environment's temporary directory is used, so the copy, build and install steps are performed with each test run ensuring the current collection code is used.
 
-`tox-ansible` also sets the `ANSIBLE_COLLECTIONS_PATHS` environment variable to point to the virtual environment's temporary directory. This ensures that the collection under test is used when running tests. The `pytest-ansible-units` pytest plugin injects the `ANSIBLE_COLLECTIONS_PATHS` environment variable into the collection loader so ansible-core can locate the collection.
+`tox-ansible` also sets the `ANSIBLE_COLLECTIONS_PATH` environment variable to point to the virtual environment's temporary directory. This ensures that the collection under test is used when running tests. The `pytest-ansible-units` pytest plugin injects the `ANSIBLE_COLLECTIONS_PATH` environment variable into the collection loader so ansible-core can locate the collection.
 
 `pytest` is ued to run both the `unit` and `integration tests`.
 `ansible-test sanity` is used to run the `sanity` tests.
 
 For a full configuration examples for each of the sanity, integration, and unit tests including the commands being run and the environments variables being set and passed, see the following:
 
 - [integration](docs/integration.ini)
```

### Comparing `tox-ansible-2.0.5/cspell.config.yaml` & `tox-ansible-2.0.6/cspell.config.yaml`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.5/docs/galaxy.yml` & `tox-ansible-2.0.6/docs/galaxy.yml`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.5/docs/integration.ini` & `tox-ansible-2.0.6/docs/integration.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [testenv:integration-py3.11-devel]
 type = VirtualEnvRunner
 set_env =
-  ANSIBLE_COLLECTIONS_PATHS=/home/bthornto/github/tox-ansible/docs/integration-py3.11-devel/tmp/collections/
+  ANSIBLE_COLLECTIONS_PATH=/home/bthornto/github/tox-ansible/docs/integration-py3.11-devel/tmp/collections/
   PIP_DISABLE_PIP_VERSION_CHECK=1
   PYTHONHASHSEED=3119075902
   PYTHONIOENCODING=utf-8
 base = testenv
 runner = virtualenv
 description = Integration tests using ansible-core devel and python 3.11
 depends =
```

### Comparing `tox-ansible-2.0.5/docs/sanity.ini` & `tox-ansible-2.0.6/docs/sanity.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [testenv:sanity-py3.11-devel]
 type = VirtualEnvRunner
 set_env =
-  ANSIBLE_COLLECTIONS_PATHS=/home/bthornto/github/tox-ansible/docs/sanity-py3.11-devel/tmp/collections/
+  ANSIBLE_COLLECTIONS_PATH=/home/bthornto/github/tox-ansible/docs/sanity-py3.11-devel/tmp/collections/
   PIP_DISABLE_PIP_VERSION_CHECK=1
   PYTHONHASHSEED=3868722208
   PYTHONIOENCODING=utf-8
 base = testenv
 runner = virtualenv
 description = Sanity tests using ansible-core devel and python 3.11
 depends =
```

### Comparing `tox-ansible-2.0.5/docs/unit.ini` & `tox-ansible-2.0.6/docs/unit.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [testenv:unit-py3.11-devel]
 type = VirtualEnvRunner
 set_env =
-  ANSIBLE_COLLECTIONS_PATHS=/home/bthornto/github/tox-ansible/docs/unit-py3.11-devel/tmp/collections/
+  ANSIBLE_COLLECTIONS_PATH=/home/bthornto/github/tox-ansible/docs/unit-py3.11-devel/tmp/collections/
   PIP_DISABLE_PIP_VERSION_CHECK=1
   PYTHONHASHSEED=1318243417
   PYTHONIOENCODING=utf-8
 base = testenv
 runner = virtualenv
 description = Unit tests using ansible-core devel and python 3.11
 depends =
```

### Comparing `tox-ansible-2.0.5/pyproject.toml` & `tox-ansible-2.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.5/requirements.txt` & `tox-ansible-2.0.6/requirements.txt`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.5/src/tox_ansible/plugin.py` & `tox-ansible-2.0.6/src/tox_ansible/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 # cspell:ignore envlist
 """tox plugin to emit a github matrix."""
 
+from __future__ import annotations
+
 import json
 import logging
 import os
 import re
 import sys
 import uuid
 
 from dataclasses import asdict, dataclass, field
 from pathlib import Path
-from typing import List, Tuple, TypeVar
+from typing import TYPE_CHECKING, TypeVar
 
 import yaml
 
-from tox.config.cli.parser import ToxParser
 from tox.config.loader.memory import MemoryLoader
 from tox.config.loader.section import Section
 from tox.config.loader.str_convert import StrConvert
 from tox.config.sets import ConfigSet, CoreConfigSet, EnvConfigSet
-from tox.config.types import EnvList
 from tox.plugin import impl
-from tox.session.state import State
 from tox.tox_env.python.api import PY_FACTORS_RE
 
 
+if TYPE_CHECKING:
+    from tox.config.cli.parser import ToxParser
+    from tox.config.types import EnvList
+    from tox.session.state import State
+
+
 ALLOWED_EXTERNALS = [
     "bash",
     "cp",
     "git",
     "rm",
     "rsync",
     "mkdir",
     "cd",
     "echo",
 ]
 ENV_LIST = """
 {integration, sanity, unit}-py3.7-2.9
 {integration, sanity, unit}-py3.8-{2.9, 2.12, 2.13}
-{integration, sanity, unit}-py3.9-{2.12, 2.13, 2.14, 2.15, milestone, devel}
+{integration, sanity, unit}-py3.9-{2.12, 2.13, 2.14, 2.15}
 {integration, sanity, unit}-py3.10-{2.12, 2.13, 2.14, 2.15, milestone, devel}
 {integration, sanity, unit}-py3.11-{2.14, 2.15, milestone, devel}
 """
 TOX_WORK_DIR = Path()
 OUR_DEPS = [
     "pytest",
     "pytest-xdist",
@@ -55,50 +60,50 @@
 class AnsibleConfigSet(ConfigSet):
     """The ansible configuration."""
 
     def register_config(self: T) -> None:
         """Register the ansible configuration."""
         self.add_config(
             "skip",
-            of_type=List[str],
+            of_type=list,
             default=[],
             desc="ansible configuration",
         )
 
 
 @dataclass
 class AnsibleTestConf:  # pylint: disable=too-many-instance-attributes
     """Ansible test configuration."""
 
     description: str
     deps: str
     setenv: str
     skip_install: bool
-    allowlist_externals: List[str] = field(default_factory=list)
-    commands_pre: List[str] = field(default_factory=list)
-    commands: List[str] = field(default_factory=list)
-    passenv: List[str] = field(default_factory=list)
+    allowlist_externals: list[str] = field(default_factory=list)
+    commands_pre: list[str] = field(default_factory=list)
+    commands: list[str] = field(default_factory=list)
+    passenv: list[str] = field(default_factory=list)
 
 
-def custom_sort(string: str) -> Tuple[int, ...]:
+def custom_sort(string: str) -> tuple[int, ...]:
     """Convert a env name into a tuple of ints.
 
     In the case of a string, use the ord() of the first two characters.
 
     :param string: The string to sort.
     :return: The tuple of converted values.
     """
     parts = re.split(r"\.|-|py", string)
     converted = []
     for part in parts:
         if not part:
             continue
         try:
             converted.append(int(part))
-        except ValueError:
+        except ValueError:  # noqa: PERF203
             num_part = "".join((str(ord(char)).rjust(3, "0")) for char in part[0:2])
             converted.append(int(num_part))
     return tuple(converted)
 
 
 @impl
 def tox_add_option(parser: ToxParser) -> None:
@@ -304,15 +309,15 @@
     else:
         encoded = f"envlist={value}\n"
 
     with Path(gh_output).open("a", encoding="utf-8") as fileh:
         fileh.write(encoded)
 
 
-def get_collection_name(galaxy_path: Path) -> Tuple[str, str]:
+def get_collection_name(galaxy_path: Path) -> tuple[str, str]:
     """Extract collection information from the galaxy.yml file.
 
     :param galaxy_path: The path to the galaxy.yml file.
     :return: The collection name.
     """
     try:
         with galaxy_path.open() as galaxy_file:
@@ -333,15 +338,15 @@
 
 
 def conf_commands(
     c_name: str,
     c_namespace: str,
     env_conf: EnvConfigSet,
     test_type: str,
-) -> List[str]:
+) -> list[str]:
     """Build the commands for the tox environment.
 
     :param c_name: The collection name.
     :param c_namespace: The collection namespace.
     :param test_type: The test type, either "integration", "unit", or "sanity".
     :param env_conf: The tox environment configuration object.
     :return: The commands to run.
@@ -361,15 +366,15 @@
     logging.critical(err)
     sys.exit(1)
 
 
 def conf_commands_for_integration_unit(
     env_conf: EnvConfigSet,
     test_type: str,
-) -> List[str]:
+) -> list[str]:
     """Build the commands for integration and unit tests.
 
     :param env_conf: The tox environment configuration object.
     :param test_type: The test type, either "integration" or "unit".
     :return: The command to run.
     """
     commands = []
@@ -385,41 +390,39 @@
     return commands
 
 
 def conf_commands_for_sanity(
     c_name: str,
     c_namespace: str,
     env_conf: EnvConfigSet,
-) -> List[str]:
+) -> list[str]:
     """Add commands for sanity tests.
 
     :param c_name: The collection name.
     :param c_namespace: The collection namespace.
     :param env_conf: The tox environment configuration object.
     :return: The commands to run.
     """
     commands = []
     envtmpdir = env_conf["envtmpdir"]
 
-    py_ver = env_conf["basepython"][0].replace("py", "")
-    if "." not in py_ver:
-        py_ver = f"{py_ver[0]}.{py_ver[1:]}"
+    py_ver = env_conf.name.split("-")[1].replace("py", "")
 
     command = f"ansible-test sanity --local --requirements --python {py_ver}"
     ch_dir = f"cd {envtmpdir}/collections/ansible_collections/{c_namespace}/{c_name}"
     full_command = f"bash -c '{ch_dir} && {command}'"
     commands.append(full_command)
     return commands
 
 
 def conf_commands_pre(
     env_conf: EnvConfigSet,
     c_name: str,
     c_namespace: str,
-) -> List[str]:
+) -> list[str]:
     """Build and install the collection.
 
     :param env_conf: The tox environment configuration object.
     :param c_name: The collection name.
     :param c_namespace: The collection namespace.
     :return: The commands to pre run.
     """
@@ -514,15 +517,15 @@
         ansible_package = f"{base_url}{ansible_version}.tar.gz"
     else:
         ansible_package = f"{base_url}stable-{ansible_version}.tar.gz"
     deps.append(ansible_package)
     return "\n".join(deps)
 
 
-def conf_passenv() -> List[str]:
+def conf_passenv() -> list[str]:
     """Build the pass environment variables for the tox environment.
 
     :return: The pass environment variables.
     """
     passenv = []
     passenv.append("GITHUB_TOKEN")
     return passenv
@@ -532,9 +535,9 @@
     """Build the set environment variables for the tox environment.
 
     :param env_conf: The environment configuration.
     :return: The set environment variables.
     """
     envtmpdir = env_conf["envtmpdir"]
     setenv = []
-    setenv.append(f"ANSIBLE_COLLECTIONS_PATHS={envtmpdir}/collections/")
+    setenv.append(f"ANSIBLE_COLLECTIONS_PATH={envtmpdir}/collections/")
     return "\n".join(setenv)
```

### Comparing `tox-ansible-2.0.5/src/tox_ansible.egg-info/PKG-INFO` & `tox-ansible-2.0.6/src/tox_ansible.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tox-ansible
-Version: 2.0.5
+Version: 2.0.6
 Summary: A radical approach to testing ansible content
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: MIT
 Keywords: ansible,collections,tox
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -226,15 +226,15 @@
 ]
 ```
 
 ## How does it work?
 
 `tox` will, by default, create a python virtual environment for a given environment. `tox-ansible` adds ansible collection specific build and test logic to tox. The collection is copied into the virtual environment created by tox, built, and installed into the virtual environment. The installation of the collection will include the collection's collection dependencies. `tox-ansible` will also install any python dependencies from a `test-requirements.txt` and `requirements.txt` file. The virtual environment's temporary directory is used, so the copy, build and install steps are performed with each test run ensuring the current collection code is used.
 
-`tox-ansible` also sets the `ANSIBLE_COLLECTIONS_PATHS` environment variable to point to the virtual environment's temporary directory. This ensures that the collection under test is used when running tests. The `pytest-ansible-units` pytest plugin injects the `ANSIBLE_COLLECTIONS_PATHS` environment variable into the collection loader so ansible-core can locate the collection.
+`tox-ansible` also sets the `ANSIBLE_COLLECTIONS_PATH` environment variable to point to the virtual environment's temporary directory. This ensures that the collection under test is used when running tests. The `pytest-ansible-units` pytest plugin injects the `ANSIBLE_COLLECTIONS_PATH` environment variable into the collection loader so ansible-core can locate the collection.
 
 `pytest` is ued to run both the `unit` and `integration tests`.
 `ansible-test sanity` is used to run the `sanity` tests.
 
 For a full configuration examples for each of the sanity, integration, and unit tests including the commands being run and the environments variables being set and passed, see the following:
 
 - [integration](docs/integration.ini)
```

### Comparing `tox-ansible-2.0.5/src/tox_ansible.egg-info/SOURCES.txt` & `tox-ansible-2.0.6/src/tox_ansible.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.5/tests/conftest.py` & `tox-ansible-2.0.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.5/tests/integration/test_basic.py` & `tox-ansible-2.0.6/tests/integration/test_basic.py`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.5/tests/integration/test_user_provided.py` & `tox-ansible-2.0.6/tests/integration/test_user_provided.py`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.5/tox.ini` & `tox-ansible-2.0.6/tox.ini`

 * *Files identical despite different names*

