# Comparing `tmp/drb-2.1.4.tar.gz` & `tmp/drb-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-2.1.4.tar", last modified: Wed May  3 12:14:31 2023, max compression
+gzip compressed data, was "drb-2.1.5.tar", last modified: Mon Jul 31 10:05:44 2023, max compression
```

## Comparing `drb-2.1.4.tar` & `drb-2.1.5.tar`

### file list

```diff
@@ -1,88 +1,90 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:14:31.099683 drb-2.1.4/
--rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-23 09:38:20.000000 drb-2.1.4/LICENCE.txt
--rw-rw-rw-   0 root         (0) root         (0)       51 2022-11-29 12:51:50.000000 drb-2.1.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    10378 2023-05-03 12:14:31.099683 drb-2.1.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    10007 2022-01-31 14:39:35.000000 drb-2.1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:14:30.911680 drb-2.1.4/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:14:31.103684 drb-2.1.4/drb/core/
--rw-rw-rw-   0 root         (0) root         (0)      440 2022-11-29 12:51:50.000000 drb-2.1.4/drb/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-05-03 12:14:31.103684 drb-2.1.4/drb/core/_version.py
--rw-rw-rw-   0 root         (0) root         (0)      426 2023-01-23 09:38:20.000000 drb-2.1.4/drb/core/cortex_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     1154 2022-11-29 12:51:50.000000 drb-2.1.4/drb/core/events.py
--rw-rw-rw-   0 root         (0) root         (0)     3831 2023-03-08 16:35:51.000000 drb-2.1.4/drb/core/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     2783 2023-03-08 16:35:51.000000 drb-2.1.4/drb/core/item.py
--rw-rw-rw-   0 root         (0) root         (0)    14860 2023-03-23 12:42:47.000000 drb-2.1.4/drb/core/node.py
--rw-rw-rw-   0 root         (0) root         (0)     9956 2023-03-08 16:35:51.000000 drb-2.1.4/drb/core/path.py
--rw-rw-rw-   0 root         (0) root         (0)     1411 2022-11-29 12:51:50.000000 drb-2.1.4/drb/core/predicate.py
--rw-rw-rw-   0 root         (0) root         (0)     3674 2022-11-29 12:51:50.000000 drb-2.1.4/drb/core/signature.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:14:30.907680 drb-2.1.4/drb/drivers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:14:30.935681 drb-2.1.4/drb/drivers/file/
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-03-08 16:35:51.000000 drb-2.1.4/drb/drivers/file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4467 2023-05-02 15:56:43.000000 drb-2.1.4/drb/drivers/file/file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:14:30.939681 drb-2.1.4/drb/drivers/xml/
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-01-23 09:38:20.000000 drb-2.1.4/drb/drivers/xml/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1073 2023-01-23 09:38:20.000000 drb-2.1.4/drb/drivers/xml/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     7022 2023-05-02 15:56:44.000000 drb-2.1.4/drb/drivers/xml/node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:14:30.939681 drb-2.1.4/drb/exceptions/
--rw-rw-rw-   0 root         (0) root         (0)      301 2023-01-23 09:38:20.000000 drb-2.1.4/drb/exceptions/core.py
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-01-23 09:38:20.000000 drb-2.1.4/drb/exceptions/file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:14:30.911680 drb-2.1.4/drb/keyring/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:14:30.943681 drb-2.1.4/drb/keyring/bitwarden/
--rw-rw-rw-   0 root         (0) root         (0)      152 2023-01-23 09:38:20.000000 drb-2.1.4/drb/keyring/bitwarden/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4897 2023-03-02 15:39:38.000000 drb-2.1.4/drb/keyring/bitwarden/bitwarden.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:14:30.947681 drb-2.1.4/drb/nodes/
--rw-rw-rw-   0 root         (0) root         (0)     7255 2023-03-15 13:58:12.000000 drb-2.1.4/drb/nodes/abstract_node.py
--rw-rw-rw-   0 root         (0) root         (0)     8125 2023-03-08 16:35:51.000000 drb-2.1.4/drb/nodes/logical_node.py
--rw-rw-rw-   0 root         (0) root         (0)    13171 2023-03-15 13:58:12.000000 drb-2.1.4/drb/nodes/mutable_node.py
--rw-rw-rw-   0 root         (0) root         (0)     3277 2023-03-08 16:35:51.000000 drb-2.1.4/drb/nodes/url_node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:14:30.947681 drb-2.1.4/drb/signatures/
--rw-rw-rw-   0 root         (0) root         (0)     6868 2022-11-29 12:51:50.000000 drb-2.1.4/drb/signatures/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:14:30.951681 drb-2.1.4/drb/topics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:14:30.963681 drb-2.1.4/drb/topics/dao/
--rw-rw-rw-   0 root         (0) root         (0)      193 2023-01-23 09:38:20.000000 drb-2.1.4/drb/topics/dao/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6624 2023-01-23 09:38:20.000000 drb-2.1.4/drb/topics/dao/manager_dao.py
--rw-rw-rw-   0 root         (0) root         (0)      866 2023-01-23 09:38:20.000000 drb-2.1.4/drb/topics/dao/topic_dao.py
--rw-rw-rw-   0 root         (0) root         (0)     2143 2023-01-23 09:38:20.000000 drb-2.1.4/drb/topics/dao/topic_schema.yml
--rw-rw-rw-   0 root         (0) root         (0)     5214 2023-01-23 09:38:20.000000 drb-2.1.4/drb/topics/dao/xml_dao.py
--rw-rw-rw-   0 root         (0) root         (0)     8789 2023-01-23 09:38:20.000000 drb-2.1.4/drb/topics/dao/yaml_dao.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:14:30.963681 drb-2.1.4/drb/topics/file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-23 09:38:20.000000 drb-2.1.4/drb/topics/file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      208 2023-05-03 12:13:36.000000 drb-2.1.4/drb/topics/file/cortex.yml
--rw-rw-rw-   0 root         (0) root         (0)    13635 2023-03-17 13:56:33.000000 drb-2.1.4/drb/topics/resolver.py
--rw-rw-rw-   0 root         (0) root         (0)     1368 2023-01-23 09:38:20.000000 drb-2.1.4/drb/topics/topic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:14:30.963681 drb-2.1.4/drb/topics/xml/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-23 09:38:20.000000 drb-2.1.4/drb/topics/xml/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-05-03 12:13:36.000000 drb-2.1.4/drb/topics/xml/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:14:30.967681 drb-2.1.4/drb/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-12-14 10:20:32.000000 drb-2.1.4/drb/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1078 2022-11-29 12:51:50.000000 drb-2.1.4/drb/utils/drb_python_script.py
--rw-rw-rw-   0 root         (0) root         (0)      630 2022-11-29 12:51:50.000000 drb-2.1.4/drb/utils/plugins.py
--rw-rw-rw-   0 root         (0) root         (0)     1045 2023-03-08 16:35:51.000000 drb-2.1.4/drb/utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:14:30.923681 drb-2.1.4/drb.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10378 2023-05-03 12:14:30.000000 drb-2.1.4/drb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1625 2023-05-03 12:14:30.000000 drb-2.1.4/drb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 12:14:30.000000 drb-2.1.4/drb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      517 2023-05-03 12:14:30.000000 drb-2.1.4/drb.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 12:14:30.000000 drb-2.1.4/drb.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      142 2023-05-03 12:14:30.000000 drb-2.1.4/drb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-03 12:14:30.000000 drb-2.1.4/drb.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-03-08 16:35:52.000000 drb-2.1.4/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      142 2023-03-08 16:35:52.000000 drb-2.1.4/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1423 2023-05-03 12:14:31.103684 drb-2.1.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-03-08 16:35:52.000000 drb-2.1.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:14:31.099683 drb-2.1.4/tests/
--rw-rw-rw-   0 root         (0) root         (0)    12469 2023-03-23 12:42:47.000000 drb-2.1.4/tests/test_abstract_node.py
--rw-rw-rw-   0 root         (0) root         (0)     3544 2022-11-29 12:51:50.000000 drb-2.1.4/tests/test_drb_node_list.py
--rw-rw-rw-   0 root         (0) root         (0)     1468 2022-11-29 12:51:50.000000 drb-2.1.4/tests/test_event.py
--rw-rw-rw-   0 root         (0) root         (0)     2114 2023-01-23 09:38:21.000000 drb-2.1.4/tests/test_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     6925 2023-01-23 09:38:21.000000 drb-2.1.4/tests/test_factory_resolver.py
--rw-rw-rw-   0 root         (0) root         (0)     6874 2023-01-23 09:38:21.000000 drb-2.1.4/tests/test_keyring_bitwarden.py
--rw-rw-rw-   0 root         (0) root         (0)    23074 2022-11-29 12:51:50.000000 drb-2.1.4/tests/test_logical_node.py
--rw-rw-rw-   0 root         (0) root         (0)     5213 2023-01-23 09:38:21.000000 drb-2.1.4/tests/test_manager_dao.py
--rw-rw-rw-   0 root         (0) root         (0)    15747 2023-03-02 15:39:38.000000 drb-2.1.4/tests/test_path.py
--rw-rw-rw-   0 root         (0) root         (0)     6697 2022-11-29 12:51:50.000000 drb-2.1.4/tests/test_signatures.py
--rw-rw-rw-   0 root         (0) root         (0)     1729 2023-01-23 09:38:21.000000 drb-2.1.4/tests/test_topic.py
--rw-rw-rw-   0 root         (0) root         (0)     3993 2023-03-02 15:39:38.000000 drb-2.1.4/tests/test_url_node.py
--rw-rw-rw-   0 root         (0) root         (0)     1855 2023-01-23 09:38:21.000000 drb-2.1.4/tests/test_xml_dao.py
--rw-rw-rw-   0 root         (0) root         (0)     3102 2023-01-23 09:38:21.000000 drb-2.1.4/tests/test_yaml_dao.py
--rw-rw-rw-   0 root         (0) root         (0)    70144 2022-10-19 07:59:20.000000 drb-2.1.4/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:05:44.539329 drb-2.1.5/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-07-31 10:05:22.000000 drb-2.1.5/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-07-31 10:05:22.000000 drb-2.1.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    10378 2023-07-31 10:05:44.539329 drb-2.1.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    10007 2023-07-31 10:05:22.000000 drb-2.1.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:05:44.519329 drb-2.1.5/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:05:44.527329 drb-2.1.5/drb/core/
+-rw-rw-rw-   0 root         (0) root         (0)      440 2023-07-31 10:05:22.000000 drb-2.1.5/drb/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2023-07-31 10:05:44.539329 drb-2.1.5/drb/core/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      426 2023-07-31 10:05:22.000000 drb-2.1.5/drb/core/cortex_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-07-31 10:05:22.000000 drb-2.1.5/drb/core/events.py
+-rw-rw-rw-   0 root         (0) root         (0)     3831 2023-07-31 10:05:22.000000 drb-2.1.5/drb/core/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     2783 2023-07-31 10:05:22.000000 drb-2.1.5/drb/core/item.py
+-rw-rw-rw-   0 root         (0) root         (0)    15344 2023-07-31 10:05:22.000000 drb-2.1.5/drb/core/node.py
+-rw-rw-rw-   0 root         (0) root         (0)     9956 2023-07-31 10:05:22.000000 drb-2.1.5/drb/core/path.py
+-rw-rw-rw-   0 root         (0) root         (0)     1411 2023-07-31 10:05:22.000000 drb-2.1.5/drb/core/predicate.py
+-rw-rw-rw-   0 root         (0) root         (0)     3676 2023-07-31 10:05:22.000000 drb-2.1.5/drb/core/signature.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:05:44.519329 drb-2.1.5/drb/drivers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:05:44.527329 drb-2.1.5/drb/drivers/file/
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-31 10:05:22.000000 drb-2.1.5/drb/drivers/file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5544 2023-07-31 10:05:22.000000 drb-2.1.5/drb/drivers/file/file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:05:44.527329 drb-2.1.5/drb/drivers/xml/
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-07-31 10:05:22.000000 drb-2.1.5/drb/drivers/xml/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2023-07-31 10:05:22.000000 drb-2.1.5/drb/drivers/xml/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     7022 2023-07-31 10:05:22.000000 drb-2.1.5/drb/drivers/xml/node.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:05:44.527329 drb-2.1.5/drb/exceptions/
+-rw-rw-rw-   0 root         (0) root         (0)      301 2023-07-31 10:05:22.000000 drb-2.1.5/drb/exceptions/core.py
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-07-31 10:05:22.000000 drb-2.1.5/drb/exceptions/file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:05:44.519329 drb-2.1.5/drb/keyring/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:05:44.527329 drb-2.1.5/drb/keyring/bitwarden/
+-rw-rw-rw-   0 root         (0) root         (0)      152 2023-07-31 10:05:22.000000 drb-2.1.5/drb/keyring/bitwarden/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4897 2023-07-31 10:05:22.000000 drb-2.1.5/drb/keyring/bitwarden/bitwarden.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:05:44.531329 drb-2.1.5/drb/nodes/
+-rw-rw-rw-   0 root         (0) root         (0)     7255 2023-07-31 10:05:22.000000 drb-2.1.5/drb/nodes/abstract_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     8125 2023-07-31 10:05:22.000000 drb-2.1.5/drb/nodes/logical_node.py
+-rw-rw-rw-   0 root         (0) root         (0)    13171 2023-07-31 10:05:22.000000 drb-2.1.5/drb/nodes/mutable_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     3277 2023-07-31 10:05:22.000000 drb-2.1.5/drb/nodes/url_node.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:05:44.531329 drb-2.1.5/drb/signatures/
+-rw-rw-rw-   0 root         (0) root         (0)     6868 2023-07-31 10:05:22.000000 drb-2.1.5/drb/signatures/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:05:44.531329 drb-2.1.5/drb/topics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:05:44.531329 drb-2.1.5/drb/topics/dao/
+-rw-rw-rw-   0 root         (0) root         (0)      193 2023-07-31 10:05:22.000000 drb-2.1.5/drb/topics/dao/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7381 2023-07-31 10:05:22.000000 drb-2.1.5/drb/topics/dao/manager_dao.py
+-rw-rw-rw-   0 root         (0) root         (0)     6488 2023-07-31 10:05:22.000000 drb-2.1.5/drb/topics/dao/rdf_dao.py
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-07-31 10:05:22.000000 drb-2.1.5/drb/topics/dao/topic_dao.py
+-rw-rw-rw-   0 root         (0) root         (0)     2143 2023-07-31 10:05:22.000000 drb-2.1.5/drb/topics/dao/topic_schema.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5571 2023-07-31 10:05:22.000000 drb-2.1.5/drb/topics/dao/xml_dao.py
+-rw-rw-rw-   0 root         (0) root         (0)     8833 2023-07-31 10:05:22.000000 drb-2.1.5/drb/topics/dao/yaml_dao.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:05:44.531329 drb-2.1.5/drb/topics/file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-31 10:05:22.000000 drb-2.1.5/drb/topics/file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      208 2023-07-31 10:05:22.000000 drb-2.1.5/drb/topics/file/cortex.yml
+-rw-rw-rw-   0 root         (0) root         (0)    12884 2023-07-31 10:05:22.000000 drb-2.1.5/drb/topics/resolver.py
+-rw-rw-rw-   0 root         (0) root         (0)     1806 2023-07-31 10:05:22.000000 drb-2.1.5/drb/topics/topic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:05:44.531329 drb-2.1.5/drb/topics/xml/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-31 10:05:22.000000 drb-2.1.5/drb/topics/xml/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-07-31 10:05:22.000000 drb-2.1.5/drb/topics/xml/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:05:44.535329 drb-2.1.5/drb/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-31 10:05:22.000000 drb-2.1.5/drb/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2023-07-31 10:05:22.000000 drb-2.1.5/drb/utils/drb_python_script.py
+-rw-rw-rw-   0 root         (0) root         (0)      630 2023-07-31 10:05:22.000000 drb-2.1.5/drb/utils/plugins.py
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2023-07-31 10:05:22.000000 drb-2.1.5/drb/utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:05:44.523329 drb-2.1.5/drb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10378 2023-07-31 10:05:44.000000 drb-2.1.5/drb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1673 2023-07-31 10:05:44.000000 drb-2.1.5/drb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 10:05:44.000000 drb-2.1.5/drb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      517 2023-07-31 10:05:44.000000 drb-2.1.5/drb.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 10:05:44.000000 drb-2.1.5/drb.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      174 2023-07-31 10:05:44.000000 drb-2.1.5/drb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-31 10:05:44.000000 drb-2.1.5/drb.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-31 10:05:22.000000 drb-2.1.5/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-07-31 10:05:22.000000 drb-2.1.5/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1423 2023-07-31 10:05:44.539329 drb-2.1.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-07-31 10:05:22.000000 drb-2.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 10:05:44.539329 drb-2.1.5/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    12469 2023-07-31 10:05:22.000000 drb-2.1.5/tests/test_abstract_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     3544 2023-07-31 10:05:22.000000 drb-2.1.5/tests/test_drb_node_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     1468 2023-07-31 10:05:22.000000 drb-2.1.5/tests/test_event.py
+-rw-rw-rw-   0 root         (0) root         (0)     2044 2023-07-31 10:05:22.000000 drb-2.1.5/tests/test_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     6862 2023-07-31 10:05:22.000000 drb-2.1.5/tests/test_factory_resolver.py
+-rw-rw-rw-   0 root         (0) root         (0)     6874 2023-07-31 10:05:22.000000 drb-2.1.5/tests/test_keyring_bitwarden.py
+-rw-rw-rw-   0 root         (0) root         (0)    23074 2023-07-31 10:05:22.000000 drb-2.1.5/tests/test_logical_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     5243 2023-07-31 10:05:22.000000 drb-2.1.5/tests/test_manager_dao.py
+-rw-rw-rw-   0 root         (0) root         (0)    15747 2023-07-31 10:05:22.000000 drb-2.1.5/tests/test_path.py
+-rw-rw-rw-   0 root         (0) root         (0)     2251 2023-07-31 10:05:22.000000 drb-2.1.5/tests/test_rdf_dao.py
+-rw-rw-rw-   0 root         (0) root         (0)     6697 2023-07-31 10:05:22.000000 drb-2.1.5/tests/test_signatures.py
+-rw-rw-rw-   0 root         (0) root         (0)     1614 2023-07-31 10:05:22.000000 drb-2.1.5/tests/test_topic.py
+-rw-rw-rw-   0 root         (0) root         (0)     3993 2023-07-31 10:05:22.000000 drb-2.1.5/tests/test_url_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     2123 2023-07-31 10:05:22.000000 drb-2.1.5/tests/test_xml_dao.py
+-rw-rw-rw-   0 root         (0) root         (0)     3138 2023-07-31 10:05:22.000000 drb-2.1.5/tests/test_yaml_dao.py
+-rw-rw-rw-   0 root         (0) root         (0)    70144 2023-07-31 10:05:22.000000 drb-2.1.5/versioneer.py
```

### Comparing `drb-2.1.4/LICENCE.txt` & `drb-2.1.5/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `drb-2.1.4/PKG-INFO` & `drb-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drb
-Version: 2.1.4
+Version: 2.1.5
 Summary: Data Request Broker
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
```

### Comparing `drb-2.1.4/README.md` & `drb-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `drb-2.1.4/drb/core/events.py` & `drb-2.1.5/drb/core/events.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.4/drb/core/factory.py` & `drb-2.1.5/drb/core/factory.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.4/drb/core/item.py` & `drb-2.1.5/drb/core/item.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.4/drb/core/node.py` & `drb-2.1.5/drb/core/node.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,39 +41,51 @@
     def __matmul__(self, other):
         """
         Returns a specific attribute requested in argument,
         this argument can be a str the name of the attribute,
         or a tuple representing the name and namespace of the
         attribute.
 
-        the usage:
-            node @ name -> retrieve the attribute
-            node @ (name, namespace) -> retrieve the attribute
-
         Returns:
             Any: The value of the attribute
+
+        Example:
+
+        .. code-block:: python
+
+            # equivalent to `node @ (name, None)`
+            attribute_value = node @ name
+            attribute_value = node @ (name, namespace)
         """
         try:
             key = get_name_namespace_index(other)
             return self._attrs[(key[0], key[1])]
         except (IndexError, TypeError, KeyError) as error:
             raise DrbException(f'No attribute {other} found') from error
 
     def __imatmul__(self, other):
         """
         Allow to add, update or delete an attributes.
 
         the usage:
-            node @= (name, value) -> add/update the attribute
-            node @= (name, namespace, value) -> add/update the attribute
-            node @ (name, None) -> delete the attribute
-            node @ (name, namespace, None) -> delete the attribute
+
 
         Returns:
-            DrbNode: The node requested
+            DrbNode: returns this node
+
+        Example:
+
+        .. code-block:: python
+
+            # add or update an attribute
+            node @= (name, namespace, value)
+            node @= (name, value)
+            # delete an attribute
+            node @= (name, namespace, None)
+            node @= (name, None)
         """
         name, namespace, value = get_name_namespace_value(other)
         if value is None:
             del self._attrs[(name, namespace)]
         else:
             self._attrs[(name, namespace)] = value
         return self
@@ -296,15 +308,15 @@
         * ``tuple``: the following tuple must be supported per each node
           implementation:
 
             * (name: ``str``, namespace: ``str``): delete first child by is
               name and namespace_uri.
 
         Raises:
-            DrbException: if no child is found, except for ```` case
+            DrbException: if no child is found, except for ``Predicate`` case
                           where an empty may return.
         Examples:
 
         .. code-block:: python
 
             # Delete an existing children
             del node['name']
@@ -323,18 +335,18 @@
             bool: ``True`` if current node has a child following name and
             namespace criteria, otherwise ``False``
         """
         raise NotImplementedError
 
     def impl_capabilities(self) -> List[type]:
         """
-        List all the possible interface the node can provide.
+        List all the possible interfaces the node can provide.
 
         Returns:
-            List[type]: A list of all interface possible
+            List[type]: A list of all possible interfaces
         """
         return self._available_impl.copy()
 
     def has_impl(self, impl: type) -> bool:
         """
         Tests if a specific interface can be provided. These operation tests
         with a minimum of time and memory consumption if the current
@@ -415,14 +427,29 @@
             raise ValueError('Only a value boolean is expected here !')
         self.__namespace_aware = value
 
     def __hash__(self):
         return hash(self.path.name)
 
     def __contains__(self, item) -> bool:
+        """
+        Allows to use the ``in`` keyword on a node, in order to check child
+        existence.
+
+        Returns:
+            bool: True if the node have the expected child, otherwise False
+
+        Example:
+
+        .. code-block:: python
+
+            # equivalent to `(name, None) in node`
+            'name' in node
+            ('name', 'namespace') in node
+        """
         if isinstance(item, str):
             return self.has_child(item)
         if isinstance(item, tuple) and len(item) == 2:
             return self.has_child(*item)
         return False
 
     def __eq__(self, other):
```

### Comparing `drb-2.1.4/drb/core/path.py` & `drb-2.1.5/drb/core/path.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.4/drb/core/predicate.py` & `drb-2.1.5/drb/core/predicate.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.4/drb/core/signature.py` & `drb-2.1.5/drb/core/signature.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,18 @@
     Item (ItemClass). This recognition mechanism is applied on a DRB Node.
     """
 
     @abc.abstractmethod
     def matches(self, node: DrbNode) -> bool:
         """
         Allowing to check if the given node match the signature.
+
         Parameters:
             node (DrbNode): item to check
+
         Returns:
             bool - ``True`` if the given node match, otherwise ``False``
         """
         raise NotImplementedError
 
     @abc.abstractmethod
     def to_dict(self) -> dict:
```

### Comparing `drb-2.1.4/drb/drivers/file/file.py` & `drb-2.1.5/drb/drivers/file/file.py`

 * *Files 22% similar despite different names*

```diff
@@ -37,23 +37,39 @@
     return io.FileIO(path, 'r+')
 
 
 def impl_buffered_stream(path: str) -> io.BufferedReader:
     return io.BufferedReader(impl_stream(path))
 
 
+def _retrieve_file_mode(st_mode) -> str:
+    if stat.S_ISREG(st_mode):
+        return 'REGULAR'
+    if stat.S_ISDIR(st_mode):
+        return 'DIRECTORY'
+    if stat.S_ISLNK(st_mode):
+        return 'LINK'
+    if stat.S_ISSOCK(st_mode):
+        return 'SOCKET'
+    if stat.S_ISFIFO(st_mode):
+        return 'FIFO'
+    if stat.S_ISBLK(st_mode):
+        return 'BLOCK'
+    if stat.S_ISCHR(st_mode):
+        return 'CHAR'
+    return 'UNKNOWN'
+
+
 class DrbFileNode(AbstractNode):
     """
     Parameters:
         path (Union[str, ParsedPath]): The path of the file
                                        to read with this node.
         parent (DrbNode): The parent of this node (default: None)
     """
-    __attributes = [
-        'directory', 'size', 'modified', 'readable', 'writable', 'hidden']
 
     def __init__(self, path, parent: DrbNode = None):
         super().__init__()
         if isinstance(path, ParsedPath):
             self._path = path
         else:
             if platform.uname()[0] == 'Windows':
@@ -67,26 +83,24 @@
 
     @property
     def path(self) -> ParsedPath:
         return self._path
 
     def __init_attr(self):
         file_stat = os.stat(self.path.path)
-
-        self @= (self.__attributes[0], os.path.isdir(self.path.path))
-
-        self @= (self.__attributes[1], file_stat.st_size)
-
-        self @= (self.__attributes[2], file_stat.st_mtime)
-
-        self @= (self.__attributes[3], os.access(self.path.path, os.R_OK))
-
-        self @= (self.__attributes[4], os.access(self.path.path, os.W_OK))
-
-        self @= (self.__attributes[5], is_hidden(self.path.path))
+        self @= ('size', file_stat.st_size)
+        self @= ('mode', _retrieve_file_mode(file_stat.st_mode))
+        self @= ('creation_time', file_stat.st_ctime)
+        self @= ('last_modification_time', file_stat.st_mtime)
+        self @= ('last_access_time', file_stat.st_atime)
+        self @= ('owner', file_stat.st_uid)
+        self @= ('group', file_stat.st_gid)
+        self @= ('link_number', file_stat.st_nlink)
+        self @= ('inode', file_stat.st_ino)
+        self @= ('hidden', is_hidden(self.path.path))
 
     @property
     @resolver.resolve_children
     @deprecated(version='2.1.0', reason='Only bracket browse should be use')
     def children(self) -> List[DrbNode]:
         if self._children is None:
             self._children = []
@@ -118,17 +132,33 @@
 
 class DrbFileFactory(DrbFactory):
 
     @staticmethod
     def _create_from_uri_of_node(node: DrbNode):
         uri = node.path.name
         parsed_uri = urlparse(uri)
-        if (platform.uname()[0] == "Windows"
-                and re.match(r"^/[a-zA-Z]:", parsed_uri.path)):
-            path = parsed_uri.path[:1].replace('%20', ' ')
+        if (platform.uname()[0] == "Windows"):
+
+            # not sure this code is executed
+            # on windows plateform the urlparse split the drive letter
+            # into parsed_uri.scheme.
+            # parsed_uri has no drive letter
+            if re.match(r"^/[a-zA-Z]:", parsed_uri.path):
+                path = parsed_uri.path[:1].replace('%20', ' ')
+
+            # PYDRB 547
+            # test if it is a local file by testing if
+            # its existence. This is the only way found to check whether
+            # the uri is a local path or an url
+            # if it is a loal path, simply keep the full uri
+            if pathlib.Path(uri).exists():
+                path = uri
+            else:
+                path = parsed_uri.path
+
         else:
             path = parsed_uri.path
         if os.path.exists(path):
             return DrbFileNode(path, node)
         raise DrbFileNodeFactoryException(f'File not found: {path}')
 
     def _create(self, node: DrbNode) -> DrbNode:
```

### Comparing `drb-2.1.4/drb/drivers/xml/factory.py` & `drb-2.1.5/drb/drivers/xml/factory.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.4/drb/drivers/xml/node.py` & `drb-2.1.5/drb/drivers/xml/node.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.4/drb/keyring/bitwarden/bitwarden.py` & `drb-2.1.5/drb/keyring/bitwarden/bitwarden.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.4/drb/nodes/abstract_node.py` & `drb-2.1.5/drb/nodes/abstract_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
             named_children = [x for x in self.children if x.name == name]
         if len(named_children) <= 0:
             raise DrbException(f'No child found having name: {name} and'
                                f' namespace: {namespace_uri}')
         return named_children[occurrence]
 
     def __eq__(self, other):
-        if type(other) == type(self):
+        if type(other) is type(self):
             return self.name == other.name and \
                    self.namespace_uri == other.namespace_uri and \
                    self.value == other.value
         else:
             return False
 
     def has_child(self, name: str = None, namespace: str = None) -> bool:
```

### Comparing `drb-2.1.4/drb/nodes/logical_node.py` & `drb-2.1.5/drb/nodes/logical_node.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.4/drb/nodes/mutable_node.py` & `drb-2.1.5/drb/nodes/mutable_node.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.4/drb/nodes/url_node.py` & `drb-2.1.5/drb/nodes/url_node.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.4/drb/signatures/core.py` & `drb-2.1.5/drb/signatures/core.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.4/drb/topics/dao/manager_dao.py` & `drb-2.1.5/drb/topics/dao/manager_dao.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 import logging
 import importlib
 import drb.utils.plugins
 from jsonschema.exceptions import ValidationError
 
 from .topic_dao import DrbTopicDao
 from .yaml_dao import YamlDao
-from drb.topics.topic import DrbTopic
+from .rdf_dao import RDFDao
+from drb.topics.topic import DrbTopic, TopicCategory
 from drb.exceptions.core import DrbException, DaoException
 
 
 logger = logging.getLogger('DrbTopic')
 
 
 def _load_all_drb_topic_dao() -> Dict[uuid.UUID, DrbTopicDao]:
@@ -63,15 +64,17 @@
     __instance = None
     __known_dao = None
 
     def __new__(cls, *args, **kwargs):
         if cls.__instance is None:
             cls.__instance = super(DaoFactory, cls).__new__(cls)
             from .xml_dao import XmlDao
-            cls.__known_dao = {'.yml': YamlDao, '.owl': XmlDao}
+            cls.__known_dao = {'.yml': YamlDao,
+                               '.owl': RDFDao,
+                               '.ttl': RDFDao}
         return cls.__instance
 
     def create(self, path: str) -> DrbTopicDao:
         ext = splitext(path)[1]
         try:
             dao = self.__known_dao[ext]
             return dao(path)
@@ -81,35 +84,53 @@
 
 class ManagerDao:
     """
     Manages loading and retrieving of topics defined in the Python
     context.
     """
     __instance = None
+    __topic_dao = None
     __added_dao = []
 
     def __new__(cls, *args, **kwargs):
         if cls.__instance is None:
             cls.__instance = super(ManagerDao, cls).__new__(cls)
             cls.__topic_dao = _load_all_drb_topic_dao()
+            cls.__topics = []
+            cls.__update_topics(cls.__instance)
 
         return cls.__instance
 
+    def __update_topics(self):
+        self.__topics = []
+        for identifier in self.__topic_dao.keys():
+            topic = self.__topic_dao[identifier].read(identifier)
+            self.__topics.append(topic)
+
     def get_all_drb_topics(self) -> Iterable[DrbTopic]:
         """
         Returns all loaded topics.
         Returns:
             Iterable: An iterable containing all loaded topics.
         """
-        topics = []
+        return self.__topics
 
-        for identifier in self.__topic_dao.keys():
-            topic = self.__topic_dao[identifier].read(identifier)
-            topics.append(topic)
+    def get_overridden_drb_topics(self) -> Iterable[DrbTopic]:
+        topics = []
+        for ic in self.__topics:
+            if ic.override:
+                topics.append(ic)
+        return topics
 
+    def get_drb_topics_by_category(
+            self, category: TopicCategory) -> Iterable[DrbTopic]:
+        topics = []
+        for ic in self.__topics:
+            if category == ic.category:
+                topics.append(ic)
         return topics
 
     def get_drb_topic(self, identifier: uuid.UUID) -> DrbTopic:
         """
         Retrieves a topic.
         Parameters:
             identifier (UUID): topic UUID
@@ -215,9 +236,10 @@
                 """
 
         dao = DaoFactory().create(path)
         self.__added_dao.append(dao)
         topics = dao.read_all()
         for topic in topics:
             self.__topic_dao[topic.id] = dao
+        self.__update_topics()
 
         return dao
```

### Comparing `drb-2.1.4/drb/topics/dao/topic_dao.py` & `drb-2.1.5/drb/topics/dao/topic_dao.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,13 +24,13 @@
         raise NotImplementedError
 
     @abstractmethod
     def delete(self, identifier: uuid.UUID) -> None:
         raise NotImplementedError
 
     @abstractmethod
-    def find(self, label: str) -> DrbTopic:
+    def find(self, search: str) -> List[DrbTopic]:
         raise NotImplementedError
 
     @abstractmethod
     def read_all(self) -> List[DrbTopic]:
         raise NotImplementedError
```

### Comparing `drb-2.1.4/drb/topics/dao/topic_schema.yml` & `drb-2.1.5/drb/topics/dao/topic_schema.yml`

 * *Files identical despite different names*

### Comparing `drb-2.1.4/drb/topics/dao/xml_dao.py` & `drb-2.1.5/drb/topics/dao/xml_dao.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import logging
 import uuid
 from pathlib import Path
 from typing import List
+from deprecated import deprecated
 
 from drb.drivers.xml import XmlNodeFactory, XmlNode
 
 from .topic_dao import DrbTopicDao
 from drb.core.signature import parse_signature
 from drb.topics.topic import DrbTopic, TopicCategory
 from drb.exceptions.core import DrbException
@@ -16,14 +17,16 @@
 
 ns = {'owl': 'http://www.w3.org/2002/07/owl#',
       'drb': 'http://www.gael.fr/drb#',
       'rdfs': 'http://www.w3.org/2000/01/rdf-schema#',
       'rdf': 'http://www.w3.org/1999/02/22-rdf-syntax-ns#'}
 
 
+@deprecated(version='2.1.4',
+            reason='Usage of the RDFDao is recommended')
 class XmlDao(DrbTopicDao):
 
     def __init__(self, path: str):
         # if not existing, generate a new file.
         Path(path).touch(exist_ok=True)
 
         self.__file = path
@@ -50,22 +53,22 @@
         Returns:
             DrbTopic: the corresponding topic
         """
         data = {}
         uri_parent = None
         uri = list(node.attributes.values())[0]
 
+        data['uri'] = uri
         data['id'] = self.generate_id(uri)
         data['category'] = TopicCategory('CONTAINER')
 
         signatures = []
         parents = []
 
         for child in node.children:
-
             if child.name == 'subClassOf':
 
                 try:
                     uri_parent = list(child.attributes.values())[0]
 
                 except (IndexError, DrbException):
                     for grandchild in child.children:
@@ -93,14 +96,18 @@
                         signature['name'] = grandchild.value
                         signatures.append(signature)
 
                     elif grandchild.name == 'parentClassName':
                         signature['parent'] = grandchild.value
                         signatures.append(signature)
 
+                    elif grandchild.name == 'xqueryTest':
+                        signature['xquery'] = grandchild.value
+                        signatures.append(signature)
+
                 data['signatures'] = [parse_signature(s) for s in signatures]
         topic = DrbTopic(**data)
 
         return topic
 
     @staticmethod
     def generate_id(uri: str) -> uuid.UUID:
@@ -130,32 +137,32 @@
                 topic = self.__generate_topic_from_xml_node(node)
                 return topic
             else:
                 continue
 
         raise DrbException
 
-    def find(self, label: str) -> DrbTopic:
+    def find(self, search: str) -> List[DrbTopic]:
         """
         Finds a topic from an XML file.
         Parameters:
-            label (str): label of topic to read from file
+            search (str): label of topic to read from file
         Returns:
-            DrbTopic: the topic corresponding to the given label
+            List[DrbTopic]: the topic corresponding to the given label
         """
-
+        topics = []
         for node in self.__nodes:
             for child in node.children:
 
                 if child.name == 'label':
-                    if child.value == label:
+                    if search in child.value:
                         topic = self.__generate_topic_from_xml_node(node)
-                        return topic
+                        topics.append(topic)
 
-        raise DrbException
+        return topics
 
     def read_all(self) -> List[DrbTopic]:
         """
         Loads all topics defined in XML files.
         """
 
         topics = []
```

### Comparing `drb-2.1.4/drb/topics/dao/yaml_dao.py` & `drb-2.1.5/drb/topics/dao/yaml_dao.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,15 @@
             ic_data (dict): dictionary from YAML file
         Returns:
             DrbTopic: the corresponding topic
         """
         data = {'id': uuid.UUID(ic_data['id']), 'label': ic_data['label'],
                 'category': TopicCategory(ic_data['category']),
                 'description': ic_data.get('description', None),
+                'uri': ic_data.get('uri', None),
                 'factory': ic_data.get('factory', None),
                 'forced': ic_data.get('forced', False)}
 
         signatures = ic_data.get('signatures', None)
         if signatures is not None:
             data['signatures'] = [parse_signature(s) for s in signatures]
         else:
@@ -246,34 +247,33 @@
                 topic_data = self.__write_topic_to_yaml_file(topic)
                 docs.append(topic_data)
 
         with open(self.__file, 'w') as file:
             yaml.safe_dump_all(docs, file,
                                default_flow_style=False, sort_keys=False)
 
-    def find(self, label: str) -> DrbTopic:
+    def find(self, search: str) -> List[DrbTopic]:
         """
         Finds a topic in a YAML file.
         Parameters:
-        label (str): id of topic to read from file
+        search (str): id of topic to read from file
         Returns:
-        DrbTopic: the topic corresponding to the given label
+        List[DrbTopic]: the topic corresponding to the given label
         """
+        topics = []
         with open(self.__file, 'r') as file:
             data = yaml.safe_load_all(file)
             for topic_data in data:
 
-                if topic_data['label'] == label:
+                if search in topic_data['label']:
                     topic = self.__generate_topic_from_yaml_file(
                             topic_data)
+                    topics.append(topic)
 
-        try:
-            return topic
-        except UnboundLocalError:
-            raise DrbException
+        return topics
 
     def read_all(self) -> List[DrbTopic]:
         """
         Loads all topics defined in a Cortex YAML file.
         """
 
         topics = []
```

### Comparing `drb-2.1.4/drb/topics/resolver.py` & `drb-2.1.5/drb/topics/resolver.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,44 +41,19 @@
     """ The factory resolver
 
     The factory resolver aims to parametrize the selection of the factory
     able to resolves the nodes according to its physical input.
     """
 
     __instance = None
-    __topics = None
-    __overridden: List[DrbTopic] = None
-    __protocols: List[DrbTopic] = None
-    __containers: List[DrbTopic] = None
-    __highest_containers: List[DrbTopic] = None
-    __formats: List[DrbTopic] = None
 
     def __new__(cls, *args, **kwargs):
         if cls.__instance is None:
             cls.__instance = super(_DrbFactoryResolver, cls).__new__(cls)
-            cls.__topics = ManagerDao().get_all_drb_topics()
 
-            cls.__overridden = []
-            cls.__protocols = []
-            cls.__containers = []
-            cls.__formats = []
-            for ic in cls.__topics:
-                if ic.override:
-                    cls.__overridden.append(ic)
-                if TopicCategory.PROTOCOL == ic.category:
-                    cls.__protocols.append(ic)
-                elif TopicCategory.CONTAINER == ic.category:
-                    cls.__containers.append(ic)
-                elif TopicCategory.FORMATTING == ic.category:
-                    cls.__formats.append(ic)
-                else:
-                    logger.warning('DRB resolver does not support item type: '
-                                   f'{ic.category.name}')
-            cls.__highest_containers = [x for x in cls.__containers
-                                        if x.subClassOf is None]
         return cls.__instance
 
     def _create(self, node: DrbNode) -> DrbNode:
         topic, n = self.resolve(node)
         return n
 
     def __retrieve_protocol(self, node: DrbNode) -> Optional[DrbTopic]:
@@ -87,15 +62,16 @@
 
         Parameters:
             node (DrbNode): node which need to be resolved
         Returns:
             DrbNode: a protocol topic associated to the given node or
                      ``None`` if no protocol item class is found.
         """
-        for protocol in self.__protocols:
+        for protocol in ManagerDao().get_drb_topics_by_category(
+                TopicCategory.PROTOCOL):
             node = forced_factory(protocol, node)
             if protocol.matches(node):
                 return protocol
         return None
 
     def __retrieve_container(self, node: DrbNode) -> Tuple[DrbTopic, DrbNode]:
         """
@@ -103,15 +79,20 @@
 
         Parameters:
             node (DrbNode): node which need to be resolved
         Returns:
             DrbTopic, DrbNode: A topic matching the given node and the
                                 associated node
         """
-        for s in self.__highest_containers:
+        highest_containers = [x for x in
+                              ManagerDao().get_drb_topics_by_category(
+                                  TopicCategory.CONTAINER)
+                              if x.subClassOf is None]
+
+        for s in highest_containers:
             node = forced_factory(s, node)
             if s.matches(node):
                 return self.__finest_drb_topic(node, s)
         return None, node
 
     def __finest_drb_topic(self, node: DrbNode, finest: DrbTopic) \
             -> Tuple[DrbTopic, DrbNode]:
@@ -121,16 +102,16 @@
         Parameters:
             node (DrbNode): node which need to be resolved
             finest (DrbTopic): current finest topic matching the given
                                 node
         Returns:
             DrbTopic: the finest topic matching the given node
         """
-        topics = [x for x in self.__topics if x.subClassOf is not None
-                  if x.subClassOf[0] == finest.id]
+        topics = [x for x in ManagerDao().get_all_drb_topics()
+                  if x.subClassOf is not None if x.subClassOf[0] == finest.id]
         for topic in topics:
             node = forced_factory(topic, node)
             if topic.matches(node):
                 n = node
                 if topic.factory is not None:
                     n = FactoryLoader().get_factory(
                         topic.factory).create(node)
@@ -143,15 +124,16 @@
 
         Parameters:
             node (DrbNode): node which need to be resolved
         Returns:
             DrbTopic: A formatting topic matching the given node,
                        otherwise ``None``
         """
-        for topic in self.__formats:
+        for topic in ManagerDao().get_drb_topics_by_category(
+                TopicCategory.FORMATTING):
             node = forced_factory(topic, node)
             if topic.matches(node):
                 return topic
         return None
 
     def __create_from_url(self, url: str, curl: str = None,
                           path: List[str] = None) -> DrbNode:
@@ -217,15 +199,15 @@
                 curl += f'/{seg}'
             else:
                 curl = os.path.join(curl, path.pop(0))
             return self.__create_from_url(url, curl, path)
 
     def _resolve_overridden(self, source: DrbNode) -> \
             Optional[Tuple[DrbTopic, Optional[DrbNode]]]:
-        for ic in self.__overridden:
+        for ic in ManagerDao().get_overridden_drb_topics():
             source = forced_factory(ic, source)
             if ic.matches(source):
                 return self.__finest_drb_topic(source, ic)
         return None
 
     def _basic_resolve(self, source: DrbNode) -> \
             Tuple[DrbTopic, Optional[DrbNode]]:
```

### Comparing `drb-2.1.4/drb/utils/drb_python_script.py` & `drb-2.1.5/drb/utils/drb_python_script.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,12 +24,12 @@
 
     my_globals = globals()
     my_globals['node'] = node
     for k, v in kwargs.items():
         my_globals[k] = v
 
     exec(compile(init_ast, "<ast>", "exec"), my_globals)
-    if type(last_ast.body[0]) == ast.Expr:
+    if type(last_ast.body[0]) is ast.Expr:
         return eval(compile(_convert_expr2expression(last_ast.body[0]),
                             "<ast>", "eval"), my_globals)
     else:
         exec(compile(last_ast, "<ast>", "exec"), my_globals)
```

### Comparing `drb-2.1.4/drb/utils/plugins.py` & `drb-2.1.5/drb/utils/plugins.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.4/drb/utils/utils.py` & `drb-2.1.5/drb/utils/utils.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.4/drb.egg-info/PKG-INFO` & `drb-2.1.5/drb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drb
-Version: 2.1.4
+Version: 2.1.5
 Summary: Data Request Broker
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
```

### Comparing `drb-2.1.4/drb.egg-info/SOURCES.txt` & `drb-2.1.5/drb.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 drb/nodes/mutable_node.py
 drb/nodes/url_node.py
 drb/signatures/core.py
 drb/topics/resolver.py
 drb/topics/topic.py
 drb/topics/dao/__init__.py
 drb/topics/dao/manager_dao.py
+drb/topics/dao/rdf_dao.py
 drb/topics/dao/topic_dao.py
 drb/topics/dao/topic_schema.yml
 drb/topics/dao/xml_dao.py
 drb/topics/dao/yaml_dao.py
 drb/topics/file/__init__.py
 drb/topics/file/cortex.yml
 drb/topics/xml/__init__.py
@@ -58,12 +59,13 @@
 tests/test_event.py
 tests/test_factory.py
 tests/test_factory_resolver.py
 tests/test_keyring_bitwarden.py
 tests/test_logical_node.py
 tests/test_manager_dao.py
 tests/test_path.py
+tests/test_rdf_dao.py
 tests/test_signatures.py
 tests/test_topic.py
 tests/test_url_node.py
 tests/test_xml_dao.py
 tests/test_yaml_dao.py
```

### Comparing `drb-2.1.4/drb.egg-info/entry_points.txt` & `drb-2.1.5/drb.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `drb-2.1.4/setup.cfg` & `drb-2.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `drb-2.1.4/tests/test_abstract_node.py` & `drb-2.1.5/tests/test_abstract_node.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.4/tests/test_drb_node_list.py` & `drb-2.1.5/tests/test_drb_node_list.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.4/tests/test_event.py` & `drb-2.1.5/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.4/tests/test_factory.py` & `drb-2.1.5/tests/test_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import unittest
 from drb.core import DrbNode
 from drb.core.factory import DrbFactory, FactoryLoader
-from drb.exceptions.core import DrbException
 from tests.utils import DrbTestNode
-from typing import Union
 
 
 class DefaultFactory(DrbFactory):
     def _create(self, node: DrbNode) -> DrbNode:
         return DrbTestNode(f"DefaultNode_{node.name}")
```

### Comparing `drb-2.1.4/tests/test_factory_resolver.py` & `drb-2.1.5/tests/test_factory_resolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import unittest
 from uuid import UUID
 
 import drb.topics.resolver as resolver
 from drb.nodes.logical_node import DrbLogicalNode
 from drb.nodes.url_node import UrlNode
 from drb.exceptions.core import DrbFactoryException
-from drb.topics.dao.manager_dao import _load_all_drb_topic_dao
 
 
 class TestDrbFactoryResolver(unittest.TestCase):
     mock_package_path: str = None
     signature_uuid: dict = None
 
     @classmethod
```

### Comparing `drb-2.1.4/tests/test_keyring_bitwarden.py` & `drb-2.1.5/tests/test_keyring_bitwarden.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.4/tests/test_logical_node.py` & `drb-2.1.5/tests/test_logical_node.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.4/tests/test_manager_dao.py` & `drb-2.1.5/tests/test_manager_dao.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
                             'resources', 'packages')
         sys.path.append(path)
 
     def test_get_all_drb_topics(self):
         manager = ManagerDao()
         topics = manager.get_all_drb_topics()
         self.assertIsNotNone(topics)
-        self.assertEqual(31, len(list(topics)))
+        self.assertEqual(32, len(list(topics)))
 
     def test_get_drb_topic(self):
         manager = ManagerDao()
         identifier = uuid.UUID('3d797648-281a-11ec-9621-0242ac130002')
         label = 'Text'
 
         topic = manager.get_drb_topic(identifier)
@@ -55,14 +55,15 @@
         identifier = uuid.UUID('84a54dea-2800-11ec-9621-0242ac130002')
 
         parent_identifier = uuid.UUID('4cd8fe12-827c-11ec-a8a3-0242ac120002')
         parent_label = 'Sentinel SAFE Product'
 
         topic = manager.get_drb_topic(identifier)
         parents = manager.get_parents(topic)
+        print(parents[0].uri)
 
         self.assertIsNotNone(parents)
         self.assertIsInstance(parents[0], DrbTopic)
         self.assertEqual(parent_identifier, parents[0].id)
         self.assertEqual(parent_label, parents[0].label)
 
     def test_get_children(self):
```

### Comparing `drb-2.1.4/tests/test_path.py` & `drb-2.1.5/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.4/tests/test_signatures.py` & `drb-2.1.5/tests/test_signatures.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.4/tests/test_topic.py` & `drb-2.1.5/tests/test_topic.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,33 +12,30 @@
     def test_drb_topic(self):
         data = {
             'id': uuid.UUID('93b508a0-6ee8-11ec-90d6-0242ac120003'),
             'subClassOf': uuid.UUID('096ad7b2-e17b-4a4b-a6c3-c07ad5879203'),
             'label': 'test',
             'description': 'test topic description',
             'category': TopicCategory('FORMATTING'),
-            'factory': {
-                'name': 'test',
-                'classpath': 'tests.utils:DrbTestFactory'
-            },
+            'factory': 'test',
             'signatures': [
                 parse_signature({'name': 'test_.+'}),
                 parse_signature({'name': '.+_test'}),
             ]
         }
 
         topic = DrbTopic(**data)
         self.assertEqual(data['id'], topic.id)
         self.assertEqual(data['subClassOf'], topic.subClassOf)
         self.assertEqual(data['label'], topic.label)
         self.assertEqual(data['description'], topic.description)
         self.assertEqual(TopicCategory.FORMATTING, topic.category)
 
-        FactoryLoader().get_factory(topic.factory['name'])
-        factory = FactoryLoader().get_factory(topic.factory['name'])
+        FactoryLoader().get_factory(topic.factory)
+        factory = FactoryLoader().get_factory(topic.factory)
         self.assertIsNotNone(factory)
         self.assertIsInstance(factory, DrbTestFactory)
 
         self.assertEqual(2, len(topic.signatures))
         self.assertTrue(topic.matches(DrbLogicalNode('test_foobar')))
         self.assertTrue(topic.matches(DrbLogicalNode('foobar_test')))
         self.assertFalse(topic.matches(DrbLogicalNode('foobar')))
```

### Comparing `drb-2.1.4/tests/test_url_node.py` & `drb-2.1.5/tests/test_url_node.py`

 * *Files identical despite different names*

### Comparing `drb-2.1.4/tests/test_yaml_dao.py` & `drb-2.1.5/tests/test_yaml_dao.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,24 +22,28 @@
 
         self.assertIsNotNone(topic)
         self.assertIsInstance(topic, DrbTopic)
         self.assertEqual(identifier, topic.id)
         self.assertEqual(label, topic.label)
 
     def test_find(self):
-        identifier = uuid.UUID('50f9cd76-e1ab-4c08-8b4d-619bc1e413c2')
-        label = 'Sentinel-3 SYNERGIE Level-2 VGP Product'
-        topic = self.dao.find(label)
+        search = 'Sentinel-3 SYNERGIE Level-2 V'
+        topics = self.dao.find(search)
 
-        self.assertIsNotNone(topic)
-        self.assertIsInstance(topic, DrbTopic)
-        self.assertEqual(identifier, topic.id)
-        self.assertEqual(label, topic.label)
-        with self.assertRaises(DrbException):
-            self.dao.find("None")
+        self.assertIsNotNone(topics)
+        self.assertEqual(5, len(list(topics)))
+        found_topic = None
+
+        for topic in topics:
+            self.assertIsInstance(topic, DrbTopic)
+            if topic.label == 'Sentinel-3 SYNERGIE Level-2 V10 Product':
+                found_topic = topic
+                continue
+
+        self.assertIsNotNone(found_topic)
 
     def test_read_all(self):
 
         topics = self.dao.read_all()
 
         self.assertIsNotNone(topics)
         self.assertIsInstance(topics, List)
```

### Comparing `drb-2.1.4/versioneer.py` & `drb-2.1.5/versioneer.py`

 * *Files identical despite different names*

