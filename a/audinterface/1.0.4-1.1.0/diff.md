# Comparing `tmp/audinterface-1.0.4.tar.gz` & `tmp/audinterface-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audinterface-1.0.4.tar", last modified: Thu Jul 13 10:15:19 2023, max compression
+gzip compressed data, was "audinterface-1.1.0.tar", last modified: Mon Jul 31 08:03:41 2023, max compression
```

## Comparing `audinterface-1.0.4.tar` & `audinterface-1.1.0.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:15:19.541213 audinterface-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-13 10:15:02.000000 audinterface-1.0.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:15:19.529214 audinterface-1.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:15:19.533213 audinterface-1.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-13 10:15:02.000000 audinterface-1.0.4/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-13 10:15:02.000000 audinterface-1.0.4/.github/workflows/linter.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-13 10:15:02.000000 audinterface-1.0.4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-13 10:15:02.000000 audinterface-1.0.4/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-13 10:15:02.000000 audinterface-1.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-13 10:15:02.000000 audinterface-1.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-07-13 10:15:02.000000 audinterface-1.0.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-13 10:15:02.000000 audinterface-1.0.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-13 10:15:02.000000 audinterface-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-13 10:15:19.541213 audinterface-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-13 10:15:02.000000 audinterface-1.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:15:19.533213 audinterface-1.0.4/audinterface/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-13 10:15:02.000000 audinterface-1.0.4/audinterface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:15:19.537213 audinterface-1.0.4/audinterface/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 10:15:02.000000 audinterface-1.0.4/audinterface/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32332 2023-07-13 10:15:02.000000 audinterface-1.0.4/audinterface/core/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)    30259 2023-07-13 10:15:02.000000 audinterface-1.0.4/audinterface/core/process.py
--rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-07-13 10:15:02.000000 audinterface-1.0.4/audinterface/core/process_with_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    20091 2023-07-13 10:15:02.000000 audinterface-1.0.4/audinterface/core/segment.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-13 10:15:02.000000 audinterface-1.0.4/audinterface/core/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    14676 2023-07-13 10:15:02.000000 audinterface-1.0.4/audinterface/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:15:19.537213 audinterface-1.0.4/audinterface/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-13 10:15:02.000000 audinterface-1.0.4/audinterface/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:15:19.533213 audinterface-1.0.4/audinterface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-13 10:15:19.000000 audinterface-1.0.4/audinterface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-13 10:15:19.000000 audinterface-1.0.4/audinterface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 10:15:19.000000 audinterface-1.0.4/audinterface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-13 10:15:19.000000 audinterface-1.0.4/audinterface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 10:15:19.000000 audinterface-1.0.4/audinterface.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:15:19.537213 audinterface-1.0.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:15:19.529214 audinterface-1.0.4/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:15:19.537213 audinterface-1.0.4/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-13 10:15:02.000000 audinterface-1.0.4/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-13 10:15:02.000000 audinterface-1.0.4/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-13 10:15:02.000000 audinterface-1.0.4/docs/_templates/autosummary/function.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:15:19.537213 audinterface-1.0.4/docs/api-src/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-13 10:15:02.000000 audinterface-1.0.4/docs/api-src/audinterface.rst
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-13 10:15:02.000000 audinterface-1.0.4/docs/api-src/audinterface.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-13 10:15:02.000000 audinterface-1.0.4/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-13 10:15:02.000000 audinterface-1.0.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-13 10:15:02.000000 audinterface-1.0.4/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-13 10:15:02.000000 audinterface-1.0.4/docs/genindex.rst
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-13 10:15:02.000000 audinterface-1.0.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-13 10:15:02.000000 audinterface-1.0.4/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-13 10:15:02.000000 audinterface-1.0.4/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11456 2023-07-13 10:15:02.000000 audinterface-1.0.4/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:15:19.537213 audinterface-1.0.4/misc/
--rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-07-13 10:15:02.000000 audinterface-1.0.4/misc/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-13 10:15:02.000000 audinterface-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-13 10:15:02.000000 audinterface-1.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 10:15:19.541213 audinterface-1.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:15:19.541213 audinterface-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 10:15:02.000000 audinterface-1.0.4/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    29831 2023-07-13 10:15:02.000000 audinterface-1.0.4/tests/test_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)    40495 2023-07-13 10:15:02.000000 audinterface-1.0.4/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-07-13 10:15:02.000000 audinterface-1.0.4/tests/test_process_with_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    12548 2023-07-13 10:15:02.000000 audinterface-1.0.4/tests/test_segment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11689 2023-07-13 10:15:02.000000 audinterface-1.0.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:03:41.482178 audinterface-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-31 08:03:21.000000 audinterface-1.1.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:03:41.474178 audinterface-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:03:41.478178 audinterface-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-31 08:03:21.000000 audinterface-1.1.0/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-31 08:03:21.000000 audinterface-1.1.0/.github/workflows/linter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-31 08:03:21.000000 audinterface-1.1.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-31 08:03:21.000000 audinterface-1.1.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-31 08:03:21.000000 audinterface-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-31 08:03:21.000000 audinterface-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11492 2023-07-31 08:03:21.000000 audinterface-1.1.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-31 08:03:21.000000 audinterface-1.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-31 08:03:21.000000 audinterface-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-31 08:03:41.482178 audinterface-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-31 08:03:21.000000 audinterface-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:03:41.478178 audinterface-1.1.0/audinterface/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-31 08:03:21.000000 audinterface-1.1.0/audinterface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:03:41.478178 audinterface-1.1.0/audinterface/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 08:03:21.000000 audinterface-1.1.0/audinterface/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32705 2023-07-31 08:03:21.000000 audinterface-1.1.0/audinterface/core/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31320 2023-07-31 08:03:21.000000 audinterface-1.1.0/audinterface/core/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-07-31 08:03:21.000000 audinterface-1.1.0/audinterface/core/process_with_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20647 2023-07-31 08:03:21.000000 audinterface-1.1.0/audinterface/core/segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-31 08:03:21.000000 audinterface-1.1.0/audinterface/core/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14790 2023-07-31 08:03:21.000000 audinterface-1.1.0/audinterface/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:03:41.478178 audinterface-1.1.0/audinterface/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-31 08:03:21.000000 audinterface-1.1.0/audinterface/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:03:41.478178 audinterface-1.1.0/audinterface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-31 08:03:41.000000 audinterface-1.1.0/audinterface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-31 08:03:41.000000 audinterface-1.1.0/audinterface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 08:03:41.000000 audinterface-1.1.0/audinterface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-31 08:03:41.000000 audinterface-1.1.0/audinterface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-31 08:03:41.000000 audinterface-1.1.0/audinterface.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:03:41.482178 audinterface-1.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:03:41.474178 audinterface-1.1.0/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:03:41.482178 audinterface-1.1.0/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-31 08:03:21.000000 audinterface-1.1.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-31 08:03:21.000000 audinterface-1.1.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-31 08:03:21.000000 audinterface-1.1.0/docs/_templates/autosummary/function.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:03:41.482178 audinterface-1.1.0/docs/api-src/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-31 08:03:21.000000 audinterface-1.1.0/docs/api-src/audinterface.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-31 08:03:21.000000 audinterface-1.1.0/docs/api-src/audinterface.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-31 08:03:21.000000 audinterface-1.1.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-31 08:03:21.000000 audinterface-1.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-31 08:03:21.000000 audinterface-1.1.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-31 08:03:21.000000 audinterface-1.1.0/docs/genindex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-31 08:03:21.000000 audinterface-1.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-31 08:03:21.000000 audinterface-1.1.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-31 08:03:21.000000 audinterface-1.1.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11456 2023-07-31 08:03:21.000000 audinterface-1.1.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:03:41.482178 audinterface-1.1.0/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-07-31 08:03:21.000000 audinterface-1.1.0/misc/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-31 08:03:21.000000 audinterface-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-31 08:03:21.000000 audinterface-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 08:03:41.482178 audinterface-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:03:41.482178 audinterface-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-31 08:03:21.000000 audinterface-1.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-31 08:03:21.000000 audinterface-1.1.0/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35171 2023-07-31 08:03:21.000000 audinterface-1.1.0/tests/test_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42475 2023-07-31 08:03:21.000000 audinterface-1.1.0/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-07-31 08:03:21.000000 audinterface-1.1.0/tests/test_process_with_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12548 2023-07-31 08:03:21.000000 audinterface-1.1.0/tests/test_segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14415 2023-07-31 08:03:21.000000 audinterface-1.1.0/tests/test_utils.py
```

### Comparing `audinterface-1.0.4/.github/workflows/doc.yml` & `audinterface-1.1.0/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.4/.github/workflows/publish.yml` & `audinterface-1.1.0/.github/workflows/publish.yml`

 * *Files 9% similar despite different names*

```diff
@@ -58,18 +58,18 @@
         CHANGELOG=$(git diff -U0 HEAD^ HEAD | grep '^[+][\* ]' | sed 's/\+//')
         # Support for multiline, see
         # https://github.com/actions/create-release/pull/11#issuecomment-640071918
         CHANGELOG="${CHANGELOG//'%'/'%25'}"
         CHANGELOG="${CHANGELOG//$'\n'/'%0A'}"
         CHANGELOG="${CHANGELOG//$'\r'/'%0D'}"
         echo "Got changelog: $CHANGELOG"
-        run echo "body=$CHANGELOG" >> $GITHUB_OUTPUT
+        echo "body=$CHANGELOG" >> $GITHUB_OUTPUT
 
     - name: Create release on Github
       id: create_release
       uses: softprops/action-gh-release@v1
       env:
         GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
       with:
         tag_name: ${{ github.ref }}
-        release_name: Release ${{ github.ref }}
+        name: Release ${{ github.ref_name }}
         body: ${{ steps.changelog.outputs.body }}
```

### Comparing `audinterface-1.0.4/.github/workflows/test.yml` & `audinterface-1.1.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.4/.pre-commit-config.yaml` & `audinterface-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.4/CHANGELOG.rst` & `audinterface-1.1.0/CHANGELOG.rst`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,56 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 1.1.0 (2023/07/28)
+--------------------------
+
+* Added: ``include_root`` argument to
+  ``audinterface.Feature.process_folder()``,
+  ``audinterface.Process.process_folder()``,
+  ``audinterface.Segment.process_folder()``.
+  Returns relative file path
+  in index
+  if set to ``False``.
+  Default value is ``True``
+* Changed: when ``audinterface.Feature``
+  is instantiated with an ``audinterface.Segment``
+  object that returns an empty index,
+  ``audinterface.Feature.process_*()``
+  no longer return ``Index([], dtype='object')``
+  but ``MultiIndex([], names=['file', 'start', 'end'])``
+* Fixed: preserve order of ``start`` and ``end`` values
+  as returned by the segmentation callable
+  in the index returned by ``audinterface.Segment``
+  processing functions
+* Fixed: precision of ``audinterface.utils.to_timedelta()``
+  for ``pd.Timedelta`` objects as input,
+  e.g.
+  ``to_timedelta(pd.Timedelta('0 days 00:00:35.511437999'))``
+  now returns
+  ``Timedelta('0 days 00:00:35.511437999')``
+  instead of
+  ``Timedelta('0 days 00:00:35.511437')``.
+  This also affects the output of
+  ``audinterface.utils.signal_index()``
+* Fixed: preserve requested ``start`` and ``end`` values in
+  ``process_file()``,
+  ``process_files()``,
+  ``process_folder()``
+  methods of ``audinterface.Process``
+  and ``audinterface.Feature()``.
+  Before they were rounded
+  to the next sample
+  in the returned index
+
+
 Version 1.0.4 (2023/07/13)
 --------------------------
 
 * Changed: require ``audmath>=1.3.0``
 * Changed: require ``audiofile>=1.3.0``
 * Changed: always evenly round
   ``start`` and ``end``
```

### Comparing `audinterface-1.0.4/CONTRIBUTING.rst` & `audinterface-1.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.4/LICENSE` & `audinterface-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.4/PKG-INFO` & `audinterface-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audinterface
-Version: 1.0.4
+Version: 1.1.0
 Summary: Generic interfaces for signal processing
 Author-email: Hagen Wierstorf <hwierstorf@audeering.com>, Johannes Wagner <jwagner@audeering.com>, Andreas Triantafyllopoulos <andreas.triantafyllopoulos@uni-a.de>
 License: MIT License
         
         Copyright (c) 2018-2020 audEERING GmbH and Contributors
         
         Authors:
```

### Comparing `audinterface-1.0.4/README.rst` & `audinterface-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.4/audinterface/__init__.py` & `audinterface-1.1.0/audinterface/__init__.py`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.4/audinterface/core/feature.py` & `audinterface-1.1.0/audinterface/core/feature.py`

 * *Files 2% similar despite different names*

```diff
@@ -476,22 +476,27 @@
         return self._series_to_frame(series)
 
     def process_folder(
             self,
             root: str,
             *,
             filetype: str = 'wav',
+            include_root: bool = True,
     ) -> pd.DataFrame:
         r"""Extract features from files in a folder.
 
         .. note:: At the moment does not scan in sub-folders!
 
         Args:
             root: root folder
             filetype: file extension
+            include_root: if ``True``
+                the file paths are absolute
+                in the index
+                of the returned result
 
         Raises:
             FileNotFoundError: if folder does not exist
             RuntimeError: if sampling rates do not match
             RuntimeError: if channel selection is invalid
             RuntimeError: if multiple frames are returned,
                 but ``win_dur`` is not set
@@ -501,17 +506,20 @@
         if not os.path.exists(root):
             raise FileNotFoundError(
                 errno.ENOENT,
                 os.strerror(errno.ENOENT),
                 root,
             )
 
-        files = audeer.list_file_names(root, filetype=filetype)
-        files = [os.path.join(root, os.path.basename(f)) for f in files]
-        return self.process_files(files)
+        files = audeer.list_file_names(
+            root,
+            filetype=filetype,
+            basenames=not include_root,
+        )
+        return self.process_files(files, root=root)
 
     def process_index(
             self,
             index: pd.Index,
             *,
             preserve_index: bool = False,
             root: str = None,
@@ -755,15 +763,20 @@
 
     def _series_to_frame(
             self,
             y: pd.Series,
     ) -> pd.DataFrame:
 
         if y.empty:
+            if self.process.segment is None:
+                index = []
+            else:
+                index = audformat.segmented_index()
             return pd.DataFrame(
+                index=index,
                 columns=self.column_names,
                 dtype=object,
             )
 
         if (
                 self.win_dur is not None and
                 self.process_func_applies_sliding_window
```

### Comparing `audinterface-1.0.4/audinterface/core/process.py` & `audinterface-1.1.0/audinterface/core/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import typing
 
 import numpy as np
 import pandas as pd
 
 import audeer
 import audformat
+import audmath
 
 from audinterface.core import utils
 from audinterface.core.segment import Segment
 from audinterface.core.typing import Timestamp
 from audinterface.core.typing import Timestamps
 
 
@@ -265,24 +266,36 @@
             signal,
             sampling_rate,
             idx=idx,
             root=root,
             file=file,
         )
 
+        def precision_offset(duration, sampling_rate):
+            # Ensure we get the same precision
+            # by storing what is lost due to rounding
+            # when reading the file
+            duration_at_sample = utils.to_timedelta(
+                audmath.samples(duration.total_seconds(), sampling_rate)
+                / sampling_rate
+            )
+            return duration - duration_at_sample
+
         if self.win_dur is not None:
             if start is not None:
                 starts = starts + start
                 ends = ends + start
         else:
             if start is not None and not pd.isna(start):
                 starts[0] += start
-                ends[0] += start
+                ends[0] += start - precision_offset(start, sampling_rate)
             if self.keep_nat and (end is None or pd.isna(end)):
                 ends[0] = pd.NaT
+            if end is not None and not pd.isna(end):
+                ends[-1] += precision_offset(end, sampling_rate)
 
         return y, files, starts, ends
 
     def process_file(
             self,
             file: str,
             *,
@@ -369,14 +382,23 @@
 
         .. _audformat: https://audeering.github.io/audformat/data-format.html
 
         """
         if len(files) == 0:
             return pd.Series(dtype=object)
 
+        if self.segment is not None:
+            index = self.segment.process_files(
+                files,
+                starts=starts,
+                ends=ends,
+                root=root,
+            )
+            return self._process_index_wo_segment(index, root)
+
         if isinstance(starts, (type(None), float, int, str, pd.Timedelta)):
             starts = [starts] * len(files)
         if isinstance(ends, (type(None), float, int, str, pd.Timedelta)):
             ends = [ends] * len(files)
 
         params = [
             (
@@ -414,22 +436,27 @@
         return y
 
     def process_folder(
             self,
             root: str,
             *,
             filetype: str = 'wav',
+            include_root: bool = True,
     ) -> pd.Series:
         r"""Process files in a folder.
 
         .. note:: At the moment does not scan in sub-folders!
 
         Args:
             root: root folder
             filetype: file extension
+            include_root: if ``True``
+                the file paths are absolute
+                in the index
+                of the returned result
 
         Returns:
             Series with processed files conform to audformat_
 
         Raises:
             FileNotFoundError: if folder does not exist
             RuntimeError: if sampling rates do not match
@@ -442,17 +469,20 @@
         if not os.path.exists(root):
             raise FileNotFoundError(
                 errno.ENOENT,
                 os.strerror(errno.ENOENT),
                 root,
             )
 
-        files = audeer.list_file_names(root, filetype=filetype)
-        files = [os.path.join(root, os.path.basename(f)) for f in files]
-        return self.process_files(files)
+        files = audeer.list_file_names(
+            root,
+            filetype=filetype,
+            basenames=not include_root,
+        )
+        return self.process_files(files, root=root)
 
     def _process_index_wo_segment(
             self,
             index: pd.Index,
             root: typing.Optional[str],
     ) -> pd.Series:
         r"""Like process_index, but does not apply segmentation."""
```

### Comparing `audinterface-1.0.4/audinterface/core/process_with_context.py` & `audinterface-1.1.0/audinterface/core/process_with_context.py`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.4/audinterface/core/segment.py` & `audinterface-1.1.0/audinterface/core/segment.py`

 * *Files 2% similar despite different names*

```diff
@@ -268,16 +268,16 @@
             file,
             start=start,
             end=end,
             root=root,
         ).values[0]
         return audformat.segmented_index(
             files=[file] * len(index),
-            starts=index.levels[0] + start,
-            ends=index.levels[1] + start,
+            starts=index.get_level_values('start') + start,
+            ends=index.get_level_values('end') + start,
         )
 
     def process_files(
             self,
             files: typing.Sequence[str],
             *,
             starts: Timestamps = None,
@@ -320,32 +320,37 @@
             return audformat.filewise_index()
 
         files = []
         starts = []
         ends = []
         for (file, start, _), index in y.items():
             files.extend([file] * len(index))
-            starts.extend(index.levels[0] + start)
-            ends.extend(index.levels[1] + start)
+            starts.extend(index.get_level_values('start') + start)
+            ends.extend(index.get_level_values('end') + start)
 
         return audformat.segmented_index(files, starts, ends)
 
     def process_folder(
             self,
             root: str,
             *,
             filetype: str = 'wav',
+            include_root: bool = True,
     ) -> pd.Index:
         r"""Segment files in a folder.
 
         .. note:: At the moment does not scan in sub-folders!
 
         Args:
             root: root folder
             filetype: file extension
+            include_root: if ``True``
+                the file paths are absolute
+                in the index
+                of the returned result
 
         Returns:
             Segmented index conform to audformat_
 
         Raises:
             FileNotFoundError: if folder does not exist
             RuntimeError: if sampling rates do not match
@@ -358,17 +363,20 @@
         if not os.path.exists(root):
             raise FileNotFoundError(
                 errno.ENOENT,
                 os.strerror(errno.ENOENT),
                 root,
             )
 
-        files = audeer.list_file_names(root, filetype=filetype)
-        files = [os.path.join(root, os.path.basename(f)) for f in files]
-        return self.process_files(files)
+        files = audeer.list_file_names(
+            root,
+            filetype=filetype,
+            basenames=not include_root,
+        )
+        return self.process_files(files, root=root)
 
     def process_index(
             self,
             index: pd.Index,
             *,
             root: str = None,
             cache_root: str = None,
@@ -412,16 +420,16 @@
         )
 
         files = []
         starts = []
         ends = []
         for (file, start, _), index in y.items():
             files.extend([file] * len(index))
-            starts.extend(index.levels[0] + start)
-            ends.extend(index.levels[1] + start)
+            starts.extend(index.get_level_values('start') + start)
+            ends.extend(index.get_level_values('end') + start)
 
         return audformat.segmented_index(files, starts, ends)
 
     def process_signal(
             self,
             signal: np.ndarray,
             sampling_rate: int,
@@ -462,27 +470,34 @@
             sampling_rate,
             file=file,
             start=start,
             end=end,
         ).values[0]
         utils.assert_index(index)
         if start is not None:
+            start = utils.to_timedelta(start)
+            # Here we change directly the levels,
+            # so we need to use
+            # `index.levels[0]`
+            # instead of
+            # `index.get_level_values('start')`
             index = index.set_levels(
                 [
                     index.levels[0] + start,
                     index.levels[1] + start,
                 ],
                 level=[0, 1],
             )
         if file is not None:
             index = audformat.segmented_index(
                 files=[file] * len(index),
-                starts=index.levels[0],
-                ends=index.levels[1],
+                starts=index.get_level_values('start'),
+                ends=index.get_level_values('end'),
             )
+
         return index
 
     def process_signal_from_index(
             self,
             signal: np.ndarray,
             sampling_rate: int,
             index: pd.Index,
```

### Comparing `audinterface-1.0.4/audinterface/core/utils.py` & `audinterface-1.1.0/audinterface/core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -455,20 +455,22 @@
 
     if (
             not isinstance(durations, str)
             and isinstance(durations, collections.abc.Iterable)
     ):
         # sequence of duration entries
         durations = [
-            duration_in_seconds(duration, sampling_rate)
+            to_timedelta(duration, sampling_rate)
             for duration in durations
         ]
     else:
         # single duration entry
-        durations = duration_in_seconds(durations, sampling_rate)
 
-    durations = pd.to_timedelta(durations, unit='s')
+        # avoid converting Timedelta values to ensure precision
+        # https://github.com/audeering/audinterface/pull/137
+        if isinstance(durations, pd.Timedelta):
+            return durations
 
-    if isinstance(durations, pd.TimedeltaIndex):
-        durations = list(durations)
+        durations = duration_in_seconds(durations, sampling_rate)
+        durations = pd.to_timedelta(durations, unit='s')
 
     return durations
```

### Comparing `audinterface-1.0.4/audinterface.egg-info/PKG-INFO` & `audinterface-1.1.0/audinterface.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audinterface
-Version: 1.0.4
+Version: 1.1.0
 Summary: Generic interfaces for signal processing
 Author-email: Hagen Wierstorf <hwierstorf@audeering.com>, Johannes Wagner <jwagner@audeering.com>, Andreas Triantafyllopoulos <andreas.triantafyllopoulos@uni-a.de>
 License: MIT License
         
         Copyright (c) 2018-2020 audEERING GmbH and Contributors
         
         Authors:
```

### Comparing `audinterface-1.0.4/audinterface.egg-info/SOURCES.txt` & `audinterface-1.1.0/audinterface.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -35,13 +35,14 @@
 docs/usage.rst
 docs/_templates/autosummary/base.rst
 docs/_templates/autosummary/class.rst
 docs/_templates/autosummary/function.rst
 docs/api-src/audinterface.rst
 docs/api-src/audinterface.utils.rst
 misc/logo.png
+tests/conftest.py
 tests/requirements.txt
 tests/test_feature.py
 tests/test_process.py
 tests/test_process_with_context.py
 tests/test_segment.py
 tests/test_utils.py
```

### Comparing `audinterface-1.0.4/docs/_templates/autosummary/class.rst` & `audinterface-1.1.0/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.4/docs/api-src/audinterface.rst` & `audinterface-1.1.0/docs/api-src/audinterface.rst`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.4/docs/conf.py` & `audinterface-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.4/docs/index.rst` & `audinterface-1.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.4/docs/usage.rst` & `audinterface-1.1.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.4/misc/logo.png` & `audinterface-1.1.0/misc/logo.png`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.4/pyproject.toml` & `audinterface-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.4/tests/test_feature.py` & `audinterface-1.1.0/tests/test_feature.py`

 * *Files 13% similar despite different names*

```diff
@@ -385,23 +385,30 @@
         sampling_rate=None,
         channels=range(NUM_CHANNELS),
         resample=False,
         verbose=False,
     )
 
     path = str(tmpdir.mkdir('wav'))
-    files = [
-        os.path.join(path, f'file{n}.wav') for n in range(3)
-    ]
-    for file in files:
+    files = [f'file{n}.wav' for n in range(3)]
+    files_abs = [os.path.join(path, file) for file in files]
+    for file in files_abs:
         af.write(file, SIGNAL_2D, SAMPLING_RATE)
 
+    # folder with include_root=True
     y = feature.process_folder(path)
     y_expected = np.ones((3, NUM_CHANNELS * NUM_FEATURES))
+    assert all(y.index.levels[0] == files_abs)
+    assert all(y.index.levels[1] == index.levels[0])
+    assert all(y.index.levels[2] == index.levels[1])
+    np.testing.assert_array_equal(y.values, y_expected)
 
+    # folder with include_root=False
+    y = feature.process_folder(path, include_root=False)
+    y_expected = np.ones((3, NUM_CHANNELS * NUM_FEATURES))
     assert all(y.index.levels[0] == files)
     assert all(y.index.levels[1] == index.levels[0])
     assert all(y.index.levels[2] == index.levels[1])
     np.testing.assert_array_equal(y.values, y_expected)
 
     # non-existing folder
     with pytest.raises(FileNotFoundError):
@@ -409,14 +416,15 @@
 
     # empty folder
     root = str(tmpdir.mkdir('empty'))
     df = feature.process_folder(root)
     pd.testing.assert_frame_equal(
         df,
         pd.DataFrame(
+            index=pd.Index([], dtype='object'),
             dtype=object,
             columns=feature.column_names,
         ),
     )
 
 
 def test_process_func_args():
@@ -975,14 +983,158 @@
         signal,
         sampling_rate,
         index,
     )
     np.testing.assert_array_equal(df.values, expected)
 
 
+@pytest.mark.parametrize('audio', [(3, 8000)], indirect=True)  # s, Hz
+@pytest.mark.parametrize(
+    # `starts` and `ends`
+    # are used to create a segment object
+    # using audinterface.utils.signal_index()
+    'starts, ends',
+    [
+        (None, None),
+        (0, 1.5),
+        (1.5, 3),
+        ([0, 1.5], [1.5, 3]),
+        ([0, 2], [1, 3]),
+        ([0, 1], [2, 2]),
+        # https://github.com/audeering/audinterface/pull/145
+        ([0, 1.5], [1, 2.000000003]),
+        ([0.000000003, 1.5], [1, 2]),
+        ([1.000000003, 1.5], [1.1, 2]),
+        ([1.000000003, 2.1], [2.000000003, 2.5]),
+        # https://github.com/audeering/audinterface/issues/135
+        ([0, 1], [3, 2]),
+    ]
+)
+def test_feature_with_segment(audio, starts, ends):
+
+    path, signal, sampling_rate = audio
+    root, file = os.path.split(path)
+    duration = signal.shape[1] / sampling_rate
+
+    # Segment and process objects
+    segment = audinterface.Segment(
+        process_func=lambda x, sr:
+        audinterface.utils.signal_index(starts, ends)
+    )
+    feature = audinterface.Feature('f')
+    feature_with_segment = audinterface.Feature('f', segment=segment)
+
+    # Expected index
+    if starts is None:
+        files = None
+        files_abs = None
+    else:
+        files = [file] * len(audeer.to_list(starts))
+        files_abs = [audeer.path(root, file) for file in files]
+    expected = audformat.segmented_index(files, starts, ends)
+    expected_folder_index = audformat.segmented_index(files_abs, starts, ends)
+    expected_signal_index = audinterface.utils.signal_index(starts, ends)
+
+    # process signal
+    index = segment.process_signal(signal, sampling_rate)
+    pd.testing.assert_index_equal(index, expected_signal_index)
+
+    # process signal with start argument
+    index = segment.process_signal(signal, sampling_rate, start=0)
+    pd.testing.assert_index_equal(index, expected_signal_index)
+
+    # process signal with file argument
+    index = segment.process_signal(signal, sampling_rate, file=file)
+    pd.testing.assert_index_equal(index, expected)
+
+    pd.testing.assert_frame_equal(
+        feature.process_index(index, root=root, preserve_index=True),
+        feature_with_segment.process_signal(signal, sampling_rate, file=file)
+    )
+
+    # process signal from index
+    index = segment.process_signal_from_index(
+        signal,
+        sampling_rate,
+        audinterface.utils.signal_index(0, duration),
+    )
+    pd.testing.assert_index_equal(index, expected_signal_index)
+    index = segment.process_signal_from_index(
+        signal,
+        sampling_rate,
+        audformat.segmented_index(file, 0, duration),
+    )
+    pd.testing.assert_index_equal(index, expected)
+    index = segment.process_signal_from_index(
+        signal,
+        sampling_rate,
+        audformat.filewise_index(file),
+    )
+    pd.testing.assert_index_equal(index, expected)
+
+    pd.testing.assert_frame_equal(
+        feature.process_index(index, root=root, preserve_index=True),
+        feature_with_segment.process_signal_from_index(
+            signal,
+            sampling_rate,
+            audformat.filewise_index(file),
+        ),
+    )
+
+    # process file
+    index = segment.process_file(file, root=root)
+    pd.testing.assert_index_equal(index, expected)
+
+    pd.testing.assert_frame_equal(
+        feature.process_index(index, root=root, preserve_index=True),
+        feature_with_segment.process_file(file, root=root),
+    )
+
+    # process files
+    index = segment.process_files([file], root=root)
+    pd.testing.assert_index_equal(index, expected)
+
+    # https://github.com/audeering/audinterface/issues/138
+    pd.testing.assert_frame_equal(
+        feature.process_index(index, root=root, preserve_index=True),
+        feature_with_segment.process_files([file], root=root)
+    )
+
+    # process folder
+    index = segment.process_folder(root)
+    pd.testing.assert_index_equal(index, expected_folder_index)
+
+    pd.testing.assert_frame_equal(
+        feature.process_index(index, root=root, preserve_index=True),
+        feature_with_segment.process_folder(root),
+    )
+
+    # process folder without root
+    # https://github.com/audeering/audinterface/issues/139
+    index = segment.process_folder(root, include_root=False)
+    pd.testing.assert_index_equal(index, expected)
+
+    pd.testing.assert_frame_equal(
+        feature.process_index(index, root=root, preserve_index=True),
+        feature_with_segment.process_folder(root, include_root=False),
+    )
+
+    # process index
+    index = segment.process_index(audformat.filewise_index(file), root=root)
+    pd.testing.assert_index_equal(index, expected)
+
+    pd.testing.assert_frame_equal(
+        feature.process_index(index, root=root, preserve_index=True),
+        feature_with_segment.process_index(
+            audformat.filewise_index(file),
+            root=root,
+        ),
+    )
+
+
 @pytest.mark.parametrize(
     'signal, num_channels, sampling_rate',
     [
         (SIGNAL_1D, 1, SAMPLING_RATE),
         (SIGNAL_2D, 2, SAMPLING_RATE),
     ]
 )
```

### Comparing `audinterface-1.0.4/tests/test_process.py` & `audinterface-1.1.0/tests/test_process.py`

 * *Files 3% similar despite different names*

```diff
@@ -1516,117 +1516,160 @@
         num_workers=num_workers,
     )
     y = process.process_index(index, root=root)
     expected = pd.Series([(99, 'my/file', None)] * len(index), index)
     pd.testing.assert_series_equal(y, expected)
 
 
+@pytest.mark.parametrize('audio', [(3, 8000)], indirect=True)  # s, Hz
 @pytest.mark.parametrize(
-    'segment',
+    # `starts` and `ends`
+    # are used to create a segment object
+    # using audinterface.utils.signal_index()
+    'starts, ends',
     [
-        audinterface.Segment(
-            process_func=lambda x, sr: audinterface.utils.signal_index()
-        ),
-        audinterface.Segment(
-            process_func=lambda x, sr:
-                audinterface.utils.signal_index(
-                    pd.to_timedelta(0),
-                    pd.to_timedelta(x.shape[1] / sr, unit='s') / 2,
-                )
-        ),
-        audinterface.Segment(
-            process_func=lambda x, sr:
-            audinterface.utils.signal_index(
-                pd.to_timedelta(x.shape[1] / sr, unit='s') / 2,
-                pd.to_timedelta(x.shape[1] / sr, unit='s'),
-            )
-        ),
-        audinterface.Segment(
-            process_func=lambda x, sr:
-                audinterface.utils.signal_index(
-                    [
-                        pd.to_timedelta(0),
-                        pd.to_timedelta(x.shape[1] / sr, unit='s') / 2,
-                    ],
-                    [
-                        pd.to_timedelta(x.shape[1] / sr, unit='s') / 2,
-                        pd.to_timedelta(x.shape[1] / sr),
-                    ],
-                )
-        )
+        (None, None),
+        (0, 1.5),
+        (1.5, 3),
+        ([0, 1.5], [1.5, 3]),
+        ([0, 2], [1, 3]),
+        ([0, 1], [2, 2]),
+        # https://github.com/audeering/audinterface/pull/145
+        ([0, 1.5], [1, 2.000000003]),
+        ([0.000000003, 1.5], [1, 2]),
+        ([1.000000003, 1.5], [1.1, 2]),
+        ([1.000000003, 2.1], [2.000000003, 2.5]),
+        # https://github.com/audeering/audinterface/issues/135
+        ([0, 1], [3, 2]),
     ]
 )
-def test_process_with_segment(tmpdir, segment):
+def test_process_with_segment(audio, starts, ends):
 
-    process = audinterface.Process()
-    process_with_segment = audinterface.Process(
-        segment=segment,
+    path, signal, sampling_rate = audio
+    root, file = os.path.split(path)
+    duration = signal.shape[1] / sampling_rate
+
+    # Segment and process objects
+    segment = audinterface.Segment(
+        process_func=lambda x, sr:
+        audinterface.utils.signal_index(starts, ends)
     )
+    process = audinterface.Process()
+    process_with_segment = audinterface.Process(segment=segment)
 
-    # create signal and file
-    sampling_rate = 8000
-    signal = np.zeros((1, sampling_rate))
-    root = tmpdir
-    file = 'file.wav'
-    path = os.path.join(root, file)
-    audiofile.write(path, signal, sampling_rate)
+    # Expected index
+    if starts is None:
+        files = None
+        files_abs = None
+    else:
+        files = [file] * len(audeer.to_list(starts))
+        files_abs = [audeer.path(root, file) for file in files]
+    expected = audformat.segmented_index(files, starts, ends)
+    expected_folder_index = audformat.segmented_index(files_abs, starts, ends)
+    expected_signal_index = audinterface.utils.signal_index(starts, ends)
 
     # process signal
-    index = segment.process_signal(
+    index = segment.process_signal(signal, sampling_rate)
+    pd.testing.assert_index_equal(index, expected_signal_index)
+
+    # process signal with start argument
+    index = segment.process_signal(signal, sampling_rate, start=0)
+    pd.testing.assert_index_equal(index, expected_signal_index)
+
+    # process signal with file argument
+    index = segment.process_signal(signal, sampling_rate, file=file)
+    pd.testing.assert_index_equal(index, expected)
+
+    pd.testing.assert_series_equal(
+        process.process_index(index, root=root, preserve_index=True),
+        process_with_segment.process_signal(signal, sampling_rate, file=file)
+    )
+
+    # process signal from index
+    index = segment.process_signal_from_index(
         signal,
         sampling_rate,
-        file=file,
+        audinterface.utils.signal_index(0, duration),
     )
-    pd.testing.assert_series_equal(
-        process.process_index(index, root=root),
-        process_with_segment.process_signal(
-            signal,
-            sampling_rate,
-            file=file,
-        )
+    pd.testing.assert_index_equal(index, expected_signal_index)
+    index = segment.process_signal_from_index(
+        signal,
+        sampling_rate,
+        audformat.segmented_index(file, 0, duration),
     )
+    pd.testing.assert_index_equal(index, expected)
     index = segment.process_signal_from_index(
         signal,
         sampling_rate,
         audformat.filewise_index(file),
     )
+    pd.testing.assert_index_equal(index, expected)
+
     pd.testing.assert_series_equal(
-        process.process_index(index, root=root),
+        process.process_index(index, root=root, preserve_index=True),
         process_with_segment.process_signal_from_index(
             signal,
             sampling_rate,
             audformat.filewise_index(file),
-        )
+        ),
     )
 
     # process file
     index = segment.process_file(file, root=root)
+    pd.testing.assert_index_equal(index, expected)
+
     pd.testing.assert_series_equal(
-        process.process_index(index, root=root),
-        process_with_segment.process_file(file, root=root)
+        process.process_index(index, root=root, preserve_index=True),
+        process_with_segment.process_file(file, root=root),
     )
-    index = segment.process_index(
-        audformat.filewise_index(file),
-        root=root,
+
+    # process files
+    index = segment.process_files([file], root=root)
+    pd.testing.assert_index_equal(index, expected)
+
+    # https://github.com/audeering/audinterface/issues/138
+    pd.testing.assert_series_equal(
+        process.process_index(index, root=root, preserve_index=True),
+        process_with_segment.process_files([file], root=root)
+    )
+
+    # process folder
+    index = segment.process_folder(root)
+    pd.testing.assert_index_equal(index, expected_folder_index)
+
+    pd.testing.assert_series_equal(
+        process.process_index(index, root=root, preserve_index=True),
+        process_with_segment.process_folder(root),
     )
+
+    # process folder without root
+    # https://github.com/audeering/audinterface/issues/139
+    index = segment.process_folder(root, include_root=False)
+    pd.testing.assert_index_equal(index, expected)
+
     pd.testing.assert_series_equal(
-        process.process_index(index, root=root),
+        process.process_index(index, root=root, preserve_index=True),
+        process_with_segment.process_folder(root, include_root=False),
+    )
+
+    # process index
+    index = segment.process_index(audformat.filewise_index(file), root=root)
+    pd.testing.assert_index_equal(index, expected)
+
+    pd.testing.assert_series_equal(
+        process.process_index(index, root=root, preserve_index=True),
         process_with_segment.process_index(
             audformat.filewise_index(file),
             root=root,
-        )
+        ),
     )
 
-
-def test_read_audio(tmpdir):
-    sampling_rate = 8000
-    signal = np.ones((1, 8000))
-    path = str(tmpdir.mkdir('wav'))
-    file = os.path.join(path, 'file.wav')
-    af.write(file, signal, sampling_rate)
+@pytest.mark.parametrize('audio', [(1, 8000)], indirect=True)  # s, Hz
+def test_read_audio(audio):
+    file, _, sampling_rate = audio
     s, sr = audinterface.utils.read_audio(
         file,
         start=pd.Timedelta('00:00:00.1'),
         end=pd.Timedelta('00:00:00.2'),
     )
     assert sr == sampling_rate
     assert s.shape[1] == 0.1 * sr
```

### Comparing `audinterface-1.0.4/tests/test_process_with_context.py` & `audinterface-1.1.0/tests/test_process_with_context.py`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.4/tests/test_segment.py` & `audinterface-1.1.0/tests/test_segment.py`

 * *Files identical despite different names*

