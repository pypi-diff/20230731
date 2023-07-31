# Comparing `tmp/trytond_party-6.8.0.tar.gz` & `tmp/trytond_party-6.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_party-6.8.0.tar", last modified: Mon May  1 11:35:48 2023, max compression
+gzip compressed data, was "trytond_party-6.8.1.tar", last modified: Mon Jul 31 17:12:09 2023, max compression
```

## Comparing `trytond_party-6.8.0.tar` & `trytond_party-6.8.1.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:48.048093 trytond_party-6.8.0/
--rw-r--r--   0 ced       (1000) ced       (1000)     5736 2023-05-01 10:57:18.000000 trytond_party-6.8.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      884 2023-05-01 10:57:18.000000 trytond_party-6.8.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:20.000000 trytond_party-6.8.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_party-6.8.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2621 2023-05-01 11:35:48.048093 trytond_party-6.8.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-04-15 07:12:15.000000 trytond_party-6.8.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1062 2023-04-15 07:12:15.000000 trytond_party-6.8.0/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    16613 2023-04-15 07:12:15.000000 trytond_party-6.8.0/address.py
--rw-r--r--   0 ced       (1000) ced       (1000)    25257 2023-04-15 07:12:15.000000 trytond_party-6.8.0/address.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1449 2023-04-15 07:12:15.000000 trytond_party-6.8.0/category.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3658 2023-04-15 07:12:15.000000 trytond_party-6.8.0/category.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4573 2023-04-15 07:12:15.000000 trytond_party-6.8.0/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2497 2023-04-15 07:12:15.000000 trytond_party-6.8.0/configuration.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    12269 2023-04-29 22:04:03.000000 trytond_party-6.8.0/contact_mechanism.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2097 2023-04-15 07:12:15.000000 trytond_party-6.8.0/contact_mechanism.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-04-15 07:12:15.000000 trytond_party-6.8.0/country.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:48.044760 trytond_party-6.8.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_party-6.8.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6349 2023-04-15 07:12:15.000000 trytond_party-6.8.0/doc/design.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-04-15 07:12:15.000000 trytond_party-6.8.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_party-6.8.0/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4129 2023-04-15 07:12:15.000000 trytond_party-6.8.0/doc/usage.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      551 2023-04-29 22:04:03.000000 trytond_party-6.8.0/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:48.044760 trytond_party-6.8.0/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_party-6.8.0/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      259 2023-01-16 14:00:20.000000 trytond_party-6.8.0/icons/tryton-party.svg
--rw-r--r--   0 ced       (1000) ced       (1000)     3841 2023-04-15 07:12:15.000000 trytond_party-6.8.0/ir.py
--rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-04-15 07:12:15.000000 trytond_party-6.8.0/ir.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    31778 2023-01-16 14:00:20.000000 trytond_party-6.8.0/label.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:48.038093 trytond_party-6.8.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    32339 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38662 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    30984 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    40303 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    39063 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    30787 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    36147 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35855 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    30769 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38585 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33391 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    31510 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33799 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    35167 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37051 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    38370 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37264 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33790 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37727 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    32852 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    33577 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    30769 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    45703 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    37550 2023-04-30 10:46:36.000000 trytond_party-6.8.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     3058 2023-04-29 22:04:03.000000 trytond_party-6.8.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    37925 2023-04-21 08:36:08.000000 trytond_party-6.8.0/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8099 2023-04-15 07:12:15.000000 trytond_party-6.8.0/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:35:48.048093 trytond_party-6.8.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4597 2023-04-15 07:12:15.000000 trytond_party-6.8.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:48.041427 trytond_party-6.8.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      227 2023-04-15 07:12:15.000000 trytond_party-6.8.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1638 2023-04-15 07:12:15.000000 trytond_party-6.8.0/tests/scenario_party_erase.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      868 2023-04-15 07:12:15.000000 trytond_party-6.8.0/tests/scenario_party_identifier_notifications.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1109 2023-04-15 07:12:15.000000 trytond_party-6.8.0/tests/scenario_party_phone_number.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1381 2023-04-15 07:12:15.000000 trytond_party-6.8.0/tests/scenario_party_replace.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    16012 2023-04-15 07:12:15.000000 trytond_party-6.8.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_party-6.8.0/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_party-6.8.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      186 2023-05-01 10:57:12.000000 trytond_party-6.8.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:48.048093 trytond_party-6.8.0/trytond_party.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2621 2023-05-01 11:35:47.000000 trytond_party-6.8.0/trytond_party.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     3475 2023-05-01 11:35:47.000000 trytond_party-6.8.0/trytond_party.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:35:47.000000 trytond_party-6.8.0/trytond_party.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       48 2023-05-01 11:35:47.000000 trytond_party-6.8.0/trytond_party.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-02-14 15:56:20.000000 trytond_party-6.8.0/trytond_party.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      176 2023-05-01 11:35:47.000000 trytond_party-6.8.0/trytond_party.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:35:47.000000 trytond_party-6.8.0/trytond_party.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:35:48.044760 trytond_party-6.8.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)     1556 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/address_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      999 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/address_form_simple.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/address_format_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      104 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/address_format_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/address_subdivision_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      256 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/address_subdivision_type_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      498 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/address_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/address_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-01-16 14:00:20.000000 trytond_party-6.8.0/view/category_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-01-16 14:00:20.000000 trytond_party-6.8.0/view/category_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      239 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/category_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      265 2023-01-16 14:00:20.000000 trytond_party-6.8.0/view/check_vies_result.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      412 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1195 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/contact_mechanism_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      460 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/contact_mechanism_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      530 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/contact_mechanism_tree_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/email_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-01-16 14:00:20.000000 trytond_party-6.8.0/view/erase_ask_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      599 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/identifier_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/identifier_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/identifier_list_sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1581 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-04-15 07:12:15.000000 trytond_party-6.8.0/view/party_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      190 2023-01-16 14:00:20.000000 trytond_party-6.8.0/view/replace_ask_form.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 17:12:09.111679 trytond_party-6.8.1/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5837 2023-07-31 17:12:05.000000 trytond_party-6.8.1/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      884 2023-07-31 17:12:05.000000 trytond_party-6.8.1/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-05-01 12:17:31.000000 trytond_party-6.8.1/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-05-01 12:17:31.000000 trytond_party-6.8.1/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2621 2023-07-31 17:12:09.111679 trytond_party-6.8.1/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-05-01 12:17:31.000000 trytond_party-6.8.1/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1062 2023-05-01 12:17:31.000000 trytond_party-6.8.1/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    16749 2023-07-10 21:28:50.000000 trytond_party-6.8.1/address.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    25257 2023-05-01 12:17:31.000000 trytond_party-6.8.1/address.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1449 2023-05-01 12:17:31.000000 trytond_party-6.8.1/category.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3658 2023-05-01 12:17:31.000000 trytond_party-6.8.1/category.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4573 2023-05-01 12:17:31.000000 trytond_party-6.8.1/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2497 2023-05-01 12:17:31.000000 trytond_party-6.8.1/configuration.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    12269 2023-05-01 12:17:31.000000 trytond_party-6.8.1/contact_mechanism.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2097 2023-05-01 12:17:31.000000 trytond_party-6.8.1/contact_mechanism.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      658 2023-05-01 12:17:31.000000 trytond_party-6.8.1/country.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 17:12:09.108346 trytond_party-6.8.1/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-05-01 12:17:31.000000 trytond_party-6.8.1/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6349 2023-05-01 12:17:31.000000 trytond_party-6.8.1/doc/design.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      361 2023-05-01 12:17:31.000000 trytond_party-6.8.1/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-05-01 12:17:31.000000 trytond_party-6.8.1/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4129 2023-05-01 12:17:31.000000 trytond_party-6.8.1/doc/usage.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      551 2023-05-01 12:17:31.000000 trytond_party-6.8.1/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 17:12:09.111679 trytond_party-6.8.1/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-05-01 12:17:31.000000 trytond_party-6.8.1/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      259 2023-05-01 12:17:31.000000 trytond_party-6.8.1/icons/tryton-party.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)     3841 2023-05-01 12:17:31.000000 trytond_party-6.8.1/ir.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      484 2023-05-01 12:17:31.000000 trytond_party-6.8.1/ir.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    31778 2023-05-01 12:17:31.000000 trytond_party-6.8.1/label.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 17:12:09.098346 trytond_party-6.8.1/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    32339 2023-05-01 12:17:31.000000 trytond_party-6.8.1/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38662 2023-05-01 12:17:31.000000 trytond_party-6.8.1/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    30984 2023-05-01 12:17:31.000000 trytond_party-6.8.1/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    40303 2023-05-01 12:17:31.000000 trytond_party-6.8.1/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    39063 2023-05-01 12:17:31.000000 trytond_party-6.8.1/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    30787 2023-05-01 12:17:31.000000 trytond_party-6.8.1/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    36147 2023-05-01 12:17:31.000000 trytond_party-6.8.1/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35855 2023-05-01 12:17:31.000000 trytond_party-6.8.1/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    30769 2023-05-01 12:17:31.000000 trytond_party-6.8.1/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38585 2023-05-01 12:17:31.000000 trytond_party-6.8.1/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33391 2023-05-01 12:17:31.000000 trytond_party-6.8.1/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    31510 2023-05-01 12:17:31.000000 trytond_party-6.8.1/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33799 2023-05-01 12:17:31.000000 trytond_party-6.8.1/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    35167 2023-05-01 12:17:31.000000 trytond_party-6.8.1/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37051 2023-05-01 12:17:31.000000 trytond_party-6.8.1/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    38370 2023-05-01 12:17:31.000000 trytond_party-6.8.1/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37264 2023-05-01 12:17:31.000000 trytond_party-6.8.1/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33790 2023-05-01 12:17:31.000000 trytond_party-6.8.1/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37727 2023-05-01 12:17:31.000000 trytond_party-6.8.1/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    32852 2023-05-01 12:17:31.000000 trytond_party-6.8.1/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    33577 2023-05-01 12:17:31.000000 trytond_party-6.8.1/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    30769 2023-05-01 12:17:31.000000 trytond_party-6.8.1/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    45703 2023-05-01 12:17:31.000000 trytond_party-6.8.1/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    37550 2023-05-01 12:17:31.000000 trytond_party-6.8.1/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     3058 2023-05-01 12:17:31.000000 trytond_party-6.8.1/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    37925 2023-05-01 12:17:31.000000 trytond_party-6.8.1/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8099 2023-05-01 12:17:31.000000 trytond_party-6.8.1/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-07-31 17:12:09.111679 trytond_party-6.8.1/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4597 2023-05-01 12:17:31.000000 trytond_party-6.8.1/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 17:12:09.101679 trytond_party-6.8.1/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      227 2023-05-01 12:17:31.000000 trytond_party-6.8.1/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1638 2023-05-01 12:17:31.000000 trytond_party-6.8.1/tests/scenario_party_erase.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      868 2023-05-01 12:17:31.000000 trytond_party-6.8.1/tests/scenario_party_identifier_notifications.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1109 2023-05-01 12:17:31.000000 trytond_party-6.8.1/tests/scenario_party_phone_number.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1381 2023-05-01 12:17:31.000000 trytond_party-6.8.1/tests/scenario_party_replace.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    16012 2023-05-01 12:17:31.000000 trytond_party-6.8.1/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-05-01 12:17:31.000000 trytond_party-6.8.1/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-05-01 12:17:31.000000 trytond_party-6.8.1/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      186 2023-05-01 12:18:02.000000 trytond_party-6.8.1/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 17:12:09.111679 trytond_party-6.8.1/trytond_party.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2621 2023-07-31 17:12:08.000000 trytond_party-6.8.1/trytond_party.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     3475 2023-07-31 17:12:09.000000 trytond_party-6.8.1/trytond_party.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-07-31 17:12:08.000000 trytond_party-6.8.1/trytond_party.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       48 2023-07-31 17:12:08.000000 trytond_party-6.8.1/trytond_party.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-31 12:36:15.000000 trytond_party-6.8.1/trytond_party.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      176 2023-07-31 17:12:08.000000 trytond_party-6.8.1/trytond_party.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-07-31 17:12:08.000000 trytond_party-6.8.1/trytond_party.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 17:12:09.108346 trytond_party-6.8.1/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1556 2023-05-01 12:17:31.000000 trytond_party-6.8.1/view/address_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      999 2023-05-01 12:17:31.000000 trytond_party-6.8.1/view/address_form_simple.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      317 2023-05-01 12:17:31.000000 trytond_party-6.8.1/view/address_format_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      104 2023-05-01 12:17:31.000000 trytond_party-6.8.1/view/address_format_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      386 2023-05-01 12:17:31.000000 trytond_party-6.8.1/view/address_subdivision_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      256 2023-05-01 12:17:31.000000 trytond_party-6.8.1/view/address_subdivision_type_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      498 2023-05-01 12:17:31.000000 trytond_party-6.8.1/view/address_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      518 2023-05-01 12:17:31.000000 trytond_party-6.8.1/view/address_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      383 2023-05-01 12:17:31.000000 trytond_party-6.8.1/view/category_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      226 2023-05-01 12:17:31.000000 trytond_party-6.8.1/view/category_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      239 2023-05-01 12:17:31.000000 trytond_party-6.8.1/view/category_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      265 2023-05-01 12:17:31.000000 trytond_party-6.8.1/view/check_vies_result.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      412 2023-05-01 12:17:31.000000 trytond_party-6.8.1/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1195 2023-05-01 12:17:31.000000 trytond_party-6.8.1/view/contact_mechanism_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      460 2023-05-01 12:17:31.000000 trytond_party-6.8.1/view/contact_mechanism_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      530 2023-05-01 12:17:31.000000 trytond_party-6.8.1/view/contact_mechanism_tree_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      366 2023-05-01 12:17:31.000000 trytond_party-6.8.1/view/email_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-05-01 12:17:31.000000 trytond_party-6.8.1/view/erase_ask_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      599 2023-05-01 12:17:31.000000 trytond_party-6.8.1/view/identifier_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      334 2023-05-01 12:17:31.000000 trytond_party-6.8.1/view/identifier_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-05-01 12:17:31.000000 trytond_party-6.8.1/view/identifier_list_sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1581 2023-05-01 12:17:31.000000 trytond_party-6.8.1/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      333 2023-05-01 12:17:31.000000 trytond_party-6.8.1/view/party_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      190 2023-05-01 12:17:31.000000 trytond_party-6.8.1/view/replace_ask_form.xml
```

### Comparing `trytond_party-6.8.0/CHANGELOG` & `trytond_party-6.8.1/CHANGELOG`

 * *Files 2% similar despite different names*

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
 * Notify for duplicate identifier
```

### Comparing `trytond_party-6.8.0/COPYRIGHT` & `trytond_party-6.8.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/LICENSE` & `trytond_party-6.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/PKG-INFO` & `trytond_party-6.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond_party
-Version: 6.8.0
+Version: 6.8.1
 Summary: Tryton module with parties and addresses
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_party-6.8.0/__init__.py` & `trytond_party-6.8.1/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/address.py` & `trytond_party-6.8.1/address.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,15 +261,16 @@
                 and self.subdivision.country != self.country):
             self.subdivision = None
 
     @classmethod
     def get_subdivision_types(cls):
         pool = Pool()
         Subdivision = pool.get('country.subdivision')
-        return Subdivision.fields_get(['type'])['type']['selection']
+        selection = Subdivision.fields_get(['type'])['type']['selection']
+        return [(k, v) for k, v in selection if k is not None]
 
     @fields.depends('country')
     def on_change_with_subdivision_types(self, name=None):
         pool = Pool()
         Types = pool.get('party.address.subdivision_type')
         return Types.get_types(self.country)
 
@@ -433,15 +434,16 @@
             ]
         cls._order.insert(0, ('country_code', 'ASC NULLS LAST'))
 
     @classmethod
     def get_subdivision_types(cls):
         pool = Pool()
         Subdivision = pool.get('country.subdivision')
-        return Subdivision.fields_get(['type'])['type']['selection']
+        selection = Subdivision.fields_get(['type'])['type']['selection']
+        return [(k, v) for k, v in selection if k is not None]
 
     @classmethod
     def create(cls, *args, **kwargs):
         records = super().create(*args, **kwargs)
         cls._get_types_cache.clear()
         return records
```

### Comparing `trytond_party-6.8.0/address.xml` & `trytond_party-6.8.1/address.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/category.py` & `trytond_party-6.8.1/category.py`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/category.xml` & `trytond_party-6.8.1/category.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/configuration.py` & `trytond_party-6.8.1/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/configuration.xml` & `trytond_party-6.8.1/configuration.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/contact_mechanism.py` & `trytond_party-6.8.1/contact_mechanism.py`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/contact_mechanism.xml` & `trytond_party-6.8.1/contact_mechanism.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/country.py` & `trytond_party-6.8.1/country.py`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/doc/conf.py` & `trytond_party-6.8.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/doc/design.rst` & `trytond_party-6.8.1/doc/design.rst`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/doc/usage.rst` & `trytond_party-6.8.1/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/exceptions.py` & `trytond_party-6.8.1/exceptions.py`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/icons/LICENSE` & `trytond_party-6.8.1/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/ir.py` & `trytond_party-6.8.1/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/label.fodt` & `trytond_party-6.8.1/label.fodt`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/locale/bg.po` & `trytond_party-6.8.1/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/locale/ca.po` & `trytond_party-6.8.1/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/locale/cs.po` & `trytond_party-6.8.1/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/locale/de.po` & `trytond_party-6.8.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/locale/es.po` & `trytond_party-6.8.1/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/locale/es_419.po` & `trytond_party-6.8.1/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/locale/et.po` & `trytond_party-6.8.1/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/locale/fa.po` & `trytond_party-6.8.1/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/locale/fi.po` & `trytond_party-6.8.1/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/locale/fr.po` & `trytond_party-6.8.1/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/locale/hu.po` & `trytond_party-6.8.1/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/locale/id.po` & `trytond_party-6.8.1/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/locale/it.po` & `trytond_party-6.8.1/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/locale/lo.po` & `trytond_party-6.8.1/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/locale/lt.po` & `trytond_party-6.8.1/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/locale/nl.po` & `trytond_party-6.8.1/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/locale/pl.po` & `trytond_party-6.8.1/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/locale/pt.po` & `trytond_party-6.8.1/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/locale/ro.po` & `trytond_party-6.8.1/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/locale/ru.po` & `trytond_party-6.8.1/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/locale/sl.po` & `trytond_party-6.8.1/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/locale/tr.po` & `trytond_party-6.8.1/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/locale/uk.po` & `trytond_party-6.8.1/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/locale/zh_CN.po` & `trytond_party-6.8.1/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/message.xml` & `trytond_party-6.8.1/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/party.py` & `trytond_party-6.8.1/party.py`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/party.xml` & `trytond_party-6.8.1/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/setup.py` & `trytond_party-6.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/tests/scenario_party_erase.rst` & `trytond_party-6.8.1/tests/scenario_party_erase.rst`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/tests/scenario_party_identifier_notifications.rst` & `trytond_party-6.8.1/tests/scenario_party_identifier_notifications.rst`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/tests/scenario_party_phone_number.rst` & `trytond_party-6.8.1/tests/scenario_party_phone_number.rst`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/tests/scenario_party_replace.rst` & `trytond_party-6.8.1/tests/scenario_party_replace.rst`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/tests/test_module.py` & `trytond_party-6.8.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/tox.ini` & `trytond_party-6.8.1/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/trytond_party.egg-info/PKG-INFO` & `trytond_party-6.8.1/trytond_party.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond-party
-Version: 6.8.0
+Version: 6.8.1
 Summary: Tryton module with parties and addresses
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond_party-6.8.0/trytond_party.egg-info/SOURCES.txt` & `trytond_party-6.8.1/trytond_party.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/view/address_form.xml` & `trytond_party-6.8.1/view/address_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/view/address_form_simple.xml` & `trytond_party-6.8.1/view/address_form_simple.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/view/address_tree_sequence.xml` & `trytond_party-6.8.1/view/address_tree_sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/view/contact_mechanism_form.xml` & `trytond_party-6.8.1/view/contact_mechanism_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/view/contact_mechanism_tree_sequence.xml` & `trytond_party-6.8.1/view/contact_mechanism_tree_sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/view/identifier_form.xml` & `trytond_party-6.8.1/view/identifier_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_party-6.8.0/view/party_form.xml` & `trytond_party-6.8.1/view/party_form.xml`

 * *Files identical despite different names*

