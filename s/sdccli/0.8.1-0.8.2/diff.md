# Comparing `tmp/sdccli-0.8.1.tar.gz` & `tmp/sdccli-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdccli-0.8.1.tar", max compression
+gzip compressed data, was "sdccli-0.8.2.tar", max compression
```

## Comparing `sdccli-0.8.1.tar` & `sdccli-0.8.2.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0     1067 2023-07-18 08:40:59.586828 sdccli-0.8.1/LICENSE.txt
--rw-r--r--   0        0        0      952 2023-07-18 08:41:17.111039 sdccli-0.8.1/pyproject.toml
--rw-r--r--   0        0        0       21 2023-07-18 08:41:17.111039 sdccli-0.8.1/sdccli/__init__.py
--rw-r--r--   0        0        0     2153 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/__init__.py
--rw-r--r--   0        0        0     5291 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/alert.py
--rw-r--r--   0        0        0     9586 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/backup.py
--rw-r--r--   0        0        0     5549 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/capture.py
--rw-r--r--   0        0        0     3924 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/command.py
--rw-r--r--   0        0        0     8177 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/compliance.py
--rw-r--r--   0        0        0     8388 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/dashboard/__init__.py
--rw-r--r--   0        0        0     5036 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/dashboard/panel.py
--rw-r--r--   0        0        0     7875 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/dashboardv2.py
--rw-r--r--   0        0        0     4617 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/event.py
--rw-r--r--   0        0        0     4406 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/eventv1.py
--rw-r--r--   0        0        0        0 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/formatter/__init__.py
--rw-r--r--   0        0        0      139 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/formatter/json_formatter/__init__.py
--rw-r--r--   0        0        0      841 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/formatter/text_formatter/__init__.py
--rw-r--r--   0        0        0      464 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/formatter/text_formatter/alert.py
--rw-r--r--   0        0        0      887 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/formatter/text_formatter/dashboard.py
--rw-r--r--   0        0        0     1017 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/formatter/text_formatter/panel.py
--rw-r--r--   0        0        0     1992 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/formatter/text_formatter/policy_events.py
--rw-r--r--   0        0        0        0 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/formatter/text_formatter/scanning/__init__.py
--rw-r--r--   0        0        0      537 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/formatter/text_formatter/scanning/alert.py
--rw-r--r--   0        0        0     4553 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/formatter/text_formatter/scanning/image.py
--rw-r--r--   0        0        0     3583 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/formatter/text_formatter/scanning/vulnerability.py
--rw-r--r--   0        0        0    18732 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/policy/__init__.py
--rw-r--r--   0        0        0     3528 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/policy/falco_list.py
--rw-r--r--   0        0        0     3548 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/policy/falco_macro.py
--rw-r--r--   0        0        0    10159 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/policy/rule.py
--rw-r--r--   0        0        0     6687 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/profile.py
--rw-r--r--   0        0        0      884 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/scanning/__init__.py
--rw-r--r--   0        0        0     3788 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/scanning/alert.py
--rw-r--r--   0        0        0     7778 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/scanning/cve_report.py
--rw-r--r--   0        0        0     8444 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/scanning/image.py
--rw-r--r--   0        0        0     3925 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/scanning/policy.py
--rw-r--r--   0        0        0     3702 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/scanning/query.py
--rw-r--r--   0        0        0     4148 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/scanning/registry.py
--rw-r--r--   0        0        0     3419 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/scanning/repo.py
--rw-r--r--   0        0        0     1470 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/scanning/runtime.py
--rw-r--r--   0        0        0     2484 2023-07-18 08:40:59.586828 sdccli-0.8.1/sdccli/cli/scanning/subscription.py
--rw-r--r--   0        0        0     4079 2023-07-18 08:40:59.590828 sdccli-0.8.1/sdccli/cli/scanning/vulnerability/__init__.py
--rw-r--r--   0        0        0     1848 2023-07-18 08:40:59.590828 sdccli-0.8.1/sdccli/cli/scanning/vulnerability/bundle.py
--rw-r--r--   0        0        0      587 2023-07-18 08:40:59.590828 sdccli-0.8.1/sdccli/cli/settings/__init__.py
--rw-r--r--   0        0        0     1893 2023-07-18 08:40:59.590828 sdccli-0.8.1/sdccli/cli/settings/access_key.py
--rw-r--r--   0        0        0     3071 2023-07-18 08:40:59.590828 sdccli-0.8.1/sdccli/cli/settings/notification.py
--rw-r--r--   0        0        0     7376 2023-07-18 08:40:59.590828 sdccli-0.8.1/sdccli/cli/settings/team.py
--rw-r--r--   0        0        0     3749 2023-07-18 08:40:59.590828 sdccli-0.8.1/sdccli/cli/settings/user.py
--rw-r--r--   0        0        0     7450 2023-07-18 08:40:59.590828 sdccli-0.8.1/sdccli/config.py
--rw-r--r--   0        0        0     9102 2023-07-18 08:40:59.590828 sdccli-0.8.1/sdccli/drop.py
--rw-r--r--   0        0        0     2804 2023-07-18 08:40:59.590828 sdccli-0.8.1/sdccli/falco_macro.py
--rw-r--r--   0        0        0      769 2023-07-18 08:40:59.590828 sdccli-0.8.1/sdccli/helpers.py
--rw-r--r--   0        0        0      796 2023-07-18 08:40:59.590828 sdccli-0.8.1/sdccli/printer.py
--rw-r--r--   0        0        0    23837 2023-07-18 08:40:59.590828 sdccli-0.8.1/sdccli/restore.py
--rw-r--r--   0        0        0     1493 2023-07-18 08:40:59.590828 sdccli-0.8.1/sdccli/time.py
--rw-r--r--   0        0        0        0 2023-07-18 08:40:59.590828 sdccli-0.8.1/sdccli/usecases/__init__.py
--rw-r--r--   0        0        0     2379 2023-07-18 08:40:59.590828 sdccli-0.8.1/sdccli/usecases/alert.py
--rw-r--r--   0        0        0        0 2023-07-18 08:40:59.590828 sdccli-0.8.1/sdccli/usecases/backup/Pipfile
--rw-r--r--   0        0        0       42 2023-07-18 08:40:59.590828 sdccli-0.8.1/sdccli/usecases/backup/__init__.py
--rw-r--r--   0        0        0    13890 2023-07-18 08:40:59.590828 sdccli-0.8.1/sdccli/usecases/backup/dump.py
--rw-r--r--   0        0        0    15088 2023-07-18 08:40:59.590828 sdccli-0.8.1/sdccli/usecases/backup/restore.py
--rw-r--r--   0        0        0        0 2023-07-18 08:40:59.590828 sdccli-0.8.1/sdccli/usecases/dashboard/__init__.py
--rw-r--r--   0        0        0     5161 2023-07-18 08:40:59.590828 sdccli-0.8.1/sdccli/usecases/dashboard/dashboard_v2.py
--rw-r--r--   0        0        0     7644 2023-07-18 08:40:59.590828 sdccli-0.8.1/sdccli/usecases/dashboard/dashboard_v3.py
--rw-r--r--   0        0        0     6903 2023-07-18 08:40:59.590828 sdccli-0.8.1/sdccli/usecases/dashboard/panel.py
--rw-r--r--   0        0        0        0 2023-07-18 08:40:59.590828 sdccli-0.8.1/sdccli/usecases/policy/__init__.py
--rw-r--r--   0        0        0     2247 2023-07-18 08:40:59.590828 sdccli-0.8.1/sdccli/usecases/policy/events.py
--rw-r--r--   0        0        0        0 2023-07-18 08:40:59.590828 sdccli-0.8.1/sdccli/usecases/scanning/__init__.py
--rw-r--r--   0        0        0     1137 2023-07-18 08:40:59.590828 sdccli-0.8.1/sdccli/usecases/scanning/alert.py
--rw-r--r--   0        0        0     4084 2023-07-18 08:40:59.590828 sdccli-0.8.1/sdccli/usecases/scanning/image.py
--rw-r--r--   0        0        0     3781 2023-07-18 08:40:59.590828 sdccli-0.8.1/sdccli/usecases/scanning/vulnerability.py
--rw-r--r--   0        0        0        0 2023-07-18 08:40:59.590828 sdccli-0.8.1/sdccli/usecases/settings/__init__.py
--rw-r--r--   0        0        0      530 2023-07-18 08:40:59.590828 sdccli-0.8.1/sdccli/usecases/settings/team.py
--rw-r--r--   0        0        0     1006 1970-01-01 00:00:00.000000 sdccli-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-31 07:51:36.124984 sdccli-0.8.2/LICENSE.txt
+-rw-r--r--   0        0        0      952 2023-07-31 07:51:51.169206 sdccli-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-07-31 07:51:51.173206 sdccli-0.8.2/sdccli/__init__.py
+-rw-r--r--   0        0        0     2153 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/__init__.py
+-rw-r--r--   0        0        0     5291 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/alert.py
+-rw-r--r--   0        0        0     9586 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/backup.py
+-rw-r--r--   0        0        0     5549 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/capture.py
+-rw-r--r--   0        0        0     3924 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/command.py
+-rw-r--r--   0        0        0     8177 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/compliance.py
+-rw-r--r--   0        0        0     8388 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/dashboard/__init__.py
+-rw-r--r--   0        0        0     5036 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/dashboard/panel.py
+-rw-r--r--   0        0        0     7875 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/dashboardv2.py
+-rw-r--r--   0        0        0     4617 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/event.py
+-rw-r--r--   0        0        0     4406 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/eventv1.py
+-rw-r--r--   0        0        0        0 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/formatter/__init__.py
+-rw-r--r--   0        0        0      139 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/formatter/json_formatter/__init__.py
+-rw-r--r--   0        0        0      841 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/formatter/text_formatter/__init__.py
+-rw-r--r--   0        0        0      464 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/formatter/text_formatter/alert.py
+-rw-r--r--   0        0        0      887 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/formatter/text_formatter/dashboard.py
+-rw-r--r--   0        0        0     1017 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/formatter/text_formatter/panel.py
+-rw-r--r--   0        0        0     1992 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/formatter/text_formatter/policy_events.py
+-rw-r--r--   0        0        0        0 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/formatter/text_formatter/scanning/__init__.py
+-rw-r--r--   0        0        0      537 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/formatter/text_formatter/scanning/alert.py
+-rw-r--r--   0        0        0     4553 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/formatter/text_formatter/scanning/image.py
+-rw-r--r--   0        0        0     3583 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/formatter/text_formatter/scanning/vulnerability.py
+-rw-r--r--   0        0        0    18732 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/policy/__init__.py
+-rw-r--r--   0        0        0     3528 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/policy/falco_list.py
+-rw-r--r--   0        0        0     3548 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/policy/falco_macro.py
+-rw-r--r--   0        0        0    10159 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/policy/rule.py
+-rw-r--r--   0        0        0     6687 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/profile.py
+-rw-r--r--   0        0        0      884 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/scanning/__init__.py
+-rw-r--r--   0        0        0     3788 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/scanning/alert.py
+-rw-r--r--   0        0        0     7778 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/scanning/cve_report.py
+-rw-r--r--   0        0        0     8444 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/scanning/image.py
+-rw-r--r--   0        0        0     3925 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/scanning/policy.py
+-rw-r--r--   0        0        0     3702 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/scanning/query.py
+-rw-r--r--   0        0        0     4148 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/scanning/registry.py
+-rw-r--r--   0        0        0     3419 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/scanning/repo.py
+-rw-r--r--   0        0        0     1470 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/scanning/runtime.py
+-rw-r--r--   0        0        0     2484 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/scanning/subscription.py
+-rw-r--r--   0        0        0     4079 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/scanning/vulnerability/__init__.py
+-rw-r--r--   0        0        0     1848 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/scanning/vulnerability/bundle.py
+-rw-r--r--   0        0        0      587 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/settings/__init__.py
+-rw-r--r--   0        0        0     1893 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/settings/access_key.py
+-rw-r--r--   0        0        0     3071 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/settings/notification.py
+-rw-r--r--   0        0        0     7376 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/settings/team.py
+-rw-r--r--   0        0        0     3749 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/cli/settings/user.py
+-rw-r--r--   0        0        0     7450 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/config.py
+-rw-r--r--   0        0        0     9102 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/drop.py
+-rw-r--r--   0        0        0     2804 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/falco_macro.py
+-rw-r--r--   0        0        0      769 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/helpers.py
+-rw-r--r--   0        0        0      796 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/printer.py
+-rw-r--r--   0        0        0    24025 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/restore.py
+-rw-r--r--   0        0        0     1493 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/time.py
+-rw-r--r--   0        0        0        0 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/usecases/__init__.py
+-rw-r--r--   0        0        0     2379 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/usecases/alert.py
+-rw-r--r--   0        0        0        0 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/usecases/backup/Pipfile
+-rw-r--r--   0        0        0       42 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/usecases/backup/__init__.py
+-rw-r--r--   0        0        0    14339 2023-07-31 07:51:36.128984 sdccli-0.8.2/sdccli/usecases/backup/dump.py
+-rw-r--r--   0        0        0    15305 2023-07-31 07:51:36.132984 sdccli-0.8.2/sdccli/usecases/backup/restore.py
+-rw-r--r--   0        0        0        0 2023-07-31 07:51:36.132984 sdccli-0.8.2/sdccli/usecases/dashboard/__init__.py
+-rw-r--r--   0        0        0     5161 2023-07-31 07:51:36.132984 sdccli-0.8.2/sdccli/usecases/dashboard/dashboard_v2.py
+-rw-r--r--   0        0        0     7644 2023-07-31 07:51:36.132984 sdccli-0.8.2/sdccli/usecases/dashboard/dashboard_v3.py
+-rw-r--r--   0        0        0     6903 2023-07-31 07:51:36.132984 sdccli-0.8.2/sdccli/usecases/dashboard/panel.py
+-rw-r--r--   0        0        0        0 2023-07-31 07:51:36.132984 sdccli-0.8.2/sdccli/usecases/policy/__init__.py
+-rw-r--r--   0        0        0     2247 2023-07-31 07:51:36.132984 sdccli-0.8.2/sdccli/usecases/policy/events.py
+-rw-r--r--   0        0        0        0 2023-07-31 07:51:36.132984 sdccli-0.8.2/sdccli/usecases/scanning/__init__.py
+-rw-r--r--   0        0        0     1137 2023-07-31 07:51:36.132984 sdccli-0.8.2/sdccli/usecases/scanning/alert.py
+-rw-r--r--   0        0        0     4084 2023-07-31 07:51:36.132984 sdccli-0.8.2/sdccli/usecases/scanning/image.py
+-rw-r--r--   0        0        0     3781 2023-07-31 07:51:36.132984 sdccli-0.8.2/sdccli/usecases/scanning/vulnerability.py
+-rw-r--r--   0        0        0        0 2023-07-31 07:51:36.132984 sdccli-0.8.2/sdccli/usecases/settings/__init__.py
+-rw-r--r--   0        0        0      530 2023-07-31 07:51:36.132984 sdccli-0.8.2/sdccli/usecases/settings/team.py
+-rw-r--r--   0        0        0     1006 1970-01-01 00:00:00.000000 sdccli-0.8.2/PKG-INFO
```

### Comparing `sdccli-0.8.1/LICENSE.txt` & `sdccli-0.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/pyproject.toml` & `sdccli-0.8.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdccli"
-version = "0.8.1"
+version = "0.8.2"
 description = "CLI client for Sysdig Cloud"
 authors = ["Sysdig Inc. <info@sysdig.com>"]
 license = "MIT"
 maintainers = [
     "Nestor Salceda <nestor.salceda@sysdig.com>",
     "Federico Barcelona <fede.barcelona@sysdig.com>"
 ]
```

### Comparing `sdccli-0.8.1/sdccli/cli/__init__.py` & `sdccli-0.8.2/sdccli/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/alert.py` & `sdccli-0.8.2/sdccli/cli/alert.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/backup.py` & `sdccli-0.8.2/sdccli/cli/backup.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/capture.py` & `sdccli-0.8.2/sdccli/cli/capture.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/command.py` & `sdccli-0.8.2/sdccli/cli/command.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/compliance.py` & `sdccli-0.8.2/sdccli/cli/compliance.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/dashboard/__init__.py` & `sdccli-0.8.2/sdccli/cli/dashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/dashboard/panel.py` & `sdccli-0.8.2/sdccli/cli/dashboard/panel.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/dashboardv2.py` & `sdccli-0.8.2/sdccli/cli/dashboardv2.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/event.py` & `sdccli-0.8.2/sdccli/cli/event.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/eventv1.py` & `sdccli-0.8.2/sdccli/cli/eventv1.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/formatter/text_formatter/__init__.py` & `sdccli-0.8.2/sdccli/cli/formatter/text_formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/formatter/text_formatter/dashboard.py` & `sdccli-0.8.2/sdccli/cli/formatter/text_formatter/dashboard.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/formatter/text_formatter/panel.py` & `sdccli-0.8.2/sdccli/cli/formatter/text_formatter/panel.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/formatter/text_formatter/policy_events.py` & `sdccli-0.8.2/sdccli/cli/formatter/text_formatter/policy_events.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/formatter/text_formatter/scanning/alert.py` & `sdccli-0.8.2/sdccli/cli/formatter/text_formatter/scanning/alert.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/formatter/text_formatter/scanning/image.py` & `sdccli-0.8.2/sdccli/cli/formatter/text_formatter/scanning/image.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/formatter/text_formatter/scanning/vulnerability.py` & `sdccli-0.8.2/sdccli/cli/formatter/text_formatter/scanning/vulnerability.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/policy/__init__.py` & `sdccli-0.8.2/sdccli/cli/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/policy/falco_list.py` & `sdccli-0.8.2/sdccli/cli/policy/falco_list.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/policy/falco_macro.py` & `sdccli-0.8.2/sdccli/cli/policy/falco_macro.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/policy/rule.py` & `sdccli-0.8.2/sdccli/cli/policy/rule.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/profile.py` & `sdccli-0.8.2/sdccli/cli/profile.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/scanning/__init__.py` & `sdccli-0.8.2/sdccli/cli/scanning/__init__.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/scanning/alert.py` & `sdccli-0.8.2/sdccli/cli/scanning/alert.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/scanning/cve_report.py` & `sdccli-0.8.2/sdccli/cli/scanning/cve_report.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/scanning/image.py` & `sdccli-0.8.2/sdccli/cli/scanning/image.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/scanning/policy.py` & `sdccli-0.8.2/sdccli/cli/scanning/policy.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/scanning/query.py` & `sdccli-0.8.2/sdccli/cli/scanning/query.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/scanning/registry.py` & `sdccli-0.8.2/sdccli/cli/scanning/registry.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/scanning/repo.py` & `sdccli-0.8.2/sdccli/cli/scanning/repo.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/scanning/runtime.py` & `sdccli-0.8.2/sdccli/cli/scanning/runtime.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/scanning/subscription.py` & `sdccli-0.8.2/sdccli/cli/scanning/subscription.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/scanning/vulnerability/__init__.py` & `sdccli-0.8.2/sdccli/cli/scanning/vulnerability/__init__.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/scanning/vulnerability/bundle.py` & `sdccli-0.8.2/sdccli/cli/scanning/vulnerability/bundle.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/settings/__init__.py` & `sdccli-0.8.2/sdccli/cli/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/settings/access_key.py` & `sdccli-0.8.2/sdccli/cli/settings/access_key.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/settings/notification.py` & `sdccli-0.8.2/sdccli/cli/settings/notification.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/settings/team.py` & `sdccli-0.8.2/sdccli/cli/settings/team.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/cli/settings/user.py` & `sdccli-0.8.2/sdccli/cli/settings/user.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/config.py` & `sdccli-0.8.2/sdccli/config.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/drop.py` & `sdccli-0.8.2/sdccli/drop.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/falco_macro.py` & `sdccli-0.8.2/sdccli/falco_macro.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/helpers.py` & `sdccli-0.8.2/sdccli/helpers.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/printer.py` & `sdccli-0.8.2/sdccli/printer.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/restore.py` & `sdccli-0.8.2/sdccli/restore.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,57 +53,63 @@
             errors.append("couldn't recreate dashboard " + name + ': ' + result)
 
     if len(errors) != 0:
         return False, errors
     return True, None
 
 
-def alerts(file_data, monitor: SdMonitorClient):
+def alerts(file_data, notif_channels, monitor: SdMonitorClient):
     errors = []
     total = len(file_data)
-    ok, res = monitor.get_alerts()
+    ok, alerts_res = monitor.get_alerts()
     if not ok:
-        return False, res
-    existing_alerts = {alert['name']: alert for alert in res['alerts']}
+        return False, alerts_res
+    existing_alerts = {alert['name']: alert for alert in alerts_res['alerts']}
 
-    ok, res = monitor.list_notification_channels()
+    ok, nc_res = monitor.list_notification_channels()
     if not ok:
-        return False, res
-    existing_notification_channels = {nc['name']: nc['id'] for nc in res['notificationChannels']}
+        return False, nc_res
+    existing_nc = {nc['name']: nc for nc in nc_res['notificationChannels']}
 
+    out = []
     for i, alert in enumerate(file_data, start=1):
         name = alert['name']
-        alert['notificationChannelIds'] = []
-        for nc in alert.get('notificationChannelNames', []):
-            if nc in existing_notification_channels:
-                alert['notificationChannelIds'].append(existing_notification_channels[nc])
-            else:
-                print(f"  Warning: The Notification Channel '{nc}' does not exist in the environment, "
-                      f"the restored alert won't be assigned to this NC.")
+
         print(f"[{i}/{total}] Creating alert {name}... ")
+
         if name in existing_alerts:
             if same_dict(alert, existing_alerts[name],
                          ['id', 'teamId', 'autoCreated',
                           'notificationChannelNames', 'notificationCount', 'invalidMetrics',
-                          'valid']):
+                          'valid', 'createdOn', 'modifiedOn', 'version']):
                 print("      already exists, skip")
                 continue
             else:
-                ok, res = monitor.delete_alert(existing_alerts[name])
-                if not ok:
-                    errors.append(res)
-                    continue
+                alert['name'] = unique_name(alert['name'], set(existing_alerts.keys()))
+
+        new_nc_ids = []
+        old_nc_ids = alert.get('notificationChannelIds', None)
+        if isinstance(old_nc_ids, list):
+            alert_nc = [notif_channels[nc_id] for nc_id in old_nc_ids]
+            for nc in alert_nc:
+                if nc['name'] in existing_nc:
+                    new_nc_ids.append(existing_nc[nc['name']]['id'])
+                else:
+                    print(f'  Warning: The Notification Channel "{nc["name"]}" does not exist in the environment, '
+                          f'the restored alert won\'t be assigned to this NC.')
+            alert['notificationChannelIds'] = new_nc_ids
 
         ok, result = monitor.create_alert(alert_obj=alert)
         if not ok:
             errors.append(result)
-
+        else:
+            out.append(result)
     if len(errors) > 0:
         return False, errors
-    return True, None
+    return True, out
 
 
 def users(sdcommon, filename):
     '''
     Restores users without dropping the existing ones
     '''
     with open(filename) as file:
@@ -533,29 +539,30 @@
         print('Restoring user falco rules...')
         ok, result = sdsecure.set_user_falco_rules(file_data["userRulesFile"]["content"])
         if not ok:
             return False, result
         return True, None
 
 
+def unique_name(name: str, names: typing.Set[str]) -> str:
+    new_name = name
+    i = 1
+
+    while new_name in names:
+        new_name = f'{name} ({i})'
+        i += 1
+
+    return new_name
+
+
 def scanning_alerts(alerts: typing.List[dict],
                     notif_channels: typing.Dict[str, dict],
                     secure: SdSecureClientV1,
                     scanning: ScanningAlertsClientV1):
 
-    def unique_name(name: str, names: typing.Set[str]) -> str:
-        new_name = name
-        i = 1
-
-        while new_name in names:
-            new_name = f'{name} ({i})'
-            i += 1
-
-        return new_name
-
     errors = []
 
     ok, res = scanning.list_alerts()
     if not ok:
         return False, res
 
     existing_alerts = {alert['name']: alert for alert in res['alerts']}
```

### Comparing `sdccli-0.8.1/sdccli/time.py` & `sdccli-0.8.2/sdccli/time.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/usecases/alert.py` & `sdccli-0.8.2/sdccli/usecases/alert.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/usecases/backup/dump.py` & `sdccli-0.8.2/sdccli/usecases/backup/dump.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,20 +97,36 @@
 
     def execute(self):
         ok, res = self._monitor.get_alerts()
         if not ok:
             return ok, res
         self._sort_res(res)
 
-        ok, resNC = self._monitor.list_notification_channels()
+        ok, res_nc = self._monitor.list_notification_channels()
         if not ok:
-            return ok, resNC
+            return ok, res_nc
 
-
-        res = [{"kind": "alerts", "version": 1, "spec": res}]
+        used_nc = {
+            nc
+            for alert in res.get('alerts')
+            for nc in alert.get('notificationChannelIds', [])
+        }
+
+        res = [{
+            'kind': 'alerts',
+            'version': 1,
+            'spec': {
+                'alerts_response': res,
+                'notification_channels': {
+                    nc['id']: nc
+                    for nc in res_nc['notificationChannels']
+                    if nc['id'] in used_nc
+                }
+            },
+        }]
 
         self._repository.write(self._formatter(res))
         return ok, res
 
 
 class DumpTeamsMonitorUseCase(DumpMonitorUseCase):
     def __init__(self, monitor, repository):
```

### Comparing `sdccli-0.8.1/sdccli/usecases/backup/restore.py` & `sdccli-0.8.2/sdccli/usecases/backup/restore.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,38 +170,51 @@
 
         ok, res = drop.dashboards(self._monitor, remove_unowned=True)
         if not ok:
             return ok, res
         return restore.dashboards(file_data, self._monitor, existing_dashboards={}, restore_unowned=True)
 
 
+def alerts_from_backup(data):
+    alerts = [
+        alert
+        for kind in data
+        for alert in kind['alerts_response']['alerts']
+    ]
+
+    notif_channels = {
+        id: nc
+        for kind in data
+        for id, nc in kind['notification_channels'].items()
+    }
+    return alerts, notif_channels
+
+
 class RestoreAlertsUseCase(RestoreMonitorUseCase):
     def __init__(self, monitor, repository, formatter=yaml.safe_load):
         super().__init__(monitor, repository, formatter)
 
     def execute(self):
-        file_data = self._load_data_from_repo("alerts")
-        file_data = [item for sublist in file_data for item in sublist['alerts']]  # Flatten lists
+        alerts, notif_channels = alerts_from_backup(list(self._load_data_from_repo("alerts")))
 
-        return restore.alerts(file_data, self._monitor)
+        return restore.alerts(alerts, notif_channels, self._monitor)
 
 
 class RemoveAndRestoreAlertsUseCase(RestoreMonitorUseCase):
     def __init__(self, monitor, repository, formatter=yaml.safe_load):
         super().__init__(monitor, repository, formatter)
 
     def execute(self):
-        file_data = self._load_data_from_repo("alerts")
-        file_data = [item for sublist in file_data for item in sublist['alerts']]  # Flatten lists
+        alerts, notif_channels = alerts_from_backup(list(self._load_data_from_repo("alerts")))
 
         ok, res = drop.alerts(self._monitor)
         if not ok:
             return False, res
 
-        return restore.alerts(file_data, self._monitor)
+        return restore.alerts(alerts, notif_channels, self._monitor)
 
 
 class RestoreTeamsMonitorUseCase(RestoreMonitorUseCase):
     def __init__(self, monitor, repository, formatter=yaml.safe_load):
         super().__init__(monitor, repository, formatter)
 
     def execute(self):
```

### Comparing `sdccli-0.8.1/sdccli/usecases/dashboard/dashboard_v2.py` & `sdccli-0.8.2/sdccli/usecases/dashboard/dashboard_v2.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/usecases/dashboard/dashboard_v3.py` & `sdccli-0.8.2/sdccli/usecases/dashboard/dashboard_v3.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/usecases/dashboard/panel.py` & `sdccli-0.8.2/sdccli/usecases/dashboard/panel.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/usecases/policy/events.py` & `sdccli-0.8.2/sdccli/usecases/policy/events.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/usecases/scanning/alert.py` & `sdccli-0.8.2/sdccli/usecases/scanning/alert.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/usecases/scanning/image.py` & `sdccli-0.8.2/sdccli/usecases/scanning/image.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/usecases/scanning/vulnerability.py` & `sdccli-0.8.2/sdccli/usecases/scanning/vulnerability.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/sdccli/usecases/settings/team.py` & `sdccli-0.8.2/sdccli/usecases/settings/team.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.8.1/PKG-INFO` & `sdccli-0.8.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdccli
-Version: 0.8.1
+Version: 0.8.2
 Summary: CLI client for Sysdig Cloud
 License: MIT
 Author: Sysdig Inc.
 Author-email: info@sysdig.com
 Maintainer: Nestor Salceda
 Maintainer-email: nestor.salceda@sysdig.com
 Requires-Python: >=3.6,<4.0
```

