# Comparing `tmp/sharetop-2.4.5.tar.gz` & `tmp/sharetop-2.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharetop-2.4.5.tar", last modified: Tue Jul 18 11:58:10 2023, max compression
+gzip compressed data, was "sharetop-2.4.6.tar", last modified: Mon Jul 31 15:09:29 2023, max compression
```

## Comparing `sharetop-2.4.5.tar` & `sharetop-2.4.6.tar`

### file list

```diff
@@ -1,99 +1,100 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 11:58:10.213199 sharetop-2.4.5/
--rw-rw-rw-   0        0        0     1066 2023-04-26 14:07:21.000000 sharetop-2.4.5/LICENSE
--rw-rw-rw-   0        0        0    51253 2023-07-18 11:58:10.212184 sharetop-2.4.5/PKG-INFO
--rw-rw-rw-   0        0        0    49774 2023-07-15 03:35:16.000000 sharetop-2.4.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-18 11:58:10.214185 sharetop-2.4.5/setup.cfg
--rw-rw-rw-   0        0        0     1219 2023-04-29 06:50:50.000000 sharetop-2.4.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-18 11:58:09.275451 sharetop-2.4.5/sharetop/
--rw-rw-rw-   0        0        0      297 2023-05-18 12:23:41.000000 sharetop-2.4.5/sharetop/__init__.py
--rw-rw-rw-   0        0        0      386 2023-07-18 11:57:20.000000 sharetop-2.4.5/sharetop/__version__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 11:58:09.337640 sharetop-2.4.5/sharetop/api/
--rw-rw-rw-   0        0        0      306 2023-07-02 13:11:41.000000 sharetop-2.4.5/sharetop/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 11:58:09.363930 sharetop-2.4.5/sharetop/application/
--rw-rw-rw-   0        0        0       33 2023-04-21 11:53:52.000000 sharetop-2.4.5/sharetop/application/__init__.py
--rw-rw-rw-   0        0        0     4459 2023-07-16 22:42:50.000000 sharetop-2.4.5/sharetop/application/base.py
-drwxrwxrwx   0        0        0        0 2023-07-18 11:58:09.403177 sharetop-2.4.5/sharetop/core/
--rw-rw-rw-   0        0        0        0 2023-04-08 05:23:09.000000 sharetop-2.4.5/sharetop/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 11:58:09.485378 sharetop-2.4.5/sharetop/core/bond/
--rw-rw-rw-   0        0        0      592 2023-07-15 11:00:24.000000 sharetop-2.4.5/sharetop/core/bond/__init__.py
--rw-rw-rw-   0        0        0     1869 2023-04-24 04:28:03.000000 sharetop-2.4.5/sharetop/core/bond/config.py
--rw-rw-rw-   0        0        0     9571 2023-07-16 01:28:38.000000 sharetop-2.4.5/sharetop/core/bond/get_bond_info.py
--rw-rw-rw-   0        0        0    19614 2023-07-15 10:59:53.000000 sharetop-2.4.5/sharetop/core/bond/get_bond_public_info.py
--rw-rw-rw-   0        0        0      598 2023-04-10 05:06:06.000000 sharetop-2.4.5/sharetop/core/cache.py
-drwxrwxrwx   0        0        0        0 2023-07-18 11:58:09.514515 sharetop-2.4.5/sharetop/core/capital_flow/
--rw-rw-rw-   0        0        0      367 2023-07-15 15:19:38.000000 sharetop-2.4.5/sharetop/core/capital_flow/__init__.py
--rw-rw-rw-   0        0        0     6356 2023-07-15 15:19:38.000000 sharetop-2.4.5/sharetop/core/capital_flow/capital_flow_monitor.py
-drwxrwxrwx   0        0        0        0 2023-07-18 11:58:09.574929 sharetop-2.4.5/sharetop/core/common/
--rw-rw-rw-   0        0        0      188 2023-04-27 15:24:55.000000 sharetop-2.4.5/sharetop/core/common/__init__.py
--rw-rw-rw-   0        0        0     3727 2023-07-15 09:06:11.000000 sharetop-2.4.5/sharetop/core/common/common_base.py
--rw-rw-rw-   0        0        0     8688 2023-05-25 01:16:42.000000 sharetop-2.4.5/sharetop/core/common/config.py
--rw-rw-rw-   0        0        0    12428 2023-07-16 01:53:16.000000 sharetop-2.4.5/sharetop/core/common/getter.py
--rw-rw-rw-   0        0        0      750 2023-04-09 05:42:43.000000 sharetop-2.4.5/sharetop/core/config.py
-drwxrwxrwx   0        0        0        0 2023-07-18 11:58:09.614658 sharetop-2.4.5/sharetop/core/country/
--rw-rw-rw-   0        0        0       91 2023-07-16 02:39:07.000000 sharetop-2.4.5/sharetop/core/country/__init__.py
--rw-rw-rw-   0        0        0      491 2023-05-09 01:30:20.000000 sharetop-2.4.5/sharetop/core/country/config.py
--rw-rw-rw-   0        0        0      697 2023-07-16 02:39:07.000000 sharetop-2.4.5/sharetop/core/country/country_base_info.py
-drwxrwxrwx   0        0        0        0 2023-07-18 11:58:09.780117 sharetop-2.4.5/sharetop/core/fund/
--rw-rw-rw-   0        0        0     1017 2023-07-15 10:39:55.000000 sharetop-2.4.5/sharetop/core/fund/__init__.py
--rw-rw-rw-   0        0        0      904 2023-07-07 04:55:12.000000 sharetop-2.4.5/sharetop/core/fund/config.py
--rw-rw-rw-   0        0        0     2593 2023-07-06 01:13:48.000000 sharetop-2.4.5/sharetop/core/fund/fund_list.py
--rw-rw-rw-   0        0        0     1694 2023-07-15 09:54:03.000000 sharetop-2.4.5/sharetop/core/fund/get_fund_base_info.py
--rw-rw-rw-   0        0        0     2490 2023-07-15 10:09:17.000000 sharetop-2.4.5/sharetop/core/fund/get_fund_history_data.py
--rw-rw-rw-   0        0        0     3716 2023-07-15 10:12:05.000000 sharetop-2.4.5/sharetop/core/fund/get_fund_industry_info.py
--rw-rw-rw-   0        0        0     5474 2023-07-15 10:19:50.000000 sharetop-2.4.5/sharetop/core/fund/get_fund_invest_info.py
--rw-rw-rw-   0        0        0    12057 2023-07-15 10:32:02.000000 sharetop-2.4.5/sharetop/core/fund/get_fund_rank.py
--rw-rw-rw-   0        0        0     1466 2023-04-22 03:27:53.000000 sharetop-2.4.5/sharetop/core/fund/get_fund_real_time.py
--rw-rw-rw-   0        0        0     2497 2023-07-15 10:37:11.000000 sharetop-2.4.5/sharetop/core/fund/get_period_change_info.py
--rw-rw-rw-   0        0        0     2451 2023-07-15 10:39:55.000000 sharetop-2.4.5/sharetop/core/fund/get_types_percentage_info.py
-drwxrwxrwx   0        0        0        0 2023-07-18 11:58:09.808215 sharetop-2.4.5/sharetop/core/futures/
--rw-rw-rw-   0        0        0      250 2023-07-16 02:07:46.000000 sharetop-2.4.5/sharetop/core/futures/__init__.py
--rw-rw-rw-   0        0        0    10057 2023-07-16 02:09:22.000000 sharetop-2.4.5/sharetop/core/futures/get_futures_info.py
-drwxrwxrwx   0        0        0        0 2023-07-18 11:58:09.842958 sharetop-2.4.5/sharetop/core/oil/
--rw-rw-rw-   0        0        0      402 2023-05-16 01:17:51.000000 sharetop-2.4.5/sharetop/core/oil/__init__.py
--rw-rw-rw-   0        0        0     1685 2023-05-15 00:28:25.000000 sharetop-2.4.5/sharetop/core/oil/config.py
--rw-rw-rw-   0        0        0     3614 2023-07-10 00:25:56.000000 sharetop-2.4.5/sharetop/core/oil/oil_detail.py
-drwxrwxrwx   0        0        0        0 2023-07-18 11:58:09.877195 sharetop-2.4.5/sharetop/core/pig/
--rw-rw-rw-   0        0        0       84 2023-07-15 10:46:51.000000 sharetop-2.4.5/sharetop/core/pig/__init__.py
--rw-rw-rw-   0        0        0      163 2023-05-16 00:42:46.000000 sharetop-2.4.5/sharetop/core/pig/config.py
--rw-rw-rw-   0        0        0     1428 2023-07-15 10:46:51.000000 sharetop-2.4.5/sharetop/core/pig/pig_detail.py
-drwxrwxrwx   0        0        0        0 2023-07-18 11:58:09.964515 sharetop-2.4.5/sharetop/core/stock/
--rw-rw-rw-   0        0        0      662 2023-07-15 09:27:19.000000 sharetop-2.4.5/sharetop/core/stock/__init__.py
--rw-rw-rw-   0        0        0     4705 2023-07-15 03:35:15.000000 sharetop-2.4.5/sharetop/core/stock/bill_monitor.py
--rw-rw-rw-   0        0        0     1924 2023-07-17 00:35:01.000000 sharetop-2.4.5/sharetop/core/stock/config.py
--rw-rw-rw-   0        0        0    14859 2023-07-17 00:49:08.000000 sharetop-2.4.5/sharetop/core/stock/getter.py
--rw-rw-rw-   0        0        0    10345 2023-07-15 08:48:35.000000 sharetop-2.4.5/sharetop/core/stock/quarterly_report.py
--rw-rw-rw-   0        0        0    10130 2023-07-15 08:58:53.000000 sharetop-2.4.5/sharetop/core/stock/rank_list.py
--rw-rw-rw-   0        0        0      520 2023-07-10 12:22:58.000000 sharetop-2.4.5/sharetop/core/stock/stock_base_info.py
--rw-rw-rw-   0        0        0     7299 2023-07-10 03:31:49.000000 sharetop-2.4.5/sharetop/core/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-18 11:58:10.004552 sharetop-2.4.5/sharetop/crawl/
--rw-rw-rw-   0        0        0       29 2023-04-09 23:19:21.000000 sharetop-2.4.5/sharetop/crawl/__init__.py
--rw-rw-rw-   0        0        0     1088 2023-07-16 09:52:34.000000 sharetop-2.4.5/sharetop/crawl/base.py
--rw-rw-rw-   0        0        0     3271 2023-07-09 23:57:40.000000 sharetop-2.4.5/sharetop/crawl/settings.py
-drwxrwxrwx   0        0        0        0 2023-07-18 11:58:10.034783 sharetop-2.4.5/sharetop/parser/
--rw-rw-rw-   0        0        0       27 2023-04-10 00:54:05.000000 sharetop-2.4.5/sharetop/parser/__init__.py
--rw-rw-rw-   0        0        0     4239 2023-05-23 12:33:52.000000 sharetop-2.4.5/sharetop/parser/base.py
--rw-rw-rw-   0        0        0     2906 2023-05-19 00:08:10.000000 sharetop-2.4.5/sharetop/parser/config.py
-drwxrwxrwx   0        0        0        0 2023-07-18 11:58:10.211184 sharetop-2.4.5/sharetop/test/
--rw-rw-rw-   0        0        0        0 2023-04-29 10:57:35.000000 sharetop-2.4.5/sharetop/test/__init__.py
--rw-rw-rw-   0        0        0      432 2023-07-16 01:29:33.000000 sharetop-2.4.5/sharetop/test/bond_test.py
--rw-rw-rw-   0        0        0      199 2023-05-17 04:49:54.000000 sharetop-2.4.5/sharetop/test/captial.py
--rw-rw-rw-   0        0        0      172 2023-07-16 02:38:09.000000 sharetop-2.4.5/sharetop/test/country_test.py
--rw-rw-rw-   0        0        0      523 2023-07-15 15:16:22.000000 sharetop-2.4.5/sharetop/test/flow_monitor_test.py
--rw-rw-rw-   0        0        0     1450 2023-07-16 01:04:05.000000 sharetop-2.4.5/sharetop/test/fund_test.py
--rw-rw-rw-   0        0        0      382 2023-07-16 02:09:22.000000 sharetop-2.4.5/sharetop/test/futures_test.py
--rw-rw-rw-   0        0        0      504 2023-07-10 00:25:56.000000 sharetop-2.4.5/sharetop/test/oil_test.py
--rw-rw-rw-   0        0        0      198 2023-07-15 10:47:58.000000 sharetop-2.4.5/sharetop/test/pig_test.py
--rw-rw-rw-   0        0        0     1318 2023-07-18 04:55:00.000000 sharetop-2.4.5/sharetop/test/stock_test.py
--rw-rw-rw-   0        0        0      992 2023-07-17 01:23:58.000000 sharetop-2.4.5/sharetop/test/test1.py
--rw-rw-rw-   0        0        0     1997 2023-05-02 03:48:40.000000 sharetop-2.4.5/sharetop/test/test2-akshare.py
--rw-rw-rw-   0        0        0     3709 2023-05-03 07:10:48.000000 sharetop-2.4.5/sharetop/test/test3.py
--rw-rw-rw-   0        0        0      219 2023-05-04 04:00:10.000000 sharetop-2.4.5/sharetop/test/test4.py
--rw-rw-rw-   0        0        0      690 2023-07-15 03:35:15.000000 sharetop-2.4.5/sharetop/test/test5.py
--rw-rw-rw-   0        0        0     1227 2023-07-15 03:35:15.000000 sharetop-2.4.5/sharetop/test/test6.py
--rw-rw-rw-   0        0        0      643 2023-07-05 12:16:23.000000 sharetop-2.4.5/sharetop/test/test7.py
-drwxrwxrwx   0        0        0        0 2023-07-18 11:58:09.327276 sharetop-2.4.5/sharetop.egg-info/
--rw-rw-rw-   0        0        0    51253 2023-07-18 11:58:09.000000 sharetop-2.4.5/sharetop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2417 2023-07-18 11:58:09.000000 sharetop-2.4.5/sharetop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 11:58:09.000000 sharetop-2.4.5/sharetop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-07-18 11:58:09.000000 sharetop-2.4.5/sharetop.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-18 11:58:09.000000 sharetop-2.4.5/sharetop.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 15:09:29.820037 sharetop-2.4.6/
+-rw-rw-rw-   0        0        0     1066 2023-04-26 14:07:21.000000 sharetop-2.4.6/LICENSE
+-rw-rw-rw-   0        0        0    51253 2023-07-31 15:09:29.817675 sharetop-2.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0    49774 2023-07-15 03:35:16.000000 sharetop-2.4.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-31 15:09:29.820037 sharetop-2.4.6/setup.cfg
+-rw-rw-rw-   0        0        0     1219 2023-04-29 06:50:50.000000 sharetop-2.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 15:09:28.982454 sharetop-2.4.6/sharetop/
+-rw-rw-rw-   0        0        0      297 2023-05-18 12:23:41.000000 sharetop-2.4.6/sharetop/__init__.py
+-rw-rw-rw-   0        0        0      386 2023-07-31 15:08:44.000000 sharetop-2.4.6/sharetop/__version__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 15:09:29.044535 sharetop-2.4.6/sharetop/api/
+-rw-rw-rw-   0        0        0      306 2023-07-02 13:11:41.000000 sharetop-2.4.6/sharetop/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 15:09:29.064129 sharetop-2.4.6/sharetop/application/
+-rw-rw-rw-   0        0        0       33 2023-04-21 11:53:52.000000 sharetop-2.4.6/sharetop/application/__init__.py
+-rw-rw-rw-   0        0        0     4459 2023-07-16 22:42:50.000000 sharetop-2.4.6/sharetop/application/base.py
+drwxrwxrwx   0        0        0        0 2023-07-31 15:09:29.095302 sharetop-2.4.6/sharetop/core/
+-rw-rw-rw-   0        0        0        0 2023-04-08 05:23:09.000000 sharetop-2.4.6/sharetop/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 15:09:29.174110 sharetop-2.4.6/sharetop/core/bond/
+-rw-rw-rw-   0        0        0      592 2023-07-15 11:00:24.000000 sharetop-2.4.6/sharetop/core/bond/__init__.py
+-rw-rw-rw-   0        0        0     1869 2023-04-24 04:28:03.000000 sharetop-2.4.6/sharetop/core/bond/config.py
+-rw-rw-rw-   0        0        0     9571 2023-07-16 01:28:38.000000 sharetop-2.4.6/sharetop/core/bond/get_bond_info.py
+-rw-rw-rw-   0        0        0    19614 2023-07-15 10:59:53.000000 sharetop-2.4.6/sharetop/core/bond/get_bond_public_info.py
+-rw-rw-rw-   0        0        0      598 2023-04-10 05:06:06.000000 sharetop-2.4.6/sharetop/core/cache.py
+drwxrwxrwx   0        0        0        0 2023-07-31 15:09:29.198343 sharetop-2.4.6/sharetop/core/capital_flow/
+-rw-rw-rw-   0        0        0      367 2023-07-15 15:19:38.000000 sharetop-2.4.6/sharetop/core/capital_flow/__init__.py
+-rw-rw-rw-   0        0        0     6785 2023-07-25 15:02:39.000000 sharetop-2.4.6/sharetop/core/capital_flow/capital_flow_monitor.py
+drwxrwxrwx   0        0        0        0 2023-07-31 15:09:29.262406 sharetop-2.4.6/sharetop/core/common/
+-rw-rw-rw-   0        0        0      188 2023-04-27 15:24:55.000000 sharetop-2.4.6/sharetop/core/common/__init__.py
+-rw-rw-rw-   0        0        0     3727 2023-07-19 03:47:04.000000 sharetop-2.4.6/sharetop/core/common/common_base.py
+-rw-rw-rw-   0        0        0     8688 2023-05-25 01:16:42.000000 sharetop-2.4.6/sharetop/core/common/config.py
+-rw-rw-rw-   0        0        0    15132 2023-07-31 15:05:35.000000 sharetop-2.4.6/sharetop/core/common/explain_change.py
+-rw-rw-rw-   0        0        0    12428 2023-07-16 01:53:16.000000 sharetop-2.4.6/sharetop/core/common/getter.py
+-rw-rw-rw-   0        0        0      750 2023-04-09 05:42:43.000000 sharetop-2.4.6/sharetop/core/config.py
+drwxrwxrwx   0        0        0        0 2023-07-31 15:09:29.301096 sharetop-2.4.6/sharetop/core/country/
+-rw-rw-rw-   0        0        0       91 2023-07-16 02:39:07.000000 sharetop-2.4.6/sharetop/core/country/__init__.py
+-rw-rw-rw-   0        0        0      491 2023-05-09 01:30:20.000000 sharetop-2.4.6/sharetop/core/country/config.py
+-rw-rw-rw-   0        0        0      697 2023-07-16 02:39:07.000000 sharetop-2.4.6/sharetop/core/country/country_base_info.py
+drwxrwxrwx   0        0        0        0 2023-07-31 15:09:29.406708 sharetop-2.4.6/sharetop/core/fund/
+-rw-rw-rw-   0        0        0     1025 2023-07-31 14:59:03.000000 sharetop-2.4.6/sharetop/core/fund/__init__.py
+-rw-rw-rw-   0        0        0      927 2023-07-28 01:21:27.000000 sharetop-2.4.6/sharetop/core/fund/config.py
+-rw-rw-rw-   0        0        0     2727 2023-07-28 00:06:51.000000 sharetop-2.4.6/sharetop/core/fund/fund_list.py
+-rw-rw-rw-   0        0        0     1857 2023-07-31 14:52:45.000000 sharetop-2.4.6/sharetop/core/fund/get_fund_base_info.py
+-rw-rw-rw-   0        0        0     2624 2023-07-31 15:04:18.000000 sharetop-2.4.6/sharetop/core/fund/get_fund_history_data.py
+-rw-rw-rw-   0        0        0     3716 2023-07-15 10:12:05.000000 sharetop-2.4.6/sharetop/core/fund/get_fund_industry_info.py
+-rw-rw-rw-   0        0        0     5474 2023-07-15 10:19:50.000000 sharetop-2.4.6/sharetop/core/fund/get_fund_invest_info.py
+-rw-rw-rw-   0        0        0    12432 2023-07-31 14:59:03.000000 sharetop-2.4.6/sharetop/core/fund/get_fund_rank.py
+-rw-rw-rw-   0        0        0     1466 2023-04-22 03:27:53.000000 sharetop-2.4.6/sharetop/core/fund/get_fund_real_time.py
+-rw-rw-rw-   0        0        0     2497 2023-07-15 10:37:11.000000 sharetop-2.4.6/sharetop/core/fund/get_period_change_info.py
+-rw-rw-rw-   0        0        0     2451 2023-07-15 10:39:55.000000 sharetop-2.4.6/sharetop/core/fund/get_types_percentage_info.py
+drwxrwxrwx   0        0        0        0 2023-07-31 15:09:29.437035 sharetop-2.4.6/sharetop/core/futures/
+-rw-rw-rw-   0        0        0      250 2023-07-16 02:07:46.000000 sharetop-2.4.6/sharetop/core/futures/__init__.py
+-rw-rw-rw-   0        0        0    10057 2023-07-16 02:09:22.000000 sharetop-2.4.6/sharetop/core/futures/get_futures_info.py
+drwxrwxrwx   0        0        0        0 2023-07-31 15:09:29.472373 sharetop-2.4.6/sharetop/core/oil/
+-rw-rw-rw-   0        0        0      402 2023-05-16 01:17:51.000000 sharetop-2.4.6/sharetop/core/oil/__init__.py
+-rw-rw-rw-   0        0        0     1685 2023-05-15 00:28:25.000000 sharetop-2.4.6/sharetop/core/oil/config.py
+-rw-rw-rw-   0        0        0     3614 2023-07-10 00:25:56.000000 sharetop-2.4.6/sharetop/core/oil/oil_detail.py
+drwxrwxrwx   0        0        0        0 2023-07-31 15:09:29.505159 sharetop-2.4.6/sharetop/core/pig/
+-rw-rw-rw-   0        0        0       84 2023-07-15 10:46:51.000000 sharetop-2.4.6/sharetop/core/pig/__init__.py
+-rw-rw-rw-   0        0        0      163 2023-05-16 00:42:46.000000 sharetop-2.4.6/sharetop/core/pig/config.py
+-rw-rw-rw-   0        0        0     1428 2023-07-15 10:46:51.000000 sharetop-2.4.6/sharetop/core/pig/pig_detail.py
+drwxrwxrwx   0        0        0        0 2023-07-31 15:09:29.581350 sharetop-2.4.6/sharetop/core/stock/
+-rw-rw-rw-   0        0        0      662 2023-07-15 09:27:19.000000 sharetop-2.4.6/sharetop/core/stock/__init__.py
+-rw-rw-rw-   0        0        0     4834 2023-07-20 01:18:36.000000 sharetop-2.4.6/sharetop/core/stock/bill_monitor.py
+-rw-rw-rw-   0        0        0     1163 2023-07-19 01:27:46.000000 sharetop-2.4.6/sharetop/core/stock/config.py
+-rw-rw-rw-   0        0        0    15110 2023-07-20 01:10:32.000000 sharetop-2.4.6/sharetop/core/stock/getter.py
+-rw-rw-rw-   0        0        0    10620 2023-07-19 01:27:46.000000 sharetop-2.4.6/sharetop/core/stock/quarterly_report.py
+-rw-rw-rw-   0        0        0    10240 2023-07-27 23:27:15.000000 sharetop-2.4.6/sharetop/core/stock/rank_list.py
+-rw-rw-rw-   0        0        0      693 2023-07-19 12:30:45.000000 sharetop-2.4.6/sharetop/core/stock/stock_base_info.py
+-rw-rw-rw-   0        0        0     7299 2023-07-19 04:12:02.000000 sharetop-2.4.6/sharetop/core/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-31 15:09:29.614196 sharetop-2.4.6/sharetop/crawl/
+-rw-rw-rw-   0        0        0       29 2023-04-09 23:19:21.000000 sharetop-2.4.6/sharetop/crawl/__init__.py
+-rw-rw-rw-   0        0        0     1088 2023-07-19 05:03:18.000000 sharetop-2.4.6/sharetop/crawl/base.py
+-rw-rw-rw-   0        0        0     3271 2023-07-09 23:57:40.000000 sharetop-2.4.6/sharetop/crawl/settings.py
+drwxrwxrwx   0        0        0        0 2023-07-31 15:09:29.648774 sharetop-2.4.6/sharetop/parser/
+-rw-rw-rw-   0        0        0       27 2023-04-10 00:54:05.000000 sharetop-2.4.6/sharetop/parser/__init__.py
+-rw-rw-rw-   0        0        0     4364 2023-07-19 04:59:24.000000 sharetop-2.4.6/sharetop/parser/base.py
+-rw-rw-rw-   0        0        0     2911 2023-07-19 05:36:09.000000 sharetop-2.4.6/sharetop/parser/config.py
+drwxrwxrwx   0        0        0        0 2023-07-31 15:09:29.817107 sharetop-2.4.6/sharetop/test/
+-rw-rw-rw-   0        0        0        0 2023-04-29 10:57:35.000000 sharetop-2.4.6/sharetop/test/__init__.py
+-rw-rw-rw-   0        0        0      432 2023-07-16 01:29:33.000000 sharetop-2.4.6/sharetop/test/bond_test.py
+-rw-rw-rw-   0        0        0      199 2023-05-17 04:49:54.000000 sharetop-2.4.6/sharetop/test/captial.py
+-rw-rw-rw-   0        0        0      172 2023-07-16 02:38:09.000000 sharetop-2.4.6/sharetop/test/country_test.py
+-rw-rw-rw-   0        0        0      582 2023-07-25 15:03:47.000000 sharetop-2.4.6/sharetop/test/flow_monitor_test.py
+-rw-rw-rw-   0        0        0     1558 2023-07-31 15:01:19.000000 sharetop-2.4.6/sharetop/test/fund_test.py
+-rw-rw-rw-   0        0        0      382 2023-07-16 02:09:22.000000 sharetop-2.4.6/sharetop/test/futures_test.py
+-rw-rw-rw-   0        0        0      504 2023-07-10 00:25:56.000000 sharetop-2.4.6/sharetop/test/oil_test.py
+-rw-rw-rw-   0        0        0      198 2023-07-15 10:47:58.000000 sharetop-2.4.6/sharetop/test/pig_test.py
+-rw-rw-rw-   0        0        0     1205 2023-07-27 23:28:24.000000 sharetop-2.4.6/sharetop/test/stock_test.py
+-rw-rw-rw-   0        0        0      992 2023-07-17 01:23:58.000000 sharetop-2.4.6/sharetop/test/test1.py
+-rw-rw-rw-   0        0        0     1997 2023-05-02 03:48:40.000000 sharetop-2.4.6/sharetop/test/test2-akshare.py
+-rw-rw-rw-   0        0        0     3709 2023-05-03 07:10:48.000000 sharetop-2.4.6/sharetop/test/test3.py
+-rw-rw-rw-   0        0        0      221 2023-07-30 10:45:50.000000 sharetop-2.4.6/sharetop/test/test4.py
+-rw-rw-rw-   0        0        0      690 2023-07-15 03:35:15.000000 sharetop-2.4.6/sharetop/test/test5.py
+-rw-rw-rw-   0        0        0     1227 2023-07-15 03:35:15.000000 sharetop-2.4.6/sharetop/test/test6.py
+-rw-rw-rw-   0        0        0      643 2023-07-05 12:16:23.000000 sharetop-2.4.6/sharetop/test/test7.py
+drwxrwxrwx   0        0        0        0 2023-07-31 15:09:29.032958 sharetop-2.4.6/sharetop.egg-info/
+-rw-rw-rw-   0        0        0    51253 2023-07-31 15:09:28.000000 sharetop-2.4.6/sharetop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2456 2023-07-31 15:09:28.000000 sharetop-2.4.6/sharetop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 15:09:28.000000 sharetop-2.4.6/sharetop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-07-31 15:09:28.000000 sharetop-2.4.6/sharetop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-31 15:09:28.000000 sharetop-2.4.6/sharetop.egg-info/top_level.txt
```

### Comparing `sharetop-2.4.5/LICENSE` & `sharetop-2.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.5/PKG-INFO` & `sharetop-2.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharetop
-Version: 2.4.5
+Version: 2.4.6
 Summary: Provide data related to the economic market
 Home-page: https://github.com/nrliangxy/sharetop
 Author: nrliangxy
 Author-email: nrliangxy@foxmail.com
 License: MIT
 Project-URL: Source, https://github.com/nrliangxy/sharetop
 Keywords: data,finance,quant,stock,fund,futures,share
```

### Comparing `sharetop-2.4.5/README.md` & `sharetop-2.4.6/README.md`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.5/setup.py` & `sharetop-2.4.6/setup.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.5/sharetop/application/base.py` & `sharetop-2.4.6/sharetop/application/base.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.5/sharetop/core/bond/__init__.py` & `sharetop-2.4.6/sharetop/core/bond/__init__.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.5/sharetop/core/bond/config.py` & `sharetop-2.4.6/sharetop/core/bond/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.5/sharetop/core/bond/get_bond_info.py` & `sharetop-2.4.6/sharetop/core/bond/get_bond_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.5/sharetop/core/bond/get_bond_public_info.py` & `sharetop-2.4.6/sharetop/core/bond/get_bond_public_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.5/sharetop/core/cache.py` & `sharetop-2.4.6/sharetop/core/cache.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.5/sharetop/core/capital_flow/capital_flow_monitor.py` & `sharetop-2.4.6/sharetop/core/capital_flow/capital_flow_monitor.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from ..utils import to_numeric, validate_request
 from ..common.getter import get_history_bill as get_history_bill_for_stock
 from ..common.getter import get_real_time_bill_data_one
 from ..common.common_base import CommonFunc
+from ..common.explain_change import exchange_explain
 from typing import Dict, List, Union
 import pandas as pd
 
 common_func_obj = CommonFunc()
 
 
 @validate_request
 @to_numeric
-def get_stock_history_capital(token: str, stock_code: str) -> pd.DataFrame:
+def get_stock_history_capital(token: str, stock_code: str, is_explain: bool = False) -> pd.DataFrame:
     """
     获取单只股票历史单子流入流出数据
     Parameters
     ----------
     stock_code : str
         股票代码
     Returns
@@ -31,28 +32,28 @@
     4    贵州茅台  600519  2021-03-10 -2.044173e+08  -1551798.0  2.059690e+08 -2.378506e+08  3.343331e+07    -2.02    -0.02     2.03    -2.35      0.33  1950.72  1.72
     ..    ...     ...         ...           ...         ...           ...           ...           ...      ...      ...      ...      ...       ...      ...   ...
     97   贵州茅台  600519  2021-07-26 -1.564233e+09  13142211.0  1.551091e+09 -1.270400e+08 -1.437193e+09    -8.74     0.07     8.67    -0.71     -8.03  1804.11 -5.05
     98   贵州茅台  600519  2021-07-27 -7.803296e+08 -10424715.0  7.907544e+08  6.725104e+07 -8.475807e+08    -5.12    -0.07     5.19     0.44     -5.56  1712.89 -5.06
     99   贵州茅台  600519  2021-07-28  3.997645e+08   2603511.0 -4.023677e+08  2.315648e+08  1.681997e+08     2.70     0.02    -2.72     1.57      1.14  1768.90  3.27
     100  贵州茅台  600519  2021-07-29 -9.209842e+08  -2312235.0  9.232964e+08 -3.959741e+08 -5.250101e+08    -8.15    -0.02     8.17    -3.50     -4.65  1749.79 -1.08
     101  贵州茅台  600519  2021-07-30 -1.524740e+09  -6020099.0  1.530761e+09  1.147248e+08 -1.639465e+09   -11.63    -0.05    11.68     0.88    -12.51  1678.99 -4.05
+    :param is_explain:
     :param stock_code:
     :param token:
 
     """
     df = get_history_bill_for_stock(stock_code)
     df.rename(columns={'代码': '股票代码', '名称': '股票名称'}, inplace=True)
-    return df
+    return exchange_explain(df, is_explain)
 
 
 @to_numeric
-def get_stock_real_time_daily_capital(stock_code: str) -> pd.DataFrame:
+def get_stock_real_time_daily_capital(stock_code: str, is_explain: bool = False) -> pd.DataFrame:
     """
     获取单只股票最新交易日的日内分钟级单子流入流出数据
-
     Parameters
     ----------
     stock_code : str
         股票代码
     Returns
     -------
     DataFrame
@@ -68,46 +69,49 @@
     4    600519  2021-07-29 09:35    7853716.0  -970615.0   -6883104.0  -75692436.0   83546152.0
     ..      ...               ...          ...        ...          ...          ...          ...
     235  600519  2021-07-29 14:56 -918956019.0 -1299630.0  920255661.0 -397127393.0 -521828626.0
     236  600519  2021-07-29 14:57 -920977761.0 -2319213.0  923296987.0 -397014702.0 -523963059.0
     237  600519  2021-07-29 14:58 -920984196.0 -2312233.0  923296442.0 -395974137.0 -525010059.0
     238  600519  2021-07-29 14:59 -920984196.0 -2312233.0  923296442.0 -395974137.0 -525010059.0
     239  600519  2021-07-29 15:00 -920984196.0 -2312233.0  923296442.0 -395974137.0 -525010059.0
+    :param stock_code:
+    :param is_explain:
     """
     df = get_real_time_bill_data_one(stock_code)
-    return df
+    return exchange_explain(df, is_explain)
 
 
-def get_stock_real_time_sum_capital(stock_codes: Union[str, List[str]],
-                               ) -> Union[pd.DataFrame, Dict[str, pd.DataFrame]]:
+def get_stock_real_time_sum_capital(stock_codes: Union[str, List[str]], is_explain: bool = False
+                                    ) -> Union[pd.DataFrame, Dict[str, pd.DataFrame]]:
     """
     获取单只股票最新交易日的日内最新单子流入流出数据
     Parameters
     ----------
     stock_codes : 股票、债券代码 str 或者是 list
     如果是 str，为单支股票，如果为list，为多支股票
     Returns
     -------
     DataFrame
         单支或者多支股票、债券最新交易日的日内实时子流入流出数据
+        :param stock_codes:
+        :param is_explain:
     """
     base_func_name = get_stock_real_time_sum_capital.__name__
-    return common_func_obj.get_common_func(stock_codes, base_func_name)
+    return exchange_explain(common_func_obj.get_common_func(stock_codes, base_func_name), is_explain)
 
 
-def get_stock_real_time_sector_capital(sector: str, monitor_time: str):
+def get_stock_real_time_sector_capital(sector: str, monitor_time: str, is_explain: bool = False):
     """
+    :param is_explain:
     :param sector: industry: 行业, concept: 概念, area: 地域
     :param monitor_time: 1: 当天, 5: 5日,  10: 10日
     :return:
     """
     allowed_values = ['industry', 'concept', 'area']
     if sector not in allowed_values:
         raise ValueError(f"Invalid input: {sector}. Allowed values are {allowed_values}")
     monitor_time_allowed_values = ['1', '5', '10']
     if monitor_time not in monitor_time_allowed_values:
         raise ValueError(f"Invalid input: {monitor_time}. Allowed values are {monitor_time_allowed_values}")
     kwargs = {"monitor_time": monitor_time}
     base_func_name = get_stock_real_time_sector_capital.__name__
-    return common_func_obj.get_common_func(sector, base_func_name, **kwargs)
-
-
+    return exchange_explain(common_func_obj.get_common_func(sector, base_func_name, **kwargs), is_explain)
```

### Comparing `sharetop-2.4.5/sharetop/core/common/common_base.py` & `sharetop-2.4.6/sharetop/core/common/common_base.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.5/sharetop/core/common/config.py` & `sharetop-2.4.6/sharetop/core/common/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.5/sharetop/core/common/getter.py` & `sharetop-2.4.6/sharetop/core/common/getter.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.5/sharetop/core/config.py` & `sharetop-2.4.6/sharetop/core/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.5/sharetop/core/country/country_base_info.py` & `sharetop-2.4.6/sharetop/core/country/country_base_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.5/sharetop/core/fund/__init__.py` & `sharetop-2.4.6/sharetop/core/fund/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .get_types_percentage_info import get_fund_types_percentage
 from .get_fund_base_info import get_fund_base_info
 from .get_fund_industry_info import get_fund_industry_distribution
 from .get_fund_rank import (
     get_fund_open_rank,
     get_fund_exchange_rank,
     get_fund_money_rank,
-    fund_hk_rank
+    get_fund_hk_rank
 )
 
 __all__ = [
     'get_fund_codes',
     'get_fund_real_time_god',
     'get_fund_history_price',
     'get_fund_invest_position',
@@ -22,9 +22,9 @@
     'get_fund_period_change',
     'get_fund_types_percentage',
     'get_fund_base_info',
     'get_fund_industry_distribution',
     'get_fund_open_rank',
     'get_fund_exchange_rank',
     'get_fund_money_rank',
-    'fund_hk_rank'
+    'get_fund_hk_rank'
 ]
```

### Comparing `sharetop-2.4.5/sharetop/core/fund/config.py` & `sharetop-2.4.6/sharetop/core/fund/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,9 +21,10 @@
     "SYL_6Y": "近6月",
     "SYL_1N": "近1年",
     "SYL_2N": "近2年",
     "SYL_3N": "近3年",
     "SYL_5N": "近5年",
     "SYL_JN": "今年来",
     "SYL_LN": "成立来",
+    "index": '序号'
 }
```

### Comparing `sharetop-2.4.5/sharetop/core/fund/fund_list.py` & `sharetop-2.4.6/sharetop/core/fund/fund_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import re
 import pandas as pd
 from retry import retry
 from ..utils import requests_obj, validate_request
 from ..common.getter import BaseApplication
+from ..common.explain_change import exchange_explain
 
 
 @validate_request
 @retry(tries=3)
-def get_fund_codes(token: str, ft: str = None) -> pd.DataFrame:
+def get_fund_codes(token: str, ft: str = None, is_explain: bool = False) -> pd.DataFrame:
     """
     获取天天基金网公开的全部公墓基金名单
     Parameters
     ----------
     ft : str, optional
         基金类型可选示例如下
         - ``'zq'``  : 债券类型基金
@@ -36,14 +37,15 @@
     4     004041             金鹰医疗健康产业C
     ...      ...                   ...
     1981  012503      国泰中证环保产业50ETF联接A
     1982  012517  国泰中证细分机械设备产业主题ETF联接C
     1983  012600             中银内核驱动股票C
     1984  011043             国泰价值先锋股票C
     1985  012516  国泰中证细分机械设备产业主题ETF联接A
+    :param is_explain:
     :param ft:
     :param token:
     """
     params = [
         ('op', 'dy'),
         ('dt', 'kf'),
         ('rs', ''),
@@ -66,8 +68,8 @@
     if ft is not None:
         params.append(('ft', ft))
     url = 'http://fund.eastmoney.com/data/rankhandler.aspx'
     response = requests_obj.get(url, params, headers=headers)
     results = re.findall('\[.*\]', response.text)
     new_results = eval(results[0])
     application_obj = BaseApplication(new_results)
-    return application_obj.deal_fund_list()
+    return exchange_explain(application_obj.deal_fund_list(), is_explain)
```

### Comparing `sharetop-2.4.5/sharetop/core/fund/get_fund_base_info.py` & `sharetop-2.4.6/sharetop/core/fund/get_fund_base_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import rich
 import uuid
 import pandas as pd
 from retry import retry
 from ..utils import to_numeric, requests_obj, validate_request
 from .config import EastmoneyFundHeaders
 from ...crawl.settings import *
+from ..common.explain_change import exchange_explain
 
 
 @validate_request
 @retry(tries=3)
 @to_numeric
-def get_fund_base_info(token: str, fund_code: str) -> pd.Series:
+def get_fund_base_info(token: str, fund_code: str, is_explain: bool = False) -> pd.Series:
     """
     获取基金的一些基本信息
     Parameters
     ----------
     fund_code : str
         6 位基金代码
     Returns
     -------
     Series
         基金的一些基本信息
+        :param is_explain:
         :param fund_code:
         :param token:
     """
     str_uuid = str(uuid.uuid4()).upper()
     params = (
         ('FCODE', fund_code),
         ('deviceid', str_uuid),
@@ -43,15 +45,15 @@
         'FSRQ': '净值更新日期',
         'COMMENTS': '简介',
         'ENDNAV': '基金规模',
         'FEGMRQ': '基金规模更新时间',
         'RLEVEL_SZ': '最新评级'
     }
     items = json_response['Datas']
+    items = {columns.get(k): v for k, v in items.items() if columns.get(k)}
     if not items:
         rich.print('基金代码', fund_code, '可能有误')
         return pd.Series(index=columns.values())
 
-    s = pd.Series(json_response['Datas']).rename(index=columns)[columns.values()]
-
-    s = s.apply(lambda x: x.replace('\n', ' ').strip() if isinstance(x, str) else x)
-    return s
+    s = pd.DataFrame([items])
+    df = s.apply(lambda x: x.replace('\n', ' ').strip() if isinstance(x, str) else x)
+    return exchange_explain(df, is_explain)
```

### Comparing `sharetop-2.4.5/sharetop/core/fund/get_fund_history_data.py` & `sharetop-2.4.6/sharetop/core/fund/get_fund_history_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import pandas as pd
 from ..utils import to_numeric, requests_obj, validate_request
 from retry import retry
 from .config import EastmoneyFundHeaders
 from ...crawl.settings import *
+from ..common.explain_change import exchange_explain
 
 
 @validate_request
 @retry(tries=3)
 @to_numeric
-def get_fund_history_price(token: str, fund_code: str, pz: int = 40000) -> pd.DataFrame:
+def get_fund_history_price(token: str, fund_code: str, pz: int = 40000, is_explain: bool = False) -> pd.DataFrame:
     """
     根据基金代码和要获取的页码抓取基金净值信息
 
     Parameters
     ----------
     fund_code : str
         6 位基金代码
@@ -34,14 +35,15 @@
     4    2021-06-07  1.6466  3.2777    1.61
     ...         ...     ...     ...     ...
     1469 2015-06-08  1.0380  1.0380  2.5692
     1470 2015-06-05  1.0120  1.0120  1.5045
     1471 2015-06-04  0.9970  0.9970      --
     1472 2015-05-29  0.9950  0.9950      --
     1473 2015-05-27  1.0000  1.0000      --
+    :param is_explain:
     :param pz:
     :param fund_code:
     :param token:
 
     """
     data = {
         'FCODE': f'{fund_code}',
@@ -75,8 +77,8 @@
                 '日期': date,
                 '单位净值': stock['DWJZ'],
                 '累计净值': stock['LJJZ'],
                 '涨跌幅': stock['JZZZL'],
             }
         )
     df = pd.DataFrame(rows)
-    return df
+    return exchange_explain(df, is_explain)
```

### Comparing `sharetop-2.4.5/sharetop/core/fund/get_fund_industry_info.py` & `sharetop-2.4.6/sharetop/core/fund/get_fund_industry_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.5/sharetop/core/fund/get_fund_invest_info.py` & `sharetop-2.4.6/sharetop/core/fund/get_fund_invest_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.5/sharetop/core/fund/get_fund_rank.py` & `sharetop-2.4.6/sharetop/core/fund/get_fund_rank.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import requests
 import datetime
 import re
 import pandas as pd
 from ..utils import requests_obj, parse_obj, validate_request
 from .config import fund_money_cloumns
+from ..common.explain_change import exchange_explain
 
 
 def fund_export_df(text_data):
     json_data = parse_obj.parse_fund_json(text_data)
     temp_df = pd.DataFrame(json_data)
     temp_df = temp_df.iloc[:, 0].str.split(",", expand=True)
     temp_df.reset_index(inplace=True)
     temp_df["index"] = list(range(1, len(temp_df) + 1))
     return temp_df
 
 
 @validate_request
-def get_fund_open_rank(token: str, symbol: str = "全部") -> pd.DataFrame:
+def get_fund_open_rank(token: str, symbol: str = "全部", is_explain: bool = False) -> pd.DataFrame:
     """
     东方财富网-数据中心-开放基金排行
     https://fund.eastmoney.com/data/fundranking.html
+    :param token:
+    :param is_explain:
     :param symbol: choice of {"全部", "股票型", "混合型", "债券型", "指数型", "QDII", "LOF", "FOF"}
     :type symbol: str
     :return: 开放基金排行
     :rtype: pandas.DataFrame
     """
     current_date = datetime.datetime.now().date().isoformat()
     last_date = str(int(current_date[:4]) - 1) + current_date[4:]
@@ -104,23 +107,22 @@
             "近3月",
             "近6月",
             "近1年",
             "近2年",
             "近3年",
             "今年来",
             "成立来",
-            "自定义",
             "手续费",
         ]
     ]
-    return temp_df
+    return exchange_explain(temp_df, is_explain)
 
 
 @validate_request
-def get_fund_exchange_rank(token: str) -> pd.DataFrame:
+def get_fund_exchange_rank(token: str, is_explain: bool = False) -> pd.DataFrame:
     """
     东方财富网-数据中心-场内交易基金排行
     https://fund.eastmoney.com/data/fbsfundranking.html
     :return: 场内交易基金数据
     :rtype: pandas.DataFrame
     """
     url = "http://fund.eastmoney.com/data/rankhandler.aspx"
@@ -186,32 +188,32 @@
             "近2年",
             "近3年",
             "今年来",
             "成立来",
             "成立日期",
         ]
     ]
-    temp_df['日期'] = pd.to_datetime(temp_df['日期']).dt.date
-    temp_df['成立日期'] = pd.to_datetime(temp_df['成立日期']).dt.date
-    temp_df['单位净值'] = pd.to_numeric(temp_df['单位净值'], errors="coerce")
-    temp_df['累计净值'] = pd.to_numeric(temp_df['累计净值'], errors="coerce")
-    temp_df['近1周'] = pd.to_numeric(temp_df['近1周'], errors="coerce")
-    temp_df['近1月'] = pd.to_numeric(temp_df['近1月'], errors="coerce")
-    temp_df['近3月'] = pd.to_numeric(temp_df['近3月'], errors="coerce")
-    temp_df['近6月'] = pd.to_numeric(temp_df['近6月'], errors="coerce")
-    temp_df['近1年'] = pd.to_numeric(temp_df['近1年'], errors="coerce")
-    temp_df['近2年'] = pd.to_numeric(temp_df['近2年'], errors="coerce")
-    temp_df['近3年'] = pd.to_numeric(temp_df['近3年'], errors="coerce")
-    temp_df['今年来'] = pd.to_numeric(temp_df['今年来'], errors="coerce")
-    temp_df['成立来'] = pd.to_numeric(temp_df['成立来'], errors="coerce")
-    return temp_df
+    # temp_df['日期'] = pd.to_datetime(temp_df['日期']).dt.date
+    # temp_df['成立日期'] = pd.to_datetime(temp_df['成立日期']).dt.date
+    # temp_df['单位净值'] = pd.to_numeric(temp_df['单位净值'], errors="coerce")
+    # temp_df['累计净值'] = pd.to_numeric(temp_df['累计净值'], errors="coerce")
+    # temp_df['近1周'] = pd.to_numeric(temp_df['近1周'], errors="coerce")
+    # temp_df['近1月'] = pd.to_numeric(temp_df['近1月'], errors="coerce")
+    # temp_df['近3月'] = pd.to_numeric(temp_df['近3月'], errors="coerce")
+    # temp_df['近6月'] = pd.to_numeric(temp_df['近6月'], errors="coerce")
+    # temp_df['近1年'] = pd.to_numeric(temp_df['近1年'], errors="coerce")
+    # temp_df['近2年'] = pd.to_numeric(temp_df['近2年'], errors="coerce")
+    # temp_df['近3年'] = pd.to_numeric(temp_df['近3年'], errors="coerce")
+    # temp_df['今年来'] = pd.to_numeric(temp_df['今年来'], errors="coerce")
+    # temp_df['成立来'] = pd.to_numeric(temp_df['成立来'], errors="coerce")
+    return exchange_explain(temp_df, is_explain)
 
 
 @validate_request
-def get_fund_money_rank(token: str) -> pd.DataFrame:
+def get_fund_money_rank(token: str, is_explain: bool = False) -> pd.DataFrame:
     """
     东方财富网-数据中心-货币型基金排行
     https://fund.eastmoney.com/data/hbxfundranking.html
     :return: 货币型基金排行
     :rtype: pandas.DataFrame
     """
     url = "http://api.fund.eastmoney.com/FundRank/GetHbRankList"
@@ -235,36 +237,36 @@
     for _ in json_data["Data"]:
         temp_dict = {}
         for k, v in _.items():
             if k in fund_money_cloumns:
                 temp_dict[k] = v
         temp_data_json.append(temp_dict)
     temp_df = pd.DataFrame(temp_data_json)
-    temp_df.rename(columns=fund_money_cloumns, inplace=True)
     temp_df.reset_index(inplace=True)
     temp_df["index"] = list(range(1, len(temp_df) + 1))
-    temp_df['日期'] = pd.to_datetime(temp_df['日期']).dt.date
-    temp_df['万份收益'] = pd.to_numeric(temp_df['万份收益'], errors="coerce")
-    temp_df['年化收益率7日'] = pd.to_numeric(temp_df['年化收益率7日'], errors="coerce")
-    temp_df['年化收益率14日'] = pd.to_numeric(temp_df['年化收益率14日'], errors="coerce")
-    temp_df['年化收益率28日'] = pd.to_numeric(temp_df['年化收益率28日'], errors="coerce")
-    temp_df['近1月'] = pd.to_numeric(temp_df['近1月'], errors="coerce")
-    temp_df['近3月'] = pd.to_numeric(temp_df['近3月'], errors="coerce")
-    temp_df['近6月'] = pd.to_numeric(temp_df['近6月'], errors="coerce")
-    temp_df['近1年'] = pd.to_numeric(temp_df['近1年'], errors="coerce")
-    temp_df['近2年'] = pd.to_numeric(temp_df['近2年'], errors="coerce")
-    temp_df['近3年'] = pd.to_numeric(temp_df['近3年'], errors="coerce")
-    temp_df['近5年'] = pd.to_numeric(temp_df['近5年'], errors="coerce")
-    temp_df['今年来'] = pd.to_numeric(temp_df['今年来'], errors="coerce")
-    temp_df['成立来'] = pd.to_numeric(temp_df['成立来'], errors="coerce")
-    return temp_df
+    temp_df.rename(columns=fund_money_cloumns, inplace=True)
+    # temp_df['日期'] = pd.to_datetime(temp_df['日期']).dt.date
+    # temp_df['万份收益'] = pd.to_numeric(temp_df['万份收益'], errors="coerce")
+    # temp_df['年化收益率7日'] = pd.to_numeric(temp_df['年化收益率7日'], errors="coerce")
+    # temp_df['年化收益率14日'] = pd.to_numeric(temp_df['年化收益率14日'], errors="coerce")
+    # temp_df['年化收益率28日'] = pd.to_numeric(temp_df['年化收益率28日'], errors="coerce")
+    # temp_df['近1月'] = pd.to_numeric(temp_df['近1月'], errors="coerce")
+    # temp_df['近3月'] = pd.to_numeric(temp_df['近3月'], errors="coerce")
+    # temp_df['近6月'] = pd.to_numeric(temp_df['近6月'], errors="coerce")
+    # temp_df['近1年'] = pd.to_numeric(temp_df['近1年'], errors="coerce")
+    # temp_df['近2年'] = pd.to_numeric(temp_df['近2年'], errors="coerce")
+    # temp_df['近3年'] = pd.to_numeric(temp_df['近3年'], errors="coerce")
+    # temp_df['近5年'] = pd.to_numeric(temp_df['近5年'], errors="coerce")
+    # temp_df['今年来'] = pd.to_numeric(temp_df['今年来'], errors="coerce")
+    # temp_df['成立来'] = pd.to_numeric(temp_df['成立来'], errors="coerce")
+    return exchange_explain(temp_df, is_explain)
 
 
 @validate_request
-def fund_hk_rank(token: str) -> pd.DataFrame:
+def get_fund_hk_rank(token: str, is_explain: bool = False) -> pd.DataFrame:
     """
     东方财富网-数据中心-香港基金排行
     https://overseas.1234567.com.cn/FundList
     :return: 香港基金排行
     :rtype: pandas.DataFrame
     """
     format_date = datetime.datetime.now().date().isoformat()
@@ -333,22 +335,22 @@
             "近3年",
             "今年来",
             "成立来",
             "可购买",
             "香港基金代码",
         ]
     ]
-    temp_df['日期'] = pd.to_datetime(temp_df['日期']).dt.date
+    # temp_df['日期'] = pd.to_datetime(temp_df['日期']).dt.date
     temp_df['单位净值'] = pd.to_numeric(temp_df['单位净值'], errors="coerce")
     temp_df['日增长率'] = pd.to_numeric(temp_df['日增长率'], errors="coerce")
-    temp_df['近1周'] = pd.to_numeric(temp_df['近1周'], errors="coerce")
-    temp_df['近1月'] = pd.to_numeric(temp_df['近1月'], errors="coerce")
-    temp_df['近3月'] = pd.to_numeric(temp_df['近3月'], errors="coerce")
-    temp_df['近6月'] = pd.to_numeric(temp_df['近6月'], errors="coerce")
-    temp_df['近1年'] = pd.to_numeric(temp_df['近1年'], errors="coerce")
-    temp_df['近2年'] = pd.to_numeric(temp_df['近2年'], errors="coerce")
-    temp_df['近3年'] = pd.to_numeric(temp_df['近3年'], errors="coerce")
-    temp_df['今年来'] = pd.to_numeric(temp_df['今年来'], errors="coerce")
-    temp_df['成立来'] = pd.to_numeric(temp_df['成立来'], errors="coerce")
-    temp_df['成立来'] = pd.to_numeric(temp_df['成立来'], errors="coerce")
+    # temp_df['近1周'] = pd.to_numeric(temp_df['近1周'], errors="coerce")
+    # temp_df['近1月'] = pd.to_numeric(temp_df['近1月'], errors="coerce")
+    # temp_df['近3月'] = pd.to_numeric(temp_df['近3月'], errors="coerce")
+    # temp_df['近6月'] = pd.to_numeric(temp_df['近6月'], errors="coerce")
+    # temp_df['近1年'] = pd.to_numeric(temp_df['近1年'], errors="coerce")
+    # temp_df['近2年'] = pd.to_numeric(temp_df['近2年'], errors="coerce")
+    # temp_df['近3年'] = pd.to_numeric(temp_df['近3年'], errors="coerce")
+    # temp_df['今年来'] = pd.to_numeric(temp_df['今年来'], errors="coerce")
+    # temp_df['成立来'] = pd.to_numeric(temp_df['成立来'], errors="coerce")
+    # temp_df['成立来'] = pd.to_numeric(temp_df['成立来'], errors="coerce")
     temp_df['可购买'] = temp_df['可购买'].map(lambda x: "可购买" if x == "1" else "不可购买")
-    return temp_df
+    return exchange_explain(temp_df, is_explain)
```

### Comparing `sharetop-2.4.5/sharetop/core/fund/get_fund_real_time.py` & `sharetop-2.4.6/sharetop/core/fund/get_fund_real_time.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.5/sharetop/core/fund/get_period_change_info.py` & `sharetop-2.4.6/sharetop/core/fund/get_period_change_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.5/sharetop/core/fund/get_types_percentage_info.py` & `sharetop-2.4.6/sharetop/core/fund/get_types_percentage_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.5/sharetop/core/futures/get_futures_info.py` & `sharetop-2.4.6/sharetop/core/futures/get_futures_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.5/sharetop/core/oil/config.py` & `sharetop-2.4.6/sharetop/core/oil/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.5/sharetop/core/oil/oil_detail.py` & `sharetop-2.4.6/sharetop/core/oil/oil_detail.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.5/sharetop/core/pig/pig_detail.py` & `sharetop-2.4.6/sharetop/core/pig/pig_detail.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.5/sharetop/core/stock/__init__.py` & `sharetop-2.4.6/sharetop/core/stock/__init__.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.5/sharetop/core/stock/bill_monitor.py` & `sharetop-2.4.6/sharetop/core/stock/bill_monitor.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,73 +1,73 @@
 from ..utils import to_numeric, validate_request
 from ..common.getter import get_history_bill as get_history_bill_for_stock
 from ..common.getter import get_real_time_bill_data_one
 import pandas as pd
 
 
-@validate_request
-@to_numeric
-def get_stock_history_capital(token: str, stock_code: str) -> pd.DataFrame:
-    """
-    获取单只股票历史单子流入流出数据
-    Parameters
-    ----------
-    stock_code : str
-        股票代码
-    Returns
-    -------
-    DataFrame
-        沪深市场单只股票历史单子流入流出数据
-    Examples
-    --------
-        股票名称    股票代码          日期         主力净流入       小单净流入         中单净流入         大单净流入        超大单净流入  主力净流入占比  小单流入净占比  中单流入净占比  大单流入净占比  超大单流入净占比      收盘价   涨跌幅
-    0    贵州茅台  600519  2021-03-04 -3.670272e+06  -2282056.0  5.952143e+06  1.461528e+09 -1.465199e+09    -0.03    -0.02     0.04    10.99    -11.02  2013.71 -5.05
-    1    贵州茅台  600519  2021-03-05 -1.514880e+07  -1319066.0  1.646793e+07 -2.528896e+07  1.014016e+07    -0.12    -0.01     0.13    -0.19      0.08  2040.82  1.35
-    2    贵州茅台  600519  2021-03-08 -8.001702e+08   -877074.0  8.010473e+08  5.670671e+08 -1.367237e+09    -6.29    -0.01     6.30     4.46    -10.75  1940.71 -4.91
-    3    贵州茅台  600519  2021-03-09 -2.237770e+08  -6391767.0  2.301686e+08 -1.795013e+08 -4.427571e+07    -1.39    -0.04     1.43    -1.11     -0.27  1917.70 -1.19
-    4    贵州茅台  600519  2021-03-10 -2.044173e+08  -1551798.0  2.059690e+08 -2.378506e+08  3.343331e+07    -2.02    -0.02     2.03    -2.35      0.33  1950.72  1.72
-    ..    ...     ...         ...           ...         ...           ...           ...           ...      ...      ...      ...      ...       ...      ...   ...
-    97   贵州茅台  600519  2021-07-26 -1.564233e+09  13142211.0  1.551091e+09 -1.270400e+08 -1.437193e+09    -8.74     0.07     8.67    -0.71     -8.03  1804.11 -5.05
-    98   贵州茅台  600519  2021-07-27 -7.803296e+08 -10424715.0  7.907544e+08  6.725104e+07 -8.475807e+08    -5.12    -0.07     5.19     0.44     -5.56  1712.89 -5.06
-    99   贵州茅台  600519  2021-07-28  3.997645e+08   2603511.0 -4.023677e+08  2.315648e+08  1.681997e+08     2.70     0.02    -2.72     1.57      1.14  1768.90  3.27
-    100  贵州茅台  600519  2021-07-29 -9.209842e+08  -2312235.0  9.232964e+08 -3.959741e+08 -5.250101e+08    -8.15    -0.02     8.17    -3.50     -4.65  1749.79 -1.08
-    101  贵州茅台  600519  2021-07-30 -1.524740e+09  -6020099.0  1.530761e+09  1.147248e+08 -1.639465e+09   -11.63    -0.05    11.68     0.88    -12.51  1678.99 -4.05
-    :param stock_code:
-    :param token:
-    """
-    df = get_history_bill_for_stock(stock_code)
-    df.rename(columns={'代码': '股票代码', '名称': '股票名称'}, inplace=True)
-    return df
-
-
-@to_numeric
-def get_real_time_bill(stock_code: str) -> pd.DataFrame:
-    """
-    获取单只股票最新交易日的日内分钟级单子流入流出数据
-
-    Parameters
-    ----------
-    stock_code : str
-        股票代码
-
-    Returns
-    -------
-    DataFrame
-        单只股票最新交易日的日内分钟级单子流入流出数据
-
-    Examples
-    --------
-        股票代码                时间        主力净流入      小单净流入        中单净流入        大单净流入       超大单净流入
-    0    600519  2021-07-29 09:31   -3261705.0  -389320.0    3651025.0  -12529658.0    9267953.0
-    1    600519  2021-07-29 09:32    6437999.0  -606994.0   -5831006.0  -42615994.0   49053993.0
-    2    600519  2021-07-29 09:33   13179707.0  -606994.0  -12572715.0  -85059118.0   98238825.0
-    3    600519  2021-07-29 09:34   15385244.0  -970615.0  -14414632.0  -86865209.0  102250453.0
-    4    600519  2021-07-29 09:35    7853716.0  -970615.0   -6883104.0  -75692436.0   83546152.0
-    ..      ...               ...          ...        ...          ...          ...          ...
-    235  600519  2021-07-29 14:56 -918956019.0 -1299630.0  920255661.0 -397127393.0 -521828626.0
-    236  600519  2021-07-29 14:57 -920977761.0 -2319213.0  923296987.0 -397014702.0 -523963059.0
-    237  600519  2021-07-29 14:58 -920984196.0 -2312233.0  923296442.0 -395974137.0 -525010059.0
-    238  600519  2021-07-29 14:59 -920984196.0 -2312233.0  923296442.0 -395974137.0 -525010059.0
-    239  600519  2021-07-29 15:00 -920984196.0 -2312233.0  923296442.0 -395974137.0 -525010059.0
-    """
-    df = get_real_time_bill_data_one(stock_code)
-    return df
+# @validate_request
+# @to_numeric
+# def get_stock_history_capital(token: str, stock_code: str) -> pd.DataFrame:
+#     """
+#     获取单只股票历史单子流入流出数据
+#     Parameters
+#     ----------
+#     stock_code : str
+#         股票代码
+#     Returns
+#     -------
+#     DataFrame
+#         沪深市场单只股票历史单子流入流出数据
+#     Examples
+#     --------
+#         股票名称    股票代码          日期         主力净流入       小单净流入         中单净流入         大单净流入        超大单净流入  主力净流入占比  小单流入净占比  中单流入净占比  大单流入净占比  超大单流入净占比      收盘价   涨跌幅
+#     0    贵州茅台  600519  2021-03-04 -3.670272e+06  -2282056.0  5.952143e+06  1.461528e+09 -1.465199e+09    -0.03    -0.02     0.04    10.99    -11.02  2013.71 -5.05
+#     1    贵州茅台  600519  2021-03-05 -1.514880e+07  -1319066.0  1.646793e+07 -2.528896e+07  1.014016e+07    -0.12    -0.01     0.13    -0.19      0.08  2040.82  1.35
+#     2    贵州茅台  600519  2021-03-08 -8.001702e+08   -877074.0  8.010473e+08  5.670671e+08 -1.367237e+09    -6.29    -0.01     6.30     4.46    -10.75  1940.71 -4.91
+#     3    贵州茅台  600519  2021-03-09 -2.237770e+08  -6391767.0  2.301686e+08 -1.795013e+08 -4.427571e+07    -1.39    -0.04     1.43    -1.11     -0.27  1917.70 -1.19
+#     4    贵州茅台  600519  2021-03-10 -2.044173e+08  -1551798.0  2.059690e+08 -2.378506e+08  3.343331e+07    -2.02    -0.02     2.03    -2.35      0.33  1950.72  1.72
+#     ..    ...     ...         ...           ...         ...           ...           ...           ...      ...      ...      ...      ...       ...      ...   ...
+#     97   贵州茅台  600519  2021-07-26 -1.564233e+09  13142211.0  1.551091e+09 -1.270400e+08 -1.437193e+09    -8.74     0.07     8.67    -0.71     -8.03  1804.11 -5.05
+#     98   贵州茅台  600519  2021-07-27 -7.803296e+08 -10424715.0  7.907544e+08  6.725104e+07 -8.475807e+08    -5.12    -0.07     5.19     0.44     -5.56  1712.89 -5.06
+#     99   贵州茅台  600519  2021-07-28  3.997645e+08   2603511.0 -4.023677e+08  2.315648e+08  1.681997e+08     2.70     0.02    -2.72     1.57      1.14  1768.90  3.27
+#     100  贵州茅台  600519  2021-07-29 -9.209842e+08  -2312235.0  9.232964e+08 -3.959741e+08 -5.250101e+08    -8.15    -0.02     8.17    -3.50     -4.65  1749.79 -1.08
+#     101  贵州茅台  600519  2021-07-30 -1.524740e+09  -6020099.0  1.530761e+09  1.147248e+08 -1.639465e+09   -11.63    -0.05    11.68     0.88    -12.51  1678.99 -4.05
+#     :param stock_code:
+#     :param token:
+#     """
+#     df = get_history_bill_for_stock(stock_code)
+#     df.rename(columns={'代码': '股票代码', '名称': '股票名称'}, inplace=True)
+#     return df
+#
+#
+# @to_numeric
+# def get_real_time_bill(stock_code: str) -> pd.DataFrame:
+#     """
+#     获取单只股票最新交易日的日内分钟级单子流入流出数据
+#
+#     Parameters
+#     ----------
+#     stock_code : str
+#         股票代码
+#
+#     Returns
+#     -------
+#     DataFrame
+#         单只股票最新交易日的日内分钟级单子流入流出数据
+#
+#     Examples
+#     --------
+#         股票代码                时间        主力净流入      小单净流入        中单净流入        大单净流入       超大单净流入
+#     0    600519  2021-07-29 09:31   -3261705.0  -389320.0    3651025.0  -12529658.0    9267953.0
+#     1    600519  2021-07-29 09:32    6437999.0  -606994.0   -5831006.0  -42615994.0   49053993.0
+#     2    600519  2021-07-29 09:33   13179707.0  -606994.0  -12572715.0  -85059118.0   98238825.0
+#     3    600519  2021-07-29 09:34   15385244.0  -970615.0  -14414632.0  -86865209.0  102250453.0
+#     4    600519  2021-07-29 09:35    7853716.0  -970615.0   -6883104.0  -75692436.0   83546152.0
+#     ..      ...               ...          ...        ...          ...          ...          ...
+#     235  600519  2021-07-29 14:56 -918956019.0 -1299630.0  920255661.0 -397127393.0 -521828626.0
+#     236  600519  2021-07-29 14:57 -920977761.0 -2319213.0  923296987.0 -397014702.0 -523963059.0
+#     237  600519  2021-07-29 14:58 -920984196.0 -2312233.0  923296442.0 -395974137.0 -525010059.0
+#     238  600519  2021-07-29 14:59 -920984196.0 -2312233.0  923296442.0 -395974137.0 -525010059.0
+#     239  600519  2021-07-29 15:00 -920984196.0 -2312233.0  923296442.0 -395974137.0 -525010059.0
+#     """
+#     df = get_real_time_bill_data_one(stock_code)
+#     return df
```

### Comparing `sharetop-2.4.5/sharetop/core/stock/getter.py` & `sharetop-2.4.6/sharetop/core/stock/getter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from typing import Dict, List, Union
 import pandas as pd
 from ..common import get_history as get_history_data_for_stock
 from ..common import get_real_time
 from ..common.config import FS_DICT
 from ..common import get_market_realtime_by_fs
 from ..utils import to_numeric, process_dataframe_and_series, validate_request
-from .config import get_stock_market_real_time_data_fields
+from ..common.explain_change import exchange_explain
 
 
 @validate_request
 def get_stock_kline_data(
         token: str,
         stock_codes: Union[str, List[str]],
         beg: str = '19000101',
         end: str = '20500101',
         klt: int = 101,
         fqt: int = 1,
+        is_explain: bool = False,
         **kwargs,
 ) -> Union[pd.DataFrame, Dict[str, pd.DataFrame]]:
     """
     获取股票的 K 线数据
-
     Parameters
     ----------
     stock_codes : Union[str,List[str]]
         股票代码、名称 或者 股票代码、名称构成的列表
     beg : str, optional
         开始日期，默认为 ``'19000101'`` ，表示 1900年1月1日
     end : str, optional
@@ -79,37 +79,45 @@
             4     比亚迪  002594  2011-07-06   31.55   32.15  ...   1.10  0.35  48.90    0    0
             ...   ...     ...         ...     ...     ...  ...    ...   ...    ...  ...  ...
             2846  比亚迪  002594  2023-04-03  256.00  255.92  ...  -0.04 -0.10   1.15    0    0
             2847  比亚迪  002594  2023-04-04  255.81  250.92  ...  -1.95 -5.00   1.18    0    0
             2848  比亚迪  002594  2023-04-06  248.00  250.00  ...  -0.37 -0.92   0.70    0    0
             2849  比亚迪  002594  2023-04-07  250.05  249.28  ...  -0.29 -0.72   0.59    0    0
             2850  比亚迪  002594  2023-04-10  249.28  251.00  ...   0.69  1.72   0.84    0    0
+            :param token:
+            :param fqt:
+            :param klt:
+            :param end:
+            :param beg:
+            :param stock_codes:
+            :param is_explain:
     """
     df = get_history_data_for_stock(
         stock_codes, beg=beg, end=end, klt=klt, fqt=fqt, **kwargs
     )
     if isinstance(df, pd.DataFrame):
         df.rename(columns={'代码': '股票代码', '名称': '股票名称'}, inplace=True)
     elif isinstance(df, dict):
         for stock_code in df.keys():
             df[stock_code].rename(columns={'代码': '股票代码', '名称': '股票名称'}, inplace=True)
-    return df
+    return exchange_explain(df, is_explain)
 
 
 def get_stock_real_time_data(
-        stock_codes: Union[str, List[str]],
+        stock_codes: Union[str, List[str]], is_explain: bool = False
 ) -> Union[pd.DataFrame, Dict[str, pd.DataFrame]]:
     """
     获取单个或者多个股票的实时股价
+    :param is_explain:
     :param stock_codes: 单个或者多个股票代码
     也可以是1.000001 0为深证，1为上证， 116为港股
     :return: 获取单个或者多个股票的实时股价和相关信息
     """
     df = get_real_time(stock_codes)
-    return df
+    return exchange_explain(df, is_explain)
 
 
 @validate_request
 @process_dataframe_and_series(remove_columns_and_indexes=['市场编号'])
 @to_numeric
 def get_stock_market_real_time_data(token: str, fs: Union[str, List[str]] = None, is_explain: bool = False,
                                     **kwargs) -> pd.DataFrame:
@@ -214,11 +222,8 @@
             fs_list.append(FS_DICT[f])
         # 给空列表时 试用沪深A股行情
         if not fs_list:
             fs_list.append(FS_DICT['stock'])
     fs_str = ','.join(fs_list)
     df = get_market_realtime_by_fs(fs_str, **kwargs)
     df.rename(columns={'代码': '股票代码', '名称': '股票名称'}, inplace=True)
-    if not is_explain:
-        df.rename(columns=get_stock_market_real_time_data_fields, inplace=True)
-
-    return df
+    return exchange_explain(df, is_explain)
```

### Comparing `sharetop-2.4.5/sharetop/core/stock/quarterly_report.py` & `sharetop-2.4.6/sharetop/core/stock/quarterly_report.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import rich
 import pandas as pd
 from ..utils import to_numeric, requests_obj, validate_request
 from typing import List, Union
 from jsonpath import jsonpath
 from ...crawl.settings import *
 from ..common.getter import get_company_report
+from ..common.explain_change import exchange_explain
 
 
 @validate_request
-def get_stock_all_report_dates(token: str) -> pd.DataFrame:
+def get_stock_all_report_dates(token: str, is_explain: bool = False) -> pd.DataFrame:
     """
     获取沪深市场的全部股票报告期信息
 
     Returns
     -------
     DataFrame
         沪深市场的全部股票报告期信息
@@ -72,33 +73,37 @@
     response = requests_obj.get(url, params, user_agent=True)
     items = jsonpath(response.json(), '$..data[:]')
     if not items:
         pd.DataFrame(columns=fields.values())
     df = pd.DataFrame(items)
     df = df.rename(columns=fields)
     df['报告日期'] = df['报告日期'].apply(lambda x: x.split()[0])
-    return df
+    return exchange_explain(df, is_explain)
 
 
 @validate_request
 @to_numeric
-def get_stock_company_report_data(token: str, stock_codes: Union[str, List[str]], report_class: str = None) -> pd.DataFrame:
+def get_stock_company_report_data(token: str, stock_codes: Union[str, List[str]], report_class: str = None,
+                                  is_explain: bool = False) -> pd.DataFrame:
     """
     获取单个或者多个上市公司历史年报
+    :param is_explain: 是否需要翻译
     :param token:
     :param stock_codes: 指定的单个公司或者多个公司
     :param report_class: 默认为空是全部，剩余参数可以为：“一季报”，“半年报”，“三季报”，“年报”
     :return:
     """
-    return get_company_report(stock_codes, report_class)
+    return exchange_explain(get_company_report(stock_codes, report_class), is_explain)
+
+
 
 
 @validate_request
 @to_numeric
-def get_stock_all_company_quarterly_report(token: str, date: str = None) -> pd.DataFrame:
+def get_stock_all_company_quarterly_report(token: str, date: str = None, is_explain: bool = False) -> pd.DataFrame:
     """
     获取沪深市场股票某一季度的表现情况
     Parameters
     ----------
     date : str, optional
         报告发布日期 部分可选示例如下(默认为 ``None``)
 
@@ -138,14 +143,17 @@
     4441  002838  道恩股份  2020-04-09 00:00:00  6.191659e+08 -8.019810  -16.5445  6.939886e+07   91.601624  76.7419  0.1700   2.840665    6.20  22.575224  0.186421
     4442  600396  金山股份  2020-04-08 00:00:00  2.023133e+09  0.518504   -3.0629  1.878432e+08  114.304022  61.2733  0.1275   1.511012    8.81  21.422393  0.085698
     4443  002913   奥士康  2020-04-08 00:00:00  4.898977e+08 -3.883035  -23.2268  2.524717e+07  -47.239162 -58.8136  0.1700  16.666749    1.03  22.470020  0.552624
     4444  002007  华兰生物  2020-04-08 00:00:00  6.775414e+08 -2.622289  -36.1714  2.472864e+08   -4.708821 -22.6345  0.1354   4.842456    3.71  61.408522  0.068341
 
     Notes
     -----
+    :param is_explain:
+    :param date:
+    :param token:
 
     """
     # TODO 加速
     fields = {
         'SECURITY_CODE': '股票代码',
         'SECURITY_NAME_ABBR': '股票简称',
         'NOTICE_DATE': '公告日期',
@@ -159,15 +167,15 @@
         'BPS': '每股净资产',
         'WEIGHTAVG_ROE': '净资产收益率',
         'XSMLL': '销售毛利率',
         'MGJYXJJE': '每股经营现金流量'
         # 'ISNEW':'是否最新'
     }
 
-    dates = get_stock_all_report_dates(token)['报告日期'].to_list()
+    dates = get_stock_all_report_dates(token)['report_date'].to_list()
     if date is None:
         date = dates[0]
     if date not in dates:
         rich.print('日期输入有误，可选日期如下:')
         rich.print(dates)
         return pd.DataFrame(columns=fields.values())
 
@@ -184,20 +192,19 @@
             ('sty', 'ALL'),
             ('token', '894050c76af8597a853f5b408b759f5d'),
             # ! 只选沪深A股
             ('filter', f'(SECURITY_TYPE_CODE in ("058001001","058001008")){date}'),
         )
         url = "".join(quarterly_report_url_list)
         response = requests_obj.get(url, params, user_agent=True)
-        # response = session.get(url, headers=EASTMONEY_REQUEST_HEADERS, params=params)
         items = jsonpath(response.json(), '$..data[:]')
         if not items:
             break
         df = pd.DataFrame(items)
         dfs.append(df)
         page += 1
     if len(dfs) == 0:
         df = pd.DataFrame(columns=fields.values())
         return df
     df = pd.concat(dfs, axis=0, ignore_index=True)
     df = df.rename(columns=fields)[fields.values()]
-    return df
+    return exchange_explain(df, is_explain)
```

### Comparing `sharetop-2.4.5/sharetop/core/stock/rank_list.py` & `sharetop-2.4.6/sharetop/core/stock/rank_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 from ..utils import to_numeric, requests_obj, validate_request
 from typing import List
 from jsonpath import jsonpath
 from .config import (
     EASTMONEY_STOCK_DAILY_BILL_BOARD_FIELDS,
 )
 from ...crawl.settings import *
+from ..common.explain_change import exchange_explain
 
 
 @validate_request
 @to_numeric
 @retry(tries=3)
-def get_stock_dragon_tiger_list(token: str, start_date: str = None, end_date: str = None) -> pd.DataFrame:
+def get_stock_dragon_tiger_list(token: str, start_date: str = None, end_date: str = None, is_explain: bool = False) -> pd.DataFrame:
     """
     获取指定日期区间的龙虎榜详情数据
     Parameters
     ----------
     start_date : str, optional
         开始日期
         部分可选示例如下
@@ -131,8 +132,8 @@
             break
     if len(dfs) == 0:
         df = pd.DataFrame(columns=fields.values())
         return df
 
     df = pd.concat(dfs, ignore_index=True)
     df['上榜日期'] = df['上榜日期'].astype('str').apply(lambda x: x.split(' ')[0])
-    return df
+    return exchange_explain(df, is_explain)
```

### Comparing `sharetop-2.4.5/sharetop/core/stock/stock_base_info.py` & `sharetop-2.4.6/sharetop/core/stock/stock_base_info.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import pandas as pd
 from typing import Dict, List, Union
 from ..common.common_base import CommonFunc
+from ..common.explain_change import exchange_explain
+from ..utils import validate_request
 
 common_func_obj = CommonFunc()
 
 
-def get_stock_base_info(stock_codes: Union[str, List[str]],
+def get_stock_base_info(stock_codes: Union[str, List[str]], is_explain: bool = False
 ) -> Union[pd.DataFrame, Dict[str, pd.DataFrame]]:
     """
     获取股票的基本信息
+    :param is_explain:
     :param stock_codes: 一个或者多个股票代码
     :return: 股票的基本信息
     """
     base_func_name = get_stock_base_info.__name__
-    return common_func_obj.get_common_func(stock_codes, base_func_name)
+    return exchange_explain(common_func_obj.get_common_func(stock_codes, base_func_name), is_explain)
```

### Comparing `sharetop-2.4.5/sharetop/core/utils.py` & `sharetop-2.4.6/sharetop/core/utils.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.5/sharetop/crawl/base.py` & `sharetop-2.4.6/sharetop/crawl/base.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.5/sharetop/crawl/settings.py` & `sharetop-2.4.6/sharetop/crawl/settings.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.5/sharetop/parser/base.py` & `sharetop-2.4.6/sharetop/parser/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,17 @@
             use_map = field_map
         else:
             use_map = CAPITAL_FLOW_DICT
         df.rename(columns=use_map, inplace=True)
         return df
 
     def parse_stock_base_info(self, base_data):
+        status = base_data.get("status")
+        if status and status == -1:
+            return pd.DataFrame([base_data])
         jbzl = base_data['jbzl'][0]
         fxxg = base_data['fxxg'][0]
         fxxg = {k.lower(): v for k, v in fxxg.items()}
         jbzl = {k.lower(): v for k, v in jbzl.items()}
         secucode = jbzl['secucode']
         code, mk_code = secucode.split(".")
         name = jbzl['security_name_abbr']
```

### Comparing `sharetop-2.4.5/sharetop/parser/config.py` & `sharetop-2.4.6/sharetop/parser/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
                         "em_industry": '东财行业',
                         "industrycsrc1": '证监会行业',
                         "chairman": '董事长',
                         "legal_person": '法人代表',
                         "president": '总经理',
                         "secretary": '董秘',
                         "secpresent": '证券事务代表',
-                        "reg_capital": '单位：万',
+                        "reg_capital": '注册资本(万)',
                         "found_date": '公司成立日期',
                         "listing_date": '公司上市日期',
                         "province": '所在省份',
                         "city": '所在城市',
                         "introduction": '公司简介',
                         "business_scope": '经营范围',
                         "website": '公司主页',
```

### Comparing `sharetop-2.4.5/sharetop/test/flow_monitor_test.py` & `sharetop-2.4.6/sharetop/test/flow_monitor_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from sharetop.core.capital_flow.capital_flow_monitor import get_stock_real_time_daily_capital, \
     get_stock_real_time_sum_capital, get_stock_real_time_sector_capital, get_stock_history_capital
 
 stock_code = "002714"
 token = "f109298d079b5f60"
 
-# d = get_stock_real_time_daily_capital(stock_code)
 
-d = get_stock_history_capital(token, stock_code)
+# d = get_stock_real_time_daily_capital(stock_code, is_explain=True)
 
-# d = get_stock_real_time_sum_capital([stock_code, '300033'])
+# d = get_stock_history_capital(token, stock_code, is_explain=False)
 
-# d = get_stock_real_time_sector_capital("industry", "1")
+# d = get_stock_real_time_sum_capital(stock_code, is_explain=True)
+
+d = get_stock_real_time_sector_capital("industry", "1", is_explain=True)
 
 print("d====:", d.to_dict("records"))
```

### Comparing `sharetop-2.4.5/sharetop/test/fund_test.py` & `sharetop-2.4.6/sharetop/test/fund_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from sharetop.core.fund.fund_list import get_fund_codes
 from sharetop.core.fund.get_fund_base_info import get_fund_base_info
 from sharetop.core.fund.get_fund_history_data import get_fund_history_price
 from sharetop.core.fund.get_fund_industry_info import get_fund_industry_distribution
 from sharetop.core.fund.get_fund_invest_info import get_fund_public_dates, get_fund_invest_position
-from sharetop.core.fund.get_fund_rank import get_fund_open_rank, get_fund_exchange_rank, get_fund_money_rank, fund_hk_rank
+from sharetop.core.fund.get_fund_rank import get_fund_open_rank, get_fund_exchange_rank, get_fund_money_rank, get_fund_hk_rank
 from sharetop.core.fund.get_period_change_info import get_fund_period_change
 from sharetop.core.fund.get_types_percentage_info import get_fund_types_percentage
 
 token = "f109298d079b5f60"
 
-d = get_fund_base_info(token, "001299")
+# d = get_fund_base_info(token, "001299")
 
-# d = get_fund_history_price(token, "001299")
+d = get_fund_history_price(token, "001299")
 
 # d = get_public_dates(token, "001299")
 
 # d = get_fund_industry_distribution(token, "161725", "2023-03-31")
 
 # d = get_fund_invest_position(token, "161725", "2023-03-31")
 
 # d = get_fund_public_dates(token, "161725")
 
 # d = fund_open_fund_rank(token, "债券型")
 
-# d = get_fund_open_rank(token)
+# d = get_fund_open_rank(token, is_explain=True)
 
 # d = get_fund_exchange_rank(token)
 
 # d = get_fund_money_rank(token)
 
 # d = get_fund_period_change(token, "161725")
 
@@ -35,10 +35,12 @@
 
 # d = fund_money_rank(token)
 
 # d = get_period_change(token, "001299")
 
 # d = get_types_percentage(token, "001299")
 
-# d = get_fund_codes(token)
+# d = get_fund_codes(token, is_explain=True)
 
-print(d)
+# d = get_fund_hk_rank(token, is_explain=False)
+
+print(d.to_dict("records"))
```

### Comparing `sharetop-2.4.5/sharetop/test/stock_test.py` & `sharetop-2.4.6/sharetop/test/stock_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,34 @@
-from sharetop.core.stock.bill_monitor import get_stock_history_capital, get_real_time_bill
 
 from sharetop.core.stock.getter import get_stock_kline_data, get_stock_real_time_data, get_stock_market_real_time_data
 from sharetop.core.stock.quarterly_report import get_stock_all_report_dates, get_stock_company_report_data, get_stock_all_company_quarterly_report
 from sharetop.core.stock.rank_list import get_stock_dragon_tiger_list
 
 from sharetop.core.stock.stock_base_info import get_stock_base_info
 
-
 token = "f109298d079b5f60"
 
-# d = get_stock_history_capital(token, "002714")
 
-# d = get_stock_kline_data(token, ["002714", "300033"])
+# d = get_stock_kline_data(token, ["002714", "516110"], is_explain=True)
 
 # d = get_real_time_bill("002714")
 
 # d = get_history_data(token, "002714", klt=102)
 
 # d = get_real_time_data(["002714", "516110"])
 
 # d = get_stock_market_real_time_data(token, is_explain=True)
 
-# d = get_stock_company_report_data(token, '002714', "一季报")
-
-# d = get_stock_all_company_quarterly_report(token, '2021-03-31')
-
-# d = get_stock_dragon_tiger_list(token)
+# d = get_stock_company_report_data(token, '002714', "一季报", False)
 
-# d = get_stock_base_info("002714")
+# d = get_stock_all_company_quarterly_report(token, '2021-03-31', True)
 
-# d = get_stock_all_report_dates(token)
+d = get_stock_dragon_tiger_list(token, is_explain=True)
 
-# d = get_stock_real_time_data("002714")
+# d = get_stock_base_info(["002714", "562510"])
+# d = get_stock_base_info(["002714", "600809"], is_explain=True)
 
-# print(d.to_dict("records"))
+# d = get_stock_all_report_dates(token, is_explain=True)
 
-from sharetop.core.stock import get_stock_market_real_time_data
+# d = get_stock_real_time_data("002714", is_explain=False)
 
-df = get_stock_market_real_time_data(token)
-print(df)
+print(d.to_dict("records"))
```

### Comparing `sharetop-2.4.5/sharetop/test/test1.py` & `sharetop-2.4.6/sharetop/test/test1.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.5/sharetop/test/test2-akshare.py` & `sharetop-2.4.6/sharetop/test/test2-akshare.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.5/sharetop/test/test3.py` & `sharetop-2.4.6/sharetop/test/test3.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.5/sharetop/test/test5.py` & `sharetop-2.4.6/sharetop/test/test5.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.5/sharetop/test/test6.py` & `sharetop-2.4.6/sharetop/test/test6.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.5/sharetop/test/test7.py` & `sharetop-2.4.6/sharetop/test/test7.py`

 * *Files identical despite different names*

### Comparing `sharetop-2.4.5/sharetop.egg-info/PKG-INFO` & `sharetop-2.4.6/sharetop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharetop
-Version: 2.4.5
+Version: 2.4.6
 Summary: Provide data related to the economic market
 Home-page: https://github.com/nrliangxy/sharetop
 Author: nrliangxy
 Author-email: nrliangxy@foxmail.com
 License: MIT
 Project-URL: Source, https://github.com/nrliangxy/sharetop
 Keywords: data,finance,quant,stock,fund,futures,share
```

### Comparing `sharetop-2.4.5/sharetop.egg-info/SOURCES.txt` & `sharetop-2.4.6/sharetop.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 sharetop/core/bond/get_bond_info.py
 sharetop/core/bond/get_bond_public_info.py
 sharetop/core/capital_flow/__init__.py
 sharetop/core/capital_flow/capital_flow_monitor.py
 sharetop/core/common/__init__.py
 sharetop/core/common/common_base.py
 sharetop/core/common/config.py
+sharetop/core/common/explain_change.py
 sharetop/core/common/getter.py
 sharetop/core/country/__init__.py
 sharetop/core/country/config.py
 sharetop/core/country/country_base_info.py
 sharetop/core/fund/__init__.py
 sharetop/core/fund/config.py
 sharetop/core/fund/fund_list.py
```

