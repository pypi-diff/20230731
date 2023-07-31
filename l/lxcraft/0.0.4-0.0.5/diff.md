# Comparing `tmp/lxcraft-0.0.4.tar.gz` & `tmp/lxcraft-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lxcraft-0.0.4.tar", last modified: Wed Jul 26 20:09:42 2023, max compression
+gzip compressed data, was "lxcraft-0.0.5.tar", last modified: Mon Jul 31 20:44:30 2023, max compression
```

## Comparing `lxcraft-0.0.4.tar` & `lxcraft-0.0.5.tar`

### file list

```diff
@@ -1,73 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:09:42.508579 lxcraft-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-26 20:09:33.000000 lxcraft-0.0.4/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:09:42.500579 lxcraft-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:09:42.504579 lxcraft-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-26 20:09:33.000000 lxcraft-0.0.4/.github/workflows/docker-test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-26 20:09:33.000000 lxcraft-0.0.4/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-07-26 20:09:33.000000 lxcraft-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-26 20:09:33.000000 lxcraft-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-26 20:09:33.000000 lxcraft-0.0.4/.python-version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:09:42.504579 lxcraft-0.0.4/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-26 20:09:33.000000 lxcraft-0.0.4/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-26 20:09:33.000000 lxcraft-0.0.4/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-26 20:09:33.000000 lxcraft-0.0.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-26 20:09:33.000000 lxcraft-0.0.4/Justfile
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-26 20:09:33.000000 lxcraft-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-26 20:09:33.000000 lxcraft-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-26 20:09:42.508579 lxcraft-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-26 20:09:33.000000 lxcraft-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:09:42.504579 lxcraft-0.0.4/develop/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-26 20:09:33.000000 lxcraft-0.0.4/develop/docker-bash
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-26 20:09:33.000000 lxcraft-0.0.4/develop/just-test.sh
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-26 20:09:33.000000 lxcraft-0.0.4/develop/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:09:42.504579 lxcraft-0.0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-26 20:09:33.000000 lxcraft-0.0.4/docs/debugging.md
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-26 20:09:33.000000 lxcraft-0.0.4/docs/resource.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:09:42.504579 lxcraft-0.0.4/lxcraft/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-26 20:09:33.000000 lxcraft-0.0.4/lxcraft/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:09:42.504579 lxcraft-0.0.4/lxcraft/debian/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-26 20:09:33.000000 lxcraft-0.0.4/lxcraft/debian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-26 20:09:33.000000 lxcraft-0.0.4/lxcraft/debian/apt_package.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-26 20:09:33.000000 lxcraft-0.0.4/lxcraft/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:09:42.504579 lxcraft-0.0.4/lxcraft/path/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-26 20:09:33.000000 lxcraft-0.0.4/lxcraft/path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-26 20:09:33.000000 lxcraft-0.0.4/lxcraft/path/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-26 20:09:33.000000 lxcraft-0.0.4/lxcraft/path/filecontent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-07-26 20:09:33.000000 lxcraft-0.0.4/lxcraft/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:09:42.504579 lxcraft-0.0.4/lxcraft/python/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-26 20:09:33.000000 lxcraft-0.0.4/lxcraft/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-26 20:09:33.000000 lxcraft-0.0.4/lxcraft/python/pip_package.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-26 20:09:33.000000 lxcraft-0.0.4/lxcraft/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-26 20:09:33.000000 lxcraft-0.0.4/lxcraft/system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:09:42.508579 lxcraft-0.0.4/lxcraft/user/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-26 20:09:33.000000 lxcraft-0.0.4/lxcraft/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-26 20:09:33.000000 lxcraft-0.0.4/lxcraft/user/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-26 20:09:42.000000 lxcraft-0.0.4/lxcraft/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:09:42.504579 lxcraft-0.0.4/lxcraft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-26 20:09:42.000000 lxcraft-0.0.4/lxcraft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-26 20:09:42.000000 lxcraft-0.0.4/lxcraft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 20:09:42.000000 lxcraft-0.0.4/lxcraft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-26 20:09:42.000000 lxcraft-0.0.4/lxcraft.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-26 20:09:42.000000 lxcraft-0.0.4/lxcraft.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-26 20:09:33.000000 lxcraft-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-26 20:09:33.000000 lxcraft-0.0.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 20:09:33.000000 lxcraft-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-26 20:09:33.000000 lxcraft-0.0.4/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-26 20:09:42.508579 lxcraft-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-26 20:09:33.000000 lxcraft-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:09:42.508579 lxcraft-0.0.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:09:42.508579 lxcraft-0.0.4/tests/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-26 20:09:33.000000 lxcraft-0.0.4/tests/templates/gunicorn_start
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-26 20:09:33.000000 lxcraft-0.0.4/tests/templates/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 20:09:33.000000 lxcraft-0.0.4/tests/templates/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-26 20:09:33.000000 lxcraft-0.0.4/tests/templates/wwwkindos.conf
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-26 20:09:33.000000 lxcraft-0.0.4/tests/test_apt_package.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-26 20:09:33.000000 lxcraft-0.0.4/tests/test_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-26 20:09:33.000000 lxcraft-0.0.4/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-26 20:09:33.000000 lxcraft-0.0.4/tests/test_fastapi_uvicorn_gunicorn_supervisor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-26 20:09:33.000000 lxcraft-0.0.4/tests/test_filecontent.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-26 20:09:33.000000 lxcraft-0.0.4/tests/test_pip_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-26 20:09:33.000000 lxcraft-0.0.4/tests/test_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-26 20:09:33.000000 lxcraft-0.0.4/tests/test_resourrce.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-26 20:09:33.000000 lxcraft-0.0.4/tests/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-26 20:09:33.000000 lxcraft-0.0.4/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:44:30.015621 lxcraft-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-31 20:44:16.000000 lxcraft-0.0.5/.cruft.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:44:30.003620 lxcraft-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:44:30.007620 lxcraft-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-31 20:44:16.000000 lxcraft-0.0.5/.github/workflows/docker-test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-31 20:44:16.000000 lxcraft-0.0.5/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-31 20:44:16.000000 lxcraft-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-31 20:44:16.000000 lxcraft-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-31 20:44:16.000000 lxcraft-0.0.5/.python-version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:44:30.007620 lxcraft-0.0.5/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-31 20:44:16.000000 lxcraft-0.0.5/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-31 20:44:16.000000 lxcraft-0.0.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 20:44:16.000000 lxcraft-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-31 20:44:16.000000 lxcraft-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-31 20:44:30.015621 lxcraft-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-31 20:44:16.000000 lxcraft-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:44:30.007620 lxcraft-0.0.5/develop/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-31 20:44:16.000000 lxcraft-0.0.5/develop/docker-bash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-31 20:44:16.000000 lxcraft-0.0.5/develop/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:44:30.007620 lxcraft-0.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-31 20:44:16.000000 lxcraft-0.0.5/docs/debugging.md
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-31 20:44:16.000000 lxcraft-0.0.5/docs/resource.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:44:30.011621 lxcraft-0.0.5/lxcraft/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-31 20:44:16.000000 lxcraft-0.0.5/lxcraft/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:44:30.011621 lxcraft-0.0.5/lxcraft/debian/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-31 20:44:16.000000 lxcraft-0.0.5/lxcraft/debian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-31 20:44:16.000000 lxcraft-0.0.5/lxcraft/debian/apt_package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:44:30.011621 lxcraft-0.0.5/lxcraft/path/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-31 20:44:16.000000 lxcraft-0.0.5/lxcraft/path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-31 20:44:16.000000 lxcraft-0.0.5/lxcraft/path/directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-07-31 20:44:16.000000 lxcraft-0.0.5/lxcraft/path/filecontent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-31 20:44:16.000000 lxcraft-0.0.5/lxcraft/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:44:30.011621 lxcraft-0.0.5/lxcraft/python/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-31 20:44:16.000000 lxcraft-0.0.5/lxcraft/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-31 20:44:16.000000 lxcraft-0.0.5/lxcraft/python/pip_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-31 20:44:16.000000 lxcraft-0.0.5/lxcraft/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-31 20:44:16.000000 lxcraft-0.0.5/lxcraft/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:44:30.015621 lxcraft-0.0.5/lxcraft/user/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-31 20:44:16.000000 lxcraft-0.0.5/lxcraft/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-31 20:44:16.000000 lxcraft-0.0.5/lxcraft/user/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-31 20:44:29.000000 lxcraft-0.0.5/lxcraft/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:44:30.011621 lxcraft-0.0.5/lxcraft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-31 20:44:29.000000 lxcraft-0.0.5/lxcraft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-31 20:44:29.000000 lxcraft-0.0.5/lxcraft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 20:44:29.000000 lxcraft-0.0.5/lxcraft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-31 20:44:29.000000 lxcraft-0.0.5/lxcraft.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-31 20:44:29.000000 lxcraft-0.0.5/lxcraft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-31 20:44:29.000000 lxcraft-0.0.5/lxcraft.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-31 20:44:17.000000 lxcraft-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-31 20:44:17.000000 lxcraft-0.0.5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-31 20:44:17.000000 lxcraft-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-31 20:44:17.000000 lxcraft-0.0.5/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-31 20:44:30.015621 lxcraft-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-31 20:44:17.000000 lxcraft-0.0.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-31 20:44:17.000000 lxcraft-0.0.5/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:44:30.015621 lxcraft-0.0.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:44:30.015621 lxcraft-0.0.5/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-31 20:44:17.000000 lxcraft-0.0.5/tests/templates/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-31 20:44:17.000000 lxcraft-0.0.5/tests/test_apt_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-31 20:44:17.000000 lxcraft-0.0.5/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-31 20:44:17.000000 lxcraft-0.0.5/tests/test_filecontent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-31 20:44:17.000000 lxcraft-0.0.5/tests/test_pip_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-31 20:44:17.000000 lxcraft-0.0.5/tests/test_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-31 20:44:17.000000 lxcraft-0.0.5/tests/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-31 20:44:17.000000 lxcraft-0.0.5/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-31 20:44:17.000000 lxcraft-0.0.5/tests/test_version.py
```

### Comparing `lxcraft-0.0.4/.cruft.json` & `lxcraft-0.0.5/.cruft.json`

 * *Files identical despite different names*

### Comparing `lxcraft-0.0.4/.github/workflows/release.yaml` & `lxcraft-0.0.5/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `lxcraft-0.0.4/.gitignore` & `lxcraft-0.0.5/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -134,7 +134,9 @@
 # pytype static type analyzer
 .pytype/
 
 # Cython debug symbols
 cython_debug/
 
 lxcraft/version.py
+
+.coverage
```

### Comparing `lxcraft-0.0.4/.pre-commit-config.yaml` & `lxcraft-0.0.5/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -26,25 +26,16 @@
     hooks:
     - id: python-check-mock-methods
     - id: python-use-type-annotations
     - id: python-check-blanket-type-ignore
     - id: python-check-blanket-noqa
 
 -   repo: https://github.com/psf/black/
-    rev: '23.3.0'
+    rev: '23.7.0'
     hooks:
     - id: black
 
 -   repo: https://github.com/charliermarsh/ruff-pre-commit
     # Ruff version.
-    rev: 'v0.0.265'
+    rev: 'v0.0.280'
     hooks:
     - id: ruff
-
--   repo: local
-    hooks:
-    -   id: run-just
-        name: Run tests using just
-        entry:
-            just all
-        language: system
-        pass_filenames: false
```

### Comparing `lxcraft-0.0.4/LICENSE` & `lxcraft-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lxcraft-0.0.4/PKG-INFO` & `lxcraft-0.0.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lxcraft
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple declarative configuration build tool for Linux systems
 Home-page: https://github.com/joaompinto/lxcraft
 Author: João Pinto
 Author-email: lamego.pinto@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -34,13 +34,19 @@
 Plan([
     AptPackages(["nginx"])
 ]).execute()
 ```
 
 ## How to develop
 
+### Requirements
+
+- Python 3.10+ is required.
+- Linux or WSL.
+
 In order to develop you must use Linux or WSL with docker.
 
 ```sh
-develop/docker-bash     # Enter the development docker instance
-just                    # Run the tests
+python develop/docker-bash.py
+invoke setup
+invoke test
 ```
```

### Comparing `lxcraft-0.0.4/README.md` & `lxcraft-0.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -23,13 +23,19 @@
 Plan([
     AptPackages(["nginx"])
 ]).execute()
 ```
 
 ## How to develop
 
+### Requirements
+
+- Python 3.10+ is required.
+- Linux or WSL.
+
 In order to develop you must use Linux or WSL with docker.
 
 ```sh
-develop/docker-bash     # Enter the development docker instance
-just                    # Run the tests
+python develop/docker-bash.py
+invoke setup
+invoke test
 ```
```

### Comparing `lxcraft-0.0.4/docs/resource.md` & `lxcraft-0.0.5/docs/resource.md`

 * *Files identical despite different names*

### Comparing `lxcraft-0.0.4/lxcraft/debian/apt_package.py` & `lxcraft-0.0.5/lxcraft/debian/apt_package.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from dataclasses import dataclass
 from subprocess import getstatusoutput
 
+from taglogger import tlog
+
 import lxcraft
 
 
 @dataclass
 class AptPackages(lxcraft.Resource):
     """List of packages that must be installed"""
 
@@ -31,9 +33,9 @@
     @staticmethod
     def is_installed(package_name: str):
         command = (
             "dpkg-query --showformat '${Status}'"
             f" --show {package_name} | grep -q '^install ok installed$'"
         )
         rc, _ = getstatusoutput(command)
-        lxcraft.debug("command", command, f"# rc={rc}")
+        tlog("command", command, f"# rc={rc}")
         return rc == 0
```

### Comparing `lxcraft-0.0.4/lxcraft/path/filecontent.py` & `lxcraft-0.0.5/lxcraft/path/filecontent.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,15 @@
         Path(self.target_path).unlink()
 
     def is_created(self):
         return Path(self.target_path).exists()
 
     def is_consistent(self):
         return (
-            self.is_created()
-            and self.get_template_text() == Path(self.target_path).read_text()
+            self.get_template_text() == Path(self.target_path).read_text()
             and self.mode_matches()
             and self.owner_matches()
         )
 
     def get_template_text(self):
         if self.source_path:
             source_path = Path(self.source_path)
```

### Comparing `lxcraft-0.0.4/lxcraft/plan.py` & `lxcraft-0.0.5/lxcraft/plan.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 from dataclasses import dataclass, field
 from typing import Callable
 
-import lxcraft
+from taglogger import tlog
 
 from .resource import Resource
 
 
 @dataclass
 class Plan:
     resources: list[Resource] = field(
@@ -22,19 +22,19 @@
         #     ), f"{resource} is not based on Resource"
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         for resource in self.resources:
-            lxcraft.debug("destroy", "__exit__ Destroying", resource)
+            tlog("destroy", "__exit__ Destroying", resource)
             resource.destroy()  # type: ignore[attr-defined]
 
     def try_and_point(self, action: Callable):
-        lxcraft.debug("action", "Trying to execute", action)
+        tlog("action", "Trying to execute", action)
         try:
             action()
         except Exception as e:
             print(
                 "EXCEPTION related to ",
                 action.__self__.source_repr(),  # type: ignore[attr-defined]
                 file=sys.stderr,
@@ -42,24 +42,24 @@
             raise e
 
     def execute(self):
         """Execute all the actions required to create the resources
         and bring them to a consistent state"""
         for resource in self.resources:
             if not resource.is_created():  # type: ignore[attr-defined]
-                lxcraft.debug("action", "Creating missing", resource)
+                tlog("action", "Creating missing", resource)
                 self.try_and_point(resource.create)  # type: ignore[attr-defined]
                 on_change_callback = getattr(resource, "on_change_callback", None)
                 if on_change_callback:
-                    lxcraft.debug("action", "on_change", resource, on_change_callback)
+                    tlog("action", "on_change", resource, on_change_callback)
                     on_change_callback()
             if not resource.is_consistent():  # type: ignore[attr-defined]
                 self.try_and_point(resource.destroy)  # type: ignore[attr-defined]
                 self.try_and_point(resource.create)  # type: ignore[attr-defined]
 
     def destroy(self):
         """Destroy all the resources"""
         for resource in self.resources:
-            lxcraft.debug("destroy", "Destroying all resources")
+            tlog("destroy", "Destroying all resources")
             for resource in self.resources:
                 if resource.is_created():  # type: ignore[attr-defined]
                     self.try_and_point(resource.destroy)  # type: ignore[attr-defined]
```

### Comparing `lxcraft-0.0.4/lxcraft/python/pip_package.py` & `lxcraft-0.0.5/lxcraft/python/pip_package.py`

 * *Files identical despite different names*

### Comparing `lxcraft-0.0.4/lxcraft/system.py` & `lxcraft-0.0.5/lxcraft/system.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import os
 
-import lxcraft
+from taglogger import tlog
 
 
 def system(*args, ignore_errors=False, **kwargs):
     """Run a shell command"""
     rc = os.system(*args, **kwargs)
-    lxcraft.debug(
+    tlog(
         "command",
         *args,
         **kwargs,
     )
-    lxcraft.debug("command", f"# rc={rc}, ignore_errors={ignore_errors}")
+    tlog("command", f"# rc={rc}, ignore_errors={ignore_errors}")
     if not ignore_errors and rc != 0:
         raise Exception(f"Command terminated with non zero exit code {rc}")
 
 
 # def get_output(*args, **kwargs):
 #     """Run a shell command"""
 #     rc, output = subprocess.getstatusoutput(*args, **kwargs)
-#     lxcraft.debug(
+#     tlog(
 #         "command",
 #         *args,
 #         f"# rc= {rc}",
 #         **kwargs,
 #     )
 #     if rc != 0:
 #         raise Exception(f"Command terminated with non zero exit code {rc}")
```

### Comparing `lxcraft-0.0.4/lxcraft/user/user.py` & `lxcraft-0.0.5/lxcraft/user/user.py`

 * *Files identical despite different names*

### Comparing `lxcraft-0.0.4/lxcraft.egg-info/PKG-INFO` & `lxcraft-0.0.5/lxcraft.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lxcraft
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple declarative configuration build tool for Linux systems
 Home-page: https://github.com/joaompinto/lxcraft
 Author: João Pinto
 Author-email: lamego.pinto@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -34,13 +34,19 @@
 Plan([
     AptPackages(["nginx"])
 ]).execute()
 ```
 
 ## How to develop
 
+### Requirements
+
+- Python 3.10+ is required.
+- Linux or WSL.
+
 In order to develop you must use Linux or WSL with docker.
 
 ```sh
-develop/docker-bash     # Enter the development docker instance
-just                    # Run the tests
+python develop/docker-bash.py
+invoke setup
+invoke test
 ```
```

### Comparing `lxcraft-0.0.4/lxcraft.egg-info/SOURCES.txt` & `lxcraft-0.0.5/lxcraft.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,58 +1,51 @@
 .cruft.json
 .gitignore
 .pre-commit-config.yaml
 .python-version
 CHANGELOG.md
-Justfile
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 ruff.toml
 setup.cfg
 setup.py
+tasks.py
 .github/workflows/docker-test.yaml
 .github/workflows/release.yaml
-.vscode/launch.json
 .vscode/settings.json
-develop/docker-bash
-develop/just-test.sh
+develop/docker-bash.py
 develop/setup.sh
 docs/debugging.md
 docs/resource.md
 lxcraft/__init__.py
-lxcraft/debug.py
 lxcraft/plan.py
 lxcraft/resource.py
 lxcraft/system.py
 lxcraft/version.py
 lxcraft.egg-info/PKG-INFO
 lxcraft.egg-info/SOURCES.txt
 lxcraft.egg-info/dependency_links.txt
 lxcraft.egg-info/entry_points.txt
+lxcraft.egg-info/requires.txt
 lxcraft.egg-info/top_level.txt
 lxcraft/debian/__init__.py
 lxcraft/debian/apt_package.py
 lxcraft/path/__init__.py
 lxcraft/path/directory.py
 lxcraft/path/filecontent.py
 lxcraft/python/__init__.py
 lxcraft/python/pip_package.py
 lxcraft/user/__init__.py
 lxcraft/user/user.py
 tests/test_apt_package.py
-tests/test_debug.py
 tests/test_directory.py
-tests/test_fastapi_uvicorn_gunicorn_supervisor.py
 tests/test_filecontent.py
 tests/test_pip_package.py
 tests/test_plan.py
-tests/test_resourrce.py
+tests/test_resource.py
 tests/test_user.py
 tests/test_version.py
-tests/templates/gunicorn_start
-tests/templates/main.py
-tests/templates/test.txt
-tests/templates/wwwkindos.conf
+tests/templates/test.txt
```

### Comparing `lxcraft-0.0.4/setup.py` & `lxcraft-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `lxcraft-0.0.4/tests/test_filecontent.py` & `lxcraft-0.0.5/tests/test_filecontent.py`

 * *Files identical despite different names*

### Comparing `lxcraft-0.0.4/tests/test_plan.py` & `lxcraft-0.0.5/tests/test_plan.py`

 * *Files identical despite different names*

### Comparing `lxcraft-0.0.4/tests/test_resourrce.py` & `lxcraft-0.0.5/tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `lxcraft-0.0.4/tests/test_user.py` & `lxcraft-0.0.5/tests/test_user.py`

 * *Files identical despite different names*

