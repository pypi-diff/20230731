# Comparing `tmp/teneva_bm-0.6.2.tar.gz` & `tmp/teneva_bm-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teneva_bm-0.6.2.tar", last modified: Sun Jul 30 19:13:54 2023, max compression
+gzip compressed data, was "teneva_bm-0.6.3.tar", last modified: Sun Jul 30 20:26:42 2023, max compression
```

## Comparing `teneva_bm-0.6.2.tar` & `teneva_bm-0.6.3.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-30 19:13:54.653960 teneva_bm-0.6.2/
--rw-r--r--   0 andrei     (501) staff       (20)     1090 2023-02-25 19:29:59.000000 teneva_bm-0.6.2/LICENSE.txt
--rw-r--r--   0 andrei     (501) staff       (20)       79 2023-07-27 07:17:23.000000 teneva_bm-0.6.2/MANIFEST.in
--rw-r--r--   0 andrei     (501) staff       (20)    19920 2023-07-30 19:13:54.654301 teneva_bm-0.6.2/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)    18659 2023-07-30 19:13:43.000000 teneva_bm-0.6.2/README.md
--rw-r--r--   0 andrei     (501) staff       (20)      899 2023-07-29 14:29:03.000000 teneva_bm-0.6.2/demo.py
--rw-r--r--   0 andrei     (501) staff       (20)       33 2023-07-29 13:15:53.000000 teneva_bm-0.6.2/requirements.txt
--rw-r--r--   0 andrei     (501) staff       (20)      107 2023-07-30 19:13:54.655551 teneva_bm-0.6.2/setup.cfg
--rw-r--r--   0 andrei     (501) staff       (20)     2518 2023-07-16 14:04:06.000000 teneva_bm-0.6.2/setup.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-30 19:13:54.617971 teneva_bm-0.6.2/teneva_bm/
--rw-r--r--   0 andrei     (501) staff       (20)      211 2023-07-30 19:13:38.000000 teneva_bm-0.6.2/teneva_bm/__init__.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-30 19:13:54.626872 teneva_bm-0.6.2/teneva_bm/agent/
--rw-r--r--   0 andrei     (501) staff       (20)      319 2023-07-30 16:47:21.000000 teneva_bm-0.6.2/teneva_bm/agent/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     7572 2023-07-30 19:13:15.000000 teneva_bm-0.6.2/teneva_bm/agent/agent.py
--rw-r--r--   0 andrei     (501) staff       (20)     2076 2023-07-30 16:06:42.000000 teneva_bm-0.6.2/teneva_bm/agent/bm_agent_ant.py
--rw-r--r--   0 andrei     (501) staff       (20)     2092 2023-07-30 15:54:04.000000 teneva_bm-0.6.2/teneva_bm/agent/bm_agent_human.py
--rw-r--r--   0 andrei     (501) staff       (20)     2139 2023-07-30 15:53:56.000000 teneva_bm-0.6.2/teneva_bm/agent/bm_agent_human_stand.py
--rw-r--r--   0 andrei     (501) staff       (20)     6617 2023-07-30 18:20:22.000000 teneva_bm-0.6.2/teneva_bm/agent/bm_agent_lake.py
--rw-r--r--   0 andrei     (501) staff       (20)     2136 2023-07-30 16:47:47.000000 teneva_bm-0.6.2/teneva_bm/agent/bm_agent_pend_inv.py
--rw-r--r--   0 andrei     (501) staff       (20)     2185 2023-07-30 16:47:42.000000 teneva_bm-0.6.2/teneva_bm/agent/bm_agent_pend_inv_double.py
--rw-r--r--   0 andrei     (501) staff       (20)     2288 2023-07-30 15:24:14.000000 teneva_bm-0.6.2/teneva_bm/agent/bm_agent_swimmer.py
--rw-r--r--   0 andrei     (501) staff       (20)     3323 2023-07-30 15:46:50.000000 teneva_bm-0.6.2/teneva_bm/agent/policy.py
--rw-r--r--   0 andrei     (501) staff       (20)    35039 2023-07-30 14:19:05.000000 teneva_bm-0.6.2/teneva_bm/bm.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-30 19:13:54.634485 teneva_bm-0.6.2/teneva_bm/func/
--rw-r--r--   0 andrei     (501) staff       (20)      516 2023-07-13 07:42:30.000000 teneva_bm-0.6.2/teneva_bm/func/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     3548 2023-07-30 10:47:49.000000 teneva_bm-0.6.2/teneva_bm/func/bm_func_ackley.py
--rw-r--r--   0 andrei     (501) staff       (20)     2301 2023-07-30 10:08:14.000000 teneva_bm-0.6.2/teneva_bm/func/bm_func_alpine.py
--rw-r--r--   0 andrei     (501) staff       (20)     2430 2023-07-30 10:52:13.000000 teneva_bm-0.6.2/teneva_bm/func/bm_func_dixon.py
--rw-r--r--   0 andrei     (501) staff       (20)     2295 2023-07-30 10:52:30.000000 teneva_bm-0.6.2/teneva_bm/func/bm_func_exp.py
--rw-r--r--   0 andrei     (501) staff       (20)     2746 2023-07-30 10:13:15.000000 teneva_bm-0.6.2/teneva_bm/func/bm_func_griewank.py
--rw-r--r--   0 andrei     (501) staff       (20)     3590 2023-07-30 10:53:24.000000 teneva_bm-0.6.2/teneva_bm/func/bm_func_michalewicz.py
--rw-r--r--   0 andrei     (501) staff       (20)     2421 2023-07-30 10:17:40.000000 teneva_bm-0.6.2/teneva_bm/func/bm_func_piston.py
--rw-r--r--   0 andrei     (501) staff       (20)     2478 2023-07-30 10:55:11.000000 teneva_bm-0.6.2/teneva_bm/func/bm_func_qing.py
--rw-r--r--   0 andrei     (501) staff       (20)     3091 2023-07-30 10:19:45.000000 teneva_bm-0.6.2/teneva_bm/func/bm_func_rastrigin.py
--rw-r--r--   0 andrei     (501) staff       (20)     3155 2023-07-30 10:56:44.000000 teneva_bm-0.6.2/teneva_bm/func/bm_func_rosenbrock.py
--rw-r--r--   0 andrei     (501) staff       (20)     2129 2023-07-30 10:56:51.000000 teneva_bm-0.6.2/teneva_bm/func/bm_func_schaffer.py
--rw-r--r--   0 andrei     (501) staff       (20)     3132 2023-07-30 10:22:30.000000 teneva_bm-0.6.2/teneva_bm/func/bm_func_schwefel.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-30 19:13:54.636139 teneva_bm-0.6.2/teneva_bm/hs/
--rw-r--r--   0 andrei     (501) staff       (20)       78 2023-07-17 21:02:17.000000 teneva_bm-0.6.2/teneva_bm/hs/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     1755 2023-07-30 11:13:53.000000 teneva_bm-0.6.2/teneva_bm/hs/bm_hs_func001.py
--rw-r--r--   0 andrei     (501) staff       (20)     2430 2023-07-30 11:26:02.000000 teneva_bm-0.6.2/teneva_bm/hs/bm_hs_func006.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-30 19:13:54.640335 teneva_bm-0.6.2/teneva_bm/hs/draft_constrained_functions/
--rw-r--r--   0 andrei     (501) staff       (20)      209 2023-07-17 20:25:36.000000 teneva_bm-0.6.2/teneva_bm/hs/draft_constrained_functions/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     2272 2023-07-17 20:25:36.000000 teneva_bm-0.6.2/teneva_bm/hs/draft_constrained_functions/bm_hs007.py
--rw-r--r--   0 andrei     (501) staff       (20)     2459 2023-07-17 20:25:36.000000 teneva_bm-0.6.2/teneva_bm/hs/draft_constrained_functions/bm_hs008.py
--rw-r--r--   0 andrei     (501) staff       (20)     2318 2023-07-17 20:25:36.000000 teneva_bm-0.6.2/teneva_bm/hs/draft_constrained_functions/bm_hs009.py
--rw-r--r--   0 andrei     (501) staff       (20)     2266 2023-07-17 20:25:36.000000 teneva_bm-0.6.2/teneva_bm/hs/draft_constrained_functions/bm_hs010.py
--rw-r--r--   0 andrei     (501) staff       (20)     2251 2023-07-17 20:25:36.000000 teneva_bm-0.6.2/teneva_bm/hs/draft_constrained_functions/bm_hs011.py
--rw-r--r--   0 andrei     (501) staff       (20)     2376 2023-07-17 20:25:36.000000 teneva_bm-0.6.2/teneva_bm/hs/draft_constrained_functions/bm_hs012.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-30 19:13:54.644940 teneva_bm-0.6.2/teneva_bm/hs/draft_unconstrained_functions/
--rw-r--r--   0 andrei     (501) staff       (20)      209 2023-07-17 20:25:36.000000 teneva_bm-0.6.2/teneva_bm/hs/draft_unconstrained_functions/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     1937 2023-07-17 20:25:36.000000 teneva_bm-0.6.2/teneva_bm/hs/draft_unconstrained_functions/bm_hs002.py
--rw-r--r--   0 andrei     (501) staff       (20)     1857 2023-07-17 20:25:36.000000 teneva_bm-0.6.2/teneva_bm/hs/draft_unconstrained_functions/bm_hs003.py
--rw-r--r--   0 andrei     (501) staff       (20)     1839 2023-07-17 20:25:36.000000 teneva_bm-0.6.2/teneva_bm/hs/draft_unconstrained_functions/bm_hs004.py
--rw-r--r--   0 andrei     (501) staff       (20)     2197 2023-07-17 20:25:36.000000 teneva_bm-0.6.2/teneva_bm/hs/draft_unconstrained_functions/bm_hs005.py
--rw-r--r--   0 andrei     (501) staff       (20)     2275 2023-07-17 20:25:36.000000 teneva_bm-0.6.2/teneva_bm/hs/draft_unconstrained_functions/bm_hs038.py
--rw-r--r--   0 andrei     (501) staff       (20)     1929 2023-07-17 20:25:36.000000 teneva_bm-0.6.2/teneva_bm/hs/draft_unconstrained_functions/bm_hs045.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-30 19:13:54.647046 teneva_bm-0.6.2/teneva_bm/odeoc/
--rw-r--r--   0 andrei     (501) staff       (20)       99 2023-07-30 11:32:37.000000 teneva_bm-0.6.2/teneva_bm/odeoc/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     4237 2023-07-30 11:37:21.000000 teneva_bm-0.6.2/teneva_bm/odeoc/bm_odeoc_simple.py
--rw-r--r--   0 andrei     (501) staff       (20)     2292 2023-07-30 11:37:44.000000 teneva_bm-0.6.2/teneva_bm/odeoc/bm_odeoc_simple_constr.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-30 19:13:54.650830 teneva_bm-0.6.2/teneva_bm/qubo/
--rw-r--r--   0 andrei     (501) staff       (20)      166 2023-07-22 15:44:37.000000 teneva_bm-0.6.2/teneva_bm/qubo/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     7111 2023-07-30 11:04:30.000000 teneva_bm-0.6.2/teneva_bm/qubo/bm_qubo_knap_det.py
--rw-r--r--   0 andrei     (501) staff       (20)     1834 2023-07-30 11:06:13.000000 teneva_bm-0.6.2/teneva_bm/qubo/bm_qubo_knap_quad.py
--rw-r--r--   0 andrei     (501) staff       (20)     2967 2023-07-30 11:07:28.000000 teneva_bm-0.6.2/teneva_bm/qubo/bm_qubo_maxcut.py
--rw-r--r--   0 andrei     (501) staff       (20)     2973 2023-07-30 11:08:28.000000 teneva_bm-0.6.2/teneva_bm/qubo/bm_qubo_mvc.py
--rw-r--r--   0 andrei     (501) staff       (20)     3377 2023-07-29 14:31:04.000000 teneva_bm-0.6.2/teneva_bm/teneva_bm_demo.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-30 19:13:54.653418 teneva_bm-0.6.2/teneva_bm/various/
--rw-r--r--   0 andrei     (501) staff       (20)      105 2023-07-13 07:41:21.000000 teneva_bm-0.6.2/teneva_bm/various/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     7790 2023-07-30 11:28:44.000000 teneva_bm-0.6.2/teneva_bm/various/bm_matmul.py
--rw-r--r--   0 andrei     (501) staff       (20)    12645 2023-07-30 11:24:08.000000 teneva_bm-0.6.2/teneva_bm/various/bm_topopt.py
--rw-r--r--   0 andrei     (501) staff       (20)     1867 2023-07-30 11:18:40.000000 teneva_bm-0.6.2/teneva_bm/various/bm_wall_simple.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-30 19:13:54.620983 teneva_bm-0.6.2/teneva_bm.egg-info/
--rw-r--r--   0 andrei     (501) staff       (20)    19920 2023-07-30 19:13:54.000000 teneva_bm-0.6.2/teneva_bm.egg-info/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)     2312 2023-07-30 19:13:54.000000 teneva_bm-0.6.2/teneva_bm.egg-info/SOURCES.txt
--rw-r--r--   0 andrei     (501) staff       (20)        1 2023-07-30 19:13:54.000000 teneva_bm-0.6.2/teneva_bm.egg-info/dependency_links.txt
--rw-r--r--   0 andrei     (501) staff       (20)       33 2023-07-30 19:13:54.000000 teneva_bm-0.6.2/teneva_bm.egg-info/requires.txt
--rw-r--r--   0 andrei     (501) staff       (20)       10 2023-07-30 19:13:54.000000 teneva_bm-0.6.2/teneva_bm.egg-info/top_level.txt
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-30 20:26:42.397567 teneva_bm-0.6.3/
+-rw-r--r--   0 andrei     (501) staff       (20)     1090 2023-02-25 19:29:59.000000 teneva_bm-0.6.3/LICENSE.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       79 2023-07-27 07:17:23.000000 teneva_bm-0.6.3/MANIFEST.in
+-rw-r--r--   0 andrei     (501) staff       (20)    19920 2023-07-30 20:26:42.397994 teneva_bm-0.6.3/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)    18659 2023-07-30 20:26:25.000000 teneva_bm-0.6.3/README.md
+-rw-r--r--   0 andrei     (501) staff       (20)      899 2023-07-29 14:29:03.000000 teneva_bm-0.6.3/demo.py
+-rw-r--r--   0 andrei     (501) staff       (20)       33 2023-07-29 13:15:53.000000 teneva_bm-0.6.3/requirements.txt
+-rw-r--r--   0 andrei     (501) staff       (20)      107 2023-07-30 20:26:42.399182 teneva_bm-0.6.3/setup.cfg
+-rw-r--r--   0 andrei     (501) staff       (20)     2518 2023-07-16 14:04:06.000000 teneva_bm-0.6.3/setup.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-30 20:26:42.343594 teneva_bm-0.6.3/teneva_bm/
+-rw-r--r--   0 andrei     (501) staff       (20)      211 2023-07-30 20:26:21.000000 teneva_bm-0.6.3/teneva_bm/__init__.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-30 20:26:42.354104 teneva_bm-0.6.3/teneva_bm/agent/
+-rw-r--r--   0 andrei     (501) staff       (20)      319 2023-07-30 16:47:21.000000 teneva_bm-0.6.3/teneva_bm/agent/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     7572 2023-07-30 19:13:15.000000 teneva_bm-0.6.3/teneva_bm/agent/agent.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2076 2023-07-30 16:06:42.000000 teneva_bm-0.6.3/teneva_bm/agent/bm_agent_ant.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2092 2023-07-30 15:54:04.000000 teneva_bm-0.6.3/teneva_bm/agent/bm_agent_human.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2139 2023-07-30 15:53:56.000000 teneva_bm-0.6.3/teneva_bm/agent/bm_agent_human_stand.py
+-rw-r--r--   0 andrei     (501) staff       (20)     6926 2023-07-30 19:52:28.000000 teneva_bm-0.6.3/teneva_bm/agent/bm_agent_lake.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2136 2023-07-30 16:47:47.000000 teneva_bm-0.6.3/teneva_bm/agent/bm_agent_pend_inv.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2185 2023-07-30 16:47:42.000000 teneva_bm-0.6.3/teneva_bm/agent/bm_agent_pend_inv_double.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2288 2023-07-30 15:24:14.000000 teneva_bm-0.6.3/teneva_bm/agent/bm_agent_swimmer.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3323 2023-07-30 15:46:50.000000 teneva_bm-0.6.3/teneva_bm/agent/policy.py
+-rw-r--r--   0 andrei     (501) staff       (20)    35039 2023-07-30 14:19:05.000000 teneva_bm-0.6.3/teneva_bm/bm.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-30 20:26:42.365755 teneva_bm-0.6.3/teneva_bm/func/
+-rw-r--r--   0 andrei     (501) staff       (20)      516 2023-07-13 07:42:30.000000 teneva_bm-0.6.3/teneva_bm/func/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3548 2023-07-30 10:47:49.000000 teneva_bm-0.6.3/teneva_bm/func/bm_func_ackley.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2301 2023-07-30 10:08:14.000000 teneva_bm-0.6.3/teneva_bm/func/bm_func_alpine.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2430 2023-07-30 10:52:13.000000 teneva_bm-0.6.3/teneva_bm/func/bm_func_dixon.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2295 2023-07-30 10:52:30.000000 teneva_bm-0.6.3/teneva_bm/func/bm_func_exp.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2746 2023-07-30 10:13:15.000000 teneva_bm-0.6.3/teneva_bm/func/bm_func_griewank.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3590 2023-07-30 10:53:24.000000 teneva_bm-0.6.3/teneva_bm/func/bm_func_michalewicz.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2421 2023-07-30 10:17:40.000000 teneva_bm-0.6.3/teneva_bm/func/bm_func_piston.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2478 2023-07-30 10:55:11.000000 teneva_bm-0.6.3/teneva_bm/func/bm_func_qing.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3091 2023-07-30 10:19:45.000000 teneva_bm-0.6.3/teneva_bm/func/bm_func_rastrigin.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3155 2023-07-30 10:56:44.000000 teneva_bm-0.6.3/teneva_bm/func/bm_func_rosenbrock.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2129 2023-07-30 10:56:51.000000 teneva_bm-0.6.3/teneva_bm/func/bm_func_schaffer.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3132 2023-07-30 10:22:30.000000 teneva_bm-0.6.3/teneva_bm/func/bm_func_schwefel.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-30 20:26:42.368597 teneva_bm-0.6.3/teneva_bm/hs/
+-rw-r--r--   0 andrei     (501) staff       (20)       78 2023-07-17 21:02:17.000000 teneva_bm-0.6.3/teneva_bm/hs/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1755 2023-07-30 11:13:53.000000 teneva_bm-0.6.3/teneva_bm/hs/bm_hs_func001.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2430 2023-07-30 11:26:02.000000 teneva_bm-0.6.3/teneva_bm/hs/bm_hs_func006.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-30 20:26:42.377515 teneva_bm-0.6.3/teneva_bm/hs/draft_constrained_functions/
+-rw-r--r--   0 andrei     (501) staff       (20)      209 2023-07-17 20:25:36.000000 teneva_bm-0.6.3/teneva_bm/hs/draft_constrained_functions/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2272 2023-07-17 20:25:36.000000 teneva_bm-0.6.3/teneva_bm/hs/draft_constrained_functions/bm_hs007.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2459 2023-07-17 20:25:36.000000 teneva_bm-0.6.3/teneva_bm/hs/draft_constrained_functions/bm_hs008.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2318 2023-07-17 20:25:36.000000 teneva_bm-0.6.3/teneva_bm/hs/draft_constrained_functions/bm_hs009.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2266 2023-07-17 20:25:36.000000 teneva_bm-0.6.3/teneva_bm/hs/draft_constrained_functions/bm_hs010.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2251 2023-07-17 20:25:36.000000 teneva_bm-0.6.3/teneva_bm/hs/draft_constrained_functions/bm_hs011.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2376 2023-07-17 20:25:36.000000 teneva_bm-0.6.3/teneva_bm/hs/draft_constrained_functions/bm_hs012.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-30 20:26:42.384335 teneva_bm-0.6.3/teneva_bm/hs/draft_unconstrained_functions/
+-rw-r--r--   0 andrei     (501) staff       (20)      209 2023-07-17 20:25:36.000000 teneva_bm-0.6.3/teneva_bm/hs/draft_unconstrained_functions/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1937 2023-07-17 20:25:36.000000 teneva_bm-0.6.3/teneva_bm/hs/draft_unconstrained_functions/bm_hs002.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1857 2023-07-17 20:25:36.000000 teneva_bm-0.6.3/teneva_bm/hs/draft_unconstrained_functions/bm_hs003.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1839 2023-07-17 20:25:36.000000 teneva_bm-0.6.3/teneva_bm/hs/draft_unconstrained_functions/bm_hs004.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2197 2023-07-17 20:25:36.000000 teneva_bm-0.6.3/teneva_bm/hs/draft_unconstrained_functions/bm_hs005.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2275 2023-07-17 20:25:36.000000 teneva_bm-0.6.3/teneva_bm/hs/draft_unconstrained_functions/bm_hs038.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1929 2023-07-17 20:25:36.000000 teneva_bm-0.6.3/teneva_bm/hs/draft_unconstrained_functions/bm_hs045.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-30 20:26:42.387393 teneva_bm-0.6.3/teneva_bm/odeoc/
+-rw-r--r--   0 andrei     (501) staff       (20)       99 2023-07-30 11:32:37.000000 teneva_bm-0.6.3/teneva_bm/odeoc/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     4237 2023-07-30 11:37:21.000000 teneva_bm-0.6.3/teneva_bm/odeoc/bm_odeoc_simple.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2292 2023-07-30 11:37:44.000000 teneva_bm-0.6.3/teneva_bm/odeoc/bm_odeoc_simple_constr.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-30 20:26:42.392368 teneva_bm-0.6.3/teneva_bm/qubo/
+-rw-r--r--   0 andrei     (501) staff       (20)      166 2023-07-22 15:44:37.000000 teneva_bm-0.6.3/teneva_bm/qubo/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     7111 2023-07-30 11:04:30.000000 teneva_bm-0.6.3/teneva_bm/qubo/bm_qubo_knap_det.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1834 2023-07-30 11:06:13.000000 teneva_bm-0.6.3/teneva_bm/qubo/bm_qubo_knap_quad.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2967 2023-07-30 11:07:28.000000 teneva_bm-0.6.3/teneva_bm/qubo/bm_qubo_maxcut.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2973 2023-07-30 11:08:28.000000 teneva_bm-0.6.3/teneva_bm/qubo/bm_qubo_mvc.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3377 2023-07-29 14:31:04.000000 teneva_bm-0.6.3/teneva_bm/teneva_bm_demo.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-30 20:26:42.396711 teneva_bm-0.6.3/teneva_bm/various/
+-rw-r--r--   0 andrei     (501) staff       (20)      105 2023-07-13 07:41:21.000000 teneva_bm-0.6.3/teneva_bm/various/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     7790 2023-07-30 11:28:44.000000 teneva_bm-0.6.3/teneva_bm/various/bm_matmul.py
+-rw-r--r--   0 andrei     (501) staff       (20)    12645 2023-07-30 11:24:08.000000 teneva_bm-0.6.3/teneva_bm/various/bm_topopt.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1867 2023-07-30 11:18:40.000000 teneva_bm-0.6.3/teneva_bm/various/bm_wall_simple.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-30 20:26:42.346565 teneva_bm-0.6.3/teneva_bm.egg-info/
+-rw-r--r--   0 andrei     (501) staff       (20)    19920 2023-07-30 20:26:42.000000 teneva_bm-0.6.3/teneva_bm.egg-info/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)     2312 2023-07-30 20:26:42.000000 teneva_bm-0.6.3/teneva_bm.egg-info/SOURCES.txt
+-rw-r--r--   0 andrei     (501) staff       (20)        1 2023-07-30 20:26:42.000000 teneva_bm-0.6.3/teneva_bm.egg-info/dependency_links.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       33 2023-07-30 20:26:42.000000 teneva_bm-0.6.3/teneva_bm.egg-info/requires.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       10 2023-07-30 20:26:42.000000 teneva_bm-0.6.3/teneva_bm.egg-info/top_level.txt
```

### Comparing `teneva_bm-0.6.2/LICENSE.txt` & `teneva_bm-0.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/PKG-INFO` & `teneva_bm-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teneva_bm
-Version: 0.6.2
+Version: 0.6.3
 Summary: Benchmarks library, based on the software product teneva, for testing multivariate approximation and optimization methods
 Home-page: https://github.com/AndreiChertkov/teneva_bm
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AndreiChertkov/teneva_bm
 Keywords: benchmarks approximation optimization multidimensional array multivariate function low-rank representation tensor train format TT-decomposition
@@ -30,15 +30,15 @@
 ## Description
 
 Benchmarks library, based on the software product [teneva](https://github.com/AndreiChertkov/teneva), for testing multidimensional approximation and optimization methods. Our benchmarks include both multidimensional data arrays and discretized functions of many variables.
 
 
 ## Installation
 
-> Current version "0.6.2".
+> Current version "0.6.3".
 
 The package can be installed via pip: `pip install teneva_bm` (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9). It can be also downloaded from the repository [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) and installed by `python setup.py install` command from the root folder of the project.
 
 > Required python packages (see `requirements.txt`) [matplotlib](https://matplotlib.org/) (3.7.0+) and [teneva](https://github.com/AndreiChertkov/teneva) (0.14.5+) will be automatically installed during the installation of the main software product.
 
 Some benchmarks require additional installation of specialized libraries. The corresponding instructions are given in the description of each benchmark (see `DESC` string in the python files with benchmarks). Installation of all required libraries for all benchmarks can be done with the following commands:
```

### Comparing `teneva_bm-0.6.2/README.md` & `teneva_bm-0.6.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ## Description
 
 Benchmarks library, based on the software product [teneva](https://github.com/AndreiChertkov/teneva), for testing multidimensional approximation and optimization methods. Our benchmarks include both multidimensional data arrays and discretized functions of many variables.
 
 
 ## Installation
 
-> Current version "0.6.2".
+> Current version "0.6.3".
 
 The package can be installed via pip: `pip install teneva_bm` (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9). It can be also downloaded from the repository [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) and installed by `python setup.py install` command from the root folder of the project.
 
 > Required python packages (see `requirements.txt`) [matplotlib](https://matplotlib.org/) (3.7.0+) and [teneva](https://github.com/AndreiChertkov/teneva) (0.14.5+) will be automatically installed during the installation of the main software product.
 
 Some benchmarks require additional installation of specialized libraries. The corresponding instructions are given in the description of each benchmark (see `DESC` string in the python files with benchmarks). Installation of all required libraries for all benchmarks can be done with the following commands:
```

### Comparing `teneva_bm-0.6.2/demo.py` & `teneva_bm-0.6.3/demo.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/setup.py` & `teneva_bm-0.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/agent/agent.py` & `teneva_bm-0.6.3/teneva_bm/agent/agent.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/agent/bm_agent_ant.py` & `teneva_bm-0.6.3/teneva_bm/agent/bm_agent_ant.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/agent/bm_agent_human.py` & `teneva_bm-0.6.3/teneva_bm/agent/bm_agent_human.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/agent/bm_agent_human_stand.py` & `teneva_bm-0.6.3/teneva_bm/agent/bm_agent_human_stand.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/agent/bm_agent_lake.py` & `teneva_bm-0.6.3/teneva_bm/agent/bm_agent_lake.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,22 +28,29 @@
         holes = []
         for i in range(size):
             for j in range(size):
                 if map[i][j] == BmAgentLake.HOLE:
                     holes.append(np.array([i, j], dtype=int))
         return holes
 
-    def map(size=5, prob_hole=0.4, seed=42):
+    def map(size=5, prob_hole=0.4, seed=42, iters=1.E+9):
         map = []
         rand = np.random.default_rng(seed) if isinstance(seed, int) else seed
+        iter = 0
         while len(map) == 0 or not Agent.frozen_lake.is_valid(map, size):
+            iter += 1
+            if iter > iters:
+                msg = 'Can not build the map for selected probability'
+                raise ValueError(msg)
+
             map = rand.choice([BmAgentLake.FROZ, BmAgentLake.HOLE],
                 (size, size), p=[1-prob_hole, prob_hole])
             map[0, 0] = BmAgentLake.INIT
             map[-1, -1] = BmAgentLake.GOAL
+
         return [''.join(x) for x in map]
 
     def __init__(self, d=None, n=4, name='AgentLake', desc=DESC,
                  steps=100, policy='direct',
                  size=5, prob_hole=0.4, with_state_ext=False):
         super().__init__(d, n, name, desc, steps, policy)
 
@@ -148,14 +155,18 @@
         v = self._size
         text += f'{v}x{v}\n'
 
         text += 'Probability of the hole                  : '
         v = self._prob_hole
         text += f'{v}\n'
 
+        text += 'Number of holes                          : '
+        v = len(self._holes)
+        text += f'{v}\n'
+
         text += 'State is extended                        : '
         v = 'YES' if self._with_state_ext else 'no'
         text += f'{v}\n'
 
         return super().info(text+footer)
 
     def prep_bm(self, policy=None):
```

### Comparing `teneva_bm-0.6.2/teneva_bm/agent/bm_agent_pend_inv.py` & `teneva_bm-0.6.3/teneva_bm/agent/bm_agent_pend_inv.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/agent/bm_agent_pend_inv_double.py` & `teneva_bm-0.6.3/teneva_bm/agent/bm_agent_pend_inv_double.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/agent/bm_agent_swimmer.py` & `teneva_bm-0.6.3/teneva_bm/agent/bm_agent_swimmer.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/agent/policy.py` & `teneva_bm-0.6.3/teneva_bm/agent/policy.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/bm.py` & `teneva_bm-0.6.3/teneva_bm/bm.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/func/__init__.py` & `teneva_bm-0.6.3/teneva_bm/func/__init__.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/func/bm_func_ackley.py` & `teneva_bm-0.6.3/teneva_bm/func/bm_func_ackley.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/func/bm_func_alpine.py` & `teneva_bm-0.6.3/teneva_bm/func/bm_func_alpine.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/func/bm_func_dixon.py` & `teneva_bm-0.6.3/teneva_bm/func/bm_func_dixon.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/func/bm_func_exp.py` & `teneva_bm-0.6.3/teneva_bm/func/bm_func_exp.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/func/bm_func_griewank.py` & `teneva_bm-0.6.3/teneva_bm/func/bm_func_griewank.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/func/bm_func_michalewicz.py` & `teneva_bm-0.6.3/teneva_bm/func/bm_func_michalewicz.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/func/bm_func_piston.py` & `teneva_bm-0.6.3/teneva_bm/func/bm_func_piston.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/func/bm_func_qing.py` & `teneva_bm-0.6.3/teneva_bm/func/bm_func_qing.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/func/bm_func_rastrigin.py` & `teneva_bm-0.6.3/teneva_bm/func/bm_func_rastrigin.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/func/bm_func_rosenbrock.py` & `teneva_bm-0.6.3/teneva_bm/func/bm_func_rosenbrock.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/func/bm_func_schaffer.py` & `teneva_bm-0.6.3/teneva_bm/func/bm_func_schaffer.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/func/bm_func_schwefel.py` & `teneva_bm-0.6.3/teneva_bm/func/bm_func_schwefel.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/hs/bm_hs_func001.py` & `teneva_bm-0.6.3/teneva_bm/hs/bm_hs_func001.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/hs/bm_hs_func006.py` & `teneva_bm-0.6.3/teneva_bm/hs/bm_hs_func006.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/hs/draft_constrained_functions/bm_hs007.py` & `teneva_bm-0.6.3/teneva_bm/hs/draft_constrained_functions/bm_hs007.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/hs/draft_constrained_functions/bm_hs008.py` & `teneva_bm-0.6.3/teneva_bm/hs/draft_constrained_functions/bm_hs008.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/hs/draft_constrained_functions/bm_hs009.py` & `teneva_bm-0.6.3/teneva_bm/hs/draft_constrained_functions/bm_hs009.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/hs/draft_constrained_functions/bm_hs010.py` & `teneva_bm-0.6.3/teneva_bm/hs/draft_constrained_functions/bm_hs010.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/hs/draft_constrained_functions/bm_hs011.py` & `teneva_bm-0.6.3/teneva_bm/hs/draft_constrained_functions/bm_hs011.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/hs/draft_constrained_functions/bm_hs012.py` & `teneva_bm-0.6.3/teneva_bm/hs/draft_constrained_functions/bm_hs012.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/hs/draft_unconstrained_functions/bm_hs002.py` & `teneva_bm-0.6.3/teneva_bm/hs/draft_unconstrained_functions/bm_hs002.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/hs/draft_unconstrained_functions/bm_hs003.py` & `teneva_bm-0.6.3/teneva_bm/hs/draft_unconstrained_functions/bm_hs003.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/hs/draft_unconstrained_functions/bm_hs004.py` & `teneva_bm-0.6.3/teneva_bm/hs/draft_unconstrained_functions/bm_hs004.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/hs/draft_unconstrained_functions/bm_hs005.py` & `teneva_bm-0.6.3/teneva_bm/hs/draft_unconstrained_functions/bm_hs005.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/hs/draft_unconstrained_functions/bm_hs038.py` & `teneva_bm-0.6.3/teneva_bm/hs/draft_unconstrained_functions/bm_hs038.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/hs/draft_unconstrained_functions/bm_hs045.py` & `teneva_bm-0.6.3/teneva_bm/hs/draft_unconstrained_functions/bm_hs045.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/odeoc/bm_odeoc_simple.py` & `teneva_bm-0.6.3/teneva_bm/odeoc/bm_odeoc_simple.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/odeoc/bm_odeoc_simple_constr.py` & `teneva_bm-0.6.3/teneva_bm/odeoc/bm_odeoc_simple_constr.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/qubo/bm_qubo_knap_det.py` & `teneva_bm-0.6.3/teneva_bm/qubo/bm_qubo_knap_det.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/qubo/bm_qubo_knap_quad.py` & `teneva_bm-0.6.3/teneva_bm/qubo/bm_qubo_knap_quad.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/qubo/bm_qubo_maxcut.py` & `teneva_bm-0.6.3/teneva_bm/qubo/bm_qubo_maxcut.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/qubo/bm_qubo_mvc.py` & `teneva_bm-0.6.3/teneva_bm/qubo/bm_qubo_mvc.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/teneva_bm_demo.py` & `teneva_bm-0.6.3/teneva_bm/teneva_bm_demo.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/various/bm_matmul.py` & `teneva_bm-0.6.3/teneva_bm/various/bm_matmul.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/various/bm_topopt.py` & `teneva_bm-0.6.3/teneva_bm/various/bm_topopt.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm/various/bm_wall_simple.py` & `teneva_bm-0.6.3/teneva_bm/various/bm_wall_simple.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.2/teneva_bm.egg-info/PKG-INFO` & `teneva_bm-0.6.3/teneva_bm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teneva-bm
-Version: 0.6.2
+Version: 0.6.3
 Summary: Benchmarks library, based on the software product teneva, for testing multivariate approximation and optimization methods
 Home-page: https://github.com/AndreiChertkov/teneva_bm
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AndreiChertkov/teneva_bm
 Keywords: benchmarks approximation optimization multidimensional array multivariate function low-rank representation tensor train format TT-decomposition
@@ -30,15 +30,15 @@
 ## Description
 
 Benchmarks library, based on the software product [teneva](https://github.com/AndreiChertkov/teneva), for testing multidimensional approximation and optimization methods. Our benchmarks include both multidimensional data arrays and discretized functions of many variables.
 
 
 ## Installation
 
-> Current version "0.6.2".
+> Current version "0.6.3".
 
 The package can be installed via pip: `pip install teneva_bm` (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9). It can be also downloaded from the repository [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) and installed by `python setup.py install` command from the root folder of the project.
 
 > Required python packages (see `requirements.txt`) [matplotlib](https://matplotlib.org/) (3.7.0+) and [teneva](https://github.com/AndreiChertkov/teneva) (0.14.5+) will be automatically installed during the installation of the main software product.
 
 Some benchmarks require additional installation of specialized libraries. The corresponding instructions are given in the description of each benchmark (see `DESC` string in the python files with benchmarks). Installation of all required libraries for all benchmarks can be done with the following commands:
```

### Comparing `teneva_bm-0.6.2/teneva_bm.egg-info/SOURCES.txt` & `teneva_bm-0.6.3/teneva_bm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

