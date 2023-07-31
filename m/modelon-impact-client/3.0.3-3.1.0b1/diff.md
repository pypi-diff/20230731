# Comparing `tmp/modelon_impact_client-3.0.3.tar.gz` & `tmp/modelon_impact_client-3.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelon_impact_client-3.0.3.tar", max compression
+gzip compressed data, was "modelon_impact_client-3.1.0b1.tar", max compression
```

## Comparing `modelon_impact_client-3.0.3.tar` & `modelon_impact_client-3.1.0b1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0     1479 2023-06-13 10:51:29.729589 modelon_impact_client-3.0.3/LICENSE.md
--rw-r--r--   0        0        0     2748 2023-06-13 10:51:29.740589 modelon_impact_client-3.0.3/README.md
--rw-r--r--   0        0        0        0 2023-06-13 10:51:29.696588 modelon_impact_client-3.0.3/modelon/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 10:51:29.726589 modelon_impact_client-3.0.3/modelon/impact/__init__.py
--rw-r--r--   0        0        0      830 2023-06-13 10:51:29.721588 modelon_impact_client-3.0.3/modelon/impact/client/__init__.py
--rw-r--r--   0        0        0    24886 2023-06-13 10:51:29.699588 modelon_impact_client-3.0.3/modelon/impact/client/client.py
--rw-r--r--   0        0        0      835 2023-06-13 10:51:29.741589 modelon_impact_client-3.0.3/modelon/impact/client/configuration.py
--rw-r--r--   0        0        0     1938 2023-06-13 10:51:29.699588 modelon_impact_client-3.0.3/modelon/impact/client/credential_manager.py
--rw-r--r--   0        0        0      119 2023-06-13 10:51:29.709588 modelon_impact_client-3.0.3/modelon/impact/client/entities/__init__.py
--rw-r--r--   0        0        0      639 2023-06-13 10:51:29.694588 modelon_impact_client-3.0.3/modelon/impact/client/entities/asserts.py
--rw-r--r--   0        0        0    24767 2023-06-13 10:51:29.739589 modelon_impact_client-3.0.3/modelon/impact/client/entities/case.py
--rw-r--r--   0        0        0     2259 2023-06-13 10:51:29.748589 modelon_impact_client-3.0.3/modelon/impact/client/entities/content.py
--rw-r--r--   0        0        0     6620 2023-06-13 10:51:29.700588 modelon_impact_client-3.0.3/modelon/impact/client/entities/custom_function.py
--rw-r--r--   0        0        0    18419 2023-06-13 10:51:29.703588 modelon_impact_client-3.0.3/modelon/impact/client/entities/experiment.py
--rw-r--r--   0        0        0     2511 2023-06-13 10:51:29.693588 modelon_impact_client-3.0.3/modelon/impact/client/entities/external_result.py
--rw-r--r--   0        0        0        0 2023-06-13 10:51:29.747589 modelon_impact_client-3.0.3/modelon/impact/client/entities/interfaces/__init__.py
--rw-r--r--   0        0        0      180 2023-06-13 10:51:29.690588 modelon_impact_client-3.0.3/modelon/impact/client/entities/interfaces/case.py
--rw-r--r--   0        0        0      200 2023-06-13 10:51:29.725588 modelon_impact_client-3.0.3/modelon/impact/client/entities/interfaces/custom_function.py
--rw-r--r--   0        0        0      366 2023-06-13 10:51:29.717588 modelon_impact_client-3.0.3/modelon/impact/client/entities/interfaces/experiment.py
--rw-r--r--   0        0        0      192 2023-06-13 10:51:29.721588 modelon_impact_client-3.0.3/modelon/impact/client/entities/interfaces/external_result.py
--rw-r--r--   0        0        0      186 2023-06-13 10:51:29.719588 modelon_impact_client-3.0.3/modelon/impact/client/entities/interfaces/model.py
--rw-r--r--   0        0        0      190 2023-06-13 10:51:29.710588 modelon_impact_client-3.0.3/modelon/impact/client/entities/interfaces/model_executable.py
--rw-r--r--   0        0        0      190 2023-06-13 10:51:29.695588 modelon_impact_client-3.0.3/modelon/impact/client/entities/interfaces/workspace.py
--rw-r--r--   0        0        0      156 2023-06-13 10:51:29.714588 modelon_impact_client-3.0.3/modelon/impact/client/entities/log.py
--rw-r--r--   0        0        0    16840 2023-06-13 10:51:29.703588 modelon_impact_client-3.0.3/modelon/impact/client/entities/model.py
--rw-r--r--   0        0        0    12111 2023-06-13 10:51:29.698588 modelon_impact_client-3.0.3/modelon/impact/client/entities/model_executable.py
--rw-r--r--   0        0        0    12288 2023-06-13 10:51:29.746589 modelon_impact_client-3.0.3/modelon/impact/client/entities/project.py
--rw-r--r--   0        0        0     1986 2023-06-13 10:51:29.718588 modelon_impact_client-3.0.3/modelon/impact/client/entities/result.py
--rw-r--r--   0        0        0     1487 2023-06-13 10:51:29.690588 modelon_impact_client-3.0.3/modelon/impact/client/entities/status.py
--rw-r--r--   0        0        0    20712 2023-06-13 10:51:29.745589 modelon_impact_client-3.0.3/modelon/impact/client/entities/workspace.py
--rw-r--r--   0        0        0     1365 2023-06-13 10:51:29.701588 modelon_impact_client-3.0.3/modelon/impact/client/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-13 10:51:29.694588 modelon_impact_client-3.0.3/modelon/impact/client/experiment_definition/__init__.py
--rw-r--r--   0        0        0     5284 2023-06-13 10:51:29.750589 modelon_impact_client-3.0.3/modelon/impact/client/experiment_definition/asserts.py
--rw-r--r--   0        0        0     3085 2023-06-13 10:51:29.699588 modelon_impact_client-3.0.3/modelon/impact/client/experiment_definition/expansion.py
--rw-r--r--   0        0        0    10251 2023-06-13 10:51:29.691588 modelon_impact_client-3.0.3/modelon/impact/client/experiment_definition/extension.py
--rw-r--r--   0        0        0    12659 2023-06-13 10:51:29.733589 modelon_impact_client-3.0.3/modelon/impact/client/experiment_definition/fmu_based.py
--rw-r--r--   0        0        0        0 2023-06-13 10:51:29.727589 modelon_impact_client-3.0.3/modelon/impact/client/experiment_definition/interfaces/__init__.py
--rw-r--r--   0        0        0      506 2023-06-13 10:51:29.700588 modelon_impact_client-3.0.3/modelon/impact/client/experiment_definition/interfaces/definition.py
--rw-r--r--   0        0        0      409 2023-06-13 10:51:29.701588 modelon_impact_client-3.0.3/modelon/impact/client/experiment_definition/interfaces/expansion.py
--rw-r--r--   0        0        0      187 2023-06-13 10:51:29.687588 modelon_impact_client-3.0.3/modelon/impact/client/experiment_definition/interfaces/extension.py
--rw-r--r--   0        0        0    18576 2023-06-13 10:51:29.703588 modelon_impact_client-3.0.3/modelon/impact/client/experiment_definition/model_based.py
--rw-r--r--   0        0        0     4704 2023-06-13 10:51:29.693588 modelon_impact_client-3.0.3/modelon/impact/client/experiment_definition/operators.py
--rw-r--r--   0        0        0      641 2023-06-13 10:51:29.694588 modelon_impact_client-3.0.3/modelon/impact/client/experiment_definition/util.py
--rw-r--r--   0        0        0       65 2023-06-13 10:51:29.749589 modelon_impact_client-3.0.3/modelon/impact/client/jupyterhub/__init__.py
--rw-r--r--   0        0        0     3019 2023-06-13 10:51:29.732589 modelon_impact_client-3.0.3/modelon/impact/client/jupyterhub/authorize.py
--rw-r--r--   0        0        0      281 2023-06-13 10:51:29.751589 modelon_impact_client-3.0.3/modelon/impact/client/jupyterhub/exceptions.py
--rw-r--r--   0        0        0     2894 2023-06-13 10:51:29.702588 modelon_impact_client-3.0.3/modelon/impact/client/jupyterhub/sal.py
--rw-r--r--   0        0        0       79 2023-06-13 10:51:29.695588 modelon_impact_client-3.0.3/modelon/impact/client/operations/__init__.py
--rw-r--r--   0        0        0     5804 2023-06-13 10:51:29.705588 modelon_impact_client-3.0.3/modelon/impact/client/operations/base.py
--rw-r--r--   0        0        0     2439 2023-06-13 10:51:29.719588 modelon_impact_client-3.0.3/modelon/impact/client/operations/case.py
--rw-r--r--   0        0        0     2502 2023-06-13 10:51:29.720589 modelon_impact_client-3.0.3/modelon/impact/client/operations/content_import.py
--rw-r--r--   0        0        0     2243 2023-06-13 10:51:29.694588 modelon_impact_client-3.0.3/modelon/impact/client/operations/experiment.py
--rw-r--r--   0        0        0     2408 2023-06-13 10:51:29.722588 modelon_impact_client-3.0.3/modelon/impact/client/operations/external_result_import.py
--rw-r--r--   0        0        0     2719 2023-06-13 10:51:29.713588 modelon_impact_client-3.0.3/modelon/impact/client/operations/fmu_import.py
--rw-r--r--   0        0        0     5845 2023-06-13 10:51:29.749589 modelon_impact_client-3.0.3/modelon/impact/client/operations/model_executable.py
--rw-r--r--   0        0        0     2629 2023-06-13 10:51:29.754589 modelon_impact_client-3.0.3/modelon/impact/client/operations/project_import.py
--rw-r--r--   0        0        0        0 2023-06-13 10:51:29.697588 modelon_impact_client-3.0.3/modelon/impact/client/operations/workspace/__init__.py
--rw-r--r--   0        0        0     2599 2023-06-13 10:51:29.749589 modelon_impact_client-3.0.3/modelon/impact/client/operations/workspace/conversion.py
--rw-r--r--   0        0        0     3512 2023-06-13 10:51:29.750589 modelon_impact_client-3.0.3/modelon/impact/client/operations/workspace/exports.py
--rw-r--r--   0        0        0     2532 2023-06-13 10:51:29.734588 modelon_impact_client-3.0.3/modelon/impact/client/operations/workspace/imports.py
--rw-r--r--   0        0        0     3772 2023-06-13 10:51:29.743589 modelon_impact_client-3.0.3/modelon/impact/client/options.py
--rw-r--r--   0        0        0        0 2023-06-13 10:51:29.690588 modelon_impact_client-3.0.3/modelon/impact/client/py.typed
--rw-r--r--   0        0        0        0 2023-06-13 10:51:29.730589 modelon_impact_client-3.0.3/modelon/impact/client/sal/__init__.py
--rw-r--r--   0        0        0      132 2023-06-13 10:51:29.726589 modelon_impact_client-3.0.3/modelon/impact/client/sal/context.py
--rw-r--r--   0        0        0     1543 2023-06-13 10:51:29.706588 modelon_impact_client-3.0.3/modelon/impact/client/sal/custom_function.py
--rw-r--r--   0        0        0      671 2023-06-13 10:51:29.688588 modelon_impact_client-3.0.3/modelon/impact/client/sal/exceptions.py
--rw-r--r--   0        0        0     6785 2023-06-13 10:51:29.734588 modelon_impact_client-3.0.3/modelon/impact/client/sal/experiment.py
--rw-r--r--   0        0        0      629 2023-06-13 10:51:29.698588 modelon_impact_client-3.0.3/modelon/impact/client/sal/exports.py
--rw-r--r--   0        0        0     1475 2023-06-13 10:51:29.752589 modelon_impact_client-3.0.3/modelon/impact/client/sal/external_result.py
--rw-r--r--   0        0        0     3124 2023-06-13 10:51:29.723589 modelon_impact_client-3.0.3/modelon/impact/client/sal/http.py
--rw-r--r--   0        0        0      475 2023-06-13 10:51:29.753589 modelon_impact_client-3.0.3/modelon/impact/client/sal/imports.py
--rw-r--r--   0        0        0     3083 2023-06-13 10:51:29.742589 modelon_impact_client-3.0.3/modelon/impact/client/sal/model_executable.py
--rw-r--r--   0        0        0     4641 2023-06-13 10:51:29.735589 modelon_impact_client-3.0.3/modelon/impact/client/sal/project.py
--rw-r--r--   0        0        0     4877 2023-06-13 10:51:29.700588 modelon_impact_client-3.0.3/modelon/impact/client/sal/request.py
--rw-r--r--   0        0        0     5113 2023-06-13 10:51:29.718588 modelon_impact_client-3.0.3/modelon/impact/client/sal/response.py
--rw-r--r--   0        0        0     5082 2023-06-13 10:51:29.695588 modelon_impact_client-3.0.3/modelon/impact/client/sal/service.py
--rw-r--r--   0        0        0      884 2023-06-13 10:51:29.692588 modelon_impact_client-3.0.3/modelon/impact/client/sal/uri.py
--rw-r--r--   0        0        0      453 2023-06-13 10:51:29.708588 modelon_impact_client-3.0.3/modelon/impact/client/sal/users.py
--rw-r--r--   0        0        0     6995 2023-06-13 10:51:29.706588 modelon_impact_client-3.0.3/modelon/impact/client/sal/workspace.py
--rw-r--r--   0        0        0     1359 2023-06-13 10:54:39.668525 modelon_impact_client-3.0.3/pyproject.toml
--rw-r--r--   0        0        0     3722 1970-01-01 00:00:00.000000 modelon_impact_client-3.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1479 2023-07-31 12:28:14.191898 modelon_impact_client-3.1.0b1/LICENSE.md
+-rw-r--r--   0        0        0     2748 2023-07-31 12:28:14.212899 modelon_impact_client-3.1.0b1/README.md
+-rw-r--r--   0        0        0        0 2023-07-31 12:28:14.129898 modelon_impact_client-3.1.0b1/modelon/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 12:28:14.186898 modelon_impact_client-3.1.0b1/modelon/impact/__init__.py
+-rw-r--r--   0        0        0      832 2023-07-31 12:28:14.178898 modelon_impact_client-3.1.0b1/modelon/impact/client/__init__.py
+-rw-r--r--   0        0        0    28576 2023-07-31 12:28:14.135898 modelon_impact_client-3.1.0b1/modelon/impact/client/client.py
+-rw-r--r--   0        0        0      835 2023-07-31 12:28:14.214898 modelon_impact_client-3.1.0b1/modelon/impact/client/configuration.py
+-rw-r--r--   0        0        0     1938 2023-07-31 12:28:14.137898 modelon_impact_client-3.1.0b1/modelon/impact/client/credential_manager.py
+-rw-r--r--   0        0        0      119 2023-07-31 12:28:14.162898 modelon_impact_client-3.1.0b1/modelon/impact/client/entities/__init__.py
+-rw-r--r--   0        0        0      639 2023-07-31 12:28:14.124898 modelon_impact_client-3.1.0b1/modelon/impact/client/entities/asserts.py
+-rw-r--r--   0        0        0    24767 2023-07-31 12:28:14.211898 modelon_impact_client-3.1.0b1/modelon/impact/client/entities/case.py
+-rw-r--r--   0        0        0     2259 2023-07-31 12:28:14.241899 modelon_impact_client-3.1.0b1/modelon/impact/client/entities/content.py
+-rw-r--r--   0        0        0     6621 2023-07-31 12:28:14.138898 modelon_impact_client-3.1.0b1/modelon/impact/client/entities/custom_function.py
+-rw-r--r--   0        0        0    18419 2023-07-31 12:28:14.145898 modelon_impact_client-3.1.0b1/modelon/impact/client/entities/experiment.py
+-rw-r--r--   0        0        0     2511 2023-07-31 12:28:14.124898 modelon_impact_client-3.1.0b1/modelon/impact/client/entities/external_result.py
+-rw-r--r--   0        0        0        0 2023-07-31 12:28:14.237899 modelon_impact_client-3.1.0b1/modelon/impact/client/entities/interfaces/__init__.py
+-rw-r--r--   0        0        0      180 2023-07-31 12:28:14.117898 modelon_impact_client-3.1.0b1/modelon/impact/client/entities/interfaces/case.py
+-rw-r--r--   0        0        0      200 2023-07-31 12:28:14.185898 modelon_impact_client-3.1.0b1/modelon/impact/client/entities/interfaces/custom_function.py
+-rw-r--r--   0        0        0      366 2023-07-31 12:28:14.170898 modelon_impact_client-3.1.0b1/modelon/impact/client/entities/interfaces/experiment.py
+-rw-r--r--   0        0        0      192 2023-07-31 12:28:14.178898 modelon_impact_client-3.1.0b1/modelon/impact/client/entities/interfaces/external_result.py
+-rw-r--r--   0        0        0      186 2023-07-31 12:28:14.173898 modelon_impact_client-3.1.0b1/modelon/impact/client/entities/interfaces/model.py
+-rw-r--r--   0        0        0      190 2023-07-31 12:28:14.162898 modelon_impact_client-3.1.0b1/modelon/impact/client/entities/interfaces/model_executable.py
+-rw-r--r--   0        0        0      190 2023-07-31 12:28:14.126898 modelon_impact_client-3.1.0b1/modelon/impact/client/entities/interfaces/workspace.py
+-rw-r--r--   0        0        0      156 2023-07-31 12:28:14.166898 modelon_impact_client-3.1.0b1/modelon/impact/client/entities/log.py
+-rw-r--r--   0        0        0    16833 2023-07-31 12:28:14.146898 modelon_impact_client-3.1.0b1/modelon/impact/client/entities/model.py
+-rw-r--r--   0        0        0    12111 2023-07-31 12:28:14.131898 modelon_impact_client-3.1.0b1/modelon/impact/client/entities/model_executable.py
+-rw-r--r--   0        0        0    12306 2023-07-31 12:28:14.233899 modelon_impact_client-3.1.0b1/modelon/impact/client/entities/project.py
+-rw-r--r--   0        0        0     1986 2023-07-31 12:28:14.172898 modelon_impact_client-3.1.0b1/modelon/impact/client/entities/result.py
+-rw-r--r--   0        0        0     1487 2023-07-31 12:28:14.118898 modelon_impact_client-3.1.0b1/modelon/impact/client/entities/status.py
+-rw-r--r--   0        0        0    20870 2023-07-31 12:28:14.223899 modelon_impact_client-3.1.0b1/modelon/impact/client/entities/workspace.py
+-rw-r--r--   0        0        0     1365 2023-07-31 12:28:14.141898 modelon_impact_client-3.1.0b1/modelon/impact/client/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-31 12:28:14.125898 modelon_impact_client-3.1.0b1/modelon/impact/client/experiment_definition/__init__.py
+-rw-r--r--   0        0        0     5284 2023-07-31 12:28:14.252899 modelon_impact_client-3.1.0b1/modelon/impact/client/experiment_definition/asserts.py
+-rw-r--r--   0        0        0     4043 2023-07-31 12:28:14.136898 modelon_impact_client-3.1.0b1/modelon/impact/client/experiment_definition/expansion.py
+-rw-r--r--   0        0        0    10250 2023-07-31 12:28:14.119897 modelon_impact_client-3.1.0b1/modelon/impact/client/experiment_definition/extension.py
+-rw-r--r--   0        0        0    12658 2023-07-31 12:28:14.203899 modelon_impact_client-3.1.0b1/modelon/impact/client/experiment_definition/fmu_based.py
+-rw-r--r--   0        0        0        0 2023-07-31 12:28:14.188898 modelon_impact_client-3.1.0b1/modelon/impact/client/experiment_definition/interfaces/__init__.py
+-rw-r--r--   0        0        0      506 2023-07-31 12:28:14.138898 modelon_impact_client-3.1.0b1/modelon/impact/client/experiment_definition/interfaces/definition.py
+-rw-r--r--   0        0        0      409 2023-07-31 12:28:14.140898 modelon_impact_client-3.1.0b1/modelon/impact/client/experiment_definition/interfaces/expansion.py
+-rw-r--r--   0        0        0      187 2023-07-31 12:28:14.114898 modelon_impact_client-3.1.0b1/modelon/impact/client/experiment_definition/interfaces/extension.py
+-rw-r--r--   0        0        0    18583 2023-07-31 12:28:14.147898 modelon_impact_client-3.1.0b1/modelon/impact/client/experiment_definition/model_based.py
+-rw-r--r--   0        0        0     4699 2023-07-31 12:28:14.122897 modelon_impact_client-3.1.0b1/modelon/impact/client/experiment_definition/operators.py
+-rw-r--r--   0        0        0      641 2023-07-31 12:28:14.124898 modelon_impact_client-3.1.0b1/modelon/impact/client/experiment_definition/util.py
+-rw-r--r--   0        0        0       65 2023-07-31 12:28:14.247899 modelon_impact_client-3.1.0b1/modelon/impact/client/jupyterhub/__init__.py
+-rw-r--r--   0        0        0     3019 2023-07-31 12:28:14.200899 modelon_impact_client-3.1.0b1/modelon/impact/client/jupyterhub/authorize.py
+-rw-r--r--   0        0        0      281 2023-07-31 12:28:14.258899 modelon_impact_client-3.1.0b1/modelon/impact/client/jupyterhub/exceptions.py
+-rw-r--r--   0        0        0     2894 2023-07-31 12:28:14.141898 modelon_impact_client-3.1.0b1/modelon/impact/client/jupyterhub/sal.py
+-rw-r--r--   0        0        0       79 2023-07-31 12:28:14.127898 modelon_impact_client-3.1.0b1/modelon/impact/client/operations/__init__.py
+-rw-r--r--   0        0        0     5804 2023-07-31 12:28:14.150898 modelon_impact_client-3.1.0b1/modelon/impact/client/operations/base.py
+-rw-r--r--   0        0        0     2439 2023-07-31 12:28:14.174898 modelon_impact_client-3.1.0b1/modelon/impact/client/operations/case.py
+-rw-r--r--   0        0        0     2502 2023-07-31 12:28:14.176898 modelon_impact_client-3.1.0b1/modelon/impact/client/operations/content_import.py
+-rw-r--r--   0        0        0     2243 2023-07-31 12:28:14.125898 modelon_impact_client-3.1.0b1/modelon/impact/client/operations/experiment.py
+-rw-r--r--   0        0        0     2408 2023-07-31 12:28:14.180898 modelon_impact_client-3.1.0b1/modelon/impact/client/operations/external_result_import.py
+-rw-r--r--   0        0        0     2719 2023-07-31 12:28:14.165898 modelon_impact_client-3.1.0b1/modelon/impact/client/operations/fmu_import.py
+-rw-r--r--   0        0        0     5845 2023-07-31 12:28:14.248899 modelon_impact_client-3.1.0b1/modelon/impact/client/operations/model_executable.py
+-rw-r--r--   0        0        0     2629 2023-07-31 12:28:14.267899 modelon_impact_client-3.1.0b1/modelon/impact/client/operations/project_import.py
+-rw-r--r--   0        0        0        0 2023-07-31 12:28:14.131898 modelon_impact_client-3.1.0b1/modelon/impact/client/operations/workspace/__init__.py
+-rw-r--r--   0        0        0     2599 2023-07-31 12:28:14.249899 modelon_impact_client-3.1.0b1/modelon/impact/client/operations/workspace/conversion.py
+-rw-r--r--   0        0        0     3633 2023-07-31 12:28:14.253899 modelon_impact_client-3.1.0b1/modelon/impact/client/operations/workspace/exports.py
+-rw-r--r--   0        0        0     2532 2023-07-31 12:28:14.204898 modelon_impact_client-3.1.0b1/modelon/impact/client/operations/workspace/imports.py
+-rw-r--r--   0        0        0     3773 2023-07-31 12:28:14.218899 modelon_impact_client-3.1.0b1/modelon/impact/client/options.py
+-rw-r--r--   0        0        0        0 2023-07-31 12:28:14.118898 modelon_impact_client-3.1.0b1/modelon/impact/client/py.typed
+-rw-r--r--   0        0        0        0 2023-07-31 12:28:14.196898 modelon_impact_client-3.1.0b1/modelon/impact/client/sal/__init__.py
+-rw-r--r--   0        0        0      132 2023-07-31 12:28:14.188898 modelon_impact_client-3.1.0b1/modelon/impact/client/sal/context.py
+-rw-r--r--   0        0        0     1543 2023-07-31 12:28:14.153898 modelon_impact_client-3.1.0b1/modelon/impact/client/sal/custom_function.py
+-rw-r--r--   0        0        0      671 2023-07-31 12:28:14.115898 modelon_impact_client-3.1.0b1/modelon/impact/client/sal/exceptions.py
+-rw-r--r--   0        0        0     6785 2023-07-31 12:28:14.204898 modelon_impact_client-3.1.0b1/modelon/impact/client/sal/experiment.py
+-rw-r--r--   0        0        0      629 2023-07-31 12:28:14.134898 modelon_impact_client-3.1.0b1/modelon/impact/client/sal/exports.py
+-rw-r--r--   0        0        0     1475 2023-07-31 12:28:14.259899 modelon_impact_client-3.1.0b1/modelon/impact/client/sal/external_result.py
+-rw-r--r--   0        0        0     3124 2023-07-31 12:28:14.183898 modelon_impact_client-3.1.0b1/modelon/impact/client/sal/http.py
+-rw-r--r--   0        0        0      475 2023-07-31 12:28:14.265899 modelon_impact_client-3.1.0b1/modelon/impact/client/sal/imports.py
+-rw-r--r--   0        0        0     3083 2023-07-31 12:28:14.217898 modelon_impact_client-3.1.0b1/modelon/impact/client/sal/model_executable.py
+-rw-r--r--   0        0        0     4641 2023-07-31 12:28:14.205898 modelon_impact_client-3.1.0b1/modelon/impact/client/sal/project.py
+-rw-r--r--   0        0        0     4877 2023-07-31 12:28:14.138898 modelon_impact_client-3.1.0b1/modelon/impact/client/sal/request.py
+-rw-r--r--   0        0        0     5113 2023-07-31 12:28:14.173898 modelon_impact_client-3.1.0b1/modelon/impact/client/sal/response.py
+-rw-r--r--   0        0        0     5740 2023-07-31 12:28:14.126898 modelon_impact_client-3.1.0b1/modelon/impact/client/sal/service.py
+-rw-r--r--   0        0        0      884 2023-07-31 12:28:14.120898 modelon_impact_client-3.1.0b1/modelon/impact/client/sal/uri.py
+-rw-r--r--   0        0        0      453 2023-07-31 12:28:14.159898 modelon_impact_client-3.1.0b1/modelon/impact/client/sal/users.py
+-rw-r--r--   0        0        0     7383 2023-07-31 12:28:14.155898 modelon_impact_client-3.1.0b1/modelon/impact/client/sal/workspace.py
+-rw-r--r--   0        0        0     1366 2023-07-31 12:29:25.016631 modelon_impact_client-3.1.0b1/pyproject.toml
+-rw-r--r--   0        0        0     3724 1970-01-01 00:00:00.000000 modelon_impact_client-3.1.0b1/PKG-INFO
```

### Comparing `modelon_impact_client-3.0.3/LICENSE.md` & `modelon_impact_client-3.1.0b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/README.md` & `modelon_impact_client-3.1.0b1/README.md`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/__init__.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,8 +19,8 @@
     Sobol,
     FullFactorial,
     LatinHypercube,
 )
 from modelon.impact.client.entities.project import ContentType
 from modelon.impact.client.entities.workspace import WorkspaceDefinition
 
-SimpleExperimentDefinition = SimpleFMUExperimentDefinition  # For compability
+SimpleExperimentDefinition = SimpleFMUExperimentDefinition  # For compatibility
```

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/client.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,14 +31,42 @@
 
 @enum.unique
 class ExecutionKind(enum.Enum):
     COMPILATION = 'COMPILATION'
     EXPERIMENT = 'EXPERIMENT'
 
 
+@enum.unique
+class SharedWorkspaceUploadStatus(enum.Enum):
+    INITIALIZING = 'initializing'
+    CREATED = 'created'
+    DELETING = 'deleting'
+
+
+@dataclass
+class SharedWorkspaceSnapshot:
+    id: str
+    workspace_id: str
+    workspace_name: str
+    group: str
+    size: int
+    status: SharedWorkspaceUploadStatus
+
+    @classmethod
+    def from_dict(cls, data: Dict[str, Any]) -> SharedWorkspaceSnapshot:
+        return cls(
+            id=data['id'],
+            workspace_id=data['workspaceId'],
+            workspace_name=data['displayName'],
+            group=data['group'],
+            size=data['size'],
+            status=SharedWorkspaceUploadStatus(data['status']),
+        )
+
+
 @dataclass
 class Execution:
     kind: ExecutionKind
     workspace_id: str
     id: str
 
     @classmethod
@@ -167,22 +195,26 @@
                 shared_definition, selections
             ).wait()
 
         """
         return [e.make_selection_interactive() for e in self.entries]
 
 
+def _bool_to_str(boolean: bool) -> str:
+    return "true" if boolean else "false"
+
+
 class Client:
     """This Class contains methods to authenticate logins, create new
     workspaces and upload or fetch existing workspaces.
 
     Args:
         url:
             The URL for Modelon Impact client host. Defaults to the value specified
-            by env variable 'MODELON_IMPACT_CLIENT_URL' if set else uses the URL
+            by environment variable 'MODELON_IMPACT_CLIENT_URL' if set else uses the URL
             'https://impact.modelon.cloud/'.
         interactive:
             If True the client will prompt for an API key if no other login information
             can be found. An API key entered for this prompt will be saved to disk
             and re-used next time the Client is instantiated. If False no prompt will
             be given if no other login information can be found and login will be done
             as if no API key was given (anonymous login).
@@ -302,15 +334,15 @@
                 "No Modelon Impact API key could be found, "
                 "will log in as anonymous user. Permissions may be limited"
             )
 
         self._sal.api_login(api_key=api_key)
         if api_key and interactive:
             # Save the api_key for next time if
-            # running interactively and login was successfuly
+            # running interactively and login was successfully
             self._credential_manager.write_key_to_file(api_key)
 
         return api_key
 
     def get_workspace(self, workspace_id: str) -> Workspace:
         """Returns a Workspace class object.
 
@@ -557,14 +589,33 @@
             if selections
             else None,
         )
         return WorkspaceImportOperation[Workspace](
             resp["data"]["location"], self._sal, Workspace.from_import_operation
         )
 
+    def import_workspace_from_blob(self, sharing_id: str) -> WorkspaceImportOperation:
+        """Imports a shared workspace snapshot via sharing ID.
+
+        Args:
+            sharing_id: The ID of the shared workspace.
+
+        Returns:
+            A WorkspaceImportOperation class object.
+
+        Example::
+
+            client.import_workspace_from_blob("ncjdnjdnjcnjd").wait()
+
+        """
+        resp = self._sal.workspace.import_from_blob(sharing_id)
+        return WorkspaceImportOperation[Workspace](
+            resp["data"]["location"], self._sal, Workspace.from_import_operation
+        )
+
     def get_project_matchings(
         self, shared_definition: WorkspaceDefinition
     ) -> ProjectMatchings:
         """Returns all projects matchings that would happen during a workspace import.
         As import will fail if there are multiple possible matchings of local projects
         for a project, this method is used to get these matchings which can be
         resolved to an unequivocal 'selection'. Selections are used as (optional) input
@@ -667,15 +718,15 @@
         if execution.kind == ExecutionKind.EXPERIMENT:
             return self._experiment_operation_from_execution(execution)
         return self._model_executable_operation_from_execution(execution)
 
     def get_executions(
         self, workspace_id: Optional[str] = None
     ) -> Iterable[Optional[Union[ExperimentOperation, ModelExecutableOperation]]]:
-        """Yields running/acitve executions.
+        """Yields running/active executions.
 
         Args:
             workspace_id: The id of the workspace.
 
         Yields:
             An ExperimentOperation or a ModelExecutableOperation class.
 
@@ -686,7 +737,78 @@
         """
         executions = self._sal.get_executions()["data"]["items"]
         for execution in executions:
             execution = Execution.from_dict(execution)
             if workspace_id and execution.workspace_id != workspace_id:
                 continue
             yield self._operation_from_execution(execution)
+
+    def get_my_snapshots(
+        self,
+        *,
+        workspace_id: str = "",
+        only_latest: bool = False,
+        first: int = 0,
+        maximum: int = 20,
+        has_data: bool = False,
+    ) -> List[SharedWorkspaceSnapshot]:
+        """Returns a list of snapshots owned by the logged in user. The
+        snapshots could be filtered based on the key-worded arguments.
+
+        Args:
+            workspace_id: ID of the workspace.
+            only_latest: If true, then only returns the latest version for
+            each "workspace_id".
+            first: Index of first matching resource to return.
+            maximum: Maximum number of resources to return.
+            has_data: If true, filters with status==SharedWorkspaceUploadStatus.CREATED.
+             If false returns everything.
+
+        Returns:
+            A list of workspace snapshot class objects.
+
+        Example::
+
+            client.get_my_snapshots()
+
+        """
+        query = {}
+        if workspace_id:
+            query["workspaceId"] = workspace_id
+        if only_latest:
+            query["onlyLatest"] = _bool_to_str(only_latest)
+        if has_data:
+            query["hasData"] = _bool_to_str(has_data)
+        if first > 0:
+            query["first"] = str(first)
+        if maximum >= 0:
+            query["max"] = str(maximum)
+        query_args = '&'.join(f'{key}={value}' for key, value in query.items())
+        data = self._sal.get_shared_workspaces(query_args)["data"]["items"]
+        return [SharedWorkspaceSnapshot.from_dict(item) for item in data]
+
+    def get_snapshot(self, sharing_id: str) -> SharedWorkspaceSnapshot:
+        """Returns the workspace snapshot class object with the given ID.
+
+        Args:
+            sharing_id: ID of the workspace snapshot.
+
+        Returns:
+            The workspace snapshot class object.
+
+        Example::
+
+            client.get_snapshot("2h98hciwsniucwincj")
+
+        """
+        data = self._sal.get_shared_workspace(sharing_id)
+        return SharedWorkspaceSnapshot.from_dict(data)
+
+    def delete_snapshot(self, sharing_id: str) -> None:
+        """Deletes the workspace snapshot with the given ID.
+
+        Example::
+
+            client.delete_snapshot("2839283ur8ewjfuehfu")
+
+        """
+        self._sal.delete_shared_workspace(sharing_id)
```

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/configuration.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/configuration.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/credential_manager.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/credential_manager.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/entities/asserts.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/entities/asserts.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/entities/case.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/entities/case.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/entities/content.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/entities/content.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/entities/custom_function.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/entities/custom_function.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         "Custom function name"
         return self._name
 
     def with_parameters(self, **modified: Any) -> CustomFunction:
         """Sets/updates the custom_function parameters for an experiment.
 
         Args:
-            parameters: A keyworded, variable-length argument list of custom_function
+            parameters: A key-worded, variable-length argument list of custom_function
                 parameters.
 
         Example::
 
             custom_function.with_parameters(start_time=0.0, final_time=2.0)
 
         """
```

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/entities/experiment.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/entities/experiment.py`

 * *Files 0% similar despite different names*

```diff
@@ -405,15 +405,15 @@
         )
 
     def get_trajectories(self, variables: List[str]) -> Dict[str, Any]:
         """Returns a dictionary containing the result trajectories for a list
         of result variables for all the cases.
 
         Args:
-            variables: A list of result variables to fecth trajectories for.
+            variables: A list of result variables to fetch trajectories for.
 
         Returns:
             A dictionary object containing the result trajectories for all cases.
 
         Raises:
             OperationNotCompleteError if simulation process is in progress.
             OperationFailureError if simulation process was cancelled.
```

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/entities/external_result.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/entities/external_result.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/entities/model.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/entities/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,15 +323,15 @@
                 not matching the pattern as model variables. If top_level_inputs = '',
                 then no input is imported as an input.
                 Default value: None (which means all inputs are kept as inputs)
                 Type: str or a list of strings
             step_size:
                 Specify what value to set for the parameter for step size in the
                 generated model. By default the parameter is set to zero, which
-                inturn means that the step size will be set during simulation based
+                means that the step size will be set during simulation based
                 on simulation properties such as the time interval.
                 This can also be manually set to any real non-negative number.
                 The value of the step size parameter can also be set via the function
                 set_step_size, which must be invoked before importing the model.
                 Default value: 0.0 (which during simulation is set according to the
                 description above).
```

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/entities/model_executable.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/entities/model_executable.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/entities/project.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/entities/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,20 +25,20 @@
     LOCAL = 'LOCAL'
     RELEASED = 'RELEASED'
     SYSTEM = 'SYSTEM'
 
 
 @dataclass
 class GitRepoURL:
-    """GitRepoURL represents a project referenced in a git repo String
+    """GitRepoURL represents a project referenced in a git repository String
     representation is url[@[refname][:sha1]]"""
 
     url: str
     """URL without protocol part, e.g.,
-    gitlab.modelon.com/group/project/repo."""
+    gitlab.modelon.com/group/project/repository."""
 
     refname: str = ""
     """Reference name (branch, tag or similar)"""
 
     sha1: str = ""
     """Commit hash."""
 
@@ -57,16 +57,16 @@
         return cls(
             url=data.get("url"), refname=data.get("refname"), sha1=data.get("sha1")
         )
 
 
 @dataclass
 class SvnRepoURL:
-    """SvnRepoURL represents a project referenced in a Subversion repo String
-    representation is url/trunk/subdir[@[rev]]"""
+    """SvnRepoURL represents a project referenced in a Subversion repository
+    String representation is url/trunk/subdir[@[rev]]"""
 
     root_url: str
     """URL without protocol part up to branch part, e.g.,
     svn.modelon.com/PNNN/"""
 
     branch: str = ""
     """Non-empty if it's standard layout and can be either trunk or
```

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/entities/result.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/entities/result.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/entities/status.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/entities/status.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/entities/workspace.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/entities/workspace.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,29 +268,34 @@
         resp = self._sal.external_result.result_upload(
             self._workspace_id, path_to_result, label=label, description=description
         )
         return ExternalResultImportOperation[ExternalResult](
             resp["data"]["location"], self._sal, ExternalResult.from_operation
         )
 
-    def export(self) -> WorkspaceExportOperation:
+    def export(self, blob_storage: bool = False) -> WorkspaceExportOperation:
         """Exports the workspace as a binary compressed archive. Similar to
         :obj:`~modelon.impact.client.entities.workspace.Workspace.download`,
         but gives more control for getting the workspace async.
         Returns an modelon.impact.client.operations.workspace.exports
         .WorkspaceExportOperation class object.
 
+        Args:
+            blob_storage: To export the workspace and save it to blob storage.
+
         Returns:
             An WorkspaceExportOperation class object.
 
         Example::
 
             path = workspace.export().wait().download_as('/home/workspace.zip')
         """
-        resp = self._sal.workspace.workspace_export_setup(self._workspace_id)
+        resp = self._sal.workspace.workspace_export_setup(
+            self._workspace_id, blob_storage
+        )
         return WorkspaceExportOperation[Workspace](
             resp["data"]["location"], self._sal, Export.from_operation
         )
 
     def download(self, path: str) -> str:
         """Downloads the workspace as a binary compressed archive. Returns the
         local path to the downloaded workspace archive. Similar to
@@ -484,15 +489,15 @@
     ) -> List[Project]:
         """Return the list of projects for a workspace.
 
         Args:
             vcs_info: If True, the versioning details are returned for the
             project(if under version control).
             include_disabled: If True, projects disabled in the workspace
-            are also lsited.
+            are also listed.
 
         Returns:
             A list of Project class objects.
 
         Example::
 
             projects = workspace.get_projects()
@@ -518,15 +523,15 @@
     ) -> List[Project]:
         """Return the list of project dependencies for a workspace.
 
         Args:
             vcs_info: If True, the versioning details are returned for the
             project(if under version control).
             include_disabled: If True, projects disabled in the workspace
-            are also lsited.
+            are also listed.
 
         Returns:
             A list of Project class object.
 
         Example::
 
             dependencies = workspace.get_dependencies()
```

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/exceptions.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/experiment_definition/asserts.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/experiment_definition/asserts.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/experiment_definition/extension.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/experiment_definition/extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         raise ValueError(
             "Cannot initialize from an experiment containing multiple"
             " cases! Please specify a case object instead."
         )
 
 
 class SimpleExperimentExtension(BaseExperimentExtension):
-    """A simple experiment extension class for defining experiement extensions.
+    """A simple experiment extension class for defining experiment extensions.
 
     Args:
         parameter_modifiers: The custom function parameters passes as a dictionary.
             By default, the parameter_modifier is set to None, which means the options
             set in the experiment definition will be used.
         solver_options: A solver options class instance of SolverOptions or
             a dictionary object containing the solver options. By
```

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/experiment_definition/fmu_based.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/experiment_definition/fmu_based.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         )
 
 
 class SimpleFMUExperimentDefinition(BaseExperimentDefinition):
     """A simple experiment definition class for defining experiments.
 
     Args:
-        fmu: The FMU to be excecuted for this experiment.
+        fmu: The FMU to be executed for this experiment.
         custom_function: The custom function to use for this experiment.
 
         solver_options: The solver options to use for this experiment.
             By default, the options is set to None, which means the
             default options for the custom_function input is used.
         simulation_options: The simulation_options to use for this
             experiment. By default, the options is set to None, which
```

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/experiment_definition/model_based.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/experiment_definition/model_based.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,21 +204,21 @@
 
     def with_expansion(
         self, expansion: Optional[Type[ExpansionAlgorithm]] = None
     ) -> SimpleModelicaExperimentDefinition:
         """Sets the expansion algorithm for an experiment.
 
         Args:
-            expansion: An expansion algorithm. Avaialable algorithms are LatinHypercube,
+            expansion: An expansion algorithm. Available algorithms are LatinHypercube,
                 Sobol and FullFactorial.
                 Default: FullFactorial.
 
         Example::
 
-            from modelon.impact.client import Sobol, Beta
+            from modelon.impact.client import Sobol, Beta, Normal
 
             model = workspace.get_model("Modelica.Blocks.Examples.PID_Controller")
             experiment_definition = model.new_experiment_definition(
                 custom_function).with_modifiers({'inertia1.J': Beta(0.1, 0.9),
                 'inertia2.J': Normal(0.1, 0.5)}).with_expansion(Sobol(5))
 
         """
```

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/experiment_definition/operators.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/experiment_definition/operators.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     @abstractmethod
     def __str__(self) -> str:
         "Returns a string representation of the operator"
 
 
 @dataclass
 class Range(Operator):
-    """Range operator class for parameterizing batch runs. Range(a, b, c)
+    """Range operator class for parametrizing batch runs. Range(a, b, c)
     represents c linearly spaced values in the (real) interval [a, b]; b >= a.
     The functionality is analogous to numpy.linspace.
 
     Args:
         start_value: The start value for the sweep parameter.
         end_value: The end value for the sweep parameter.
         no_of_steps: The number of steps to intermediate steps
@@ -40,15 +40,15 @@
     no_of_steps: int
 
     def __str__(self) -> str:
         return f"range({self.start_value},{self.end_value},{self.no_of_steps})"
 
 
 class Choices(Operator):
-    """Choices operator class for parameterizing batch runs. Choices defines a
+    """Choices operator class for parametrizing batch runs. Choices defines a
     list of specified values a Modifier expression can take.
 
     Args:
         values: Variable number of numerical arguments to sweep.
 
     Example::
 
@@ -66,16 +66,16 @@
 
     def __str__(self) -> str:
         return f"choices({', '.join(map(str, self.values))})"
 
 
 @dataclass
 class Uniform(Operator):
-    """Uniform distribution class for parameterizing batch runs.For
-    mathematical background, see e.g.,
+    """Uniform distribution class for parametrizing batch runs.For mathematical
+    background, see e.g.,
     https://en.wikipedia.org/wiki/Continuous_uniform_distribution.
 
     Args:
         start (float): Starting value of the interval.
         end (float): End value of the interval. Requires start <= end.
 
     Example::
@@ -94,15 +94,15 @@
 
     def __str__(self) -> str:
         return f"uniform({self.start},{self.end})"
 
 
 @dataclass
 class Beta(Operator):
-    """Beta distribution class for parameterizing batch runs. For mathematical
+    """Beta distribution class for parametrizing batch runs. For mathematical
     background, see e.g., https://en.wikipedia.org/wiki/Beta_distribution.
 
     Args:
         alpha (float): 'alpha' resp. 'a' parameter of beta distribution, requires
             alpha > 0
         beta (float): 'beta' resp. 'b' parameter of beta distribution, requires
             beta > 0
@@ -123,15 +123,15 @@
 
     def __str__(self) -> str:
         return f"beta({self.alpha},{self.alpha})"
 
 
 @dataclass
 class Normal(Operator):
-    """Normal distribution class for parameterizing batch runs.For mathematical
+    """Normal distribution class for parametrizing batch runs.For mathematical
     background, see e.g., https://en.wikipedia.org/wiki/Normal_distribution
     https://en.wikipedia.org/wiki/Truncated_normal_distribution Supports both
     the standard and truncated Normal distribution. The standard Normal
     distribution is the default, add additional start & end parameters for
     truncation.
 
     Args:
```

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/experiment_definition/util.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/experiment_definition/util.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/jupyterhub/authorize.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/jupyterhub/authorize.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/jupyterhub/sal.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/jupyterhub/sal.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/operations/base.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/operations/base.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/operations/case.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/operations/case.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/operations/content_import.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/operations/content_import.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/operations/experiment.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/operations/experiment.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/operations/external_result_import.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/operations/external_result_import.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/operations/fmu_import.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/operations/fmu_import.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/operations/model_executable.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/operations/model_executable.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/operations/project_import.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/operations/project_import.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/operations/workspace/conversion.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/operations/workspace/conversion.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/operations/workspace/exports.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/operations/workspace/exports.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,19 @@
 
 
 class Export:
     def __init__(self, export_service: ExportService, download_uri: str):
         self._export_sal = export_service
         self._download_uri = download_uri
 
+    @property
+    def id(self) -> str:
+        """ID of the export."""
+        return self._download_uri.split('/')[-1]
+
     def download_as(self, path_to_download: str) -> str:
         """Writes the binary archive to a file. Returns the path to downloaded
         archive.
 
         Args:
             path_to_download: The path to store the downloaded workspace.
```

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/operations/workspace/imports.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/operations/workspace/imports.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/options.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     def __len__(self) -> int:
         return self._values.__len__()
 
     def with_values(self, **modified: Any) -> Any:
         """Sets/updates the options.
 
         Args:
-            parameters: A keyworded, variable-length argument list of options.
+            parameters: A key-worded, variable-length argument list of options.
 
         Example::
 
             cmp_opts = custom_function.get_compiler_options().with_values(
                 c_compiler='gcc')
             runtime_opts = custom_function.get_runtime_options().with_values(
                 cs_solver=0)
```

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/sal/custom_function.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/sal/custom_function.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/sal/exceptions.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/sal/exceptions.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/sal/experiment.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/sal/experiment.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/sal/exports.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/sal/exports.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/sal/external_result.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/sal/external_result.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/sal/http.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/sal/http.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/sal/model_executable.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/sal/model_executable.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/sal/project.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/sal/project.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/sal/request.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/sal/request.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/sal/response.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/sal/response.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/sal/service.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/sal/service.py`

 * *Files 17% similar despite different names*

```diff
@@ -114,7 +114,21 @@
         url = (self._base_uri / "api/login").resolve()
         return self._http_client.post_json(url, login_data)
 
     def get_executions(self) -> Dict[str, Any]:
         url = (self._base_uri / "api/executions").resolve()
         resp = self._http_client.get_json_response(url)
         return resp.data
+
+    def get_shared_workspaces(self, query_args: str) -> Dict[str, Any]:
+        url = (self._base_uri / f"api/shared-workspaces?{query_args}").resolve()
+        resp = self._http_client.get_json_response(url)
+        return resp.data
+
+    def get_shared_workspace(self, sharing_id: str) -> Dict[str, Any]:
+        url = (self._base_uri / f"api/shared-workspaces/{sharing_id}").resolve()
+        resp = self._http_client.get_json_response(url)
+        return resp.data
+
+    def delete_shared_workspace(self, sharing_id: str) -> None:
+        url = (self._base_uri / f"api/shared-workspaces/{sharing_id}").resolve()
+        self._http_client.delete_json(url)
```

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/sal/uri.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/sal/uri.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.3/modelon/impact/client/sal/workspace.py` & `modelon_impact_client-3.1.0b1/modelon/impact/client/sal/workspace.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,17 +47,19 @@
         url = (
             self._base_uri
             / f"api/workspaces/{workspace_id}/dependencies?vcsInfo={vcs_info}"
             f"&includeDisabled={include_disabled}"
         ).resolve()
         return self._http_client.get_json(url)
 
-    def workspace_export_setup(self, workspace_id: str) -> Dict[str, Any]:
+    def workspace_export_setup(
+        self, workspace_id: str, blob_storage: bool
+    ) -> Dict[str, Any]:
         url = (self._base_uri / "api/workspace-exports").resolve()
-        body = {"workspaceId": workspace_id}
+        body = {"workspaceId": workspace_id, 'blobStorage': blob_storage}
         return self._http_client.post_json(url, body=body)
 
     def workspace_conversion_setup(
         self, workspace_id: str, backup_name: Optional[str]
     ) -> Dict[str, Any]:
         url = (self._base_uri / "api/workspace-conversions").resolve()
         backup_data = {'backup': {'name': backup_name}} if backup_name else {}
@@ -144,14 +146,22 @@
             shared_definition = {
                 **shared_definition,
                 **{"selectedMatchings": {"entries": selected_matchings}},
             }
         url = (self._base_uri / "api/workspace-imports").resolve()
         return self._http_client.post_json(url, body=shared_definition)
 
+    def import_from_blob(self, sharing_id: str) -> Dict[str, Any]:
+        url = (self._base_uri / "api/workspace-imports").resolve()
+        return self._http_client.post_json(
+            url,
+            headers={"Accept": "application/vnd.impact.shared-snapshot.v1+json"},
+            body={"id": sharing_id},
+        )
+
     def get_project_matchings(
         self, shared_definition: Dict[str, Any]
     ) -> Dict[str, Any]:
         url = (self._base_uri / "api/workspace-imports-matchings").resolve()
         return self._http_client.post_json(url, body=shared_definition)
 
     def import_project_from_zip(
```

### Comparing `modelon_impact_client-3.0.3/pyproject.toml` & `modelon_impact_client-3.1.0b1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "modelon-impact-client"
 packages = [
     { include = "modelon" },
 ]
-version = "3.0.3"
+version = "3.1.0-beta.1"
 description = "Client library for easy scripting against Modelon Impact"
 readme = "README.md"
 homepage = "https://www.modelon.com/modelon-impact"
 repository = "https://github.com/modelon-community/impact-client-python"
 documentation = "https://modelon-impact-client.readthedocs.io"
 license = "BSD"
 authors = [
```

### Comparing `modelon_impact_client-3.0.3/PKG-INFO` & `modelon_impact_client-3.1.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelon-impact-client
-Version: 3.0.3
+Version: 3.1.0b1
 Summary: Client library for easy scripting against Modelon Impact
 Home-page: https://www.modelon.com/modelon-impact
 License: BSD
 Keywords: impact,client,API
 Author: WEP
 Author-email: impact@modelon.com
 Requires-Python: >=3.9.0,<4.0.0
```

