# Comparing `tmp/trytond_account_invoice_stock-6.8.0.tar.gz` & `tmp/trytond_account_invoice_stock-6.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_account_invoice_stock-6.8.0.tar", last modified: Mon May  1 11:42:07 2023, max compression
+gzip compressed data, was "trytond_account_invoice_stock-6.8.1.tar", last modified: Mon Jul 31 17:11:37 2023, max compression
```

## Comparing `trytond_account_invoice_stock-6.8.0.tar` & `trytond_account_invoice_stock-6.8.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:07.689471 trytond_account_invoice_stock-6.8.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     2461 2023-05-01 11:01:33.000000 trytond_account_invoice_stock-6.8.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-05-01 11:01:33.000000 trytond_account_invoice_stock-6.8.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_account_invoice_stock-6.8.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-6.8.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2609 2023-05-01 11:42:07.686138 trytond_account_invoice_stock-6.8.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-6.8.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      436 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-6.8.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5162 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-6.8.0/account.py
--rw-r--r--   0 ced       (1000) ced       (1000)      494 2023-01-16 14:00:20.000000 trytond_account_invoice_stock-6.8.0/account.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:07.686138 trytond_account_invoice_stock-6.8.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-6.8.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-6.8.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-6.8.0/doc/releases.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:07.682804 trytond_account_invoice_stock-6.8.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     1302 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1320 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1060 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1309 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1317 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1071 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1152 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1257 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1060 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1298 2023-04-30 10:46:36.000000 trytond_account_invoice_stock-6.8.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1236 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1159 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1291 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1270 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1253 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1277 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1060 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1217 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1255 2023-04-30 10:46:36.000000 trytond_account_invoice_stock-6.8.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1321 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1183 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1060 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1060 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1060 2023-04-29 08:02:40.000000 trytond_account_invoice_stock-6.8.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:42:07.689471 trytond_account_invoice_stock-6.8.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4593 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-6.8.0/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4448 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-6.8.0/stock.py
--rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-01-16 14:00:20.000000 trytond_account_invoice_stock-6.8.0/stock.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:07.682804 trytond_account_invoice_stock-6.8.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-6.8.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4004 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-6.8.0/tests/scenario_account_invoice_stock.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3792 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-6.8.0/tests/scenario_account_invoice_stock_correction.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-6.8.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-6.8.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-6.8.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      116 2023-05-01 11:01:27.000000 trytond_account_invoice_stock-6.8.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:07.686138 trytond_account_invoice_stock-6.8.0/trytond_account_invoice_stock.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2609 2023-05-01 11:42:06.000000 trytond_account_invoice_stock-6.8.0/trytond_account_invoice_stock.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1726 2023-05-01 11:42:07.000000 trytond_account_invoice_stock-6.8.0/trytond_account_invoice_stock.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:42:06.000000 trytond_account_invoice_stock-6.8.0/trytond_account_invoice_stock.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       80 2023-05-01 11:42:06.000000 trytond_account_invoice_stock-6.8.0/trytond_account_invoice_stock.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:39:58.000000 trytond_account_invoice_stock-6.8.0/trytond_account_invoice_stock.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      128 2023-05-01 11:42:06.000000 trytond_account_invoice_stock-6.8.0/trytond_account_invoice_stock.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:42:06.000000 trytond_account_invoice_stock-6.8.0/trytond_account_invoice_stock.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:42:07.682804 trytond_account_invoice_stock-6.8.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      530 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-6.8.0/view/invoice_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-04-15 07:12:15.000000 trytond_account_invoice_stock-6.8.0/view/move_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 17:11:37.714757 trytond_account_invoice_stock-6.8.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2562 2023-07-31 17:11:34.000000 trytond_account_invoice_stock-6.8.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      687 2023-07-31 17:11:34.000000 trytond_account_invoice_stock-6.8.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2609 2023-07-31 17:11:37.714757 trytond_account_invoice_stock-6.8.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      436 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5162 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/account.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      494 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/account.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 17:11:37.711423 trytond_account_invoice_stock-6.8.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/doc/releases.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 17:11:37.708090 trytond_account_invoice_stock-6.8.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1302 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1320 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1060 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1309 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1317 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1071 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1152 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1257 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1060 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1298 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1236 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1159 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1291 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1270 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1253 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1277 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1060 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1217 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1255 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1321 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1183 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1060 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1060 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1060 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-07-31 17:11:37.714757 trytond_account_invoice_stock-6.8.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4593 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4433 2023-07-10 21:28:50.000000 trytond_account_invoice_stock-6.8.1/stock.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/stock.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 17:11:37.711423 trytond_account_invoice_stock-6.8.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4004 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/tests/scenario_account_invoice_stock.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3792 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/tests/scenario_account_invoice_stock_correction.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      347 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      116 2023-05-01 12:18:02.000000 trytond_account_invoice_stock-6.8.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 17:11:37.714757 trytond_account_invoice_stock-6.8.1/trytond_account_invoice_stock.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2609 2023-07-31 17:11:37.000000 trytond_account_invoice_stock-6.8.1/trytond_account_invoice_stock.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1726 2023-07-31 17:11:37.000000 trytond_account_invoice_stock-6.8.1/trytond_account_invoice_stock.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-07-31 17:11:37.000000 trytond_account_invoice_stock-6.8.1/trytond_account_invoice_stock.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       80 2023-07-31 17:11:37.000000 trytond_account_invoice_stock-6.8.1/trytond_account_invoice_stock.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-31 12:36:17.000000 trytond_account_invoice_stock-6.8.1/trytond_account_invoice_stock.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      128 2023-07-31 17:11:37.000000 trytond_account_invoice_stock-6.8.1/trytond_account_invoice_stock.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-07-31 17:11:37.000000 trytond_account_invoice_stock-6.8.1/trytond_account_invoice_stock.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 17:11:37.711423 trytond_account_invoice_stock-6.8.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      530 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/view/invoice_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-05-01 12:17:30.000000 trytond_account_invoice_stock-6.8.1/view/move_form.xml
```

### Comparing `trytond_account_invoice_stock-6.8.0/CHANGELOG` & `trytond_account_invoice_stock-6.8.1/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 
+Version 6.8.1 - 2023-07-31
+--------------------------
+* Bug fixes (see mercurial logs for details)
+
+
 Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Remove support for Python 3.7
 * Add support for Python 3.11
 
 Version 6.6.0 - 2022-10-31
```

### Comparing `trytond_account_invoice_stock-6.8.0/COPYRIGHT` & `trytond_account_invoice_stock-6.8.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.8.0/LICENSE` & `trytond_account_invoice_stock-6.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.8.0/PKG-INFO` & `trytond_account_invoice_stock-6.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_account_invoice_stock
-Version: 6.8.0
+Version: 6.8.1
 Summary: Tryton module to link stock and invoice
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_invoice_stock-6.8.0/account.py` & `trytond_account_invoice_stock-6.8.1/account.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.8.0/doc/conf.py` & `trytond_account_invoice_stock-6.8.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.8.0/locale/bg.po` & `trytond_account_invoice_stock-6.8.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.8.0/locale/ca.po` & `trytond_account_invoice_stock-6.8.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.8.0/locale/cs.po` & `trytond_account_invoice_stock-6.8.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.8.0/locale/de.po` & `trytond_account_invoice_stock-6.8.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.8.0/locale/es.po` & `trytond_account_invoice_stock-6.8.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.8.0/locale/es_419.po` & `trytond_account_invoice_stock-6.8.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.8.0/locale/et.po` & `trytond_account_invoice_stock-6.8.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.8.0/locale/fa.po` & `trytond_account_invoice_stock-6.8.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.8.0/locale/fi.po` & `trytond_account_invoice_stock-6.8.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.8.0/locale/fr.po` & `trytond_account_invoice_stock-6.8.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.8.0/locale/hu.po` & `trytond_account_invoice_stock-6.8.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.8.0/locale/id.po` & `trytond_account_invoice_stock-6.8.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.8.0/locale/it.po` & `trytond_account_invoice_stock-6.8.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.8.0/locale/lo.po` & `trytond_account_invoice_stock-6.8.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.8.0/locale/lt.po` & `trytond_account_invoice_stock-6.8.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.8.0/locale/nl.po` & `trytond_account_invoice_stock-6.8.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.8.0/locale/pl.po` & `trytond_account_invoice_stock-6.8.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.8.0/locale/pt.po` & `trytond_account_invoice_stock-6.8.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.8.0/locale/ro.po` & `trytond_account_invoice_stock-6.8.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.8.0/locale/ru.po` & `trytond_account_invoice_stock-6.8.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.8.0/locale/sl.po` & `trytond_account_invoice_stock-6.8.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.8.0/locale/tr.po` & `trytond_account_invoice_stock-6.8.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.8.0/locale/uk.po` & `trytond_account_invoice_stock-6.8.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.8.0/locale/zh_CN.po` & `trytond_account_invoice_stock-6.8.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.8.0/setup.py` & `trytond_account_invoice_stock-6.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.8.0/stock.py` & `trytond_account_invoice_stock-6.8.1/stock.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         super().__setup__()
         cls._allow_modify_closed_period.add('invoice_lines')
 
     @classmethod
     def get_invoice_types(cls):
         pool = Pool()
         Invoice = pool.get('account.invoice')
-        return Invoice.fields_get(['type'])['type']['selection'] + [(None, '')]
+        return Invoice.fields_get(['type'])['type']['selection']
 
     @fields.depends('from_location', 'to_location')
     def on_change_with_invoice_types(self, name=None):
         types = set()
         for location in [self.from_location, self.to_location]:
             if location:
                 if location.type == 'customer':
```

### Comparing `trytond_account_invoice_stock-6.8.0/tests/scenario_account_invoice_stock.rst` & `trytond_account_invoice_stock-6.8.1/tests/scenario_account_invoice_stock.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.8.0/tests/scenario_account_invoice_stock_correction.rst` & `trytond_account_invoice_stock-6.8.1/tests/scenario_account_invoice_stock_correction.rst`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.8.0/tox.ini` & `trytond_account_invoice_stock-6.8.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.8.0/trytond_account_invoice_stock.egg-info/PKG-INFO` & `trytond_account_invoice_stock-6.8.1/trytond_account_invoice_stock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond-account-invoice-stock
-Version: 6.8.0
+Version: 6.8.1
 Summary: Tryton module to link stock and invoice
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_account_invoice_stock-6.8.0/trytond_account_invoice_stock.egg-info/SOURCES.txt` & `trytond_account_invoice_stock-6.8.1/trytond_account_invoice_stock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_account_invoice_stock-6.8.0/view/invoice_line_form.xml` & `trytond_account_invoice_stock-6.8.1/view/invoice_line_form.xml`

 * *Files identical despite different names*

