# Comparing `tmp/asyncua-1.0.2.tar.gz` & `tmp/asyncua-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncua-1.0.2.tar", last modified: Wed Apr  5 15:41:52 2023, max compression
+gzip compressed data, was "asyncua-1.0.3.tar", last modified: Mon Jul 31 17:53:23 2023, max compression
```

## Comparing `asyncua-1.0.2.tar` & `asyncua-1.0.3.tar`

### file list

```diff
@@ -1,92 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:41:52.486804 asyncua-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-05 15:41:43.000000 asyncua-1.0.2/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-04-05 15:41:52.486804 asyncua-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-04-05 15:41:43.000000 asyncua-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:41:52.466804 asyncua-1.0.2/asyncua/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:41:52.466804 asyncua-1.0.2/asyncua/client/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39711 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:41:52.470804 asyncua-1.0.2/asyncua/client/ha/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/client/ha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/client/ha/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    20851 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/client/ha/ha_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17959 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/client/ha/reconciliator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/client/ha/virtual_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    36703 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/client/ua_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/client/ua_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    14064 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/client/ua_file_transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:41:52.470804 asyncua-1.0.2/asyncua/common/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/common/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    21504 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/common/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/common/copy_node_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    57878 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/common/event_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    12718 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/common/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/common/instantiate_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    18578 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/common/manage_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/common/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)    29476 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/common/node.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/common/node_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    10695 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/common/session_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/common/shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/common/sql_injection.py
--rw-r--r--   0 runner    (1001) docker     (123)    18906 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/common/statemachine.py
--rw-r--r--   0 runner    (1001) docker     (123)    12230 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/common/structures.py
--rw-r--r--   0 runner    (1001) docker     (123)    20872 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/common/structures104.py
--rw-r--r--   0 runner    (1001) docker     (123)    23427 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/common/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    12929 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/common/type_dictionary_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/common/ua_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23287 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/common/xmlexporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    33433 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/common/xmlimporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16344 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/common/xmlparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:41:52.470804 asyncua-1.0.2/asyncua/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/crypto/permission_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    28638 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/crypto/security_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     8353 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/crypto/uacrypto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:41:52.474804 asyncua-1.0.2/asyncua/server/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38773 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/server/address_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/server/binary_server_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/server/event_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15848 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/server/history.py
--rw-r--r--   0 runner    (1001) docker     (123)    13926 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/server/history_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)    16795 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/server/internal_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    10937 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/server/internal_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    11037 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/server/internal_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    16022 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/server/monitored_item_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    34493 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:41:52.474804 asyncua-1.0.2/asyncua/server/standard_address_space/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/server/standard_address_space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/server/standard_address_space/standard_address_space.py
--rw-r--r--   0 runner    (1001) docker     (123)  7910304 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/server/standard_address_space/standard_address_space_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/server/subscription_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    28769 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/server/uaprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/server/user_managers.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/server/users.py
--rw-r--r--   0 runner    (1001) docker     (123)    17381 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)    30269 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:41:52.486804 asyncua-1.0.2/asyncua/ua/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/ua/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/ua/attribute_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)  2533939 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/ua/object_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)    41076 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/ua/status_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)    24936 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/ua/ua_binary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:41:52.486804 asyncua-1.0.2/asyncua/ua/uaerrors/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/ua/uaerrors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15665 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/ua/uaerrors/_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/ua/uaerrors/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)   343641 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/ua/uaprotocol_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     9437 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/ua/uaprotocol_hand.py
--rw-r--r--   0 runner    (1001) docker     (123)    36912 2023-04-05 15:41:43.000000 asyncua-1.0.2/asyncua/ua/uatypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:41:52.466804 asyncua-1.0.2/asyncua.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-04-05 15:41:52.000000 asyncua-1.0.2/asyncua.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-04-05 15:41:52.000000 asyncua-1.0.2/asyncua.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 15:41:52.000000 asyncua-1.0.2/asyncua.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-05 15:41:52.000000 asyncua-1.0.2/asyncua.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-05 15:41:52.000000 asyncua-1.0.2/asyncua.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-05 15:41:52.000000 asyncua-1.0.2/asyncua.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-05 15:41:52.486804 asyncua-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-05 15:41:43.000000 asyncua-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:53:23.626843 asyncua-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-07-31 17:53:11.000000 asyncua-1.0.3/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     9014 2023-07-31 17:53:23.626843 asyncua-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-07-31 17:53:11.000000 asyncua-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:53:23.598843 asyncua-1.0.3/asyncua/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:53:23.598843 asyncua-1.0.3/asyncua/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40259 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:53:23.598843 asyncua-1.0.3/asyncua/client/ha/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/client/ha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/client/ha/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20991 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/client/ha/ha_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17949 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/client/ha/reconciliator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/client/ha/virtual_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36830 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/client/ua_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/client/ua_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/client/ua_file_transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:53:23.602843 asyncua-1.0.3/asyncua/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/common/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21523 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/common/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/common/copy_node_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56734 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/common/event_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13206 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/common/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/common/instantiate_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18578 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/common/manage_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/common/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30785 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/common/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/common/node_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10695 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/common/session_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/common/shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/common/sql_injection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18997 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/common/statemachine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12230 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/common/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21040 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/common/structures104.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23110 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/common/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12929 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/common/type_dictionary_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10335 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/common/ua_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23306 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/common/xmlexporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33433 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/common/xmlimporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16498 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/common/xmlparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:53:23.602843 asyncua-1.0.3/asyncua/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/crypto/cert_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/crypto/permission_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28636 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/crypto/security_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8995 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/crypto/uacrypto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:53:23.606843 asyncua-1.0.3/asyncua/server/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39009 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/server/address_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/server/binary_server_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/server/event_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15848 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/server/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13926 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/server/history_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17789 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/server/internal_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10937 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/server/internal_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11037 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/server/internal_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16539 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/server/monitored_item_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36999 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:53:23.606843 asyncua-1.0.3/asyncua/server/standard_address_space/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/server/standard_address_space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/server/standard_address_space/standard_address_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)  7910304 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/server/standard_address_space/standard_address_space_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/server/subscription_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28769 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/server/uaprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/server/user_managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/server/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19443 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30228 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:53:23.622843 asyncua-1.0.3/asyncua/ua/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/ua/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/ua/attribute_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2533914 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/ua/object_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41026 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/ua/status_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24939 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/ua/ua_binary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:53:23.626843 asyncua-1.0.3/asyncua/ua/uaerrors/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/ua/uaerrors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15665 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/ua/uaerrors/_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/ua/uaerrors/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   343641 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/ua/uaprotocol_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9386 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/ua/uaprotocol_hand.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36928 2023-07-31 17:53:11.000000 asyncua-1.0.3/asyncua/ua/uatypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:53:23.598843 asyncua-1.0.3/asyncua.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9014 2023-07-31 17:53:23.000000 asyncua-1.0.3/asyncua.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-31 17:53:23.000000 asyncua-1.0.3/asyncua.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 17:53:23.000000 asyncua-1.0.3/asyncua.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-31 17:53:23.000000 asyncua-1.0.3/asyncua.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-31 17:53:23.000000 asyncua-1.0.3/asyncua.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-31 17:53:23.000000 asyncua-1.0.3/asyncua.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-31 17:53:23.626843 asyncua-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-31 17:53:11.000000 asyncua-1.0.3/setup.py
```

### Comparing `asyncua-1.0.2/COPYING` & `asyncua-1.0.3/COPYING`

 * *Files identical despite different names*

### Comparing `asyncua-1.0.2/PKG-INFO` & `asyncua-1.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,71 +1,50 @@
-Metadata-Version: 2.1
-Name: asyncua
-Version: 1.0.2
-Summary: Pure Python OPC-UA client and server library
-Home-page: http://freeopcua.github.io/
-Author: Olivier Roulet-Dubonnet
-Author-email: olivier.roulet@gmail.com
-License: GNU Lesser General Public License v3 or later
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Provides: asyncua
-Description-Content-Type: text/markdown
-License-File: COPYING
-
 OPC UA / IEC 62541 Client and Server for Python >= 3.7 and pypy3 .
 http://freeopcua.github.io/, https://github.com/FreeOpcUa/opcua-asyncio
 
 [![Python package](https://github.com/FreeOpcUa/opcua-asyncio/workflows/Python%20package/badge.svg)](https://github.com/FreeOpcUa/opcua-asyncio/actions)
 
 [![PyPI Package](https://badge.fury.io/py/asyncua.svg)](https://badge.fury.io/py/asyncua)
 
 # opcua-asyncio
 
 opcua-asyncio is an asyncio-based asynchronous OPC UA client and server based on python-opcua, removing support of python < 3.7.
-Asynchronous programming allows for simpler code (e.g. less need for locks) and potentially performance gains.
-This library has also [sync wrapper](https://github.com/FreeOpcUa/opcua-asyncio/blob/master/asyncua/sync.py) over async API which may can be used in sync code instead of python-opcua
+Asynchronous programming allows for simpler code (e.g. less need for locks) and can potentially provide performance improvements.
+This library also provides a [synchronous wrapper](https://github.com/FreeOpcUa/opcua-asyncio/blob/master/asyncua/sync.py) over the async API, which can be used in synchronous code instead of python-opcua.
 
 ---
 
-OPC UA binary protocol implementation has been tested against many different OPC UA stacks. API offers both a low level interface to send and receive all UA defined structures and high level classes allowing to write a server or a client in a few lines. It is easy to mix high level objects and low level UA calls in one application. Most low level code is autogenerated from xml specification.
-
-coverage.py reports a test coverage of over 95 % of code, most of non-tested code is autogenerated code that is not used yet.
+The OPC UA binary protocol implementation has undergone extensive testing with various OPC UA stacks. The API offers both a low level interface to send and receive all UA defined structures and high level classes allowing to write a server or a client in a few lines. It is easy to mix high level objects and low level UA calls in one application. Most low level code is autogenerated from xml specification.
 
+The test coverage reported by coverage.py is over 95%, with the majority of the non-tested code being autogenerated code that is not currently in use.
 
 # Warnings
 
-opcua-asyncio is open-source and comes with absolutely no warranty. We try to keep it as much bug-free as possible and try to keep API stable but bugs and API changes will happen! Especially API changes will happen before any 1.0 release.
+opcua-asyncio is open-source and comes with absolutely no warranty. We try to keep it as bug-free as possible, and try to keep the API stable, but bugs and API changes will happen! In particular, API changes are expected to take place prior to any 1.0 release.
 
 Some renaming of methods from get_xx to read_xx and set_xx to write_xxx have been made to better follow OPC UA naming conventions
 
-Version 0.9.9 introduces some argument renaming due to more automatic code generation. Especially the arguments to NodeId, BrowseName, LocalizedText and DataValue are now CamelCase instead of lower case, thus follow the OPC Ua convention used in all other structures in this library
+Version 0.9.9 introduces some argument renaming due to more automatic code generation. Especially the arguments to NodeId, BrowseName, LocalizedText and DataValue, which are now CamelCase instead of lower case, following the OPC UA conventions used in all other structures in this library
 
 # Installation
 
 With pip
 
     pip install asyncua
 
 # Usage
 
 We assume that you already have some experience with Python, the asyncio module, the async / await syntax and the concept of asyncio Tasks.
 
 ## Client class
 
-The `Client` class provides a high level API for connecting to APU UA servers, session management and access to basic
+The `Client` class provides a high level API for connecting to OPC UA servers, session management and access to basic
 address space services.
 The client can be used as a context manager. The client will then automatically connect and disconnect withing the `with`syntax.
 
-
 ```python
 from asyncua import Client
 
 async with Client(url='opc.tcp://localhost:4840/freeopcua/server/') as client:
     while True:
         # Do something with client
         node = client.get_node('i=85')
@@ -88,144 +67,146 @@
 
 The `Server` class provides a high level API for creation of OPC UA server instances.
 
 # Documentation
 
 The documentation is available here [ReadTheDocs](http://opcua-asyncio.readthedocs.org/en/latest/).
 
-The API remains mostly unchanged in regards to [python-opcua](http://opcua-asyncio.rtfd.io/).
-Main difference is that most methods are now async.
+The API remains mostly unchanged with regards to [python-opcua](http://opcua-asyncio.rtfd.io/).
+The main difference is that most methods are now asynchronous.
 Please have a look at [the examples](https://github.com/FreeOpcUa/opcua-asyncio/blob/master/examples) and/or the code.
 
-A simple GUI client is available: https://github.com/FreeOpcUa/opcua-client-gui
+A simple GUI client is available at: https://github.com/FreeOpcUa/opcua-client-gui
 
 Browse the examples: https://github.com/FreeOpcUa/opcua-asyncio/tree/master/examples
 
-A good starting point are the minimal examples.
+The minimal examples are a good starting point.
 Minimal client example: https://github.com/FreeOpcUa/opcua-asyncio/blob/master/examples/client-minimal.py
 Minimal server example: https://github.com/FreeOpcUa/opcua-asyncio/blob/master/examples/server-minimal.py
 
 A set of command line tools also available: https://github.com/FreeOpcUa/opcua-asyncio/tree/master/tools
-* `uadiscover `(find_servers, get_endpoints and find_servers_on_network calls)
-* `uals `(list children of a node)
-* `uahistoryread`
-* `uaread `(read attribute of a node)
-* `uawrite `(write attribute of a node)
-* `uacall `(call method of a node)
-* `uasubscribe `(subscribe to a node and print datachange events)
-* `uaclient `(connect to server and start python shell)
-* `uaserver `(starts a demo OPC UA server)
-  `tools/uaserver --populate --certificate cert.pem --private_key pk.pem`
+
+-   `uadiscover `(find_servers, get_endpoints and find_servers_on_network calls)
+-   `uals `(list children of a node)
+-   `uahistoryread`
+-   `uaread `(read attribute of a node)
+-   `uawrite `(write attribute of a node)
+-   `uacall `(call method of a node)
+-   `uasubscribe `(subscribe to a node and print datachange events)
+-   `uaclient `(connect to server and start python shell)
+-   `uaserver `(starts a demo OPC UA server)
+    `tools/uaserver --populate --certificate cert.pem --private_key pk.pem`
 
 How to generate certificate: https://github.com/FreeOpcUa/opcua-asyncio/tree/master/examples/generate_certificate.sh
 
 ## Client support
 
 What works:
 
-* connection to server, opening channel, session
-* browsing and reading attributes value
-* getting nodes by path and nodeids
-* creating subscriptions
-* subscribing to items for data change
-* subscribing to events
-* adding nodes
-* method call
-* user and password
-* history read
-* login with certificate
-* communication encryption
-* removing nodes
+-   connection to server, opening channel, session
+-   browsing and reading attributes value
+-   getting nodes by path and nodeids
+-   creating subscriptions
+-   subscribing to items for data change
+-   subscribing to events
+-   adding nodes
+-   method call
+-   user and password
+-   history read
+-   login with certificate
+-   communication encryption
+-   removing nodes
 
 Tested servers: freeopcua C++, freeopcua Python, prosys, kepware, beckhoff, winCC, B&R, …
 
 Not implemented yet:
 
-* localized text feature
-* XML protocol
-* UDP (PubSub stuff)
-* WebSocket
-* maybe automatic reconnection...
-
+-   localized text feature
+-   XML protocol
+-   UDP (PubSub stuff)
+-   WebSocket
+-   maybe automatic reconnection...
 
 ## Server support
 
 What works:
 
-* creating channel and sessions
-* read/set attributes and browse
-* getting nodes by path and nodeids
-* autogenerate address space from spec
-* adding nodes to address space
-* datachange events
-* events
-* methods
-* basic user implementation (one existing user called admin, which can be disabled, all others are read only)
-* encryption
-* certificate handling
-* removing nodes
-* history support for data change and events
-* more high level solution to create custom structures
+-   creating channel and sessions
+-   read/set attributes and browse
+-   getting nodes by path and nodeids
+-   autogenerate address space from spec
+-   adding nodes to address space
+-   datachange events
+-   events
+-   methods
+-   basic user implementation (one existing user called admin, which can be disabled, all others are read only)
+-   encryption
+-   certificate handling
+-   removing nodes
+-   history support for data change and events
+-   more high level solution to create custom structures
 
 Tested clients: freeopcua C++, freeopcua Python, uaexpert, prosys, quickopc
 
 Not yet implemented:
 
-* UDP (PubSub stuff)
-* WebSocket
-* session restore
-* alarms
-* XML protocol
-* views
-* localized text features
-* better security model with users and password
-
+-   UDP (PubSub stuff)
+-   WebSocket
+-   session restore
+-   alarms
+-   XML protocol
+-   views
+-   localized text features
+-   better security model with users and password
 
 ### Running a server on a Raspberry Pi
 
 Setting up the standard address-space from XML is the most time-consuming step of the startup process which may lead to
 long startup times on less powerful devices like a Raspberry Pi. By passing a path to a cache-file to the server constructor,
 a shelve holding the address space will be created during the first startup. All following startups will make use of the
 cache-file which leads to significantly better startup performance (~3.5 vs 125 seconds on a Raspberry Pi Model B).
 
-
 # Development
 
 Code follows PEP8 apart for line lengths which should be max 160 characters and OPC UA structures that keep camel case
 from XML definition.
 
 All protocol code is under opcua directory
 
-- `asyncua/ua` contains all UA structures from specification, most are autogenerated
-- `asyncua/common` contains high level objects and methods used both in server and client
-- `asyncua/client` contains client specific code
-- `asyncua/server` contains server specific code
-- `asyncua/utils` contains some utilities function and classes
-- `asyncua/tools` contains code for command lines tools
-- `schemas` contains the XML and text files from specification and the python scripts used to autogenerate code
-- `tests` contains tests
-- `docs` contains files to auto generate documentation from doc strings
-- `examples` contains many example files
-- `examples/sync` contains many example files using sync API
-- `tools` contains python scripts that can be used to run command line tools from repository without installing
+-   `asyncua/ua` contains all UA structures from specification, most are autogenerated
+-   `asyncua/common` contains high level objects and methods used both in server and client
+-   `asyncua/client` contains client specific code
+-   `asyncua/server` contains server specific code
+-   `asyncua/utils` contains some utilities function and classes
+-   `asyncua/tools` contains code for command lines tools
+-   `schemas` contains the XML and text files from specification and the python scripts used to autogenerate code
+-   `tests` contains tests
+-   `docs` contains files to auto generate documentation from doc strings
+-   `examples` contains many example files
+-   `examples/sync` contains many example files using sync API
+-   `tools` contains python scripts that can be used to run command line tools from repository without installing
 
 ## Running tests:
 
 ```
 python -m pip install -r requirements.txt
 python -m pip install -r dev_requirements.txt
 pytest -v -s
 ```
+
 Or
+
 ```
 ./run-test.sh -v -s
 ```
 
 ## Coverage
 
 ```
 pytest -v -s --cov asyncua --cov-report=html
 ```
+
 Or
+
 ```
 ./run-test.sh -v -s --cov asyncua --cov-report=html
 ```
```

### Comparing `asyncua-1.0.2/README.md` & `asyncua-1.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,69 @@
+Metadata-Version: 2.1
+Name: asyncua
+Version: 1.0.3
+Summary: Pure Python OPC-UA client and server library
+Home-page: http://freeopcua.github.io/
+Author: Olivier Roulet-Dubonnet
+Author-email: olivier.roulet@gmail.com
+License: GNU Lesser General Public License v3 or later
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides: asyncua
+Description-Content-Type: text/markdown
+License-File: COPYING
+
 OPC UA / IEC 62541 Client and Server for Python >= 3.7 and pypy3 .
 http://freeopcua.github.io/, https://github.com/FreeOpcUa/opcua-asyncio
 
 [![Python package](https://github.com/FreeOpcUa/opcua-asyncio/workflows/Python%20package/badge.svg)](https://github.com/FreeOpcUa/opcua-asyncio/actions)
 
 [![PyPI Package](https://badge.fury.io/py/asyncua.svg)](https://badge.fury.io/py/asyncua)
 
 # opcua-asyncio
 
 opcua-asyncio is an asyncio-based asynchronous OPC UA client and server based on python-opcua, removing support of python < 3.7.
-Asynchronous programming allows for simpler code (e.g. less need for locks) and potentially performance gains.
-This library has also [sync wrapper](https://github.com/FreeOpcUa/opcua-asyncio/blob/master/asyncua/sync.py) over async API which may can be used in sync code instead of python-opcua
+Asynchronous programming allows for simpler code (e.g. less need for locks) and can potentially provide performance improvements.
+This library also provides a [synchronous wrapper](https://github.com/FreeOpcUa/opcua-asyncio/blob/master/asyncua/sync.py) over the async API, which can be used in synchronous code instead of python-opcua.
 
 ---
 
-OPC UA binary protocol implementation has been tested against many different OPC UA stacks. API offers both a low level interface to send and receive all UA defined structures and high level classes allowing to write a server or a client in a few lines. It is easy to mix high level objects and low level UA calls in one application. Most low level code is autogenerated from xml specification.
-
-coverage.py reports a test coverage of over 95 % of code, most of non-tested code is autogenerated code that is not used yet.
+The OPC UA binary protocol implementation has undergone extensive testing with various OPC UA stacks. The API offers both a low level interface to send and receive all UA defined structures and high level classes allowing to write a server or a client in a few lines. It is easy to mix high level objects and low level UA calls in one application. Most low level code is autogenerated from xml specification.
 
+The test coverage reported by coverage.py is over 95%, with the majority of the non-tested code being autogenerated code that is not currently in use.
 
 # Warnings
 
-opcua-asyncio is open-source and comes with absolutely no warranty. We try to keep it as much bug-free as possible and try to keep API stable but bugs and API changes will happen! Especially API changes will happen before any 1.0 release.
+opcua-asyncio is open-source and comes with absolutely no warranty. We try to keep it as bug-free as possible, and try to keep the API stable, but bugs and API changes will happen! In particular, API changes are expected to take place prior to any 1.0 release.
 
 Some renaming of methods from get_xx to read_xx and set_xx to write_xxx have been made to better follow OPC UA naming conventions
 
-Version 0.9.9 introduces some argument renaming due to more automatic code generation. Especially the arguments to NodeId, BrowseName, LocalizedText and DataValue are now CamelCase instead of lower case, thus follow the OPC Ua convention used in all other structures in this library
+Version 0.9.9 introduces some argument renaming due to more automatic code generation. Especially the arguments to NodeId, BrowseName, LocalizedText and DataValue, which are now CamelCase instead of lower case, following the OPC UA conventions used in all other structures in this library
 
 # Installation
 
 With pip
 
     pip install asyncua
 
 # Usage
 
 We assume that you already have some experience with Python, the asyncio module, the async / await syntax and the concept of asyncio Tasks.
 
 ## Client class
 
-The `Client` class provides a high level API for connecting to APU UA servers, session management and access to basic
+The `Client` class provides a high level API for connecting to OPC UA servers, session management and access to basic
 address space services.
 The client can be used as a context manager. The client will then automatically connect and disconnect withing the `with`syntax.
 
-
 ```python
 from asyncua import Client
 
 async with Client(url='opc.tcp://localhost:4840/freeopcua/server/') as client:
     while True:
         # Do something with client
         node = client.get_node('i=85')
@@ -69,144 +86,146 @@
 
 The `Server` class provides a high level API for creation of OPC UA server instances.
 
 # Documentation
 
 The documentation is available here [ReadTheDocs](http://opcua-asyncio.readthedocs.org/en/latest/).
 
-The API remains mostly unchanged in regards to [python-opcua](http://opcua-asyncio.rtfd.io/).
-Main difference is that most methods are now async.
+The API remains mostly unchanged with regards to [python-opcua](http://opcua-asyncio.rtfd.io/).
+The main difference is that most methods are now asynchronous.
 Please have a look at [the examples](https://github.com/FreeOpcUa/opcua-asyncio/blob/master/examples) and/or the code.
 
-A simple GUI client is available: https://github.com/FreeOpcUa/opcua-client-gui
+A simple GUI client is available at: https://github.com/FreeOpcUa/opcua-client-gui
 
 Browse the examples: https://github.com/FreeOpcUa/opcua-asyncio/tree/master/examples
 
-A good starting point are the minimal examples.
+The minimal examples are a good starting point.
 Minimal client example: https://github.com/FreeOpcUa/opcua-asyncio/blob/master/examples/client-minimal.py
 Minimal server example: https://github.com/FreeOpcUa/opcua-asyncio/blob/master/examples/server-minimal.py
 
 A set of command line tools also available: https://github.com/FreeOpcUa/opcua-asyncio/tree/master/tools
-* `uadiscover `(find_servers, get_endpoints and find_servers_on_network calls)
-* `uals `(list children of a node)
-* `uahistoryread`
-* `uaread `(read attribute of a node)
-* `uawrite `(write attribute of a node)
-* `uacall `(call method of a node)
-* `uasubscribe `(subscribe to a node and print datachange events)
-* `uaclient `(connect to server and start python shell)
-* `uaserver `(starts a demo OPC UA server)
-  `tools/uaserver --populate --certificate cert.pem --private_key pk.pem`
+
+-   `uadiscover `(find_servers, get_endpoints and find_servers_on_network calls)
+-   `uals `(list children of a node)
+-   `uahistoryread`
+-   `uaread `(read attribute of a node)
+-   `uawrite `(write attribute of a node)
+-   `uacall `(call method of a node)
+-   `uasubscribe `(subscribe to a node and print datachange events)
+-   `uaclient `(connect to server and start python shell)
+-   `uaserver `(starts a demo OPC UA server)
+    `tools/uaserver --populate --certificate cert.pem --private_key pk.pem`
 
 How to generate certificate: https://github.com/FreeOpcUa/opcua-asyncio/tree/master/examples/generate_certificate.sh
 
 ## Client support
 
 What works:
 
-* connection to server, opening channel, session
-* browsing and reading attributes value
-* getting nodes by path and nodeids
-* creating subscriptions
-* subscribing to items for data change
-* subscribing to events
-* adding nodes
-* method call
-* user and password
-* history read
-* login with certificate
-* communication encryption
-* removing nodes
+-   connection to server, opening channel, session
+-   browsing and reading attributes value
+-   getting nodes by path and nodeids
+-   creating subscriptions
+-   subscribing to items for data change
+-   subscribing to events
+-   adding nodes
+-   method call
+-   user and password
+-   history read
+-   login with certificate
+-   communication encryption
+-   removing nodes
 
 Tested servers: freeopcua C++, freeopcua Python, prosys, kepware, beckhoff, winCC, B&R, …
 
 Not implemented yet:
 
-* localized text feature
-* XML protocol
-* UDP (PubSub stuff)
-* WebSocket
-* maybe automatic reconnection...
-
+-   localized text feature
+-   XML protocol
+-   UDP (PubSub stuff)
+-   WebSocket
+-   maybe automatic reconnection...
 
 ## Server support
 
 What works:
 
-* creating channel and sessions
-* read/set attributes and browse
-* getting nodes by path and nodeids
-* autogenerate address space from spec
-* adding nodes to address space
-* datachange events
-* events
-* methods
-* basic user implementation (one existing user called admin, which can be disabled, all others are read only)
-* encryption
-* certificate handling
-* removing nodes
-* history support for data change and events
-* more high level solution to create custom structures
+-   creating channel and sessions
+-   read/set attributes and browse
+-   getting nodes by path and nodeids
+-   autogenerate address space from spec
+-   adding nodes to address space
+-   datachange events
+-   events
+-   methods
+-   basic user implementation (one existing user called admin, which can be disabled, all others are read only)
+-   encryption
+-   certificate handling
+-   removing nodes
+-   history support for data change and events
+-   more high level solution to create custom structures
 
 Tested clients: freeopcua C++, freeopcua Python, uaexpert, prosys, quickopc
 
 Not yet implemented:
 
-* UDP (PubSub stuff)
-* WebSocket
-* session restore
-* alarms
-* XML protocol
-* views
-* localized text features
-* better security model with users and password
-
+-   UDP (PubSub stuff)
+-   WebSocket
+-   session restore
+-   alarms
+-   XML protocol
+-   views
+-   localized text features
+-   better security model with users and password
 
 ### Running a server on a Raspberry Pi
 
 Setting up the standard address-space from XML is the most time-consuming step of the startup process which may lead to
 long startup times on less powerful devices like a Raspberry Pi. By passing a path to a cache-file to the server constructor,
 a shelve holding the address space will be created during the first startup. All following startups will make use of the
 cache-file which leads to significantly better startup performance (~3.5 vs 125 seconds on a Raspberry Pi Model B).
 
-
 # Development
 
 Code follows PEP8 apart for line lengths which should be max 160 characters and OPC UA structures that keep camel case
 from XML definition.
 
 All protocol code is under opcua directory
 
-- `asyncua/ua` contains all UA structures from specification, most are autogenerated
-- `asyncua/common` contains high level objects and methods used both in server and client
-- `asyncua/client` contains client specific code
-- `asyncua/server` contains server specific code
-- `asyncua/utils` contains some utilities function and classes
-- `asyncua/tools` contains code for command lines tools
-- `schemas` contains the XML and text files from specification and the python scripts used to autogenerate code
-- `tests` contains tests
-- `docs` contains files to auto generate documentation from doc strings
-- `examples` contains many example files
-- `examples/sync` contains many example files using sync API
-- `tools` contains python scripts that can be used to run command line tools from repository without installing
+-   `asyncua/ua` contains all UA structures from specification, most are autogenerated
+-   `asyncua/common` contains high level objects and methods used both in server and client
+-   `asyncua/client` contains client specific code
+-   `asyncua/server` contains server specific code
+-   `asyncua/utils` contains some utilities function and classes
+-   `asyncua/tools` contains code for command lines tools
+-   `schemas` contains the XML and text files from specification and the python scripts used to autogenerate code
+-   `tests` contains tests
+-   `docs` contains files to auto generate documentation from doc strings
+-   `examples` contains many example files
+-   `examples/sync` contains many example files using sync API
+-   `tools` contains python scripts that can be used to run command line tools from repository without installing
 
 ## Running tests:
 
 ```
 python -m pip install -r requirements.txt
 python -m pip install -r dev_requirements.txt
 pytest -v -s
 ```
+
 Or
+
 ```
 ./run-test.sh -v -s
 ```
 
 ## Coverage
 
 ```
 pytest -v -s --cov asyncua --cov-report=html
 ```
+
 Or
+
 ```
 ./run-test.sh -v -s --cov asyncua --cov-report=html
 ```
```

### Comparing `asyncua-1.0.2/asyncua/client/client.py` & `asyncua-1.0.3/asyncua/client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -516,19 +516,19 @@
         try:
             while not self._closing:
                 await asyncio.sleep(timeout)
                 # @FIXME handle state change
                 _ = await self.nodes.server_state.read_value()
         except ConnectionError as e:
             _logger.info("connection error in watchdog loop %s", e, exc_info=True)
-            await self.uaclient.inform_subscriptions(ua.StatusCodes.BadShutdown)
+            await self.uaclient.inform_subscriptions(ua.StatusCode(ua.StatusCodes.BadShutdown))
             raise
         except Exception:
             _logger.exception("Error in watchdog loop")
-            await self.uaclient.inform_subscriptions(ua.StatusCodes.BadShutdown)
+            await self.uaclient.inform_subscriptions(ua.StatusCode(ua.StatusCodes.BadShutdown))
             raise
 
     async def _renew_channel_loop(self):
         """
         Renew the SecureChannel before the SecureChannelTimeout will happen.
         In theory, we could do that only if no session activity,
         but it does not cost much.
@@ -750,14 +750,20 @@
             modified_params.RequestedPublishingInterval = (
                 results.RevisedPublishingInterval
             )
             # update LifetimeCount but chances are it will be re-revised again
             modified_params.RequestedLifetimeCount = results.RevisedLifetimeCount
             return modified_params
 
+    async def delete_subscriptions(self, subscription_ids):
+        """
+        Deletes the provided list of subscription_ids
+        """
+        await self.uaclient.delete_subscriptions(subscription_ids)
+
     def get_keepalive_count(self, period) -> int:
         """
         We request the server to send a Keepalive notification when
         no notification has been received for 75% of the session lifetime.
         This is especially useful to keep the session up
         when self.session_timeout < self.secure_channel_timeout.
 
@@ -855,31 +861,39 @@
         await self.uaclient.unregister_nodes(nodeids)
         for node in nodes:
             if not node.basenodeid:
                 continue
             node.nodeid = node.basenodeid
             node.basenodeid = None
 
+    async def read_attributes(self, nodes: List[Node], attr: ua.AttributeIds = ua.AttributeIds.Value):
+        """
+        Read the attributes of multiple nodes.
+        """
+        nodeids = [node.nodeid for node in nodes]
+        return await self.uaclient.read_attributes(nodeids, attr)
+
     async def read_values(self, nodes):
         """
         Read the value of multiple nodes in one ua call.
         """
-        nodeids = [node.nodeid for node in nodes]
-        results = await self.uaclient.read_attributes(nodeids, ua.AttributeIds.Value)
-        return [result.Value.Value for result in results]
+        res = await self.read_attributes(nodes, attr=ua.AttributeIds.Value)
+        return [r.Value.Value for r in res]
 
-    async def write_values(self, nodes, values):
+    async def write_values(self, nodes, values, raise_on_partial_error=True):
         """
         Write values to multiple nodes in one ua call
         """
         nodeids = [node.nodeid for node in nodes]
         dvs = [value_to_datavalue(val) for val in values]
         results = await self.uaclient.write_attributes(nodeids, dvs, ua.AttributeIds.Value)
-        for result in results:
-            result.check()
+        if raise_on_partial_error:
+            for result in results:
+                result.check()
+        return results
 
     get_values = read_values  # legacy compatibility
     set_values = write_values  # legacy compatibility
 
     async def browse_nodes(self, nodes):
         """
         Browses multiple nodes in one ua call
```

### Comparing `asyncua-1.0.2/asyncua/client/ha/common.py` & `asyncua-1.0.3/asyncua/client/ha/common.py`

 * *Files identical despite different names*

### Comparing `asyncua-1.0.2/asyncua/client/ha/ha_client.py` & `asyncua-1.0.3/asyncua/client/ha/ha_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,15 +235,16 @@
         sub_name: str,
         nodes: Union[Iterable[Node], Iterable[str]],
         attr=ua.AttributeIds.Value,
         queuesize=0,
     ) -> None:
 
         async with self._ideal_map_lock:
-            nodes = [n.nodeid.to_string() if isinstance(n, Node) else n for n in nodes]
+            # FIXME: nodeid can be None
+            nodes = [n.nodeid.to_string() if isinstance(n, Node) else n for n in nodes]  # type: ignore[union-attr]
             for url in self.urls:
                 vs = self.ideal_map[url].get(sub_name)
                 if not vs:
                     _logger.warning(
                         f"The subscription specified for the data_change: {sub_name} doesn't exist in ideal_map"
                     )
                     return
@@ -282,16 +283,17 @@
         await client.connect()
 
     async def unsubscribe(self, nodes: Union[Iterable[Node], Iterable[str]]) -> None:
         async with self._ideal_map_lock:
             sub_to_nodes = {}
             first_url = self.urls[0]
             for sub_name, vs in self.ideal_map[first_url].items():
+                # FIXME: nodeid can be None
                 node_set = {
-                    n.nodeid.to_string() if isinstance(n, Node) else n for n in nodes
+                    n.nodeid.to_string() if isinstance(n, Node) else n for n in nodes  # type: ignore[union-attr]
                 }
                 to_del = node_set & vs.get_nodes()
                 if to_del:
                     sub_to_nodes[sub_name] = to_del
             for url in self.urls:
                 for sub_name, str_nodes in sub_to_nodes.items():
                     vs = self.ideal_map[url][sub_name]
```

### Comparing `asyncua-1.0.2/asyncua/client/ha/reconciliator.py` & `asyncua-1.0.3/asyncua/client/ha/reconciliator.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 import time
 
 from collections import defaultdict
 from dataclasses import astuple
 from enum import Enum
 from functools import partial
-from typing import TYPE_CHECKING, Dict, Set, Union, List, Optional
+from typing import TYPE_CHECKING, Dict, Set, Union, List
 from sortedcontainers import SortedDict  # type: ignore
 from asyncua import ua, Client
 from pickle import PicklingError
 
 from .common import batch, event_wait, get_digest
 from .virtual_subscription import VirtualSubscription
```

### Comparing `asyncua-1.0.2/asyncua/client/ha/virtual_subscription.py` & `asyncua-1.0.3/asyncua/client/ha/virtual_subscription.py`

 * *Files identical despite different names*

### Comparing `asyncua-1.0.2/asyncua/client/ua_client.py` & `asyncua-1.0.3/asyncua/client/ua_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Low level binary client
 """
 import asyncio
 import copy
 import logging
-from typing import Awaitable, Callable, Dict, List, Optional, Union
+from typing import Awaitable, Callable, Dict, List, Optional, Union, Coroutine, Any
 
 from asyncua import ua
 from asyncua.common.session_interface import AbstractSession
 from ..ua.ua_binary import struct_from_binary, uatcp_to_binary, struct_to_binary, nodeid_from_binary, header_from_binary
 from ..ua.uaerrors import BadTimeout, BadNoSubscription, BadSessionClosed, BadUserAccessDenied, UaStructParsingError
 from ..common.connection import SecureConnection, TransportLimits
 
@@ -35,15 +35,15 @@
         self.authentication_token = ua.NodeId()
         self._request_id = 0
         self._request_handle = 0
         self._callbackmap: Dict[int, asyncio.Future] = {}
         if limits is None:
             limits = TransportLimits(65535, 65535, 0, 0)
         else:
-            limits = copy.deep_copy(limits)  # Make a copy because the limits can change in the session
+            limits = copy.deepcopy(limits)  # Make a copy because the limits can change in the session
         self._connection = SecureConnection(security_policy, limits)
 
         self.state = self.INITIALIZED
         self.closed: bool = False
         # needed to pass params from asynchronous request to synchronous data receive callback, as well as
         # passing back the processed response to the request so that it can return it.
         self._open_secure_channel_exchange: Union[ua.OpenSecureChannelResponse, ua.OpenSecureChannelParameters, None] = None
@@ -272,27 +272,27 @@
 
     def _make_protocol(self):
         self.protocol = UASocketProtocol(self._timeout, security_policy=self.security_policy)
         self.protocol.pre_request_hook = self._pre_request_hook
         return self.protocol
 
     @property
-    def pre_request_hook(self) -> Callable[[], Awaitable[None]]:
+    def pre_request_hook(self) -> Optional[Callable[[], Awaitable[None]]]:
         return self._pre_request_hook
 
     @pre_request_hook.setter
     def pre_request_hook(self, hook: Optional[Callable[[], Awaitable[None]]]):
         self._pre_request_hook = hook
         if self.protocol:
             self.protocol.pre_request_hook = self._pre_request_hook
 
     async def connect_socket(self, host: str, port: int):
         """Connect to server socket."""
         self.logger.info("opening connection")
-        self._closing: bool = False
+        self._closing = False
         # Timeout the connection when the server isn't available
         await asyncio.wait_for(asyncio.get_running_loop().create_connection(self._make_protocol, host, port), self._timeout)
 
     def disconnect_socket(self):
         if not self.protocol:
             return
         if self.protocol and self.protocol.state == UASocketProtocol.CLOSED:
@@ -486,17 +486,17 @@
         request.Parameters.BrowsePaths = browse_paths
         data = await self.protocol.send_request(request)
         response = struct_from_binary(ua.TranslateBrowsePathsToNodeIdsResponse, data)
         self.logger.debug(response)
         response.ResponseHeader.ServiceResult.check()
         return response.Results
 
-    async def create_subscription(
-        self, params, callback
-    ) -> ua.CreateSubscriptionResult:
+    async def create_subscription(   # type: ignore[override]
+        self, params: ua.CreateSubscriptionParameters, callback
+    ) -> Coroutine[Any, Any, ua.CreateSubscriptionResult]:
         self.logger.debug("create_subscription")
         request = ua.CreateSubscriptionRequest()
         request.Parameters = params
         data = await self.protocol.send_request(request)
         response = struct_from_binary(ua.CreateSubscriptionResponse, data)
         response.ResponseHeader.ServiceResult.check()
         self._subscription_callbacks[response.Parameters.SubscriptionId] = callback
@@ -513,15 +513,15 @@
         return response.Parameters
 
     async def inform_subscriptions(self, status: ua.StatusCode):
         """
             Inform all current subscriptions with a status code. This calls the handler's status_change_notification
         """
         status_message = ua.StatusChangeNotification(Status=status)
-        notification_message = ua.NotificationMessage(NotificationData=[status_message])
+        notification_message = ua.NotificationMessage(NotificationData=[status_message])  # type: ignore[list-item]
         for subid, callback in self._subscription_callbacks.items():
             try:
                 parameters = ua.PublishResult(
                     subid,
                     NotificationMessage_=notification_message
                 )
                 if asyncio.iscoroutinefunction(callback):
```

### Comparing `asyncua-1.0.2/asyncua/client/ua_file.py` & `asyncua-1.0.3/asyncua/client/ua_file.py`

 * *Files identical despite different names*

### Comparing `asyncua-1.0.2/asyncua/client/ua_file_transfer.py` & `asyncua-1.0.3/asyncua/client/ua_file_transfer.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,18 +5,20 @@
 
 See also:
 OPC 10000-5: OPC Unified Architecture V1.04
 Part 5: Information Model - Annex C (normative) File Transfer
 https://reference.opcfoundation.org/Core/docs/Part5/C.1/
 """
 import logging
+from typing import Tuple
 
 from asyncua.common.node import Node
 from asyncua.ua import NodeId, OpenFileMode, Variant, VariantType 
 
+
 _logger = logging.getLogger(__name__)
 
 
 class UaFile:
     """
     Provides the functionality to work with "C.2 FileType".
     """
@@ -190,15 +192,15 @@
         :return: The NodeId of the created directory Object.
         """
         _logger.debug("Request to create directory %s in %s", directory_name, self._directory_node)
         create_directory_node = await self._directory_node.get_child("CreateDirectory")
         arg1_directory_name = Variant(directory_name, VariantType.String)
         return await self._directory_node.call_method(create_directory_node, arg1_directory_name)
 
-    async def create_file(self, file_name: str, request_file_open: bool) -> [NodeId, int]:
+    async def create_file(self, file_name: str, request_file_open: bool) -> Tuple[NodeId, int]:
         """
         CreateFile is used to create a new FileType Object organized by this Object.
         The created file can be written using the Write Method of the FileType.
         :param file_name: The name of the file to create. The name is used for the
         BrowseName and DisplayName of the file object and also for the file in the
         file system.
         For the BrowseName, the fileName is used for the name part of the QualifiedName.
```

### Comparing `asyncua-1.0.2/asyncua/common/callback.py` & `asyncua-1.0.3/asyncua/common/callback.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-server side implementation of callback event 
+server side implementation of callback event
 """
 
 from collections import OrderedDict
 from enum import Enum
 import asyncio
 
 
@@ -80,17 +80,17 @@
 
     def removeListener(self, eventName, listener=None):
         if eventName not in self._listeners:
             return
         if not listener:
             del self._listeners[eventName]
         else:
-            for p, l in self._listeners[eventName].items():
-                if l is listener:
-                    self._listeners[eventName].pop(p)
+            for name, mylistener in self._listeners[eventName].items():
+                if mylistener is listener:
+                    self._listeners[eventName].pop(name)
                     return
 
     def addSubscriber(self, subscriber):
         if not isinstance(subscriber, CallbackSubscriberInterface):
             raise ValueError('Unexpected subscriber type given')
         for eventName, params in subscriber.getSubscribedEvents().items():
             if isinstance(params, str):
```

### Comparing `asyncua-1.0.2/asyncua/common/connection.py` & `asyncua-1.0.3/asyncua/common/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,14 +64,15 @@
         return ack
 
     def create_hello_limits(self, msg: ua.Hello) -> ua.Hello:
         msg.ReceiveBufferSize = self.max_recv_buffer
         msg.SendBufferSize = self.max_send_buffer
         msg.MaxChunkCount = self.max_chunk_count
         msg.MaxMessageSize = self.max_chunk_count
+        return msg
 
     def update_client_limits(self, msg: ua.Acknowledge) -> None:
         self.max_chunk_count = msg.MaxChunkCount
         self.max_recv_buffer = msg.ReceiveBufferSize
         self.max_send_buffer = msg.SendBufferSize
         self.max_message_size = msg.MaxMessageSize
         _logger.info("updating client limits to: %s", self)
```

### Comparing `asyncua-1.0.2/asyncua/common/copy_node_util.py` & `asyncua-1.0.3/asyncua/common/copy_node_util.py`

 * *Files identical despite different names*

### Comparing `asyncua-1.0.2/asyncua/common/event_objects.py` & `asyncua-1.0.3/asyncua/common/event_objects.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 Autogenerated code from xml"
 
 Model Uri:http://opcfoundation.org/UA/"
 Version:1.05.01"
 Publication date:2022-02-24T00:00:00Z"
 
-File creation Date:2022-09-22 16:18:40.843698"
+File creation Date:2023-07-25 09:08:45.084676"
 """
 from asyncua import ua
 from .events import Event
 
 
 __all__ = ["BaseEvent", "AuditEvent", "AuditSecurityEvent", "AuditChannelEvent", "AuditOpenSecureChannelEvent", "AuditSessionEvent", "AuditCreateSessionEvent", "AuditActivateSessionEvent", "AuditCancelEvent", "AuditCertificateEvent", "AuditCertificateDataMismatchEvent", "AuditCertificateExpiredEvent", "AuditCertificateInvalidEvent", "AuditCertificateUntrustedEvent", "AuditCertificateRevokedEvent", "AuditCertificateMismatchEvent", "AuditNodeManagementEvent", "AuditAddNodesEvent", "AuditDeleteNodesEvent", "AuditAddReferencesEvent", "AuditDeleteReferencesEvent", "AuditUpdateEvent", "AuditWriteUpdateEvent", "AuditHistoryUpdateEvent", "AuditUpdateMethodEvent", "SystemEvent", "DeviceFailureEvent", "BaseModelChangeEvent", "GeneralModelChangeEvent", "TransitionEvent", "AuditUpdateStateEvent", "ProgramTransitionEvent", "SemanticChangeEvent", "AuditUrlMismatchEvent", "Condition", "RefreshStartEvent", "RefreshEndEvent", "RefreshRequiredEvent", "AuditConditionEvent", "AuditConditionEnableEvent", "AuditConditionCommentEvent", "DialogCondition", "AcknowledgeableCondition", "AlarmCondition", "LimitAlarm", "AuditHistoryEventUpdateEvent", "AuditHistoryValueUpdateEvent", "AuditHistoryDeleteEvent", "AuditHistoryRawModifyDeleteEvent", "AuditHistoryAtTimeDeleteEvent", "AuditHistoryEventDeleteEvent", "EventQueueOverflowEvent", "ProgramTransitionAuditEvent", "AuditConditionRespondEvent", "AuditConditionAcknowledgeEvent", "AuditConditionConfirmEvent", "ExclusiveLimitAlarm", "ExclusiveLevelAlarm", "ExclusiveRateOfChangeAlarm", "ExclusiveDeviationAlarm", "NonExclusiveLimitAlarm", "NonExclusiveLevelAlarm", "NonExclusiveRateOfChangeAlarm", "NonExclusiveDeviationAlarm", "DiscreteAlarm", "OffNormalAlarm", "TripAlarm", "AuditConditionShelvingEvent", "ProgressEvent", "SystemStatusChangeEvent", "SystemOffNormalAlarm", "AuditProgramTransitionEvent", "TrustListUpdatedAuditEvent", "CertificateUpdatedAuditEvent", "CertificateExpirationAlarm", "AuditConditionResetEvent", "PubSubStatusEvent", "PubSubTransportLimitsExceedEvent", "PubSubCommunicationFailureEvent", "DiscrepancyAlarm", "AuditConditionSuppressionEvent", "AuditConditionSilenceEvent", "AuditConditionOutOfServiceEvent", "RoleMappingRuleChangedAuditEvent", "KeyCredentialAuditEvent", "KeyCredentialUpdatedAuditEvent", "KeyCredentialDeletedAuditEvent", "InstrumentDiagnosticAlarm", "SystemDiagnosticAlarm", "AuditHistoryAnnotationUpdateEvent", "TrustListOutOfDateAlarm", "AuditClientEvent", "AuditClientUpdateMethodResultEvent"]
 
@@ -86,15 +86,15 @@
 class AuditSessionEvent(AuditSecurityEvent):
     """
     AuditSessionEvent:
     """
     def __init__(self, sourcenode=None, message=None, severity=1):
         super().__init__(sourcenode, message, severity)
         self.EventType = ua.NodeId(ua.ObjectIds.AuditSessionEventType)
-        self.add_property('SessionId', ua.NodeId(ua.ObjectIds.AuditSessionEventType), ua.VariantType.NodeId)
+        self.add_property('SessionId', None, ua.VariantType.NodeId)
 
 
 class AuditCreateSessionEvent(AuditSessionEvent):
     """
     AuditCreateSessionEvent:
     """
     def __init__(self, sourcenode=None, message=None, severity=1):
@@ -268,25 +268,25 @@
 class AuditHistoryUpdateEvent(AuditUpdateEvent):
     """
     AuditHistoryUpdateEvent:
     """
     def __init__(self, sourcenode=None, message=None, severity=1):
         super().__init__(sourcenode, message, severity)
         self.EventType = ua.NodeId(ua.ObjectIds.AuditHistoryUpdateEventType)
-        self.add_property('ParameterDataTypeId', ua.NodeId(ua.ObjectIds.AuditHistoryUpdateEventType), ua.VariantType.NodeId)
+        self.add_property('ParameterDataTypeId', None, ua.VariantType.NodeId)
 
 
 class AuditUpdateMethodEvent(AuditEvent):
     """
     AuditUpdateMethodEvent:
     """
     def __init__(self, sourcenode=None, message=None, severity=1):
         super().__init__(sourcenode, message, severity)
         self.EventType = ua.NodeId(ua.ObjectIds.AuditUpdateMethodEventType)
-        self.add_property('MethodId', ua.NodeId(ua.ObjectIds.AuditUpdateMethodEventType), ua.VariantType.NodeId)
+        self.add_property('MethodId', None, ua.VariantType.NodeId)
         self.add_property('InputArguments', None, ua.VariantType.Variant)
 
 
 class SystemEvent(BaseEvent):
     """
     SystemEvent:
     """
@@ -382,20 +382,20 @@
 class Condition(BaseEvent):
     """
     Condition:
     """
     def __init__(self, sourcenode=None, message=None, severity=1):
         super().__init__(sourcenode, message, severity)
         self.EventType = ua.NodeId(ua.ObjectIds.ConditionType)
-        self.add_property('ConditionClassId', ua.NodeId(ua.ObjectIds.ConditionType), ua.VariantType.NodeId)
+        self.add_property('ConditionClassId', None, ua.VariantType.NodeId)
         self.add_property('ConditionClassName', None, ua.VariantType.LocalizedText)
-        self.add_property('ConditionSubClassId', ua.NodeId(ua.ObjectIds.ConditionType), ua.VariantType.NodeId)
+        self.add_property('ConditionSubClassId', None, ua.VariantType.NodeId)
         self.add_property('ConditionSubClassName', None, ua.VariantType.LocalizedText)
         self.add_property('ConditionName', None, ua.VariantType.String)
-        self.add_property('BranchId', ua.NodeId(ua.ObjectIds.ConditionType), ua.VariantType.NodeId)
+        self.add_property('BranchId', None, ua.VariantType.NodeId)
         self.add_property('Retain', None, ua.VariantType.Boolean)
         self.add_property('EnabledState/Id', None, ua.VariantType.Boolean)
         self.add_property('EnabledState/EffectiveDisplayName', None, ua.VariantType.LocalizedText)
         self.add_property('EnabledState/TransitionTime', None, ua.NodeId(ua.ObjectIds.UtcTime))
         self.add_property('EnabledState/EffectiveTransitionTime', None, ua.NodeId(ua.ObjectIds.UtcTime))
         self.add_property('EnabledState/TrueState', None, ua.VariantType.LocalizedText)
         self.add_property('EnabledState/FalseState', None, ua.VariantType.LocalizedText)
@@ -520,15 +520,15 @@
         self.add_property('ActiveState/Id', None, ua.VariantType.Boolean)
         self.add_property('ActiveState/EffectiveDisplayName', None, ua.VariantType.LocalizedText)
         self.add_property('ActiveState/TransitionTime', None, ua.NodeId(ua.ObjectIds.UtcTime))
         self.add_property('ActiveState/EffectiveTransitionTime', None, ua.NodeId(ua.ObjectIds.UtcTime))
         self.add_property('ActiveState/TrueState', None, ua.VariantType.LocalizedText)
         self.add_property('ActiveState/FalseState', None, ua.VariantType.LocalizedText)
         self.add_variable('ActiveState', None, ua.VariantType.LocalizedText)
-        self.add_property('InputNode', ua.NodeId(ua.ObjectIds.AlarmConditionType), ua.VariantType.NodeId)
+        self.add_property('InputNode', None, ua.VariantType.NodeId)
         self.add_property('SuppressedState/Id', None, ua.VariantType.Boolean)
         self.add_property('SuppressedState/TransitionTime', None, ua.NodeId(ua.ObjectIds.UtcTime))
         self.add_property('SuppressedState/TrueState', None, ua.VariantType.LocalizedText)
         self.add_property('SuppressedState/FalseState', None, ua.VariantType.LocalizedText)
         self.add_variable('SuppressedState', None, ua.VariantType.LocalizedText)
         self.add_property('OutOfServiceState/Id', None, ua.VariantType.Boolean)
         self.add_property('OutOfServiceState/TransitionTime', None, ua.NodeId(ua.ObjectIds.UtcTime))
@@ -584,42 +584,42 @@
 class AuditHistoryEventUpdateEvent(AuditHistoryUpdateEvent):
     """
     AuditHistoryEventUpdateEvent:
     """
     def __init__(self, sourcenode=None, message=None, severity=1):
         super().__init__(sourcenode, message, severity)
         self.EventType = ua.NodeId(ua.ObjectIds.AuditHistoryEventUpdateEventType)
-        self.add_property('UpdatedNode', ua.NodeId(ua.ObjectIds.AuditHistoryEventUpdateEventType), ua.VariantType.NodeId)
+        self.add_property('UpdatedNode', None, ua.VariantType.NodeId)
         self.add_property('PerformInsertReplace', None, ua.NodeId(ua.ObjectIds.PerformUpdateType))
         self.add_property('Filter', None, ua.NodeId(ua.ObjectIds.EventFilter))
         self.add_property('NewValues', None, ua.NodeId(ua.ObjectIds.HistoryEventFieldList))
         self.add_property('OldValues', None, ua.NodeId(ua.ObjectIds.HistoryEventFieldList))
 
 
 class AuditHistoryValueUpdateEvent(AuditHistoryUpdateEvent):
     """
     AuditHistoryValueUpdateEvent:
     """
     def __init__(self, sourcenode=None, message=None, severity=1):
         super().__init__(sourcenode, message, severity)
         self.EventType = ua.NodeId(ua.ObjectIds.AuditHistoryValueUpdateEventType)
-        self.add_property('UpdatedNode', ua.NodeId(ua.ObjectIds.AuditHistoryValueUpdateEventType), ua.VariantType.NodeId)
+        self.add_property('UpdatedNode', None, ua.VariantType.NodeId)
         self.add_property('PerformInsertReplace', None, ua.NodeId(ua.ObjectIds.PerformUpdateType))
         self.add_property('NewValues', None, ua.NodeId(ua.ObjectIds.DataValue))
         self.add_property('OldValues', None, ua.NodeId(ua.ObjectIds.DataValue))
 
 
 class AuditHistoryDeleteEvent(AuditHistoryUpdateEvent):
     """
     AuditHistoryDeleteEvent:
     """
     def __init__(self, sourcenode=None, message=None, severity=1):
         super().__init__(sourcenode, message, severity)
         self.EventType = ua.NodeId(ua.ObjectIds.AuditHistoryDeleteEventType)
-        self.add_property('UpdatedNode', ua.NodeId(ua.ObjectIds.AuditHistoryDeleteEventType), ua.VariantType.NodeId)
+        self.add_property('UpdatedNode', None, ua.VariantType.NodeId)
 
 
 class AuditHistoryRawModifyDeleteEvent(AuditHistoryDeleteEvent):
     """
     AuditHistoryRawModifyDeleteEvent:
     """
     def __init__(self, sourcenode=None, message=None, severity=1):
@@ -665,15 +665,15 @@
 class ProgramTransitionAuditEvent(AuditUpdateStateEvent):
     """
     ProgramTransitionAuditEvent:
     """
     def __init__(self, sourcenode=None, message=None, severity=1):
         super().__init__(sourcenode, message, severity)
         self.EventType = ua.NodeId(ua.ObjectIds.ProgramTransitionAuditEventType)
-        self.add_property('Transition/Id', ua.NodeId(ua.ObjectIds.ProgramTransitionAuditEventType), ua.VariantType.NodeId)
+        self.add_property('Transition/Id', None, ua.VariantType.NodeId)
         self.add_variable('Transition', None, ua.VariantType.LocalizedText)
 
 
 class AuditConditionRespondEvent(AuditConditionEvent):
     """
     AuditConditionRespondEvent:
     """
@@ -738,16 +738,16 @@
 class ExclusiveDeviationAlarm(ExclusiveLimitAlarm):
     """
     ExclusiveDeviationAlarm:
     """
     def __init__(self, sourcenode=None, message=None, severity=1):
         super().__init__(sourcenode, message, severity)
         self.EventType = ua.NodeId(ua.ObjectIds.ExclusiveDeviationAlarmType)
-        self.add_property('SetpointNode', ua.NodeId(ua.ObjectIds.ExclusiveDeviationAlarmType), ua.VariantType.NodeId)
-        self.add_property('BaseSetpointNode', ua.NodeId(ua.ObjectIds.ExclusiveDeviationAlarmType), ua.VariantType.NodeId)
+        self.add_property('SetpointNode', None, ua.VariantType.NodeId)
+        self.add_property('BaseSetpointNode', None, ua.VariantType.NodeId)
 
 
 class NonExclusiveLimitAlarm(LimitAlarm):
     """
     NonExclusiveLimitAlarm:
     """
     def __init__(self, sourcenode=None, message=None, severity=1):
@@ -799,16 +799,16 @@
 class NonExclusiveDeviationAlarm(NonExclusiveLimitAlarm):
     """
     NonExclusiveDeviationAlarm:
     """
     def __init__(self, sourcenode=None, message=None, severity=1):
         super().__init__(sourcenode, message, severity)
         self.EventType = ua.NodeId(ua.ObjectIds.NonExclusiveDeviationAlarmType)
-        self.add_property('SetpointNode', ua.NodeId(ua.ObjectIds.NonExclusiveDeviationAlarmType), ua.VariantType.NodeId)
-        self.add_property('BaseSetpointNode', ua.NodeId(ua.ObjectIds.NonExclusiveDeviationAlarmType), ua.VariantType.NodeId)
+        self.add_property('SetpointNode', None, ua.VariantType.NodeId)
+        self.add_property('BaseSetpointNode', None, ua.VariantType.NodeId)
 
 
 class DiscreteAlarm(AlarmCondition):
     """
     DiscreteAlarm:
     """
     def __init__(self, sourcenode=None, message=None, severity=1):
@@ -819,15 +819,15 @@
 class OffNormalAlarm(DiscreteAlarm):
     """
     OffNormalAlarm:
     """
     def __init__(self, sourcenode=None, message=None, severity=1):
         super().__init__(sourcenode, message, severity)
         self.EventType = ua.NodeId(ua.ObjectIds.OffNormalAlarmType)
-        self.add_property('NormalState', ua.NodeId(ua.ObjectIds.OffNormalAlarmType), ua.VariantType.NodeId)
+        self.add_property('NormalState', None, ua.VariantType.NodeId)
 
 
 class TripAlarm(OffNormalAlarm):
     """
     TripAlarm:
     """
     def __init__(self, sourcenode=None, message=None, severity=1):
@@ -897,28 +897,28 @@
 class CertificateUpdatedAuditEvent(AuditUpdateMethodEvent):
     """
     CertificateUpdatedAuditEvent:
     """
     def __init__(self, sourcenode=None, message=None, severity=1):
         super().__init__(sourcenode, message, severity)
         self.EventType = ua.NodeId(ua.ObjectIds.CertificateUpdatedAuditEventType)
-        self.add_property('CertificateGroup', ua.NodeId(ua.ObjectIds.CertificateUpdatedAuditEventType), ua.VariantType.NodeId)
-        self.add_property('CertificateType', ua.NodeId(ua.ObjectIds.CertificateUpdatedAuditEventType), ua.VariantType.NodeId)
+        self.add_property('CertificateGroup', None, ua.VariantType.NodeId)
+        self.add_property('CertificateType', None, ua.VariantType.NodeId)
 
 
 class CertificateExpirationAlarm(SystemOffNormalAlarm):
     """
     CertificateExpirationAlarm:
     """
     def __init__(self, sourcenode=None, message=None, severity=1):
         super().__init__(sourcenode, message, severity)
         self.EventType = ua.NodeId(ua.ObjectIds.CertificateExpirationAlarmType)
         self.add_property('ExpirationDate', None, ua.VariantType.DateTime)
         self.add_property('ExpirationLimit', None, ua.NodeId(ua.ObjectIds.Duration))
-        self.add_property('CertificateType', ua.NodeId(ua.ObjectIds.CertificateExpirationAlarmType), ua.VariantType.NodeId)
+        self.add_property('CertificateType', None, ua.VariantType.NodeId)
         self.add_property('Certificate', None, ua.VariantType.ByteString)
 
 
 class AuditConditionResetEvent(AuditConditionEvent):
     """
     AuditConditionResetEvent:
     """
@@ -930,16 +930,16 @@
 class PubSubStatusEvent(SystemEvent):
     """
     PubSubStatusEvent:
     """
     def __init__(self, sourcenode=None, message=None, severity=1):
         super().__init__(sourcenode, message, severity)
         self.EventType = ua.NodeId(ua.ObjectIds.PubSubStatusEventType)
-        self.add_property('ConnectionId', ua.NodeId(ua.ObjectIds.PubSubStatusEventType), ua.VariantType.NodeId)
-        self.add_property('GroupId', ua.NodeId(ua.ObjectIds.PubSubStatusEventType), ua.VariantType.NodeId)
+        self.add_property('ConnectionId', None, ua.VariantType.NodeId)
+        self.add_property('GroupId', None, ua.VariantType.NodeId)
         self.add_property('State', None, ua.NodeId(ua.ObjectIds.PubSubState))
 
 
 class PubSubTransportLimitsExceedEvent(PubSubStatusEvent):
     """
     PubSubTransportLimitsExceedEvent:
     """
@@ -963,15 +963,15 @@
 class DiscrepancyAlarm(AlarmCondition):
     """
     DiscrepancyAlarm:
     """
     def __init__(self, sourcenode=None, message=None, severity=1):
         super().__init__(sourcenode, message, severity)
         self.EventType = ua.NodeId(ua.ObjectIds.DiscrepancyAlarmType)
-        self.add_property('TargetValueNode', ua.NodeId(ua.ObjectIds.DiscrepancyAlarmType), ua.VariantType.NodeId)
+        self.add_property('TargetValueNode', None, ua.VariantType.NodeId)
         self.add_property('ExpectedTime', None, ua.NodeId(ua.ObjectIds.Duration))
         self.add_property('Tolerance', None, ua.VariantType.Double)
 
 
 class AuditConditionSuppressionEvent(AuditConditionEvent):
     """
     AuditConditionSuppressionEvent:
@@ -1070,15 +1070,15 @@
 class TrustListOutOfDateAlarm(SystemOffNormalAlarm):
     """
     TrustListOutOfDateAlarm:
     """
     def __init__(self, sourcenode=None, message=None, severity=1):
         super().__init__(sourcenode, message, severity)
         self.EventType = ua.NodeId(ua.ObjectIds.TrustListOutOfDateAlarmType)
-        self.add_property('TrustListId', ua.NodeId(ua.ObjectIds.TrustListOutOfDateAlarmType), ua.VariantType.NodeId)
+        self.add_property('TrustListId', None, ua.VariantType.NodeId)
         self.add_property('LastUpdateTime', None, ua.NodeId(ua.ObjectIds.UtcTime))
         self.add_property('UpdateFrequency', None, ua.NodeId(ua.ObjectIds.Duration))
 
 
 class AuditClientEvent(AuditEvent):
     """
     AuditClientEvent:
@@ -1092,16 +1092,16 @@
 class AuditClientUpdateMethodResultEvent(AuditClientEvent):
     """
     AuditClientUpdateMethodResultEvent:
     """
     def __init__(self, sourcenode=None, message=None, severity=1):
         super().__init__(sourcenode, message, severity)
         self.EventType = ua.NodeId(ua.ObjectIds.AuditClientUpdateMethodResultEventType)
-        self.add_property('ObjectId', ua.NodeId(ua.ObjectIds.AuditClientUpdateMethodResultEventType), ua.VariantType.NodeId)
-        self.add_property('MethodId', ua.NodeId(ua.ObjectIds.AuditClientUpdateMethodResultEventType), ua.VariantType.NodeId)
+        self.add_property('ObjectId', None, ua.VariantType.NodeId)
+        self.add_property('MethodId', None, ua.VariantType.NodeId)
         self.add_property('StatusCodeId', None, ua.VariantType.StatusCode)
         self.add_property('InputArguments', None, ua.NodeId(ua.ObjectIds.Argument))
         self.add_property('OutputArguments', None, ua.NodeId(ua.ObjectIds.Argument))
 
 
 IMPLEMENTED_EVENTS = {
     ua.ObjectIds.BaseEventType: BaseEvent,
```

### Comparing `asyncua-1.0.2/asyncua/common/events.py` & `asyncua-1.0.3/asyncua/common/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import copy
 from typing import Dict, List, TYPE_CHECKING
 from asyncua import ua
 import asyncua
 from ..ua.uaerrors import UaError
-from .ua_utils import get_node_subtypes
+from .ua_utils import get_node_subtypes, is_subtype
 if TYPE_CHECKING:
     from asyncua.common.node import Node
 
 
 _BROWSE_MASK =  ua.BrowseResultMask.NodeClass |  ua.BrowseResultMask.ReferenceTypeId |  ua.BrowseResultMask.BrowseName
 
 
@@ -174,18 +174,27 @@
             refs = await obj.get_references(ua.ObjectIds.Aggregates, ua.BrowseDirection.Forward, ua.NodeClass.Object | ua.NodeClass.Variable, True, _BROWSE_MASK)
             await _select_clause_from_childs(obj, refs, select_clauses, already_selected, browse_path + [ref.BrowseName])
 
 
 async def select_clauses_from_evtype(evtypes: List["Node"]):
     select_clauses = []
     already_selected = {}
+    add_condition_id = False
     for evtype in evtypes:
+        if not add_condition_id and await is_subtype(evtype, ua.NodeId(ua.ObjectIds.ConditionType)):
+            add_condition_id = True
         refs = await select_event_attributes_from_type_node(evtype, lambda n: n.get_references(ua.ObjectIds.Aggregates, ua.BrowseDirection.Forward, ua.NodeClass.Object | ua.NodeClass.Variable, True, _BROWSE_MASK))
         if refs:
             await _select_clause_from_childs(evtype, refs, select_clauses, already_selected, [])
+    if add_condition_id:
+        # also request ConditionId, which is not modelled as a component of the ConditionType
+        op = ua.SimpleAttributeOperand()
+        op.AttributeId = ua.AttributeIds.NodeId
+        op.TypeDefinitionId = ua.NodeId(ua.ObjectIds.ConditionType)
+        select_clauses.append(op)
     return select_clauses
 
 
 async def where_clause_from_evtype(evtypes: List["Node"]):
     cf = ua.ContentFilter()
     el = ua.ContentFilterElement()
     # operands can be ElementOperand, LiteralOperand, AttributeOperand, SimpleAttribute
```

### Comparing `asyncua-1.0.2/asyncua/common/instantiate_util.py` & `asyncua-1.0.3/asyncua/common/instantiate_util.py`

 * *Files identical despite different names*

### Comparing `asyncua-1.0.2/asyncua/common/manage_nodes.py` & `asyncua-1.0.3/asyncua/common/manage_nodes.py`

 * *Files identical despite different names*

### Comparing `asyncua-1.0.2/asyncua/common/methods.py` & `asyncua-1.0.3/asyncua/common/methods.py`

 * *Files identical despite different names*

### Comparing `asyncua-1.0.2/asyncua/common/node.py` & `asyncua-1.0.3/asyncua/common/node.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     browse and populate address space.
     Node objects are useful as-is but they do not expose the entire
     OPC-UA protocol. Feel free to look at the code of this class and call
     directly UA services methods to optimize your code
     """
     def __init__(self, session: AbstractSession, nodeid: Union[ua.NodeId, str, int]):
         self.session = session
-        self.nodeid = None
+        self.nodeid: ua.NodeId
         if isinstance(nodeid, Node):
             self.nodeid = nodeid.nodeid
         elif isinstance(nodeid, ua.NodeId):
             self.nodeid = nodeid
         elif type(nodeid) in (str, bytes):
             self.nodeid = ua.NodeId.from_string(nodeid)
         elif isinstance(nodeid, int):
@@ -504,14 +504,47 @@
         result = await self.session.translate_browsepaths_to_nodeids([bpath])
         result = result[0]
         result.StatusCode.check()
         if return_all:
             return [Node(self.session, target.TargetId) for target in result.Targets]
         return Node(self.session, result.Targets[0].TargetId)
 
+    async def get_children_by_path(self, paths, raise_on_partial_error=True):
+        """
+        get children specified by their paths from this node.
+        A path might be:
+        * a string representing a qualified name.
+        * a qualified name
+        * a list of string
+        * a list of qualified names
+        """
+        bpaths = []
+        for path in paths:
+            if type(path) not in (list, tuple):
+                path = [path]
+            rpath = self._make_relative_path(path)
+            bpath = ua.BrowsePath()
+            bpath.StartingNode = self.nodeid
+            bpath.RelativePath = rpath
+            bpaths.append(bpath)
+
+        results = await self.session.translate_browsepaths_to_nodeids(bpaths)
+        try:
+            if raise_on_partial_error:
+                for result in results:
+                    result.StatusCode.check()
+        except ua.UaStatusCodeError:
+            codes = [result.StatusCode.value for result in results]
+            raise ua.UaStatusCodeErrors(codes)
+        return [
+            [Node(self.session, target.TargetId) for target in result.Targets]
+            if result.StatusCode.is_good() else None
+            for result in results
+        ]
+
     def _make_relative_path(self, path):
         rpath = ua.RelativePath()
         for item in path:
             el = ua.RelativePathElement()
             el.ReferenceTypeId = ua.TwoByteNodeId(ua.ObjectIds.HierarchicalReferences)
             el.IsInverse = False
             el.IncludeSubtypes = True
@@ -547,15 +580,17 @@
             result = await self.history_read(details, continuation_point)
             result.StatusCode.check()
             continuation_point = result.ContinuationPoint
             history.extend(result.HistoryData.DataValues)
             # No more data available
             if continuation_point is None:
                 break
-
+            # No more data needed
+            if numvalues > 0:
+                break
         return history
 
     async def history_read(self, details, continuation_point=None):
         """
         Read raw history of a node, low-level function
         result code from server is checked and an exception is raised in case of error
         """
```

### Comparing `asyncua-1.0.2/asyncua/common/session_interface.py` & `asyncua-1.0.3/asyncua/common/session_interface.py`

 * *Files identical despite different names*

### Comparing `asyncua-1.0.2/asyncua/common/shortcuts.py` & `asyncua-1.0.3/asyncua/common/shortcuts.py`

 * *Files identical despite different names*

### Comparing `asyncua-1.0.2/asyncua/common/sql_injection.py` & `asyncua-1.0.3/asyncua/common/sql_injection.py`

 * *Files identical despite different names*

### Comparing `asyncua-1.0.2/asyncua/common/statemachine.py` & `asyncua-1.0.3/asyncua/common/statemachine.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,15 +198,15 @@
 
     async def _write_state(self, state: State):
         if not isinstance(state, State):
             raise ValueError(f"Statemachine: {self._name} -> state: {state} is not a instance of StateMachine.State class")
         await self._current_state_node.write_value(ua.LocalizedText(state.name, self.locale), ua.VariantType.LocalizedText)
         if state.node:
             if self._current_state_id_node:
-                await self._current_state_id_node.write_value(state.id)
+                await self._current_state_id_node.write_value(state.node.nodeid, varianttype=ua.VariantType.NodeId)
             if self._current_state_name_node and state.name:
                 await self._current_state_name_node.write_value(state.name, ua.VariantType.QualifiedName)
             if self._current_state_number_node and state.number:
                 await self._current_state_number_node.write_value(state.number, ua.VariantType.UInt32)
             if self._current_state_effective_display_name_node and state.effectivedisplayname:
                 await self._current_state_effective_display_name_node.write_value(state.effectivedisplayname, ua.VariantType.LocalizedText)
 
@@ -217,15 +217,15 @@
         '''
         if not isinstance(transition, Transition):
             raise ValueError(f"Statemachine: {self._name} -> state: {transition} is not a instance of StateMachine.Transition class")
         transition._transitiontime = datetime.datetime.utcnow()
         await self._last_transition_node.write_value(ua.LocalizedText(transition.name, self.locale), ua.VariantType.LocalizedText)
         if self._optionals:
             if self._last_transition_id_node:
-                await self._last_transition_id_node.write_value(transition.id)
+                await self._last_transition_id_node.write_value(transition.node.nodeid, varianttype=ua.VariantType.NodeId)
             if self._last_transition_name_node and transition.name:
                 await self._last_transition_name_node.write_value(ua.QualifiedName(transition.name, self._idx), ua.VariantType.QualifiedName)
             if self._last_transition_number_node and transition.number:
                 await self._last_transition_number_node.write_value(transition.number, ua.VariantType.UInt32)
             if self._last_transition_transitiontime_node and transition._transitiontime:
                 await self._last_transition_transitiontime_node.write_value(transition._transitiontime, ua.VariantType.DateTime)
             
@@ -235,15 +235,15 @@
         state: State,
         InitialStateType: ua.NodeId(2309, 0),
         StateType: ua.NodeId(2307, 0),
         ChoiceStateType: ua.NodeId(15109,0),
         '''
         if not isinstance(state, State):
             raise ValueError(f"Statemachine: {self._name} -> state: {state} is not a instance of StateMachine.State class")
-        if not state_type in [ua.NodeId(2309, 0),ua.NodeId(2307, 0),ua.NodeId(15109,0)]:
+        if state_type not in [ua.NodeId(2309, 0), ua.NodeId(2307, 0), ua.NodeId(15109, 0)]:
             # unknown state type!
             raise ValueError(f"Statemachine: {self._name} -> state_type: {state_type} is not in list: [ua.NodeId(2309, 0),ua.NodeId(2307, 0),ua.NodeId(15109,0)]")
         if not state.name:
             raise ValueError(f"Statemachine: {self._name} -> State.name is None")
         if not state.number:
             raise ValueError(f"Statemachine: {self._name} -> State.number is None")
         state.node = await self._state_machine_node.add_object(
```

### Comparing `asyncua-1.0.2/asyncua/common/structures.py` & `asyncua-1.0.3/asyncua/common/structures.py`

 * *Files identical despite different names*

### Comparing `asyncua-1.0.2/asyncua/common/structures104.py` & `asyncua-1.0.3/asyncua/common/structures104.py`

 * *Files 1% similar despite different names*

```diff
@@ -384,15 +384,16 @@
 async def load_custom_struct_xml_import(node_id: ua.NodeId, attrs: ua.DataTypeAttributes):
     """
     This function is used to load custom structs from xmlimporter
     """
     name = attrs.DisplayName.Text
     if hasattr(ua, name):
         return getattr(ua, name)
-    sdef = attrs.DataTypeDefinition
+    # FIXME : mypy attribute not defined
+    sdef = attrs.DataTypeDefinition  # type: ignore[attr-defined]
     env = await _generate_object(name, sdef, data_type=node_id)
     struct = env[name]
     ua.register_extension_object(name, sdef.DefaultEncodingId, struct, node_id)
     return env[name]
 
 
 async def _recursive_parse_basedatatypes(server, base_node, parent_datatype, new_alias) -> Any:
@@ -554,10 +555,11 @@
 async def load_enum_xml_import(node_id: ua.NodeId, attrs: ua.DataTypeAttributes, option_set: bool):
     """
     This function is used to load enums from xmlimporter
     """
     name = attrs.DisplayName.Text
     if hasattr(ua, name):
         return getattr(ua, name)
-    env = await _generate_object(name, attrs.DataTypeDefinition, enum=True, option_set=option_set)
+    # FIXME: DateTypeDefinition is not a known attribute for mypy
+    env = await _generate_object(name, attrs.DataTypeDefinition, enum=True, option_set=option_set)   # type: ignore[attr-defined]
     ua.register_enum(name, node_id, env[name])
     return env[name]
```

### Comparing `asyncua-1.0.2/asyncua/common/subscription.py` & `asyncua-1.0.3/asyncua/common/subscription.py`

 * *Files 8% similar despite different names*

```diff
@@ -137,27 +137,31 @@
         known_handles_args: List[Tuple] = []
         for item in datachange.MonitoredItems:
             if item.ClientHandle not in self._monitored_items:
                 self.logger.warning("Received a notification for unknown handle: %s", item.ClientHandle)
                 continue
             data = self._monitored_items[item.ClientHandle]
             event_data = DataChangeNotif(data, item)
-            known_handles_args.append((data.node, item.Value.Value.Value, event_data))
+            # FIXME: Value can be None
+            known_handles_args.append((data.node, item.Value.Value.Value, event_data))  # type: ignore[union-attr]
 
         try:
             tasks = [
                 self._handler.datachange_notification(*args) for args in known_handles_args
             ]
             if asyncio.iscoroutinefunction(self._handler.datachange_notification):
                 await asyncio.gather(*tasks)
         except Exception as ex:
             self.logger.exception("Exception calling data change handler. Error: %s", ex)
 
     async def _call_event(self, eventlist: ua.EventNotificationList):
         for event in eventlist.Events:
+            if event.ClientHandle not in self._monitored_items:
+                self.logger.warning("Received a notification for unknown handle: %s", event.ClientHandle)
+                continue
             data = self._monitored_items[event.ClientHandle]
             result = Event.from_event_fields(data.mfilter.SelectClauses, event.EventFields)
             result.server_handle = data.server_handle
             if hasattr(self._handler, "event_notification"):
                 try:
                     if asyncio.iscoroutinefunction(self._handler.event_notification):
                         await self._handler.event_notification(result)
@@ -206,18 +210,18 @@
         :return: Handle for changing/cancelling of the subscription
         """
         return await self._subscribe(
             nodes, attr, queuesize=queuesize, monitoring=monitoring, sampling_interval=sampling_interval
         )
 
     async def _create_eventfilter(self, evtypes: Union[ua.ObjectIds, List[ua.ObjectIds], ua.NodeId, List[ua.NodeId]], where_clause_generation: bool = True):
-        if not type(evtypes) in (list, tuple):
+        if not isinstance(evtypes, (list, tuple)):
             evtypes = [evtypes]
-        evtypes = [Node(self.server, evtype) for evtype in evtypes]
-        evfilter = await get_filter_from_event_type(evtypes, where_clause_generation)
+        evtypes = [Node(self.server, evtype) for evtype in evtypes]  # type: ignore[union-attr]
+        evfilter = await get_filter_from_event_type(evtypes, where_clause_generation) # type: ignore[union-attr]
         return evfilter
 
     async def subscribe_events(
         self,
         sourcenode: Node = ua.ObjectIds.Server,
         evtypes: Union[ua.ObjectIds, List[ua.ObjectIds], ua.NodeId, List[ua.NodeId]] = ua.ObjectIds.BaseEventType,
         evfilter: ua.EventFilter = None,
@@ -237,15 +241,15 @@
         :param queuesize: 0 for default queue size, 1 for minimum queue size, n for FIFO queue,
         MaxUInt32 for max queue size
         :param where_clause_generation: No where_clause generation when no eventfilter is provided. Need for TwinCAT, Codesys
         :return: Handle for changing/cancelling of the subscription
         """
         sourcenode = Node(self.server, sourcenode)
         if evfilter is None:
-            if not type(evtypes) in (list, tuple) and evtypes == ua.ObjectIds.BaseEventType:
+            if type(evtypes) not in (list, tuple) and evtypes == ua.ObjectIds.BaseEventType:
                 # Remove where clause for base event type, for servers that have problems with long WhereClauses.
                 # Also because BaseEventType wants every event we can ommit it. Issue: #1205
                 where_clause_generation = False
             evfilter = await self._create_eventfilter(evtypes, where_clause_generation)
         return await self._subscribe(sourcenode, ua.AttributeIds.EventNotifier, evfilter, queuesize=queuesize)  # type: ignore
 
     async def subscribe_alarms_and_conditions(
@@ -265,25 +269,15 @@
         :param sourcenode: Node
         :param evtypes: ua.ObjectIds or ua.NodeId
         :param evfilter: ua.EventFilter which provides the SelectClauses and WhereClause
         :param queuesize: 0 for default queue size, 1 for minimum queue size, n for FIFO queue,
         MaxUInt32 for max queue size
         :return: Handle for changing/cancelling of the subscription
         """
-        sourcenode = Node(self.server, sourcenode)
-        if evfilter is None:
-            evfilter = await self._create_eventfilter(evtypes)
-        # Add SimpleAttribute for NodeId if missing.
-        matches = [a for a in evfilter.SelectClauses if a.AttributeId == ua.AttributeIds.NodeId]
-        if not matches:
-            conditionIdOperand = ua.SimpleAttributeOperand()
-            conditionIdOperand.TypeDefinitionId = ua.NodeId(ua.ObjectIds.ConditionType)
-            conditionIdOperand.AttributeId = ua.AttributeIds.NodeId
-            evfilter.SelectClauses.append(conditionIdOperand)
-        return await self._subscribe(sourcenode, ua.AttributeIds.EventNotifier, evfilter, queuesize=queuesize)  # type: ignore
+        return await self.subscribe_events(sourcenode, evtypes, evfilter, queuesize)
 
     async def _subscribe(
         self,
         nodes: Union[Node, Iterable[Node]],
         attr = ua.AttributeIds.Value,
         mfilter: ua.MonitoringFilter = None,
         queuesize: int = 0,
```

### Comparing `asyncua-1.0.2/asyncua/common/type_dictionary_builder.py` & `asyncua-1.0.3/asyncua/common/type_dictionary_builder.py`

 * *Files identical despite different names*

### Comparing `asyncua-1.0.2/asyncua/common/ua_utils.py` & `asyncua-1.0.3/asyncua/common/ua_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
 def string_to_val(string, vtype):
     """
     Convert back a string to a python or python-asyncua object
     Note: no error checking is done here, supplying null strings could raise exceptions (datetime and guid)
     """
     string = string.strip()
-    if string.startswith("["):
+    if string.startswith("[") and string.endswith("]"):
         string = string[1:-1]
         var = []
         for s in string.split(","):
             s = s.strip()
             val = string_to_val(s, vtype)
             var.append(val)
         return var
@@ -207,14 +207,25 @@
         refs=ua.ObjectIds.HasSubtype, direction=ua.BrowseDirection.Inverse
     )
     if supertypes:
         return supertypes[0]
     return None
 
 
+async def is_subtype(node, supertype):
+    """
+    return if a node is a subtype of a specified nodeid
+    """
+    while node:
+        if node.nodeid == supertype:
+            return True
+        node = await get_node_supertype(node)
+    return False
+
+
 async def is_child_present(node, browsename):
     """
     return if a browsename is present a child from the provide node
     :param node: node wherein to find the browsename
     :param browsename: browsename to search
     :returns returns True if the browsename is present else False
     """
```

### Comparing `asyncua-1.0.2/asyncua/common/utils.py` & `asyncua-1.0.3/asyncua/common/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,19 +114,19 @@
     if sys.version_info.major == 3 and sys.version_info.minor <= 8:
         resolved_fieldtypes = get_type_hints(
             class_or_instance,
             globalns=globalns,
             localns=localns
         )
     else:
-        resolved_fieldtypes = get_type_hints(
+        resolved_fieldtypes = get_type_hints(  # type: ignore[call-arg]
             class_or_instance,
             globalns=globalns,
             localns=localns,
-            include_extras=include_extras
+            include_extras=include_extras 
         )
     for field in fields_:
         try:
             field.type = resolved_fieldtypes[field.name]
         except KeyError:
             _logger.info(f"could not resolve fieldtype for field={field} of class_or_instance={class_or_instance}")
             pass
```

### Comparing `asyncua-1.0.2/asyncua/common/xmlexporter.py` & `asyncua-1.0.3/asyncua/common/xmlexporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 import logging
 import asyncio
 import functools
 from collections import OrderedDict
 import xml.etree.ElementTree as Et
 import base64
-from dataclasses import fields, is_dataclass
+from dataclasses import is_dataclass
 from enum import Enum
 
 from asyncua import ua
 from asyncua.ua.uatypes import type_string_from_type
 from asyncua.ua.uaerrors import UaError
 from .. import Node
 from ..ua import object_ids as o_ids
@@ -264,15 +264,15 @@
         # We only write these values if they are different from defaults
         # Not sure where default is defined....
         if accesslevel not in (0, ua.AccessLevel.CurrentRead.mask):
             var_el.attrib["AccessLevel"] = str(accesslevel)
         if useraccesslevel not in (0, ua.AccessLevel.CurrentRead.mask):
             var_el.attrib["UserAccessLevel"] = str(useraccesslevel)
 
-        var = await node.read_attribute(ua.AttributeIds.MinimumSamplingInterval)
+        var = await node.read_attribute(ua.AttributeIds.MinimumSamplingInterval, raise_on_bad_status=False)
         if var.Value.Value:
             var_el.attrib["MinimumSamplingInterval"] = str(var.Value.Value)
         var = await node.read_attribute(ua.AttributeIds.Historizing)
         if var.Value.Value:
             var_el.attrib["Historizing"] = 'true'
 
     async def add_etree_variable_type(self, node):
```

### Comparing `asyncua-1.0.2/asyncua/common/xmlimporter.py` & `asyncua-1.0.3/asyncua/common/xmlimporter.py`

 * *Files identical despite different names*

### Comparing `asyncua-1.0.2/asyncua/common/xmlparser.py` & `asyncua-1.0.3/asyncua/common/xmlparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -455,11 +455,13 @@
         for model in self.root.findall('base:Models/base:Model', self.ns):
             uri = model.attrib.get('ModelUri')
             if uri is not None:
                 version = model.attrib.get('Version', '')
                 date_time = model.attrib.get('PublicationDate')
                 if date_time is None:
                     date_time = ua.DateTime(1, 1, 1)
-                else:
+                elif date_time is not None and date_time[-1]=="Z":
                     date_time = ua.DateTime.strptime(date_time, "%Y-%m-%dT%H:%M:%SZ")
+                else:
+                    date_time = ua.DateTime.strptime(date_time, "%Y-%m-%dT%H:%M:%S%z")
                 ns.append((uri, version, date_time))
         return ns
```

### Comparing `asyncua-1.0.2/asyncua/crypto/permission_rules.py` & `asyncua-1.0.3/asyncua/crypto/permission_rules.py`

 * *Files identical despite different names*

### Comparing `asyncua-1.0.2/asyncua/crypto/security_policies.py` & `asyncua-1.0.3/asyncua/crypto/security_policies.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
     def vsignature_size(self):
         return self.Verifier.signature_size()
 
     def verify(self, data, sig):
         if not self.use_prev_key:
             self.Verifier.verify(data, sig)
         else:
-            _logger.debug(f"Message verification fallback: trying with previous secure channel key")
+            _logger.debug("Message verification fallback: trying with previous secure channel key")
             self.Prev_Verifier.verify(data, sig)
 
     def encrypt(self, data):
         if self.is_encrypted:
             if not len(data) % self.Encryptor.plain_block_size() == 0:
                 raise ValueError
             return self.Encryptor.encrypt(data)
@@ -205,15 +205,15 @@
         now = time.time()
         if now > self.prev_key_expiration:
             if self.Prev_Decryptor and self.Prev_Verifier:
                 self.Prev_Decryptor.reset()
                 self.Prev_Decryptor = None
                 self.Prev_Verifier.reset()
                 self.Prev_Verifier = None
-                _logger.debug(f"Expired secure_channel keys removed")
+                _logger.debug("Expired secure_channel keys removed")
 
     @property
     def use_prev_key(self):
         if self._use_prev_key:
             if self.Prev_Decryptor and self.Prev_Verifier:
                 return True
             raise uacrypto.InvalidSignature
```

### Comparing `asyncua-1.0.2/asyncua/crypto/uacrypto.py` & `asyncua-1.0.3/asyncua/crypto/uacrypto.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,23 +4,31 @@
 from typing import Optional, Union
 
 from cryptography import x509
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives import hmac
-from cryptography.hazmat.primitives.asymmetric import padding
+from cryptography.hazmat.primitives.asymmetric import padding, rsa
 from cryptography.hazmat.primitives.ciphers import Cipher
 from cryptography.hazmat.primitives.ciphers import algorithms
 from cryptography.hazmat.primitives.ciphers import modes
+
+# We redefine InvalidSignature as part of this module. Do not remove this line.
+from cryptography.exceptions import InvalidSignature  # noqa: F811
+
 from dataclasses import dataclass
 import logging
 _logger = logging.getLogger(__name__)
 
 
+class InvalidSignature(Exception):  # type: ignore # noqa: F811
+    pass
+
+
 @dataclass
 class CertProperties:
     path_or_content: Union[bytes, Path, str]
     extension: Optional[str] = None
     password: Optional[Union[str, bytes]] = None
 
 
@@ -73,14 +81,24 @@
 
 
 def der_from_x509(certificate):
     if certificate is None:
         return b""
     return certificate.public_bytes(serialization.Encoding.DER)
 
+def pem_from_key(private_key: rsa.RSAPrivateKey) -> bytes:
+    """dumps a private key in PEM format
+
+    Args:
+        private_key (rsa.RSAPrivateKey): The privatekey to dump
+
+    Returns:
+        bytes: The private as PEM/PKCS8 format
+    """
+    return private_key.private_bytes(encoding=serialization.Encoding.PEM, format=serialization.PrivateFormat.PKCS8, encryption_algorithm=serialization.NoEncryption())
 
 def sign_sha1(private_key, data):
     return private_key.sign(
         data,
         padding.PKCS1v15(),
         hashes.SHA1()
     )
@@ -269,19 +287,19 @@
         err = True
     if cert.not_valid_before > now:
         _logger.error(f'certificate is not yet vaild: valid after {cert.not_valid_before}')
         err = True
     try:
         san = cert.extensions.get_extension_for_class(x509.SubjectAlternativeName)
         san_uri = san.value.get_values_for_type(x509.UniformResourceIdentifier)
-        if application_uri is not san_uri:
-            _logger.error(f'certificate does not cotain the application uri ({application_uri}). Most applications will reject a connection without it.')
+        if application_uri not in san_uri:
+            _logger.error(f'certificate does not contain the application uri ({application_uri}). Most applications will reject a connection without it.')
             err = True
         if hostname is not None:
             san_dns_names = san.value.get_values_for_type(x509.DNSName)
-            if hostname is not san_dns_names:
-                _logger.error(f'certificate does not cotain the hostname in DNSNames {hostname}. Some applications will check this.')
+            if hostname not in san_dns_names:
+                _logger.error(f'certificate does not contain the hostname in DNSNames {hostname}. Some applications will check this.')
                 err = True
     except x509.ExtensionNotFound:
         _logger.error('certificate has no SubjectAlternativeName this is need for application verification!')
         err = True
     return err
```

### Comparing `asyncua-1.0.2/asyncua/server/address_space.py` & `asyncua-1.0.3/asyncua/server/address_space.py`

 * *Files 2% similar despite different names*

```diff
@@ -369,15 +369,15 @@
         self._add_unique_reference(parentdata, desc) # FIXME return StatusCode is not evaluated
 
     def _add_ref_to_parent(self, nodedata: NodeData, item: ua.AddNodesItem, parentdata: NodeData):
         addref = ua.AddReferencesItem()
         addref.ReferenceTypeId = item.ReferenceTypeId
         addref.SourceNodeId = nodedata.nodeid
         addref.TargetNodeId = item.ParentNodeId
-        addref.TargetNodeClass = parentdata.attributes[ua.AttributeIds.NodeClass].value.Value.Value
+        addref.TargetNodeClass = parentdata.attributes[ua.AttributeIds.NodeClass].value.Value.Value # type: ignore[union-attr]
         addref.IsForward = False # FIXME in uaprotocol_auto.py
         self._add_reference_no_check(nodedata, addref) # FIXME return StatusCode is not evaluated
 
     def _add_type_definition(self, nodedata: NodeData, item: ua.AddNodesItem):
         addref = ua.AddReferencesItem()
         addref.SourceNodeId = nodedata.nodeid
         addref.IsForward = True # FIXME in uaprotocol_auto.py
@@ -448,23 +448,24 @@
 
     def _add_reference_no_check(self, sourcedata: NodeData, addref: ua.AddReferencesItem) -> ua.StatusCode:
         rdesc = ua.ReferenceDescription()
         rdesc.ReferenceTypeId = addref.ReferenceTypeId
         rdesc.IsForward = addref.IsForward
         rdesc.NodeId = addref.TargetNodeId
         if addref.TargetNodeClass == ua.NodeClass.Unspecified:
-            rdesc.NodeClass = self._aspace.read_attribute_value(
+            rdesc.NodeClass = self._aspace.read_attribute_value(   # type: ignore[union-attr]
                 addref.TargetNodeId, ua.AttributeIds.NodeClass
-            ).Value.Value
+            ).Value.Value  
         else:
             rdesc.NodeClass = addref.TargetNodeClass
-        bname = self._aspace.read_attribute_value(addref.TargetNodeId, ua.AttributeIds.BrowseName).Value.Value
+        bname = self._aspace.read_attribute_value(addref.TargetNodeId, ua.AttributeIds.BrowseName).Value.Value   # type: ignore[union-attr]
+
         if bname:
             rdesc.BrowseName = bname
-        dname = self._aspace.read_attribute_value(addref.TargetNodeId, ua.AttributeIds.DisplayName).Value.Value
+        dname = self._aspace.read_attribute_value(addref.TargetNodeId, ua.AttributeIds.DisplayName).Value.Value  # type: ignore[union-attr]
         if dname:
             rdesc.DisplayName = dname
         return self._add_unique_reference(sourcedata, rdesc)
 
     def delete_references(self, refs: List[ua.DeleteReferencesItem], user: User = User(role=UserRole.Admin)) -> List[ua.StatusCode]:
         result: List[ua.StatusCode] = []
         for ref in refs:
@@ -795,29 +796,30 @@
                 await v(k, value)
             except Exception as ex:
                 self.logger.exception("Error calling datachange callback %s, %s, %s", k, v, ex)
 
         return ua.StatusCode()
 
     def _is_expected_variant_type(self, value: ua.DataValue, attval: AttributeValue, node: NodeData) -> bool:
-        vtype = attval.value.Value.VariantType # FIXME Type hinting reveals that it is possible that Value (Optional) is None which would raise an exception
+        # FIXME Type hinting reveals that it is possible that Value (Optional) is None which would raise an exception
+        vtype = attval.value.Value.VariantType # type: ignore[union-attr] 
         if vtype == ua.VariantType.Null:
             # Node had a null value, many nodes are initialized with that value
             # we should check what the real type is
-            dtype = node.attributes[ua.AttributeIds.DataType].value.Value.Value
+            dtype = node.attributes[ua.AttributeIds.DataType].value.Value.Value # type: ignore[union-attr]
             if dtype.NamespaceIndex == 0 and dtype.Identifier <= 25:
                 vtype = ua.VariantType(dtype.Identifier)
             else:
                 # FIXME: should find the correct variant type given data type but
                 # this is a bit complicaed so trusting the first write
                 return True
-        if value.Value.VariantType == vtype:
+        if value.Value.VariantType == vtype:  # type: ignore[union-attr]
             return True
         _logger.warning("Write refused: Variant: %s with type %s does not have expected type: %s",
-                value.Value, value.Value.VariantType, attval.value.Value.VariantType)
+                value.Value, value.Value.VariantType, attval.value.Value.VariantType)  # type: ignore[union-attr] 
         return False
 
     def add_datachange_callback(self, nodeid: ua.NodeId, attr: ua.AttributeIds, callback: Callable) -> Tuple[ua.StatusCode, int]:
         # self.logger.debug("set attr callback: %s %s %s", nodeid, attr, callback)
         if nodeid not in self._nodes:
             return ua.StatusCode(ua.StatusCodes.BadNodeIdUnknown), 0
         node = self._nodes[nodeid]
```

### Comparing `asyncua-1.0.2/asyncua/server/binary_server_asyncio.py` & `asyncua-1.0.3/asyncua/server/binary_server_asyncio.py`

 * *Files identical despite different names*

### Comparing `asyncua-1.0.2/asyncua/server/event_generator.py` & `asyncua-1.0.3/asyncua/server/event_generator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
 from datetime import datetime
 import time
 import uuid
-from typing import Optional
 import sys
 
 from asyncua import ua
 from ..common import events, event_objects, Node
 
 
 class EventGenerator:
@@ -21,30 +20,32 @@
         etype: The event type, either an objectId, a NodeId or a Node object
     """
 
     def __init__(self, isession):
         self.logger = logging.getLogger(__name__)
         self.isession = isession
         self.event: event_objects.BaseEvent = None
-        self.emitting_node: Optional[Node] = None
 
-    async def init(self, etype=None, emitting_node=ua.ObjectIds.Server):
+    async def init(self, etype=None, emitting_node=ua.ObjectIds.Server, add_generates_event=True):
         node = None
 
         if isinstance(etype, event_objects.BaseEvent):
             self.event = etype
         elif isinstance(etype, Node):
             node = etype
         elif isinstance(etype, ua.NodeId):
             node = Node(self.isession, etype)
         else:
             node = Node(self.isession, ua.NodeId(etype))
 
         if node:
             self.event = await events.get_event_obj_from_type_node(node)
+            if isinstance(self.event, event_objects.Condition):
+                # Add ConditionId, which is not modelled as a component of the ConditionType
+                self.event.add_property('NodeId', None, ua.VariantType.NodeId)
 
         if isinstance(emitting_node, Node):
             pass
         elif isinstance(emitting_node, ua.NodeId):
             emitting_node = Node(self.isession, emitting_node)
         else:
             emitting_node = Node(self.isession, ua.NodeId(emitting_node))
@@ -52,34 +53,35 @@
         self.event.emitting_node = emitting_node.nodeid
         if not self.event.SourceNode:
             self.event.SourceNode = emitting_node.nodeid
         if not self.event.SourceName:
             self.event.SourceName = (await Node(self.isession, self.event.SourceNode).read_browse_name()).Name
 
         await emitting_node.set_event_notifier([ua.EventNotifier.SubscribeToEvents])
-        refs = []
-        ref = ua.AddReferencesItem()
-        ref.IsForward = True
-        ref.ReferenceTypeId = ua.NodeId(ua.ObjectIds.GeneratesEvent)
-        ref.SourceNodeId = emitting_node.nodeid
-        ref.TargetNodeClass = ua.NodeClass.ObjectType
-        ref.TargetNodeId = self.event.EventType
-        refs.append(ref)
-        results = await self.isession.add_references(refs)
-        # result.StatusCode.check()
 
-        self.emitting_node = emitting_node
+        if add_generates_event:
+            refs = []
+            ref = ua.AddReferencesItem()
+            ref.IsForward = True
+            ref.ReferenceTypeId = ua.NodeId(ua.ObjectIds.GeneratesEvent)
+            ref.SourceNodeId = emitting_node.nodeid
+            ref.TargetNodeClass = ua.NodeClass.ObjectType
+            ref.TargetNodeId = self.event.EventType
+            refs.append(ref)
+            results = await self.isession.add_references(refs)
+            for result in results:
+                result.check()
 
     def __str__(self):
-        return f"EventGenerator(Type:{self.event.EventType}, Emitting Node:{self.emitting_node}, " \
+        return f"EventGenerator(Type:{self.event.EventType}, Emitting Node:{self.event.emitting_node.to_string()}, " \
                f"Time:{self.event.Time}, Message: {self.event.Message})"
 
     __repr__ = __str__
 
-    async def trigger(self, time_attr=None, message=None):
+    async def trigger(self, time_attr=None, message=None, subscription_id=None):
         """
         Trigger the event. This will send a notification to all subscribed clients
         """
         self.event.EventId = ua.Variant(uuid.uuid4().hex.encode('utf-8'), ua.VariantType.ByteString)
         if time_attr:
             self.event.Time = time_attr
         else:
@@ -96,8 +98,8 @@
         self.event.LocalTime.DaylightSavingInOffset = bool(localtime.tm_isdst != -1)
 
         if message:
             self.event.Message = ua.LocalizedText(message)
         elif not self.event.Message:
             self.event.Message = ua.LocalizedText((await Node(self.isession, self.event.SourceNode).read_browse_name()).Name).Text
 
-        await self.isession.subscription_service.trigger_event(self.event)
+        await self.isession.subscription_service.trigger_event(self.event, subscription_id=subscription_id)
```

### Comparing `asyncua-1.0.2/asyncua/server/history.py` & `asyncua-1.0.3/asyncua/server/history.py`

 * *Files identical despite different names*

### Comparing `asyncua-1.0.2/asyncua/server/history_sql.py` & `asyncua-1.0.3/asyncua/server/history_sql.py`

 * *Files identical despite different names*

### Comparing `asyncua-1.0.2/asyncua/server/internal_server.py` & `asyncua-1.0.3/asyncua/server/internal_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,27 @@
 import asyncio
 from datetime import datetime, timedelta
 from copy import copy
 from struct import unpack_from
 from pathlib import Path
 import logging
 from urllib.parse import urlparse
-from typing import Coroutine, Tuple
+from typing import Coroutine
 
 from asyncua import ua
 from .user_managers import PermissiveUserManager, UserManager
 from ..common.callback import CallbackService
 from ..common.node import Node
 from .history import HistoryManager
 from .address_space import AddressSpace, AttributeService, ViewService, NodeManagementService, MethodService
 from .subscription_service import SubscriptionService
 from .standard_address_space import standard_address_space
 from .users import User, UserRole
 from .internal_session import InternalSession
+from .event_generator import EventGenerator
 
 try:
     from asyncua.crypto import uacrypto
 except ImportError:
     logging.getLogger(__name__).warning("cryptography is not installed, use of crypto disabled")
     uacrypto = False
 
@@ -45,14 +46,15 @@
 
     def __init__(self, user_manager: UserManager = None):
         self.logger = logging.getLogger(__name__)
         self.callback_service = CallbackService()
         self.endpoints = []
         self._channel_id_counter = 5
         self.allow_remote_admin = True
+        self.bind_condition_methods = False
         self.disabled_clock = False  # for debugging, we may want to disable clock that writes too much in log
         self._known_servers = {}  # used if we are a discovery server
         self.certificate = None
         self.private_key = None
         self.aspace = AddressSpace()
         self.attribute_service = AttributeService(self.aspace)
         self.view_service = ViewService(self.aspace)
@@ -77,14 +79,28 @@
         self.supported_tokens = []
 
     async def init(self, shelffile=None):
         await self.load_standard_address_space(shelffile)
         await self._address_space_fixes()
         await self.setup_nodes()
         await self.history_manager.init()
+        if self.bind_condition_methods:
+            await self.setup_condition_methods()
+
+    async def setup_condition_methods(self):
+        for etype in (ua.ObjectIds.RefreshStartEventType, ua.ObjectIds.RefreshEndEventType):
+            evgen = EventGenerator(self.isession)
+            await evgen.init(etype, add_generates_event=False)
+            # don't use isinstance(int), it also matches bool
+            if type(self.bind_condition_methods) is int:
+                evgen.event.Severity = self.bind_condition_methods
+            self.subscription_service.standard_events[etype] = evgen
+
+        self.isession.add_method_callback(ua.NodeId(ua.ObjectIds.ConditionType_ConditionRefresh), self.subscription_service.condition_refresh)
+        self.isession.add_method_callback(ua.NodeId(ua.ObjectIds.ConditionType_ConditionRefresh2), self.subscription_service.condition_refresh)
 
     async def setup_nodes(self):
         """
         Set up some nodes as defined by spec
         """
         uries = ['http://opcfoundation.org/UA/']
         ns_node = Node(self.isession, ua.NodeId(ua.ObjectIds.Server_NamespaceArray))
@@ -227,15 +243,15 @@
                 for url in edp.Server.DiscoveryUrls
             ]
             edps.append(edp)
         return edps
 
     def find_servers(self, params, sockname=None):
         servers = []
-        params_server_uris = [uri.split(':') for uri in params.ServerUris]
+        params_server_uris = [uri.split(':') for uri in params.ServerUris] if params.ServerUris else []
         our_application_uris = [edp.Server.ApplicationUri for edp in self.endpoints]
         for desc in self._known_servers.values():
             if params_server_uris:
                 serv_uri = desc.Server.ApplicationUri.split(':')
                 if not any(serv_uri[: len(uri)] == uri for uri in params_server_uris):
                     continue
             if desc.Server.ApplicationUri in our_application_uris:
```

### Comparing `asyncua-1.0.2/asyncua/server/internal_session.py` & `asyncua-1.0.3/asyncua/server/internal_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from enum import Enum
-from typing import Coroutine, Iterable, Optional, List
+from typing import Iterable, Optional, List
 
 from asyncua import ua
 from asyncua.common.session_interface import AbstractSession
 from ..common.callback import CallbackType, ServerItemCallback
 from ..common.utils import create_nonce, ServiceError
 from .address_space import AddressSpace
 from .users import User, UserRole
@@ -128,15 +128,15 @@
         await self.iserver.callback_service.dispatch(CallbackType.PreRead,
                                                      ServerItemCallback(params, None, user, self.external))
         results = self.iserver.attribute_service.read(params)
         await self.iserver.callback_service.dispatch(CallbackType.PostRead,
                                                      ServerItemCallback(params, results, user, self.external))
         return results
 
-    async def history_read(self, params) -> Coroutine:
+    async def history_read(self, params) -> ua.HistoryReadResult:
         return await self.iserver.history_manager.read_history(params)
 
     async def write(self, params):
         if self.user is None:
             user = User()
         else:
             user = self.user
```

### Comparing `asyncua-1.0.2/asyncua/server/internal_subscription.py` & `asyncua-1.0.3/asyncua/server/internal_subscription.py`

 * *Files identical despite different names*

### Comparing `asyncua-1.0.2/asyncua/server/monitored_item_service.py` & `asyncua-1.0.3/asyncua/server/monitored_item_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,18 +27,18 @@
         self.old_dvalue: Optional[ua.DataValue] = None
 
     def set_current_datavalue(self, cur_val: ua.DataValue):
         self.old_dvalue = self.current_dvalue
         # We need to clone the value, to prevent referencing the inner value
         self.current_dvalue = copy.deepcopy(cur_val)
 
-    def get_current_datavalue(self) -> ua.DataValue:
+    def get_current_datavalue(self) -> Optional[ua.DataValue]:
         return self.current_dvalue
 
-    def get_old_datavalue(self) -> ua.DataValue:
+    def get_old_datavalue(self) -> Optional[ua.DataValue]:
         return self.old_dvalue
 
 
 class MonitoredItemService:
     """
     Implements monitored item service for one subscription
     """
@@ -113,16 +113,16 @@
         return result, mdata
 
     def _create_events_monitored_item(self, params: ua.MonitoredItemCreateRequest):
         self.logger.info("request to subscribe to events for node %s and attribute %s", params.ItemToMonitor.NodeId,
                          params.ItemToMonitor.AttributeId)
 
         result, mdata = self._make_monitored_item_common(params)
-        ev_notify_byte = self.aspace.read_attribute_value(params.ItemToMonitor.NodeId,
-                                                          ua.AttributeIds.EventNotifier).Value.Value
+        ev_notify_byte = self.aspace.read_attribute_value(params.ItemToMonitor.NodeId,   # type: ignore[union-attr]
+                                                          ua.AttributeIds.EventNotifier).Value.Value 
 
         if ev_notify_byte is None or not ua.ua_binary.test_bit(ev_notify_byte, ua.EventNotifier.SubscribeToEvents):
             result.StatusCode = ua.StatusCode(ua.StatusCodes.BadServiceUnsupported)
             return result
         # result.FilterResult = ua.EventFilterResult()  # spec says we can ignore if not error
         mdata.where_clause_evaluator = WhereClauseEvaluator(self.logger, self.aspace, mdata.filter.WhereClause)
         self._commit_monitored_item(result, mdata)
@@ -174,16 +174,23 @@
         self._monitored_items.pop(mid)
         return ua.StatusCode()
 
     @staticmethod
     def _is_data_changed(values: MonitoredItemValues, trg: ua.DataChangeTrigger) -> bool:
         old = values.get_old_datavalue()
         current = values.get_current_datavalue()
+        if old is None and current is None:
+            return False
+        elif (old is None) != (current is None):
+            return True
+        elif old is None or current is None:
+            # This should never happen with the above logic, adding this check for mypy
+            raise ValueError('This is an implementation error')
 
-        if old is None or old.StatusCode != current.StatusCode:
+        if old.StatusCode != current.StatusCode:
             return True
 
         if trg in [ua.DataChangeTrigger.StatusValue,ua.DataChangeTrigger.StatusValueTimestamp ] and \
                 old.Value != current.Value:
             return True
 
         if trg == ua.DataChangeTrigger.StatusValueTimestamp and \
@@ -216,30 +223,34 @@
                 event.ClientHandle = mdata.client_handle
                 event.Value = value
                 await self.isub.enqueue_datachange_event(mid, event, mdata.queue_size)
 
     def _is_deadband_exceeded(self, values: MonitoredItemValues, flt: ua.DataChangeFilter):
         if flt.DeadbandType == ua.DeadbandType.None_ or values.get_old_datavalue() is None:
             return True
-        delta = values.get_current_datavalue().Value.Value - values.get_old_datavalue().Value.Value
+        delta = values.get_current_datavalue().Value.Value - values.get_old_datavalue().Value.Value  # type: ignore[union-attr]
         if flt.DeadbandType == ua.DeadbandType.Absolute and ((abs(delta)) > flt.DeadbandValue):
             return True
         if flt.DeadbandType == ua.DeadbandType.Percent:
             self.logger.warning("DeadbandType Percent is not implemented !")
             return True
         return False
 
-    async def trigger_event(self, event):
+    async def trigger_event(self, event, mid=None):
         if event.emitting_node not in self._monitored_events:
             self.logger.debug("%s has NO subscription for events %s from node: %s", self, event, event.emitting_node)
             return False
+
         self.logger.debug("%s has subscription for events %s from node: %s", self, event, event.emitting_node)
-        mids = self._monitored_events[event.emitting_node]
-        for mid in mids:
+        if mid is not None:
             await self._trigger_event(event, mid)
+        else:
+            mids = self._monitored_events[event.emitting_node]
+            for mid in mids:
+                await self._trigger_event(event, mid)
         return True
 
     async def _trigger_event(self, event, mid: int):
         if mid not in self._monitored_items:
             self.logger.debug("Could not find monitored items for id %s for event %s in subscription %s", mid, event,
                               self)
             return
```

### Comparing `asyncua-1.0.2/asyncua/server/server.py` & `asyncua-1.0.3/asyncua/server/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -398,14 +398,71 @@
             if ua.SecurityPolicyType.Aes128Sha256RsaOaep_Sign in self._security_policy:
                 self._set_endpoints(security_policies.SecurityPolicyAes128Sha256RsaOaep, ua.MessageSecurityMode.Sign)
                 self._policies.append(
                     ua.SecurityPolicyFactory(security_policies.SecurityPolicyAes128Sha256RsaOaep,
                                              ua.MessageSecurityMode.Sign, self.certificate, self.iserver.private_key,
                                              permission_ruleset=self._permission_ruleset))
 
+
+    @staticmethod
+    def lookup_security_level_for_policy_type( security_policy_type: ua.SecurityPolicyType ) -> ua.Byte:
+        """Returns the security level for an ua.SecurityPolicyType.
+
+        This is endpoint & server implementation specific!
+
+        Returns:
+            ua.Byte: the found security level
+        """
+
+        return ua.Byte({
+            ua.SecurityPolicyType.NoSecurity : 0,
+            ua.SecurityPolicyType.Basic128Rsa15_Sign : 1,
+            ua.SecurityPolicyType.Basic128Rsa15_SignAndEncrypt : 2,
+            ua.SecurityPolicyType.Basic256_Sign : 11,
+            ua.SecurityPolicyType.Basic256_SignAndEncrypt : 21,
+            ua.SecurityPolicyType.Basic256Sha256_Sign : 50,
+            ua.SecurityPolicyType.Basic256Sha256_SignAndEncrypt : 70,
+            ua.SecurityPolicyType.Aes128Sha256RsaOaep_Sign : 55,
+            ua.SecurityPolicyType.Aes128Sha256RsaOaep_SignAndEncrypt : 75
+        }[security_policy_type])
+
+
+    @staticmethod
+    def determine_security_level(security_policy_uri:str, security_mode: ua.MessageSecurityMode) -> ua.Byte:
+        """Determine the security level of an EndPoint.
+        The security level indicates how secure an EndPoint is, compared to other EndPoints of the same server.
+        Value 0 is a special value; EndPoint isn't recommended, typical for ua.MessageSecurityMode.None_.
+
+        See Part 4 7.10
+
+        To the determine the level the value of ua.SecurityPolicyType is used.
+        The enum values already correspond to and
+        The Enum ua.SecurityPolicyType already contains a value per Enum entry that already correspond to
+
+
+        Args:
+            security_policy (ua.SecurityPolicy): the used policy
+            security_mode (ua.MessageSecurityMode): the used security mode for the messages.
+
+        Returns:
+            ua.Byte: the returned security level
+        """
+        security_level: ua.Byte = ua.Byte(0)
+
+        if security_mode != ua.MessageSecurityMode.None_:
+            security_policy_name = f'{security_policy_uri.split("#")[1].replace("_","")}_{security_mode.name}'
+
+            try:
+                security_policy_type: ua.SecurityPolicyType = ua.SecurityPolicyType[security_policy_name]
+                security_level = Server.lookup_security_level_for_policy_type(security_policy_type)
+            except KeyError:
+                _logger.error('"%s" isn\'t a valid security policy', security_policy_name)
+
+        return security_level
+
     def _set_endpoints(self, policy=ua.SecurityPolicy, mode=ua.MessageSecurityMode.None_):
         idtokens = []
         supported_token_classes = []
         if "Anonymous" in self._policyIDs:
             idtoken = ua.UserTokenPolicy()
             idtoken.PolicyId = "anonymous"
             idtoken.TokenType = ua.UserTokenType.Anonymous
@@ -438,15 +495,15 @@
         edp.Server = appdesc
         if self.certificate:
             edp.ServerCertificate = uacrypto.der_from_x509(self.certificate)
         edp.SecurityMode = mode
         edp.SecurityPolicyUri = policy.URI
         edp.UserIdentityTokens = idtokens
         edp.TransportProfileUri = "http://opcfoundation.org/UA-Profile/Transport/uatcp-uasc-uabinary"
-        edp.SecurityLevel = 0
+        edp.SecurityLevel = Server.determine_security_level(policy.URI, mode)
         self.iserver.add_endpoint(edp)
         self.iserver.supported_tokens = tuple(supported_token_classes)
 
     def set_server_name(self, name):
         self.name = name
 
     async def start(self):
```

### Comparing `asyncua-1.0.2/asyncua/server/standard_address_space/standard_address_space.py` & `asyncua-1.0.3/asyncua/server/standard_address_space/standard_address_space.py`

 * *Files identical despite different names*

### Comparing `asyncua-1.0.2/asyncua/server/standard_address_space/standard_address_space_services.py` & `asyncua-1.0.3/asyncua/server/standard_address_space/standard_address_space_services.py`

 * *Files identical despite different names*

### Comparing `asyncua-1.0.2/asyncua/server/subscription_service.py` & `asyncua-1.0.3/asyncua/server/subscription_service.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 import asyncio
 import logging
 from typing import Dict, Iterable
 
 from asyncua import ua
-from asyncua.common import utils
+from asyncua.common import utils, uamethod
 from .address_space import AddressSpace
 from .internal_subscription import InternalSubscription
 
 
 class SubscriptionService:
     """
     Manages subscriptions on the server side.
@@ -19,14 +19,16 @@
     """
 
     def __init__(self, aspace: AddressSpace):
         self.logger = logging.getLogger(__name__)
         self.aspace: AddressSpace = aspace
         self.subscriptions: Dict[int, InternalSubscription] = {}
         self._sub_id_counter = 77
+        self.standard_events = {}
+        self._conditions = {}
 
     async def create_subscription(self, params, callback, request_callback=None):
         self.logger.info("create subscription")
         result = ua.CreateSubscriptionResult()
         result.RevisedPublishingInterval = params.RequestedPublishingInterval
         result.RevisedLifetimeCount = params.RequestedLifetimeCount
         result.RevisedMaxKeepAliveCount = params.RequestedMaxKeepAliveCount
@@ -109,10 +111,33 @@
 
     def republish(self, params):
         if params.SubscriptionId not in self.subscriptions:
             # TODO: what should I do?
             return ua.NotificationMessage()
         return self.subscriptions[params.SubscriptionId].republish(params.RetransmitSequenceNumber)
 
-    async def trigger_event(self, event):
-        for sub in self.subscriptions.values():
-            await sub.monitored_item_srv.trigger_event(event)
+    async def trigger_event(self, event, subscription_id=None):
+        if hasattr(event, 'Retain') and hasattr(event, 'NodeId'):
+            if event.Retain:
+                self._conditions[event.NodeId] = event
+            elif event.NodeId in self._conditions:
+                del self._conditions[event.NodeId]
+        if subscription_id is not None:
+            if subscription_id in self.subscriptions:
+                await self.subscriptions[subscription_id].monitored_item_srv.trigger_event(event)
+        else:
+            for sub in self.subscriptions.values():
+                await sub.monitored_item_srv.trigger_event(event)
+
+    @uamethod
+    async def condition_refresh(self, parent, subscription_id, mid=None):
+        if subscription_id not in self.subscriptions:
+            return ua.StatusCode(ua.StatusCodes.BadSubscriptionIdInvalid)
+        sub = self.subscriptions[subscription_id]
+        if mid is not None and mid not in sub.monitored_item_srv._monitored_items:
+            return ua.StatusCode(ua.StatusCodes.BadMonitoredItemIdInvalid)
+        if ua.ObjectIds.RefreshStartEventType in self.standard_events:
+            await self.standard_events[ua.ObjectIds.RefreshStartEventType].trigger(subscription_id=subscription_id)
+        for event in self._conditions.values():
+            await sub.monitored_item_srv.trigger_event(event, mid)
+        if ua.ObjectIds.RefreshEndEventType in self.standard_events:
+            await self.standard_events[ua.ObjectIds.RefreshEndEventType].trigger(subscription_id=subscription_id)
```

### Comparing `asyncua-1.0.2/asyncua/server/uaprocessor.py` & `asyncua-1.0.3/asyncua/server/uaprocessor.py`

 * *Files identical despite different names*

### Comparing `asyncua-1.0.2/asyncua/server/user_managers.py` & `asyncua-1.0.3/asyncua/server/user_managers.py`

 * *Files identical despite different names*

### Comparing `asyncua-1.0.2/asyncua/sync.py` & `asyncua-1.0.3/asyncua/sync.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 sync API of asyncua
 """
 import asyncio
+import functools
 from pathlib import Path
 from threading import Thread, Condition
 import logging
 from typing import List, Tuple, Union, Optional
 
 from asyncua import ua
 from asyncua import client
@@ -94,38 +95,83 @@
         aio_func = getattr(self.aio_obj, func.__name__)
         result = self.tloop.post(aio_func(*args, **kwargs))
         return _to_sync(self.tloop, result)
 
     return wrapper
 
 
+def sync_wrapper(aio_func):
+    def wrapper(*args, **kwargs):
+        if not args:
+            raise RuntimeError("first argument of function must a ThreadLoop object")
+        if isinstance(args[0], ThreadLoop):
+            tloop = args[0]
+            args = list(args)[1:]
+        elif hasattr(args[0], "tloop"):
+            tloop = args[0].tloop
+        else:
+            raise RuntimeError("first argument of function must a ThreadLoop object")
+        args, kwargs = _to_async(args, kwargs)
+        result = tloop.post(aio_func(*args, **kwargs))
+        return _to_sync(tloop, result)
+
+    return wrapper
+
+
 def syncfunc(aio_func):
     """
     decorator for sync function
     """
     def decorator(func, *args, **kwargs):
-        def wrapper(*args, **kwargs):
-            if not args:
-                raise RuntimeError("first argument of function must a ThreadLoop object")
-            if isinstance(args[0], ThreadLoop):
-                tloop = args[0]
-                args = list(args)[1:]
-            elif hasattr(args[0], "tloop"):
-                tloop = args[0].tloop
-            else:
-                raise RuntimeError("first argument of function must a ThreadLoop object")
-            args, kwargs = _to_async(args, kwargs)
-            result = tloop.post(aio_func(*args, **kwargs))
-            return _to_sync(tloop, result)
-
-        return wrapper
+        return sync_wrapper(aio_func)
 
     return decorator
 
 
+def sync_uaclient_method(aio_func):
+    """
+    Usage:
+
+    ```python
+    from asyncua.client.ua_client import UaClient
+    from asyncua.sync import Client
+
+    with Client('otp.tcp://localhost') as client:
+        read_attributes = sync_uaclient_method(UaClient.read_attributes)(client)
+        results = read_attributes(...)
+        ...
+    ```
+    """
+    def sync_method(client: 'Client'):
+        uaclient = client.aio_obj.uaclient
+        return functools.partial(sync_wrapper(aio_func), client.tloop, uaclient)
+
+    return sync_method
+
+
+def sync_async_client_method(aio_func):
+    """
+    Usage:
+
+    ```python
+    from asyncua.client import Client as AsyncClient
+    from asyncua.sync import Client
+
+    with Client('otp.tcp://localhost') as client:
+        read_attributes = sync_async_client_method(AsyncClient.read_attributes)(client)
+        results = read_attributes(...)
+        ...
+    ```
+    """
+    def sync_method(client: 'Client'):
+        return functools.partial(sync_wrapper(aio_func), client.tloop, client)
+
+    return sync_method
+
+
 @syncfunc(aio_func=common.methods.call_method_full)
 def call_method_full(parent, methodid, *args):
     pass
 
 
 @syncfunc(aio_func=common.ua_utils.data_type_to_variant_type)
 def data_type_to_variant_type(dtype_node):
@@ -148,15 +194,15 @@
         self.sync_handler = sync_handler
 
     def datachange_notification(self, node, val, data):
         self.sync_handler.datachange_notification(SyncNode(self.tloop, node), val, data)
 
     def event_notification(self, event):
         self.sync_handler.event_notification(event)
-        
+
     def status_change_notification(self, status: ua.StatusChangeNotification):
         self.sync_handler.status_change_notification(status)
 
 class Client:
     def __init__(self, url: str, timeout: int = 4, tloop=None):
         self.tloop = tloop
         self.close_tloop = False
@@ -231,33 +277,41 @@
 
     def create_subscription(self, period, handler):
         coro = self.aio_obj.create_subscription(period, _SubHandler(self.tloop, handler))
         aio_sub = self.tloop.post(coro)
         return Subscription(self.tloop, aio_sub)
 
     @syncmethod
+    def delete_subscriptions(self, subscription_ids):
+        pass
+
+    @syncmethod
     def get_namespace_index(self, url):
         pass
 
     def get_node(self, nodeid):
         return SyncNode(self.tloop, self.aio_obj.get_node(nodeid))
 
     def get_root_node(self):
         return SyncNode(self.tloop, self.aio_obj.get_root_node())
 
     @syncmethod
     def connect_and_get_server_endpoints(self):
         pass
 
     @syncmethod
+    def read_attributes(self, nodes, attr=ua.AttributeIds.Value):
+        pass
+
+    @syncmethod
     def read_values(self, nodes):
         pass
 
     @syncmethod
-    def write_values(self, nodes, values):
+    def write_values(self, nodes, values, raise_on_partial_error=True):
         pass
 
     def __enter__(self):
         try:
             self.connect()
         except Exception as ex:
             self.disconnect()
@@ -495,14 +549,34 @@
         pass
 
     @syncmethod
     def get_child(self, path):
         pass
 
     @syncmethod
+    def get_children_by_path(self, paths, raise_on_partial_error=True):
+        pass
+
+    @syncmethod
+    def read_raw_history(self, starttime=None, endtime=None, numvalues=0, return_bounds=True):
+        pass
+
+    @syncmethod
+    def history_read(self, details, continuation_point=None):
+        pass
+
+    @syncmethod
+    def read_event_history(self, starttime=None, endtime=None, numvalues=0, evtypes=ua.ObjectIds.BaseEventType):
+        pass
+
+    @syncmethod
+    def history_read_events(self, details):
+        pass
+
+    @syncmethod
     def set_modelling_rule(self, mandatory: bool):
         pass
 
     @syncmethod
     def add_variable(self, ns, name, val):
         pass
 
@@ -607,15 +681,19 @@
 
 class Subscription:
     def __init__(self, tloop, sub):
         self.tloop = tloop
         self.aio_obj = sub
 
     @syncmethod
-    def subscribe_data_change(self, nodes, attr=ua.AttributeIds.Value, queuesize=0):
+    def subscribe_data_change(self, nodes,
+                              attr=ua.AttributeIds.Value,
+                              queuesize=0,
+                              monitoring=ua.MonitoringMode.Reporting,
+                              sampling_interval=0.0):
         pass
 
     @syncmethod
     def subscribe_events(
         self,
         sourcenode=ua.ObjectIds.Server,
         evtypes=ua.ObjectIds.BaseEventType,
@@ -686,25 +764,25 @@
 ) -> ua.StructureField:
     if isinstance(dtype, SyncNode):
         dtype = dtype.aio_obj
     return common.structures104.new_struct_field(name, dtype, array, optional, description)
 
 
 @syncfunc(aio_func=common.structures104.new_enum)
-def new_enum(
+def new_enum(  # type: ignore[empty-body]
     server: Union["Server", "Client"],
     idx: Union[int, ua.NodeId],
     name: Union[int, ua.QualifiedName],
     values: List[str],
     optional: bool = False
 ) -> SyncNode:
     pass
 
 
 @syncfunc(aio_func=common.structures104.new_struct)
-def new_struct(
+def new_struct(  # type: ignore[empty-body]
     server: Union["Server", "Client"],
     idx: Union[int, ua.NodeId],
     name: Union[int, ua.QualifiedName],
     fields: List[ua.StructureField],
 ) -> Tuple[SyncNode, List[SyncNode]]:
     pass
```

### Comparing `asyncua-1.0.2/asyncua/tools.py` & `asyncua-1.0.3/asyncua/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import asyncio
 import logging
 import sys
 import argparse
 from datetime import datetime, timedelta
 import math
-import time
 import concurrent.futures
 
 try:
     from IPython import embed  # type: ignore
 except ImportError:
     import code
 
@@ -585,15 +584,15 @@
     if args.certificate:
         await client.load_client_certificate(args.certificate)
     if args.private_key:
         await client.load_private_key(args.private_key)
 
     try:
         async with client:
-            mynode = await get_node(client, args)
+            await get_node(client, args)
     except (OSError, concurrent.futures.TimeoutError) as e:
         print(e)
         sys.exit(1)
 
     sys.exit(0)
 
 
@@ -665,16 +664,16 @@
         idx = await server.register_namespace(uri)
         objects = server.nodes.objects
         myobj = await objects.add_object(idx, "MyObject")
         mywritablevar = await myobj.add_variable(idx, "MyWritableVariable", 6.7)
         await mywritablevar.set_writable()  # Set MyVariable to be writable by clients
         myvar = await myobj.add_variable(idx, "MyVariable", 6.7)
         myarrayvar = await myobj.add_variable(idx, "MyVarArray", [6.7, 7.9])
-        myprop = await myobj.add_property(idx, "MyProperty", "I am a property")
-        mymethod = await myobj.add_method(
+        await myobj.add_property(idx, "MyProperty", "I am a property")
+        await myobj.add_method(
             idx,
             "MyMethod",
             multiply,
             [ua.VariantType.Double, ua.VariantType.Int64],
             [ua.VariantType.Double],
         )
```

### Comparing `asyncua-1.0.2/asyncua/ua/attribute_ids.py` & `asyncua-1.0.3/asyncua/ua/attribute_ids.py`

 * *Files identical despite different names*

### Comparing `asyncua-1.0.2/asyncua/ua/object_ids.py` & `asyncua-1.0.3/asyncua/ua/object_ids.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #AUTOGENERATED!!!
 
-from enum import IntEnum
 
 class ObjectIds:
     Null = 0
     Boolean = 1
     SByte = 2
     Byte = 3
     Int16 = 4
```

### Comparing `asyncua-1.0.2/asyncua/ua/status_codes.py` & `asyncua-1.0.3/asyncua/ua/status_codes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #AUTOGENERATED!!! Date: 2022-09-22 16:18:40.855698
 
-from asyncua.ua.uaerrors import UaStatusCodeError
 
 class StatusCodes:
     Good = 0x00000000
     Uncertain = 0x40000000
     Bad = 0x80000000
     BadUnexpectedError = 0x80010000
     BadInternalError = 0x80020000
```

### Comparing `asyncua-1.0.2/asyncua/ua/ua_binary.py` & `asyncua-1.0.3/asyncua/ua/ua_binary.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Binary protocol specific functions and constants
 """
 
 import functools
 import struct
 import logging
-from typing import Any, Callable, Union
+from typing import Any, Callable
 import typing
 import uuid
 from enum import Enum, IntFlag
 from dataclasses import is_dataclass, fields
 from asyncua import ua
 from .uaerrors import UaError
 from ..common.utils import Buffer
@@ -280,15 +280,15 @@
 def create_dataclass_serializer(dataclazz):
     """Given a dataclass, return a function that serializes instances of this dataclass"""
     data_fields = fields(dataclazz)
     # TODO: adding the 'ua' module to the globals to resolve the type hints might not be enough.
     #       it is possible that the type annotations also refere to classes defined in other modules.
     try:
         resolved_fieldtypes = typing.get_type_hints(dataclazz, {'ua': ua})
-    except NameError as e:
+    except NameError:
         resolved_fieldtypes = typing.get_type_hints(dataclazz)
 
     for f in data_fields:
         f.type = resolved_fieldtypes[f.name]
 
     if issubclass(dataclazz, ua.UaUnion):
         # Union is a class with Encoding and Value field
@@ -572,18 +572,18 @@
         packet.append(Primitives.Bytes.pack(body))
     return b''.join(packet)
 
 
 def _create_list_deserializer(uatype, recursive: bool = False):
     if recursive:
 
-        def _deserialize(data):
+        def _deserialize_recursive(data):
             size = Primitives.Int32.unpack(data)
             return [_create_type_deserializer(uatype, type(None))(data) for _ in range(size)]
-        return _deserialize
+        return _deserialize_recursive
     element_deserializer = _create_type_deserializer(uatype, type(None))
 
     def _deserialize(data):
         size = Primitives.Int32.unpack(data)
         return [element_deserializer(data) for _ in range(size)]
     return _deserialize
 
@@ -653,15 +653,15 @@
         return decode_union
     enc_count = 0
     field_deserializers = []
     # TODO: adding the 'ua' module to the globals to resolve the type hints might not be enough.
     #       its possible that the type annotations also refere to classes defined in other modules.
     try:
         resolved_fieldtypes = typing.get_type_hints(objtype, {'ua': ua})
-    except NameError as e:
+    except NameError:
         resolved_fieldtypes = typing.get_type_hints(objtype)
 
     for field in fields(objtype):
         optional_enc_bit = 0
         field_type = resolved_fieldtypes[field.name]
         subtypes = type_allow_subclass(field.type)
         # if our member has a switch and it is not set we will need to skip it
```

### Comparing `asyncua-1.0.2/asyncua/ua/uaerrors/_auto.py` & `asyncua-1.0.3/asyncua/ua/uaerrors/_auto.py`

 * *Files identical despite different names*

### Comparing `asyncua-1.0.2/asyncua/ua/uaerrors/_base.py` & `asyncua-1.0.3/asyncua/ua/uaerrors/_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -62,13 +62,43 @@
     def code(self):
         """
         The code of the status error.
         """
         return self.args[0]
 
 
+class UaStatusCodeErrors(UaStatusCodeError):
+    def __new__(cls, *args):
+        # use the default implementation
+        self = UaError.__new__(cls, *args)
+        return self
+
+    def __init__(self, codes):
+        """
+        :param codes: The codes of the results.
+        """
+        self.codes = codes
+
+    def __str__(self):
+        # import here to avoid circular import problems
+        import asyncua.ua.status_codes as status_codes
+
+        return "[{0}]".format(", ".join(["{1}({0})".format(*status_codes.get_name_and_doc(code)) for code in self.codes]))
+
+    @property
+    def code(self):
+        """
+        The code of the status error.
+        """
+        # import here to avoid circular import problems
+        from asyncua.ua.uatypes import StatusCode
+
+        error_codes = [code for code in self.codes if not StatusCode(code).is_good()]
+        return error_codes[0] if len(error_codes) > 0 else None
+
+
 class UaStringParsingError(UaError):
     pass
 
 
 class UaStructParsingError(UaError):
     pass
```

### Comparing `asyncua-1.0.2/asyncua/ua/uaprotocol_auto.py` & `asyncua-1.0.3/asyncua/ua/uaprotocol_auto.py`

 * *Files identical despite different names*

### Comparing `asyncua-1.0.2/asyncua/ua/uaprotocol_hand.py` & `asyncua-1.0.3/asyncua/ua/uaprotocol_hand.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import struct
 from dataclasses import dataclass, field
 from typing import List
 
 from asyncua.ua import uaprotocol_auto as auto
 from asyncua.ua import uatypes
 from asyncua.common import utils
-from asyncua.ua.uatypes import AccessLevel
 
 OPC_TCP_SCHEME = 'opc.tcp'
 
 
 @dataclass
 class Hello:
     ProtocolVersion: uatypes.UInt32 = 0
@@ -78,15 +77,15 @@
 @dataclass
 class AsymmetricAlgorithmHeader:
     SecurityPolicyURI: uatypes.String = 'http://opcfoundation.org/UA/SecurityPolicy#None'
     SenderCertificate: uatypes.ByteString = None
     ReceiverCertificateThumbPrint: uatypes.ByteString = None
 
     def __str__(self):
-        size1 = len(self.SenderCertificate) if self.SenderCertificate is not None else None
+        len(self.SenderCertificate) if self.SenderCertificate is not None else None
         size2 = len(self.ReceiverCertificateThumbPrint) if self.ReceiverCertificateThumbPrint is not None else None
         return f'{self.__class__.__name__}(SecurityPolicy:{self.SecurityPolicyURI},' \
                f' certificatesize:{size2}, receiverCertificatesize:{size2} )'
 
     __repr__ = __str__
```

### Comparing `asyncua-1.0.2/asyncua/ua/uatypes.py` & `asyncua-1.0.3/asyncua/ua/uatypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Optional, Any, Union, Generic, List
 import collections
 import logging
 from enum import Enum, IntEnum
 import uuid
 import re
 import itertools
-from datetime import datetime, timedelta, MAXYEAR, timezone
+from datetime import datetime, timedelta, timezone
 from dataclasses import dataclass, field
 
 # hack to support python < 3.8
 if sys.version_info.minor < 10:
     def get_origin(tp):
         if hasattr(tp, "__origin__"):
             return tp.__origin__
@@ -679,23 +679,23 @@
         if not isinstance(self.NamespaceIndex, int) or not isinstance(self.Name, (str, type(None))):
             raise ValueError(f"QualifiedName constructor args have wrong types, {self}")
 
     def to_string(self):
         return f"{self.NamespaceIndex}:{self.Name}"
 
     @staticmethod
-    def from_string(string):
+    def from_string(string, default_idx=0):
         if ":" in string:
             try:
                 idx, name = string.split(":", 1)
                 idx = int(idx)
             except (TypeError, ValueError) as ex:
                 raise UaStringParsingError(f"Error parsing string {string}", ex) from ex
         else:
-            idx = 0
+            idx = default_idx
             name = string
         return QualifiedName(Name=name, NamespaceIndex=idx)
 
 
 @dataclass(frozen=True, init=False)
 class LocalizedText:
     """
```

### Comparing `asyncua-1.0.2/asyncua.egg-info/PKG-INFO` & `asyncua-1.0.3/asyncua.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncua
-Version: 1.0.2
+Version: 1.0.3
 Summary: Pure Python OPC-UA client and server library
 Home-page: http://freeopcua.github.io/
 Author: Olivier Roulet-Dubonnet
 Author-email: olivier.roulet@gmail.com
 License: GNU Lesser General Public License v3 or later
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -23,49 +23,47 @@
 [![Python package](https://github.com/FreeOpcUa/opcua-asyncio/workflows/Python%20package/badge.svg)](https://github.com/FreeOpcUa/opcua-asyncio/actions)
 
 [![PyPI Package](https://badge.fury.io/py/asyncua.svg)](https://badge.fury.io/py/asyncua)
 
 # opcua-asyncio
 
 opcua-asyncio is an asyncio-based asynchronous OPC UA client and server based on python-opcua, removing support of python < 3.7.
-Asynchronous programming allows for simpler code (e.g. less need for locks) and potentially performance gains.
-This library has also [sync wrapper](https://github.com/FreeOpcUa/opcua-asyncio/blob/master/asyncua/sync.py) over async API which may can be used in sync code instead of python-opcua
+Asynchronous programming allows for simpler code (e.g. less need for locks) and can potentially provide performance improvements.
+This library also provides a [synchronous wrapper](https://github.com/FreeOpcUa/opcua-asyncio/blob/master/asyncua/sync.py) over the async API, which can be used in synchronous code instead of python-opcua.
 
 ---
 
-OPC UA binary protocol implementation has been tested against many different OPC UA stacks. API offers both a low level interface to send and receive all UA defined structures and high level classes allowing to write a server or a client in a few lines. It is easy to mix high level objects and low level UA calls in one application. Most low level code is autogenerated from xml specification.
-
-coverage.py reports a test coverage of over 95 % of code, most of non-tested code is autogenerated code that is not used yet.
+The OPC UA binary protocol implementation has undergone extensive testing with various OPC UA stacks. The API offers both a low level interface to send and receive all UA defined structures and high level classes allowing to write a server or a client in a few lines. It is easy to mix high level objects and low level UA calls in one application. Most low level code is autogenerated from xml specification.
 
+The test coverage reported by coverage.py is over 95%, with the majority of the non-tested code being autogenerated code that is not currently in use.
 
 # Warnings
 
-opcua-asyncio is open-source and comes with absolutely no warranty. We try to keep it as much bug-free as possible and try to keep API stable but bugs and API changes will happen! Especially API changes will happen before any 1.0 release.
+opcua-asyncio is open-source and comes with absolutely no warranty. We try to keep it as bug-free as possible, and try to keep the API stable, but bugs and API changes will happen! In particular, API changes are expected to take place prior to any 1.0 release.
 
 Some renaming of methods from get_xx to read_xx and set_xx to write_xxx have been made to better follow OPC UA naming conventions
 
-Version 0.9.9 introduces some argument renaming due to more automatic code generation. Especially the arguments to NodeId, BrowseName, LocalizedText and DataValue are now CamelCase instead of lower case, thus follow the OPC Ua convention used in all other structures in this library
+Version 0.9.9 introduces some argument renaming due to more automatic code generation. Especially the arguments to NodeId, BrowseName, LocalizedText and DataValue, which are now CamelCase instead of lower case, following the OPC UA conventions used in all other structures in this library
 
 # Installation
 
 With pip
 
     pip install asyncua
 
 # Usage
 
 We assume that you already have some experience with Python, the asyncio module, the async / await syntax and the concept of asyncio Tasks.
 
 ## Client class
 
-The `Client` class provides a high level API for connecting to APU UA servers, session management and access to basic
+The `Client` class provides a high level API for connecting to OPC UA servers, session management and access to basic
 address space services.
 The client can be used as a context manager. The client will then automatically connect and disconnect withing the `with`syntax.
 
-
 ```python
 from asyncua import Client
 
 async with Client(url='opc.tcp://localhost:4840/freeopcua/server/') as client:
     while True:
         # Do something with client
         node = client.get_node('i=85')
@@ -88,144 +86,146 @@
 
 The `Server` class provides a high level API for creation of OPC UA server instances.
 
 # Documentation
 
 The documentation is available here [ReadTheDocs](http://opcua-asyncio.readthedocs.org/en/latest/).
 
-The API remains mostly unchanged in regards to [python-opcua](http://opcua-asyncio.rtfd.io/).
-Main difference is that most methods are now async.
+The API remains mostly unchanged with regards to [python-opcua](http://opcua-asyncio.rtfd.io/).
+The main difference is that most methods are now asynchronous.
 Please have a look at [the examples](https://github.com/FreeOpcUa/opcua-asyncio/blob/master/examples) and/or the code.
 
-A simple GUI client is available: https://github.com/FreeOpcUa/opcua-client-gui
+A simple GUI client is available at: https://github.com/FreeOpcUa/opcua-client-gui
 
 Browse the examples: https://github.com/FreeOpcUa/opcua-asyncio/tree/master/examples
 
-A good starting point are the minimal examples.
+The minimal examples are a good starting point.
 Minimal client example: https://github.com/FreeOpcUa/opcua-asyncio/blob/master/examples/client-minimal.py
 Minimal server example: https://github.com/FreeOpcUa/opcua-asyncio/blob/master/examples/server-minimal.py
 
 A set of command line tools also available: https://github.com/FreeOpcUa/opcua-asyncio/tree/master/tools
-* `uadiscover `(find_servers, get_endpoints and find_servers_on_network calls)
-* `uals `(list children of a node)
-* `uahistoryread`
-* `uaread `(read attribute of a node)
-* `uawrite `(write attribute of a node)
-* `uacall `(call method of a node)
-* `uasubscribe `(subscribe to a node and print datachange events)
-* `uaclient `(connect to server and start python shell)
-* `uaserver `(starts a demo OPC UA server)
-  `tools/uaserver --populate --certificate cert.pem --private_key pk.pem`
+
+-   `uadiscover `(find_servers, get_endpoints and find_servers_on_network calls)
+-   `uals `(list children of a node)
+-   `uahistoryread`
+-   `uaread `(read attribute of a node)
+-   `uawrite `(write attribute of a node)
+-   `uacall `(call method of a node)
+-   `uasubscribe `(subscribe to a node and print datachange events)
+-   `uaclient `(connect to server and start python shell)
+-   `uaserver `(starts a demo OPC UA server)
+    `tools/uaserver --populate --certificate cert.pem --private_key pk.pem`
 
 How to generate certificate: https://github.com/FreeOpcUa/opcua-asyncio/tree/master/examples/generate_certificate.sh
 
 ## Client support
 
 What works:
 
-* connection to server, opening channel, session
-* browsing and reading attributes value
-* getting nodes by path and nodeids
-* creating subscriptions
-* subscribing to items for data change
-* subscribing to events
-* adding nodes
-* method call
-* user and password
-* history read
-* login with certificate
-* communication encryption
-* removing nodes
+-   connection to server, opening channel, session
+-   browsing and reading attributes value
+-   getting nodes by path and nodeids
+-   creating subscriptions
+-   subscribing to items for data change
+-   subscribing to events
+-   adding nodes
+-   method call
+-   user and password
+-   history read
+-   login with certificate
+-   communication encryption
+-   removing nodes
 
 Tested servers: freeopcua C++, freeopcua Python, prosys, kepware, beckhoff, winCC, B&R, …
 
 Not implemented yet:
 
-* localized text feature
-* XML protocol
-* UDP (PubSub stuff)
-* WebSocket
-* maybe automatic reconnection...
-
+-   localized text feature
+-   XML protocol
+-   UDP (PubSub stuff)
+-   WebSocket
+-   maybe automatic reconnection...
 
 ## Server support
 
 What works:
 
-* creating channel and sessions
-* read/set attributes and browse
-* getting nodes by path and nodeids
-* autogenerate address space from spec
-* adding nodes to address space
-* datachange events
-* events
-* methods
-* basic user implementation (one existing user called admin, which can be disabled, all others are read only)
-* encryption
-* certificate handling
-* removing nodes
-* history support for data change and events
-* more high level solution to create custom structures
+-   creating channel and sessions
+-   read/set attributes and browse
+-   getting nodes by path and nodeids
+-   autogenerate address space from spec
+-   adding nodes to address space
+-   datachange events
+-   events
+-   methods
+-   basic user implementation (one existing user called admin, which can be disabled, all others are read only)
+-   encryption
+-   certificate handling
+-   removing nodes
+-   history support for data change and events
+-   more high level solution to create custom structures
 
 Tested clients: freeopcua C++, freeopcua Python, uaexpert, prosys, quickopc
 
 Not yet implemented:
 
-* UDP (PubSub stuff)
-* WebSocket
-* session restore
-* alarms
-* XML protocol
-* views
-* localized text features
-* better security model with users and password
-
+-   UDP (PubSub stuff)
+-   WebSocket
+-   session restore
+-   alarms
+-   XML protocol
+-   views
+-   localized text features
+-   better security model with users and password
 
 ### Running a server on a Raspberry Pi
 
 Setting up the standard address-space from XML is the most time-consuming step of the startup process which may lead to
 long startup times on less powerful devices like a Raspberry Pi. By passing a path to a cache-file to the server constructor,
 a shelve holding the address space will be created during the first startup. All following startups will make use of the
 cache-file which leads to significantly better startup performance (~3.5 vs 125 seconds on a Raspberry Pi Model B).
 
-
 # Development
 
 Code follows PEP8 apart for line lengths which should be max 160 characters and OPC UA structures that keep camel case
 from XML definition.
 
 All protocol code is under opcua directory
 
-- `asyncua/ua` contains all UA structures from specification, most are autogenerated
-- `asyncua/common` contains high level objects and methods used both in server and client
-- `asyncua/client` contains client specific code
-- `asyncua/server` contains server specific code
-- `asyncua/utils` contains some utilities function and classes
-- `asyncua/tools` contains code for command lines tools
-- `schemas` contains the XML and text files from specification and the python scripts used to autogenerate code
-- `tests` contains tests
-- `docs` contains files to auto generate documentation from doc strings
-- `examples` contains many example files
-- `examples/sync` contains many example files using sync API
-- `tools` contains python scripts that can be used to run command line tools from repository without installing
+-   `asyncua/ua` contains all UA structures from specification, most are autogenerated
+-   `asyncua/common` contains high level objects and methods used both in server and client
+-   `asyncua/client` contains client specific code
+-   `asyncua/server` contains server specific code
+-   `asyncua/utils` contains some utilities function and classes
+-   `asyncua/tools` contains code for command lines tools
+-   `schemas` contains the XML and text files from specification and the python scripts used to autogenerate code
+-   `tests` contains tests
+-   `docs` contains files to auto generate documentation from doc strings
+-   `examples` contains many example files
+-   `examples/sync` contains many example files using sync API
+-   `tools` contains python scripts that can be used to run command line tools from repository without installing
 
 ## Running tests:
 
 ```
 python -m pip install -r requirements.txt
 python -m pip install -r dev_requirements.txt
 pytest -v -s
 ```
+
 Or
+
 ```
 ./run-test.sh -v -s
 ```
 
 ## Coverage
 
 ```
 pytest -v -s --cov asyncua --cov-report=html
 ```
+
 Or
+
 ```
 ./run-test.sh -v -s --cov asyncua --cov-report=html
 ```
```

### Comparing `asyncua-1.0.2/asyncua.egg-info/SOURCES.txt` & `asyncua-1.0.3/asyncua.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 asyncua/common/type_dictionary_builder.py
 asyncua/common/ua_utils.py
 asyncua/common/utils.py
 asyncua/common/xmlexporter.py
 asyncua/common/xmlimporter.py
 asyncua/common/xmlparser.py
 asyncua/crypto/__init__.py
+asyncua/crypto/cert_gen.py
 asyncua/crypto/permission_rules.py
 asyncua/crypto/security_policies.py
 asyncua/crypto/uacrypto.py
 asyncua/server/__init__.py
 asyncua/server/address_space.py
 asyncua/server/binary_server_asyncio.py
 asyncua/server/event_generator.py
```

### Comparing `asyncua-1.0.2/setup.py` & `asyncua-1.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # don't require pytest-runner unless we have been invoked as a test launch
 needs_pytest = {'pytest', 'test', 'ptr'}.intersection(sys.argv)
 pytest_runner = ['pytest-runner'] if needs_pytest else []
 
 setup(
     name="asyncua",
-    version="1.0.2",
+    version="1.0.3",
     description="Pure Python OPC-UA client and server library",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Olivier Roulet-Dubonnet",
     author_email="olivier.roulet@gmail.com",
     url='http://freeopcua.github.io/',
     packages=find_packages(exclude=["tests"]),
```

