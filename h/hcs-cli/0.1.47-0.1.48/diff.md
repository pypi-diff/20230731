# Comparing `tmp/hcs-cli-0.1.47.tar.gz` & `tmp/hcs-cli-0.1.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcs-cli-0.1.47.tar", last modified: Wed Jul 26 02:23:36 2023, max compression
+gzip compressed data, was "hcs-cli-0.1.48.tar", last modified: Mon Jul 31 01:12:46 2023, max compression
```

## Comparing `hcs-cli-0.1.47.tar` & `hcs-cli-0.1.48.tar`

### file list

```diff
@@ -1,330 +1,338 @@
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.746806 hcs-cli-0.1.47/
--rw-r--r--   0 nanw       (501) staff       (20)     2824 2023-06-21 18:44:48.000000 hcs-cli-0.1.47/.gitignore
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.541936 hcs-cli-0.1.47/.vscode/
--rw-r--r--   0 nanw       (501) staff       (20)     4099 2023-07-26 01:38:46.000000 hcs-cli-0.1.47/.vscode/launch.json
--rw-r--r--   0 nanw       (501) staff       (20)      391 2023-07-26 01:21:48.000000 hcs-cli-0.1.47/.vscode/settings.json
--rw-r--r--   0 nanw       (501) staff       (20)       98 2023-06-13 19:57:56.000000 hcs-cli-0.1.47/CHANGELOG.md
--rw-r--r--   0 nanw       (501) staff       (20)     5258 2023-06-13 16:45:49.000000 hcs-cli-0.1.47/CODE_OF_CONDUCT.md
--rw-r--r--   0 nanw       (501) staff       (20)     2706 2023-06-13 18:53:18.000000 hcs-cli-0.1.47/CONTRIBUTING_CLA.md
--rw-r--r--   0 nanw       (501) staff       (20)     6095 2023-04-25 23:13:27.000000 hcs-cli-0.1.47/GOVERNANCE.md
--rw-r--r--   0 nanw       (501) staff       (20)    10449 2023-06-13 16:45:49.000000 hcs-cli-0.1.47/LICENSE
--rw-r--r--   0 nanw       (501) staff       (20)      881 2023-07-11 00:05:40.000000 hcs-cli-0.1.47/Makefile
--rw-r--r--   0 nanw       (501) staff       (20)      411 2023-06-13 16:45:49.000000 hcs-cli-0.1.47/NOTICE
--rw-r--r--   0 nanw       (501) staff       (20)     3332 2023-07-26 02:23:36.745650 hcs-cli-0.1.47/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     2458 2023-07-06 08:03:28.000000 hcs-cli-0.1.47/README.md
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.548447 hcs-cli-0.1.47/doc/
--rw-r--r--   0 nanw       (501) staff       (20)      639 2023-07-10 17:49:04.000000 hcs-cli-0.1.47/doc/az-cheatsheet.md
--rw-r--r--   0 nanw       (501) staff       (20)     5950 2023-06-15 17:50:47.000000 hcs-cli-0.1.47/doc/dev-setup.md
--rw-r--r--   0 nanw       (501) staff       (20)      763 2023-06-13 17:49:20.000000 hcs-cli-0.1.47/doc/get-csp-user-api-token.md
--rw-r--r--   0 nanw       (501) staff       (20)     6802 2023-07-06 01:23:30.000000 hcs-cli-0.1.47/doc/hcs-cli-cheatsheet.md
--rw-r--r--   0 nanw       (501) staff       (20)     6164 2023-07-18 01:31:14.000000 hcs-cli-0.1.47/doc/hcs-plan.md
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.553564 hcs-cli-0.1.47/hcs_cli.egg-info/
--rw-r--r--   0 nanw       (501) staff       (20)     3332 2023-07-26 02:23:35.000000 hcs-cli-0.1.47/hcs_cli.egg-info/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     7841 2023-07-26 02:23:36.000000 hcs-cli-0.1.47/hcs_cli.egg-info/SOURCES.txt
--rw-r--r--   0 nanw       (501) staff       (20)        1 2023-07-26 02:23:35.000000 hcs-cli-0.1.47/hcs_cli.egg-info/dependency_links.txt
--rw-r--r--   0 nanw       (501) staff       (20)       43 2023-07-26 02:23:35.000000 hcs-cli-0.1.47/hcs_cli.egg-info/entry_points.txt
--rw-r--r--   0 nanw       (501) staff       (20)      213 2023-07-26 02:23:35.000000 hcs-cli-0.1.47/hcs_cli.egg-info/requires.txt
--rw-r--r--   0 nanw       (501) staff       (20)       11 2023-07-26 02:23:35.000000 hcs-cli-0.1.47/hcs_cli.egg-info/top_level.txt
--rw-r--r--   0 nanw       (501) staff       (20)       92 2023-04-24 20:24:05.000000 hcs-cli-0.1.47/mypy.ini
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.495096 hcs-cli-0.1.47/payload/
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.554481 hcs-cli-0.1.47/payload/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)      752 2023-04-24 20:24:05.000000 hcs-cli-0.1.47/payload/lcm/zero.json
--rw-r--r--   0 nanw       (501) staff       (20)     1187 2023-06-13 19:56:09.000000 hcs-cli-0.1.47/pyproject.toml
--rw-r--r--   0 nanw       (501) staff       (20)      194 2023-07-05 20:09:57.000000 hcs-cli-0.1.47/requirements-dev.txt
--rw-r--r--   0 nanw       (501) staff       (20)      213 2023-07-05 20:09:23.000000 hcs-cli-0.1.47/requirements.txt
--rw-r--r--   0 nanw       (501) staff       (20)       38 2023-07-26 02:23:36.747286 hcs-cli-0.1.47/setup.cfg
--rw-r--r--   0 nanw       (501) staff       (20)     1154 2023-07-26 02:23:28.000000 hcs-cli-0.1.47/setup.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.557622 hcs-cli-0.1.47/tests/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.47/tests/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.47/tests/conftest.py
--rwxr-xr-x   0 nanw       (501) staff       (20)       85 2023-07-26 00:47:17.000000 hcs-cli-0.1.47/tests/test.sh
--rw-r--r--   0 nanw       (501) staff       (20)     3363 2023-07-26 01:38:26.000000 hcs-cli-0.1.47/tests/test_utils.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.558419 hcs-cli-0.1.47/tests/vhcs/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.47/tests/vhcs/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.559217 hcs-cli-0.1.47/tests/vhcs/cli/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.47/tests/vhcs/cli/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.562121 hcs-cli-0.1.47/tests/vhcs/cli/cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.47/tests/vhcs/cli/cmds/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.563497 hcs-cli-0.1.47/tests/vhcs/cli/cmds/pki/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.47/tests/vhcs/cli/cmds/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.47/tests/vhcs/cli/cmds/pki/get_root_ca.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.564862 hcs-cli-0.1.47/tests/vhcs/cli/cmds/plan/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-07-05 15:13:25.000000 hcs-cli-0.1.47/tests/vhcs/cli/cmds/plan/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     9408 2023-07-26 02:20:32.000000 hcs-cli-0.1.47/tests/vhcs/cli/cmds/plan/test_plan.py
--rw-r--r--   0 nanw       (501) staff       (20)     1943 2023-06-13 19:40:36.000000 hcs-cli-0.1.47/tests/vhcs/cli/cmds/test_context.py
--rw-r--r--   0 nanw       (501) staff       (20)      918 2023-07-03 19:18:10.000000 hcs-cli-0.1.47/tests/vhcs/cli/cmds/test_login.py
--rw-r--r--   0 nanw       (501) staff       (20)     1151 2023-07-05 08:29:47.000000 hcs-cli-0.1.47/tests/vhcs/cli/cmds/test_profile.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.566270 hcs-cli-0.1.47/vhcs/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 21:25:27.000000 hcs-cli-0.1.47/vhcs/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      687 2023-06-13 19:40:36.000000 hcs-cli-0.1.47/vhcs/__main__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.567533 hcs-cli-0.1.47/vhcs/cli/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.47/vhcs/cli/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.569400 hcs-cli-0.1.47/vhcs/cli/cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.47/vhcs/cli/cmds/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.569992 hcs-cli-0.1.47/vhcs/cli/cmds/admin/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-13 19:40:36.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.572439 hcs-cli-0.1.47/vhcs/cli/cmds/admin/ad/
--rw-r--r--   0 nanw       (501) staff       (20)      636 2023-07-24 16:33:32.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/ad/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      984 2023-07-24 16:35:03.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/ad/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      943 2023-07-24 16:35:13.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/ad/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      855 2023-07-24 16:35:24.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/ad/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.572966 hcs-cli-0.1.47/vhcs/cli/cmds/admin/azure-infra/
--rw-r--r--   0 nanw       (501) staff       (20)     1016 2023-07-19 21:52:53.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/azure-infra/main.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.575215 hcs-cli-0.1.47/vhcs/cli/cmds/admin/edge/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/edge/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     2303 2023-07-24 18:15:37.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/edge/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      926 2023-07-19 21:53:29.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/edge/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      861 2023-07-25 02:42:47.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/edge/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.577491 hcs-cli-0.1.47/vhcs/cli/cmds/admin/provider/
--rw-r--r--   0 nanw       (501) staff       (20)     2606 2023-07-19 22:02:33.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/provider/create.py
--rw-r--r--   0 nanw       (501) staff       (20)     1039 2023-07-24 18:12:59.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/provider/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)     1059 2023-07-19 21:54:27.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/provider/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1205 2023-07-19 21:54:48.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/provider/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.579903 hcs-cli-0.1.47/vhcs/cli/cmds/admin/template/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/template/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1119 2023-07-24 21:42:00.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/template/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      933 2023-07-19 21:54:59.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/template/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1845 2023-07-24 21:40:06.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/template/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.581720 hcs-cli-0.1.47/vhcs/cli/cmds/admin/template/vm/
--rw-r--r--   0 nanw       (501) staff       (20)      622 2023-07-08 00:36:46.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/template/vm/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1002 2023-07-19 21:55:21.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/template/vm/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      933 2023-07-19 21:55:32.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/template/vm/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.584237 hcs-cli-0.1.47/vhcs/cli/cmds/admin/uag/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-07-17 17:45:02.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/uag/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1205 2023-07-21 02:40:22.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/uag/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      922 2023-07-19 22:38:04.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/uag/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      857 2023-07-19 22:46:04.000000 hcs-cli-0.1.47/vhcs/cli/cmds/admin/uag/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.584885 hcs-cli-0.1.47/vhcs/cli/cmds/auth/
--rw-r--r--   0 nanw       (501) staff       (20)      632 2023-07-11 01:47:20.000000 hcs-cli-0.1.47/vhcs/cli/cmds/auth/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.586249 hcs-cli-0.1.47/vhcs/cli/cmds/auth/admin/
--rw-r--r--   0 nanw       (501) staff       (20)      642 2023-07-11 01:47:42.000000 hcs-cli-0.1.47/vhcs/cli/cmds/auth/admin/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      915 2023-07-24 16:53:46.000000 hcs-cli-0.1.47/vhcs/cli/cmds/auth/admin/get_org_idp_map.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.586867 hcs-cli-0.1.47/vhcs/cli/cmds/daas/
--rw-r--r--   0 nanw       (501) staff       (20)      642 2023-06-15 22:15:00.000000 hcs-cli-0.1.47/vhcs/cli/cmds/daas/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.588687 hcs-cli-0.1.47/vhcs/cli/cmds/daas/infra/
--rw-r--r--   0 nanw       (501) staff       (20)      648 2023-06-21 17:56:47.000000 hcs-cli-0.1.47/vhcs/cli/cmds/daas/infra/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1041 2023-06-30 16:52:44.000000 hcs-cli-0.1.47/vhcs/cli/cmds/daas/infra/basic.py
--rw-r--r--   0 nanw       (501) staff       (20)     4488 2023-07-19 00:05:29.000000 hcs-cli-0.1.47/vhcs/cli/cmds/daas/infra/plan.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.589817 hcs-cli-0.1.47/vhcs/cli/cmds/daas/tenant/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-21 17:36:22.000000 hcs-cli-0.1.47/vhcs/cli/cmds/daas/tenant/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     3366 2023-07-21 18:06:04.000000 hcs-cli-0.1.47/vhcs/cli/cmds/daas/tenant/plan.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.592617 hcs-cli-0.1.47/vhcs/cli/cmds/ims/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-27 19:52:41.000000 hcs-cli-0.1.47/vhcs/cli/cmds/ims/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      969 2023-07-25 21:09:30.000000 hcs-cli-0.1.47/vhcs/cli/cmds/ims/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      907 2023-07-25 15:46:38.000000 hcs-cli-0.1.47/vhcs/cli/cmds/ims/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      928 2023-07-25 00:33:49.000000 hcs-cli-0.1.47/vhcs/cli/cmds/ims/list.py
--rw-r--r--   0 nanw       (501) staff       (20)     1002 2023-07-24 23:58:01.000000 hcs-cli-0.1.47/vhcs/cli/cmds/ims/list_copies.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.595291 hcs-cli-0.1.47/vhcs/cli/cmds/ims/version/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-07-18 20:31:16.000000 hcs-cli-0.1.47/vhcs/cli/cmds/ims/version/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1722 2023-07-24 18:08:29.000000 hcs-cli-0.1.47/vhcs/cli/cmds/ims/version/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)     1284 2023-07-24 18:08:33.000000 hcs-cli-0.1.47/vhcs/cli/cmds/ims/version/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1144 2023-07-19 21:58:21.000000 hcs-cli-0.1.47/vhcs/cli/cmds/ims/version/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.596978 hcs-cli-0.1.47/vhcs/cli/cmds/inventory/
--rw-r--r--   0 nanw       (501) staff       (20)      637 2023-07-08 00:10:13.000000 hcs-cli-0.1.47/vhcs/cli/cmds/inventory/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1049 2023-07-19 21:58:33.000000 hcs-cli-0.1.47/vhcs/cli/cmds/inventory/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      942 2023-07-19 21:58:43.000000 hcs-cli-0.1.47/vhcs/cli/cmds/inventory/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.597552 hcs-cli-0.1.47/vhcs/cli/cmds/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)      631 2023-06-27 19:52:37.000000 hcs-cli-0.1.47/vhcs/cli/cmds/lcm/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.599933 hcs-cli-0.1.47/vhcs/cli/cmds/lcm/provider/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.47/vhcs/cli/cmds/lcm/provider/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      801 2023-06-23 02:35:21.000000 hcs-cli-0.1.47/vhcs/cli/cmds/lcm/provider/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      792 2023-06-23 02:35:30.000000 hcs-cli-0.1.47/vhcs/cli/cmds/lcm/provider/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      971 2023-07-19 21:58:53.000000 hcs-cli-0.1.47/vhcs/cli/cmds/lcm/provider/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.603324 hcs-cli-0.1.47/vhcs/cli/cmds/lcm/template/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.47/vhcs/cli/cmds/lcm/template/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1992 2023-07-19 22:34:00.000000 hcs-cli-0.1.47/vhcs/cli/cmds/lcm/template/create.py
--rw-r--r--   0 nanw       (501) staff       (20)     1063 2023-07-19 21:59:46.000000 hcs-cli-0.1.47/vhcs/cli/cmds/lcm/template/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      840 2023-06-23 02:37:07.000000 hcs-cli-0.1.47/vhcs/cli/cmds/lcm/template/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1572 2023-07-19 21:59:58.000000 hcs-cli-0.1.47/vhcs/cli/cmds/lcm/template/list.py
--rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-07-19 22:32:52.000000 hcs-cli-0.1.47/vhcs/cli/cmds/lcm/template/wait.py
--rw-r--r--   0 nanw       (501) staff       (20)     6922 2023-07-06 00:55:04.000000 hcs-cli-0.1.47/vhcs/cli/cmds/login.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.509862 hcs-cli-0.1.47/vhcs/cli/cmds/org/
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.604495 hcs-cli-0.1.47/vhcs/cli/cmds/org/datacenter/
--rw-r--r--   0 nanw       (501) staff       (20)      848 2023-06-30 15:40:06.000000 hcs-cli-0.1.47/vhcs/cli/cmds/org/datacenter/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      981 2023-07-19 22:00:09.000000 hcs-cli-0.1.47/vhcs/cli/cmds/org/datacenter/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.605645 hcs-cli-0.1.47/vhcs/cli/cmds/org/detail/
--rw-r--r--   0 nanw       (501) staff       (20)      890 2023-07-19 22:00:19.000000 hcs-cli-0.1.47/vhcs/cli/cmds/org/detail/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1201 2023-06-30 15:40:25.000000 hcs-cli-0.1.47/vhcs/cli/cmds/org/detail/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.609084 hcs-cli-0.1.47/vhcs/cli/cmds/pki/
--rw-r--r--   0 nanw       (501) staff       (20)      631 2023-06-13 19:45:45.000000 hcs-cli-0.1.47/vhcs/cli/cmds/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1139 2023-07-19 22:02:33.000000 hcs-cli-0.1.47/vhcs/cli/cmds/pki/delete_org_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      890 2023-07-19 22:02:33.000000 hcs-cli-0.1.47/vhcs/cli/cmds/pki/get_org_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      775 2023-06-30 15:38:40.000000 hcs-cli-0.1.47/vhcs/cli/cmds/pki/get_root_ca.py
--rw-r--r--   0 nanw       (501) staff       (20)     1788 2023-07-19 22:02:33.000000 hcs-cli-0.1.47/vhcs/cli/cmds/pki/sign_resource_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      726 2023-06-30 15:38:40.000000 hcs-cli-0.1.47/vhcs/cli/cmds/pki/test.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.611362 hcs-cli-0.1.47/vhcs/cli/cmds/plan/
--rw-r--r--   0 nanw       (501) staff       (20)      665 2023-06-28 17:52:44.000000 hcs-cli-0.1.47/vhcs/cli/cmds/plan/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     2131 2023-07-21 03:10:13.000000 hcs-cli-0.1.47/vhcs/cli/cmds/plan/deploy.py
--rw-r--r--   0 nanw       (501) staff       (20)     1853 2023-07-25 02:15:59.000000 hcs-cli-0.1.47/vhcs/cli/cmds/plan/destroy.py
--rw-r--r--   0 nanw       (501) staff       (20)     1682 2023-07-20 01:42:45.000000 hcs-cli-0.1.47/vhcs/cli/cmds/plan/graph.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.611928 hcs-cli-0.1.47/vhcs/cli/cmds/portal/
--rw-r--r--   0 nanw       (501) staff       (20)      634 2023-07-10 08:01:20.000000 hcs-cli-0.1.47/vhcs/cli/cmds/portal/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.616015 hcs-cli-0.1.47/vhcs/cli/cmds/portal/entitlement/
--rw-r--r--   0 nanw       (501) staff       (20)      624 2023-07-11 03:23:55.000000 hcs-cli-0.1.47/vhcs/cli/cmds/portal/entitlement/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      926 2023-07-19 22:02:34.000000 hcs-cli-0.1.47/vhcs/cli/cmds/portal/entitlement/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      953 2023-07-24 21:35:27.000000 hcs-cli-0.1.47/vhcs/cli/cmds/portal/entitlement/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      862 2023-07-24 21:32:49.000000 hcs-cli-0.1.47/vhcs/cli/cmds/portal/entitlement/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.620846 hcs-cli-0.1.47/vhcs/cli/cmds/portal/pool/
--rw-r--r--   0 nanw       (501) staff       (20)      624 2023-07-10 08:01:44.000000 hcs-cli-0.1.47/vhcs/cli/cmds/portal/pool/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      915 2023-07-19 22:02:34.000000 hcs-cli-0.1.47/vhcs/cli/cmds/portal/pool/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      940 2023-07-19 22:02:34.000000 hcs-cli-0.1.47/vhcs/cli/cmds/portal/pool/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      931 2023-07-24 21:37:06.000000 hcs-cli-0.1.47/vhcs/cli/cmds/portal/pool/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.624714 hcs-cli-0.1.47/vhcs/cli/cmds/portal/site/
--rw-r--r--   0 nanw       (501) staff       (20)      624 2023-07-11 20:43:14.000000 hcs-cli-0.1.47/vhcs/cli/cmds/portal/site/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1108 2023-07-19 22:02:33.000000 hcs-cli-0.1.47/vhcs/cli/cmds/portal/site/create.py
--rw-r--r--   0 nanw       (501) staff       (20)      912 2023-07-19 22:02:33.000000 hcs-cli-0.1.47/vhcs/cli/cmds/portal/site/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      934 2023-07-19 22:02:33.000000 hcs-cli-0.1.47/vhcs/cli/cmds/portal/site/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      837 2023-07-21 18:40:45.000000 hcs-cli-0.1.47/vhcs/cli/cmds/portal/site/list.py
--rw-r--r--   0 nanw       (501) staff       (20)     1022 2023-07-21 18:42:53.000000 hcs-cli-0.1.47/vhcs/cli/cmds/portal/site/set-edge.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.625914 hcs-cli-0.1.47/vhcs/cli/cmds/profile/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.47/vhcs/cli/cmds/profile/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1765 2023-07-05 06:16:00.000000 hcs-cli-0.1.47/vhcs/cli/cmds/profile/init.py
--rw-r--r--   0 nanw       (501) staff       (20)      932 2023-06-13 19:40:36.000000 hcs-cli-0.1.47/vhcs/cli/cmds/upgrade.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.626467 hcs-cli-0.1.47/vhcs/cli/cmds/vmhub/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-13 19:40:36.000000 hcs-cli-0.1.47/vhcs/cli/cmds/vmhub/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.628155 hcs-cli-0.1.47/vhcs/cli/cmds/vmhub/otp/
--rw-r--r--   0 nanw       (501) staff       (20)      643 2023-06-29 21:49:43.000000 hcs-cli-0.1.47/vhcs/cli/cmds/vmhub/otp/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1234 2023-06-29 21:49:20.000000 hcs-cli-0.1.47/vhcs/cli/cmds/vmhub/otp/redeem.py
--rw-r--r--   0 nanw       (501) staff       (20)     1127 2023-07-19 22:02:33.000000 hcs-cli-0.1.47/vhcs/cli/cmds/vmhub/otp/request.py
--rwxr-xr-x   0 nanw       (501) staff       (20)     2865 2023-06-23 02:40:39.000000 hcs-cli-0.1.47/vhcs/cli/main.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.630514 hcs-cli-0.1.47/vhcs/common/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.47/vhcs/common/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.639062 hcs-cli-0.1.47/vhcs/common/ctxp/
--rw-r--r--   0 nanw       (501) staff       (20)     1538 2023-07-03 20:20:16.000000 hcs-cli-0.1.47/vhcs/common/ctxp/README.md
--rw-r--r--   0 nanw       (501) staff       (20)      790 2023-07-03 20:45:37.000000 hcs-cli-0.1.47/vhcs/common/ctxp/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1155 2023-07-03 21:18:13.000000 hcs-cli-0.1.47/vhcs/common/ctxp/_init.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.640839 hcs-cli-0.1.47/vhcs/common/ctxp/built_in_cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.47/vhcs/common/ctxp/built_in_cmds/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     2421 2023-06-21 17:26:56.000000 hcs-cli-0.1.47/vhcs/common/ctxp/built_in_cmds/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     3989 2023-07-05 23:22:13.000000 hcs-cli-0.1.47/vhcs/common/ctxp/built_in_cmds/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     5129 2023-07-05 06:22:51.000000 hcs-cli-0.1.47/vhcs/common/ctxp/cli_processor.py
--rw-r--r--   0 nanw       (501) staff       (20)      936 2023-07-03 21:17:12.000000 hcs-cli-0.1.47/vhcs/common/ctxp/config.py
--rw-r--r--   0 nanw       (501) staff       (20)     1205 2023-07-03 21:08:50.000000 hcs-cli-0.1.47/vhcs/common/ctxp/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     6467 2023-06-23 00:26:19.000000 hcs-cli-0.1.47/vhcs/common/ctxp/fstore.py
--rw-r--r--   0 nanw       (501) staff       (20)     1200 2023-06-13 19:40:36.000000 hcs-cli-0.1.47/vhcs/common/ctxp/init.py
--rw-r--r--   0 nanw       (501) staff       (20)     3060 2023-07-11 23:13:07.000000 hcs-cli-0.1.47/vhcs/common/ctxp/jsondot.py
--rw-r--r--   0 nanw       (501) staff       (20)     5526 2023-07-11 08:29:40.000000 hcs-cli-0.1.47/vhcs/common/ctxp/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     1565 2023-07-05 06:52:28.000000 hcs-cli-0.1.47/vhcs/common/ctxp/profile_store.py
--rw-r--r--   0 nanw       (501) staff       (20)     1604 2023-07-03 22:06:25.000000 hcs-cli-0.1.47/vhcs/common/ctxp/state.py
--rw-r--r--   0 nanw       (501) staff       (20)     6812 2023-07-25 22:42:34.000000 hcs-cli-0.1.47/vhcs/common/ctxp/util.py
--rw-r--r--   0 nanw       (501) staff       (20)     3256 2023-06-13 19:40:36.000000 hcs-cli-0.1.47/vhcs/common/ctxp/var_template.py
--rw-r--r--   0 nanw       (501) staff       (20)     2259 2023-07-05 18:05:17.000000 hcs-cli-0.1.47/vhcs/common/duration.py
--rw-r--r--   0 nanw       (501) staff       (20)     6329 2023-07-13 00:38:57.000000 hcs-cli-0.1.47/vhcs/common/logger.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.645627 hcs-cli-0.1.47/vhcs/common/sglib/
--rw-r--r--   0 nanw       (501) staff       (20)      654 2023-06-13 19:40:36.000000 hcs-cli-0.1.47/vhcs/common/sglib/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     4648 2023-07-07 17:06:56.000000 hcs-cli-0.1.47/vhcs/common/sglib/auth.py
--rw-r--r--   0 nanw       (501) staff       (20)     1808 2023-07-19 22:44:47.000000 hcs-cli-0.1.47/vhcs/common/sglib/cli_options.py
--rw-r--r--   0 nanw       (501) staff       (20)     8079 2023-07-05 07:42:49.000000 hcs-cli-0.1.47/vhcs/common/sglib/csp.py
--rw-r--r--   0 nanw       (501) staff       (20)     5200 2023-07-18 18:53:18.000000 hcs-cli-0.1.47/vhcs/common/sglib/ez_client.py
--rw-r--r--   0 nanw       (501) staff       (20)      906 2023-07-07 17:01:14.000000 hcs-cli-0.1.47/vhcs/common/sglib/hcs_client.py
--rw-r--r--   0 nanw       (501) staff       (20)     8243 2023-07-05 08:11:32.000000 hcs-cli-0.1.47/vhcs/common/sglib/login_support.py
--rw-r--r--   0 nanw       (501) staff       (20)      600 2023-07-19 22:16:46.000000 hcs-cli-0.1.47/vhcs/common/sglib/util.py
--rw-r--r--   0 nanw       (501) staff       (20)     9986 2023-07-19 00:35:32.000000 hcs-cli-0.1.47/vhcs/common/util.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.647378 hcs-cli-0.1.47/vhcs/config/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.47/vhcs/config/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     7771 2023-07-03 22:19:24.000000 hcs-cli-0.1.47/vhcs/config/hcs-deployments.yaml
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.652955 hcs-cli-0.1.47/vhcs/plan/
--rw-r--r--   0 nanw       (501) staff       (20)      142 2023-07-25 17:16:12.000000 hcs-cli-0.1.47/vhcs/plan/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      103 2023-07-25 20:51:20.000000 hcs-cli-0.1.47/vhcs/plan/actions.py
--rw-r--r--   0 nanw       (501) staff       (20)      113 2023-07-25 17:15:18.000000 hcs-cli-0.1.47/vhcs/plan/context.py
--rw-r--r--   0 nanw       (501) staff       (20)    15923 2023-07-26 02:14:28.000000 hcs-cli-0.1.47/vhcs/plan/core.py
--rw-r--r--   0 nanw       (501) staff       (20)     7169 2023-07-26 01:45:08.000000 hcs-cli-0.1.47/vhcs/plan/dag.py
--rw-r--r--   0 nanw       (501) staff       (20)     6243 2023-07-20 01:40:19.000000 hcs-cli-0.1.47/vhcs/plan/helper.py
--rw-r--r--   0 nanw       (501) staff       (20)     5070 2023-07-26 02:12:47.000000 hcs-cli-0.1.47/vhcs/plan/kop.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.654144 hcs-cli-0.1.47/vhcs/plan/provider/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-28 17:25:18.000000 hcs-cli-0.1.47/vhcs/plan/provider/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.659016 hcs-cli-0.1.47/vhcs/plan/provider/azure/
--rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-30 00:51:51.000000 hcs-cli-0.1.47/vhcs/plan/provider/azure/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     5381 2023-07-13 00:28:42.000000 hcs-cli-0.1.47/vhcs/plan/provider/azure/_az_facade.py
--rw-r--r--   0 nanw       (501) staff       (20)      563 2023-07-17 22:53:19.000000 hcs-cli-0.1.47/vhcs/plan/provider/azure/_prepare.py
--rw-r--r--   0 nanw       (501) staff       (20)     1436 2023-07-20 00:02:39.000000 hcs-cli-0.1.47/vhcs/plan/provider/azure/aad_group.py
--rw-r--r--   0 nanw       (501) staff       (20)     1983 2023-07-20 00:02:46.000000 hcs-cli-0.1.47/vhcs/plan/provider/azure/aad_user.py
--rw-r--r--   0 nanw       (501) staff       (20)     1310 2023-07-20 00:02:49.000000 hcs-cli-0.1.47/vhcs/plan/provider/azure/nsg.py
--rw-r--r--   0 nanw       (501) staff       (20)     1087 2023-07-20 00:02:52.000000 hcs-cli-0.1.47/vhcs/plan/provider/azure/resource_group.py
--rw-r--r--   0 nanw       (501) staff       (20)     1364 2023-07-20 00:02:56.000000 hcs-cli-0.1.47/vhcs/plan/provider/azure/subnet.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.660711 hcs-cli-0.1.47/vhcs/plan/provider/dev/
--rw-r--r--   0 nanw       (501) staff       (20)       29 2023-07-05 15:12:02.000000 hcs-cli-0.1.47/vhcs/plan/provider/dev/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)       33 2023-07-05 15:12:02.000000 hcs-cli-0.1.47/vhcs/plan/provider/dev/_prepare.py
--rw-r--r--   0 nanw       (501) staff       (20)     1455 2023-07-20 01:40:39.000000 hcs-cli-0.1.47/vhcs/plan/provider/dev/dummy.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.668383 hcs-cli-0.1.47/vhcs/plan/provider/hcs/
--rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-29 23:41:13.000000 hcs-cli-0.1.47/vhcs/plan/provider/hcs/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)       33 2023-06-29 23:41:19.000000 hcs-cli-0.1.47/vhcs/plan/provider/hcs/_prepare.py
--rw-r--r--   0 nanw       (501) staff       (20)     1325 2023-07-24 16:43:18.000000 hcs-cli-0.1.47/vhcs/plan/provider/hcs/ad.py
--rw-r--r--   0 nanw       (501) staff       (20)     2144 2023-07-25 02:48:50.000000 hcs-cli-0.1.47/vhcs/plan/provider/hcs/edge.py
--rw-r--r--   0 nanw       (501) staff       (20)     1150 2023-07-20 00:01:09.000000 hcs-cli-0.1.47/vhcs/plan/provider/hcs/entitlement.py
--rw-r--r--   0 nanw       (501) staff       (20)     1238 2023-07-24 16:56:20.000000 hcs-cli-0.1.47/vhcs/plan/provider/hcs/identity_provider.py
--rw-r--r--   0 nanw       (501) staff       (20)     3162 2023-07-25 23:34:57.000000 hcs-cli-0.1.47/vhcs/plan/provider/hcs/image.py
--rw-r--r--   0 nanw       (501) staff       (20)     1431 2023-07-20 00:03:09.000000 hcs-cli-0.1.47/vhcs/plan/provider/hcs/launch_item.py
--rw-r--r--   0 nanw       (501) staff       (20)     1332 2023-07-20 00:03:13.000000 hcs-cli-0.1.47/vhcs/plan/provider/hcs/pool_group.py
--rw-r--r--   0 nanw       (501) staff       (20)     1882 2023-07-21 02:43:52.000000 hcs-cli-0.1.47/vhcs/plan/provider/hcs/pool_template.py
--rw-r--r--   0 nanw       (501) staff       (20)     1456 2023-07-20 00:03:22.000000 hcs-cli-0.1.47/vhcs/plan/provider/hcs/provider.py
--rw-r--r--   0 nanw       (501) staff       (20)     1238 2023-07-20 02:11:18.000000 hcs-cli-0.1.47/vhcs/plan/provider/hcs/site.py
--rw-r--r--   0 nanw       (501) staff       (20)     1831 2023-07-25 22:45:13.000000 hcs-cli-0.1.47/vhcs/plan/provider/hcs/uag.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.669438 hcs-cli-0.1.47/vhcs/service/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.47/vhcs/service/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     5494 2023-07-25 18:36:04.000000 hcs-cli-0.1.47/vhcs/service/_util.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.673476 hcs-cli-0.1.47/vhcs/service/admin/
--rw-r--r--   0 nanw       (501) staff       (20)       68 2023-07-24 16:34:10.000000 hcs-cli-0.1.47/vhcs/service/admin/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      853 2023-07-24 16:32:50.000000 hcs-cli-0.1.47/vhcs/service/admin/ad.py
--rw-r--r--   0 nanw       (501) staff       (20)     1211 2023-07-06 14:56:48.000000 hcs-cli-0.1.47/vhcs/service/admin/azure_infra.py
--rw-r--r--   0 nanw       (501) staff       (20)     2759 2023-07-25 18:27:51.000000 hcs-cli-0.1.47/vhcs/service/admin/edge.py
--rw-r--r--   0 nanw       (501) staff       (20)     1082 2023-07-24 17:45:25.000000 hcs-cli-0.1.47/vhcs/service/admin/helper.py
--rw-r--r--   0 nanw       (501) staff       (20)     1459 2023-07-18 19:54:38.000000 hcs-cli-0.1.47/vhcs/service/admin/provider.py
--rw-r--r--   0 nanw       (501) staff       (20)     1934 2023-07-25 18:21:27.000000 hcs-cli-0.1.47/vhcs/service/admin/template.py
--rw-r--r--   0 nanw       (501) staff       (20)     2279 2023-07-25 18:16:29.000000 hcs-cli-0.1.47/vhcs/service/admin/uag.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.674494 hcs-cli-0.1.47/vhcs/service/auth/
--rw-r--r--   0 nanw       (501) staff       (20)       19 2023-06-22 18:49:46.000000 hcs-cli-0.1.47/vhcs/service/auth/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      879 2023-07-24 17:10:24.000000 hcs-cli-0.1.47/vhcs/service/auth/admin.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.677368 hcs-cli-0.1.47/vhcs/service/ims/
--rw-r--r--   0 nanw       (501) staff       (20)       71 2023-07-18 21:11:37.000000 hcs-cli-0.1.47/vhcs/service/ims/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     2231 2023-07-25 23:34:52.000000 hcs-cli-0.1.47/vhcs/service/ims/helper.py
--rw-r--r--   0 nanw       (501) staff       (20)      944 2023-07-19 21:57:09.000000 hcs-cli-0.1.47/vhcs/service/ims/image_copies.py
--rw-r--r--   0 nanw       (501) staff       (20)     1912 2023-07-25 22:16:59.000000 hcs-cli-0.1.47/vhcs/service/ims/images.py
--rw-r--r--   0 nanw       (501) staff       (20)     3140 2023-07-25 18:34:44.000000 hcs-cli-0.1.47/vhcs/service/ims/version.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.678380 hcs-cli-0.1.47/vhcs/service/inventory/
--rw-r--r--   0 nanw       (501) staff       (20)       25 2023-07-08 00:42:34.000000 hcs-cli-0.1.47/vhcs/service/inventory/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1290 2023-07-08 00:32:38.000000 hcs-cli-0.1.47/vhcs/service/inventory/vm.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.680609 hcs-cli-0.1.47/vhcs/service/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)       32 2023-06-22 18:49:27.000000 hcs-cli-0.1.47/vhcs/service/lcm/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1437 2023-06-22 18:48:08.000000 hcs-cli-0.1.47/vhcs/service/lcm/provider.py
--rw-r--r--   0 nanw       (501) staff       (20)     2755 2023-07-21 02:58:07.000000 hcs-cli-0.1.47/vhcs/service/lcm/template.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.682275 hcs-cli-0.1.47/vhcs/service/org_service/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:38:56.000000 hcs-cli-0.1.47/vhcs/service/org_service/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1083 2023-06-30 15:37:59.000000 hcs-cli-0.1.47/vhcs/service/org_service/datacenter.py
--rw-r--r--   0 nanw       (501) staff       (20)     1040 2023-06-30 15:37:42.000000 hcs-cli-0.1.47/vhcs/service/org_service/details.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.683427 hcs-cli-0.1.47/vhcs/service/pki/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:38:50.000000 hcs-cli-0.1.47/vhcs/service/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1211 2023-06-30 15:38:16.000000 hcs-cli-0.1.47/vhcs/service/pki/certificate.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.685924 hcs-cli-0.1.47/vhcs/service/portal/
--rw-r--r--   0 nanw       (501) staff       (20)       37 2023-07-11 20:44:21.000000 hcs-cli-0.1.47/vhcs/service/portal/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      942 2023-07-24 21:34:40.000000 hcs-cli-0.1.47/vhcs/service/portal/entitlement.py
--rw-r--r--   0 nanw       (501) staff       (20)      929 2023-07-24 21:37:58.000000 hcs-cli-0.1.47/vhcs/service/portal/pool.py
--rw-r--r--   0 nanw       (501) staff       (20)     1493 2023-07-21 18:45:40.000000 hcs-cli-0.1.47/vhcs/service/portal/site.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.687646 hcs-cli-0.1.47/vhcs/service/vmhub/
--rw-r--r--   0 nanw       (501) staff       (20)       17 2023-07-03 19:03:42.000000 hcs-cli-0.1.47/vhcs/service/vmhub/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1406 2023-06-29 21:48:05.000000 hcs-cli-0.1.47/vhcs/service/vmhub/otp.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.689797 hcs-cli-0.1.47/vhcs/support/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:35:24.000000 hcs-cli-0.1.47/vhcs/support/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.715250 hcs-cli-0.1.47/vhcs/support/daas/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-21 23:10:31.000000 hcs-cli-0.1.47/vhcs/support/daas/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1482 2023-07-13 00:23:42.000000 hcs-cli-0.1.47/vhcs/support/daas/cidr_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     3840 2023-07-21 18:07:07.000000 hcs-cli-0.1.47/vhcs/support/daas/helper.py
--rw-r--r--   0 nanw       (501) staff       (20)     1794 2023-07-17 22:53:28.000000 hcs-cli-0.1.47/vhcs/support/daas/infra.py
--rw-r--r--   0 nanw       (501) staff       (20)     3971 2023-07-25 17:39:54.000000 hcs-cli-0.1.47/vhcs/support/daas/infra_calc.py
--rw-r--r--   0 nanw       (501) staff       (20)      424 2023-07-11 23:57:51.000000 hcs-cli-0.1.47/vhcs/support/daas/template.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.526387 hcs-cli-0.1.47/vhcs/support/daas/templates/
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.731636 hcs-cli-0.1.47/vhcs/support/daas/templates/v1/
--rw-r--r--   0 nanw       (501) staff       (20)     7411 2023-07-20 16:47:59.000000 hcs-cli-0.1.47/vhcs/support/daas/templates/v1/infra.blueprint.yml
--rw-r--r--   0 nanw       (501) staff       (20)      517 2023-07-20 02:14:59.000000 hcs-cli-0.1.47/vhcs/support/daas/templates/v1/infra.vars.yml
--rw-r--r--   0 nanw       (501) staff       (20)     3690 2023-07-12 23:33:06.000000 hcs-cli-0.1.47/vhcs/support/daas/templates/v1/tenant.blueprint.yml
--rw-r--r--   0 nanw       (501) staff       (20)      236 2023-07-17 22:53:38.000000 hcs-cli-0.1.47/vhcs/support/daas/templates/v1/tenant.vars.yml
--rw-r--r--   0 nanw       (501) staff       (20)     4102 2023-07-18 23:24:45.000000 hcs-cli-0.1.47/vhcs/support/daas/tenant_calc.py
--rw-r--r--   0 nanw       (501) staff       (20)     1455 2023-07-11 20:14:32.000000 hcs-cli-0.1.47/vhcs/support/plan_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     2621 2023-07-05 07:42:08.000000 hcs-cli-0.1.47/vhcs/support/profile.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-26 02:23:36.743398 hcs-cli-0.1.47/vhcs/util/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.47/vhcs/util/__init__.py
--rwxr-xr-x   0 nanw       (501) staff       (20)     2535 2023-06-13 19:40:36.000000 hcs-cli-0.1.47/vhcs/util/check_license.py
--rw-r--r--   0 nanw       (501) staff       (20)     2759 2023-06-13 19:40:36.000000 hcs-cli-0.1.47/vhcs/util/duration.py
--rw-r--r--   0 nanw       (501) staff       (20)     5288 2023-06-13 19:40:36.000000 hcs-cli-0.1.47/vhcs/util/pki_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     1929 2023-07-18 18:58:54.000000 hcs-cli-0.1.47/vhcs/util/query_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     1725 2023-06-13 19:40:36.000000 hcs-cli-0.1.47/vhcs/util/versions.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.294866 hcs-cli-0.1.48/
+-rw-r--r--   0 nanw       (501) staff       (20)     2824 2023-06-21 18:44:48.000000 hcs-cli-0.1.48/.gitignore
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.047145 hcs-cli-0.1.48/.vscode/
+-rw-r--r--   0 nanw       (501) staff       (20)     3314 2023-07-31 00:05:25.000000 hcs-cli-0.1.48/.vscode/launch.json
+-rw-r--r--   0 nanw       (501) staff       (20)      391 2023-07-26 01:21:48.000000 hcs-cli-0.1.48/.vscode/settings.json
+-rw-r--r--   0 nanw       (501) staff       (20)       98 2023-06-13 19:57:56.000000 hcs-cli-0.1.48/CHANGELOG.md
+-rw-r--r--   0 nanw       (501) staff       (20)     5258 2023-06-13 16:45:49.000000 hcs-cli-0.1.48/CODE_OF_CONDUCT.md
+-rw-r--r--   0 nanw       (501) staff       (20)     2706 2023-06-13 18:53:18.000000 hcs-cli-0.1.48/CONTRIBUTING_CLA.md
+-rw-r--r--   0 nanw       (501) staff       (20)     6095 2023-04-25 23:13:27.000000 hcs-cli-0.1.48/GOVERNANCE.md
+-rw-r--r--   0 nanw       (501) staff       (20)    10449 2023-06-13 16:45:49.000000 hcs-cli-0.1.48/LICENSE
+-rw-r--r--   0 nanw       (501) staff       (20)      881 2023-07-11 00:05:40.000000 hcs-cli-0.1.48/Makefile
+-rw-r--r--   0 nanw       (501) staff       (20)      411 2023-06-13 16:45:49.000000 hcs-cli-0.1.48/NOTICE
+-rw-r--r--   0 nanw       (501) staff       (20)     3769 2023-07-31 01:12:46.294457 hcs-cli-0.1.48/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     2895 2023-07-26 02:28:33.000000 hcs-cli-0.1.48/README.md
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.053218 hcs-cli-0.1.48/doc/
+-rw-r--r--   0 nanw       (501) staff       (20)      639 2023-07-10 17:49:04.000000 hcs-cli-0.1.48/doc/az-cheatsheet.md
+-rw-r--r--   0 nanw       (501) staff       (20)     5950 2023-06-15 17:50:47.000000 hcs-cli-0.1.48/doc/dev-setup.md
+-rw-r--r--   0 nanw       (501) staff       (20)      763 2023-06-13 17:49:20.000000 hcs-cli-0.1.48/doc/get-csp-user-api-token.md
+-rw-r--r--   0 nanw       (501) staff       (20)     6802 2023-07-06 01:23:30.000000 hcs-cli-0.1.48/doc/hcs-cli-cheatsheet.md
+-rw-r--r--   0 nanw       (501) staff       (20)     6164 2023-07-18 01:31:14.000000 hcs-cli-0.1.48/doc/hcs-plan.md
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.057561 hcs-cli-0.1.48/hcs_cli.egg-info/
+-rw-r--r--   0 nanw       (501) staff       (20)     3769 2023-07-31 01:12:45.000000 hcs-cli-0.1.48/hcs_cli.egg-info/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     8169 2023-07-31 01:12:45.000000 hcs-cli-0.1.48/hcs_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 nanw       (501) staff       (20)        1 2023-07-31 01:12:45.000000 hcs-cli-0.1.48/hcs_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       43 2023-07-31 01:12:45.000000 hcs-cli-0.1.48/hcs_cli.egg-info/entry_points.txt
+-rw-r--r--   0 nanw       (501) staff       (20)      295 2023-07-31 01:12:45.000000 hcs-cli-0.1.48/hcs_cli.egg-info/requires.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       11 2023-07-31 01:12:45.000000 hcs-cli-0.1.48/hcs_cli.egg-info/top_level.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       92 2023-04-24 20:24:05.000000 hcs-cli-0.1.48/mypy.ini
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:45.999303 hcs-cli-0.1.48/payload/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.058479 hcs-cli-0.1.48/payload/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)      752 2023-04-24 20:24:05.000000 hcs-cli-0.1.48/payload/lcm/zero.json
+-rw-r--r--   0 nanw       (501) staff       (20)     1187 2023-06-13 19:56:09.000000 hcs-cli-0.1.48/pyproject.toml
+-rw-r--r--   0 nanw       (501) staff       (20)      194 2023-07-05 20:09:57.000000 hcs-cli-0.1.48/requirements-dev.txt
+-rw-r--r--   0 nanw       (501) staff       (20)      296 2023-07-29 05:49:51.000000 hcs-cli-0.1.48/requirements.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       38 2023-07-31 01:12:46.294995 hcs-cli-0.1.48/setup.cfg
+-rw-r--r--   0 nanw       (501) staff       (20)     1154 2023-07-31 01:11:59.000000 hcs-cli-0.1.48/setup.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.061777 hcs-cli-0.1.48/tests/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.48/tests/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.48/tests/conftest.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)       85 2023-07-26 00:47:17.000000 hcs-cli-0.1.48/tests/test.sh
+-rw-r--r--   0 nanw       (501) staff       (20)     3363 2023-07-26 01:38:26.000000 hcs-cli-0.1.48/tests/test_utils.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.062493 hcs-cli-0.1.48/tests/vhcs/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.48/tests/vhcs/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.063109 hcs-cli-0.1.48/tests/vhcs/cli/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.48/tests/vhcs/cli/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.065537 hcs-cli-0.1.48/tests/vhcs/cli/cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.48/tests/vhcs/cli/cmds/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.067183 hcs-cli-0.1.48/tests/vhcs/cli/cmds/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.48/tests/vhcs/cli/cmds/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.48/tests/vhcs/cli/cmds/pki/get_root_ca.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.068751 hcs-cli-0.1.48/tests/vhcs/cli/cmds/plan/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-07-05 15:13:25.000000 hcs-cli-0.1.48/tests/vhcs/cli/cmds/plan/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)    12447 2023-07-29 15:57:43.000000 hcs-cli-0.1.48/tests/vhcs/cli/cmds/plan/test_plan.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1943 2023-06-13 19:40:36.000000 hcs-cli-0.1.48/tests/vhcs/cli/cmds/test_context.py
+-rw-r--r--   0 nanw       (501) staff       (20)      918 2023-07-03 19:18:10.000000 hcs-cli-0.1.48/tests/vhcs/cli/cmds/test_login.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1151 2023-07-05 08:29:47.000000 hcs-cli-0.1.48/tests/vhcs/cli/cmds/test_profile.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.070272 hcs-cli-0.1.48/vhcs/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 21:25:27.000000 hcs-cli-0.1.48/vhcs/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      687 2023-06-13 19:40:36.000000 hcs-cli-0.1.48/vhcs/__main__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.072281 hcs-cli-0.1.48/vhcs/cli/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.48/vhcs/cli/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.077117 hcs-cli-0.1.48/vhcs/cli/cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.48/vhcs/cli/cmds/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.078173 hcs-cli-0.1.48/vhcs/cli/cmds/admin/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-13 19:40:36.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.082434 hcs-cli-0.1.48/vhcs/cli/cmds/admin/ad/
+-rw-r--r--   0 nanw       (501) staff       (20)      636 2023-07-24 16:33:32.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/ad/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      984 2023-07-24 16:35:03.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/ad/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      943 2023-07-24 16:35:13.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/ad/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      855 2023-07-24 16:35:24.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/ad/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.083393 hcs-cli-0.1.48/vhcs/cli/cmds/admin/azure-infra/
+-rw-r--r--   0 nanw       (501) staff       (20)     1016 2023-07-19 21:52:53.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/azure-infra/main.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.088367 hcs-cli-0.1.48/vhcs/cli/cmds/admin/edge/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/edge/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2303 2023-07-24 18:15:37.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/edge/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      926 2023-07-19 21:53:29.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/edge/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      861 2023-07-25 02:42:47.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/edge/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.093833 hcs-cli-0.1.48/vhcs/cli/cmds/admin/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)     2606 2023-07-19 22:02:33.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/provider/create.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1039 2023-07-24 18:12:59.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/provider/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1059 2023-07-19 21:54:27.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/provider/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1101 2023-07-28 18:11:23.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/provider/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.097622 hcs-cli-0.1.48/vhcs/cli/cmds/admin/template/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/template/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1119 2023-07-24 21:42:00.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/template/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      933 2023-07-19 21:54:59.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/template/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1845 2023-07-24 21:40:06.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/template/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.101685 hcs-cli-0.1.48/vhcs/cli/cmds/admin/template/vm/
+-rw-r--r--   0 nanw       (501) staff       (20)      622 2023-07-08 00:36:46.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/template/vm/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1002 2023-07-19 21:55:21.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/template/vm/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      933 2023-07-19 21:55:32.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/template/vm/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.105594 hcs-cli-0.1.48/vhcs/cli/cmds/admin/uag/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-07-17 17:45:02.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/uag/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1205 2023-07-21 02:40:22.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/uag/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      922 2023-07-19 22:38:04.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/uag/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      857 2023-07-19 22:46:04.000000 hcs-cli-0.1.48/vhcs/cli/cmds/admin/uag/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.106569 hcs-cli-0.1.48/vhcs/cli/cmds/auth/
+-rw-r--r--   0 nanw       (501) staff       (20)      632 2023-07-11 01:47:20.000000 hcs-cli-0.1.48/vhcs/cli/cmds/auth/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.108189 hcs-cli-0.1.48/vhcs/cli/cmds/auth/admin/
+-rw-r--r--   0 nanw       (501) staff       (20)      642 2023-07-11 01:47:42.000000 hcs-cli-0.1.48/vhcs/cli/cmds/auth/admin/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      915 2023-07-24 16:53:46.000000 hcs-cli-0.1.48/vhcs/cli/cmds/auth/admin/get_org_idp_map.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.108924 hcs-cli-0.1.48/vhcs/cli/cmds/daas/
+-rw-r--r--   0 nanw       (501) staff       (20)      642 2023-06-15 22:15:00.000000 hcs-cli-0.1.48/vhcs/cli/cmds/daas/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.111401 hcs-cli-0.1.48/vhcs/cli/cmds/daas/infra/
+-rw-r--r--   0 nanw       (501) staff       (20)      648 2023-06-21 17:56:47.000000 hcs-cli-0.1.48/vhcs/cli/cmds/daas/infra/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1041 2023-07-28 06:07:51.000000 hcs-cli-0.1.48/vhcs/cli/cmds/daas/infra/basic.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6571 2023-07-29 06:15:08.000000 hcs-cli-0.1.48/vhcs/cli/cmds/daas/infra/plan.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.113767 hcs-cli-0.1.48/vhcs/cli/cmds/daas/tenant/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-21 17:36:22.000000 hcs-cli-0.1.48/vhcs/cli/cmds/daas/tenant/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4149 2023-07-31 00:47:53.000000 hcs-cli-0.1.48/vhcs/cli/cmds/daas/tenant/plan.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.118409 hcs-cli-0.1.48/vhcs/cli/cmds/ims/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-27 19:52:41.000000 hcs-cli-0.1.48/vhcs/cli/cmds/ims/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      957 2023-07-29 14:34:24.000000 hcs-cli-0.1.48/vhcs/cli/cmds/ims/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      907 2023-07-25 15:46:38.000000 hcs-cli-0.1.48/vhcs/cli/cmds/ims/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      928 2023-07-25 00:33:49.000000 hcs-cli-0.1.48/vhcs/cli/cmds/ims/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1002 2023-07-24 23:58:01.000000 hcs-cli-0.1.48/vhcs/cli/cmds/ims/list_copies.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.122747 hcs-cli-0.1.48/vhcs/cli/cmds/ims/version/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-07-18 20:31:16.000000 hcs-cli-0.1.48/vhcs/cli/cmds/ims/version/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1722 2023-07-24 18:08:29.000000 hcs-cli-0.1.48/vhcs/cli/cmds/ims/version/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1284 2023-07-24 18:08:33.000000 hcs-cli-0.1.48/vhcs/cli/cmds/ims/version/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1144 2023-07-19 21:58:21.000000 hcs-cli-0.1.48/vhcs/cli/cmds/ims/version/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.126257 hcs-cli-0.1.48/vhcs/cli/cmds/inventory/
+-rw-r--r--   0 nanw       (501) staff       (20)      637 2023-07-08 00:10:13.000000 hcs-cli-0.1.48/vhcs/cli/cmds/inventory/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1049 2023-07-19 21:58:33.000000 hcs-cli-0.1.48/vhcs/cli/cmds/inventory/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      942 2023-07-19 21:58:43.000000 hcs-cli-0.1.48/vhcs/cli/cmds/inventory/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.127990 hcs-cli-0.1.48/vhcs/cli/cmds/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)      631 2023-06-27 19:52:37.000000 hcs-cli-0.1.48/vhcs/cli/cmds/lcm/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.133658 hcs-cli-0.1.48/vhcs/cli/cmds/lcm/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.48/vhcs/cli/cmds/lcm/provider/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      801 2023-06-23 02:35:21.000000 hcs-cli-0.1.48/vhcs/cli/cmds/lcm/provider/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      792 2023-06-23 02:35:30.000000 hcs-cli-0.1.48/vhcs/cli/cmds/lcm/provider/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      971 2023-07-19 21:58:53.000000 hcs-cli-0.1.48/vhcs/cli/cmds/lcm/provider/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.140554 hcs-cli-0.1.48/vhcs/cli/cmds/lcm/template/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.48/vhcs/cli/cmds/lcm/template/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1992 2023-07-19 22:34:00.000000 hcs-cli-0.1.48/vhcs/cli/cmds/lcm/template/create.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1063 2023-07-19 21:59:46.000000 hcs-cli-0.1.48/vhcs/cli/cmds/lcm/template/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      840 2023-06-23 02:37:07.000000 hcs-cli-0.1.48/vhcs/cli/cmds/lcm/template/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1572 2023-07-19 21:59:58.000000 hcs-cli-0.1.48/vhcs/cli/cmds/lcm/template/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-07-19 22:32:52.000000 hcs-cli-0.1.48/vhcs/cli/cmds/lcm/template/wait.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6922 2023-07-06 00:55:04.000000 hcs-cli-0.1.48/vhcs/cli/cmds/login.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.011717 hcs-cli-0.1.48/vhcs/cli/cmds/org/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.142536 hcs-cli-0.1.48/vhcs/cli/cmds/org/datacenter/
+-rw-r--r--   0 nanw       (501) staff       (20)      848 2023-06-30 15:40:06.000000 hcs-cli-0.1.48/vhcs/cli/cmds/org/datacenter/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      981 2023-07-19 22:00:09.000000 hcs-cli-0.1.48/vhcs/cli/cmds/org/datacenter/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.144313 hcs-cli-0.1.48/vhcs/cli/cmds/org/detail/
+-rw-r--r--   0 nanw       (501) staff       (20)      890 2023-07-19 22:00:19.000000 hcs-cli-0.1.48/vhcs/cli/cmds/org/detail/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1201 2023-06-30 15:40:25.000000 hcs-cli-0.1.48/vhcs/cli/cmds/org/detail/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.149324 hcs-cli-0.1.48/vhcs/cli/cmds/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)      631 2023-06-13 19:45:45.000000 hcs-cli-0.1.48/vhcs/cli/cmds/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1139 2023-07-19 22:02:33.000000 hcs-cli-0.1.48/vhcs/cli/cmds/pki/delete_org_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      890 2023-07-19 22:02:33.000000 hcs-cli-0.1.48/vhcs/cli/cmds/pki/get_org_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      775 2023-06-30 15:38:40.000000 hcs-cli-0.1.48/vhcs/cli/cmds/pki/get_root_ca.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1788 2023-07-19 22:02:33.000000 hcs-cli-0.1.48/vhcs/cli/cmds/pki/sign_resource_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      726 2023-06-30 15:38:40.000000 hcs-cli-0.1.48/vhcs/cli/cmds/pki/test.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.153260 hcs-cli-0.1.48/vhcs/cli/cmds/plan/
+-rw-r--r--   0 nanw       (501) staff       (20)      665 2023-06-28 17:52:44.000000 hcs-cli-0.1.48/vhcs/cli/cmds/plan/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2744 2023-07-30 23:31:00.000000 hcs-cli-0.1.48/vhcs/cli/cmds/plan/deploy.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2273 2023-07-30 23:31:29.000000 hcs-cli-0.1.48/vhcs/cli/cmds/plan/destroy.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2113 2023-07-30 23:23:45.000000 hcs-cli-0.1.48/vhcs/cli/cmds/plan/graph.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.154875 hcs-cli-0.1.48/vhcs/cli/cmds/portal/
+-rw-r--r--   0 nanw       (501) staff       (20)      634 2023-07-10 08:01:20.000000 hcs-cli-0.1.48/vhcs/cli/cmds/portal/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.159183 hcs-cli-0.1.48/vhcs/cli/cmds/portal/entitlement/
+-rw-r--r--   0 nanw       (501) staff       (20)      624 2023-07-11 03:23:55.000000 hcs-cli-0.1.48/vhcs/cli/cmds/portal/entitlement/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      926 2023-07-19 22:02:34.000000 hcs-cli-0.1.48/vhcs/cli/cmds/portal/entitlement/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      953 2023-07-24 21:35:27.000000 hcs-cli-0.1.48/vhcs/cli/cmds/portal/entitlement/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      862 2023-07-24 21:32:49.000000 hcs-cli-0.1.48/vhcs/cli/cmds/portal/entitlement/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.163090 hcs-cli-0.1.48/vhcs/cli/cmds/portal/pool/
+-rw-r--r--   0 nanw       (501) staff       (20)      624 2023-07-10 08:01:44.000000 hcs-cli-0.1.48/vhcs/cli/cmds/portal/pool/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      915 2023-07-19 22:02:34.000000 hcs-cli-0.1.48/vhcs/cli/cmds/portal/pool/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      940 2023-07-19 22:02:34.000000 hcs-cli-0.1.48/vhcs/cli/cmds/portal/pool/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      931 2023-07-24 21:37:06.000000 hcs-cli-0.1.48/vhcs/cli/cmds/portal/pool/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.170931 hcs-cli-0.1.48/vhcs/cli/cmds/portal/site/
+-rw-r--r--   0 nanw       (501) staff       (20)      624 2023-07-11 20:43:14.000000 hcs-cli-0.1.48/vhcs/cli/cmds/portal/site/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1108 2023-07-19 22:02:33.000000 hcs-cli-0.1.48/vhcs/cli/cmds/portal/site/create.py
+-rw-r--r--   0 nanw       (501) staff       (20)      912 2023-07-19 22:02:33.000000 hcs-cli-0.1.48/vhcs/cli/cmds/portal/site/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      934 2023-07-19 22:02:33.000000 hcs-cli-0.1.48/vhcs/cli/cmds/portal/site/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      837 2023-07-21 18:40:45.000000 hcs-cli-0.1.48/vhcs/cli/cmds/portal/site/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1022 2023-07-21 18:42:53.000000 hcs-cli-0.1.48/vhcs/cli/cmds/portal/site/set-edge.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.173005 hcs-cli-0.1.48/vhcs/cli/cmds/profile/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.48/vhcs/cli/cmds/profile/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1765 2023-07-05 06:16:00.000000 hcs-cli-0.1.48/vhcs/cli/cmds/profile/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)      932 2023-06-13 19:40:36.000000 hcs-cli-0.1.48/vhcs/cli/cmds/upgrade.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.174016 hcs-cli-0.1.48/vhcs/cli/cmds/vmhub/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-13 19:40:36.000000 hcs-cli-0.1.48/vhcs/cli/cmds/vmhub/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.177160 hcs-cli-0.1.48/vhcs/cli/cmds/vmhub/otp/
+-rw-r--r--   0 nanw       (501) staff       (20)      643 2023-06-29 21:49:43.000000 hcs-cli-0.1.48/vhcs/cli/cmds/vmhub/otp/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1234 2023-06-29 21:49:20.000000 hcs-cli-0.1.48/vhcs/cli/cmds/vmhub/otp/redeem.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1127 2023-07-19 22:02:33.000000 hcs-cli-0.1.48/vhcs/cli/cmds/vmhub/otp/request.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)     2865 2023-06-23 02:40:39.000000 hcs-cli-0.1.48/vhcs/cli/main.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.182558 hcs-cli-0.1.48/vhcs/common/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-07-27 01:24:59.000000 hcs-cli-0.1.48/vhcs/common/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.195508 hcs-cli-0.1.48/vhcs/common/ctxp/
+-rw-r--r--   0 nanw       (501) staff       (20)     1538 2023-07-03 20:20:16.000000 hcs-cli-0.1.48/vhcs/common/ctxp/README.md
+-rw-r--r--   0 nanw       (501) staff       (20)      790 2023-07-03 20:45:37.000000 hcs-cli-0.1.48/vhcs/common/ctxp/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1155 2023-07-03 21:18:13.000000 hcs-cli-0.1.48/vhcs/common/ctxp/_init.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.197594 hcs-cli-0.1.48/vhcs/common/ctxp/built_in_cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.48/vhcs/common/ctxp/built_in_cmds/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2421 2023-06-21 17:26:56.000000 hcs-cli-0.1.48/vhcs/common/ctxp/built_in_cmds/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3989 2023-07-05 23:22:13.000000 hcs-cli-0.1.48/vhcs/common/ctxp/built_in_cmds/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5129 2023-07-05 06:22:51.000000 hcs-cli-0.1.48/vhcs/common/ctxp/cli_processor.py
+-rw-r--r--   0 nanw       (501) staff       (20)      936 2023-07-03 21:17:12.000000 hcs-cli-0.1.48/vhcs/common/ctxp/config.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1205 2023-07-03 21:08:50.000000 hcs-cli-0.1.48/vhcs/common/ctxp/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6467 2023-06-23 00:26:19.000000 hcs-cli-0.1.48/vhcs/common/ctxp/fstore.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1200 2023-06-13 19:40:36.000000 hcs-cli-0.1.48/vhcs/common/ctxp/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3060 2023-07-11 23:13:07.000000 hcs-cli-0.1.48/vhcs/common/ctxp/jsondot.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5526 2023-07-11 08:29:40.000000 hcs-cli-0.1.48/vhcs/common/ctxp/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1565 2023-07-05 06:52:28.000000 hcs-cli-0.1.48/vhcs/common/ctxp/profile_store.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1604 2023-07-03 22:06:25.000000 hcs-cli-0.1.48/vhcs/common/ctxp/state.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6919 2023-07-28 02:46:20.000000 hcs-cli-0.1.48/vhcs/common/ctxp/util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3256 2023-06-13 19:40:36.000000 hcs-cli-0.1.48/vhcs/common/ctxp/var_template.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2859 2023-07-27 01:21:30.000000 hcs-cli-0.1.48/vhcs/common/duration.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7606 2023-07-29 14:44:11.000000 hcs-cli-0.1.48/vhcs/common/job_view.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6329 2023-07-13 00:38:57.000000 hcs-cli-0.1.48/vhcs/common/logger.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.203191 hcs-cli-0.1.48/vhcs/common/sglib/
+-rw-r--r--   0 nanw       (501) staff       (20)      654 2023-06-13 19:40:36.000000 hcs-cli-0.1.48/vhcs/common/sglib/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4648 2023-07-07 17:06:56.000000 hcs-cli-0.1.48/vhcs/common/sglib/auth.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1808 2023-07-19 22:44:47.000000 hcs-cli-0.1.48/vhcs/common/sglib/cli_options.py
+-rw-r--r--   0 nanw       (501) staff       (20)     8079 2023-07-05 07:42:49.000000 hcs-cli-0.1.48/vhcs/common/sglib/csp.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5200 2023-07-18 18:53:18.000000 hcs-cli-0.1.48/vhcs/common/sglib/ez_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)      906 2023-07-07 17:01:14.000000 hcs-cli-0.1.48/vhcs/common/sglib/hcs_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)     8243 2023-07-05 08:11:32.000000 hcs-cli-0.1.48/vhcs/common/sglib/login_support.py
+-rw-r--r--   0 nanw       (501) staff       (20)      600 2023-07-19 22:16:46.000000 hcs-cli-0.1.48/vhcs/common/sglib/util.py
+-rw-r--r--   0 nanw       (501) staff       (20)    10097 2023-07-29 00:16:03.000000 hcs-cli-0.1.48/vhcs/common/util.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.204928 hcs-cli-0.1.48/vhcs/config/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.48/vhcs/config/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7771 2023-07-03 22:19:24.000000 hcs-cli-0.1.48/vhcs/config/hcs-deployments.yaml
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.212051 hcs-cli-0.1.48/vhcs/plan/
+-rw-r--r--   0 nanw       (501) staff       (20)      175 2023-07-27 17:24:35.000000 hcs-cli-0.1.48/vhcs/plan/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      125 2023-07-27 23:00:30.000000 hcs-cli-0.1.48/vhcs/plan/actions.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1299 2023-07-27 22:49:14.000000 hcs-cli-0.1.48/vhcs/plan/base_provider.py
+-rw-r--r--   0 nanw       (501) staff       (20)      113 2023-07-25 17:15:18.000000 hcs-cli-0.1.48/vhcs/plan/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)    16672 2023-07-31 01:09:30.000000 hcs-cli-0.1.48/vhcs/plan/core.py
+-rw-r--r--   0 nanw       (501) staff       (20)    10264 2023-07-30 23:25:14.000000 hcs-cli-0.1.48/vhcs/plan/dag.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6037 2023-07-30 19:15:09.000000 hcs-cli-0.1.48/vhcs/plan/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5804 2023-07-31 00:03:11.000000 hcs-cli-0.1.48/vhcs/plan/kop.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.212823 hcs-cli-0.1.48/vhcs/plan/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-28 17:25:18.000000 hcs-cli-0.1.48/vhcs/plan/provider/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.223219 hcs-cli-0.1.48/vhcs/plan/provider/azure/
+-rw-r--r--   0 nanw       (501) staff       (20)      166 2023-07-28 23:53:29.000000 hcs-cli-0.1.48/vhcs/plan/provider/azure/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7207 2023-07-29 05:50:22.000000 hcs-cli-0.1.48/vhcs/plan/provider/azure/_az_facade.py
+-rw-r--r--   0 nanw       (501) staff       (20)      650 2023-07-30 23:35:50.000000 hcs-cli-0.1.48/vhcs/plan/provider/azure/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1569 2023-07-29 15:07:09.000000 hcs-cli-0.1.48/vhcs/plan/provider/azure/aad_group.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2217 2023-07-29 15:07:18.000000 hcs-cli-0.1.48/vhcs/plan/provider/azure/aad_user.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1418 2023-07-29 15:07:24.000000 hcs-cli-0.1.48/vhcs/plan/provider/azure/nat_gateway.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1564 2023-07-29 15:07:29.000000 hcs-cli-0.1.48/vhcs/plan/provider/azure/nsg.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1628 2023-07-29 15:07:34.000000 hcs-cli-0.1.48/vhcs/plan/provider/azure/public_ip.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1511 2023-07-31 00:16:15.000000 hcs-cli-0.1.48/vhcs/plan/provider/azure/resource_group.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1962 2023-07-29 15:07:44.000000 hcs-cli-0.1.48/vhcs/plan/provider/azure/subnet.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1569 2023-07-29 15:07:48.000000 hcs-cli-0.1.48/vhcs/plan/provider/azure/virtual_network.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.226370 hcs-cli-0.1.48/vhcs/plan/provider/dev/
+-rw-r--r--   0 nanw       (501) staff       (20)       29 2023-07-05 15:12:02.000000 hcs-cli-0.1.48/vhcs/plan/provider/dev/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)       33 2023-07-05 15:12:02.000000 hcs-cli-0.1.48/vhcs/plan/provider/dev/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1695 2023-07-29 15:07:54.000000 hcs-cli-0.1.48/vhcs/plan/provider/dev/dummy.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.242772 hcs-cli-0.1.48/vhcs/plan/provider/hcs/
+-rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-29 23:41:13.000000 hcs-cli-0.1.48/vhcs/plan/provider/hcs/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)       33 2023-06-29 23:41:19.000000 hcs-cli-0.1.48/vhcs/plan/provider/hcs/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1493 2023-07-29 15:07:59.000000 hcs-cli-0.1.48/vhcs/plan/provider/hcs/ad.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3857 2023-07-29 15:08:03.000000 hcs-cli-0.1.48/vhcs/plan/provider/hcs/edge.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1317 2023-07-29 15:08:08.000000 hcs-cli-0.1.48/vhcs/plan/provider/hcs/entitlement.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1405 2023-07-29 15:08:12.000000 hcs-cli-0.1.48/vhcs/plan/provider/hcs/identity_provider.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3515 2023-07-29 15:08:15.000000 hcs-cli-0.1.48/vhcs/plan/provider/hcs/image.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1598 2023-07-29 15:08:19.000000 hcs-cli-0.1.48/vhcs/plan/provider/hcs/launch_item.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1527 2023-07-29 15:08:23.000000 hcs-cli-0.1.48/vhcs/plan/provider/hcs/pool_group.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2044 2023-07-29 15:08:26.000000 hcs-cli-0.1.48/vhcs/plan/provider/hcs/pool_template.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1646 2023-07-29 15:08:30.000000 hcs-cli-0.1.48/vhcs/plan/provider/hcs/provider.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1405 2023-07-29 15:08:34.000000 hcs-cli-0.1.48/vhcs/plan/provider/hcs/site.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2003 2023-07-29 15:08:37.000000 hcs-cli-0.1.48/vhcs/plan/provider/hcs/uag.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.244284 hcs-cli-0.1.48/vhcs/service/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.48/vhcs/service/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6989 2023-07-28 20:25:17.000000 hcs-cli-0.1.48/vhcs/service/_util.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.250053 hcs-cli-0.1.48/vhcs/service/admin/
+-rw-r--r--   0 nanw       (501) staff       (20)       68 2023-07-24 16:34:10.000000 hcs-cli-0.1.48/vhcs/service/admin/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      853 2023-07-24 16:32:50.000000 hcs-cli-0.1.48/vhcs/service/admin/ad.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1211 2023-07-06 14:56:48.000000 hcs-cli-0.1.48/vhcs/service/admin/azure_infra.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3997 2023-07-28 20:25:54.000000 hcs-cli-0.1.48/vhcs/service/admin/edge.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1082 2023-07-24 17:45:25.000000 hcs-cli-0.1.48/vhcs/service/admin/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1459 2023-07-18 19:54:38.000000 hcs-cli-0.1.48/vhcs/service/admin/provider.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2106 2023-07-26 19:27:04.000000 hcs-cli-0.1.48/vhcs/service/admin/template.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2458 2023-07-26 04:28:07.000000 hcs-cli-0.1.48/vhcs/service/admin/uag.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.251636 hcs-cli-0.1.48/vhcs/service/auth/
+-rw-r--r--   0 nanw       (501) staff       (20)       19 2023-06-22 18:49:46.000000 hcs-cli-0.1.48/vhcs/service/auth/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      879 2023-07-24 17:10:24.000000 hcs-cli-0.1.48/vhcs/service/auth/admin.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.254807 hcs-cli-0.1.48/vhcs/service/ims/
+-rw-r--r--   0 nanw       (501) staff       (20)       71 2023-07-18 21:11:37.000000 hcs-cli-0.1.48/vhcs/service/ims/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2383 2023-07-28 19:05:05.000000 hcs-cli-0.1.48/vhcs/service/ims/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)      944 2023-07-19 21:57:09.000000 hcs-cli-0.1.48/vhcs/service/ims/image_copies.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2083 2023-07-26 17:02:49.000000 hcs-cli-0.1.48/vhcs/service/ims/images.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3307 2023-07-26 04:28:49.000000 hcs-cli-0.1.48/vhcs/service/ims/version.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.256142 hcs-cli-0.1.48/vhcs/service/inventory/
+-rw-r--r--   0 nanw       (501) staff       (20)       25 2023-07-08 00:42:34.000000 hcs-cli-0.1.48/vhcs/service/inventory/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1290 2023-07-08 00:32:38.000000 hcs-cli-0.1.48/vhcs/service/inventory/vm.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.258153 hcs-cli-0.1.48/vhcs/service/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)       32 2023-06-22 18:49:27.000000 hcs-cli-0.1.48/vhcs/service/lcm/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1437 2023-06-22 18:48:08.000000 hcs-cli-0.1.48/vhcs/service/lcm/provider.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2755 2023-07-21 02:58:07.000000 hcs-cli-0.1.48/vhcs/service/lcm/template.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.260550 hcs-cli-0.1.48/vhcs/service/org_service/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:38:56.000000 hcs-cli-0.1.48/vhcs/service/org_service/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1083 2023-06-30 15:37:59.000000 hcs-cli-0.1.48/vhcs/service/org_service/datacenter.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1040 2023-06-30 15:37:42.000000 hcs-cli-0.1.48/vhcs/service/org_service/details.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.262317 hcs-cli-0.1.48/vhcs/service/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:38:50.000000 hcs-cli-0.1.48/vhcs/service/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1211 2023-06-30 15:38:16.000000 hcs-cli-0.1.48/vhcs/service/pki/certificate.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.265548 hcs-cli-0.1.48/vhcs/service/portal/
+-rw-r--r--   0 nanw       (501) staff       (20)       37 2023-07-11 20:44:21.000000 hcs-cli-0.1.48/vhcs/service/portal/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      942 2023-07-24 21:34:40.000000 hcs-cli-0.1.48/vhcs/service/portal/entitlement.py
+-rw-r--r--   0 nanw       (501) staff       (20)      929 2023-07-24 21:37:58.000000 hcs-cli-0.1.48/vhcs/service/portal/pool.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1493 2023-07-21 18:45:40.000000 hcs-cli-0.1.48/vhcs/service/portal/site.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.267440 hcs-cli-0.1.48/vhcs/service/vmhub/
+-rw-r--r--   0 nanw       (501) staff       (20)       17 2023-07-03 19:03:42.000000 hcs-cli-0.1.48/vhcs/service/vmhub/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1406 2023-06-29 21:48:05.000000 hcs-cli-0.1.48/vhcs/service/vmhub/otp.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.270277 hcs-cli-0.1.48/vhcs/support/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:35:24.000000 hcs-cli-0.1.48/vhcs/support/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.277938 hcs-cli-0.1.48/vhcs/support/daas/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-21 23:10:31.000000 hcs-cli-0.1.48/vhcs/support/daas/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1482 2023-07-13 00:23:42.000000 hcs-cli-0.1.48/vhcs/support/daas/cidr_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3840 2023-07-28 06:08:00.000000 hcs-cli-0.1.48/vhcs/support/daas/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1320 2023-07-28 06:07:21.000000 hcs-cli-0.1.48/vhcs/support/daas/infra.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4369 2023-07-29 06:18:32.000000 hcs-cli-0.1.48/vhcs/support/daas/infra_green.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4072 2023-07-28 15:37:09.000000 hcs-cli-0.1.48/vhcs/support/daas/infra_reuse.py
+-rw-r--r--   0 nanw       (501) staff       (20)      424 2023-07-11 23:57:51.000000 hcs-cli-0.1.48/vhcs/support/daas/template.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.030846 hcs-cli-0.1.48/vhcs/support/daas/templates/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.289034 hcs-cli-0.1.48/vhcs/support/daas/templates/v1/
+-rw-r--r--   0 nanw       (501) staff       (20)    14930 2023-07-30 19:46:33.000000 hcs-cli-0.1.48/vhcs/support/daas/templates/v1/infra-green.blueprint.yml
+-rw-r--r--   0 nanw       (501) staff       (20)      365 2023-07-29 05:52:51.000000 hcs-cli-0.1.48/vhcs/support/daas/templates/v1/infra-green.vars.yml
+-rw-r--r--   0 nanw       (501) staff       (20)    13147 2023-07-30 18:26:48.000000 hcs-cli-0.1.48/vhcs/support/daas/templates/v1/infra-reuse.blueprint.yml
+-rw-r--r--   0 nanw       (501) staff       (20)      518 2023-07-28 22:09:28.000000 hcs-cli-0.1.48/vhcs/support/daas/templates/v1/infra-reuse.vars.yml
+-rw-r--r--   0 nanw       (501) staff       (20)     3820 2023-07-31 01:07:28.000000 hcs-cli-0.1.48/vhcs/support/daas/templates/v1/tenant.blueprint.yml
+-rw-r--r--   0 nanw       (501) staff       (20)      143 2023-07-30 16:28:42.000000 hcs-cli-0.1.48/vhcs/support/daas/templates/v1/tenant.vars.yml
+-rw-r--r--   0 nanw       (501) staff       (20)     4684 2023-07-31 00:13:55.000000 hcs-cli-0.1.48/vhcs/support/daas/tenant_calc.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1455 2023-07-11 20:14:32.000000 hcs-cli-0.1.48/vhcs/support/plan_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2621 2023-07-05 07:42:08.000000 hcs-cli-0.1.48/vhcs/support/profile.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-31 01:12:46.293732 hcs-cli-0.1.48/vhcs/util/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.48/vhcs/util/__init__.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)     2535 2023-06-13 19:40:36.000000 hcs-cli-0.1.48/vhcs/util/check_license.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2759 2023-06-13 19:40:36.000000 hcs-cli-0.1.48/vhcs/util/duration.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5288 2023-06-13 19:40:36.000000 hcs-cli-0.1.48/vhcs/util/pki_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1929 2023-07-18 18:58:54.000000 hcs-cli-0.1.48/vhcs/util/query_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1725 2023-06-13 19:40:36.000000 hcs-cli-0.1.48/vhcs/util/versions.py
```

### Comparing `hcs-cli-0.1.47/.gitignore` & `hcs-cli-0.1.48/.gitignore`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/.vscode/launch.json` & `hcs-cli-0.1.48/.vscode/launch.json`

 * *Files 10% similar despite different names*

```diff
@@ -6,58 +6,48 @@
     "configurations": [
         {
             "name": "Python: Current File",
             "type": "python",
             "request": "launch",
             "program": "${file}",
             "console": "integratedTerminal",
-            "justMyCode": true
+            "justMyCode": false
         },
         {
             "name": "hcs login -di",
             "type": "python",
             "request": "launch",
             "program": "/usr/local/bin/hcs",
             "console": "integratedTerminal",
             "justMyCode": true,
             "cwd": "${workspaceFolder}/lab",
             "args" : ["login", "-di"]
         },
         {
-            "name": "hcs tenant plan",
+            "name": "tenant plan",
             "type": "python",
             "request": "launch",
             "program": "/usr/local/bin/hcs",
             "console": "integratedTerminal",
             "justMyCode": true,
             "cwd": "${workspaceFolder}/lab",
             "args" : ["daas", "tenant", "plan", "nanw",]
         },
         {
-            "name": "hcs daas infra plan",
+            "name": "infra plan",
             "type": "python",
             "request": "launch",
             "program": "/usr/local/bin/hcs",
             "console": "integratedTerminal",
             "justMyCode": false,
             "cwd": "${workspaceFolder}/lab",
-            "args" : ["daas", "infra", "plan", "westus2"]
+            "args" : ["daas", "infra", "plan", "block1"]
         },
         {
-            "name": "hcs plan deploy",
-            "type": "python",
-            "request": "launch",
-            "program": "/usr/local/bin/hcs",
-            "console": "integratedTerminal",
-            "justMyCode": true,
-            "cwd": "${workspaceFolder}/lab",
-            "args" : ["plan", "deploy", "-f", "infra.plan.yml", "--sequential"]
-        },
-        {
-            "name": "hcs destroy",
+            "name": "plan destroy",
             "type": "python",
             "request": "launch",
             "program": "/usr/local/bin/hcs",
             "console": "integratedTerminal",
             "justMyCode": true,
             "cwd": "${workspaceFolder}/lab",
             "args" : ["plan", "destroy", "-f", "nanw.plan.yml"]
@@ -66,51 +56,41 @@
             "name": "plan deploy",
             "type": "python",
             "request": "launch",
             "program": "/usr/local/bin/hcs",
             "console": "integratedTerminal",
             "justMyCode": false,
             "cwd": "${workspaceFolder}/lab",
-            "args" : ["plan", "deploy", "-f", "infra.plan.yml", "-r", "myImageMultiSession"]
+            "args" : ["plan", "deploy", "-f", "starter.plan.yml", "--sequential"]
         },
         {
-            "name": "plan destroy",
+            "name": "UT",
             "type": "python",
             "request": "launch",
-            "program": "/usr/local/bin/hcs",
+            "program": "/usr/local/bin/python3",
             "console": "integratedTerminal",
             "justMyCode": false,
-            "cwd": "${workspaceFolder}/lab",
-            "args" : ["plan", "destroy", "-f", "infra.plan.yml", "-r", "myImage", "--sequential"]
+            "cwd": "${workspaceFolder}/tests",
+            "args" : ["-m", "unittest", "vhcs.cli.cmds.plan.test_plan.TestPlan", "-v", "--failfast"]
         },
         {
-            "name": "plan deploy -f t",
+            "name": "deploy t",
             "type": "python",
             "request": "launch",
             "program": "/usr/local/bin/hcs",
             "console": "integratedTerminal",
             "justMyCode": false,
             "cwd": "${workspaceFolder}/lab",
             "args" : ["plan", "deploy", "-f", "t.plan.yml"]
         },
         {
-            "name": "plan destroy -f t",
+            "name": "tmp",
             "type": "python",
             "request": "launch",
             "program": "/usr/local/bin/hcs",
             "console": "integratedTerminal",
             "justMyCode": false,
             "cwd": "${workspaceFolder}/lab",
-            "args" : ["plan", "destroy", "-f", "t.plan.yml"]
-        },
-        {
-            "name": "UT",
-            "type": "python",
-            "request": "launch",
-            "program": "/usr/local/bin/python3",
-            "console": "integratedTerminal",
-            "justMyCode": false,
-            "cwd": "${workspaceFolder}/tests",
-            "args" : ["-m", "unittest", "vhcs.cli.cmds.plan.test_plan.TestPlan", "-v", "--failfast"]
+            "args" : ["plan", "deploy", "-f", "t1.plan.yml", "--sequential"]
         },
     ]
 }
```

### Comparing `hcs-cli-0.1.47/CODE_OF_CONDUCT.md` & `hcs-cli-0.1.48/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/CONTRIBUTING_CLA.md` & `hcs-cli-0.1.48/CONTRIBUTING_CLA.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/GOVERNANCE.md` & `hcs-cli-0.1.48/GOVERNANCE.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/LICENSE` & `hcs-cli-0.1.48/LICENSE`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/Makefile` & `hcs-cli-0.1.48/Makefile`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/PKG-INFO` & `hcs-cli-0.1.48/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-cli
-Version: 0.1.47
+Version: 0.1.48
 Summary: Horizon Cloud Service CLI
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: Bug Tracker, https://github.com/vmware/horizon-cloud-service-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: changelog, https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md
@@ -18,27 +18,40 @@
 License-File: LICENSE
 License-File: NOTICE
 
 # horizon-cloud-service-cli
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue)](https://github.com/vmware-labs/compliance-dashboard-for-kubernetes/blob/main/LICENSE)
 
+- [horizon-cloud-service-cli](#horizon-cloud-service-cli)
+  - [Overview](#overview)
+  - [Try it out](#try-it-out)
+    - [Prerequisites](#prerequisites)
+    - [Installation](#installation)
+      - [Mac \& Linux](#mac--linux)
+  - [Authentication Methods](#authentication-methods)
+  - [Working with Development Environments](#working-with-development-environments)
+  - [Documentation](#documentation)
+  - [Contributing](#contributing)
+  - [License](#license)
+
+
 ## Overview
 Command line toolbox for [VMware Horizon Cloud Service (HCS) Next-Gen](https://www.vmware.com/products/horizon-cloud.html). It provides human-friendly operations based on HCS REST API.
 
 ## Try it out
 
 
 ### Prerequisites
 * Python 3.10+
 * Pip3
 
 Refer to [Setup Prerequisites](doc/dev-setup.md#setup-prerequisites) for more details.
 
-### Use the published version on PyPI
+### Installation
 
 #### Mac & Linux
 
 Install the tool
 ```
 pip3 install hcs-cli
 ```
```

### Comparing `hcs-cli-0.1.47/README.md` & `hcs-cli-0.1.48/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,37 @@
 # horizon-cloud-service-cli
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue)](https://github.com/vmware-labs/compliance-dashboard-for-kubernetes/blob/main/LICENSE)
 
+- [horizon-cloud-service-cli](#horizon-cloud-service-cli)
+  - [Overview](#overview)
+  - [Try it out](#try-it-out)
+    - [Prerequisites](#prerequisites)
+    - [Installation](#installation)
+      - [Mac \& Linux](#mac--linux)
+  - [Authentication Methods](#authentication-methods)
+  - [Working with Development Environments](#working-with-development-environments)
+  - [Documentation](#documentation)
+  - [Contributing](#contributing)
+  - [License](#license)
+
+
 ## Overview
 Command line toolbox for [VMware Horizon Cloud Service (HCS) Next-Gen](https://www.vmware.com/products/horizon-cloud.html). It provides human-friendly operations based on HCS REST API.
 
 ## Try it out
 
 
 ### Prerequisites
 * Python 3.10+
 * Pip3
 
 Refer to [Setup Prerequisites](doc/dev-setup.md#setup-prerequisites) for more details.
 
-### Use the published version on PyPI
+### Installation
 
 #### Mac & Linux
 
 Install the tool
 ```
 pip3 install hcs-cli
 ```
```

### Comparing `hcs-cli-0.1.47/doc/az-cheatsheet.md` & `hcs-cli-0.1.48/doc/az-cheatsheet.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/doc/dev-setup.md` & `hcs-cli-0.1.48/doc/dev-setup.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/doc/get-csp-user-api-token.md` & `hcs-cli-0.1.48/doc/get-csp-user-api-token.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/doc/hcs-cli-cheatsheet.md` & `hcs-cli-0.1.48/doc/hcs-cli-cheatsheet.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/doc/hcs-plan.md` & `hcs-cli-0.1.48/doc/hcs-plan.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/hcs_cli.egg-info/PKG-INFO` & `hcs-cli-0.1.48/hcs_cli.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-cli
-Version: 0.1.47
+Version: 0.1.48
 Summary: Horizon Cloud Service CLI
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: Bug Tracker, https://github.com/vmware/horizon-cloud-service-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: changelog, https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md
@@ -18,27 +18,40 @@
 License-File: LICENSE
 License-File: NOTICE
 
 # horizon-cloud-service-cli
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue)](https://github.com/vmware-labs/compliance-dashboard-for-kubernetes/blob/main/LICENSE)
 
+- [horizon-cloud-service-cli](#horizon-cloud-service-cli)
+  - [Overview](#overview)
+  - [Try it out](#try-it-out)
+    - [Prerequisites](#prerequisites)
+    - [Installation](#installation)
+      - [Mac \& Linux](#mac--linux)
+  - [Authentication Methods](#authentication-methods)
+  - [Working with Development Environments](#working-with-development-environments)
+  - [Documentation](#documentation)
+  - [Contributing](#contributing)
+  - [License](#license)
+
+
 ## Overview
 Command line toolbox for [VMware Horizon Cloud Service (HCS) Next-Gen](https://www.vmware.com/products/horizon-cloud.html). It provides human-friendly operations based on HCS REST API.
 
 ## Try it out
 
 
 ### Prerequisites
 * Python 3.10+
 * Pip3
 
 Refer to [Setup Prerequisites](doc/dev-setup.md#setup-prerequisites) for more details.
 
-### Use the published version on PyPI
+### Installation
 
 #### Mac & Linux
 
 Install the tool
 ```
 pip3 install hcs-cli
 ```
```

### Comparing `hcs-cli-0.1.47/hcs_cli.egg-info/SOURCES.txt` & `hcs-cli-0.1.48/hcs_cli.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -137,14 +137,15 @@
 vhcs/cli/cmds/profile/init.py
 vhcs/cli/cmds/vmhub/__init__.py
 vhcs/cli/cmds/vmhub/otp/__init__.py
 vhcs/cli/cmds/vmhub/otp/redeem.py
 vhcs/cli/cmds/vmhub/otp/request.py
 vhcs/common/__init__.py
 vhcs/common/duration.py
+vhcs/common/job_view.py
 vhcs/common/logger.py
 vhcs/common/util.py
 vhcs/common/ctxp/README.md
 vhcs/common/ctxp/__init__.py
 vhcs/common/ctxp/_init.py
 vhcs/common/ctxp/cli_processor.py
 vhcs/common/ctxp/config.py
@@ -168,28 +169,32 @@
 vhcs/common/sglib/hcs_client.py
 vhcs/common/sglib/login_support.py
 vhcs/common/sglib/util.py
 vhcs/config/__init__.py
 vhcs/config/hcs-deployments.yaml
 vhcs/plan/__init__.py
 vhcs/plan/actions.py
+vhcs/plan/base_provider.py
 vhcs/plan/context.py
 vhcs/plan/core.py
 vhcs/plan/dag.py
 vhcs/plan/helper.py
 vhcs/plan/kop.py
 vhcs/plan/provider/__init__.py
 vhcs/plan/provider/azure/__init__.py
 vhcs/plan/provider/azure/_az_facade.py
 vhcs/plan/provider/azure/_prepare.py
 vhcs/plan/provider/azure/aad_group.py
 vhcs/plan/provider/azure/aad_user.py
+vhcs/plan/provider/azure/nat_gateway.py
 vhcs/plan/provider/azure/nsg.py
+vhcs/plan/provider/azure/public_ip.py
 vhcs/plan/provider/azure/resource_group.py
 vhcs/plan/provider/azure/subnet.py
+vhcs/plan/provider/azure/virtual_network.py
 vhcs/plan/provider/dev/__init__.py
 vhcs/plan/provider/dev/_prepare.py
 vhcs/plan/provider/dev/dummy.py
 vhcs/plan/provider/hcs/__init__.py
 vhcs/plan/provider/hcs/_prepare.py
 vhcs/plan/provider/hcs/ad.py
 vhcs/plan/provider/hcs/edge.py
@@ -238,19 +243,22 @@
 vhcs/support/__init__.py
 vhcs/support/plan_util.py
 vhcs/support/profile.py
 vhcs/support/daas/__init__.py
 vhcs/support/daas/cidr_util.py
 vhcs/support/daas/helper.py
 vhcs/support/daas/infra.py
-vhcs/support/daas/infra_calc.py
+vhcs/support/daas/infra_green.py
+vhcs/support/daas/infra_reuse.py
 vhcs/support/daas/template.py
 vhcs/support/daas/tenant_calc.py
-vhcs/support/daas/templates/v1/infra.blueprint.yml
-vhcs/support/daas/templates/v1/infra.vars.yml
+vhcs/support/daas/templates/v1/infra-green.blueprint.yml
+vhcs/support/daas/templates/v1/infra-green.vars.yml
+vhcs/support/daas/templates/v1/infra-reuse.blueprint.yml
+vhcs/support/daas/templates/v1/infra-reuse.vars.yml
 vhcs/support/daas/templates/v1/tenant.blueprint.yml
 vhcs/support/daas/templates/v1/tenant.vars.yml
 vhcs/util/__init__.py
 vhcs/util/check_license.py
 vhcs/util/duration.py
 vhcs/util/pki_util.py
 vhcs/util/query_util.py
```

### Comparing `hcs-cli-0.1.47/payload/lcm/zero.json` & `hcs-cli-0.1.48/payload/lcm/zero.json`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/pyproject.toml` & `hcs-cli-0.1.48/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/setup.py` & `hcs-cli-0.1.48/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from setuptools_scm import get_version
 import os
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
-VERSION = "0.1.47"
+VERSION = "0.1.48"
 
 
 def get_version():
     version = VERSION
     local_version = os.environ.get("SCM_REV")
     if local_version:
         version += "+" + local_version
```

### Comparing `hcs-cli-0.1.47/tests/conftest.py` & `hcs-cli-0.1.48/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/tests/test_utils.py` & `hcs-cli-0.1.48/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/tests/vhcs/cli/cmds/pki/get_root_ca.py` & `hcs-cli-0.1.48/tests/vhcs/cli/cmds/pki/get_root_ca.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/tests/vhcs/cli/cmds/test_context.py` & `hcs-cli-0.1.48/tests/vhcs/cli/cmds/test_context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/tests/vhcs/cli/cmds/test_login.py` & `hcs-cli-0.1.48/tests/vhcs/cli/cmds/test_login.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/tests/vhcs/cli/cmds/test_profile.py` & `hcs-cli-0.1.48/tests/vhcs/cli/cmds/test_profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/__main__.py` & `hcs-cli-0.1.48/vhcs/__main__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/admin/__init__.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/admin/ad/__init__.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/admin/ad/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/admin/ad/delete.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/admin/ad/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/admin/ad/get.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/admin/ad/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/admin/ad/list.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/admin/ad/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/admin/azure-infra/main.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/admin/azure-infra/main.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/admin/edge/__init__.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/admin/edge/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/admin/edge/delete.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/admin/edge/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/admin/edge/get.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/admin/edge/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/admin/edge/list.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/admin/edge/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/admin/provider/create.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/admin/provider/create.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/admin/provider/delete.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/admin/provider/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/admin/provider/get.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/admin/provider/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/admin/provider/list.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/admin/provider/list.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import vhcs.common.sglib.cli_options as cli
 
 
 @click.command()
 @cli.org_id
 @cli.limit
 @cli.sort
-@click.option("--search", type=str, required=False, help="Search expression. E.g. --search 'name $eq myProvider1'")
+@cli.search
 @click.option(
     "--label", 
     type=click.Choice(["azure", "vsphere"]),
     required=False, 
     default="azure", 
     help="Specify the provider label")
 def list(org: str, label: str, **kwargs):
```

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/admin/template/__init__.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/admin/template/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/admin/template/delete.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/admin/template/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/admin/template/get.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/admin/template/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/admin/template/list.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/admin/template/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/admin/template/vm/__init__.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/admin/template/vm/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/admin/template/vm/get.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/admin/template/vm/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/admin/template/vm/list.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/admin/template/vm/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/admin/uag/__init__.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/admin/uag/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/admin/uag/delete.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/admin/uag/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/admin/uag/get.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/admin/uag/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/admin/uag/list.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/admin/uag/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/auth/__init__.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/auth/admin/__init__.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/auth/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/auth/admin/get_org_idp_map.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/auth/admin/get_org_idp_map.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/daas/__init__.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/daas/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/daas/infra/__init__.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/daas/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/daas/infra/basic.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/daas/infra/basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import click
 import vhcs.common.ctxp as ctxp
 from vhcs.support.daas import infra
 
 @click.command()
 def get():
     """Get the shared infrastructure config."""
-    return infra.all()
+    return infra.get()
 
 @click.command()
 def file():
     """Get the infrastructure config file path."""
     return infra.file()
 
 @click.command()
```

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/daas/infra/plan.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/daas/infra/plan.py`

 * *Files 27% similar despite different names*

```diff
@@ -20,32 +20,78 @@
 from vhcs.support.daas import infra
 from vhcs.service import admin
 from vhcs.support.daas import infra, helper, cidr_util
 
 file_name = '.plan.yml'
 
 @click.command()
-@click.argument("name", type=str, required=True)
-def plan(name: str):
+def plan():
     """Interactive setup for shared infrastructure."""
 
+    name = click.prompt("Name of the infrastructure", default="starter")
+    modes = ['Create default infrastructure (automatic)', 'Reuse existing infrastructure (manual)']
+    mode = choose("Name of the infrastructure:", modes, selected=modes[0])
+
+    if mode == modes[0]:
+        _create_default_infra(name)
+    else:
+        _reuse_existing_infra(name)
+    
+def _create_default_infra(name):
     def collect_information(data):
         vars = data['vars']
         org_id = vars['orgId']
+        _select_region(vars)
         _select_provider(vars, org_id)
+        _select_managed_identity(vars)
+        _input_vnet_cidr(vars['network'])
+        _config_desktop_defaults(vars['desktop'])
+        infra.set(data)
+
+    return helper.prepare_plan_file(name, 'v1/infra-green.blueprint.yml', collect_information)
+
+def _reuse_existing_infra(name):
+    def collect_information(data):
+        vars = data['vars']
+        org_id = vars['orgId']
+        _select_region(vars)
+        _select_provider(vars, org_id)
+        _select_managed_identity(vars)
         _select_vnet(vars['network'])
         _config_desktop_defaults(vars['desktop'])
-        infra.save(data)
+        infra.set(data)
 
-    return helper.prepare_plan_file(name, 'v1/infra.blueprint.yml', collect_information)
+    return helper.prepare_plan_file(name, 'v1/infra-reuse.blueprint.yml', collect_information)
 
-    
+def _input_vnet_cidr(network):
+    cidr = click.prompt("vNet CIDR (/16):", default=network['cidr'] or "10.0.0.0/16")
+    network['cidr'] = cidr
+
+def _select_region(vars):
+    locations = az.locations()
+    selected = None
+    for l in locations:
+        if l['name'] == 'eastus':
+            selected = l
+            break
+    fn_get_text = lambda l: l['regionalDisplayName'] + f" ({l['name']})"
+    region = choose("Select location:", locations, fn_get_text, selected)
+    vars['region'] = region['name']
+
+def _select_managed_identity(vars):
+    identities = list(az.managed_identity_client().user_assigned_identities.list_by_subscription())
+    fn_get_text = lambda i: i.name
+    selected = choose("Select managed identity:", identities, fn_get_text)
+    vars['edge']['managedIdentityId'] = selected.id
 
-def _select_provider(vars, org_id):
+def _select_provider(vars: dict, org_id: str):
     providers = admin.provider.list('azure', org_id)
+    region = vars['region']
+    filter_by_region = lambda p: p['providerDetails']['data']['region'] == region
+    providers = list(filter(filter_by_region, providers))
     if providers:
         def _is_create_new(p):
             return isinstance(p, str)
 
         def fn_provider_text(p):
             if _is_create_new(p):
                 return p
@@ -53,17 +99,21 @@
 
         providers.append("<Create New Provider>")
         p = choose("Select region and provider", providers, fn_provider_text)
         if not p:
             return
         if not _is_create_new(p):
             vars['provider']['id'] = p['id']
+            subscription_id = p['providerDetails']['data']['subscriptionId']
+            vars['provider']['subscriptionId'] = subscription_id
+            del vars['newProvider']
+            az.set_subscription(subscription_id)
             return p
     else:
-        click.echo("No provider configured. Need to create a new provider.")
+        click.echo(f"No provider configured for region {region}. Need to create a new provider.")
     _input_azure_sp(vars['newProvider'])
     
 
 def _input_azure_sp(data):
     data['subscriptionId'] = click.prompt("Azure subscription ID", default=data['subscriptionId'])
     data['region'] = click.prompt("Azure Region", default=data['region'])
     data['directoryId'] = click.prompt("Azure Directory ID", default=data['directoryId'])
```

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/daas/tenant/__init__.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/daas/tenant/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/daas/tenant/plan.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/daas/tenant/plan.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,72 +10,94 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-from vhcs.service import admin, ims
+from vhcs.service import admin, ims, portal
 from vhcs.common.ctxp import choose, util as cli_util
 from vhcs.common.sglib.cli_options import get_org_id
 from vhcs.support.daas import infra, helper
 
+_context = {}
 
 @click.command()
 @click.argument("name", type=str, required=True)
 def plan(name: str):
     """Interactive command to request a DaaS tenant"""
     return helper.prepare_plan_file(name, 'v1/tenant.blueprint.yml', _collect_info)
 
 def _collect_info(data):
     #_fill_info_from_infra()
     vars = data['vars']
+    _select_edge(vars)
     _config_desktop(vars)
     _input_user_emails(vars)
 
-def _config_desktop(data):
-    org_id = get_org_id(None)
-    def _select_image_and_vm_sku(data):
-        images = ims.helper.get_images_by_provider_instance_with_asset_details(data['provider']['id'], org_id)
+def _select_edge(vars):
+    org_id = vars['orgId']
+    edges = admin.edge.list(org_id)
+    titan_lite_infra = []
+    edge_id = vars['edgeId']
+    prev_selected = None
+    for s in edges:
+        name = s['name']
+        if name.startswith('titanlite-'):
+            titan_lite_infra.append(s)
+            if edge_id == s['id']:
+                prev_selected = s
+
+    fn_get_text = lambda s: f"{s['name']} ({s['hdc']['vmHub']['name']})"
+    selected_edge = choose("Select edge", titan_lite_infra, fn_get_text, prev_selected)
+    vars['edgeId'] = selected_edge['id']
+    _context['provider_instance_id'] = selected_edge['providerInstanceId']
+
+
+def _config_desktop(vars: dict):
+    org_id = vars['orgId']
+    def _select_image_and_vm_sku():
+        images = ims.helper.get_images_by_provider_instance_with_asset_details(_context['provider_instance_id'], org_id)
         fn_get_text = lambda d: f"{d['name']}: {d['description']}"
         prev_selected_image = None
-        if data['desktop']['streamId']:
+        if vars['desktop']['streamId']:
             for i in images:
-                if i['id'] == data['desktop']['streamId']:
+                if i['id'] == vars['desktop']['streamId']:
                     prev_selected_image = i
                     break
         selected_image = choose("Select image:", images, fn_get_text, selected=prev_selected_image)
-        data['desktop']['streamId'] = selected_image['id']
+        vars['desktop']['streamId'] = selected_image['id']
 
         fn_get_text = lambda m: f"{m['name']}"
         selected_marker = choose("Select marker:", selected_image['markers'], fn_get_text)
-        data['desktop']['markerId'] = selected_marker['id']
+        vars['desktop']['markerId'] = selected_marker['id']
 
         image_asset_details = selected_image['_assetDetails']['data']
 
-        search = f"capabilities.HyperVGenerations $in {image_asset_details['generationType']}"
-        vm_skus = admin.azure_infra.get_compute_vm_skus(data['provider']['id'], limit=200, search=search)
-        prev_selected_vm_sku = None
-        if data['desktop']['vmSkuName']:
-            selected_vm_sku_name = data['desktop']['vmSkuName']
-        else:
-            selected_vm_sku_name = image_asset_details['vmSize']
-        if selected_vm_sku_name:
-            for sku in vm_skus:
-                if sku['id'] == selected_vm_sku_name:
-                    prev_selected_vm_sku = sku
-                    break
-
-        fn_get_text = lambda d: f"{d['data']['name']} (CPU: {d['data']['capabilities']['vCPUs']}, RAM: {d['data']['capabilities']['MemoryGB']})"
-
-        selected = choose("Select VM size:", vm_skus, fn_get_text, selected=prev_selected_vm_sku)
-        data['desktop']['vmSkuName'] = selected['data']['name']
-
-    def _select_desktop_type(data):
-        types = ['MULTI_SESSION', 'FLOATING']
-        data['desktop']['templateType'] = choose("Desktop type:", types)
+        # search = f"capabilities.HyperVGenerations $in {image_asset_details['generationType']}"
+        # vm_skus = admin.azure_infra.get_compute_vm_skus(data['provider']['id'], limit=200, search=search)
+        # prev_selected_vm_sku = None
+        # if data['desktop']['vmSkuName']:
+        #     selected_vm_sku_name = data['desktop']['vmSkuName']
+        # else:
+        #     selected_vm_sku_name = image_asset_details['vmSize']
+        # if selected_vm_sku_name:
+        #     for sku in vm_skus:
+        #         if sku['id'] == selected_vm_sku_name:
+        #             prev_selected_vm_sku = sku
+        #             break
+
+        # fn_get_text = lambda d: f"{d['data']['name']} (CPU: {d['data']['capabilities']['vCPUs']}, RAM: {d['data']['capabilities']['MemoryGB']})"
+
+        # selected = choose("Select VM size:", vm_skus, fn_get_text, selected=prev_selected_vm_sku)
+        # data['desktop']['vmSkuName'] = selected['data']['name']
+        vars['desktop']['vmSkuName'] = image_asset_details['vmSize']
+
+    def _select_desktop_type():
+        types = ['FLOATING', 'MULTI_SESSION']
+        vars['desktop']['templateType'] = choose("Desktop type:", types)
 
-    _select_image_and_vm_sku(data)
-    _select_desktop_type(data)
+    _select_image_and_vm_sku()
+    _select_desktop_type()
 
 def _input_user_emails(data):
     data['userEmails'] = cli_util.input_array("User emails", default=data['userEmails'])
```

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/ims/__init__.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/ims/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/ims/delete.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/ims/delete.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 @click.argument("ids", type=str, required=True, nargs=-1)
 @cli.org_id
 @cli.wait
 def delete(ids: list[str], org: str, wait: str, **kwargs):
     """Delete an image by ID"""
 
     org_id = cli.get_org_id(org)
-    ims.helper.delete_image_and_versions(ids, org_id, wait)
+    ims.helper.delete_images(ids, org_id, wait)
```

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/ims/get.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/ims/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/ims/list.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/ims/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/ims/list_copies.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/ims/list_copies.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/ims/version/__init__.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/ims/version/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/ims/version/delete.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/ims/version/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/ims/version/get.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/ims/version/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/ims/version/list.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/ims/version/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/inventory/__init__.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/inventory/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/inventory/get.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/inventory/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/inventory/list.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/inventory/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/lcm/__init__.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/lcm/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/lcm/provider/__init__.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/lcm/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/lcm/provider/delete.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/lcm/provider/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/lcm/provider/get.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/lcm/provider/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/lcm/provider/list.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/lcm/provider/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/lcm/template/__init__.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/lcm/template/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/lcm/template/create.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/lcm/template/create.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/lcm/template/delete.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/lcm/template/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/lcm/template/get.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/lcm/template/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/lcm/template/list.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/lcm/template/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/lcm/template/wait.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/lcm/template/wait.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/login.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/login.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/org/datacenter/get.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/org/datacenter/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/org/datacenter/list.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/org/datacenter/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/org/detail/get.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/org/detail/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/org/detail/list.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/org/detail/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/pki/__init__.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/pki/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/pki/delete_org_cert.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/pki/delete_org_cert.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/pki/get_org_cert.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/pki/get_org_cert.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/pki/get_root_ca.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/pki/get_root_ca.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/pki/sign_resource_cert.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/pki/sign_resource_cert.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/pki/test.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/pki/test.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/plan/__init__.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/plan/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/plan/deploy.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/plan/deploy.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,33 +9,48 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
+import sys
 import click
 import vhcs.plan as plan
 import vhcs.support.plan_util as util
 from vhcs.common.ctxp.util import error_details
 
 @click.command()
 @click.option("--file", "-f", type=click.File("rt"), required=False, help="Specified the combined plan file.")
 @click.option("--resource", "-r", type=str, required=False, help="Specify a single resource in the plan to deploy. This includes deploying dependent resources.")
-@click.option("--include-related-resources/--single-resource-only", type=bool, default=True, required=False, help="Used with --resource. Specify whether to process related resources, or just the target resource.")
+@click.option("--include-dependencies/--single-resource-only", type=bool, default=False, required=False, help="Used with --resource. Specify whether to process related resources, or just the target resource.")
 @click.option("--parallel/--sequential", type=bool, default=True, required=False, help="Specify deployment mode, parallel or sequential.")
-def deploy(file, resource: str, include_related_resources: bool, parallel: bool):
+@click.option("--show-progress/--show-plain-log", type=bool, default=True, help="Control output format, interactive progress or plain logs.")
+def deploy(file, resource: str, include_dependencies: bool, parallel: bool, show_progress: bool):
 
     data, extra = util.load_plan(file)
     concurrency = 10 if parallel else 1
 
+    job_view = None
+    if show_progress and sys.stdout.isatty():
+        from vhcs.common.job_view import JobView
+        job_view = JobView.create_async()
+        plan.attach_job_view(job_view)
+        
     try:        
-        return plan.deploy(data, extra, resource, include_related_resources, concurrency)
+        return plan.deploy(data, 
+                           additional_context=extra, 
+                           target_resource_name=resource, 
+                           include_dependencies=include_dependencies, 
+                           concurrency=concurrency)
     except (FileNotFoundError, plan.PlanException, plan.PluginException) as e:
         return error_details(e), 1
+    finally:
+        if job_view:
+            job_view.close()
 
 # def _identify_files(file: list[str], name: str):
 #     if not file and not name:
 #         panic("Either --file or --name must be specified")
 #     if file and name:
 #         panic("--file and --name must not be specified together")
```

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/plan/destroy.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/plan/destroy.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,26 +9,38 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
+import sys
 import click
 import vhcs.plan as plan
 import vhcs.support.plan_util as util
 
 @click.command()
 @click.option("--file", "-f", type=click.File("rt"), required=False, help="Specified the combined plan file.")
 @click.option("--force/--fail-fast", type=bool, default=True, required=False, help="Force mode: try deleting everything and continue on error. Fail-fast mode: Stop on the first error.")
 @click.option("--resource", "-r", type=str, required=False, help="Specify a single resource in the plan to deploy.")
-@click.option("--include-related-resources/--single-resource-only", type=bool, default=False, required=False, help="Used with --resource. Specify whether to process related resources, or just the target resource.")
+@click.option("--include-dependencies/--single-resource-only", type=bool, default=False, required=False, help="Used with --resource. Specify whether to process related resources, or just the target resource.")
 @click.option("--parallel/--sequential", type=bool, default=True, required=False, help="Specify deployment mode, parallel or sequential.")
-def destroy(file, resource: str, include_related_resources: bool, parallel: bool, force: bool):
+@click.option("--show-progress/--show-plain-log", type=bool, default=True, help="Control output format, interactive progress or plain logs.")
+def destroy(file, force: bool, resource: str, include_dependencies: bool, parallel: bool, show_progress: bool):
 
     data, extra = util.load_plan(file)
     concurrency = 10 if parallel else 1
+
+    job_view = None
+    if show_progress and sys.stdout.isatty():
+        from vhcs.common.job_view import JobView
+        job_view = JobView.create_async()
+        plan.attach_job_view(job_view)
+
     try:
-        return plan.destroy(data, force, resource, include_related_resources, concurrency, extra)
+        return plan.destroy(data, force, resource, include_dependencies, concurrency, extra)
     except (FileNotFoundError, plan.PlanException, plan.PluginException) as e:
         return str(e), 1
+    finally:
+        if job_view:
+            job_view.close()
```

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/plan/graph.py` & `hcs-cli-0.1.48/vhcs/common/sglib/cli_options.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,32 +10,53 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import click
-import vhcs.plan as plan
-import vhcs.support.plan_util as util
+from vhcs.common.ctxp import CtxpException
 
-@click.command()
-@click.option("--file", "-f", type=click.File("rt"), required=False, help="Specified the combined plan file.")
-@click.option("--view/--output-only", "-v", type=bool, default=True, help="If view mode is specified, open browser to view the graph.")
-@click.option("--simplify/--full", "-v", type=bool, default=True, help="In simplified mode, show minimal edges. In full mode, show all edges.")
-def graph(file, view: bool, simplify: bool):
-    """Generate a graph view of the deployment, in Graphviz format."""
+org_id = click.option(
+    "--org",
+    type=str,
+    default=None,
+    required=False,
+    help="Specify org ID. If not specified, org ID from the current auth token will be used.",
+)
+wait = click.option(
+    "--wait", "-w",
+    type=str, 
+    required=False, 
+    default='10m', 
+    help="Wait time. E.g. '30s', or '5m'. Default: 10m. Specify '0' to disable waiting and return immediately."
+)
+search = click.option(
+    "--search", "-s",
+    type=str,
+    required=False,
+    help="Specify REST search. E.g. 'name $eq something'. Note: use single quote in bash/sh."
+)
+sort = click.option(
+    "--sort", 
+    type=str,
+    required=False,
+    help="Ascending/Descending. Format is property,{asc|desc} and default is ascending",
+)
+limit = click.option(
+    "--limit", 
+    type=int, 
+    required=False, 
+    default=20, 
+    help="Optionally, specify the number of records to fetch."
+)
 
-    try:
-        data, extra = util.load_plan(file)
-        g = plan.graph(data, extra, simplify)
-        if view:
-            _view_graph(g.source)
-        return g.source
-    except (FileNotFoundError, plan.PlanException, plan.PluginException) as e:
-        return str(e), 1
-    
+def get_org_id(org: str) -> str:
+    if org:
+        return org
 
-def _view_graph(src):
-    import urllib.parse
-    import webbrowser
-    url = 'https://dreampuf.github.io/GraphvizOnline/#' + urllib.parse.quote(src)
-    webbrowser.open(url, new=0, autoraise=True)
+    from vhcs.common.sglib import auth
+
+    auth_info = auth.details(False)
+    if not auth_info:
+        raise CtxpException("Not authorized. See 'hcs login --help'.")
+    return auth_info.org.id
```

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/portal/__init__.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/portal/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/portal/entitlement/__init__.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/portal/entitlement/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/portal/entitlement/delete.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/portal/entitlement/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/portal/entitlement/get.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/portal/entitlement/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/portal/entitlement/list.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/portal/entitlement/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/portal/pool/__init__.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/portal/pool/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/portal/pool/delete.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/portal/pool/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/portal/pool/get.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/portal/pool/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/portal/pool/list.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/portal/pool/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/portal/site/__init__.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/portal/site/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/portal/site/create.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/portal/site/create.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/portal/site/delete.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/portal/site/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/portal/site/get.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/portal/site/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/portal/site/list.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/portal/site/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/portal/site/set-edge.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/portal/site/set-edge.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/profile/init.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/profile/init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/upgrade.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/upgrade.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/vmhub/__init__.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/vmhub/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/vmhub/otp/__init__.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/vmhub/otp/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/vmhub/otp/redeem.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/vmhub/otp/redeem.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/cmds/vmhub/otp/request.py` & `hcs-cli-0.1.48/vhcs/cli/cmds/vmhub/otp/request.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/cli/main.py` & `hcs-cli-0.1.48/vhcs/cli/main.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/common/ctxp/README.md` & `hcs-cli-0.1.48/vhcs/common/ctxp/README.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/common/ctxp/__init__.py` & `hcs-cli-0.1.48/vhcs/common/ctxp/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/common/ctxp/_init.py` & `hcs-cli-0.1.48/vhcs/common/ctxp/_init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/common/ctxp/built_in_cmds/context.py` & `hcs-cli-0.1.48/vhcs/common/ctxp/built_in_cmds/context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/common/ctxp/built_in_cmds/profile.py` & `hcs-cli-0.1.48/vhcs/common/ctxp/built_in_cmds/profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/common/ctxp/cli_processor.py` & `hcs-cli-0.1.48/vhcs/common/ctxp/cli_processor.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/common/ctxp/config.py` & `hcs-cli-0.1.48/vhcs/common/ctxp/config.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/common/ctxp/context.py` & `hcs-cli-0.1.48/vhcs/common/ctxp/context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/common/ctxp/fstore.py` & `hcs-cli-0.1.48/vhcs/common/ctxp/fstore.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/common/ctxp/init.py` & `hcs-cli-0.1.48/vhcs/common/ctxp/init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/common/ctxp/jsondot.py` & `hcs-cli-0.1.48/vhcs/common/ctxp/jsondot.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/common/ctxp/profile.py` & `hcs-cli-0.1.48/vhcs/common/ctxp/profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/common/ctxp/profile_store.py` & `hcs-cli-0.1.48/vhcs/common/ctxp/profile_store.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/common/ctxp/state.py` & `hcs-cli-0.1.48/vhcs/common/ctxp/state.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/common/ctxp/util.py` & `hcs-cli-0.1.48/vhcs/common/ctxp/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,19 +83,28 @@
                 raise Exception(f"Unexpected output format: {output}")
         except Exception as e:
             print("Fail converting object:", e, file=sys.stderr)
             text = data
     print(text, end="", file=file)
 
 def print_error(error):
-    if isinstance(error, httpx.HTTPStatusError) or isinstance(error, CtxpException) or isinstance(error, TimeoutError) or isinstance(error, subprocess.CalledProcessError):
-        msg = error_details(error)
-        print(msg, file=sys.stderr)
-    else:
-        traceback.print_exception(type(error), error, error.__traceback__, file=sys.stderr)
+    known_exceptions = [
+        httpx.HTTPStatusError,
+        httpx.ConnectError,
+        CtxpException,
+        TimeoutError,
+        subprocess.CalledProcessError,
+        KeyboardInterrupt
+    ]
+    for ex in known_exceptions:
+        if isinstance(error, ex):
+            msg = error_details(error)
+            print(msg, file=sys.stderr)
+            return
+    traceback.print_exception(type(error), error, error.__traceback__, file=sys.stderr)
 
 def _convert_generator(data: Any):
     if isinstance(data, types.GeneratorType):
         return list(data)
     return data
 
 def _filter_fields(obj: Any, fields: str):
```

### Comparing `hcs-cli-0.1.47/vhcs/common/ctxp/var_template.py` & `hcs-cli-0.1.48/vhcs/common/ctxp/var_template.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/common/logger.py` & `hcs-cli-0.1.48/vhcs/common/logger.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/common/sglib/__init__.py` & `hcs-cli-0.1.48/vhcs/common/sglib/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/common/sglib/auth.py` & `hcs-cli-0.1.48/vhcs/common/sglib/auth.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/common/sglib/csp.py` & `hcs-cli-0.1.48/vhcs/common/sglib/csp.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/common/sglib/ez_client.py` & `hcs-cli-0.1.48/vhcs/common/sglib/ez_client.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/common/sglib/hcs_client.py` & `hcs-cli-0.1.48/vhcs/common/sglib/hcs_client.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/common/sglib/login_support.py` & `hcs-cli-0.1.48/vhcs/common/sglib/login_support.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/common/sglib/util.py` & `hcs-cli-0.1.48/vhcs/common/sglib/util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/common/util.py` & `hcs-cli-0.1.48/vhcs/common/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     return text
 
 def save_data_file(data: dict | list, file_name: str, format: str = 'yaml'):
     with open(file_name, "w") as file:
         if format == 'yaml':
             # TODO
             #yaml.safe_dump(data, file, sort_keys=False)
-            yaml.safe_dump(json.loads(json.dumps(data)), file, sort_keys=False)
+            yaml.safe_dump(json.loads(json.dumps(data, default=vars)), file, sort_keys=False)
         elif format == 'json':
             json.dump(data, file, indent=4, default=vars)
         else:
             raise Exception("Invalid format: " + format)
         
 def strict_dict_to_class(data: dict, class_type):
 
@@ -174,21 +174,22 @@
         fn_on_value(obj)
 
 def deep_find_variables(obj):
     collector = set()
     def fn_on_value(v):
         if not v or not isinstance(v, str):
             return
-        m = _pattern_var.match(v)
-        if m:
+        matches = re.findall(_pattern_var_only, v)
+        if matches:
             m2 = _pattern_var_list.match(v)
             if m2:
                 collector.add(m2.group(2))
             else:
-                collector.add(m.group(1))
+                for i in matches:
+                    collector.add(i)
     deep_iterate(obj, fn_on_value)
     return collector
 
 def process_variables(obj: dict, fn_get_var = None):
     if fn_get_var == None:
         def _fn_get_var(name):
             try:
@@ -204,15 +205,16 @@
         if not ret['changed']:
             return {
                 'data': ret['data'],
                 'changed': total_changed,
                 'pending': ret['pending'],
             }
 
-_pattern_var = re.compile('.*?\$\{(.+?)\}.*')
+_pattern_var = re.compile('.*\$\{(.+?)\}.*')
+_pattern_var_only = re.compile('\$\{(.+?)\}')
 _pattern_var_list = re.compile('\$\{\s*\[\s*for\s+(.+?)\s+in\s+(.+?)\s*\:\s*(.+)\s*]\s*\}')
 def _process_variables_impl(obj: dict, fn_get_var = None):
     changed = {}
     pending = {}
 
     def fn_change(path, v):
         resolved, pending_var = resolve_expression(v, fn_get_var, path)
```

### Comparing `hcs-cli-0.1.47/vhcs/config/hcs-deployments.yaml` & `hcs-cli-0.1.48/vhcs/config/hcs-deployments.yaml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/plan/core.py` & `hcs-cli-0.1.48/vhcs/plan/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,35 +25,47 @@
 from .helper import PlanException, process_template
 from .actions import actions
 from .kop import KOP
 from importlib import import_module
 
 import logging
 log = logging.getLogger(__name__)
-log.setLevel(logging.DEBUG)
+log.setLevel(logging.INFO)
 
-def _prepare_data(data: dict, additional_context: dict, resource_name: str):
+def _prepare_data(data: dict, additional_context: dict, target_resource_name: str):
     if additional_context:
         common_items = util.get_common_items(additional_context.keys(), data.keys())
         if common_items:
             raise PlanException("blueprint and context have conflict keys: " + str(common_items))
         data.update(additional_context)
     blueprint, pending = process_template(data)
-    if resource_name and resource_name not in blueprint['resources']:
-        raise PlanException("Resource target not found: " + resource_name)
+    if target_resource_name and target_resource_name not in blueprint['resources'] and target_resource_name not in blueprint.get('runtimes', {}):
+        raise PlanException("Target resource or runtime not found: " + target_resource_name)
     
     for k, v in pending.items():
         if v.startswith('defaults.') or v.startswith('vars.'):
-            raise PlanException(f"Invalid blueprint. Unresolved static references. Variable not found: {v}. Required by {k}")
+            if not k.find(".conditions."):
+                raise PlanException(f"Invalid blueprint. Unresolved static references. Variable not found: {v}. Required by {k}")
     deployment_id = blueprint['deploymentId']
     state_file = deployment_id + '.state.yml'
-    prev = _load_state(state_file)
+    prev = util.load_data_file(state_file, default={})
     state = {'pending': pending}
     state.update(blueprint)
-    state.update(prev)
+    if 'providers' not in state:
+        state['providers'] = {}
+    if 'runtimes' not in state:
+        state['runtimes'] = {}
+    state['output'] = prev.get('output', {})
+    state['destroy_output'] = prev.get('destroy_output', {})
+    state['log'] = prev.get('log', {})
+    exec_log = state['log']
+    if 'create' not in exec_log:
+        exec_log['create'] = []
+    if 'delete' not in exec_log:
+        exec_log['delete'] = []
 
     context.set('deploymentId', state['deploymentId'])
     
     # try solving more variables
     # for k, v in state['output'].items():
     #     if not v:
     #         continue
@@ -66,59 +78,45 @@
 # def _has_successful_deployment(state, name):
 #     for v in state['log']['create']:
 #         if v['name'] != name:
 #             continue
 #         if v['action'] == 'success':
 #             return True
         
-def deploy(data: dict, additional_context: dict = None, resource_name: str = None, include_related_resources: bool = True, concurrency: int = 4):
+def deploy(data: dict, additional_context: dict = None, target_resource_name: str = None, include_dependencies: bool = True, concurrency: int = 4):
     
-    blueprint, state, state_file = _prepare_data(data, additional_context, resource_name)
+    blueprint, state, state_file = _prepare_data(data, additional_context, target_resource_name)
     state['log']['create'] = []    # clear deploy log
 
-    def process_resource(name: str):
-        # ignore functional nodes (defaults, providers)
-        if name not in blueprint['resources']:
-            return
-        res_data = blueprint['resources'][name]
-        
-        if resource_name:
-            if name == resource_name or include_related_resources:
-                need_deploy = True
-            else:
-                need_deploy = False
-        else:
-            need_deploy = True
-        if need_deploy:
-            _deploy_res(name, res_data, state)
-            util.save_data_file(state, state_file)
-        if resource_name and name == resource_name:
-            return False    # quit dag.process_blueprint
+    def deploy_resource_or_runtime(name, res_data):
+        _deploy_res(name, res_data, state)
+        util.save_data_file(state, state_file)
 
+    def process_resource_node(name: str):
+        if name in blueprint['resources']:
+            res_data = blueprint['resources'][name]
+            return deploy_resource_or_runtime(name, res_data)
+        elif name in blueprint.get('runtimes', {}):
+            res_data = blueprint['runtimes'][name]
+            return deploy_resource_or_runtime(name, res_data)
+        elif name in blueprint.get('providers', {}):
+            # ignore.
+            # Provide init is always ensured before running the resource 
+            # and does not follow deploy/destroy sequenct.
+            pass
+        else:
+            # defaults, vars, etc.
+            pass
     try:
-        dag.process_blueprint(blueprint, process_resource, False, concurrency)
+        dag.process_blueprint(blueprint, process_resource_node, False, concurrency, target_resource_name, include_dependencies)
     except CalledProcessError as e:
         raise PlanException(str(e))
     finally:
         util.save_data_file(state, state_file)
 
-def _load_state(state_file):
-    state = util.load_data_file(state_file, default={})
-    if 'output' not in state:
-        state['output'] = {}
-    if 'destroy_output' not in state:
-        state['destroy_output'] = {}
-    if 'log' not in state:
-        state['log'] = {}
-    exec_log = state['log']
-    if 'deploy' not in exec_log:
-        exec_log['deploy'] = []
-    if 'destroy' not in exec_log:
-        exec_log['destroy'] = []
-    return state
 
 def _parse_statement_for(name, state) -> typing.Tuple[str, list]:
     # for: email in vars.userEmails
     res = state['resources'][name]
     for_statement = res.get('for')
     if not for_statement:
         return None, None
@@ -164,15 +162,15 @@
 def _get_value_by_path2(state, var_name):
     i = var_name.find('.')
     if i < 0:
         resource_name = var_name
     else:
         resource_name = var_name[:i]
 
-    if resource_name in state['resources']:
+    if resource_name in state['resources'] or resource_name in state['runtimes'] or resource_name in state['providers']:
         try:
             return util.deep_get_attr(state, "output." + var_name), True
         except Exception as e:
             log.debug(e)
             return None, False
         
     if resource_name in state:
@@ -182,15 +180,15 @@
             log.debug(e)
             return None, False
     return None, False
 
 def _deploy_res(name, res, state):
     def fn_deploy1(handler, res_data: dict, res_state: dict, fn_set_state: typing.Callable, kop: KOP):
         if _is_runtime(res):
-            kop.start(KOP.MODE.create)
+            kop.start(KOP.MODE.create, handler.eta('create', res_data, state))
             new_state = handler.process(res_data, deepcopy(state))
             if new_state:
                 fn_set_state(new_state)
             return
         
         if not res_state:
             action = actions.create
@@ -199,44 +197,43 @@
             
         if action == actions.skip:
             kop.skip('Already deployed')
             return
         
         if action == actions.recreate:
             with KOP(state, res['kind'], name) as kop2:
-                kop2.id = res_state.get('id')
-                kop2.start(KOP.MODE.delete)
-                handler.destroy(res_data, res_state)
+                kop2.id(res_state.get('id'))
+                kop2.start(KOP.MODE.delete, handler.eta(actions.delete, res_data, res_state))
+                handler.destroy(res_data, res_state, False)
             action = actions.create
 
         new_state = None
-        if action == actions.create:
-            kop.start(KOP.MODE.create)
+        if action == actions.create or action == None:
+            kop.start(KOP.MODE.create, handler.eta(actions.create, res_data, res_state))
             if _has_save_state(handler.deploy):
                 new_state = handler.deploy(res_data, res_state, fn_set_state)
             else:
                 new_state = handler.deploy(res_data, res_state)
-            kop.id(None if not new_state else new_state.get('id'))
+            kop.id(_discover_id(new_state))
         elif action == actions.update:
             kop.id(res_state.get('id'))
-            kop.start(KOP.MODE.update)
+            kop.start(KOP.MODE.update, handler.eta(actions.update, res_data, res_state))
             if _has_save_state(handler.update):
                 new_state = handler.update(res_data, res_state, fn_set_state)
             else:
                 new_state = handler.update(res_data, res_state)
         else:
-            raise PlanException(f"Unknown action. Plugin={name}, action={action}")
+            raise PlanException(f"Unknown action. This is a problem of the concrete plugin.decide function. Plugin={name}, action={action}")
         
         if new_state:
             fn_set_state(new_state)
     _handle_resource(name, res, state, True, fn_deploy1)
 
 def _is_runtime(res):
-    kind = res.get('kind')
-    return kind and kind.startswith('runtime/')
+    return 'impl' in res
 
 def _has_save_state(fn):
     signature = inspect.signature(fn)
     args = list(signature.parameters.keys())
     if len(args) < 3:
         return False
     name = args[2]
@@ -250,73 +247,89 @@
         if isinstance(value, str) and value.find('${') >= 0:
             raise PlanException(f"Unresolved variable '{path}' for plugin '{name}'. Value={value}")
         return value
     util.deep_update_object_value(data, fn_on_value)
 
 _providers = {}
 _provider_lock = threading.Lock()
-def _get_resource_handler(kind: str, state: dict):
-    provider_type, res_handler_type = kind.split('/')
-    res_handler_type = res_handler_type.replace('-', '_')
+def _ensure_provider(provider_id: str, state: dict):
     # Ensure provider initialized
     with _provider_lock:
-        if provider_type == 'runtime':
-            return import_module(res_handler_type)
-        if not provider_type in _providers:
-            provider = import_module("vhcs.plan.provider." + provider_type)
+        if not provider_id in _providers:
+            provider = import_module("vhcs.plan.provider." + provider_id)
             # Get provider data
-            filter_by_type = lambda m: m['type'] == provider_type
-            providers = state.get('providers', {})
-            meta = next(filter(filter_by_type, providers), None)
+            meta = state['providers'].get(provider_id)
+            def _get_value(path):
+                return _get_value_by_path2(state, path)
+            util.process_variables(meta, _get_value)
+
             data = meta.get('data') if meta else None
             if data:
-                _assert_all_vars_resolved(data, provider_type)
-            log.info("[init] Provider: %s", provider_type)
-            state['output'][provider_type] = provider.prepare(data)
-            log.info("[ok  ] Provider: %s", provider_type)
-            _providers[provider_type] = 1
-    module_name = f"vhcs.plan.provider.{provider_type}.{res_handler_type}"
+                _assert_all_vars_resolved(data, provider_id)
+            else:
+                data = {}
+            log.debug("[init] Provider: %s", provider_id)
+            state['output'][provider_id] = provider.prepare(data)
+            log.debug("[ok  ] Provider: %s", provider_id)
+            _providers[provider_id] = 1
+
+def _get_resource_handler(kind: str, state: dict):
+    provider_id, res_handler_type = kind.split('/')
+    res_handler_type = res_handler_type.replace('-', '_')
+    _ensure_provider(provider_id, state)
+    module_name = f"vhcs.plan.provider.{provider_id}.{res_handler_type}"
     return import_module(module_name)
 
+def _get_runtime_handler(impl_name: str):
+    return import_module(impl_name)
+
 def get_common_items(iter1, iter2):
     return set(iter1).intersection(set(iter2))
 
 def _handle_resource(name, res, state, for_deploy: bool, fn_process: typing.Callable):
-    kind = res['kind']
+    if 'kind' in res:
+        kind = res['kind']
+    elif 'impl' in res:
+        kind = 'runtime'
+    else:
+        raise PlanException("Invalid definition. Neither kind nor impl attribute found. Resource name: " + name)
 
     kop_mode = KOP.MODE.create if for_deploy else KOP.MODE.delete
     with KOP(state, kind, name, kop_mode) as kop:
-        data = res.get('data', {})
 
-        # resolve vars
         def _get_value(path):
             return _get_value_by_path2(state, path)
         
+        conditions = res.get('conditions')
+        if conditions:
+            conditions = deepcopy(conditions)
+            ret = util.process_variables(conditions, _get_value)
+            unsatisfied_condition_name = _get_unsatisfied_condition_name(conditions)
+            if unsatisfied_condition_name:
+                kop.skip('Condition not met: ' + unsatisfied_condition_name)
+                return
+            
+        # resolve vars
+        data = res.get('data', {})
         if data:
             data = deepcopy(data)
             ret = util.process_variables(data, _get_value)
             if for_deploy:
                 if ret['pending']:
                     msg = f"Fail resolving variables for resource '{name}'. Unresolvable variables: {ret['pending']}"
                     raise PlanException(msg)
         state['resources'][name] = dict(res)
         state['resources'][name]['data'] = data
 
-        conditions = res.get('conditions')
-        if conditions:
-            conditions = deepcopy(conditions)
-            ret = util.process_variables(conditions, _get_value)
-            unsatisfied_condition_name = _get_unsatisfied_condition_name(conditions)
-            if unsatisfied_condition_name:
-                kop.skip('Condition not met: ' + unsatisfied_condition_name)
-                return
-
+        if kind == 'runtime':
+            handler = _get_runtime_handler(res['impl'])
+        else:
+            handler = _get_resource_handler(kind, state)
 
-        handler = _get_resource_handler(kind, state)
-        def _handle_resource_1(resource_data, resource_state, fn_set_state, kop):
+        def _handle_resource_1(resource_data, resource_state, fn_set_state, kop) -> bool:
             if _is_runtime(res):   # runtime has no refresh
                 pass
             else:
                 new_state = handler.refresh(resource_data, resource_state)
                 fn_set_state(new_state)
                 resource_state = new_state
 
@@ -331,15 +344,15 @@
             size = len(values)
             # ensure output array placeholder
             output = state['output'].setdefault(name, [])
             while len(output) < size:
                 output.append(None)
             for i in range(size):
                 v = values[i]
-                with KOP(state, kind, name, kop_mode) as kop_per_item:
+                with KOP(state, kind, name + f'#{i}', kop_mode) as kop_per_item:
                     kop_per_item.id(str(i))
                     resource_state = output[i]
                     def _fn_set_state(o):
                         output[i] = deepcopy(o)
                     resource_data = deepcopy(data)
                     resource_data[for_var_name] = v
                     _handle_resource_1(resource_data, resource_state, _fn_set_state, kop_per_item)
@@ -356,74 +369,59 @@
     for condition_name, expr in conditions.items():
         if not expr:
             return condition_name
         if expr.find('${') >= 0: # still have unresolved variables
             return condition_name
 
 
-
+def _discover_id(obj):
+    if isinstance(obj, dict):
+        return obj.get('id')
 
 def _destroy_res(name, res_node, state, force):
     def fn_destroy1(handler, res_data: dict, res_state: dict, fn_set_state: typing.Callable, kop: KOP):
         if not res_state:
             kop.skip('Not found')
             return
-        
-        kop.id(res_state.get('id'))
-        kop.start(KOP.MODE.delete)
-        try:
-            ret = handler.destroy(res_data, res_state)
-            state['destroy_output'][name] = deepcopy(ret)
-            fn_set_state(None)
-        except Exception as e:
-            if force:
-                kop.error(e)
-                pass
-            else:
-                # add_log('error', e) will be handled by framework.
-                raise
+        kop.id(_discover_id(res_state))
+        kop.start(KOP.MODE.delete, handler.eta(actions.delete, res_data, res_state))
+        ret = handler.destroy(res_data, res_state, force)
+        state['destroy_output'][name] = deepcopy(ret)
+        fn_set_state(None)
+
     _handle_resource(name, res_node, state, False, fn_destroy1)
 
-def destroy(data, force: bool, resource_name: str = None, include_related_resources: bool = True, concurrency: int = 4, additional_context: dict = None):
+def destroy(data, force: bool, target_resource_name: str = None, include_related_resources: bool = True, concurrency: int = 4, additional_context: dict = None):
     
-    blueprint, state, state_file = _prepare_data(data, additional_context, resource_name)
+    blueprint, state, state_file = _prepare_data(data, additional_context, target_resource_name)
     state['log']['delete'] = []    # clear destroy log
 
     def destroy_resource(node_name):
         # ignore functional nodes (defaults, providers)
         node = blueprint['resources'].get(node_name)
         if not node:
-            return
+            return dag.walker.next
         # skip runtime
         if node['kind'].startswith('runtime/'):
-            return
+            return dag.walker.next
         
         res_node = state['resources'].get(node_name)
         if not res_node:
             res_node = blueprint['resources'][node_name]
 
-        if resource_name:
-            if include_related_resources:
-                pass
-            else:
-                if resource_name != node_name:
-                    return
-            _destroy_res(node_name, res_node, state, force)
-            util.save_data_file(state, state_file)
-            if resource_name == node_name:
-                return True
-        else:
-            _destroy_res(node_name, res_node, state, force)
-            util.save_data_file(state, state_file)
+        _destroy_res(node_name, res_node, state, force)
+        util.save_data_file(state, state_file)
+        return dag.walker.next
+            
 
     try:
         dag.process_blueprint(blueprint, destroy_resource, True, concurrency)
     except CalledProcessError as e:
         raise PlanException(str(e))
     finally:
         util.save_data_file(state, state_file)
 
-def graph(data: dict, additional_context: dict = None, simplify: bool = True):
+def graph(data: dict, additional_context: dict = None, reverse: bool = False, target_resource: str = None, include_dependencies: bool = True):
     blueprint, state, state_file = _prepare_data(data, additional_context, None)
-    g = dag.graph(blueprint, state, simplify)
+    g = dag.graph(blueprint, state, reverse, target_resource, include_dependencies)
     return g
```

### Comparing `hcs-cli-0.1.47/vhcs/plan/helper.py` & `hcs-cli-0.1.48/vhcs/plan/helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,17 +23,23 @@
     pass
 
 class PluginException(Exception):
     pass
 
 class Blueprint:
     vars: dict
-    defaults: dict = {}
-    providers: list = []
-    resources: list
+    defaults: dict
+    providers: dict
+    resources: dict
+
+    def __init__(self):
+        self.vars = {}
+        self.defaults = {}
+        self.providers = {}
+        self.resources = {}
 
     def __repr__(self):
         return f"Blueprint"
 
 def load_files(files: list[str]) -> dict:
     ret = {}
     for file in files:
@@ -47,26 +53,24 @@
 def process_template(template) -> Tuple[dict, dict]:
     _validate_blueprint(template)
     bp, pending = _materialize_blueprint(template)
     return bp, pending
 
 def _validate_blueprint(blueprint: dict):
     _validate_resource_schema(blueprint)
-    _validate_resource_id_no_dup(blueprint)
     _validate_resource_id_not_conflict_to_reserved_names(blueprint)
-    _validate_resource_id_not_conflict_to_provider_types(blueprint)
-    _validate_no_duplicate_provider_config(blueprint)
+    _validate_no_conflict_resource_id_provider_types_runtime_id(blueprint)
     _validate_statement_after(blueprint)
 
 def _validate_resource_schema(blueprint: dict):
     resources = blueprint.get('resources')
     if not resources:
         return
     required_keys = set(['kind'])
-    optional_keys = set(['data', 'conditions', 'for', 'after'])
+    optional_keys = set(['eta', 'data', 'conditions', 'for', 'after'])
     for k, v in resources.items():
         def _raise(reason):
             raise PlanException(f"Invalid blueprint: {reason}. Resource: {k}")
         actual_keys = set(v.keys())
         missed_keys = required_keys - actual_keys
         if missed_keys:
             _raise(f'Missing required keys: {missed_keys}')
@@ -100,41 +104,30 @@
                 if dup:
                     _raise(k, 'Duplicated keys: ' + dup)
             elif isinstance(after, str):
                 _validate_after(after, k)
             else:
                 _raise(k, "Invalid type, expect str or list, got: " + type(after).__name__)
 
-def _validate_no_duplicate_provider_config(blueprint: dict):
-    providers = blueprint.get('providers')
-    if not providers:
-        return
-    known_types = []
-    for r in providers:
-        t = r['type']
-        if t in known_types:
-            raise PlanException("Invalid blueprint. Duplicated provider config: " + r['type'])
-        known_types.append(t)
 
-def _validate_resource_id_not_conflict_to_provider_types(blueprint: dict):
+def _validate_no_conflict_resource_id_provider_types_runtime_id(blueprint: dict):
     provider_names = set()
-    for k, v in blueprint['resources'].items():
+    runtime_names = set(blueprint.get('runtimes', {}).keys())
+    for v in blueprint['resources'].values():
         name, _ = v['kind'].split('/')
         provider_names.add(name)
     for name in blueprint['resources']:
         if name in provider_names:
             raise PlanException("Invalid blueprint. Invalid resource name due to conflict to provider type. Name: " + name)
-        
-def _validate_resource_id_no_dup(blueprint: dict):
-    resource_names = set()
-    for name in blueprint['resources']:
-        if name in resource_names:
-            raise PlanException("Invalid blueprint. Duplicated resource name: " + name)
-        resource_names.add(name)
+        if name in runtime_names:
+            raise PlanException("Invalid blueprint. Invalid resource name due to conflict to runtime name. Name: " + name)
 
+    if provider_names & runtime_names:
+        raise PlanException("Invalid blueprint. Provider id and runtime id conflict. Runtime must not have conflict id as provider.")
+    
 def _validate_resource_id_not_conflict_to_reserved_names(blueprint: dict):
     reserved_names_for_state = ['result', 'pending', 'log', 'destroy_output']
     reserved_names_for_blueprint = ['defaults', 'vars', 'providers', 'resources']
     reserved_names_for_function = ['profile', 'context']
     existing_names_top_level = blueprint.keys()
     reserved_names = set([*existing_names_top_level, *reserved_names_for_blueprint, *reserved_names_for_state, *reserved_names_for_function])
     for name in blueprint['resources']:
```

### Comparing `hcs-cli-0.1.47/vhcs/plan/kop.py` & `hcs-cli-0.1.48/vhcs/plan/kop.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 limitations under the License.
 """
 
 import time
 import traceback
 import traceback
 import logging
+from typing import Any
 from vhcs.common.ctxp.util import CtxpException
 from httpx import HTTPStatusError
 from subprocess import CalledProcessError
 from vhcs.common.ctxp.util import error_details
 from .helper import PlanException, PluginException
 
 log = logging.getLogger(__name__)
@@ -34,67 +35,112 @@
 
 class KopAction:
     start = 'start'
     success = 'success'
     error = 'error'
     skip = 'skip'
 
+class _DummyJobView:
+    def add(id, name):
+        pass
+    def update(id, text: str):
+        pass
+    def start(id, eta: str):
+        pass
+    def success(id):
+        pass
+    def skip(id, reason):
+        pass
+    def error(id, err):
+        pass
+_job_view = _DummyJobView
+
+def attach_job_view(view):
+    global _job_view
+    _job_view = view
+
 class KOP:
     MODE = KopMode
 
     def __init__(self, state: dict, kind: str, name: str, mode: str = KopMode.create) -> "KOP":
         self._state = state
         self._kind = kind
         self._name = name
         self._id = None
         self._mode = mode
         self._started = False
         self._closed = False
+        job_id = kind + '/' + name
+        _job_view.add(job_id, job_id)
 
+    
+    def _job_id(self):
+        return self._kind + '/' + self._name
+    
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         if exc_value:
             self.error(exc_value)
         else:
             # default closing upon leaving scope
             if not self._closed:
                 self._success()
 
-    def id(self, id: str):
-        self._id = id
+    # Getter and setter for dollars...
+    @property
+    def dollars(self):
+        return self.total_cents // 100
+    
+    @dollars.setter
+    def dollars(self, new_dollars):
+        self.total_cents = 100 * new_dollars + self.cents
+
+    def id(self, res_id: str):
+        self._id = res_id
+        _job_view.update(self._job_id(), res_id)
 
-    def start(self, mode: str = None):
+    def start(self, mode: str = None, eta: str = None):
         if self._started:
             raise KopException("Kop already started. This is a framework logging issue.")
         if self._closed:
             raise KopException("Kop already closed. This is a framework logging issue.")
         if mode:
             self._mode = mode
         self._started = True
         self._add_log(KopAction.start)
+        _job_view.start(self._job_id(), eta)
 
     def _success(self):
         if not self._started:
             raise KopException("Kop not started. This is a framework logging issue. Call kop.start() before starting the resource operation.")
         if self._closed:
             raise KopException("Kop already closed. This is a framework logging issue.");
         self._add_log(KopAction.success)
         self._closed = True
+        _job_view.success(self._job_id())
 
-    def error(self, error):
-        self._add_log(KopAction.error, error)
+    def error(self, err):
+        if isinstance(err, Exception):
+            if _need_stack_trace(err):
+                traceback.print_exception(type(err), err, err.__traceback__)
+            details = error_details(err)
+        else:
+            details = str(details)
+        self._add_log(KopAction.error, details)
         self._closed = True
+        _job_view.error(self._job_id(), details)
 
     def skip(self, reason):
         self._add_log(KopAction.skip, reason)
         self._closed = True
+        _job_view.skip(self._job_id(), reason)
 
-    def _add_log(self, action: str, details = None):
+    def _add_log(self, action: str, details: str = None):
         labels = {
             KopMode.create: {
                 KopAction.start:    '[creating]',
                 KopAction.success:  '[created ]',
                 KopAction.skip:     '[skipped ]',
                 KopAction.error:    '[error   ]'
             },
@@ -114,45 +160,30 @@
         label_map = labels.get(self._mode)
         if not label_map:
             raise KopException(f"Invalid mode: {self._mode}")
         label = label_map[action]
         msg = f'{label} {self._kind}:{self._name}'
         if self._id:
             msg += ' ' + self._id
-        log.info(msg)
+
+        if _job_view == _DummyJobView:
+            log.info(msg)
         entry = {
             'name': self._name,
             'time': int(time.time()),
             'action': action,
             'id': self._id
         }
         if details:
-            if isinstance(details, Exception):
-                e = details
-                if _need_stack_trace(details):
-                    traceback.print_exception(type(e), e, e.__traceback__)
-                details = error_details(e)
-            else:
-                details = str(details)
             entry['details'] = details
         self._state['log'][self._mode].append(entry)
         if action == 'error':
             if self._id:
                 log.warning('Plugin "%s:%s" failed: %s. Id=%s', self._kind, self._name, details, self._id)
             else:
                 log.warning('Plugin "%s:%s" failed: %s.', self._kind, self._name, details)
 
 
 def _need_stack_trace(e):
-    if isinstance(e, PlanException):
-        return
-    if isinstance(e, PluginException):
-        return
-    if isinstance(e, CalledProcessError):
-        return
-    if isinstance(e, TimeoutError):
-        return
-    if isinstance(e, CtxpException):
-        return
-    if isinstance(e, HTTPStatusError):
-        return
-    return True
+    if isinstance(e, KeyError):
+        return True
+
```

### Comparing `hcs-cli-0.1.47/vhcs/plan/provider/azure/aad_group.py` & `hcs-cli-0.1.48/vhcs/plan/provider/azure/aad_group.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from vhcs.plan import actions
+from azure.core.exceptions import ResourceNotFoundError
 from . import _az_facade as az
 
 def deploy(data: dict, state: dict) -> dict:
     display_name = data['displayName']
     mail_nickname = data['mailNickname']
     description = data.get('description')
     parent_group = data.get('parentGroup')
@@ -30,13 +31,16 @@
 def refresh(data: dict, state: dict) -> dict:
     display_name = data['displayName']
     return az.aad.group.get(display_name)
 
 def decide(data: dict, state: dict):
     return actions.skip
 
-def destroy(data: dict, state: dict) -> dict:
+def destroy(data: dict, state: dict, force: bool) -> dict:
     if state:
         id = state['id']
         return az.aad.group.delete(id)
     display_name = data['displayName']
-    return az.aad.group.delete(display_name)
+    return az.aad.group.delete(display_name)
+
+def eta(action: str, data: dict, state: dict):
+    return '1m'
```

### Comparing `hcs-cli-0.1.47/vhcs/plan/provider/azure/aad_user.py` & `hcs-cli-0.1.48/vhcs/plan/provider/azure/aad_user.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,52 +10,59 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from vhcs.plan import actions
+from azure.core.exceptions import ResourceNotFoundError
 import random
 from . import _az_facade as az
 
-def deploy(data: dic, state: dict) -> dict:
+def deploy(data: dict, state: dict) -> dict:
     group = data['group']
     email = data['email']
     domain_name = data['domainName']
 
     pname = _convert_email_to_principle(email, domain_name)
     display_name = pname
     password = _generate_password()
     principal_name = pname
     ret = az.aad.user.create(display_name, password, principal_name)
     az.aad.group.member.add(group, ret['id'])
     ret['password'] = password
     return ret
 
 def _convert_email_to_principle(email: str, domain_name: str) -> str:
-    name = email.replace('@', '-').replace('.', '-')
+    name = email.replace('@', '_')
     return name + '@' + domain_name
 
 def _generate_password() -> str:
     ret = random.choices("ABCDEFGHJKMNPQRSTUVWXY")
     ret += random.choices("abcdefghjkmnpqrstuvwxy23456789", k=10)
     ret += random.choices("!@$%&*")
     return "".join(ret)
 
 def refresh(data: dict, state: dict) -> dict:
     if state:
         id = state['id']
         ret = az.aad.user.get(id)
         if ret:
+            ret['password'] = state.get('password')
             return ret
     email = data['email']
     domain_name = data['domainName']
     pname = _convert_email_to_principle(email, domain_name)
     return az.aad.user.get(pname)
 
 def decide(data: dict, state: dict):
+    if not state.get('password'):
+        return actions.recreate
     return actions.skip
 
-def destroy(data: dict, state: dict) -> dict:
+def destroy(data: dict, state: dict, force: bool) -> dict:
     id = state['id']
     ret = az.aad.user.delete(id)
-    return ret
+    return ret
+
+def eta(action: str, data: dict, state: dict):
+    return '1m'
```

### Comparing `hcs-cli-0.1.47/vhcs/plan/provider/azure/nsg.py` & `hcs-cli-0.1.48/vhcs/plan/provider/azure/nsg.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,30 +10,34 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from vhcs.plan import actions
-from . import _az_facade as az
+from azure.core.exceptions import ResourceNotFoundError
+from ._az_facade import network_management_client as client, adjust_tags
 
 def deploy(data: dict, state: dict) -> dict:
+    rg_name = data['resourceGroup']
     name = data['name']
-    location = data['location']
-    resourceGroup = data['resourceGroup']
-    tags = data.get('tags')
-
-    return az.network.nsg.create(resourceGroup, name, location, tags)
+    parameters = adjust_tags(data['parameters'])
+    return client().network_security_groups.begin_create_or_update(rg_name, name, parameters).result()
 
 def refresh(data: dict, state: dict) -> dict:
-    return state
+    rg_name = data['resourceGroup']
+    name = data['name']
+    try:
+        return client().network_security_groups.get(rg_name, name)
+    except ResourceNotFoundError:
+        pass
 
 def decide(data: dict, state: dict):
     return actions.skip
 
-def destroy(data: dict, state: dict) -> dict:
-    if state.get('NewNSG'):
-        id = state.get('NewNSG')['id']
-        return az.network.nsg.delete_by_id(id)
+def destroy(data: dict, state: dict, force: bool) -> dict:
+    rg_name = data['resourceGroup']
     name = data['name']
-    resourceGroup = data['resourceGroup']
-    return az.network.nsg.delete(name, resourceGroup)
+    client().network_security_groups.begin_delete(rg_name, name).wait()
+
+def eta(action: str, data: dict, state: dict):
+    return '1m'
```

### Comparing `hcs-cli-0.1.47/vhcs/plan/provider/azure/resource_group.py` & `hcs-cli-0.1.48/vhcs/plan/provider/azure/nat_gateway.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,25 +9,36 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from vhcs.plan import actions
-from . import _az_facade as az
+from vhcs.plan import actions, context
+from azure.core.exceptions import ResourceNotFoundError
+from ._az_facade import network_management_client as client, adjust_tags
+
 
 def deploy(data: dict, state: dict) -> dict:
+    rg_name = data['resourceGroup']
     name = data['name']
-    location = data['location']
-    tags = data.get('tags')
-    return az.resource_group.create(name, location, tags)
+    parameters = adjust_tags(data['parameters'])
+
+    return client().nat_gateways.begin_create_or_update(
+        rg_name,
+        name,
+        parameters
+    ).result()
 
 def refresh(data: dict, state: dict) -> dict:
     return state
 
 def decide(data: dict, state: dict):
     return actions.skip
 
-def destroy(data: dict, state: dict) -> dict:
+def destroy(data: dict, state: dict, force: bool) -> dict:
+    rg_name = data['resourceGroup']
     name = data['name']
-    return az.resource_group.delete(name)
+    client().nat_gateways.begin_delete(rg_name, name).wait()
+
+def eta(action: str, data: dict, state: dict):
+    return '1m'
```

### Comparing `hcs-cli-0.1.47/vhcs/plan/provider/azure/subnet.py` & `hcs-cli-0.1.48/vhcs/plan/provider/hcs/identity_provider.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,34 +10,35 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from vhcs.plan import actions
-from . import _az_facade as az
+from vhcs.service import portal
 
 def deploy(data: dict, state: dict) -> dict:
-    name = data['name']
-    resourceGroup = data['resourceGroup']
-    vNetName = data['vNetName']
-    cidr = data['cidr']
-    nsgName = data['nsgName']
-
-    return az.network.subnet.create(resourceGroup, vNetName, name, cidr, nsgName)
+    return portal.site.create(data)
 
 def refresh(data: dict, state: dict) -> dict:
-    return state
+    org_id = data['orgId']
+    if state:
+        id = state.get('id')
+        if id:
+            ret = portal.site.get(id, org_id)
+            if ret:
+                return ret
+    
+    # Fall back with smart find by name
+    return portal.site.find_by_name(data['name'], org_id)
 
 def decide(data: dict, state: dict):
     return actions.skip
 
-def destroy(data: dict, state: dict) -> dict:
-    id = state.get('id')
-    if id:
-        return az.network.subnet.delete_by_id(id)
-    name = data['name']
-    resourceGroup = data['resourceGroup']
-    vNetName = data['vNetName']
-    az.network.subnet.delete(resourceGroup, vNetName, name)
+def destroy(data: dict, state: dict, force: bool) -> dict:
+    return portal.site.delete(state['id'], data['orgId'])
 
-    
+def eta(action: str, data: dict, state: dict):
+    if action == actions.create:
+        return '1m'
+    if action == actions.delete:
+        return '1m'
```

### Comparing `hcs-cli-0.1.47/vhcs/plan/provider/dev/dummy.py` & `hcs-cli-0.1.48/vhcs/plan/provider/dev/dummy.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,20 +21,23 @@
 from vhcs.plan import PluginException
 
 
 def deploy(data: dict, state: dict, save_state: Callable) -> dict:
     text = data.get("text")
     error = data.get("error")
     delay = data.get("delay")
+    a = data.get("a", 0) 
+    b = data.get("b", 0)
     error_before_save = data.get("error_before_save")
     delay_seconds = duration.to_seconds(delay)
     if delay_seconds:
         time.sleep(delay_seconds)
     ret = deepcopy(data)
     ret["outputText"] = text
+    ret['n'] = a + b
 
     if not error_before_save:
         save_state(ret)
 
     if error:
         raise PluginException(error)
 
@@ -45,9 +48,15 @@
     return state
 
 
 def decide(data: dict, state: dict):
     return actions.skip
 
 
-def destroy(data: dict, state: dict) -> dict:
+def destroy(data: dict, state: dict, force: bool) -> dict:
     return {}
+
+def eta(action: str, data: dict, state: dict):
+    if action == actions.create:
+        return '10s'
+    if action == actions.delete:
+        return '10s'
```

### Comparing `hcs-cli-0.1.47/vhcs/plan/provider/hcs/ad.py` & `hcs-cli-0.1.48/vhcs/plan/provider/hcs/ad.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,11 +32,17 @@
     ads = admin.ad.list(org_id=org_id, search=search)
     if ads:
         return ads[0]
 
 def decide(data: dict, state: dict):
     return actions.skip
 
-def destroy(data: dict, state: dict) -> dict:
+def destroy(data: dict, state: dict, force: bool) -> dict:
     org_id = data['orgId']
     id = state['id']
-    return admin.ad.delete(id, org_id)
+    return admin.ad.delete(id, org_id)
+
+def eta(action: str, data: dict, state: dict):
+    if action == actions.create:
+        return '1m'
+    if action == actions.delete:
+        return '1m'
```

### Comparing `hcs-cli-0.1.47/vhcs/plan/provider/hcs/entitlement.py` & `hcs-cli-0.1.48/vhcs/plan/provider/hcs/entitlement.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,9 +26,15 @@
     
     # Fall back with smart find by users
     # TODO
 
 def decide(data: dict, state: dict):
     return actions.skip
     
-def destroy(data: dict, state: dict) -> dict:
-    return portal.entitlement.delete(state['id'], data['orgId'])
+def destroy(data: dict, state: dict, force: bool) -> dict:
+    return portal.entitlement.delete(state['id'], data['orgId'])
+
+def eta(action: str, data: dict, state: dict):
+    if action == actions.create:
+        return '1m'
+    if action == actions.delete:
+        return '1m'
```

### Comparing `hcs-cli-0.1.47/vhcs/plan/provider/hcs/identity_provider.py` & `hcs-cli-0.1.48/vhcs/plan/provider/hcs/site.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,9 +30,15 @@
     
     # Fall back with smart find by name
     return portal.site.find_by_name(data['name'], org_id)
 
 def decide(data: dict, state: dict):
     return actions.skip
 
-def destroy(data: dict, state: dict) -> dict:
-    return portal.site.delete(state['id'], data['orgId'])
+def destroy(data: dict, state: dict, force: bool) -> dict:
+    return portal.site.delete(state['id'], data['orgId'])
+
+def eta(action: str, data: dict, state: dict):
+    if action == actions.create:
+        return '1m'
+    if action == actions.delete:
+        return '1m'
```

### Comparing `hcs-cli-0.1.47/vhcs/plan/provider/hcs/image.py` & `hcs-cli-0.1.48/vhcs/plan/provider/hcs/image.py`

 * *Files 11% similar despite different names*

```diff
@@ -77,11 +77,19 @@
         'PENDING': actions.create,
     }
     action = status_to_action.get(status)
     if not action:
         raise Exception(f"Unknown image status: {status}")
     return action
 
-def destroy(data: dict, state: dict) -> dict:
+def destroy(data: dict, state: dict, force: bool) -> dict:
     org_id = data['import']['orgId']
     image_id = state['id']
     ims.helper.delete_images([image_id], org_id, '15m')
+
+def eta(action: str, data: dict, state: dict):
+    if action == actions.create:
+        return '60m'
+    # when the image is in-process creating/publishing, the deletion needs 
+    # to start after the image is ready (at least with IMS today), which could take a considerable time.
+    if action == actions.delete:    
+        return '60m'
```

### Comparing `hcs-cli-0.1.47/vhcs/plan/provider/hcs/launch_item.py` & `hcs-cli-0.1.48/vhcs/plan/provider/hcs/launch_item.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,9 +37,15 @@
 
 def refresh(data: dict, state: dict) -> dict:
     return state
 
 def decide(data: dict, state: dict):
     return actions.skip
 
-def destroy(data: dict, state: dict) -> dict:
-    return {}
+def destroy(data: dict, state: dict, force: bool) -> dict:
+    return {}
+
+def eta(action: str, data: dict, state: dict):
+    if action == actions.create:
+        return '1m'
+    if action == actions.delete:
+        return '1m'
```

### Comparing `hcs-cli-0.1.47/vhcs/plan/provider/hcs/pool_group.py` & `hcs-cli-0.1.48/vhcs/plan/provider/hcs/pool_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,27 +16,34 @@
 from vhcs.plan import actions
 import vhcs.service.portal as portal
 
 def deploy(data: dict, state: dict) -> dict:
     return portal.pool.create(data)
 
 def refresh(data: dict, state: dict) -> dict:
+    org_id = data['orgId']
     if state:
         id = state.get('id')
         if id:
-            return portal.pool.get(id, data['orgId'])
+            return portal.pool.get(id, org_id)
     
     # Fall back with smart find by name
-    pools = portal.pool.list(search=f"name $eq {data['name']}")
+    pools = portal.pool.list(org_id, search=f"name $eq {data['name']}")
     if pools and len(pools) == 1:
         return pools[0]
     return state
 
 def decide(data: dict, state: dict):
     return actions.skip
 
-def destroy(data: dict, state: dict) -> dict:
+def destroy(data: dict, state: dict, force: bool) -> dict:
     if state:
         id = state.get('id')
         if id:
             return portal.pool.delete(id, data['orgId'])
-    return state
+    return state
+
+def eta(action: str, data: dict, state: dict):
+    if action == actions.create:
+        return '1m'
+    if action == actions.delete:
+        return '1m'
```

### Comparing `hcs-cli-0.1.47/vhcs/plan/provider/hcs/pool_template.py` & `hcs-cli-0.1.48/vhcs/plan/provider/hcs/pool_template.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 def deploy(data: dict, state: dict, save_state: Callable) -> dict:
     ret = admin.template.create(data)
     save_state(ret)
     id = ret["id"]
     org_id = data["orgId"]
     try:
-        template = admin.template.wait_for_ready(id, org_id, timeout_seconds=600)
+        template = admin.template.wait_for_ready(id, org_id, timeout='20m')
     except Exception as e:
         template = admin.template.get(id, org_id)
         save_state(template)
         raise PluginException("Template deployment failed.") from e
     return template
 
 
@@ -50,12 +50,18 @@
         return templates[0]
 
 
 def decide(data: dict, state: dict):
     return actions.skip
 
 
-def destroy(data: dict, state: dict) -> dict:
+def destroy(data: dict, state: dict, force: bool) -> dict:
     id = state["id"]
     org_id = data["orgId"]
     admin.template.delete(id, org_id)
     admin.template.wait_for_deleted(id, org_id, 600)
+
+def eta(action: str, data: dict, state: dict):
+    if action == actions.create:
+        return '15m'
+    if action == actions.delete:
+        return '10m'
```

### Comparing `hcs-cli-0.1.47/vhcs/plan/provider/hcs/provider.py` & `hcs-cli-0.1.48/vhcs/plan/provider/hcs/provider.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,26 +19,34 @@
 def deploy(data: dict, state: dict) -> dict:
     label = data['providerLabel']
     return admin.provider.create(label, data)
 
 def refresh(data: dict, state: dict) -> dict:
     org_id = data['orgId']
     label = data['providerLabel']
+    id = None
     if state:
-        id = state.get('id')
-        if id:
-            return admin.provider.get(label, id, org_id)
+        id = state['id']
+        p = admin.provider.get(label, id, org_id)
+        if p:
+            return p
     
     # Fall back with smart find by name
     search = "name $eq " + data['name']
     providers = admin.provider.list(label, org_id=org_id, search=search)
     if providers:
         return providers[0]
 
 def decide(data: dict, state: dict):
     return actions.skip
 
-def destroy(data: dict, state: dict) -> dict:
+def destroy(data: dict, state: dict, force: bool) -> dict:
     org_id = data['orgId']
     label = data['providerLabel']
     id = state['id']
-    return admin.provider.delete(label, id, org_id)
+    return admin.provider.delete(label, id, org_id)
+
+def eta(action: str, data: dict, state: dict):
+    if action == actions.create:
+        return '1m'
+    if action == actions.delete:
+        return '1m'
```

### Comparing `hcs-cli-0.1.47/vhcs/plan/provider/hcs/site.py` & `hcs-cli-0.1.48/vhcs/plan/provider/azure/public_ip.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,29 +10,39 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from vhcs.plan import actions
-from vhcs.service import portal
+from azure.core.exceptions import ResourceNotFoundError
+from ._az_facade import network_management_client as client, adjust_tags
 
 def deploy(data: dict, state: dict) -> dict:
-    return portal.site.create(data)
+    name = data['name']
+    resource_group = data['resourceGroup']
+    parameters = adjust_tags(data['parameters'])
+
+    return client().public_ip_addresses.begin_create_or_update(
+        resource_group,
+        name,
+        parameters
+    ).result()
 
 def refresh(data: dict, state: dict) -> dict:
-    org_id = data['orgId']
-    if state:
-        id = state.get('id')
-        if id:
-            ret = portal.site.get(id, org_id)
-            if ret:
-                return ret
-    
-    # Fall back with smart find by name
-    return portal.site.find_by_name(data['name'], org_id)
+    name = data['name']
+    resource_group = data['resourceGroup']
+    try:
+        return client().public_ip_addresses.get(resource_group, name)
+    except ResourceNotFoundError:
+        pass
 
 def decide(data: dict, state: dict):
-    return actions.skip
+    return actions.create
+
+def destroy(data: dict, state: dict, force: bool) -> dict:
+    name = data['name']
+    resource_group = data['resourceGroup']
+    client().public_ip_addresses.begin_delete(resource_group, name).wait()
 
-def destroy(data: dict, state: dict) -> dict:
-    return portal.site.delete(state['id'], data['orgId'])
+def eta(action: str, data: dict, state: dict):
+    return '1m'
```

### Comparing `hcs-cli-0.1.47/vhcs/plan/provider/hcs/uag.py` & `hcs-cli-0.1.48/vhcs/plan/provider/hcs/uag.py`

 * *Files 14% similar despite different names*

```diff
@@ -49,13 +49,19 @@
 
 
 def decide(data: dict, state: dict):
     if state["status"] in ["READY"]:
         return actions.skip
 
 
-def destroy(data: dict, state: dict) -> dict:
+def destroy(data: dict, state: dict, force: bool) -> dict:
     id = state["id"]
     org_id = data["orgId"]
     admin.uag.delete(id, org_id)
     admin.uag.wait_for_deleted(id, org_id, '10m')
     
+def eta(action: str, data: dict, state: dict):
+    if action == actions.create:
+        return '10m'
+    if action == actions.delete:
+        return '10m'
+
```

### Comparing `hcs-cli-0.1.47/vhcs/service/_util.py` & `hcs-cli-0.1.48/vhcs/service/_util.py`

 * *Files 21% similar despite different names*

```diff
@@ -105,39 +105,73 @@
         sleep_seconds = remaining_seconds
         if sleep_seconds > polling_interval_seconds:
             sleep_seconds = polling_interval_seconds
         time.sleep(sleep_seconds)
 
 
 
-def wait_for_res_status(resource_name: str, fn_get: Callable, get_status: str | Callable, status_map: dict, timeout: str | int, polling_interval_seconds: int = 20):
+def wait_for_res_status(resource_name: str, 
+                        fn_get: Callable, 
+                        get_status: str | Callable, 
+                        status_map: dict = None, 
+                        is_ready: Callable = None, 
+                        is_error: Callable = None, 
+                        is_transition: Callable = None, 
+                        timeout: str | int = '10m', 
+                        polling_interval: str | int = '20s',
+                        not_found_as_success: bool = False):
     timeout_seconds = _parse_timeout(timeout)
+    polling_interval_seconds = _parse_timeout(polling_interval)
+    if polling_interval_seconds < 3:
+        polling_interval_seconds = 3
     start = time.time()
     prefix = f"Error waiting for resource {resource_name}: "
 
-    if isinstance(status_map['ready'], str):
-        status_map['ready'] = [status_map['ready']]
-    if isinstance(status_map['transition'], str):
-        status_map['transition'] = [status_map['transition']]
-    if isinstance(status_map['error'], str):
-        status_map['error'] = [status_map['error']]
+    if isinstance(get_status, str):
+        field_name = get_status
+        get_status = lambda t: t[field_name]
+    if status_map:
+        if isinstance(status_map['ready'], str):
+            status_map['ready'] = [status_map['ready']]
+        if isinstance(status_map['transition'], str):
+            status_map['transition'] = [status_map['transition']]
+        if isinstance(status_map['error'], str):
+            status_map['error'] = [status_map['error']]
+        if is_ready:
+            raise Exception("Can not specify is_ready when status_map is provided.")
+        if is_error:
+            raise Exception("Can not specify is_error when status_map is provided.")
+        if is_transition:
+            raise Exception("Can not specify is_transition when status_map is provided.")
+        is_ready = lambda s: s in status_map['ready']
+        is_error = lambda s: s in status_map['error']
+        is_transition = lambda s: s in status_map['transition']
+    else:
+        if not is_ready:
+            raise Exception("Either status_map or is_ready must be specified.")
+        if not is_error:
+            raise Exception("Either status_map or is_error must be specified.")
+        if not is_transition:
+            raise Exception("Either status_map or is_transition must be specified.")
 
     while True:
         t = fn_get()
         if t == None:
+            if not_found_as_success:
+                return
             raise RuntimeError(prefix + "Not found.")
-        if isinstance(get_status, str):
-            status = t[get_status]
-        else:
-            status = get_status(t)
-        if status in status_map['error']:
-            raise RuntimeError(prefix + f"Status error. Actual={status}, expected={status_map['ready']}")
-        if status in status_map['ready']:
+        status = get_status(t)
+        if is_error(status):
+            msg = prefix + f"Status error. Actual={status}"
+            if status_map:
+                msg += f", expected={status_map['ready']}"
+            raise RuntimeError(msg)
+        if is_ready(status):
             return t
-        if status not in status_map['transition']:
+        if not is_transition(status):
             raise RuntimeError(prefix + f"Unexpected status: {status}. If this is a transition, add it to status_map['transition'].")
 
         now = time.time()
         remaining_seconds = timeout_seconds - (now - start)
         if remaining_seconds < 1:
             raise TimeoutError(prefix + "Timeout.")
         sleep_seconds = remaining_seconds
```

### Comparing `hcs-cli-0.1.47/vhcs/service/admin/ad.py` & `hcs-cli-0.1.48/vhcs/service/admin/ad.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/service/admin/azure_infra.py` & `hcs-cli-0.1.48/vhcs/service/admin/azure_infra.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/service/admin/edge.py` & `hcs-cli-0.1.48/vhcs/service/admin/template.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,77 +9,49 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-import httpx
-import logging
 from .._util import hdc_service_client, default_crud, wait_for_res_status
-from . import edge
-
-log = logging.getLogger(__name__)
+from vhcs.util.query_util import with_query, PageRequest
 
 _client = hdc_service_client("admin")
-_crud = default_crud(_client, "/v2/edge-deployments", 'edge')
-
+_crud = default_crud(_client, "/v2/templates", 'template')
 get = _crud.get
 list = _crud.list
-delete = _crud.delete
-create = _crud.create
-wait_for_deleted = _crud.wait_for_deleted
-def wait_for(id: str, org_id: str, is_ready, timeout: str | int = '20m'):
-    def fn_get():
-        ret = get(id, org_id)
-        #log.info("Edge status: %s", ret['status'])
-        return ret
-    is_error = lambda t: t['status'] in ['CREATE_FAILED']
-    name = 'edge/' + id
-    return wait_for_res_status(fn_get, name, is_ready, is_error, timeout, polling_interval_seconds=60)
-
-def safe_delete(id: str, org_id: str, timeout: str | int = '20m'):
-
-    try:
-        edge.delete(id, org_id=org_id)
-    except httpx.HTTPStatusError as e:
-        if e.response.status_code != 409:
-            raise
-        _wait_for_terminal_state(id, org_id, timeout)
-        edge.delete(id, org_id=org_id)
-
-    edge.wait_for_deleted(id, org_id, "10m")
-
-def _wait_for_terminal_state(id, org_id, timeout):
-    name = 'edge/' + id
-    terminal_status = ['CREATE_FAILED', 'DELETED', 'DELETE_FAILED', 'MIGRATE_FAILED', 'READY', 'REPAIR_FAILED', 'UPDATE_FAILED', 'UPGRADE_FAILED']
-    transition_status = [
-        'CONNECT_PENDING', 
-        'CREATE_ACCEPTED', 
-        'CREATE_PENDING', 
-        'CREATING',  
-        'DELETE_PENDING', 
-        'DELETING', 
-        'FORCE_DELETE_PENDING', 
-        'FORCE_DELETING', 
-        'FORCE_REPAIR_ACCEPTED', 
-        'FORCE_REPAIR_PENDING', 
-        'MIGRATE_PENDING', 
-        'MIGRATING', 
-        'POST_PROVISIONING_CONFIG_IN_PROGRESS', 
-        'REPAIRING', 
-        'REPAIR_ACCEPTED', 
-        'REPAIR_PENDING',
-        'UPDATE_PENDING', 
-        'UPDATING', 
-        'UPGRADE_PENDING', 
-        'UPGRADING'
-    ]
-    def fn_get():
-        return get(id, org_id)
+
+def create(payload):
+    return _crud.create(payload, ignore_warnings=True)
+
+def delete(id: str, org_id: str, force: bool = True):
+    return _crud.delete(id, org_id, force=force)
+
+def wait_for_ready(id: str, org_id: str, timeout: str | int = '10m'):
+    name = 'template/' + id
+    fn_get = lambda: get(id, org_id)
+    fn_get_status = lambda t: t['reportedStatus'].get('statusValue')
     status_map = {
-        'ready': terminal_status,
-        'error': [],
-        'transition': transition_status
+        'ready': 'READY',
+        'error': 'ERROR',
+        'transition': ['EXPANDING', 'SHRINKING', 'INIT']
+        # Unexpected:
+        # DELETING
     }
-    
-    wait_for_res_status(name, fn_get, 'status', status_map, timeout)
+    return wait_for_res_status(resource_name=name, 
+                               fn_get=fn_get, 
+                               get_status=fn_get_status, 
+                               status_map=status_map, 
+                               timeout=timeout)
+
+wait_for_deleted = _crud.wait_for_deleted
+
+def list_vms(template_id: str, **kwargs):
+    def _get_page(query_string):
+        url = f"/v2/templates/{template_id}/vms?" + query_string
+        return _client.get(url)
+    return PageRequest(_get_page, **kwargs).get()
+
+def get_vm(template_id: str, vm_id: str, **kwargs):
+    url = with_query(f"/v2/templates/{template_id}/vms/{vm_id}", **kwargs)
+    return _client.get(url)
```

### Comparing `hcs-cli-0.1.47/vhcs/service/admin/helper.py` & `hcs-cli-0.1.48/vhcs/service/admin/helper.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/service/admin/provider.py` & `hcs-cli-0.1.48/vhcs/service/admin/provider.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/service/admin/template.py` & `hcs-cli-0.1.48/vhcs/service/inventory/vm.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,45 +9,30 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from .._util import hdc_service_client, default_crud, wait_for_res_status
+from .._util import hdc_service_client
 from vhcs.util.query_util import with_query, PageRequest
 
-_client = hdc_service_client("admin")
-_crud = default_crud(_client, "/v2/templates", 'template')
-get = _crud.get
-list = _crud.list
+_client = hdc_service_client("inventory")
 
-def create(payload):
-    return _crud.create(payload, ignore_warnings=True)
-
-def delete(id: str, org_id: str, force: bool = True):
-    return _crud.delete(id, org_id, force=force)
-
-def wait_for_ready(id: str, org_id: str, timeout_seconds: int = 600):
-    name = 'template/' + id
-    fn_get = lambda: get(id, org_id)
-    fn_get_status = lambda t: t['reportedStatus'].get('statusValue')
-    status_map = {
-        'ready': 'READY',
-        'error': 'ERROR',
-        'trasition': ['EXPANDING', 'SHRINKING', 'INIT']
-        # Unexpected:
-        # DELETING
-    }
-    return wait_for_res_status(name, fn_get, fn_get_status, status_map, timeout_seconds)
-
-wait_for_deleted = _crud.wait_for_deleted
+@staticmethod
+def get(template_id: str, vm_id: str, org_id: str = None, **kwargs):
+    url = f"/v1/{template_id}/{vm_id}"
+    if org_id:
+        url += "?org_id=" + org_id
+    url = with_query(url, **kwargs)
+    return _client.get(url)
 
-def list_vms(template_id: str, **kwargs):
+@staticmethod
+def list(template_id: str, org_id: str, **kwargs):
     def _get_page(query_string):
-        url = f"/v2/templates/{template_id}/vms?" + query_string
+        url = f"/v1/{template_id}?org_id={org_id}"
+        if query_string:
+            url += "&" + query_string
+        print(url)
         return _client.get(url)
-    return PageRequest(_get_page, **kwargs).get()
 
-def get_vm(template_id: str, vm_id: str, **kwargs):
-    url = with_query(f"/v2/templates/{template_id}/vms/{vm_id}", **kwargs)
-    return _client.get(url)
+    return PageRequest(_get_page, **kwargs).get()
```

### Comparing `hcs-cli-0.1.47/vhcs/service/admin/uag.py` & `hcs-cli-0.1.48/vhcs/service/admin/uag.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,8 +57,12 @@
         # 'UPDATE_FAILED', 
         # 'UPDATE_PENDING', 
         # 'UPDATING', 
         # 'UPGRADE_FAILED', 
         # 'UPGRADE_PENDING', 
         # 'UPGRADING'
     }
-    return wait_for_res_status(name, fn_get, 'status', status_map, timeout)
+    return wait_for_res_status(resource_name=name, 
+                               fn_get=fn_get, 
+                               get_status='status', 
+                               status_map=status_map, 
+                               timeout=timeout)
```

### Comparing `hcs-cli-0.1.47/vhcs/service/auth/admin.py` & `hcs-cli-0.1.48/vhcs/service/auth/admin.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/service/ims/helper.py` & `hcs-cli-0.1.48/vhcs/service/ims/helper.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import time
+import httpx
 from . import images, image_copies
 from .version import version
 
 def get_images_by_provider_instance_with_asset_details(providerInstanceId: str, org_id: str):
     all_images = images.list(org_id)
     copies = image_copies.list(org_id, include_catalog_details=True,
                       search=f"providerInstanceId $eq {providerInstanceId}")
@@ -29,37 +30,38 @@
                 # add additional info
                 image['_assetDetails'] = copy['assetDetails']
                 ret.append(image)
                 break
     return ret
 
 def delete_images(image_ids: list[str], org_id: str, timeout: int | str):
-    import httpx
-    
-    
-    def del_impl(image_id: str, tolerant: bool):
+    def del_impl(image_id: str):
         version_api = version(image_id, org_id)
         versions = version_api.list()
         everything_ok = True
         for v in versions:
-            if v['status'] == 'DELETING':
+            s = v['status']
+            if s == 'DELETING':
                 continue
+            # AVAILABLE, DELETING, DISABLED, FAILED, IMPORT_COMPLETE, IMPORT_IN_PROGRESS, PARTIALLY_AVAILABLE, PENDING, PUBLISH_IN_PROGRESS, REPLICATION_IN_PROGRESS
             try:
                 version_api.delete(v['id'])
             except httpx.HTTPStatusError:
-                if tolerant:
-                    everything_ok = False
-                    pass
-                else:
-                    raise
+                everything_ok = False
         return everything_ok
 
-    for image_id in image_ids:
-        if not del_impl(image_id, tolerant=True):
-            time.sleep(1)
-            del_impl(image_id, tolerant=False)
-    
+    to_delete = list(image_ids)
+
+    while True:
+        temp = list(to_delete)
+        for image_id in temp:
+            if del_impl(image_id):
+                to_delete.remove(image_id)
+        if not to_delete:
+            break
+        time.sleep(60)
+        
     if timeout == '0':
         return
     
     for image_id in image_ids:
         images.wait_for_deleted(image_id, org_id, timeout)  # todo: timeout
```

### Comparing `hcs-cli-0.1.47/vhcs/service/ims/image_copies.py` & `hcs-cli-0.1.48/vhcs/service/ims/image_copies.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/service/ims/images.py` & `hcs-cli-0.1.48/vhcs/service/ims/images.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,8 +37,12 @@
     fn_get = lambda: get(image_id, org_id)
     unexpected_status = set(['IMPORT_COMPLETE', 'AVAILABLE', 'FAILED', 'DELETING', 'DISABLED', 'REPLICATION_IN_PROGRESS', 'PARTIALLY_AVAILABLE'])
     status_map = {
         'ready': expected_status,
         'transition': ['IN_PROGRESS', 'PUBLISH_IN_PROGRESS', 'PENDING'],
         'error': builtins.list(unexpected_status - set(expected_status))
     }
-    return wait_for_res_status(res_name, fn_get, 'status', status_map, timeout="15m")
+    return wait_for_res_status(resource_name=res_name, 
+                               fn_get=fn_get, 
+                               get_status='status', 
+                               status_map=status_map, 
+                               timeout="60m")
```

### Comparing `hcs-cli-0.1.47/vhcs/service/ims/version.py` & `hcs-cli-0.1.48/vhcs/service/ims/version.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,8 +62,12 @@
         def fn_get():
             return self.get(id)
         status_map = {
             'ready': ['AVAILABLE'],
             'transition': ['IMPORT_COMPLETE', 'IMPORT_IN_PROGRESS', 'PENDING', 'PUBLISH_IN_PROGRESS', 'REPLICATION_IN_PROGRESS'],
             'error': ['FAILED', 'DELETING', 'DISABLED', 'PARTIALLY_AVAILABLE']
         }
-        wait_for_res_status(res_name, fn_get, 'status', status_map, timeout)
+        wait_for_res_status(resource_name=res_name, 
+                            fn_get=fn_get, 
+                            get_status='status', 
+                            status_map=status_map, 
+                            timeout=timeout)
```

### Comparing `hcs-cli-0.1.47/vhcs/service/inventory/vm.py` & `hcs-cli-0.1.48/vhcs/service/portal/site.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,30 +9,40 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
+import logging
 from .._util import hdc_service_client
 from vhcs.util.query_util import with_query, PageRequest
 
-_client = hdc_service_client("inventory")
+log = logging.getLogger(__name__)
+_client = hdc_service_client("portal")
 
-@staticmethod
-def get(template_id: str, vm_id: str, org_id: str = None, **kwargs):
-    url = f"/v1/{template_id}/{vm_id}"
-    if org_id:
-        url += "?org_id=" + org_id
-    url = with_query(url, **kwargs)
+
+def create(payload: dict):
+    url = "/v2/sites"
+    return _client.post(url, payload)
+
+def get(id: str, org_id: str):
+    url = f"/v2/sites/{id}?org_id={org_id}"
+    return _client.get(url)
+
+def list(**kwargs):
+    url = with_query(f"/v2/sites", **kwargs)
     return _client.get(url)
 
-@staticmethod
-def list(template_id: str, org_id: str, **kwargs):
-    def _get_page(query_string):
-        url = f"/v1/{template_id}?org_id={org_id}"
-        if query_string:
-            url += "&" + query_string
-        print(url)
-        return _client.get(url)
+def delete(id: str, org_id: str):
+    url = f"/v2/sites/{id}?org_id={org_id}"
+    return _client.delete(url)
 
-    return PageRequest(_get_page, **kwargs).get()
+def find_by_name(name: str, org_id: str):
+    sites = list(org_id=org_id)
+    for s in sites:
+        if s.get('name') == name:
+            return s
+    
+def set_edge(site_id: str, org_id: str, edge_deployment_id: str):
+    url = f"/v1/sites/{site_id}/edge/{edge_deployment_id}"
+    return _client.put(url, {})
```

### Comparing `hcs-cli-0.1.47/vhcs/service/lcm/provider.py` & `hcs-cli-0.1.48/vhcs/service/lcm/provider.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/service/lcm/template.py` & `hcs-cli-0.1.48/vhcs/service/lcm/template.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/service/org_service/datacenter.py` & `hcs-cli-0.1.48/vhcs/service/org_service/datacenter.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/service/org_service/details.py` & `hcs-cli-0.1.48/vhcs/service/org_service/details.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/service/pki/certificate.py` & `hcs-cli-0.1.48/vhcs/service/pki/certificate.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/service/portal/entitlement.py` & `hcs-cli-0.1.48/vhcs/service/portal/entitlement.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/service/portal/pool.py` & `hcs-cli-0.1.48/vhcs/service/portal/pool.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/service/vmhub/otp.py` & `hcs-cli-0.1.48/vhcs/service/vmhub/otp.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/support/daas/cidr_util.py` & `hcs-cli-0.1.48/vhcs/support/daas/cidr_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/support/daas/helper.py` & `hcs-cli-0.1.48/vhcs/support/daas/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     prev = data_util.load_data_file(file_name)
     if prev:
         prev_vars = prev.get('vars')
         if prev_vars:
             data_util.deep_apply_defaults(input_data['vars'], prev_vars)
 
     # Add defaults from shared infra config, if anything missing
-    data_util.deep_apply_defaults(input_data, infra.all())
+    data_util.deep_apply_defaults(input_data, infra.get())
     
     # Enforce key values
     input_data['deploymentId'] = deployment_id
     input_data['vars']['orgId'] = _get_org_id()
     
     def create_file(success):
         # Combine and save
```

### Comparing `hcs-cli-0.1.47/vhcs/support/daas/infra.py` & `hcs-cli-0.1.48/vhcs/support/daas/infra.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,38 +14,18 @@
 """
 
 from vhcs.common.ctxp import context
 
 
 _config_name = "daas-infra"
 
-def set(k: str, v: str):
-
-    data = context.get(_config_name, default={})
-    data = _with_default(data, _config_template)
-
-    data[k] = v
-    context.set(_config_name, data)
-
-def unset(k: str):
-
-    data = context.get(_config_name, default={})
-    data = _with_default(data, _config_template)
-
-    if k in data:
-        del data[k]
-        context.set(_config_name, data)
-
-def get(k: str):
-    return _get_config().get(k)
-
-def all():
+def get():
     return _get_config()
 
-def save(data: dict):
+def set(data: dict):
     return context.set(_config_name, data)
 
 def file():
     data = _get_config()
     context.set(_config_name, data)
     return context.file(_config_name)
 
@@ -56,17 +36,15 @@
 def _with_default(target : dict, default : dict) -> dict:
     ret = dict(default)
     ret.update(target)
     return ret
 
 _config_template = {
 	"provider": {
-		"id": "",
-		"applicationId": "",
-		"applicationKey": ""
+		"id": ""
 	},
 	"network": {
 		"vNetId": "",
 		"tenantCIDRs": []
 	},
 	"desktop": {
 		"markerId": "",
```

### Comparing `hcs-cli-0.1.47/vhcs/support/daas/infra_calc.py` & `hcs-cli-0.1.48/vhcs/support/daas/infra_reuse.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,20 +39,20 @@
         region = data['newProvider']['region']
         provider_id = state['output']['myProvider']['id']
 
     # identify subnets
     subnet_map = _prepare_subnet_map(data['network']['vNetId'])
 
     edge = {
-        'managementNetwork': subnet_map[data['edge']['managementNetwork']]
+        'managementNetwork': subnet_map[data['network']['managementNetworkName']]
     }
     uag = {
-        'managementNetwork': subnet_map[data['uag']['managementNetwork']],
-        'dmzNetwork': subnet_map[data['uag']['dmzNetwork']],
-        'desktopNetwork': subnet_map[data['uag']['desktopNetwork']],
+        'managementNetwork': subnet_map[data['network']['managementNetworkName']],
+        'dmzNetwork': subnet_map[data['network']['dmzNetworkName']],
+        'desktopNetwork': subnet_map[data['network']['desktopNetworkName']],
     }
     image = {
         'desktopSubnetId': uag['desktopNetwork']['id'],
         'desktopPassword': [c for c in data['desktop']['adminPassword']],
         'multiSessionImageName': _generate_image_name('m'),
         'desktopImageName': _generate_image_name('d'),
     }
@@ -107,9 +107,12 @@
     first_part = text[:limit - 4]
     second_part = text[limit - 4:]
 
     sha256_hash = hashlib.sha256(second_part.encode()).hexdigest()
     truncated_hash = sha256_hash[:3]
     return first_part + '-' + truncated_hash
 
-def destroy(data: dict, prev: dict):
-    return
+def destroy(data: dict, pstaterev: dict):
+    return
+
+def eta(action: str, data: dict, state: dict):
+    return '1m'
```

### Comparing `hcs-cli-0.1.47/vhcs/support/daas/templates/v1/infra.vars.yml` & `hcs-cli-0.1.48/vhcs/support/daas/templates/v1/infra-reuse.vars.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-deploymentId: infra
+deploymentId: 
 vars:
   orgId: 
+  region: 
   provider:
-    id: null
+    id: 
   newProvider:
     subscriptionId: 
-    region: 
     directoryId: 
     applicationId: 
     applicationKey: 
   network:
-    vNetId:
+    vNetId: 
     tenantCIDRs: []
+    cidr:
+    managementNetworkName: 
+    dmzNetworkName: 
+    desktopNetworkName: 
   edge:
     privateDNS: titan.vmware.com
     managedIdentityId: 
-    managementNetwork: mgmt-1
-  uag:
-    managementNetwork: mgmt-1
-    dmzNetwork: dmz
-    desktopNetwork: desktop-76
-
+  uag: {}
   desktop:
-    markerId: null
-    streamId: null
-    templateType: null
-    vmSkuName: null
-    userGroup: hcs-user-group
+    adminUsername: localadmin
+    adminPassword: Hellomortal1!
+    markerId: 
+    streamId: 
+    templateType: 
+    vmSkuName: 
+    userGroup: 
+
```

### Comparing `hcs-cli-0.1.47/vhcs/support/daas/templates/v1/tenant.blueprint.yml` & `hcs-cli-0.1.48/vhcs/support/daas/templates/v1/tenant.blueprint.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,105 +1,109 @@
 # 'defaults' is a group of variables that are calculated and referenced by multiple resources.
 # The defaults helps to deduplicate calculated variables, and 
 defaults:
-  name: titan-lite-${deploymentId}
+  name: tltenant-${deploymentId}
   tags:
     deployment: ${deploymentId}
     managed-by: titan-lite
 
 # The providers section specifies provider-specific data. Normally this required to initialize
 # a provider.
 providers:
-  - type: azure
-    data: ${vars.provider}
-  - type: hcs
-    data:
+  azure:
+    data: ${tenantCalc.provider}
 
-resources:
-  myRuntime:
-    kind: runtime/vhcs.support.daas.tenant_calc # Custom calculation of values
+runtimes:
+  tenantCalc:
+    impl: vhcs.support.daas.tenant_calc # Custom calculation of values
     data: ${vars} # Take the entire unchanged vars as input
 
+resources:
   myRg:
     kind: azure/resource-group
     data:
       name: ${defaults.name}
-      location: ${myRuntime.location}
-      tags: ${defaults.tags}
+      parameters:
+        name: ${defaults.name}
+        location: ${tenantCalc.location}
+        tags: ${defaults.tags}
 
   myNsg:
     kind: azure/nsg
     data:
-      name: ${myRg.name}
-      location: ${myRuntime.location}
-      resourceGroup: ${myRuntime.vNet.resourceGroup}
-      tags: ${defaults.tags}
+      name: ${defaults.name}
+      resourceGroup: ${tenantCalc.vNet.resourceGroup}
+      parameters:
+        location: ${tenantCalc.location}
+        tags: ${defaults.tags}
 
   mySubnet:
     kind: azure/subnet
     data:
       name: ${defaults.name}
-      resourceGroup: ${myRuntime.vNet.resourceGroup}
-      vNetName: ${myRuntime.vNet.name}
-      cidr: ${myRuntime.cidr}
-      nsgName: ${myNsg.NewNSG.name}
+      resourceGroup: ${tenantCalc.vNet.resourceGroup}
+      vNetName: ${tenantCalc.vNet.name}
+      parameters:
+        address_prefix: ${tenantCalc.cidr}
+        network_security_group:
+          id: ${myNsg.id}
 
   myAADGroup:
     kind: azure/aad-group
     data:
       displayName: ${defaults.name}
       mailNickname: ${defaults.name}
       description:
       parentGroup: ${vars.desktop.userGroup}
   
   myAADUser:
     kind: azure/aad-user
     for: email in vars.userEmails
     data:
       group: ${myAADGroup.id}
-      domainName: ${myRuntime.orgIdpMap.domains[0]}
+      domainName: ${tenantCalc.orgIdpMap.domains[0]}
 
   myTemplate:
     kind: hcs/pool-template
     data:
-      providerInstanceId: ${vars.provider.id}
-      uagDeploymentId: ${myRuntime.template.uag_deployment_id}
-      edgeDeploymentId: ${myRuntime.template.edge_deployment_id}
+      providerInstanceId: ${tenantCalc.provider.id}
+      uagDeploymentId: ${tenantCalc.template.uag_deployment_id}
+      edgeDeploymentId: ${tenantCalc.template.edge_deployment_id}
       orgId: ${vars.orgId}
       name: ${defaults.name}
       vmNamePattern: d-
       templateType: ${vars.desktop.templateType}
       applicationProperties:
         azureActiveDirectoryJoined: 'true'
       networks:
       - kind: subnets
         id: ${mySubnet.id}
         data:
           parent: ${mySubnet.id}
           name: ${mySubnet.name}
           availableIpAddresses: 250
-          cidr: ${myRuntime.cidr}
+          cidr: ${tenantCalc.cidr}
       imageReference:
         streamId: ${vars.desktop.streamId}
         markerId: ${vars.desktop.markerId}
       licenseProvided: true
       desktopAdminUsername: hcs-admin
-      desktopAdminPassword: ${myRuntime.template.password}
+      desktopAdminPassword: ${tenantCalc.template.password}
       diskEncryption:
         enabled: false
       sparePolicy:
-        limit: ${myRuntime.template.total_vms}
-        max: ${myRuntime.template.total_vms}
-        min: ${myRuntime.template.total_vms}
-      sessionsPerVm: ${myRuntime.number_of_users}
+        limit: ${tenantCalc.template.total_vms}
+        max: ${tenantCalc.template.total_vms}
+        min: ${tenantCalc.template.total_vms}
+      sessionsPerVm: ${tenantCalc.number_of_users}
       vmLicenseType: WINDOWS_CLIENT
       diskSizeInGB: 127
       infrastructure:
         vmSkus:
-        - ${myRuntime.template.vm_sku}
+        - ${tenantCalc.template.vm_sku}
 
   myPoolGroup:
     kind: hcs/pool-group
     data:
       orgId: ${vars.orgId}
       name: ${defaults.name}
       type: DESKTOP
@@ -125,11 +129,11 @@
       userIds: "${[for u in myAADUser: u.id]}"
 
   myLaunchItem:
     kind: hcs/launch-item
     data:
       users: ${myAADUser}
       entitlementId: ${myPoolGroup.name}
-      domainName: ${myRuntime.orgIdpMap.idpTenantDomain}
+      domainName: ${tenantCalc.orgIdpMap.idpTenantDomain}
       stackUrl: ${profile.hcs.url}
     after:
     - myEntitlement
```

### Comparing `hcs-cli-0.1.47/vhcs/support/daas/tenant_calc.py` & `hcs-cli-0.1.48/vhcs/support/daas/tenant_calc.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,35 +11,38 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import logging
 from vhcs.service import admin, auth
 from vhcs.plan.provider.azure import _az_facade as az
-from vhcs.plan import PlanException
+from vhcs.plan import PluginException
 from .cidr_util import find_available_cidr_24
 
 log = logging.getLogger(__name__)
 
 def process(data: dict, state: dict) -> dict:
-    provider = data['provider']
-    provider_id = provider['id']
-    log.info('Provider: %s', provider_id)
-    providerInstance = admin.provider.get('azure', provider_id)
-    if not providerInstance:
-        raise PlanException('Provider not found: ' + provider_id)
-    providerData = providerInstance['providerDetails']['data']
+    import time
+    time.sleep(10)
+    org_id = data['orgId']
+    edge = admin.edge.get(data['edgeId'], org_id)
+    provider_id = edge['providerInstanceId']
+    # log.info('Provider: %s', provider_id)
+    provider = admin.provider.get('azure', provider_id, org_id)
+    if not provider:
+        raise PluginException('Provider not found: ' + provider_id)
+    providerData = provider['providerDetails']['data']
     subscription_id = providerData['subscriptionId']
-    directory_id = providerData['directoryId']
-    application_id = providerData['applicationId']
+    # directory_id = providerData['directoryId']
+    # application_id = providerData['applicationId']
     region = providerData['region']
-    log.info('Subscription: %s', subscription_id)
-    log.info('Directory: %s', directory_id)
-    log.info('ApplicationId: %s', application_id)
-    log.info('Region: %s', region)
+    # log.info('Subscription: %s', subscription_id)
+    # log.info('Directory: %s', directory_id)
+    # log.info('ApplicationId: %s', application_id)
+    # log.info('Region: %s', region)
 
     template_type = data['desktop']['templateType']
     number_of_users = len(data['userEmails'])
     is_multi_session = "MULTI_SESSION" == template_type
 
     uag_deployments = admin.helper.list_resources_by_provider('uag-deployments', provider_id, limit=1)
     if not uag_deployments:
@@ -61,43 +64,58 @@
         'password': _generate_password(),
         'uag_deployment_id': uag_deployment_id,
         'edge_deployment_id': edge_deployment_id,
         'vm_sku': vm_skus[0]
     }
 
     org_idp_map = auth.admin.get_org_idp_map()
-    cidr = _calculate_cidr(data)
+    vnet = az.network.vnet.get(edge['infrastructure']['managementNetwork']['data']['parent'])
+    cidr = _calculate_cidr(vnet)
     log.info('Calculated network address: %s', cidr)
     return {
         'location': region,
         'cidr': cidr,
-        'vNet': az.network.vnet.get(data['network']['vNetId']),
-        'providerInstance': providerInstance,
+        'vNet': vnet,
+        'provider': {
+            'id': provider_id,
+            'subscriptionId': subscription_id
+        },
         'template': template,
         'number_of_users': number_of_users,
         'orgIdpMap': org_idp_map
     }
 
 def _generate_password():
     from random import choice
     upper_chars = "ABCDEFGHJKLMNPQRSTUVWXY"
     readable_chars = "abcdefghjklmnpqrstuvwxy3456789"
     special_chars = "!@#$%_"
     return '' + choice(upper_chars) + ''.join(choice(readable_chars) for i in range(12)) + choice(special_chars)
 
-def _calculate_cidr(data):
-    network_cfg = data['network']
-
-    vnet = az.network.vnet.get(network_cfg['vNetId'])
+def _calculate_cidr(vnet):
     vnet_cidrs = vnet['addressSpace']['addressPrefixes']
     used_cidrs = []
     for subnet in vnet['subnets']:
         used_cidrs.append(subnet['addressPrefix'])
-    configured_cidrs = network_cfg['tenantCIDRs']
-
-    tenant_cidr = find_available_cidr_24(vnet_cidrs, used_cidrs, configured_cidrs)
+    # https://confluence.eng.vmware.com/display/HCS/Titan+Lite+-+BOM#TitanLiteBOM-AddressSpaces
+    infra_cidr = None
+    for c in vnet_cidrs:
+        if not c.endswith(".0/16"):
+            continue
+        infra_cidr = c
+        break
+    if not infra_cidr:
+        raise PluginException("No /16 CIDR found in vNet.")
+    
+    prefix = infra_cidr[:infra_cidr.rindex('.')]
+    reserved_cidr = prefix + '.0/24'
+    used_cidrs.append(reserved_cidr)
+    tenant_cidr = find_available_cidr_24(vnet_cidrs, used_cidrs, [infra_cidr])
     if not tenant_cidr:
-        raise PlanException("Unable to find usable subnet address space for the tenant. Consider adding new address space to the config via 'hcs daas infra plan', and/or add new spaces in vnet.")
+        raise PluginException("Unable to find usable subnet address space for the tenant. Consider adding new address space to the config via 'hcs daas infra plan', and/or add new spaces in vnet.")
     return tenant_cidr
 
-def destroy(data: dict, prev: dict):
-    return
+def destroy(data: dict, state: dict):
+    return
+
+def eta(action: str, data: dict, state: dict):
+    return '1m'
```

### Comparing `hcs-cli-0.1.47/vhcs/support/plan_util.py` & `hcs-cli-0.1.48/vhcs/support/plan_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/support/profile.py` & `hcs-cli-0.1.48/vhcs/support/profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/util/check_license.py` & `hcs-cli-0.1.48/vhcs/util/check_license.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/util/duration.py` & `hcs-cli-0.1.48/vhcs/util/duration.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/util/pki_util.py` & `hcs-cli-0.1.48/vhcs/util/pki_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/util/query_util.py` & `hcs-cli-0.1.48/vhcs/util/query_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.47/vhcs/util/versions.py` & `hcs-cli-0.1.48/vhcs/util/versions.py`

 * *Files identical despite different names*

