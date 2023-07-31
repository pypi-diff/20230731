# Comparing `tmp/my_python_module-0.5.4.tar.gz` & `tmp/my_python_module-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_python_module-0.5.4.tar", last modified: Fri Jul 28 09:09:55 2023, max compression
+gzip compressed data, was "my_python_module-0.5.5.tar", last modified: Mon Jul 31 01:07:46 2023, max compression
```

## Comparing `my_python_module-0.5.4.tar` & `my_python_module-0.5.5.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:09:55.860328 my_python_module-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-28 09:09:40.000000 my_python_module-0.5.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-28 09:09:40.000000 my_python_module-0.5.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-28 09:09:40.000000 my_python_module-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-28 09:09:40.000000 my_python_module-0.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-28 09:09:55.860328 my_python_module-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-28 09:09:40.000000 my_python_module-0.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:09:55.848328 my_python_module-0.5.4/my_python_module/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:09:55.848328 my_python_module-0.5.4/my_python_module/algorithm/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/algorithm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/algorithm/binary_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:09:55.852328 my_python_module-0.5.4/my_python_module/algorithm/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/algorithm/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/algorithm/graph/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/algorithm/graph/directed_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/algorithm/graph/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/algorithm/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/algorithm/graph/undirected_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/algorithm/graph/weighted_dag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:09:55.852328 my_python_module-0.5.4/my_python_module/algorithm/problems/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/algorithm/problems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/algorithm/problems/random_walk.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/algorithm/quick_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/algorithm/select_sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:09:55.852328 my_python_module-0.5.4/my_python_module/algorithm/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/algorithm/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/algorithm/tree/binary_decision_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/algorithm/tree/binary_search_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/algorithm/tree/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/algorithm/tree/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/datetime_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/functools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:09:55.852328 my_python_module-0.5.4/my_python_module/ipynb/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/ipynb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/ipynb/linear_algebra.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:09:55.852328 my_python_module-0.5.4/my_python_module/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/nlp/chinese_stop_words.py
--rw-r--r--   0 runner    (1001) docker     (123)    25940 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/nlp/nltk_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/nlp/text.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/nlp/tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/nlp/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/pathlib.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/str.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/unique_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-07-28 09:09:40.000000 my_python_module-0.5.4/my_python_module/zhnumber.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:09:55.848328 my_python_module-0.5.4/my_python_module.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-28 09:09:55.000000 my_python_module-0.5.4/my_python_module.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-07-28 09:09:55.000000 my_python_module-0.5.4/my_python_module.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 09:09:55.000000 my_python_module-0.5.4/my_python_module.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 09:09:55.000000 my_python_module-0.5.4/my_python_module.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-28 09:09:40.000000 my_python_module-0.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-28 09:09:55.860328 my_python_module-0.5.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:09:55.856328 my_python_module-0.5.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:09:55.856328 my_python_module-0.5.4/tests/algorithm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:09:55.856328 my_python_module-0.5.4/tests/algorithm/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-28 09:09:40.000000 my_python_module-0.5.4/tests/algorithm/graph/test_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-28 09:09:40.000000 my_python_module-0.5.4/tests/algorithm/graph/test_dijkstra.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-28 09:09:40.000000 my_python_module-0.5.4/tests/algorithm/graph/test_directed_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-28 09:09:40.000000 my_python_module-0.5.4/tests/algorithm/graph/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-28 09:09:40.000000 my_python_module-0.5.4/tests/algorithm/graph/test_undirected_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-28 09:09:40.000000 my_python_module-0.5.4/tests/algorithm/test_binary_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-28 09:09:40.000000 my_python_module-0.5.4/tests/algorithm/test_quick_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-28 09:09:40.000000 my_python_module-0.5.4/tests/algorithm/test_select_sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:09:55.856328 my_python_module-0.5.4/tests/algorithm/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-28 09:09:40.000000 my_python_module-0.5.4/tests/algorithm/tree/test_binary_search_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-28 09:09:40.000000 my_python_module-0.5.4/tests/algorithm/tree/test_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:09:55.860328 my_python_module-0.5.4/tests/backup/
--rw-r--r--   0 runner    (1001) docker     (123)    85766 2023-07-28 09:09:40.000000 my_python_module-0.5.4/tests/backup/test_auto_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-28 09:09:40.000000 my_python_module-0.5.4/tests/backup/test_knapsack_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-28 09:09:40.000000 my_python_module-0.5.4/tests/backup/test_lcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-28 09:09:40.000000 my_python_module-0.5.4/tests/backup/test_load_corpora.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-28 09:09:40.000000 my_python_module-0.5.4/tests/backup/test_unique_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-28 09:09:40.000000 my_python_module-0.5.4/tests/backup/test_winreg_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-28 09:09:40.000000 my_python_module-0.5.4/tests/backup/test_winreg_utils_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-28 09:09:40.000000 my_python_module-0.5.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:09:55.860328 my_python_module-0.5.4/tests/ipynb/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-28 09:09:40.000000 my_python_module-0.5.4/tests/ipynb/test_linear_algebra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:09:55.860328 my_python_module-0.5.4/tests/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-28 09:09:40.000000 my_python_module-0.5.4/tests/nlp/test_bigrams.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-28 09:09:40.000000 my_python_module-0.5.4/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-28 09:09:40.000000 my_python_module-0.5.4/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-28 09:09:40.000000 my_python_module-0.5.4/tests/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-28 09:09:40.000000 my_python_module-0.5.4/tests/test_fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-28 09:09:40.000000 my_python_module-0.5.4/tests/test_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-28 09:09:40.000000 my_python_module-0.5.4/tests/test_math.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-28 09:09:40.000000 my_python_module-0.5.4/tests/test_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-28 09:09:40.000000 my_python_module-0.5.4/tests/test_zhnumber.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:07:46.891813 my_python_module-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-31 01:07:33.000000 my_python_module-0.5.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-31 01:07:33.000000 my_python_module-0.5.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-31 01:07:33.000000 my_python_module-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-31 01:07:33.000000 my_python_module-0.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-31 01:07:46.891813 my_python_module-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-31 01:07:33.000000 my_python_module-0.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:07:46.883813 my_python_module-0.5.5/my_python_module/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:07:46.887813 my_python_module-0.5.5/my_python_module/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/algorithm/binary_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:07:46.887813 my_python_module-0.5.5/my_python_module/algorithm/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/algorithm/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/algorithm/graph/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/algorithm/graph/directed_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/algorithm/graph/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/algorithm/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/algorithm/graph/undirected_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/algorithm/graph/weighted_dag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:07:46.887813 my_python_module-0.5.5/my_python_module/algorithm/problems/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/algorithm/problems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/algorithm/problems/random_walk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/algorithm/quick_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/algorithm/select_sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:07:46.887813 my_python_module-0.5.5/my_python_module/algorithm/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/algorithm/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/algorithm/tree/binary_decision_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/algorithm/tree/binary_search_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/algorithm/tree/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/algorithm/tree/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/datetime_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/functools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:07:46.887813 my_python_module-0.5.5/my_python_module/ipynb/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/ipynb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/ipynb/linear_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:07:46.887813 my_python_module-0.5.5/my_python_module/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/nlp/chinese_stop_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25940 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/nlp/nltk_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/nlp/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/nlp/tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/nlp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/unique_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/zhnumber.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:07:46.883813 my_python_module-0.5.5/my_python_module.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-31 01:07:46.000000 my_python_module-0.5.5/my_python_module.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-07-31 01:07:46.000000 my_python_module-0.5.5/my_python_module.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 01:07:46.000000 my_python_module-0.5.5/my_python_module.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-31 01:07:46.000000 my_python_module-0.5.5/my_python_module.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-31 01:07:33.000000 my_python_module-0.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-31 01:07:46.891813 my_python_module-0.5.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:07:46.891813 my_python_module-0.5.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:07:46.891813 my_python_module-0.5.5/tests/algorithm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:07:46.891813 my_python_module-0.5.5/tests/algorithm/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/algorithm/graph/test_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/algorithm/graph/test_dijkstra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/algorithm/graph/test_directed_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/algorithm/graph/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/algorithm/graph/test_undirected_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/algorithm/test_binary_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/algorithm/test_quick_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/algorithm/test_select_sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:07:46.891813 my_python_module-0.5.5/tests/algorithm/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/algorithm/tree/test_binary_search_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/algorithm/tree/test_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:07:46.891813 my_python_module-0.5.5/tests/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)    85766 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/backup/test_auto_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/backup/test_knapsack_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/backup/test_lcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/backup/test_load_corpora.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/backup/test_unique_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/backup/test_winreg_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/backup/test_winreg_utils_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:07:46.891813 my_python_module-0.5.5/tests/ipynb/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/ipynb/test_linear_algebra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:07:46.891813 my_python_module-0.5.5/tests/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/nlp/test_bigrams.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/test_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/test_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/test_zhnumber.py
```

### Comparing `my_python_module-0.5.4/.gitignore` & `my_python_module-0.5.5/.gitignore`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/LICENSE` & `my_python_module-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/PKG-INFO` & `my_python_module-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my_python_module
-Version: 0.5.4
+Version: 0.5.5
 Summary: a general purpose python module.
 Home-page: https://github.com/a358003542/my_python_module
 Author: wanze
 Author-email: a358003542@outlook.com
 Maintainer: wanze
 Maintainer-email: a358003542@outlook.com
 License: MIT
```

### Comparing `my_python_module-0.5.4/my_python_module/algorithm/binary_search.py` & `my_python_module-0.5.5/my_python_module/algorithm/binary_search.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/my_python_module/algorithm/graph/dag.py` & `my_python_module-0.5.5/my_python_module/algorithm/graph/dag.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/my_python_module/algorithm/graph/directed_graph.py` & `my_python_module-0.5.5/my_python_module/algorithm/graph/directed_graph.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/my_python_module/algorithm/graph/graph.py` & `my_python_module-0.5.5/my_python_module/algorithm/graph/graph.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/my_python_module/algorithm/graph/undirected_graph.py` & `my_python_module-0.5.5/my_python_module/algorithm/graph/undirected_graph.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/my_python_module/algorithm/graph/weighted_dag.py` & `my_python_module-0.5.5/my_python_module/algorithm/graph/weighted_dag.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/my_python_module/algorithm/problems/random_walk.py` & `my_python_module-0.5.5/my_python_module/algorithm/problems/random_walk.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/my_python_module/algorithm/quick_sort.py` & `my_python_module-0.5.5/my_python_module/algorithm/quick_sort.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/my_python_module/algorithm/select_sort.py` & `my_python_module-0.5.5/my_python_module/algorithm/select_sort.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/my_python_module/algorithm/tree/binary_decision_tree.py` & `my_python_module-0.5.5/my_python_module/algorithm/tree/binary_decision_tree.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/my_python_module/algorithm/tree/binary_search_tree.py` & `my_python_module-0.5.5/my_python_module/algorithm/tree/binary_search_tree.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/my_python_module/algorithm/tree/tree.py` & `my_python_module-0.5.5/my_python_module/algorithm/tree/tree.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/my_python_module/common.py` & `my_python_module-0.5.5/my_python_module/common.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/my_python_module/compat.py` & `my_python_module-0.5.5/my_python_module/compat.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/my_python_module/datetime_utils.py` & `my_python_module-0.5.5/my_python_module/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/my_python_module/dict.py` & `my_python_module-0.5.5/my_python_module/dict.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/my_python_module/encoding.py` & `my_python_module-0.5.5/my_python_module/encoding.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/my_python_module/exceptions.py` & `my_python_module-0.5.5/my_python_module/exceptions.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/my_python_module/file.py` & `my_python_module-0.5.5/my_python_module/file.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/my_python_module/functools.py` & `my_python_module-0.5.5/my_python_module/functools.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/my_python_module/ipynb/linear_algebra.py` & `my_python_module-0.5.5/my_python_module/ipynb/linear_algebra.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/my_python_module/json.py` & `my_python_module-0.5.5/my_python_module/json.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/my_python_module/list.py` & `my_python_module-0.5.5/my_python_module/list.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/my_python_module/math.py` & `my_python_module-0.5.5/my_python_module/math.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/my_python_module/nlp/chinese_stop_words.py` & `my_python_module-0.5.5/my_python_module/nlp/chinese_stop_words.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/my_python_module/nlp/nltk_utils.py` & `my_python_module-0.5.5/my_python_module/nlp/nltk_utils.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/my_python_module/nlp/text.py` & `my_python_module-0.5.5/my_python_module/nlp/text.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/my_python_module/nlp/tokenize.py` & `my_python_module-0.5.5/my_python_module/nlp/tokenize.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/my_python_module/nlp/utils.py` & `my_python_module-0.5.5/my_python_module/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/my_python_module/number.py` & `my_python_module-0.5.5/my_python_module/number.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/my_python_module/pathlib.py` & `my_python_module-0.5.5/my_python_module/pathlib.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/my_python_module/unique_key.py` & `my_python_module-0.5.5/my_python_module/unique_key.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/my_python_module/zhnumber.py` & `my_python_module-0.5.5/my_python_module/zhnumber.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/my_python_module.egg-info/PKG-INFO` & `my_python_module-0.5.5/my_python_module.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my-python-module
-Version: 0.5.4
+Version: 0.5.5
 Summary: a general purpose python module.
 Home-page: https://github.com/a358003542/my_python_module
 Author: wanze
 Author-email: a358003542@outlook.com
 Maintainer: wanze
 Maintainer-email: a358003542@outlook.com
 License: MIT
```

### Comparing `my_python_module-0.5.4/my_python_module.egg-info/SOURCES.txt` & `my_python_module-0.5.5/my_python_module.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/setup.cfg` & `my_python_module-0.5.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/tests/algorithm/graph/test_dag.py` & `my_python_module-0.5.5/tests/algorithm/graph/test_dag.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/tests/algorithm/graph/test_dijkstra.py` & `my_python_module-0.5.5/tests/algorithm/graph/test_dijkstra.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/tests/algorithm/graph/test_directed_graph.py` & `my_python_module-0.5.5/tests/algorithm/graph/test_directed_graph.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/tests/algorithm/graph/test_graph.py` & `my_python_module-0.5.5/tests/algorithm/graph/test_graph.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/tests/algorithm/graph/test_undirected_graph.py` & `my_python_module-0.5.5/tests/algorithm/graph/test_undirected_graph.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/tests/algorithm/test_binary_search.py` & `my_python_module-0.5.5/tests/algorithm/test_binary_search.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/tests/algorithm/test_quick_sort.py` & `my_python_module-0.5.5/tests/algorithm/test_quick_sort.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/tests/algorithm/test_select_sort.py` & `my_python_module-0.5.5/tests/algorithm/test_select_sort.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/tests/algorithm/tree/test_tree.py` & `my_python_module-0.5.5/tests/algorithm/tree/test_tree.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/tests/backup/test_auto_summary.py` & `my_python_module-0.5.5/tests/backup/test_auto_summary.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/tests/backup/test_knapsack_problem.py` & `my_python_module-0.5.5/tests/backup/test_knapsack_problem.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/tests/backup/test_unique_key.py` & `my_python_module-0.5.5/tests/backup/test_unique_key.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/tests/ipynb/test_linear_algebra.py` & `my_python_module-0.5.5/tests/ipynb/test_linear_algebra.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/tests/nlp/test_bigrams.py` & `my_python_module-0.5.5/tests/nlp/test_bigrams.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/tests/test_basic.py` & `my_python_module-0.5.5/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/tests/test_common.py` & `my_python_module-0.5.5/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/tests/test_list.py` & `my_python_module-0.5.5/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/tests/test_math.py` & `my_python_module-0.5.5/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.4/tests/test_zhnumber.py` & `my_python_module-0.5.5/tests/test_zhnumber.py`

 * *Files identical despite different names*

