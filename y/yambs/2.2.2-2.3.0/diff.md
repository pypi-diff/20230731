# Comparing `tmp/yambs-2.2.2.tar.gz` & `tmp/yambs-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yambs-2.2.2.tar", last modified: Sun Jul 30 05:10:34 2023, max compression
+gzip compressed data, was "yambs-2.3.0.tar", last modified: Mon Jul 31 05:26:30 2023, max compression
```

## Comparing `yambs-2.2.2.tar` & `yambs-2.3.0.tar`

### file list

```diff
@@ -1,111 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:10:34.505795 yambs-2.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-30 05:09:07.000000 yambs-2.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-30 05:10:34.505795 yambs-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8840 2023-07-30 05:09:07.000000 yambs-2.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-30 05:09:07.000000 yambs-2.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 05:10:34.505795 yambs-2.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-30 05:09:07.000000 yambs-2.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:10:34.497794 yambs-2.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-30 05:09:07.000000 yambs-2.2.2/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-30 05:09:07.000000 yambs-2.2.2/tests/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:10:34.497794 yambs-2.2.2/yambs/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:10:34.497794 yambs-2.2.2/yambs/aggregation/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/aggregation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:10:34.497794 yambs-2.2.2/yambs/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/commands/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/commands/gen.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/commands/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/commands/uf2conv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:10:34.497794 yambs-2.2.2/yambs/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/config/board.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/config/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/config/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:10:34.497794 yambs-2.2.2/yambs/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:10:34.501795 yambs-2.2.2/yambs/data/includes/
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/data/includes/chips.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/data/includes/common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/data/includes/infineon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/data/includes/microchip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/data/native.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:10:34.501795 yambs-2.2.2/yambs/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/data/schemas/Architecture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/data/schemas/Board.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/data/schemas/Chip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/data/schemas/CommonConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/data/schemas/Dependency.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/data/schemas/Github.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/data/schemas/Native.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/data/schemas/Project.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/data/schemas/Toolchain.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/data/schemas/Variant.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/data/schemas/config_common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/data/schemas/entry_common.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/data/schemas/toolchain_common.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:10:34.501795 yambs-2.2.2/yambs/data/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/data/templates/all.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/data/templates/architecture.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/data/templates/board.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/data/templates/build.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/data/templates/chip.ld.j2
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/data/templates/chip.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/data/templates/compile_commands.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/data/templates/native_all.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/data/templates/native_build.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/data/templates/native_rules.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/data/templates/rules.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/data/templates/toolchain.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/data/templates/variant.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/data/uf2families.json
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/data/yambs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:10:34.501795 yambs-2.2.2/yambs/dependency/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/dependency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/dependency/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/dependency/github.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:10:34.505795 yambs-2.2.2/yambs/dependency/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/dependency/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/dependency/handlers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/dependency/handlers/yambs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/dependency/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/dependency/state.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/dev_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:10:34.505795 yambs-2.2.2/yambs/dist/
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/dist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:10:34.505795 yambs-2.2.2/yambs/environment/
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/environment/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:10:34.505795 yambs-2.2.2/yambs/generate/
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/generate/architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/generate/boards.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/generate/chips.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/generate/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:10:34.505795 yambs-2.2.2/yambs/generate/ninja/
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/generate/ninja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/generate/ninja/format.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/generate/toolchains.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/generate/variants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:10:34.505795 yambs-2.2.2/yambs/github/
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:10:34.505795 yambs-2.2.2/yambs/translation/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/translation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:10:34.505795 yambs-2.2.2/yambs/uf2/
--rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-07-30 05:09:07.000000 yambs-2.2.2/yambs/uf2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 05:10:34.497794 yambs-2.2.2/yambs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-30 05:10:34.000000 yambs-2.2.2/yambs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-30 05:10:34.000000 yambs-2.2.2/yambs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 05:10:34.000000 yambs-2.2.2/yambs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-30 05:10:34.000000 yambs-2.2.2/yambs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-30 05:10:34.000000 yambs-2.2.2/yambs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-30 05:10:34.000000 yambs-2.2.2/yambs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.878316 yambs-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-31 05:25:07.000000 yambs-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-31 05:26:30.878316 yambs-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8840 2023-07-31 05:25:07.000000 yambs-2.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-31 05:25:07.000000 yambs-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 05:26:30.878316 yambs-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-31 05:25:07.000000 yambs-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.866316 yambs-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-31 05:25:07.000000 yambs-2.3.0/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-31 05:25:07.000000 yambs-2.3.0/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.866316 yambs-2.3.0/yambs/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.870316 yambs-2.3.0/yambs/aggregation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/aggregation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.870316 yambs-2.3.0/yambs/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/commands/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/commands/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/commands/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/commands/uf2conv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.870316 yambs-2.3.0/yambs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/config/board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/config/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/config/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.870316 yambs-2.3.0/yambs/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.870316 yambs-2.3.0/yambs/data/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/includes/chips.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/includes/common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/includes/infineon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/includes/microchip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/native.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.874316 yambs-2.3.0/yambs/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/schemas/Architecture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/schemas/Board.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/schemas/Chip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/schemas/CommonConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/schemas/Dependency.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/schemas/Github.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/schemas/Native.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/schemas/Project.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/schemas/Toolchain.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/schemas/Variant.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/schemas/config_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/schemas/entry_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/schemas/toolchain_common.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.874316 yambs-2.3.0/yambs/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/templates/all.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/templates/architecture.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/templates/board.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/templates/build.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/templates/chip.ld.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/templates/chip.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/templates/compile_commands.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/templates/native_all.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/templates/native_build.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/templates/native_rules.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/templates/rules.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/templates/toolchain.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/templates/variant.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/uf2families.json
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/data/yambs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.874316 yambs-2.3.0/yambs/dependency/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/dependency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/dependency/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/dependency/github.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.874316 yambs-2.3.0/yambs/dependency/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/dependency/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/dependency/handlers/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.874316 yambs-2.3.0/yambs/dependency/handlers/yambs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/dependency/handlers/yambs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/dependency/handlers/yambs/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/dependency/handlers/yambs/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/dependency/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/dependency/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/dev_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.874316 yambs-2.3.0/yambs/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/dist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.874316 yambs-2.3.0/yambs/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/environment/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.878316 yambs-2.3.0/yambs/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/generate/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/generate/boards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/generate/chips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/generate/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.878316 yambs-2.3.0/yambs/generate/ninja/
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/generate/ninja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/generate/ninja/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/generate/toolchains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/generate/variants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.878316 yambs-2.3.0/yambs/github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.878316 yambs-2.3.0/yambs/translation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/translation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.878316 yambs-2.3.0/yambs/uf2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-07-31 05:25:07.000000 yambs-2.3.0/yambs/uf2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:26:30.870316 yambs-2.3.0/yambs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-31 05:26:30.000000 yambs-2.3.0/yambs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-07-31 05:26:30.000000 yambs-2.3.0/yambs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 05:26:30.000000 yambs-2.3.0/yambs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-31 05:26:30.000000 yambs-2.3.0/yambs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-31 05:26:30.000000 yambs-2.3.0/yambs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 05:26:30.000000 yambs-2.3.0/yambs.egg-info/top_level.txt
```

### Comparing `yambs-2.2.2/LICENSE` & `yambs-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/PKG-INFO` & `yambs-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 2.2.2
+Version: 2.3.0
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
@@ -18,19 +18,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=c6f67ebd8082d4ff4435729188bd6f43
+    hash=da0d2fd90a670c981a7628b6eb8a2c87
     =====================================
 -->
 
-# yambs ([2.2.2](https://pypi.org/project/yambs/))
+# yambs ([2.3.0](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-2.2.2/README.md` & `yambs-2.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=c6f67ebd8082d4ff4435729188bd6f43
+    hash=da0d2fd90a670c981a7628b6eb8a2c87
     =====================================
 -->
 
-# yambs ([2.2.2](https://pypi.org/project/yambs/))
+# yambs ([2.3.0](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-2.2.2/pyproject.toml` & `yambs-2.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "yambs"
-version = "2.2.2"
+version = "2.3.0"
 description = "Yet another meta build-system."
 readme = "README.md"
 requires-python = ">=3.11"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `yambs-2.2.2/setup.py` & `yambs-2.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/tests/test_entry.py` & `yambs-2.3.0/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/aggregation/__init__.py` & `yambs-2.3.0/yambs/aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/app.py` & `yambs-2.3.0/yambs/app.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/commands/all.py` & `yambs-2.3.0/yambs/commands/all.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/commands/common.py` & `yambs-2.3.0/yambs/commands/common.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/commands/dist.py` & `yambs-2.3.0/yambs/commands/dist.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/commands/gen.py` & `yambs-2.3.0/yambs/commands/gen.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/commands/native.py` & `yambs-2.3.0/yambs/commands/native.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/commands/uf2conv.py` & `yambs-2.3.0/yambs/commands/uf2conv.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/config/__init__.py` & `yambs-2.3.0/yambs/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/config/board.py` & `yambs-2.3.0/yambs/config/board.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/config/common.py` & `yambs-2.3.0/yambs/config/common.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/data/includes/chips.yaml` & `yambs-2.3.0/yambs/data/includes/chips.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/data/includes/infineon.yaml` & `yambs-2.3.0/yambs/data/includes/infineon.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/data/includes/microchip.yaml` & `yambs-2.3.0/yambs/data/includes/microchip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/data/native.yaml` & `yambs-2.3.0/yambs/data/native.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/data/schemas/Chip.yaml` & `yambs-2.3.0/yambs/data/schemas/Chip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/data/schemas/Config.yaml` & `yambs-2.3.0/yambs/data/schemas/Config.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/data/schemas/Native.yaml` & `yambs-2.3.0/yambs/data/schemas/Native.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/data/schemas/config_common.yaml` & `yambs-2.3.0/yambs/data/schemas/config_common.yaml`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/data/templates/native_rules.ninja.j2` & `yambs-2.3.0/yambs/data/templates/native_rules.ninja.j2`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/data/templates/rules.ninja.j2` & `yambs-2.3.0/yambs/data/templates/rules.ninja.j2`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/data/uf2families.json` & `yambs-2.3.0/yambs/data/uf2families.json`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/dependency/config.py` & `yambs-2.3.0/yambs/dependency/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 A module for working with dependency configurations.
 """
 
 # built-in
 from enum import StrEnum, auto
+from pathlib import Path
 from typing import Any, Dict, Optional, cast
 
 # third-party
 from vcorelib.dict.codec import BasicDictCodec as _BasicDictCodec
 from vcorelib.io import JsonObject as _JsonObject
 
 # internal
@@ -20,36 +21,49 @@
     YAMBS = auto()
 
 
 class DependencySource(StrEnum):
     """All dependency source options."""
 
     GITHUB = auto()
+    DIRECTORY = auto()
 
 
 DependencyData = Dict[str, Any]
 
 
 class Dependency(_YambsDictCodec, _BasicDictCodec):
     """A class for describing project dependencies."""
 
     def __str__(self) -> str:
         """Get this dependency as a string."""
 
-        # Change this when other sources are supported.
-        assert self.source == DependencySource.GITHUB
-        return f"{self.github['owner']}-{self.github['repo']}"
+        if self.source == DependencySource.GITHUB:
+            return f"{self.github['owner']}-{self.github['repo']}"
+
+        assert self.directory is not None
+        return str(self.directory)
 
     def __hash__(self) -> int:
         """Compute a hash for this dependency."""
         return hash(str(self))
 
     def init(self, data: _JsonObject) -> None:
         """Initialize this instance."""
 
         self.kind = DependencyKind(cast(str, data["kind"]))
         self.source = DependencySource(cast(str, data["source"]))
+
+        self.directory: Optional[Path] = None
+        if "directory" in data:
+            self.directory = Path(data["directory"])  # type: ignore
+
+            # Don't require setting this source field explicitly in some
+            # scenarios.
+            if self.source == DependencySource.GITHUB and "github" not in data:
+                self.source = DependencySource.DIRECTORY
+
         self.github: Dict[str, Optional[str]] = data.get(
             "github",
             {},  # type: ignore
         )
         self.target: str = data["target"]  # type: ignore
```

### Comparing `yambs-2.2.2/yambs/dependency/github.py` & `yambs-2.3.0/yambs/dependency/github.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/dependency/handlers/types.py` & `yambs-2.3.0/yambs/dependency/handlers/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 
 class DependencyTask(NamedTuple):
     """A container for dependency handler invocation data."""
 
     # Useful paths.
     root: Path
+    project_root: Path
     include: Path
     static: Path
 
     build_commands: List[List[str]]
 
     compile_flags: List[str]
     link_flags: List[str]
```

### Comparing `yambs-2.2.2/yambs/dependency/manager.py` & `yambs-2.3.0/yambs/dependency/manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,18 +41,19 @@
 
     set_exec_flags(path)
 
 
 class DependencyManager:
     """A class for managing project dependencies."""
 
-    def __init__(self, root: Path) -> None:
+    def __init__(self, root: Path, project_root: Path) -> None:
         """Initialize this instance."""
 
         self.root = root
+        self.project_root = project_root
         self.state_path = self.root.joinpath("state.json")
         self.state = ARBITER.decode(self.state_path).data
 
         # A place for third-party include roots to be linked.
         self.include = self.root.joinpath("include")
         self.include.mkdir(parents=True, exist_ok=True)
 
@@ -99,14 +100,15 @@
         dep_data: DependencyData = self.state.setdefault(
             str(dep),
             {},
         )  # type: ignore
 
         return DependencyTask(
             self.root,
+            self.project_root,
             self.include,
             self.static,
             self.build_commands,
             self.compile_flags,
             self.link_flags,
             dep,
             DependencyState(dep_data.setdefault("state", "init")),
```

### Comparing `yambs-2.2.2/yambs/dist/__init__.py` & `yambs-2.3.0/yambs/dist/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/entry.py` & `yambs-2.3.0/yambs/entry.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/environment/__init__.py` & `yambs-2.3.0/yambs/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/environment/native.py` & `yambs-2.3.0/yambs/environment/native.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         """Initialize this instance."""
 
         super().__init__()
 
         self.config = config
 
         self.dependency_manager = DependencyManager(
-            self.config.third_party_root
+            self.config.third_party_root, self.config.root
         )
 
         # Collect sources.
         self.sources = collect_files(config.src_root)
         self.apps: Set[Path] = set()
         self.regular: Set[Path] = set()
         populate_sources(
```

### Comparing `yambs-2.2.2/yambs/generate/__init__.py` & `yambs-2.3.0/yambs/generate/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/generate/architectures.py` & `yambs-2.3.0/yambs/generate/architectures.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/generate/boards.py` & `yambs-2.3.0/yambs/generate/boards.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/generate/chips.py` & `yambs-2.3.0/yambs/generate/chips.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/generate/common.py` & `yambs-2.3.0/yambs/generate/common.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/generate/ninja/__init__.py` & `yambs-2.3.0/yambs/generate/ninja/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/generate/ninja/format.py` & `yambs-2.3.0/yambs/generate/ninja/format.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/generate/toolchains.py` & `yambs-2.3.0/yambs/generate/toolchains.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/generate/variants.py` & `yambs-2.3.0/yambs/generate/variants.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/github/__init__.py` & `yambs-2.3.0/yambs/github/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/schemas.py` & `yambs-2.3.0/yambs/schemas.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/translation/__init__.py` & `yambs-2.3.0/yambs/translation/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs/uf2/__init__.py` & `yambs-2.3.0/yambs/uf2/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-2.2.2/yambs.egg-info/PKG-INFO` & `yambs-2.3.0/yambs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 2.2.2
+Version: 2.3.0
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
@@ -18,19 +18,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=c6f67ebd8082d4ff4435729188bd6f43
+    hash=da0d2fd90a670c981a7628b6eb8a2c87
     =====================================
 -->
 
-# yambs ([2.2.2](https://pypi.org/project/yambs/))
+# yambs ([2.3.0](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-2.2.2/yambs.egg-info/SOURCES.txt` & `yambs-2.3.0/yambs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,17 @@
 yambs/dependency/__init__.py
 yambs/dependency/config.py
 yambs/dependency/github.py
 yambs/dependency/manager.py
 yambs/dependency/state.py
 yambs/dependency/handlers/__init__.py
 yambs/dependency/handlers/types.py
-yambs/dependency/handlers/yambs.py
+yambs/dependency/handlers/yambs/__init__.py
+yambs/dependency/handlers/yambs/config.py
+yambs/dependency/handlers/yambs/github.py
 yambs/dist/__init__.py
 yambs/environment/__init__.py
 yambs/environment/native.py
 yambs/generate/__init__.py
 yambs/generate/architectures.py
 yambs/generate/boards.py
 yambs/generate/chips.py
```

