# Comparing `tmp/python-gerrit-api-3.0.1.tar.gz` & `tmp/python-gerrit-api-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-gerrit-api-3.0.1.tar", last modified: Fri Jul  7 15:47:16 2023, max compression
+gzip compressed data, was "python-gerrit-api-3.0.2.tar", last modified: Mon Jul 31 06:46:19 2023, max compression
```

## Comparing `python-gerrit-api-3.0.1.tar` & `python-gerrit-api-3.0.2.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:47:16.032067 python-gerrit-api-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11513 2023-07-07 15:47:16.032067 python-gerrit-api-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10634 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:47:16.016067 python-gerrit-api-3.0.1/gerrit/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:47:16.020067 python-gerrit-api-3.0.1/gerrit/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18264 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/accounts/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/accounts/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/accounts/emails.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/accounts/gpg_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/accounts/ssh_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:47:16.020067 python-gerrit-api-3.0.1/gerrit/changes/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/changes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27375 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/changes/change.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/changes/changes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/changes/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/changes/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/changes/reviewers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:47:16.024067 python-gerrit-api-3.0.1/gerrit/changes/revision/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/changes/revision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12867 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/changes/revision/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/changes/revision/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/changes/revision/drafts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/changes/revision/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:47:16.024067 python-gerrit-api-3.0.1/gerrit/config/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/config/caches.py
--rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/config/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:47:16.028067 python-gerrit-api-3.0.1/gerrit/groups/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/groups/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/groups/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/groups/members.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/groups/subgroups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:47:16.028067 python-gerrit-api-3.0.1/gerrit/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/plugins/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:47:16.028067 python-gerrit-api-3.0.1/gerrit/projects/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/projects/branches.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/projects/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/projects/dashboards.py
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/projects/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)    14141 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/projects/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/projects/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/projects/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/projects/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:47:16.028067 python-gerrit-api-3.0.1/gerrit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/utils/gerritbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gerrit/utils/requester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:47:16.032067 python-gerrit-api-3.0.1/gitiles/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gitiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/gitiles/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:47:16.032067 python-gerrit-api-3.0.1/python_gerrit_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11513 2023-07-07 15:47:16.000000 python-gerrit-api-3.0.1/python_gerrit_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-07 15:47:16.000000 python-gerrit-api-3.0.1/python_gerrit_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 15:47:16.000000 python-gerrit-api-3.0.1/python_gerrit_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-07 15:47:16.000000 python-gerrit-api-3.0.1/python_gerrit_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-07 15:47:16.000000 python-gerrit-api-3.0.1/python_gerrit_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 15:47:16.032067 python-gerrit-api-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:47:16.032067 python-gerrit-api-3.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/tests/test_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/tests/test_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/tests/test_gitiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/tests/test_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/tests/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-07 15:47:03.000000 python-gerrit-api-3.0.1/tests/test_revision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:46:19.421979 python-gerrit-api-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11991 2023-07-31 06:46:19.421979 python-gerrit-api-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:46:19.409979 python-gerrit-api-3.0.2/gerrit/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:46:19.409979 python-gerrit-api-3.0.2/gerrit/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18261 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/accounts/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/accounts/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/accounts/emails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/accounts/gpg_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/accounts/ssh_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:46:19.413979 python-gerrit-api-3.0.2/gerrit/changes/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/changes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27372 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/changes/change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/changes/changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/changes/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/changes/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/changes/reviewers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:46:19.413979 python-gerrit-api-3.0.2/gerrit/changes/revision/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/changes/revision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12867 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/changes/revision/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/changes/revision/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/changes/revision/drafts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/changes/revision/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:46:19.413979 python-gerrit-api-3.0.2/gerrit/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/config/caches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/config/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:46:19.417979 python-gerrit-api-3.0.2/gerrit/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/groups/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/groups/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/groups/members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/groups/subgroups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:46:19.417979 python-gerrit-api-3.0.2/gerrit/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/plugins/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:46:19.417979 python-gerrit-api-3.0.2/gerrit/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/projects/branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/projects/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/projects/dashboards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/projects/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14138 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/projects/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/projects/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/projects/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/projects/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:46:19.417979 python-gerrit-api-3.0.2/gerrit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/utils/gerritbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6480 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gerrit/utils/requester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:46:19.417979 python-gerrit-api-3.0.2/gitiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gitiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/gitiles/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:46:19.421979 python-gerrit-api-3.0.2/python_gerrit_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11991 2023-07-31 06:46:19.000000 python-gerrit-api-3.0.2/python_gerrit_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-31 06:46:19.000000 python-gerrit-api-3.0.2/python_gerrit_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 06:46:19.000000 python-gerrit-api-3.0.2/python_gerrit_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-31 06:46:19.000000 python-gerrit-api-3.0.2/python_gerrit_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-31 06:46:19.000000 python-gerrit-api-3.0.2/python_gerrit_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 06:46:19.421979 python-gerrit-api-3.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:46:19.421979 python-gerrit-api-3.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/tests/test_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/tests/test_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/tests/test_gitiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/tests/test_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11532 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/tests/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-31 06:46:09.000000 python-gerrit-api-3.0.2/tests/test_revision.py
```

### Comparing `python-gerrit-api-3.0.1/LICENSE` & `python-gerrit-api-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.1/PKG-INFO` & `python-gerrit-api-3.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-gerrit-api
-Version: 3.0.1
+Version: 3.0.2
 Summary: Python wrapper for the Gerrit REST API.
 Home-page: https://github.com/shijl0925/python-gerrit-api
 Author: Jialiang Shi
 Author-email: kevin09254930sjl@gmail.com
 License: MIT
 Keywords: api gerrit client wrapper
 Classifier: Development Status :: 5 - Production/Stable
@@ -32,14 +32,18 @@
     :target: https://pepy.tech/project/python-gerrit-api
 .. image:: https://sonarcloud.io/api/project_badges/measure?project=shijl0925_python-gerrit-api&metric=alert_status
     :target: https://sonarcloud.io/dashboard?id=shijl0925_python-gerrit-api
 .. image:: https://sonarcloud.io/api/project_badges/measure?project=shijl0925_python-gerrit-api&metric=coverage
     :target: https://sonarcloud.io/summary/overall?id=shijl0925_python-gerrit-api
 .. image:: https://codecov.io/gh/shijl0925/python-gerrit-api/branch/master/graph/badge.svg?token=HU6U2LNHUK 
     :target: https://codecov.io/gh/shijl0925/python-gerrit-api
+.. image:: https://app.codacy.com/project/badge/Grade/fb3a59e09af8422ca2349b3974e02833
+    :target: https://app.codacy.com/gh/shijl0925/python-gerrit-api/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade
+.. image:: https://app.codacy.com/project/badge/Coverage/fb3a59e09af8422ca2349b3974e02833
+    :target: https://app.codacy.com/gh/shijl0925/python-gerrit-api/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage
 .. image:: https://img.shields.io/github/license/shijl0925/python-gerrit-api.svg
     :target: LICENSE
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 
 What is it?
 -----------
```

### Comparing `python-gerrit-api-3.0.1/README.rst` & `python-gerrit-api-3.0.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,18 @@
     :target: https://pepy.tech/project/python-gerrit-api
 .. image:: https://sonarcloud.io/api/project_badges/measure?project=shijl0925_python-gerrit-api&metric=alert_status
     :target: https://sonarcloud.io/dashboard?id=shijl0925_python-gerrit-api
 .. image:: https://sonarcloud.io/api/project_badges/measure?project=shijl0925_python-gerrit-api&metric=coverage
     :target: https://sonarcloud.io/summary/overall?id=shijl0925_python-gerrit-api
 .. image:: https://codecov.io/gh/shijl0925/python-gerrit-api/branch/master/graph/badge.svg?token=HU6U2LNHUK 
     :target: https://codecov.io/gh/shijl0925/python-gerrit-api
+.. image:: https://app.codacy.com/project/badge/Grade/fb3a59e09af8422ca2349b3974e02833
+    :target: https://app.codacy.com/gh/shijl0925/python-gerrit-api/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade
+.. image:: https://app.codacy.com/project/badge/Coverage/fb3a59e09af8422ca2349b3974e02833
+    :target: https://app.codacy.com/gh/shijl0925/python-gerrit-api/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage
 .. image:: https://img.shields.io/github/license/shijl0925/python-gerrit-api.svg
     :target: LICENSE
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 
 What is it?
 -----------
```

### Comparing `python-gerrit-api-3.0.1/gerrit/accounts/account.py` & `python-gerrit-api-3.0.2/gerrit/accounts/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 class GerritAccount(GerritBase):
     def __init__(self, account, gerrit):
         self.account = account
         self.gerrit = gerrit
         self.endpoint = f"/accounts/{self.account}"
-        GerritBase.__init__(self)
+        super().__init__(self)
 
     def __str__(self):
         return str(self.account)
 
     def get_detail(self):
         """
         fetch account info in more details, such as: registered_on
```

### Comparing `python-gerrit-api-3.0.1/gerrit/accounts/accounts.py` & `python-gerrit-api-3.0.2/gerrit/accounts/accounts.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.1/gerrit/accounts/emails.py` & `python-gerrit-api-3.0.2/gerrit/accounts/emails.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 class GerritAccountEmail(GerritBase):
     def __init__(self, email, account, gerrit):
         self.email = email
         self.account = account
         self.gerrit = gerrit
         self.endpoint = f"/accounts/{self.account}/emails/{self.email}"
-        GerritBase.__init__(self)
+        super().__init__(self)
 
     def __str__(self):
         return self.email
 
     def delete(self):
         """
         Deletes an email address of an account.
```

### Comparing `python-gerrit-api-3.0.1/gerrit/accounts/gpg_keys.py` & `python-gerrit-api-3.0.2/gerrit/accounts/gpg_keys.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 class GerritAccountGPGKey(GerritBase):
     def __init__(self, id, account, gerrit):
         self.id = id
         self.account = account
         self.gerrit = gerrit
         self.endpoint = f"/accounts/{self.account}/gpgkeys/{self.id}"
-        GerritBase.__init__(self)
+        super().__init__(self)
 
     def __str__(self):
         return self.id
 
     def delete(self):
         """
         Deletes a GPG key of a user.
```

### Comparing `python-gerrit-api-3.0.1/gerrit/accounts/ssh_keys.py` & `python-gerrit-api-3.0.2/gerrit/accounts/ssh_keys.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 class GerritAccountSSHKey(GerritBase):
     def __init__(self, seq, account, gerrit):
         self.seq = seq
         self.account = account
         self.gerrit = gerrit
         self.endpoint = f"/accounts/{self.account}/sshkeys"
-        GerritBase.__init__(self)
+        super().__init__(self)
 
     def __str__(self):
         return str(self.seq)
 
     def delete(self):
         """
         Deletes an SSH key of a user.
```

### Comparing `python-gerrit-api-3.0.1/gerrit/base.py` & `python-gerrit-api-3.0.2/gerrit/base.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.1/gerrit/changes/change.py` & `python-gerrit-api-3.0.2/gerrit/changes/change.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 class GerritChange(GerritBase):
     def __init__(self, id: str, gerrit):
         self.id = id
         self.gerrit = gerrit
         self.endpoint = f"/changes/{self.id}"
-        GerritBase.__init__(self)
+        super().__init__(self)
 
         self.revisions: Dict[str, str] = {}
         self.current_revision_number = 0
 
     def __str__(self):
         return self.id
```

### Comparing `python-gerrit-api-3.0.1/gerrit/changes/changes.py` & `python-gerrit-api-3.0.2/gerrit/changes/changes.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.1/gerrit/changes/edit.py` & `python-gerrit-api-3.0.2/gerrit/changes/edit.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.1/gerrit/changes/messages.py` & `python-gerrit-api-3.0.2/gerrit/changes/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 class GerritChangeMessage(GerritBase):
     def __init__(self, id: str, change: str, gerrit):
         self.id = id
         self.change = change
         self.gerrit = gerrit
         self.endpoint = f"/changes/{self.change}/messages/{self.id}"
-        GerritBase.__init__(self)
+        super().__init__(self)
 
     def __str__(self):
         return self.id
 
     def delete(self, input_=None):
         """
         Deletes a change message.
```

### Comparing `python-gerrit-api-3.0.1/gerrit/changes/reviewers.py` & `python-gerrit-api-3.0.2/gerrit/changes/reviewers.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 class GerritChangeReviewer(GerritBase):
     def __init__(self, account: str, change: str, gerrit):
         self.account = account
         self.change = change
         self.gerrit = gerrit
         self.endpoint = f"/changes/{self.change}/reviewers/{self.account}"
-        GerritBase.__init__(self)
+        super().__init__(self)
 
     def __str__(self):
         return str(self.account)
 
     def delete(self, input_=None):
         """
         Deletes a reviewer from a change.
```

### Comparing `python-gerrit-api-3.0.1/gerrit/changes/revision/base.py` & `python-gerrit-api-3.0.2/gerrit/changes/revision/base.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.1/gerrit/changes/revision/comments.py` & `python-gerrit-api-3.0.2/gerrit/changes/revision/comments.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 class GerritChangeRevisionComment(GerritBase):
     def __init__(self, id: str, change: str, revision: str, gerrit):
         self.id = id
         self.change = change
         self.revision = revision
         self.gerrit = gerrit
         self.endpoint = f"/changes/{self.change}/revisions/{self.revision}/comments/{self.id}"
-        GerritBase.__init__(self)
+        super().__init__(self)
 
     def __str__(self):
         return self.id
 
     def delete(self, input_=None):
         """
         Deletes a published comment of a revision. Instead of deleting the whole comment,
```

### Comparing `python-gerrit-api-3.0.1/gerrit/changes/revision/drafts.py` & `python-gerrit-api-3.0.2/gerrit/changes/revision/drafts.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 class GerritChangeRevisionDraft(GerritBase):
     def __init__(self, id: str, change: str, revision: str, gerrit):
         self.id = id
         self.change = change
         self.revision = revision
         self.gerrit = gerrit
         self.endpoint = f"/changes/{self.change}/revisions/{self.revision}/drafts/{self.id}"
-        GerritBase.__init__(self)
+        super().__init__(self)
 
     def __str__(self):
         return self.id
 
     def update(self, input_):
         """
         Updates a draft comment on a revision.
```

### Comparing `python-gerrit-api-3.0.1/gerrit/changes/revision/files.py` & `python-gerrit-api-3.0.2/gerrit/changes/revision/files.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.1/gerrit/config/caches.py` & `python-gerrit-api-3.0.2/gerrit/config/caches.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.1/gerrit/config/config.py` & `python-gerrit-api-3.0.2/gerrit/config/config.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.1/gerrit/config/tasks.py` & `python-gerrit-api-3.0.2/gerrit/config/tasks.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.1/gerrit/groups/group.py` & `python-gerrit-api-3.0.2/gerrit/groups/group.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class GerritGroup(GerritBase):
     def __init__(self, group_id: int, gerrit):
         self.id = group_id
         self.gerrit = gerrit
         self.endpoint = f"/groups/{self.id}"
-        GerritBase.__init__(self)
+        super().__init__(self)
 
     def __str__(self):
         return self.id
 
     def get_name(self):
         """
         Retrieves the name of a group.
```

### Comparing `python-gerrit-api-3.0.1/gerrit/groups/groups.py` & `python-gerrit-api-3.0.2/gerrit/groups/groups.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.1/gerrit/groups/members.py` & `python-gerrit-api-3.0.2/gerrit/groups/members.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.1/gerrit/groups/subgroups.py` & `python-gerrit-api-3.0.2/gerrit/groups/subgroups.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.1/gerrit/plugins/plugins.py` & `python-gerrit-api-3.0.2/gerrit/plugins/plugins.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.1/gerrit/projects/branches.py` & `python-gerrit-api-3.0.2/gerrit/projects/branches.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 
 class GerritProjectBranch(GerritBase):
     def __init__(self, name: str, project: str, gerrit):
         self.name = name
         self.project = project
         self.gerrit = gerrit
-        self.endpoint = f"/projects/{self.project}/branches/{self.name}"
-        GerritBase.__init__(self)
+        self.endpoint = f"/projects/{self.project}/branches/{quote_plus(self.name)}"
+        super().__init__(self)
 
     def __str__(self):
         return self.name
 
     def get_file_content(self, file, decode=False):
         """
         Gets the content of a file from the HEAD revision of a certain branch.
@@ -150,15 +150,15 @@
         try:
             self.get(name)
             message = f"Branch {name} already exists"
             logger.error(message)
             raise BranchAlreadyExistsError(message)
         except BranchNotFoundError:
             self.gerrit.put(
-                self.endpoint + f"/{name}", json=input_, headers=self.gerrit.default_headers)
+                self.endpoint + f"/{quote_plus(name)}", json=input_, headers=self.gerrit.default_headers)
 
             return self.get(name)
 
     def delete(self, name):
         """
         Delete a branch.
```

### Comparing `python-gerrit-api-3.0.1/gerrit/projects/commit.py` & `python-gerrit-api-3.0.2/gerrit/projects/commit.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 class GerritProjectCommit(GerritBase):
     def __init__(self, commit: str, project: str, gerrit):
         self.commit = commit
         self.project = project
         self.gerrit = gerrit
         self.endpoint = f"/projects/{self.project}/commits/{self.commit}"
-        GerritBase.__init__(self)
+        super().__init__(self)
 
     def __str__(self):
         return self.commit
 
     def get_include_in(self):
         """
         Retrieves the branches and tags in which a change is included.
```

### Comparing `python-gerrit-api-3.0.1/gerrit/projects/dashboards.py` & `python-gerrit-api-3.0.2/gerrit/projects/dashboards.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 class GerritProjectDashboard(GerritBase):
     def __init__(self, id: str, project: str, gerrit):
         self.id = id
         self.project = project
         self.gerrit = gerrit
         self.endpoint = f"/projects/{self.project}/dashboards/{self.id}"
-        GerritBase.__init__(self)
+        super().__init__(self)
 
     def __str__(self):
         return str(self.id)
 
     def delete(self):
         """
         Deletes a project dashboard.
```

### Comparing `python-gerrit-api-3.0.1/gerrit/projects/labels.py` & `python-gerrit-api-3.0.2/gerrit/projects/labels.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 class GerritProjectLabel(GerritBase):
     def __init__(self, name: str, project: str, gerrit):
         self.name = name
         self.project = project
         self.gerrit = gerrit
         self.endpoint = f"/projects/{self.project}/labels/{self.name}"
-        GerritBase.__init__(self)
+        super().__init__(self)
 
     def __str__(self):
         return self.name
 
     def set(self, input_):
         """
         Updates the definition of a label that is defined in this project.
```

### Comparing `python-gerrit-api-3.0.1/gerrit/projects/project.py` & `python-gerrit-api-3.0.2/gerrit/projects/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 class GerritProject(GerritBase):
     def __init__(self, project_id: str, gerrit):
         self.id = project_id
         self.gerrit = gerrit
         self.endpoint = f"/projects/{self.id}"
-        GerritBase.__init__(self)
+        super().__init__(self)
 
     def __str__(self):
         return self.id
 
     def get_description(self):
         """
         Retrieves the description of a project.
```

### Comparing `python-gerrit-api-3.0.1/gerrit/projects/projects.py` & `python-gerrit-api-3.0.2/gerrit/projects/projects.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.1/gerrit/projects/tags.py` & `python-gerrit-api-3.0.2/gerrit/projects/tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 
 class GerritProjectTag(GerritBase):
     def __init__(self, name: str, project: str, gerrit):
         self.name = name
         self.project = project
         self.gerrit = gerrit
-        self.endpoint = f"/projects/{self.project}/tags/{self.name}"
-        GerritBase.__init__(self)
+        self.endpoint = f"/projects/{self.project}/tags/{quote_plus(self.name)}"
+        super().__init__(self)
 
     def __str__(self):
         return self.name
 
     def delete(self):
         """
         Delete a tag.
@@ -100,15 +100,15 @@
         try:
             self.get(name)
             message = f"Tag {name} already exists"
             logger.error(message)
             raise TagAlreadyExistsError(message)
         except TagNotFoundError:
             self.gerrit.put(
-                self.endpoint + f"/{name}", json=input_, headers=self.gerrit.default_headers)
+                self.endpoint + f"/{quote_plus(name)}", json=input_, headers=self.gerrit.default_headers)
 
             return self.get(name)
 
     def delete(self, name):
         """
         Delete a tag.
```

### Comparing `python-gerrit-api-3.0.1/gerrit/projects/webhooks.py` & `python-gerrit-api-3.0.2/gerrit/projects/webhooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 class GerritProjectWebHook(GerritBase):
     def __init__(self, name: str, project: str, gerrit):
         self.name = name
         self.project = project
         self.gerrit = gerrit
         self.endpoint = f"/config/server/webhooks~projects/{self.project}/remotes/{self.name}"
-        GerritBase.__init__(self)
+        super().__init__(self)
 
     def __str__(self):
         return self.name
 
     def delete(self):
         """
         Delete a webhook for a project.
```

### Comparing `python-gerrit-api-3.0.1/gerrit/utils/common.py` & `python-gerrit-api-3.0.2/gerrit/utils/common.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.1/gerrit/utils/exceptions.py` & `python-gerrit-api-3.0.2/gerrit/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.1/gerrit/utils/gerritbase.py` & `python-gerrit-api-3.0.2/gerrit/utils/gerritbase.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.1/gerrit/utils/requester.py` & `python-gerrit-api-3.0.2/gerrit/utils/requester.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,19 +69,23 @@
         :return:
         """
         request_kwargs = kwargs
         if self.username and self.password:
             request_kwargs["auth"] = (self.username, self.password)
 
         if params:
-            assert isinstance(params, dict), f"Params must be a dict, got {repr(params)}"
+            if not isinstance(params, dict):
+                raise ValueError(f"Params must be a dict, got {repr(params)}")
+
             request_kwargs["params"] = params
 
         if headers:
-            assert isinstance(headers, dict), f"headers must be a dict, got {repr(headers)}"
+            if not isinstance(headers, dict):
+                raise ValueError(f"headers must be a dict, got {repr(headers)}")
+
             request_kwargs["headers"] = headers
 
         if self.AUTH_COOKIE:
             currentheaders = request_kwargs.get("headers", {})
             currentheaders.update({"Cookie": self.AUTH_COOKIE})
             request_kwargs["headers"] = currentheaders
```

### Comparing `python-gerrit-api-3.0.1/gitiles/base.py` & `python-gerrit-api-3.0.2/gitiles/base.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.1/python_gerrit_api.egg-info/PKG-INFO` & `python-gerrit-api-3.0.2/python_gerrit_api.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-gerrit-api
-Version: 3.0.1
+Version: 3.0.2
 Summary: Python wrapper for the Gerrit REST API.
 Home-page: https://github.com/shijl0925/python-gerrit-api
 Author: Jialiang Shi
 Author-email: kevin09254930sjl@gmail.com
 License: MIT
 Keywords: api gerrit client wrapper
 Classifier: Development Status :: 5 - Production/Stable
@@ -32,14 +32,18 @@
     :target: https://pepy.tech/project/python-gerrit-api
 .. image:: https://sonarcloud.io/api/project_badges/measure?project=shijl0925_python-gerrit-api&metric=alert_status
     :target: https://sonarcloud.io/dashboard?id=shijl0925_python-gerrit-api
 .. image:: https://sonarcloud.io/api/project_badges/measure?project=shijl0925_python-gerrit-api&metric=coverage
     :target: https://sonarcloud.io/summary/overall?id=shijl0925_python-gerrit-api
 .. image:: https://codecov.io/gh/shijl0925/python-gerrit-api/branch/master/graph/badge.svg?token=HU6U2LNHUK 
     :target: https://codecov.io/gh/shijl0925/python-gerrit-api
+.. image:: https://app.codacy.com/project/badge/Grade/fb3a59e09af8422ca2349b3974e02833
+    :target: https://app.codacy.com/gh/shijl0925/python-gerrit-api/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade
+.. image:: https://app.codacy.com/project/badge/Coverage/fb3a59e09af8422ca2349b3974e02833
+    :target: https://app.codacy.com/gh/shijl0925/python-gerrit-api/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage
 .. image:: https://img.shields.io/github/license/shijl0925/python-gerrit-api.svg
     :target: LICENSE
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 
 What is it?
 -----------
```

### Comparing `python-gerrit-api-3.0.1/python_gerrit_api.egg-info/SOURCES.txt` & `python-gerrit-api-3.0.2/python_gerrit_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.1/setup.py` & `python-gerrit-api-3.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """A setuptools based setup module.
 See:
 https://packaging.python.org/en/latest/distributing.html
 https://github.com/pypa/sampleproject
 """
 # Always prefer setuptools over distutils
+import ast
 from setuptools import setup, find_packages
 
 # To use a consistent encoding
 from codecs import open
 from os import path
 
 
@@ -21,15 +22,15 @@
     required = f.read().splitlines()
 
 def get_version() -> str:
     version = ""
     with open("gerrit/__init__.py", "r", encoding="utf-8") as f:
         for line in f:
             if line.startswith("__version__"):
-                version = eval(line.split("=")[-1])
+                version = ast.literal_eval(line.split("=")[-1])
                 break
     return version
 
 setup(
     name="python-gerrit-api",
     # https://packaging.python.org/en/latest/single_source_version.html
     version=get_version(),
```

### Comparing `python-gerrit-api-3.0.1/tests/test_accounts.py` & `python-gerrit-api-3.0.2/tests/test_accounts.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.1/tests/test_changes.py` & `python-gerrit-api-3.0.2/tests/test_changes.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.1/tests/test_gitiles.py` & `python-gerrit-api-3.0.2/tests/test_gitiles.py`

 * *Files identical despite different names*

### Comparing `python-gerrit-api-3.0.1/tests/test_groups.py` & `python-gerrit-api-3.0.2/tests/test_groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     from gerrit.utils.exceptions import GroupNotFoundError
     with pytest.raises(GroupNotFoundError):
         gerrit_client.groups.get(id_=1000000000)
 
     group_id = 613
     group = gerrit_client.groups.get(group_id)
 
-    assert type(group) == GerritGroup
+    assert isinstance(group, GerritGroup)
 
     assert str(group) == str(group.id)
 
     group_name = group.get_name()
     assert group_name == "Reviewers"
 
     group_info = group.to_dict()
```

### Comparing `python-gerrit-api-3.0.1/tests/test_projects.py` & `python-gerrit-api-3.0.2/tests/test_projects.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     with pytest.raises(ProjectNotFoundError):
         gerrit_client.projects.get(name="test-project0000000")
 
     project_name = gerrit_object["project_name"]
     project = gerrit_client.projects.get(name=project_name)
     logger.debug(project.to_dict())
 
-    assert type(project) == GerritProject
+    assert isinstance(project, GerritProject)
 
     attrs = ["id", "name", "parent", "state", "labels", "web_links"]
     for attr in attrs:
         logger.debug(f"{attr}, {hasattr(project, attr)}, {getattr(project, attr)}")
 
     assert all([hasattr(project, attr) for attr in attrs])
```

### Comparing `python-gerrit-api-3.0.1/tests/test_revision.py` & `python-gerrit-api-3.0.2/tests/test_revision.py`

 * *Files identical despite different names*

