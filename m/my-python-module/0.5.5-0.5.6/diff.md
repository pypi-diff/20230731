# Comparing `tmp/my_python_module-0.5.5.tar.gz` & `tmp/my_python_module-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_python_module-0.5.5.tar", last modified: Mon Jul 31 01:07:46 2023, max compression
+gzip compressed data, was "my_python_module-0.5.6.tar", last modified: Mon Jul 31 02:33:47 2023, max compression
```

## Comparing `my_python_module-0.5.5.tar` & `my_python_module-0.5.6.tar`

### file list

```diff
@@ -1,99 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:07:46.891813 my_python_module-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-31 01:07:33.000000 my_python_module-0.5.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-31 01:07:33.000000 my_python_module-0.5.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-31 01:07:33.000000 my_python_module-0.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-31 01:07:33.000000 my_python_module-0.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-31 01:07:46.891813 my_python_module-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-31 01:07:33.000000 my_python_module-0.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:07:46.883813 my_python_module-0.5.5/my_python_module/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:07:46.887813 my_python_module-0.5.5/my_python_module/algorithm/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/algorithm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/algorithm/binary_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:07:46.887813 my_python_module-0.5.5/my_python_module/algorithm/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/algorithm/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/algorithm/graph/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/algorithm/graph/directed_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/algorithm/graph/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/algorithm/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/algorithm/graph/undirected_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/algorithm/graph/weighted_dag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:07:46.887813 my_python_module-0.5.5/my_python_module/algorithm/problems/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/algorithm/problems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/algorithm/problems/random_walk.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/algorithm/quick_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/algorithm/select_sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:07:46.887813 my_python_module-0.5.5/my_python_module/algorithm/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/algorithm/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/algorithm/tree/binary_decision_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/algorithm/tree/binary_search_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/algorithm/tree/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/algorithm/tree/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/datetime_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/functools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:07:46.887813 my_python_module-0.5.5/my_python_module/ipynb/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/ipynb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/ipynb/linear_algebra.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:07:46.887813 my_python_module-0.5.5/my_python_module/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/nlp/chinese_stop_words.py
--rw-r--r--   0 runner    (1001) docker     (123)    25940 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/nlp/nltk_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/nlp/text.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/nlp/tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/nlp/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/pathlib.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/str.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/unique_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-07-31 01:07:33.000000 my_python_module-0.5.5/my_python_module/zhnumber.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:07:46.883813 my_python_module-0.5.5/my_python_module.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-31 01:07:46.000000 my_python_module-0.5.5/my_python_module.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-07-31 01:07:46.000000 my_python_module-0.5.5/my_python_module.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 01:07:46.000000 my_python_module-0.5.5/my_python_module.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-31 01:07:46.000000 my_python_module-0.5.5/my_python_module.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-31 01:07:33.000000 my_python_module-0.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-31 01:07:46.891813 my_python_module-0.5.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:07:46.891813 my_python_module-0.5.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:07:46.891813 my_python_module-0.5.5/tests/algorithm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:07:46.891813 my_python_module-0.5.5/tests/algorithm/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/algorithm/graph/test_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/algorithm/graph/test_dijkstra.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/algorithm/graph/test_directed_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/algorithm/graph/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/algorithm/graph/test_undirected_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/algorithm/test_binary_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/algorithm/test_quick_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/algorithm/test_select_sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:07:46.891813 my_python_module-0.5.5/tests/algorithm/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/algorithm/tree/test_binary_search_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/algorithm/tree/test_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:07:46.891813 my_python_module-0.5.5/tests/backup/
--rw-r--r--   0 runner    (1001) docker     (123)    85766 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/backup/test_auto_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/backup/test_knapsack_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/backup/test_lcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/backup/test_load_corpora.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/backup/test_unique_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/backup/test_winreg_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/backup/test_winreg_utils_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:07:46.891813 my_python_module-0.5.5/tests/ipynb/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/ipynb/test_linear_algebra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:07:46.891813 my_python_module-0.5.5/tests/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/nlp/test_bigrams.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/test_fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/test_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/test_math.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/test_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-31 01:07:33.000000 my_python_module-0.5.5/tests/test_zhnumber.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:33:47.489030 my_python_module-0.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-31 02:33:38.000000 my_python_module-0.5.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-31 02:33:38.000000 my_python_module-0.5.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-31 02:33:38.000000 my_python_module-0.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-31 02:33:38.000000 my_python_module-0.5.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-31 02:33:47.489030 my_python_module-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-31 02:33:38.000000 my_python_module-0.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:33:47.485030 my_python_module-0.5.6/my_python_module/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:33:47.485030 my_python_module-0.5.6/my_python_module/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/algorithm/binary_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:33:47.485030 my_python_module-0.5.6/my_python_module/algorithm/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/algorithm/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/algorithm/graph/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/algorithm/graph/directed_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/algorithm/graph/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/algorithm/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/algorithm/graph/undirected_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/algorithm/graph/weighted_dag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:33:47.485030 my_python_module-0.5.6/my_python_module/algorithm/problems/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/algorithm/problems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/algorithm/problems/random_walk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/algorithm/quick_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/algorithm/select_sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:33:47.485030 my_python_module-0.5.6/my_python_module/algorithm/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/algorithm/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/algorithm/tree/binary_decision_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/algorithm/tree/binary_search_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/algorithm/tree/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/algorithm/tree/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/functools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:33:47.485030 my_python_module-0.5.6/my_python_module/ipynb/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/ipynb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/ipynb/linear_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:33:47.489030 my_python_module-0.5.6/my_python_module/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/nlp/chinese_stop_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25940 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/nlp/nltk_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/nlp/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/nlp/tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/nlp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/unique_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-07-31 02:33:38.000000 my_python_module-0.5.6/my_python_module/zhnumber.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:33:47.485030 my_python_module-0.5.6/my_python_module.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-31 02:33:47.000000 my_python_module-0.5.6/my_python_module.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-07-31 02:33:47.000000 my_python_module-0.5.6/my_python_module.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 02:33:47.000000 my_python_module-0.5.6/my_python_module.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-31 02:33:47.000000 my_python_module-0.5.6/my_python_module.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-31 02:33:38.000000 my_python_module-0.5.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-31 02:33:47.489030 my_python_module-0.5.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:33:47.489030 my_python_module-0.5.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:33:47.489030 my_python_module-0.5.6/tests/algorithm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:33:47.489030 my_python_module-0.5.6/tests/algorithm/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-31 02:33:38.000000 my_python_module-0.5.6/tests/algorithm/graph/test_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-31 02:33:38.000000 my_python_module-0.5.6/tests/algorithm/graph/test_dijkstra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-31 02:33:38.000000 my_python_module-0.5.6/tests/algorithm/graph/test_directed_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-31 02:33:38.000000 my_python_module-0.5.6/tests/algorithm/graph/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-31 02:33:38.000000 my_python_module-0.5.6/tests/algorithm/graph/test_undirected_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-31 02:33:38.000000 my_python_module-0.5.6/tests/algorithm/test_binary_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-31 02:33:38.000000 my_python_module-0.5.6/tests/algorithm/test_quick_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-31 02:33:38.000000 my_python_module-0.5.6/tests/algorithm/test_select_sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:33:47.489030 my_python_module-0.5.6/tests/algorithm/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-31 02:33:38.000000 my_python_module-0.5.6/tests/algorithm/tree/test_binary_search_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-31 02:33:38.000000 my_python_module-0.5.6/tests/algorithm/tree/test_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:33:47.489030 my_python_module-0.5.6/tests/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)    85766 2023-07-31 02:33:38.000000 my_python_module-0.5.6/tests/backup/test_auto_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-31 02:33:38.000000 my_python_module-0.5.6/tests/backup/test_knapsack_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-31 02:33:38.000000 my_python_module-0.5.6/tests/backup/test_lcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-31 02:33:38.000000 my_python_module-0.5.6/tests/backup/test_load_corpora.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-31 02:33:38.000000 my_python_module-0.5.6/tests/backup/test_unique_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-31 02:33:38.000000 my_python_module-0.5.6/tests/backup/test_winreg_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-31 02:33:38.000000 my_python_module-0.5.6/tests/backup/test_winreg_utils_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-31 02:33:38.000000 my_python_module-0.5.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:33:47.489030 my_python_module-0.5.6/tests/ipynb/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-31 02:33:38.000000 my_python_module-0.5.6/tests/ipynb/test_linear_algebra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:33:47.489030 my_python_module-0.5.6/tests/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-31 02:33:38.000000 my_python_module-0.5.6/tests/nlp/test_bigrams.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-31 02:33:38.000000 my_python_module-0.5.6/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-31 02:33:38.000000 my_python_module-0.5.6/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-31 02:33:38.000000 my_python_module-0.5.6/tests/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-31 02:33:38.000000 my_python_module-0.5.6/tests/test_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-31 02:33:38.000000 my_python_module-0.5.6/tests/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-31 02:33:38.000000 my_python_module-0.5.6/tests/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-31 02:33:38.000000 my_python_module-0.5.6/tests/test_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-31 02:33:38.000000 my_python_module-0.5.6/tests/test_zhnumber.py
```

### Comparing `my_python_module-0.5.5/.gitignore` & `my_python_module-0.5.6/.gitignore`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/LICENSE` & `my_python_module-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/PKG-INFO` & `my_python_module-0.5.6/my_python_module.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: my_python_module
-Version: 0.5.5
+Name: my-python-module
+Version: 0.5.6
 Summary: a general purpose python module.
 Home-page: https://github.com/a358003542/my_python_module
 Author: wanze
 Author-email: a358003542@outlook.com
 Maintainer: wanze
 Maintainer-email: a358003542@outlook.com
 License: MIT
```

### Comparing `my_python_module-0.5.5/my_python_module/algorithm/binary_search.py` & `my_python_module-0.5.6/my_python_module/algorithm/binary_search.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/my_python_module/algorithm/graph/dag.py` & `my_python_module-0.5.6/my_python_module/algorithm/graph/dag.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/my_python_module/algorithm/graph/directed_graph.py` & `my_python_module-0.5.6/my_python_module/algorithm/graph/directed_graph.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/my_python_module/algorithm/graph/graph.py` & `my_python_module-0.5.6/my_python_module/algorithm/graph/graph.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/my_python_module/algorithm/graph/undirected_graph.py` & `my_python_module-0.5.6/my_python_module/algorithm/graph/undirected_graph.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/my_python_module/algorithm/graph/weighted_dag.py` & `my_python_module-0.5.6/my_python_module/algorithm/graph/weighted_dag.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/my_python_module/algorithm/problems/random_walk.py` & `my_python_module-0.5.6/my_python_module/algorithm/problems/random_walk.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/my_python_module/algorithm/quick_sort.py` & `my_python_module-0.5.6/my_python_module/algorithm/quick_sort.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/my_python_module/algorithm/select_sort.py` & `my_python_module-0.5.6/my_python_module/algorithm/select_sort.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/my_python_module/algorithm/tree/binary_decision_tree.py` & `my_python_module-0.5.6/my_python_module/algorithm/tree/binary_decision_tree.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/my_python_module/algorithm/tree/binary_search_tree.py` & `my_python_module-0.5.6/my_python_module/algorithm/tree/binary_search_tree.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/my_python_module/algorithm/tree/tree.py` & `my_python_module-0.5.6/my_python_module/algorithm/tree/tree.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/my_python_module/common.py` & `my_python_module-0.5.6/my_python_module/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 
 """
-为本模块其他内容调用的一般性函数
+common module
 """
 
 import os
 import sys
 import logging
 import ast
 
 
 from .compat import basestring
 
 logger = logging.getLogger(__name__)
 
 
 def humanize_bytes(n, precision=1):
-    # Author: Doug Latornell
+    """
+    # based on Author: Doug Latornell's work
     # Licence: MIT
     # URL: http://code.activestate.com/recipes/577081/
-    """Return a humanized string representation of a number of bytes.
+
+    Return a humanized string representation of a number of bytes.
 
 >>> humanize_bytes(1)
 '1 B'
 >>> humanize_bytes(1024)
 '1.0 KiB'
 >>> humanize_bytes(1024 * 123)
 '123.0 KiB'
@@ -61,16 +63,16 @@
         if n >= factor:
             break
 
     return '%.*f %s' % (precision, n / factor, suffix)
 
 
 def beep(a, b):
-    """make a sound , ref:\
-     http://stackoverflow.com/questions/16573051/python-sound-alarm-when-code-finishes
+    """make a sound 
+    ref: http://stackoverflow.com/questions/16573051/python-sound-alarm-when-code-finishes
     you need install  ``apt-get install sox``
 
     :param a: frenquency
     :param b: duration
 
     create a background thread,so this function does not block the main program
     """
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `my_python_module-0.5.5/my_python_module/compat.py` & `my_python_module-0.5.6/my_python_module/compat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-
+"""
+for the sake of some compat problem
+"""
 import sys
 
 version_major = sys.version_info.major
 version_minor = sys.version_info.minor
 ######
 is_py3 = ispy3 = version_major == 3
 is_py2 = ispy2 = version_major == 2
```

### Comparing `my_python_module-0.5.5/my_python_module/datetime_utils.py` & `my_python_module-0.5.6/my_python_module/datetime.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,188 +1,173 @@
 #!/usr/bin/env python
-# -*-coding:utf-8-*-
+# -*- coding: utf-8 -*-
+
+"""
+some datetime utils
+"""
+
 
 import time
 from datetime import datetime
 
 from dateutil.relativedelta import relativedelta
 from dateutil.rrule import rrule, MONTHLY
 
 
-def is_same_year(dt1, dt2):
+utcnow = datetime.utcnow()
+"""current utcnow datetime object"""
+one_week_ago = datetime.utcnow() - relativedelta(weeks=1)
+"""one_week_ago datetime object"""
+one_day_ago = datetime.utcnow() - relativedelta(days=1)
+"""one day ago datetime object"""
+two_day_ago = datetime.utcnow() - relativedelta(days=2)
+"""two day ago datetime object"""
+one_hour_ago = datetime.utcnow() - relativedelta(hours=1)
+"""one hour ago datetime object"""
+one_month_ago = datetime.utcnow() - relativedelta(months=1)
+"""one month ago datetime object"""
+
+
+def dt_to_timestamp(dt, multiplier=1):
+    """
+    change datetime object to timestamp
+    """
+    timestamp = dt.timestamp()
+
+    timestamp = timestamp * multiplier
+
+    return int(timestamp)
+
+
+def get_datetime_range(months):
+    """
+    return a list of datetime range, start from current time, and
+    counted upon previous some months.
+    """
+    now = datetime.utcnow()
+    sdt = now - relativedelta(months=months)
+    return list(rrule(freq=MONTHLY, dtstart=sdt, until=now))
+
+
+def get_dt_fromtimestamp(timestamp, utc=False, multiplier=1):
+    """
+    get datetime object from timestamp
     """
-    判断两个datetime 对象是否是同一年
-    :param dt1:
-    :param dt2:
+
+    if isinstance(timestamp, str):
+        timestamp = float(timestamp)
+
+    timestamp = timestamp * multiplier
+
+    if utc:
+        dt = datetime.utcfromtimestamp(timestamp)
+    else:
+        dt = datetime.fromtimestamp(timestamp)
+
+    return dt
+
+
+def get_timestamp(multiplier=1):
+    """
+    get current timestamp
     :return:
     """
-    if (dt1.year == dt2.year):
+    timestamp = time.time()
+
+    timestamp = timestamp * multiplier
+
+    return int(timestamp)
+
+
+def is_same_year(dt1: datetime, dt2: datetime):
+    """
+    is the two datetime objects are in the same year
+    """
+    if dt1.year == dt2.year:
         return True
     else:
         return False
 
 
 def is_same_month(dt1, dt2):
     """
-    判断两个datetime对象是否是同一月
-    :param dt1:
-    :param dt2:
-    :return:
+    is the two datetime objects are in the same month
     """
     if (dt1.year == dt2.year) and (dt1.month == dt2.month):
         return True
     else:
         return False
 
 
 def is_same_day(dt1, dt2):
     """
-    判断两个datetime对象是否是同一天
-    :param dt1:
-    :param dt2:
-    :return:
+    is the two datetime objects are in the same day
     """
-    if (dt1.year == dt2.year) and (dt1.month == dt2.month) and (
-            dt1.day == dt2.day):
+    if (dt1.year == dt2.year) and (dt1.month == dt2.month) and (dt1.day == dt2.day):
         return True
     else:
         return False
 
 
 def is_same_hour(dt1, dt2):
     """
-    判断两个datetime对象是否是同一时
-    :param dt1:
-    :param dt2:
-    :return:
+    is the two datetime objects are in the same hour
     """
-    if (dt1.year == dt2.year) and (dt1.month == dt2.month) and (
-            dt1.day == dt2.day) and (dt1.hour == dt2.hour):
+    if (
+        (dt1.year == dt2.year)
+        and (dt1.month == dt2.month)
+        and (dt1.day == dt2.day)
+        and (dt1.hour == dt2.hour)
+    ):
         return True
     else:
         return False
 
 
-def round_to_day(dt):
+def normal_format_now():
     """
-    datetime对象round到天，更小的刻度归零
-    :param dt:
+    get current normal format for now: '2018-12-21 15:39:20'
     :return:
     """
-    res = dt.replace(hour=0, minute=0, second=0, microsecond=0)
-    return res
+    return datetime.now().__format__("%Y-%m-%d %H:%M:%S")
 
 
-def round_to_hour(dt):
+def normal_format_utcnow():
     """
-    datetime对象round到小时，更小的刻度归零
-    :param dt:
+    get current normal format for utcnow: '2018-12-21 15:39:20'
     :return:
     """
-    res = dt.replace(minute=0, second=0, microsecond=0)
-    return res
+    return datetime.utcnow().__format__("%Y-%m-%d %H:%M:%S")
 
 
-def round_to_minute(dt):
+def round_to_day(dt):
     """
-    datetime对象round到分钟
-    :param dt:
-    :return:
+    round a datetime object to day
     """
-    res = dt.replace(second=0, microsecond=0)
+    res = dt.replace(hour=0, minute=0, second=0, microsecond=0)
     return res
 
 
-def round_to_second(dt):
+def round_to_hour(dt):
     """
-    datetime对象round到秒
+    round a datetime object to hour
     :param dt:
     :return:
     """
-    res = dt.replace(microsecond=0)
+    res = dt.replace(minute=0, second=0, microsecond=0)
     return res
 
 
-def get_date_range(months):
-    """
-    返回一个时间片列表，以当前时间为终点，向前数几个月
-    :param months:
-    :return:
-    """
-    now = datetime.utcnow()
-    sdt = now - relativedelta(months=months)
-    return list(rrule(freq=MONTHLY, dtstart=sdt, until=now))
-
-
-def normal_format_now():
-    """
-    标准格式 now
-
-    '2018-12-21 15:39:20'
-    :return:
-    """
-    return datetime.now().__format__('%Y-%m-%d %H:%M:%S')
-
-
-def normal_format_utcnow():
-    """
-    标准格式 utcnow 服务器那边记录时间应该都是 utcnow
-
-    '2018-12-21 15:39:20'
-    :return:
-    """
-    return datetime.utcnow().__format__('%Y-%m-%d %H:%M:%S')
-
-
-def get_timestamp(multiplier=1):
+def round_to_minute(dt):
     """
-    获得当前的timestamp
-    :return:
+    round a datetime object to minute
     """
-    timestamp = time.time()
-
-    timestamp = timestamp * multiplier
-
-    return int(timestamp)
-
-
-def dt_to_timestamp(dt, multiplier=1):
-    timestamp = dt.timestamp()
-
-    timestamp = timestamp * multiplier
-
-    return int(timestamp)
+    res = dt.replace(second=0, microsecond=0)
+    return res
 
 
-def get_dt_fromtimestamp(timestamp, utc=False, multiplier=1):
+def round_to_second(dt):
     """
-    根据timestamp获得对应的datetime对象
+    round a datetime object to second
     """
-
-    if isinstance(timestamp, str):
-        timestamp = float(timestamp)
-
-    timestamp = timestamp * multiplier
-
-    if utc:
-        dt = datetime.utcfromtimestamp(timestamp)
-    else:
-        dt = datetime.fromtimestamp(timestamp)
-
-    return dt
-
-
-utcnow = datetime.utcnow()
-one_week_ago = datetime.utcnow() - relativedelta(weeks=1)
-one_day_ago = datetime.utcnow() - relativedelta(days=1)
-two_day_ago = datetime.utcnow() - relativedelta(days=2)
-one_hour_ago = datetime.utcnow() - relativedelta(hours=1)
-one_month_ago = datetime.utcnow() - relativedelta(months=1)
-
-__all__ = [
-    'utcnow',
-    'one_week_ago',
-    'one_day_ago',
-    'two_day_ago',
-    'one_hour_ago',
-    'one_month_ago'
-]
+    res = dt.replace(microsecond=0)
+    return res
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `my_python_module-0.5.5/my_python_module/dict.py` & `my_python_module-0.5.6/my_python_module/dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 from functools import reduce
 
 from my_python_module.compat import ispy2, ispy3
 
 
-def gen_dict_strset(d):
+def _gen_dict_strset(d):
     s = set()
     for k, v in d.items():
         item = str(k) + ':' + str(v)
         s.add(item)
     return s
 
 
@@ -33,16 +33,16 @@
 True
     """
     include = include if include is not None else {}
 
     if include == {}:  # always True
         return True
 
-    ds_set = gen_dict_strset(d)
-    includes_set = gen_dict_strset(include)
+    ds_set = _gen_dict_strset(d)
+    includes_set = _gen_dict_strset(include)
     if includes_set.issubset(ds_set):
         return True
     else:
         return False
 
 
 def check_dict_has(d, has=None):
```

### Comparing `my_python_module-0.5.5/my_python_module/exceptions.py` & `my_python_module-0.5.6/my_python_module/exceptions.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/my_python_module/functools.py` & `my_python_module-0.5.6/my_python_module/functools.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,40 +3,31 @@
 
 from functools import reduce
 from functools import wraps
 
 
 def build_compose_function(*funcs):
     """
-    组建一个符合函数流对象 数据处理流模式
-
-    每个函数的参数是任意的 但严格意义上一个合格的数据流管道设计应该在进口数据格式和入口数据格式上做出一些规范
-
-    现在做出如下规范 入口是字典格式 出口也是字典格式 当然内核更细小的粒度的函数不做如此要求，这个只是数据处理流那边
-    :param args:
-    :return:
+    combine a sequence functions to a compose function
     """
-    return reduce(lambda f, g: lambda *args, **kwargs: g(f(*args, **kwargs)),
-                  funcs)
+    return reduce(lambda f, g: lambda *args, **kwargs: g(f(*args, **kwargs)), funcs)
 
 
 def build_stream_function(*funcs):
     """
-    构建流处理函数 函数参数更严格 只接受一个参数 d 字典值
-    函数执行的顺序是从左到右
-    :param funcs:
-    :return:
+    combine a sequence funtion to a compose function, and for the sake of simplicity, 
+    limited the input parameter to a dict object.
     """
 
     return reduce(lambda f, g: lambda d: g(f(d)), funcs)
 
 
 def flatten(inlst):
     """
-    将 **多层** 列表或元组变成一维 **列表**
+    make multiple layer list or tuple to one dimension list
 
         >>> flatten((1,2,(3,4),((5,6))))
         [1, 2, 3, 4, 5, 6]
         >>> flatten([[1,2,3],[[4,5],[6]]])
         [1, 2, 3, 4, 5, 6]
 
     """
@@ -46,17 +37,17 @@
             lst.append(x)
         else:
             lst += flatten(x)
     return lst
 
 
 def sumall(*args):
-    """将所有的数字都加起来，支持多层结构。
->>> sumall(1,1,2,3,[1,2,3])
-13
->>> sumall(1,1,2,3,[1,2,3],(4,5,6),[[5,5],[6]])
-44
->>>
+    """sum all numbers, support multiple layer structure.
+    
+    >>> sumall(1,1,2,3,[1,2,3])
+    13
+    >>> sumall(1,1,2,3,[1,2,3],(4,5,6),[[5,5],[6]])
+    44
+    >>>
     """
     args = flatten(args)
     return sum(args)
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `my_python_module-0.5.5/my_python_module/json.py` & `my_python_module-0.5.6/my_python_module/json.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import shutil
 
 logger = logging.getLogger(__name__)
 
 
 def write_json(file, data):
     """
-    采用更稳妥的写文件方式，先在另外一个临时文件里面写，确保写操作无误之后再更改文件名
+    wirte data to json file, use a temporary file as a medium
     """
     fp = tempfile.NamedTemporaryFile(mode='wt', encoding='utf8', delete=False)
     try:
         json.dump(data, fp, indent=4, ensure_ascii=False)
         fp.close()
     except Exception as e:
         logger.error(f"write data to tempfile {fp.name} failed!!! \n"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `my_python_module-0.5.5/my_python_module/list.py` & `my_python_module-0.5.6/my_python_module/list.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/my_python_module/math.py` & `my_python_module-0.5.6/my_python_module/math.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 
 from .exceptions import NotIntegerError, OutOfRangeError
 
 
 def is_even(n):
     """is this number is even, required input n is a integer.
 
->>> is_even(0)
-True
->>> is_even(-1)
-False
->>> is_even(-2)
-True
+    >>> is_even(0)
+    True
+    >>> is_even(-1)
+    False
+    >>> is_even(-2)
+    True
 
     """
     if not isinstance(n, int):
         raise NotIntegerError
 
     if n % 2 == 0:
         return True
@@ -27,106 +27,105 @@
 def is_odd(n):
     """is this number is odd, required input n is a integer."""
     return not is_even(n)
 
 
 def is_prime(n):
     """test input integer n is a prime.
->>> is_prime(0)
-False
->>> is_prime(-5)
-False
->>> is_prime(-5.2)
-Traceback (most recent call last):
-  File "<stdin>", line 1, in <module>
-  File "__init__.py", line 12, in is_prime
-    raise NotIntegerError
-my_python_module.exceptions.NotIntegerError
->>> is_prime(5)
-True
->>> is_prime(123)
-False
+    >>> is_prime(0)
+    False
+    >>> is_prime(-5)
+    False
+    >>> is_prime(-5.2)
+    Traceback (most recent call last):
+      File "<stdin>", line 1, in <module>
+      File "__init__.py", line 12, in is_prime
+        raise NotIntegerError
+    my_python_module.exceptions.NotIntegerError
+    >>> is_prime(5)
+    True
+    >>> is_prime(123)
+    False
 
     """
     if not isinstance(n, int):
         raise NotIntegerError
 
     if n == 2:
         return True
     elif n < 2 or not n & 1:
         return False
-    for x in range(3, int(n ** 0.5) + 1, 2):
+    for x in range(3, int(n**0.5) + 1, 2):
         if n % x == 0:
             return False
     return True
 
 
 def gen_prime(n):
-    """到第n个的所有素数的生成器函数"""
+    """generate n prime"""
     count = 0
     x = 1
     while count < n:
         if is_prime(x):
             count += 1
             yield x
         x += 1
 
 
 def gen2_prime(n):
-    """到小于某个数n的所有素数的生成器函数"""
+    """generate prime smaller than n"""
     for x in range(n):
         if is_prime(x):
             yield x
 
 
 def last_gen(genobj):
     """
-    迭代一个生成器对象，返回最后一个元素
+    get the last element of the generator
     :param genobj:
     :return:
     """
     for i in genobj:
         last_e = i
 
     return last_e
 
 
 def prime(n):
-    """第n个素数 根据last_gen函数，所以integer类型不用判断了
-    名字取做prime而不是index_prime是因为计数从1开始。"""
+    """get the nth prime"""
     if n <= 0:
         raise OutOfRangeError("第零个或者第负数个素数？")
     else:
         return last_gen(gen_prime(n))
 
 
 def gen_fibonacci(n):
-    """到第n个的斐波那契数列生成器函数"""
+    """generate fibonacci number"""
     if not isinstance(n, int):
         raise NotIntegerError
 
     count = 0
     a, b = 0, 1
 
     while count < n:
         yield a
         a, b = b, a + b
         count += 1
 
 
 def fibonacci(n):
-    """第几个斐波那契数"""
+    """get nth fibonacci number"""
     if n <= 0:
         raise OutOfRangeError("没有零个或小于零个斐波那契数的概念那。")
     else:
         return last_gen(gen_fibonacci(n))
 
 
 def gen_factorial(stop, start=1):
-    """start*....stop的生成器，默认start=1"""
+    """start*....stop factorial generator default start=1"""
     if not isinstance(stop, int):
         raise NotIntegerError
     if not isinstance(start, int):
         raise NotIntegerError
 
     count = 0
     m = start
@@ -140,14 +139,14 @@
             yield start
             start = start * (m + 1)
             m += 1
             count += 1
 
 
 def factorial(stop, start=1):
-    """start*....stop的值，默认start=1即为stop!的值"""
+    """start*....stop factorial"""
     if stop <= 0:
         raise OutOfRangeError("负数和零的阶乘没有意义")
     elif stop < start:
         raise ValueError("终值应该比初值大")
     else:
-        return last_gen(gen_factorial(stop, start))
+        return last_gen(gen_factorial(stop, start))
```

### Comparing `my_python_module-0.5.5/my_python_module/nlp/chinese_stop_words.py` & `my_python_module-0.5.6/my_python_module/nlp/chinese_stop_words.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/my_python_module/nlp/nltk_utils.py` & `my_python_module-0.5.6/my_python_module/nlp/nltk_utils.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/my_python_module/nlp/text.py` & `my_python_module-0.5.6/my_python_module/nlp/text.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/my_python_module/nlp/tokenize.py` & `my_python_module-0.5.6/my_python_module/nlp/tokenize.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/my_python_module/nlp/utils.py` & `my_python_module-0.5.6/my_python_module/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/my_python_module/number.py` & `my_python_module-0.5.6/my_python_module/number.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/my_python_module/pathlib.py` & `my_python_module-0.5.6/my_python_module/pathlib.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/my_python_module/unique_key.py` & `my_python_module-0.5.6/my_python_module/unique_key.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/my_python_module/zhnumber.py` & `my_python_module-0.5.6/my_python_module/zhnumber.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/my_python_module.egg-info/PKG-INFO` & `my_python_module-0.5.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: my-python-module
-Version: 0.5.5
+Name: my_python_module
+Version: 0.5.6
 Summary: a general purpose python module.
 Home-page: https://github.com/a358003542/my_python_module
 Author: wanze
 Author-email: a358003542@outlook.com
 Maintainer: wanze
 Maintainer-email: a358003542@outlook.com
 License: MIT
```

### Comparing `my_python_module-0.5.5/my_python_module.egg-info/SOURCES.txt` & `my_python_module-0.5.6/my_python_module.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -4,19 +4,17 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 my_python_module/__init__.py
 my_python_module/common.py
 my_python_module/compat.py
-my_python_module/datetime_utils.py
+my_python_module/datetime.py
 my_python_module/dict.py
-my_python_module/encoding.py
 my_python_module/exceptions.py
-my_python_module/file.py
 my_python_module/functools.py
 my_python_module/json.py
 my_python_module/list.py
 my_python_module/math.py
 my_python_module/number.py
 my_python_module/pathlib.py
 my_python_module/str.py
```

### Comparing `my_python_module-0.5.5/setup.cfg` & `my_python_module-0.5.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/tests/algorithm/graph/test_dag.py` & `my_python_module-0.5.6/tests/algorithm/graph/test_dag.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/tests/algorithm/graph/test_dijkstra.py` & `my_python_module-0.5.6/tests/algorithm/graph/test_dijkstra.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/tests/algorithm/graph/test_directed_graph.py` & `my_python_module-0.5.6/tests/algorithm/graph/test_directed_graph.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/tests/algorithm/graph/test_graph.py` & `my_python_module-0.5.6/tests/algorithm/graph/test_graph.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/tests/algorithm/graph/test_undirected_graph.py` & `my_python_module-0.5.6/tests/algorithm/graph/test_undirected_graph.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/tests/algorithm/test_binary_search.py` & `my_python_module-0.5.6/tests/algorithm/test_binary_search.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/tests/algorithm/test_quick_sort.py` & `my_python_module-0.5.6/tests/algorithm/test_quick_sort.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/tests/algorithm/test_select_sort.py` & `my_python_module-0.5.6/tests/algorithm/test_select_sort.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/tests/algorithm/tree/test_tree.py` & `my_python_module-0.5.6/tests/algorithm/tree/test_tree.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/tests/backup/test_auto_summary.py` & `my_python_module-0.5.6/tests/backup/test_auto_summary.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/tests/backup/test_knapsack_problem.py` & `my_python_module-0.5.6/tests/backup/test_knapsack_problem.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/tests/backup/test_unique_key.py` & `my_python_module-0.5.6/tests/backup/test_unique_key.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/tests/ipynb/test_linear_algebra.py` & `my_python_module-0.5.6/tests/ipynb/test_linear_algebra.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/tests/nlp/test_bigrams.py` & `my_python_module-0.5.6/tests/nlp/test_bigrams.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/tests/test_basic.py` & `my_python_module-0.5.6/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/tests/test_common.py` & `my_python_module-0.5.6/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/tests/test_list.py` & `my_python_module-0.5.6/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/tests/test_math.py` & `my_python_module-0.5.6/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `my_python_module-0.5.5/tests/test_zhnumber.py` & `my_python_module-0.5.6/tests/test_zhnumber.py`

 * *Files identical despite different names*

