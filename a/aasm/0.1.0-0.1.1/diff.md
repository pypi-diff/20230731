# Comparing `tmp/aasm-0.1.0.tar.gz` & `tmp/aasm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aasm-0.1.0.tar", last modified: Thu Jul 20 12:20:03 2023, max compression
+gzip compressed data, was "aasm-0.1.1.tar", last modified: Mon Jul 31 12:48:02 2023, max compression
```

## Comparing `aasm-0.1.0.tar` & `aasm-0.1.1.tar`

### file list

```diff
@@ -1,90 +1,90 @@
--rw-r--r--   0        0        0       37 2022-12-17 05:36:13.052938 aasm-0.1.0/.gitignore
--rw-r--r--   0        0        0      172 2023-05-22 10:06:04.170277 aasm-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      709 2022-12-17 01:24:38.903482 aasm-0.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    11941 2023-07-18 15:16:59.750006 aasm-0.1.0/DOCS.md
--rw-r--r--   0        0        0     1084 2023-05-22 10:07:10.253613 aasm-0.1.0/LICENSE.md
--rw-r--r--   0        0        0      349 2023-05-22 10:07:10.253613 aasm-0.1.0/Pipfile
--rw-r--r--   0        0        0    66634 2023-05-22 10:07:10.256947 aasm-0.1.0/Pipfile.lock
--rw-r--r--   0        0        0     3169 2022-12-17 01:24:38.906815 aasm-0.1.0/README.md
--rw-r--r--   0        0        0      303 2023-07-20 12:19:13.796717 aasm-0.1.0/aasm/__init__.py
--rw-r--r--   0        0        0        0 2022-12-17 01:24:38.906815 aasm-0.1.0/aasm/generating/__init__.py
--rw-r--r--   0        0        0     1309 2023-07-18 15:16:59.750006 aasm-0.1.0/aasm/generating/code.py
--rw-r--r--   0        0        0     1250 2023-07-18 15:16:59.750006 aasm-0.1.0/aasm/generating/python_code.py
--rw-r--r--   0        0        0    15718 2023-07-19 14:25:12.646717 aasm-0.1.0/aasm/generating/python_graph.py
--rw-r--r--   0        0        0     1860 2023-07-20 12:15:22.310040 aasm-0.1.0/aasm/generating/python_module.py
--rw-r--r--   0        0        0    49947 2023-07-18 15:16:59.750006 aasm-0.1.0/aasm/generating/python_spade.py
--rw-r--r--   0        0        0        0 2022-12-17 01:24:38.906815 aasm-0.1.0/aasm/intermediate/__init__.py
--rw-r--r--   0        0        0     2857 2023-07-18 15:16:59.753340 aasm-0.1.0/aasm/intermediate/action.py
--rw-r--r--   0        0        0     9515 2023-07-18 15:16:59.753340 aasm-0.1.0/aasm/intermediate/agent.py
--rw-r--r--   0        0        0    20777 2023-07-18 15:21:47.523352 aasm-0.1.0/aasm/intermediate/argument.py
--rw-r--r--   0        0        0     1323 2022-12-17 01:24:38.906815 aasm-0.1.0/aasm/intermediate/behaviour.py
--rw-r--r--   0        0        0     4263 2023-07-18 15:16:59.753340 aasm-0.1.0/aasm/intermediate/block.py
--rw-r--r--   0        0        0     1225 2023-07-18 15:16:59.753340 aasm-0.1.0/aasm/intermediate/declaration.py
--rw-r--r--   0        0        0     8031 2023-07-18 15:16:59.753340 aasm-0.1.0/aasm/intermediate/graph.py
--rw-r--r--   0        0        0    12166 2023-07-18 15:16:59.753340 aasm-0.1.0/aasm/intermediate/instruction.py
--rw-r--r--   0        0        0     4013 2023-07-18 15:16:59.753340 aasm-0.1.0/aasm/intermediate/message.py
--rw-r--r--   0        0        0       79 2023-07-18 15:16:59.753340 aasm-0.1.0/aasm/intermediate/module.py
--rw-r--r--   0        0        0        0 2023-07-18 15:16:59.753340 aasm-0.1.0/aasm/modules/__init__.py
--rw-r--r--   0        0        0     5094 2023-07-18 15:16:59.753340 aasm-0.1.0/aasm/modules/instruction.py
--rw-r--r--   0        0        0     8168 2023-07-18 15:16:59.753340 aasm-0.1.0/aasm/modules/module.py
--rw-r--r--   0        0        0      473 2023-07-18 15:16:59.756673 aasm-0.1.0/aasm/modules/type.py
--rw-r--r--   0        0        0        0 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/__init__.py
--rw-r--r--   0        0        0        0 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/__init__.py
--rw-r--r--   0        0        0     2130 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/action.py
--rw-r--r--   0        0        0     1474 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/agent.py
--rw-r--r--   0        0        0     3033 2022-12-17 05:28:29.899621 aasm-0.1.0/aasm/parsing/op/behav.py
--rw-r--r--   0        0        0      619 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/clr.py
--rw-r--r--   0        0        0     2808 2022-12-17 05:28:29.922954 aasm-0.1.0/aasm/parsing/op/conditional.py
--rw-r--r--   0        0        0     1942 2023-07-18 15:17:32.240008 aasm-0.1.0/aasm/parsing/op/decl.py
--rw-r--r--   0        0        0     3956 2023-07-19 14:25:12.646717 aasm-0.1.0/aasm/parsing/op/defg.py
--rw-r--r--   0        0        0      953 2023-07-18 15:16:59.756673 aasm-0.1.0/aasm/parsing/op/defnode.py
--rw-r--r--   0        0        0     2340 2023-07-18 15:16:59.756673 aasm-0.1.0/aasm/parsing/op/deftype.py
--rw-r--r--   0        0        0      427 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/eblock.py
--rw-r--r--   0        0        0     2378 2023-07-18 15:16:59.756673 aasm-0.1.0/aasm/parsing/op/graph.py
--rw-r--r--   0        0        0      690 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/len.py
--rw-r--r--   0        0        0     1013 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/list_inclusion.py
--rw-r--r--   0        0        0     1002 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/list_modification.py
--rw-r--r--   0        0        0     1418 2023-07-18 15:16:59.756673 aasm-0.1.0/aasm/parsing/op/logs.py
--rw-r--r--   0        0        0      771 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/lr.py
--rw-r--r--   0        0        0      783 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/lw.py
--rw-r--r--   0        0        0     1284 2022-12-17 05:28:30.012955 aasm-0.1.0/aasm/parsing/op/math.py
--rw-r--r--   0        0        0     1056 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/math_exp.py
--rw-r--r--   0        0        0      803 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/math_mod.py
--rw-r--r--   0        0        0     1695 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/message.py
--rw-r--r--   0        0        0     1139 2023-07-18 15:16:59.756673 aasm-0.1.0/aasm/parsing/op/module.py
--rw-r--r--   0        0        0      713 2023-07-18 15:16:59.756673 aasm-0.1.0/aasm/parsing/op/mparams.py
--rw-r--r--   0        0        0     5561 2023-07-18 15:21:47.523352 aasm-0.1.0/aasm/parsing/op/prm.py
--rw-r--r--   0        0        0     2289 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/rand.py
--rw-r--r--   0        0        0      748 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/remen.py
--rw-r--r--   0        0        0      620 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/round.py
--rw-r--r--   0        0        0      606 2022-12-17 05:36:13.052938 aasm-0.1.0/aasm/parsing/op/scale.py
--rw-r--r--   0        0        0      880 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/send.py
--rw-r--r--   0        0        0      690 2023-07-18 15:21:47.523352 aasm-0.1.0/aasm/parsing/op/set.py
--rw-r--r--   0        0        0      603 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/size.py
--rw-r--r--   0        0        0      803 2022-12-17 01:24:38.910148 aasm-0.1.0/aasm/parsing/op/subs.py
--rw-r--r--   0        0        0      893 2023-07-18 15:16:59.756673 aasm-0.1.0/aasm/parsing/op/types.py
--rw-r--r--   0        0        0     6593 2023-07-18 15:16:59.756673 aasm-0.1.0/aasm/parsing/parse.py
--rw-r--r--   0        0        0     5804 2023-07-18 15:16:59.756673 aasm-0.1.0/aasm/parsing/state.py
--rw-r--r--   0        0        0        0 2022-12-17 01:24:38.913482 aasm-0.1.0/aasm/preprocessor/__init__.py
--rw-r--r--   0        0        0      839 2022-12-17 01:24:38.913482 aasm-0.1.0/aasm/preprocessor/constant.py
--rw-r--r--   0        0        0     1484 2022-12-17 01:24:38.913482 aasm-0.1.0/aasm/preprocessor/macro.py
--rw-r--r--   0        0        0     7930 2022-12-17 05:36:13.056271 aasm-0.1.0/aasm/preprocessor/preprocessor.py
--rw-r--r--   0        0        0      292 2022-12-17 01:24:38.913482 aasm-0.1.0/aasm/preprocessor/preprocessor_item.py
--rw-r--r--   0        0        0     2312 2023-07-20 12:15:22.313373 aasm-0.1.0/aasm/translate.py
--rw-r--r--   0        0        0        0 2022-12-17 01:24:38.913482 aasm-0.1.0/aasm/utils/__init__.py
--rw-r--r--   0        0        0      428 2022-12-17 01:24:38.913482 aasm-0.1.0/aasm/utils/exception.py
--rw-r--r--   0        0        0      412 2022-12-17 01:24:38.913482 aasm-0.1.0/aasm/utils/iteration.py
--rw-r--r--   0        0        0     2074 2023-07-19 14:27:17.546723 aasm-0.1.0/aasm/utils/validation.py
--rw-r--r--   0        0        0      673 2023-05-22 10:07:10.256947 aasm-0.1.0/examples/EXAMPLES.md
--rw-r--r--   0        0        0      837 2023-07-18 15:16:59.756673 aasm-0.1.0/examples/basic/facebook.aasm
--rw-r--r--   0        0        0      968 2023-07-18 15:16:59.756673 aasm-0.1.0/examples/basic/facebook_macro.aasm
--rw-r--r--   0        0        0    14394 2023-07-18 15:16:59.756673 aasm-0.1.0/examples/basic/wolfsheep.aasm
--rw-r--r--   0        0        0    11149 2023-07-18 15:16:59.760006 aasm-0.1.0/examples/basic/wolfsheep_macro.aasm
--rw-r--r--   0        0        0     1115 2023-07-19 14:25:12.646717 aasm-0.1.0/examples/graphs/barabasi-albert.aasm
--rw-r--r--   0        0        0     1152 2023-07-18 15:16:59.760006 aasm-0.1.0/examples/graphs/inhomogenous.aasm
--rw-r--r--   0        0        0     1179 2023-07-18 15:16:59.760006 aasm-0.1.0/examples/graphs/matrix.aasm
--rw-r--r--   0        0        0     1129 2023-07-19 14:25:12.646717 aasm-0.1.0/examples/graphs/statistical.aasm
--rw-r--r--   0        0        0     1153 2023-07-18 15:16:59.760006 aasm-0.1.0/examples/modules/facebook_uuid.aasm
--rw-r--r--   0        0        0      649 2023-07-18 15:21:47.523352 aasm-0.1.0/examples/modules/uuid.aasm.mod
--rw-r--r--   0        0        0      499 2022-12-17 01:24:38.913482 aasm-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3495 1970-01-01 00:00:00.000000 aasm-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       37 2022-12-17 05:36:13.052938 aasm-0.1.1/.gitignore
+-rw-r--r--   0        0        0      172 2023-05-22 10:06:04.170277 aasm-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      709 2022-12-17 01:24:38.903482 aasm-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11941 2023-07-18 15:16:59.750006 aasm-0.1.1/DOCS.md
+-rw-r--r--   0        0        0     1084 2023-05-22 10:07:10.253613 aasm-0.1.1/LICENSE.md
+-rw-r--r--   0        0        0      349 2023-05-22 10:07:10.253613 aasm-0.1.1/Pipfile
+-rw-r--r--   0        0        0    66634 2023-05-22 10:07:10.256947 aasm-0.1.1/Pipfile.lock
+-rw-r--r--   0        0        0     3169 2022-12-17 01:24:38.906815 aasm-0.1.1/README.md
+-rw-r--r--   0        0        0      303 2023-07-31 12:47:35.557325 aasm-0.1.1/aasm/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-17 01:24:38.906815 aasm-0.1.1/aasm/generating/__init__.py
+-rw-r--r--   0        0        0     1309 2023-07-18 15:16:59.750006 aasm-0.1.1/aasm/generating/code.py
+-rw-r--r--   0        0        0     1250 2023-07-18 15:16:59.750006 aasm-0.1.1/aasm/generating/python_code.py
+-rw-r--r--   0        0        0    15718 2023-07-19 14:25:12.646717 aasm-0.1.1/aasm/generating/python_graph.py
+-rw-r--r--   0        0        0     1931 2023-07-27 11:49:19.420369 aasm-0.1.1/aasm/generating/python_module.py
+-rw-r--r--   0        0        0    49791 2023-07-27 11:47:49.387031 aasm-0.1.1/aasm/generating/python_spade.py
+-rw-r--r--   0        0        0        0 2022-12-17 01:24:38.906815 aasm-0.1.1/aasm/intermediate/__init__.py
+-rw-r--r--   0        0        0     2857 2023-07-18 15:16:59.753340 aasm-0.1.1/aasm/intermediate/action.py
+-rw-r--r--   0        0        0     9515 2023-07-18 15:16:59.753340 aasm-0.1.1/aasm/intermediate/agent.py
+-rw-r--r--   0        0        0    20777 2023-07-18 15:21:47.523352 aasm-0.1.1/aasm/intermediate/argument.py
+-rw-r--r--   0        0        0     1323 2022-12-17 01:24:38.906815 aasm-0.1.1/aasm/intermediate/behaviour.py
+-rw-r--r--   0        0        0     4263 2023-07-18 15:16:59.753340 aasm-0.1.1/aasm/intermediate/block.py
+-rw-r--r--   0        0        0     1225 2023-07-18 15:16:59.753340 aasm-0.1.1/aasm/intermediate/declaration.py
+-rw-r--r--   0        0        0     8031 2023-07-18 15:16:59.753340 aasm-0.1.1/aasm/intermediate/graph.py
+-rw-r--r--   0        0        0    12166 2023-07-18 15:16:59.753340 aasm-0.1.1/aasm/intermediate/instruction.py
+-rw-r--r--   0        0        0     4013 2023-07-18 15:16:59.753340 aasm-0.1.1/aasm/intermediate/message.py
+-rw-r--r--   0        0        0       79 2023-07-18 15:16:59.753340 aasm-0.1.1/aasm/intermediate/module.py
+-rw-r--r--   0        0        0        0 2023-07-18 15:16:59.753340 aasm-0.1.1/aasm/modules/__init__.py
+-rw-r--r--   0        0        0     5094 2023-07-18 15:16:59.753340 aasm-0.1.1/aasm/modules/instruction.py
+-rw-r--r--   0        0        0     8168 2023-07-18 15:16:59.753340 aasm-0.1.1/aasm/modules/module.py
+-rw-r--r--   0        0        0      473 2023-07-18 15:16:59.756673 aasm-0.1.1/aasm/modules/type.py
+-rw-r--r--   0        0        0        0 2022-12-17 01:24:38.910148 aasm-0.1.1/aasm/parsing/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-17 01:24:38.910148 aasm-0.1.1/aasm/parsing/op/__init__.py
+-rw-r--r--   0        0        0     2130 2022-12-17 01:24:38.910148 aasm-0.1.1/aasm/parsing/op/action.py
+-rw-r--r--   0        0        0     1474 2022-12-17 01:24:38.910148 aasm-0.1.1/aasm/parsing/op/agent.py
+-rw-r--r--   0        0        0     3033 2022-12-17 05:28:29.899621 aasm-0.1.1/aasm/parsing/op/behav.py
+-rw-r--r--   0        0        0      619 2022-12-17 01:24:38.910148 aasm-0.1.1/aasm/parsing/op/clr.py
+-rw-r--r--   0        0        0     2808 2022-12-17 05:28:29.922954 aasm-0.1.1/aasm/parsing/op/conditional.py
+-rw-r--r--   0        0        0     1942 2023-07-18 15:17:32.240008 aasm-0.1.1/aasm/parsing/op/decl.py
+-rw-r--r--   0        0        0     3956 2023-07-19 14:25:12.646717 aasm-0.1.1/aasm/parsing/op/defg.py
+-rw-r--r--   0        0        0      953 2023-07-18 15:16:59.756673 aasm-0.1.1/aasm/parsing/op/defnode.py
+-rw-r--r--   0        0        0     2340 2023-07-18 15:16:59.756673 aasm-0.1.1/aasm/parsing/op/deftype.py
+-rw-r--r--   0        0        0      427 2022-12-17 01:24:38.910148 aasm-0.1.1/aasm/parsing/op/eblock.py
+-rw-r--r--   0        0        0     2378 2023-07-18 15:16:59.756673 aasm-0.1.1/aasm/parsing/op/graph.py
+-rw-r--r--   0        0        0      690 2022-12-17 01:24:38.910148 aasm-0.1.1/aasm/parsing/op/len.py
+-rw-r--r--   0        0        0     1013 2022-12-17 01:24:38.910148 aasm-0.1.1/aasm/parsing/op/list_inclusion.py
+-rw-r--r--   0        0        0     1002 2022-12-17 01:24:38.910148 aasm-0.1.1/aasm/parsing/op/list_modification.py
+-rw-r--r--   0        0        0     1418 2023-07-18 15:16:59.756673 aasm-0.1.1/aasm/parsing/op/logs.py
+-rw-r--r--   0        0        0      771 2022-12-17 01:24:38.910148 aasm-0.1.1/aasm/parsing/op/lr.py
+-rw-r--r--   0        0        0      783 2022-12-17 01:24:38.910148 aasm-0.1.1/aasm/parsing/op/lw.py
+-rw-r--r--   0        0        0     1284 2022-12-17 05:28:30.012955 aasm-0.1.1/aasm/parsing/op/math.py
+-rw-r--r--   0        0        0     1056 2022-12-17 01:24:38.910148 aasm-0.1.1/aasm/parsing/op/math_exp.py
+-rw-r--r--   0        0        0      803 2022-12-17 01:24:38.910148 aasm-0.1.1/aasm/parsing/op/math_mod.py
+-rw-r--r--   0        0        0     1695 2022-12-17 01:24:38.910148 aasm-0.1.1/aasm/parsing/op/message.py
+-rw-r--r--   0        0        0     1139 2023-07-18 15:16:59.756673 aasm-0.1.1/aasm/parsing/op/module.py
+-rw-r--r--   0        0        0      713 2023-07-18 15:16:59.756673 aasm-0.1.1/aasm/parsing/op/mparams.py
+-rw-r--r--   0        0        0     5561 2023-07-18 15:21:47.523352 aasm-0.1.1/aasm/parsing/op/prm.py
+-rw-r--r--   0        0        0     2289 2022-12-17 01:24:38.910148 aasm-0.1.1/aasm/parsing/op/rand.py
+-rw-r--r--   0        0        0      748 2022-12-17 01:24:38.910148 aasm-0.1.1/aasm/parsing/op/remen.py
+-rw-r--r--   0        0        0      620 2022-12-17 01:24:38.910148 aasm-0.1.1/aasm/parsing/op/round.py
+-rw-r--r--   0        0        0      606 2022-12-17 05:36:13.052938 aasm-0.1.1/aasm/parsing/op/scale.py
+-rw-r--r--   0        0        0      880 2022-12-17 01:24:38.910148 aasm-0.1.1/aasm/parsing/op/send.py
+-rw-r--r--   0        0        0      690 2023-07-18 15:21:47.523352 aasm-0.1.1/aasm/parsing/op/set.py
+-rw-r--r--   0        0        0      603 2022-12-17 01:24:38.910148 aasm-0.1.1/aasm/parsing/op/size.py
+-rw-r--r--   0        0        0      803 2022-12-17 01:24:38.910148 aasm-0.1.1/aasm/parsing/op/subs.py
+-rw-r--r--   0        0        0      893 2023-07-18 15:16:59.756673 aasm-0.1.1/aasm/parsing/op/types.py
+-rw-r--r--   0        0        0     6593 2023-07-18 15:16:59.756673 aasm-0.1.1/aasm/parsing/parse.py
+-rw-r--r--   0        0        0     5804 2023-07-18 15:16:59.756673 aasm-0.1.1/aasm/parsing/state.py
+-rw-r--r--   0        0        0        0 2022-12-17 01:24:38.913482 aasm-0.1.1/aasm/preprocessor/__init__.py
+-rw-r--r--   0        0        0      839 2022-12-17 01:24:38.913482 aasm-0.1.1/aasm/preprocessor/constant.py
+-rw-r--r--   0        0        0     1484 2022-12-17 01:24:38.913482 aasm-0.1.1/aasm/preprocessor/macro.py
+-rw-r--r--   0        0        0     7930 2022-12-17 05:36:13.056271 aasm-0.1.1/aasm/preprocessor/preprocessor.py
+-rw-r--r--   0        0        0      292 2022-12-17 01:24:38.913482 aasm-0.1.1/aasm/preprocessor/preprocessor_item.py
+-rw-r--r--   0        0        0     2312 2023-07-20 12:15:22.313373 aasm-0.1.1/aasm/translate.py
+-rw-r--r--   0        0        0        0 2022-12-17 01:24:38.913482 aasm-0.1.1/aasm/utils/__init__.py
+-rw-r--r--   0        0        0      428 2022-12-17 01:24:38.913482 aasm-0.1.1/aasm/utils/exception.py
+-rw-r--r--   0        0        0      412 2022-12-17 01:24:38.913482 aasm-0.1.1/aasm/utils/iteration.py
+-rw-r--r--   0        0        0     2074 2023-07-19 14:27:17.546723 aasm-0.1.1/aasm/utils/validation.py
+-rw-r--r--   0        0        0      673 2023-05-22 10:07:10.256947 aasm-0.1.1/examples/EXAMPLES.md
+-rw-r--r--   0        0        0      837 2023-07-18 15:16:59.756673 aasm-0.1.1/examples/basic/facebook.aasm
+-rw-r--r--   0        0        0      968 2023-07-18 15:16:59.756673 aasm-0.1.1/examples/basic/facebook_macro.aasm
+-rw-r--r--   0        0        0    14394 2023-07-18 15:16:59.756673 aasm-0.1.1/examples/basic/wolfsheep.aasm
+-rw-r--r--   0        0        0    11149 2023-07-18 15:16:59.760006 aasm-0.1.1/examples/basic/wolfsheep_macro.aasm
+-rw-r--r--   0        0        0     1115 2023-07-19 14:25:12.646717 aasm-0.1.1/examples/graphs/barabasi-albert.aasm
+-rw-r--r--   0        0        0     1152 2023-07-18 15:16:59.760006 aasm-0.1.1/examples/graphs/inhomogenous.aasm
+-rw-r--r--   0        0        0     1179 2023-07-18 15:16:59.760006 aasm-0.1.1/examples/graphs/matrix.aasm
+-rw-r--r--   0        0        0     1129 2023-07-19 14:25:12.646717 aasm-0.1.1/examples/graphs/statistical.aasm
+-rw-r--r--   0        0        0     1153 2023-07-18 15:16:59.760006 aasm-0.1.1/examples/modules/facebook_uuid.aasm
+-rw-r--r--   0        0        0      660 2023-07-29 14:38:58.976935 aasm-0.1.1/examples/modules/uuid.aasm.mod
+-rw-r--r--   0        0        0      499 2022-12-17 01:24:38.913482 aasm-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3495 1970-01-01 00:00:00.000000 aasm-0.1.1/PKG-INFO
```

### Comparing `aasm-0.1.0/CONTRIBUTING.md` & `aasm-0.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/DOCS.md` & `aasm-0.1.1/DOCS.md`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/LICENSE.md` & `aasm-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/Pipfile.lock` & `aasm-0.1.1/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/README.md` & `aasm-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/generating/code.py` & `aasm-0.1.1/aasm/generating/code.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/generating/python_code.py` & `aasm-0.1.1/aasm/generating/python_code.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/generating/python_graph.py` & `aasm-0.1.1/aasm/generating/python_graph.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/generating/python_module.py` & `aasm-0.1.1/aasm/generating/python_module.py`

 * *Files 18% similar despite different names*

```diff
@@ -50,10 +50,12 @@
         except KeyError:
             return
 
     def create_module_implementations(self):
         for impl in self.module.impls:
             if impl[0] == self.target:
                 self.add_line(f"def {impl[1]}():")
+                self.indent_right()
                 for line in self.module.impls[impl]:
                     self.add_line(line)
+                self.indent_left()
                 self.add_newline()
```

### Comparing `aasm-0.1.0/aasm/generating/python_spade.py` & `aasm-0.1.1/aasm/generating/python_spade.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,32 +134,27 @@
 
 class PythonSpadeCode(PythonCode):
     def __init__(self, indent_size: int, agents: List[Agent], modules: List[Module]):
         super().__init__(indent_size)
         self.modules = modules
         self.target = "spade"
         self.filter_modules()
-        self.add_module_imports()
         for agent in agents:
             self.add_newlines(2)
             self.generate_agent(agent)
             self.add_required_imports()
 
     def filter_modules(self):
         self.modules = [
             target_mod
             for target_mod in self.modules
             for target in target_mod.targets
             if target.name == self.target
         ]
 
-    def add_module_imports(self):
-        for module in self.modules:
-            self.add_line(f"import {module.name}")
-
     #    spade_modules = []
     #    for target_mod in self.modules:
     #        for target in target_mod.targets:
     #            if target.name == self.target:
     #                spade_modules.append(target_mod)
     #    self.modules = spade_modules
```

### Comparing `aasm-0.1.0/aasm/intermediate/action.py` & `aasm-0.1.1/aasm/intermediate/action.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/intermediate/agent.py` & `aasm-0.1.1/aasm/intermediate/agent.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/intermediate/argument.py` & `aasm-0.1.1/aasm/intermediate/argument.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/intermediate/behaviour.py` & `aasm-0.1.1/aasm/intermediate/behaviour.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/intermediate/block.py` & `aasm-0.1.1/aasm/intermediate/block.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/intermediate/declaration.py` & `aasm-0.1.1/aasm/intermediate/declaration.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/intermediate/graph.py` & `aasm-0.1.1/aasm/intermediate/graph.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/intermediate/instruction.py` & `aasm-0.1.1/aasm/intermediate/instruction.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/intermediate/message.py` & `aasm-0.1.1/aasm/intermediate/message.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/modules/instruction.py` & `aasm-0.1.1/aasm/modules/instruction.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/modules/module.py` & `aasm-0.1.1/aasm/modules/module.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/parsing/op/action.py` & `aasm-0.1.1/aasm/parsing/op/action.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/parsing/op/agent.py` & `aasm-0.1.1/aasm/parsing/op/agent.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/parsing/op/behav.py` & `aasm-0.1.1/aasm/parsing/op/behav.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/parsing/op/clr.py` & `aasm-0.1.1/aasm/parsing/op/clr.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/parsing/op/conditional.py` & `aasm-0.1.1/aasm/parsing/op/conditional.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/parsing/op/decl.py` & `aasm-0.1.1/aasm/parsing/op/decl.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/parsing/op/defg.py` & `aasm-0.1.1/aasm/parsing/op/defg.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/parsing/op/defnode.py` & `aasm-0.1.1/aasm/parsing/op/defnode.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/parsing/op/deftype.py` & `aasm-0.1.1/aasm/parsing/op/deftype.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/parsing/op/graph.py` & `aasm-0.1.1/aasm/parsing/op/graph.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/parsing/op/len.py` & `aasm-0.1.1/aasm/parsing/op/len.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/parsing/op/list_inclusion.py` & `aasm-0.1.1/aasm/parsing/op/list_inclusion.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/parsing/op/list_modification.py` & `aasm-0.1.1/aasm/parsing/op/list_modification.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/parsing/op/logs.py` & `aasm-0.1.1/aasm/parsing/op/logs.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/parsing/op/lr.py` & `aasm-0.1.1/aasm/parsing/op/lr.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/parsing/op/lw.py` & `aasm-0.1.1/aasm/parsing/op/lw.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/parsing/op/math.py` & `aasm-0.1.1/aasm/parsing/op/math.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/parsing/op/math_exp.py` & `aasm-0.1.1/aasm/parsing/op/math_exp.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/parsing/op/math_mod.py` & `aasm-0.1.1/aasm/parsing/op/math_mod.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/parsing/op/message.py` & `aasm-0.1.1/aasm/parsing/op/message.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/parsing/op/module.py` & `aasm-0.1.1/aasm/parsing/op/module.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/parsing/op/mparams.py` & `aasm-0.1.1/aasm/parsing/op/mparams.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/parsing/op/prm.py` & `aasm-0.1.1/aasm/parsing/op/prm.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/parsing/op/rand.py` & `aasm-0.1.1/aasm/parsing/op/rand.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/parsing/op/remen.py` & `aasm-0.1.1/aasm/parsing/op/remen.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/parsing/op/round.py` & `aasm-0.1.1/aasm/parsing/op/round.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/parsing/op/scale.py` & `aasm-0.1.1/aasm/parsing/op/scale.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/parsing/op/send.py` & `aasm-0.1.1/aasm/parsing/op/send.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/parsing/op/set.py` & `aasm-0.1.1/aasm/parsing/op/set.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/parsing/op/size.py` & `aasm-0.1.1/aasm/parsing/op/size.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/parsing/op/subs.py` & `aasm-0.1.1/aasm/parsing/op/subs.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/parsing/op/types.py` & `aasm-0.1.1/aasm/parsing/op/types.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/parsing/parse.py` & `aasm-0.1.1/aasm/parsing/parse.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/parsing/state.py` & `aasm-0.1.1/aasm/parsing/state.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/preprocessor/constant.py` & `aasm-0.1.1/aasm/preprocessor/constant.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/preprocessor/macro.py` & `aasm-0.1.1/aasm/preprocessor/macro.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/preprocessor/preprocessor.py` & `aasm-0.1.1/aasm/preprocessor/preprocessor.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/translate.py` & `aasm-0.1.1/aasm/translate.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/aasm/utils/validation.py` & `aasm-0.1.1/aasm/utils/validation.py`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/examples/EXAMPLES.md` & `aasm-0.1.1/examples/EXAMPLES.md`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/examples/basic/facebook.aasm` & `aasm-0.1.1/examples/basic/facebook.aasm`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/examples/basic/facebook_macro.aasm` & `aasm-0.1.1/examples/basic/facebook_macro.aasm`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/examples/basic/wolfsheep.aasm` & `aasm-0.1.1/examples/basic/wolfsheep.aasm`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/examples/basic/wolfsheep_macro.aasm` & `aasm-0.1.1/examples/basic/wolfsheep_macro.aasm`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/examples/graphs/barabasi-albert.aasm` & `aasm-0.1.1/examples/graphs/barabasi-albert.aasm`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/examples/graphs/inhomogenous.aasm` & `aasm-0.1.1/examples/graphs/inhomogenous.aasm`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/examples/graphs/matrix.aasm` & `aasm-0.1.1/examples/graphs/matrix.aasm`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/examples/graphs/statistical.aasm` & `aasm-0.1.1/examples/graphs/statistical.aasm`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/examples/modules/facebook_uuid.aasm` & `aasm-0.1.1/examples/modules/facebook_uuid.aasm`

 * *Files identical despite different names*

### Comparing `aasm-0.1.0/examples/modules/uuid.aasm.mod` & `aasm-0.1.1/examples/modules/uuid.aasm.mod`

 * *Files 3% similar despite different names*

```diff
@@ -21,18 +21,18 @@
 ISEQ* a: uuid, b: uuid
 ISNEQ* a: uuid, b: uuid
 
 !preamble spade
 import uuid
 
 !impl GETUUID spade
-a = str(uuid.uuid4())
+return a = str(uuid.uuid4())
 
 !impl ISEQ spade
 if a == b:
-  return True
+    return True
 return False
 
 !impl ISNEQ spade
 if a != b:
-  return True
+    return True
 return False
```

### Comparing `aasm-0.1.0/PKG-INFO` & `aasm-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aasm
-Version: 0.1.0
+Version: 0.1.1
 Summary: Agents Assembly translator
 Keywords: aasm,agents assembly,agents,translator,dsl,domain specific language,simulations
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Project-URL: Documentation, https://agents-assembly.com/docs
 Project-URL: Source, https://github.com/agent-based-information-flow-simulation/agents-assembly-translator
```

