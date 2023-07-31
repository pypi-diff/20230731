# Comparing `tmp/dinghy-1.2.0.tar.gz` & `tmp/dinghy-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dinghy-1.2.0.tar", last modified: Fri Jan 27 22:12:57 2023, max compression
+gzip compressed data, was "dinghy-1.3.0.tar", last modified: Mon Jul 31 12:45:10 2023, max compression
```

## Comparing `dinghy-1.2.0.tar` & `dinghy-1.3.0.tar`

### file list

```diff
@@ -1,56 +1,55 @@
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-01-27 22:12:57.563234 dinghy-1.2.0/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      545 2022-02-20 16:03:49.000000 dinghy-1.2.0/.editorconfig
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     9077 2023-01-27 22:11:59.000000 dinghy-1.2.0/CHANGELOG.rst
--rw-r--r--   0 nedbatchelder   (503) staff       (20)    10177 2022-02-19 22:33:45.000000 dinghy-1.2.0/LICENSE.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      154 2022-09-30 02:00:36.000000 dinghy-1.2.0/MANIFEST.in
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     2210 2022-11-10 00:38:04.000000 dinghy-1.2.0/Makefile
--rw-r--r--   0 nedbatchelder   (503) staff       (20)    17096 2023-01-27 22:12:57.563539 dinghy-1.2.0/PKG-INFO
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     7021 2023-01-27 22:10:35.000000 dinghy-1.2.0/README.rst
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       74 2022-02-20 12:22:50.000000 dinghy-1.2.0/dev-requirements.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      357 2022-03-12 13:35:59.000000 dinghy-1.2.0/pylintrc
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-01-27 22:12:57.539384 dinghy-1.2.0/scriv.d/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       65 2022-02-20 12:02:34.000000 dinghy-1.2.0/scriv.d/README.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     1403 2023-01-27 22:12:57.565226 dinghy-1.2.0/setup.cfg
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       83 2022-02-19 21:32:39.000000 dinghy-1.2.0/setup.py
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-01-27 22:12:57.533957 dinghy-1.2.0/src/
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-01-27 22:12:57.543515 dinghy-1.2.0/src/dinghy/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       57 2023-01-27 22:11:47.000000 dinghy-1.2.0/src/dinghy/__init__.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      162 2022-02-25 12:50:11.000000 dinghy-1.2.0/src/dinghy/__main__.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     1356 2023-01-25 22:38:19.000000 dinghy-1.2.0/src/dinghy/adhoc.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     1892 2023-01-27 21:53:48.000000 dinghy-1.2.0/src/dinghy/cli.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)    20422 2023-01-27 21:53:48.000000 dinghy-1.2.0/src/dinghy/digest.py
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-01-27 22:12:57.560789 dinghy-1.2.0/src/dinghy/graphql/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       54 2022-03-10 23:36:30.000000 dinghy-1.2.0/src/dinghy/graphql/author_frag.graphql
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      307 2022-04-13 00:27:23.000000 dinghy-1.2.0/src/dinghy/graphql/comment_frag.graphql
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      314 2022-03-24 15:22:17.000000 dinghy-1.2.0/src/dinghy/graphql/issue_comments.graphql
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      613 2022-06-07 12:39:09.000000 dinghy-1.2.0/src/dinghy/graphql/issue_frag.graphql
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      244 2022-06-23 19:43:11.000000 dinghy-1.2.0/src/dinghy/graphql/org_project_entries.graphql
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      317 2022-04-13 00:43:42.000000 dinghy-1.2.0/src/dinghy/graphql/pr_comments.graphql
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      314 2022-04-12 22:10:18.000000 dinghy-1.2.0/src/dinghy/graphql/pr_reviews.graphql
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      338 2022-04-12 22:21:59.000000 dinghy-1.2.0/src/dinghy/graphql/pr_reviewthreads.graphql
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      427 2022-06-23 19:43:36.000000 dinghy-1.2.0/src/dinghy/graphql/project_entries_frag.graphql
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      890 2022-04-12 22:17:32.000000 dinghy-1.2.0/src/dinghy/graphql/pull_request_frag.graphql
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      364 2022-11-10 00:38:04.000000 dinghy-1.2.0/src/dinghy/graphql/release_frag.graphql
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       91 2022-02-19 21:57:26.000000 dinghy-1.2.0/src/dinghy/graphql/repo_frag.graphql
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      452 2022-03-24 15:22:38.000000 dinghy-1.2.0/src/dinghy/graphql/repo_issues.graphql
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      478 2022-03-24 15:22:40.000000 dinghy-1.2.0/src/dinghy/graphql/repo_pull_requests.graphql
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      391 2022-11-10 00:38:04.000000 dinghy-1.2.0/src/dinghy/graphql/repo_releases.graphql
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      384 2022-04-13 00:44:16.000000 dinghy-1.2.0/src/dinghy/graphql/review_comments.graphql
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      318 2022-03-10 23:36:30.000000 dinghy-1.2.0/src/dinghy/graphql/review_frag.graphql
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      396 2022-04-13 00:44:08.000000 dinghy-1.2.0/src/dinghy/graphql/reviewthread_comments.graphql
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      239 2022-04-12 23:57:00.000000 dinghy-1.2.0/src/dinghy/graphql/reviewthread_frag.graphql
--rw-r--r--   0 nedbatchelder   (503) staff       (20)      474 2022-03-24 15:22:41.000000 dinghy-1.2.0/src/dinghy/graphql/search_entries.graphql
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     7628 2023-01-25 22:06:32.000000 dinghy-1.2.0/src/dinghy/graphql_helpers.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     1545 2022-10-25 16:17:04.000000 dinghy-1.2.0/src/dinghy/helpers.py
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     1680 2023-01-25 22:38:19.000000 dinghy-1.2.0/src/dinghy/jinja_helpers.py
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-01-27 22:12:57.561972 dinghy-1.2.0/src/dinghy/templates/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)    10998 2023-01-20 12:52:42.000000 dinghy-1.2.0/src/dinghy/templates/digest.html.j2
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-01-27 22:12:57.547263 dinghy-1.2.0/src/dinghy.egg-info/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)    17096 2023-01-27 22:12:57.000000 dinghy-1.2.0/src/dinghy.egg-info/PKG-INFO
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     1429 2023-01-27 22:12:57.000000 dinghy-1.2.0/src/dinghy.egg-info/SOURCES.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)        1 2023-01-27 22:12:57.000000 dinghy-1.2.0/src/dinghy.egg-info/dependency_links.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       47 2023-01-27 22:12:57.000000 dinghy-1.2.0/src/dinghy.egg-info/entry_points.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)       76 2023-01-27 22:12:57.000000 dinghy-1.2.0/src/dinghy.egg-info/requires.txt
--rw-r--r--   0 nedbatchelder   (503) staff       (20)        7 2023-01-27 22:12:57.000000 dinghy-1.2.0/src/dinghy.egg-info/top_level.txt
-drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-01-27 22:12:57.562759 dinghy-1.2.0/tests/
--rw-r--r--   0 nedbatchelder   (503) staff       (20)     1283 2022-10-25 16:17:09.000000 dinghy-1.2.0/tests/test_helpers.py
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-07-31 12:45:10.020844 dinghy-1.3.0/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      545 2022-02-20 16:03:49.000000 dinghy-1.3.0/.editorconfig
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     9454 2023-07-31 12:41:43.000000 dinghy-1.3.0/CHANGELOG.rst
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)    10177 2022-02-19 22:33:45.000000 dinghy-1.3.0/LICENSE.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      137 2023-07-31 12:05:59.000000 dinghy-1.3.0/MANIFEST.in
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     2225 2023-07-31 12:38:14.000000 dinghy-1.3.0/Makefile
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)    17467 2023-07-31 12:45:10.019348 dinghy-1.3.0/PKG-INFO
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     7036 2023-07-31 01:50:19.000000 dinghy-1.3.0/README.rst
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       84 2023-07-31 01:09:13.000000 dinghy-1.3.0/dev-requirements.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     2075 2023-07-31 12:25:07.000000 dinghy-1.3.0/pyproject.toml
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-07-31 12:45:09.979022 dinghy-1.3.0/scriv.d/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       65 2022-02-20 12:02:34.000000 dinghy-1.3.0/scriv.d/README.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       38 2023-07-31 12:45:10.021192 dinghy-1.3.0/setup.cfg
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-07-31 12:45:09.970170 dinghy-1.3.0/src/
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-07-31 12:45:09.987621 dinghy-1.3.0/src/dinghy/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       57 2023-07-31 12:40:27.000000 dinghy-1.3.0/src/dinghy/__init__.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      162 2022-02-25 12:50:11.000000 dinghy-1.3.0/src/dinghy/__main__.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     1438 2023-06-15 16:32:50.000000 dinghy-1.3.0/src/dinghy/adhoc.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     1992 2023-07-31 01:13:41.000000 dinghy-1.3.0/src/dinghy/cli.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)    20435 2023-07-31 00:38:49.000000 dinghy-1.3.0/src/dinghy/digest.py
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-07-31 12:45:10.015646 dinghy-1.3.0/src/dinghy/graphql/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       54 2022-03-10 23:36:30.000000 dinghy-1.3.0/src/dinghy/graphql/author_frag.graphql
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      307 2022-04-13 00:27:23.000000 dinghy-1.3.0/src/dinghy/graphql/comment_frag.graphql
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      314 2022-03-24 15:22:17.000000 dinghy-1.3.0/src/dinghy/graphql/issue_comments.graphql
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      613 2022-06-07 12:39:09.000000 dinghy-1.3.0/src/dinghy/graphql/issue_frag.graphql
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      244 2022-06-23 19:43:11.000000 dinghy-1.3.0/src/dinghy/graphql/org_project_entries.graphql
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      317 2022-04-13 00:43:42.000000 dinghy-1.3.0/src/dinghy/graphql/pr_comments.graphql
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      314 2022-04-12 22:10:18.000000 dinghy-1.3.0/src/dinghy/graphql/pr_reviews.graphql
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      338 2022-04-12 22:21:59.000000 dinghy-1.3.0/src/dinghy/graphql/pr_reviewthreads.graphql
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      427 2022-06-23 19:43:36.000000 dinghy-1.3.0/src/dinghy/graphql/project_entries_frag.graphql
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      890 2022-04-12 22:17:32.000000 dinghy-1.3.0/src/dinghy/graphql/pull_request_frag.graphql
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      364 2022-11-10 00:38:04.000000 dinghy-1.3.0/src/dinghy/graphql/release_frag.graphql
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       91 2022-02-19 21:57:26.000000 dinghy-1.3.0/src/dinghy/graphql/repo_frag.graphql
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      452 2022-03-24 15:22:38.000000 dinghy-1.3.0/src/dinghy/graphql/repo_issues.graphql
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      478 2022-03-24 15:22:40.000000 dinghy-1.3.0/src/dinghy/graphql/repo_pull_requests.graphql
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      391 2022-11-10 00:38:04.000000 dinghy-1.3.0/src/dinghy/graphql/repo_releases.graphql
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      384 2022-04-13 00:44:16.000000 dinghy-1.3.0/src/dinghy/graphql/review_comments.graphql
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      318 2022-03-10 23:36:30.000000 dinghy-1.3.0/src/dinghy/graphql/review_frag.graphql
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      396 2022-04-13 00:44:08.000000 dinghy-1.3.0/src/dinghy/graphql/reviewthread_comments.graphql
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      239 2022-04-12 23:57:00.000000 dinghy-1.3.0/src/dinghy/graphql/reviewthread_frag.graphql
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      474 2022-03-24 15:22:41.000000 dinghy-1.3.0/src/dinghy/graphql/search_entries.graphql
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     7635 2023-07-30 22:16:51.000000 dinghy-1.3.0/src/dinghy/graphql_helpers.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     2298 2023-07-31 00:40:38.000000 dinghy-1.3.0/src/dinghy/helpers.py
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     1680 2023-01-25 22:38:19.000000 dinghy-1.3.0/src/dinghy/jinja_helpers.py
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-07-31 12:45:10.016774 dinghy-1.3.0/src/dinghy/templates/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)    10998 2023-01-20 12:52:42.000000 dinghy-1.3.0/src/dinghy/templates/digest.html.j2
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-07-31 12:45:09.996483 dinghy-1.3.0/src/dinghy.egg-info/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)    17467 2023-07-31 12:45:09.000000 dinghy-1.3.0/src/dinghy.egg-info/PKG-INFO
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     1416 2023-07-31 12:45:09.000000 dinghy-1.3.0/src/dinghy.egg-info/SOURCES.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)        1 2023-07-31 12:45:09.000000 dinghy-1.3.0/src/dinghy.egg-info/dependency_links.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)       47 2023-07-31 12:45:09.000000 dinghy-1.3.0/src/dinghy.egg-info/entry_points.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)      109 2023-07-31 12:45:09.000000 dinghy-1.3.0/src/dinghy.egg-info/requires.txt
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)        7 2023-07-31 12:45:09.000000 dinghy-1.3.0/src/dinghy.egg-info/top_level.txt
+drwxr-xr-x   0 nedbatchelder   (503) staff       (20)        0 2023-07-31 12:45:10.017805 dinghy-1.3.0/tests/
+-rw-r--r--   0 nedbatchelder   (503) staff       (20)     1677 2023-07-31 11:06:00.000000 dinghy-1.3.0/tests/test_helpers.py
```

### Comparing `dinghy-1.2.0/.editorconfig` & `dinghy-1.3.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `dinghy-1.2.0/CHANGELOG.rst` & `dinghy-1.3.0/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,31 @@
 See the fragment files in the `scriv.d directory`_.
 
 .. _scriv.d directory: https://github.com/nedbat/dinghy/tree/master/scriv.d
 
 
 .. scriv-insert-here
 
+.. _changelog-1.3.0:
+
+1.3.0 — 2023-07-31
+------------------
+
+Added
+.....
+
+- The ``since`` date can now be specified on the command line with ``--since``.
+  This will override any specification in the YAML file.
+
+- The ``since`` value can be specified as a specific ISO 8601 date or datetime,
+  closing `issue 26`_.
+
+.. _issue 26: https://github.com/nedbat/dinghy/issues/26
+
+
 .. _changelog-1.2.0:
 
 1.2.0 — 2023-01-27
 ------------------
 
 Added
 .....
```

### Comparing `dinghy-1.2.0/LICENSE.txt` & `dinghy-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dinghy-1.2.0/Makefile` & `dinghy-1.3.0/Makefile`

 * *Files 19% similar despite different names*

```diff
@@ -34,20 +34,22 @@
 
 _check_manifest:
 	python -m check_manifest
 
 
 .PHONY: check_release _check_version _check_scriv
 
+VERSION := $(shell python -c "import dinghy as d; print(d.__version__)")
+
 check_release: _check_manifest _check_version _check_scriv  ## check that we are ready for a release
 	@echo "Release checks passed"
 
 _check_version:
-	@if [[ $$(git tags | grep -q -w $$(python setup.py --version) && echo "x") == "x" ]]; then \
-		echo 'A git tag for this version exists! Did you forget to bump the version in src/dinghy/__init__.py?'; \
+	@if [[ $$(git tags | grep -q -w $(VERSION) && echo "x") == "x" ]]; then \
+		echo 'A git tag for $(VERSION) exists! Did you forget to bump the version in src/dinghy/__init__.py?'; \
 		exit 1; \
 	fi
 
 _check_scriv:
 	@if (( $$(ls -1 scriv.d | wc -l) != 1 )); then \
 		echo 'There are scriv fragments! Did you forget `scriv collect`?'; \
 		exit 1; \
@@ -65,12 +67,12 @@
 testpypi: ## upload the distributions to PyPI's testing server.
 	python -m twine upload --verbose --repository testpypi --password $$TWINE_TEST_PASSWORD dist/*
 
 pypi: ## upload the built distributions to PyPI.
 	python -m twine upload --verbose dist/*
 
 tag: ## make a git tag with the version number
-	git tag -a -m "Version $$(python setup.py --version)" $$(python setup.py --version)
+	git tag -a -m "Version $(VERSION)" $(VERSION)
 	git push --all
 
 gh_release: ## make a GitHub release
 	python -m scriv github-release
```

### Comparing `dinghy-1.2.0/PKG-INFO` & `dinghy-1.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,51 @@
 Metadata-Version: 2.1
 Name: dinghy
-Version: 1.2.0
+Version: 1.3.0
 Summary: Dinghy daily digest tool
-Home-page: https://github.com/nedbat/dinghy
-Author: Ned Batchelder
-Author-email: ned@nedbatchelder.com
+Author-email: Ned Batchelder <ned@nedbatchelder.com>
 License: Apache-2.0
-Project-URL: Twitter, https://twitter.com/nedbat
 Project-URL: Mastodon, https://hachyderm.io/@nedbat
 Project-URL: Funding, https://github.com/sponsors/nedbat
 Project-URL: Issues, https://github.com/nedbat/dinghy/issues
 Project-URL: Source, https://github.com/nedbat/dinghy
+Project-URL: Home, https://github.com/nedbat/dinghy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Natural Language :: English
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 ######
 Dinghy
 ######
 
 Dinghy, a GitHub activity digest tool.
 
 |pypi-badge| |pyversions-badge| |license-badge|
-|sponsor-badge| |mastodon-nedbat| |twitter-nedbat|
+|sponsor-badge| |mastodon-nedbat|
 
 Dinghy uses the GitHub GraphQL API to find recent activity on releases, issues
 and pull requests, and writes a compact HTML digest `like this <sample_>`_.
 
 
+Sample Digest
+=============
+
+Here's a sample of a Dinghy digest reporting on `some PSF repos: black,
+requests, and PEPs <sample_>`_.
+
+
 Getting Started
 ===============
 
 1. Install dinghy:
 
    .. code-block:: bash
 
@@ -128,15 +134,16 @@
 
 - The ``digest`` setting is the HTML digest file to write.
 
 - The ``since`` setting indicates how far back to look for activity. It can use
   units of weeks, days, hours, minutes and seconds, and can also be
   abbreviated, like ``1d6h``. Using ``since: forever`` will include all
   activity regardless of when it happened.  If ``since`` is omitted, it
-  defaults to one week.
+  defaults to one week.  You can specify ``--since=<SINCE>`` on the dinghy
+  command line to provide an explicit value.
 
 - The ``items`` setting is a list of things to report on, specified in a few
   different ways:
 
   - The ``url`` setting is a GitHub URL, in a number of forms:
 
     - An organization project URL will report on the issues and pull requests
@@ -215,17 +222,14 @@
     :alt: Supported Python versions
 .. |license-badge| image:: https://img.shields.io/github/license/nedbat/dinghy.svg
     :target: https://github.com/nedbat/dinghy/blob/master/LICENSE.txt
     :alt: License
 .. |mastodon-nedbat| image:: https://img.shields.io/badge/dynamic/json?style=flat&labelColor=450657&logo=mastodon&logoColor=ffffff&link=https%3A%2F%2Fhachyderm.io%2F%40nedbat&url=https%3A%2F%2Fhachyderm.io%2Fusers%2Fnedbat%2Ffollowers.json&query=totalItems&label=Mastodon
     :target: https://hachyderm.io/@nedbat
     :alt: nedbat on Mastodon
-.. |twitter-nedbat| image:: https://img.shields.io/twitter/follow/nedbat.svg?label=nedbat&style=flat&logo=twitter&logoColor=4FADFF
-    :target: https://twitter.com/nedbat
-    :alt: nedbat on Twitter
 .. |sponsor-badge| image:: https://img.shields.io/badge/%E2%9D%A4-Sponsor%20me-brightgreen?style=flat&logo=GitHub
     :target: https://github.com/sponsors/nedbat
     :alt: Sponsor me on GitHub
 
 
 .. this will be appended to README.rst
 
@@ -246,14 +250,31 @@
 See the fragment files in the `scriv.d directory`_.
 
 .. _scriv.d directory: https://github.com/nedbat/dinghy/tree/master/scriv.d
 
 
 .. scriv-insert-here
 
+.. _changelog-1.3.0:
+
+1.3.0 — 2023-07-31
+------------------
+
+Added
+.....
+
+- The ``since`` date can now be specified on the command line with ``--since``.
+  This will override any specification in the YAML file.
+
+- The ``since`` value can be specified as a specific ISO 8601 date or datetime,
+  closing `issue 26`_.
+
+.. _issue 26: https://github.com/nedbat/dinghy/issues/26
+
+
 .. _changelog-1.2.0:
 
 1.2.0 — 2023-01-27
 ------------------
 
 Added
 .....
```

### Comparing `dinghy-1.2.0/README.rst` & `dinghy-1.3.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 ######
 Dinghy
 ######
 
 Dinghy, a GitHub activity digest tool.
 
 |pypi-badge| |pyversions-badge| |license-badge|
-|sponsor-badge| |mastodon-nedbat| |twitter-nedbat|
+|sponsor-badge| |mastodon-nedbat|
 
 Dinghy uses the GitHub GraphQL API to find recent activity on releases, issues
 and pull requests, and writes a compact HTML digest `like this <sample_>`_.
 
 
+Sample Digest
+=============
+
+Here's a sample of a Dinghy digest reporting on `some PSF repos: black,
+requests, and PEPs <sample_>`_.
+
+
 Getting Started
 ===============
 
 1. Install dinghy:
 
    .. code-block:: bash
 
@@ -103,15 +110,16 @@
 
 - The ``digest`` setting is the HTML digest file to write.
 
 - The ``since`` setting indicates how far back to look for activity. It can use
   units of weeks, days, hours, minutes and seconds, and can also be
   abbreviated, like ``1d6h``. Using ``since: forever`` will include all
   activity regardless of when it happened.  If ``since`` is omitted, it
-  defaults to one week.
+  defaults to one week.  You can specify ``--since=<SINCE>`` on the dinghy
+  command line to provide an explicit value.
 
 - The ``items`` setting is a list of things to report on, specified in a few
   different ways:
 
   - The ``url`` setting is a GitHub URL, in a number of forms:
 
     - An organization project URL will report on the issues and pull requests
@@ -190,13 +198,10 @@
     :alt: Supported Python versions
 .. |license-badge| image:: https://img.shields.io/github/license/nedbat/dinghy.svg
     :target: https://github.com/nedbat/dinghy/blob/master/LICENSE.txt
     :alt: License
 .. |mastodon-nedbat| image:: https://img.shields.io/badge/dynamic/json?style=flat&labelColor=450657&logo=mastodon&logoColor=ffffff&link=https%3A%2F%2Fhachyderm.io%2F%40nedbat&url=https%3A%2F%2Fhachyderm.io%2Fusers%2Fnedbat%2Ffollowers.json&query=totalItems&label=Mastodon
     :target: https://hachyderm.io/@nedbat
     :alt: nedbat on Mastodon
-.. |twitter-nedbat| image:: https://img.shields.io/twitter/follow/nedbat.svg?label=nedbat&style=flat&logo=twitter&logoColor=4FADFF
-    :target: https://twitter.com/nedbat
-    :alt: nedbat on Twitter
 .. |sponsor-badge| image:: https://img.shields.io/badge/%E2%9D%A4-Sponsor%20me-brightgreen?style=flat&logo=GitHub
     :target: https://github.com/sponsors/nedbat
     :alt: Sponsor me on GitHub
```

### Comparing `dinghy-1.2.0/src/dinghy/adhoc.py` & `dinghy-1.3.0/src/dinghy/adhoc.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 """
 A module-main for running ad-hoc GitHub GraphQL queries.
+
+After installing dinghy, run it like this:
+
+    $ python -m dinghy.adhoc --help
+
 """
 
 import json
 import os
 import sys
 
 import click
```

### Comparing `dinghy-1.2.0/src/dinghy/cli.py` & `dinghy-1.3.0/src/dinghy/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,26 +38,27 @@
                 + f"next reset at {lrl['reset_when']}"
             )
 
 
 @click.command()
 @click_log.simple_verbosity_option(logger)
 @click.version_option()
+@click.option("--since", metavar="DELTA-OR-DATE", help="Specify a since date.")
 @click.argument("_input", metavar="[INPUT]", default="dinghy.yaml")
 @click.argument("digests", metavar="[DIGEST ...]", nargs=-1)
-def cli(_input, digests):
+def cli(since, _input, digests):
     """
     Generate HTML digests of GitHub activity.
 
     INPUT is a dinghy YAML configuration file (default: dinghy.yaml), or a
     GitHub repo URL.
 
     DIGEST(s) are the file names of digests from the configuration file to
     create.  If none are specified, all of the digests are written.
 
     """
     if "://" in _input:
         coro = make_digest([_input])
     else:
-        coro = make_digests_from_config(_input, digests or None)
+        coro = make_digests_from_config(_input, digests or None, since=since)
 
     main_run(coro)
```

### Comparing `dinghy-1.2.0/src/dinghy/digest.py` & `dinghy-1.3.0/src/dinghy/digest.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import urllib.parse
 
 import yaml
 from glom import glom
 
 from . import __version__
 from .graphql_helpers import build_query, GraphqlHelper
-from .helpers import DinghyError, json_save, parse_timedelta
+from .helpers import DinghyError, json_save, parse_since
 from .jinja_helpers import render_jinja_to_file
 
 
 logger = logging.getLogger(__name__)
 
 GITHUB_URL_MAP = []
 
@@ -502,20 +502,16 @@
 
     Args:
         since (str): a duration spec ("2 day", "3d6h", etc).
         items (list[str|dict]): a list of YAML objects or GitHub URLs to collect entries from.
         digest (str): the HTML file name to write.
 
     """
-    if since == "forever":
-        show_date = False
-        since_date = datetime.datetime(year=1980, month=1, day=1)
-    else:
-        show_date = True
-        since_date = datetime.datetime.now() - parse_timedelta(since)
+    show_date = since != "forever"
+    since_date = parse_since(since)
     digester = Digester(since=since_date, options=options)
 
     coros = []
     for item in items:
         try:
             coros.append(coro_from_item(digester, item))
         except:
@@ -540,37 +536,40 @@
         now=datetime.datetime.now(),
         __version__=__version__,
         title=options.get("title", ""),
     )
     logger.info(f"Wrote digest: {digest}")
 
 
-async def make_digests_from_config(conf_file, digests=None):
+async def make_digests_from_config(conf_file, digests=None, since=None):
     """
     Make all the digests specified by a configuration file.
 
     Args:
         conf_file (str): a file path to read as a config file.
-
+        digests (list of str): the digest names to make.
+        since (str): the spec for since when.
     """
     try:
         with open(conf_file, encoding="utf-8") as cf:
             config = yaml.safe_load(cf)
     except Exception as err:
         raise DinghyError(f"Couldn't read config file {conf_file!r}: {err}") from err
 
     if "digests" not in config:
         raise DinghyError(f"No 'digests:' clause in config file {conf_file!r}")
 
     defaults = config.get("defaults", {})
     coros = []
-    for spec in config.get("digests", []):
+    for spec in config["digests"]:
         args = {**defaults, **spec}
         if digests is not None and args["digest"] not in digests:
             continue
+        if since is not None:
+            args["since"] = since
         coros.append(make_digest(**args))
     await asyncio.gather(*coros)
 
 
 def just_render(result_file):
     """Helper function to re-render stored results.
```

### Comparing `dinghy-1.2.0/src/dinghy/graphql/issue_frag.graphql` & `dinghy-1.3.0/src/dinghy/graphql/issue_frag.graphql`

 * *Files identical despite different names*

### Comparing `dinghy-1.2.0/src/dinghy/graphql/pull_request_frag.graphql` & `dinghy-1.3.0/src/dinghy/graphql/pull_request_frag.graphql`

 * *Files identical despite different names*

### Comparing `dinghy-1.2.0/src/dinghy/graphql_helpers.py` & `dinghy-1.3.0/src/dinghy/graphql_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,30 +49,30 @@
 
 
 def _raise_if_error(data):
     """
     If `data` is an error response, raise a useful exception.
     """
     if "message" in data:
-        raise Exception(data["message"])
+        raise RuntimeError(data["message"])
     if "errors" in data:
         err = data["errors"][0]
         if user_fix_msg := USER_FIXABLE_ERR_TYPES.get(err.get("type")):
             raise DinghyError(f"{user_fix_msg} {err['message']}")
         msg = f"GraphQL error: {err['message']}"
         if "path" in err:
             msg += f" @{'.'.join(err['path'])}"
         if "locations" in err:
             loc = err["locations"][0]
             msg += f", line {loc['line']} column {loc['column']}"
         logger.debug(f"Error data: {data}")
-        raise Exception(msg)
+        raise RuntimeError(msg)
     if "data" in data and data["data"] is None:
         # Another kind of failure response?
-        raise Exception("GraphQL query returned null")
+        raise ValueError("GraphQL query returned null")
 
 
 def _query_synopsis(query, variables):
     """
     Create a one-line synopsis of the query, for debugging and error messages.
     """
     args = ", ".join(f"{k}: {v!r}" for k, v in variables.items())
```

### Comparing `dinghy-1.2.0/src/dinghy/helpers.py` & `dinghy-1.3.0/src/dinghy/helpers.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 """
 
 import datetime
 import json
 import re
 
 import aiofiles
+from backports.datetime_fromisoformat import MonkeyPatch
+
+MonkeyPatch.patch_fromisoformat()
 
 
 class DinghyError(Exception):
     """An error in how Dinghy is being used."""
 
 
 async def json_save(data, filename):
@@ -25,15 +28,15 @@
 
     From https://stackoverflow.com/a/51916936/14343
 
     Args:
         timedelta_str (str): A string identifying a duration, like "2h13m".
 
     Returns:
-        A datetime.timedelta object.
+        A datetime.timedelta object, or None if it can't be parsed.
 
     """
     parts = re.match(
         r"""(?x)
         ^
         ((?P<weeks>[.\d]+)w(eeks?)?)?
         ((?P<days>[.\d]+)d(ays?)?)?
@@ -41,19 +44,42 @@
         ((?P<minutes>[.\d]+)m(in(utes?)?)?)?
         ((?P<seconds>[.\d]+)s(ec(onds?)?)?)?
         $
         """,
         timedelta_str.replace(" ", ""),
     )
     if not timedelta_str or parts is None:
-        raise ValueError(f"Couldn't parse time delta from {timedelta_str!r}")
+        return None
     kwargs = {name: float(val) for name, val in parts.groupdict().items() if val}
     return datetime.timedelta(**kwargs)
 
 
+def parse_since(since):
+    """
+    Parse a since specification:
+
+    - "forever" uses a long-ago date.
+    - A time delta (like "1 week") computes that long ago.
+    - A specific time (like "2023-07-30") is used as-is.
+
+    """
+    if since == "forever":
+        since_date = datetime.datetime(year=1980, month=1, day=1)
+    else:
+        delta = parse_timedelta(since)
+        if delta is not None:
+            since_date = datetime.datetime.now() - delta
+        else:
+            try:
+                since_date = datetime.datetime.fromisoformat(since)
+            except ValueError:
+                raise DinghyError("Can't parse since: {since!r}") from None
+    return since_date
+
+
 def find_dict_with_key(d, key):
     """Return the subdict of `d` that has `key`."""
     if key in d:
         return d
     for dd in d.values():
         if isinstance(dd, dict):
             sd = find_dict_with_key(dd, key)
```

### Comparing `dinghy-1.2.0/src/dinghy/jinja_helpers.py` & `dinghy-1.3.0/src/dinghy/jinja_helpers.py`

 * *Files identical despite different names*

### Comparing `dinghy-1.2.0/src/dinghy/templates/digest.html.j2` & `dinghy-1.3.0/src/dinghy/templates/digest.html.j2`

 * *Files identical despite different names*

### Comparing `dinghy-1.2.0/src/dinghy.egg-info/PKG-INFO` & `dinghy-1.3.0/src/dinghy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,51 @@
 Metadata-Version: 2.1
 Name: dinghy
-Version: 1.2.0
+Version: 1.3.0
 Summary: Dinghy daily digest tool
-Home-page: https://github.com/nedbat/dinghy
-Author: Ned Batchelder
-Author-email: ned@nedbatchelder.com
+Author-email: Ned Batchelder <ned@nedbatchelder.com>
 License: Apache-2.0
-Project-URL: Twitter, https://twitter.com/nedbat
 Project-URL: Mastodon, https://hachyderm.io/@nedbat
 Project-URL: Funding, https://github.com/sponsors/nedbat
 Project-URL: Issues, https://github.com/nedbat/dinghy/issues
 Project-URL: Source, https://github.com/nedbat/dinghy
+Project-URL: Home, https://github.com/nedbat/dinghy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Natural Language :: English
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 ######
 Dinghy
 ######
 
 Dinghy, a GitHub activity digest tool.
 
 |pypi-badge| |pyversions-badge| |license-badge|
-|sponsor-badge| |mastodon-nedbat| |twitter-nedbat|
+|sponsor-badge| |mastodon-nedbat|
 
 Dinghy uses the GitHub GraphQL API to find recent activity on releases, issues
 and pull requests, and writes a compact HTML digest `like this <sample_>`_.
 
 
+Sample Digest
+=============
+
+Here's a sample of a Dinghy digest reporting on `some PSF repos: black,
+requests, and PEPs <sample_>`_.
+
+
 Getting Started
 ===============
 
 1. Install dinghy:
 
    .. code-block:: bash
 
@@ -128,15 +134,16 @@
 
 - The ``digest`` setting is the HTML digest file to write.
 
 - The ``since`` setting indicates how far back to look for activity. It can use
   units of weeks, days, hours, minutes and seconds, and can also be
   abbreviated, like ``1d6h``. Using ``since: forever`` will include all
   activity regardless of when it happened.  If ``since`` is omitted, it
-  defaults to one week.
+  defaults to one week.  You can specify ``--since=<SINCE>`` on the dinghy
+  command line to provide an explicit value.
 
 - The ``items`` setting is a list of things to report on, specified in a few
   different ways:
 
   - The ``url`` setting is a GitHub URL, in a number of forms:
 
     - An organization project URL will report on the issues and pull requests
@@ -215,17 +222,14 @@
     :alt: Supported Python versions
 .. |license-badge| image:: https://img.shields.io/github/license/nedbat/dinghy.svg
     :target: https://github.com/nedbat/dinghy/blob/master/LICENSE.txt
     :alt: License
 .. |mastodon-nedbat| image:: https://img.shields.io/badge/dynamic/json?style=flat&labelColor=450657&logo=mastodon&logoColor=ffffff&link=https%3A%2F%2Fhachyderm.io%2F%40nedbat&url=https%3A%2F%2Fhachyderm.io%2Fusers%2Fnedbat%2Ffollowers.json&query=totalItems&label=Mastodon
     :target: https://hachyderm.io/@nedbat
     :alt: nedbat on Mastodon
-.. |twitter-nedbat| image:: https://img.shields.io/twitter/follow/nedbat.svg?label=nedbat&style=flat&logo=twitter&logoColor=4FADFF
-    :target: https://twitter.com/nedbat
-    :alt: nedbat on Twitter
 .. |sponsor-badge| image:: https://img.shields.io/badge/%E2%9D%A4-Sponsor%20me-brightgreen?style=flat&logo=GitHub
     :target: https://github.com/sponsors/nedbat
     :alt: Sponsor me on GitHub
 
 
 .. this will be appended to README.rst
 
@@ -246,14 +250,31 @@
 See the fragment files in the `scriv.d directory`_.
 
 .. _scriv.d directory: https://github.com/nedbat/dinghy/tree/master/scriv.d
 
 
 .. scriv-insert-here
 
+.. _changelog-1.3.0:
+
+1.3.0 — 2023-07-31
+------------------
+
+Added
+.....
+
+- The ``since`` date can now be specified on the command line with ``--since``.
+  This will override any specification in the YAML file.
+
+- The ``since`` value can be specified as a specific ISO 8601 date or datetime,
+  closing `issue 26`_.
+
+.. _issue 26: https://github.com/nedbat/dinghy/issues/26
+
+
 .. _changelog-1.2.0:
 
 1.2.0 — 2023-01-27
 ------------------
 
 Added
 .....
```

### Comparing `dinghy-1.2.0/src/dinghy.egg-info/SOURCES.txt` & `dinghy-1.3.0/src/dinghy.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 .editorconfig
 CHANGELOG.rst
 LICENSE.txt
 MANIFEST.in
 Makefile
 README.rst
 dev-requirements.txt
-pylintrc
-setup.cfg
-setup.py
+pyproject.toml
 scriv.d/README.txt
 src/dinghy/__init__.py
 src/dinghy/__main__.py
 src/dinghy/adhoc.py
 src/dinghy/cli.py
 src/dinghy/digest.py
 src/dinghy/graphql_helpers.py
```

### Comparing `dinghy-1.2.0/tests/test_helpers.py` & `dinghy-1.3.0/tests/test_helpers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 Test dinghy.helpers
 """
 
 import datetime
 
+import freezegun
 import pytest
 
-from dinghy.helpers import find_dict_with_key, parse_timedelta
+from dinghy.helpers import find_dict_with_key, parse_since, parse_timedelta
 
 
 @pytest.mark.parametrize(
     "tds, kwargs",
     [
         ("1d", dict(days=1)),
         ("1day", dict(days=1)),
@@ -33,16 +34,31 @@
         "one",
         "123",
         "1month",
         "2 years",
     ],
 )
 def test_bad_parse_timedelta(tds):
-    with pytest.raises(ValueError, match=f"Couldn't parse time delta from {tds!r}"):
-        parse_timedelta(tds)
+    assert parse_timedelta(tds) is None
+
+
+@freezegun.freeze_time("2023-06-16")
+@pytest.mark.parametrize(
+    "since, dtargs",
+    [
+        ("20230730", (2023, 7, 30)),
+        ("2023-06-16T12:34:56", (2023, 6, 16, 12, 34, 56)),
+        ("forever", (1980, 1, 1)),
+        ("1day", (2023, 6, 15)),
+        ("2 weeks", (2023, 6, 2)),
+        ("1 week 1 day", (2023, 6, 8)),
+    ],
+)
+def test_parse_since(since, dtargs):
+    assert parse_since(since) == datetime.datetime(*dtargs)
 
 
 @pytest.mark.parametrize(
     "d, k, res",
     [
         ({"a": 1, "b": {"k": 1}, "c": "hello"}, "k", {"k": 1}),
         (
```

