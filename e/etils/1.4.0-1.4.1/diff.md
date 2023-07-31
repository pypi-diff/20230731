# Comparing `tmp/etils-1.4.0.tar.gz` & `tmp/etils-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etils-1.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "etils-1.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `etils-1.4.0.tar` & `etils-1.4.1.tar`

### file list

```diff
@@ -1,85 +1,85 @@
--rw-r--r--   0        0        0    11357 2023-07-25 14:31:41.665450 etils-1.4.0/LICENSE
--rw-r--r--   0        0        0     2167 2023-07-25 14:31:41.665450 etils-1.4.0/README.md
--rw-r--r--   0        0        0      859 2023-07-25 14:31:41.665450 etils-1.4.0/etils/__init__.py
--rw-r--r--   0        0        0     1412 2023-07-25 14:31:41.665450 etils-1.4.0/etils/array_types/__init__.py
--rw-r--r--   0        0        0      720 2023-07-25 14:31:41.665450 etils-1.4.0/etils/eapp/__init__.py
--rw-r--r--   0        0        0     2740 2023-07-25 14:31:41.665450 etils-1.4.0/etils/eapp/dataclass_flags.py
--rw-r--r--   0        0        0     3770 2023-07-25 14:31:41.665450 etils-1.4.0/etils/eapp/logging_utils.py
--rw-r--r--   0        0        0     1318 2023-07-25 14:31:41.665450 etils-1.4.0/etils/ecolab/__init__.py
--rw-r--r--   0        0        0     6379 2023-07-25 14:31:41.665450 etils-1.4.0/etils/ecolab/array_as_img.py
--rw-r--r--   0        0        0     6099 2023-07-25 14:31:41.665450 etils-1.4.0/etils/ecolab/cell_autoreload.py
--rw-r--r--   0        0        0     5442 2023-07-25 14:31:41.665450 etils-1.4.0/etils/ecolab/colab_utils.py
--rw-r--r--   0        0        0     1511 2023-07-25 14:31:41.669450 etils-1.4.0/etils/ecolab/highlight_util.py
--rw-r--r--   0        0        0     8136 2023-07-25 14:31:41.669450 etils-1.4.0/etils/ecolab/inplace_reload.py
--rw-r--r--   0        0        0      583 2023-07-25 14:31:41.669450 etils-1.4.0/etils/ecolab/inspects/__init__.py
--rw-r--r--   0        0        0     1500 2023-07-25 14:31:41.669450 etils-1.4.0/etils/ecolab/inspects/attrs.py
--rw-r--r--   0        0        0     2354 2023-07-25 14:31:41.669450 etils-1.4.0/etils/ecolab/inspects/auto_utils.py
--rw-r--r--   0        0        0     2050 2023-07-25 14:31:41.673450 etils-1.4.0/etils/ecolab/inspects/core.py
--rw-r--r--   0        0        0     2047 2023-07-25 14:31:41.673450 etils-1.4.0/etils/ecolab/inspects/html_helper.py
--rw-r--r--   0        0        0    14441 2023-07-25 14:31:41.673450 etils-1.4.0/etils/ecolab/inspects/nodes.py
--rw-r--r--   0        0        0     1540 2023-07-25 14:31:41.673450 etils-1.4.0/etils/ecolab/inspects/resource_utils.py
--rw-r--r--   0        0        0      191 2023-07-25 14:31:41.673450 etils-1.4.0/etils/ecolab/inspects/static/auto_activate.css
--rw-r--r--   0        0        0     1500 2023-07-25 14:31:41.673450 etils-1.4.0/etils/ecolab/inspects/static/auto_activate.js
--rw-r--r--   0        0        0     2487 2023-07-25 14:31:41.673450 etils-1.4.0/etils/ecolab/inspects/static/main.js
--rw-r--r--   0        0        0     2557 2023-07-25 14:31:41.673450 etils-1.4.0/etils/ecolab/inspects/static/theme.css
--rw-r--r--   0        0        0     1713 2023-07-25 14:31:41.673450 etils-1.4.0/etils/ecolab/ip_utils.py
--rw-r--r--   0        0        0     5529 2023-07-25 14:31:41.673450 etils-1.4.0/etils/ecolab/lazy_imports.py
--rw-r--r--   0        0        0    11303 2023-07-25 14:31:41.673450 etils-1.4.0/etils/ecolab/lazy_utils.py
--rw-r--r--   0        0        0     4436 2023-07-25 14:31:41.673450 etils-1.4.0/etils/ecolab/module_utils.py
--rw-r--r--   0        0        0     2441 2023-07-25 14:31:41.673450 etils-1.4.0/etils/ecolab/patch_utils.py
--rw-r--r--   0        0        0      756 2023-07-25 14:31:41.673450 etils-1.4.0/etils/ecolab/pyjs_com/__init__.py
--rw-r--r--   0        0        0     3031 2023-07-25 14:31:41.673450 etils-1.4.0/etils/ecolab/pyjs_com/py_js_com.js
--rw-r--r--   0        0        0     4460 2023-07-25 14:31:41.673450 etils-1.4.0/etils/ecolab/pyjs_com/py_js_com.py
--rw-r--r--   0        0        0     1074 2023-07-25 14:31:41.673450 etils-1.4.0/etils/ecolab/static/highlight.css
--rw-r--r--   0        0        0     1282 2023-07-25 14:31:41.673450 etils-1.4.0/etils/ecolab/test_utils.py
--rw-r--r--   0        0        0      872 2023-07-25 14:31:41.673450 etils-1.4.0/etils/edc/__init__.py
--rw-r--r--   0        0        0     1678 2023-07-25 14:31:41.673450 etils-1.4.0/etils/edc/cast_utils.py
--rw-r--r--   0        0        0     2621 2023-07-25 14:31:41.673450 etils-1.4.0/etils/edc/context.py
--rw-r--r--   0        0        0     8532 2023-07-25 14:31:41.673450 etils-1.4.0/etils/edc/dataclass_utils.py
--rw-r--r--   0        0        0     5405 2023-07-25 14:31:41.673450 etils-1.4.0/etils/edc/field_utils.py
--rw-r--r--   0        0        0     8161 2023-07-25 14:31:41.673450 etils-1.4.0/etils/edc/frozen_utils.py
--rw-r--r--   0        0        0     5001 2023-07-25 14:31:41.673450 etils-1.4.0/etils/edc/helpers.py
--rw-r--r--   0        0        0     1919 2023-07-25 14:31:41.673450 etils-1.4.0/etils/enp/__init__.py
--rw-r--r--   0        0        0     3752 2023-07-25 14:31:41.673450 etils-1.4.0/etils/enp/array_spec.py
--rw-r--r--   0        0        0      603 2023-07-25 14:31:41.673450 etils-1.4.0/etils/enp/array_types/__init__.py
--rw-r--r--   0        0        0     7867 2023-07-25 14:31:41.673450 etils-1.4.0/etils/enp/array_types/dtypes.py
--rw-r--r--   0        0        0     3725 2023-07-25 14:31:41.673450 etils-1.4.0/etils/enp/array_types/typing.py
--rw-r--r--   0        0        0     9794 2023-07-25 14:31:41.673450 etils-1.4.0/etils/enp/checking.py
--rw-r--r--   0        0        0     4233 2023-07-25 14:31:41.673450 etils-1.4.0/etils/enp/compat.py
--rw-r--r--   0        0        0     2726 2023-07-25 14:31:41.673450 etils-1.4.0/etils/enp/geo_utils.py
--rw-r--r--   0        0        0     4128 2023-07-25 14:31:41.673450 etils-1.4.0/etils/enp/interp_utils.py
--rw-r--r--   0        0        0     1034 2023-07-25 14:31:41.673450 etils-1.4.0/etils/enp/linalg.py
--rw-r--r--   0        0        0    10836 2023-07-25 14:31:41.673450 etils-1.4.0/etils/enp/numpy_utils.py
--rw-r--r--   0        0        0     2804 2023-07-25 14:31:41.673450 etils-1.4.0/etils/enp/testing.py
--rw-r--r--   0        0        0     2086 2023-07-25 14:31:41.673450 etils-1.4.0/etils/enp/type_parsing.py
--rw-r--r--   0        0        0     2063 2023-07-25 14:31:41.673450 etils-1.4.0/etils/enp/typing.py
--rw-r--r--   0        0        0      995 2023-07-25 14:31:41.673450 etils-1.4.0/etils/epath/__init__.py
--rw-r--r--   0        0        0     6237 2023-07-25 14:31:41.673450 etils-1.4.0/etils/epath/abstract_path.py
--rw-r--r--   0        0        0     9479 2023-07-25 14:31:41.673450 etils-1.4.0/etils/epath/backend.py
--rw-r--r--   0        0        0     3159 2023-07-25 14:31:41.673450 etils-1.4.0/etils/epath/flags.py
--rw-r--r--   0        0        0     9026 2023-07-25 14:31:41.673450 etils-1.4.0/etils/epath/gpath.py
--rw-r--r--   0        0        0     3410 2023-07-25 14:31:41.673450 etils-1.4.0/etils/epath/register.py
--rw-r--r--   0        0        0     4937 2023-07-25 14:31:41.673450 etils-1.4.0/etils/epath/resource_utils.py
--rw-r--r--   0        0        0     1078 2023-07-25 14:31:41.673450 etils-1.4.0/etils/epath/stat_utils.py
--rw-r--r--   0        0        0     4927 2023-07-25 14:31:41.673450 etils-1.4.0/etils/epath/testing.py
--rw-r--r--   0        0        0      940 2023-07-25 14:31:41.673450 etils-1.4.0/etils/epath/typing.py
--rw-r--r--   0        0        0     1559 2023-07-25 14:31:41.673450 etils-1.4.0/etils/epy/__init__.py
--rw-r--r--   0        0        0     1622 2023-07-25 14:31:41.673450 etils-1.4.0/etils/epy/_internal.py
--rw-r--r--   0        0        0     1629 2023-07-25 14:31:41.673450 etils-1.4.0/etils/epy/backports.py
--rw-r--r--   0        0        0     2173 2023-07-25 14:31:41.673450 etils-1.4.0/etils/epy/contextlib.py
--rw-r--r--   0        0        0     1097 2023-07-25 14:31:41.673450 etils-1.4.0/etils/epy/env_utils.py
--rw-r--r--   0        0        0     3777 2023-07-25 14:31:41.673450 etils-1.4.0/etils/epy/itertools.py
--rw-r--r--   0        0        0     3361 2023-07-25 14:31:41.677450 etils-1.4.0/etils/epy/lazy_imports_utils.py
--rw-r--r--   0        0        0     4135 2023-07-25 14:31:41.677450 etils-1.4.0/etils/epy/py_utils.py
--rw-r--r--   0        0        0     4859 2023-07-25 14:31:41.677450 etils-1.4.0/etils/epy/reraise_utils.py
--rw-r--r--   0        0        0     2843 2023-07-25 14:31:41.677450 etils-1.4.0/etils/epy/testing.py
--rw-r--r--   0        0        0     6205 2023-07-25 14:31:41.677450 etils-1.4.0/etils/epy/text_utils.py
--rw-r--r--   0        0        0      642 2023-07-25 14:31:41.677450 etils-1.4.0/etils/etqdm/__init__.py
--rw-r--r--   0        0        0     1454 2023-07-25 14:31:41.677450 etils-1.4.0/etils/etqdm/tqdm_utils.py
--rw-r--r--   0        0        0     1195 2023-07-25 14:31:41.677450 etils-1.4.0/etils/etree/__init__.py
--rw-r--r--   0        0        0     8009 2023-07-25 14:31:41.677450 etils-1.4.0/etils/etree/backend.py
--rw-r--r--   0        0        0     4998 2023-07-25 14:31:41.677450 etils-1.4.0/etils/etree/tree_utils.py
--rw-r--r--   0        0        0      906 2023-07-25 14:31:41.677450 etils-1.4.0/etils/etree/typing.py
--rw-r--r--   0        0        0      965 2023-07-25 14:31:41.677450 etils-1.4.0/etils/lazy_imports/__init__.py
--rw-r--r--   0        0        0     3099 2023-07-25 14:31:41.677450 etils-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     5869 1970-01-01 00:00:00.000000 etils-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-31 13:39:13.970790 etils-1.4.1/LICENSE
+-rw-r--r--   0        0        0     2167 2023-07-31 13:39:13.970790 etils-1.4.1/README.md
+-rw-r--r--   0        0        0      859 2023-07-31 13:39:13.970790 etils-1.4.1/etils/__init__.py
+-rw-r--r--   0        0        0     1412 2023-07-31 13:39:13.970790 etils-1.4.1/etils/array_types/__init__.py
+-rw-r--r--   0        0        0      720 2023-07-31 13:39:13.970790 etils-1.4.1/etils/eapp/__init__.py
+-rw-r--r--   0        0        0     2740 2023-07-31 13:39:13.970790 etils-1.4.1/etils/eapp/dataclass_flags.py
+-rw-r--r--   0        0        0     3770 2023-07-31 13:39:13.974790 etils-1.4.1/etils/eapp/logging_utils.py
+-rw-r--r--   0        0        0     1318 2023-07-31 13:39:13.974790 etils-1.4.1/etils/ecolab/__init__.py
+-rw-r--r--   0        0        0     6379 2023-07-31 13:39:13.974790 etils-1.4.1/etils/ecolab/array_as_img.py
+-rw-r--r--   0        0        0     6099 2023-07-31 13:39:13.974790 etils-1.4.1/etils/ecolab/cell_autoreload.py
+-rw-r--r--   0        0        0     5442 2023-07-31 13:39:13.974790 etils-1.4.1/etils/ecolab/colab_utils.py
+-rw-r--r--   0        0        0     1511 2023-07-31 13:39:13.982790 etils-1.4.1/etils/ecolab/highlight_util.py
+-rw-r--r--   0        0        0     8136 2023-07-31 13:39:13.982790 etils-1.4.1/etils/ecolab/inplace_reload.py
+-rw-r--r--   0        0        0      583 2023-07-31 13:39:13.982790 etils-1.4.1/etils/ecolab/inspects/__init__.py
+-rw-r--r--   0        0        0     1500 2023-07-31 13:39:13.982790 etils-1.4.1/etils/ecolab/inspects/attrs.py
+-rw-r--r--   0        0        0     2354 2023-07-31 13:39:13.982790 etils-1.4.1/etils/ecolab/inspects/auto_utils.py
+-rw-r--r--   0        0        0     2050 2023-07-31 13:39:13.982790 etils-1.4.1/etils/ecolab/inspects/core.py
+-rw-r--r--   0        0        0     2047 2023-07-31 13:39:13.982790 etils-1.4.1/etils/ecolab/inspects/html_helper.py
+-rw-r--r--   0        0        0    14441 2023-07-31 13:39:13.982790 etils-1.4.1/etils/ecolab/inspects/nodes.py
+-rw-r--r--   0        0        0     1540 2023-07-31 13:39:13.982790 etils-1.4.1/etils/ecolab/inspects/resource_utils.py
+-rw-r--r--   0        0        0      191 2023-07-31 13:39:13.982790 etils-1.4.1/etils/ecolab/inspects/static/auto_activate.css
+-rw-r--r--   0        0        0     1500 2023-07-31 13:39:13.982790 etils-1.4.1/etils/ecolab/inspects/static/auto_activate.js
+-rw-r--r--   0        0        0     2487 2023-07-31 13:39:13.982790 etils-1.4.1/etils/ecolab/inspects/static/main.js
+-rw-r--r--   0        0        0     2557 2023-07-31 13:39:13.982790 etils-1.4.1/etils/ecolab/inspects/static/theme.css
+-rw-r--r--   0        0        0     1713 2023-07-31 13:39:13.982790 etils-1.4.1/etils/ecolab/ip_utils.py
+-rw-r--r--   0        0        0     5598 2023-07-31 13:39:13.982790 etils-1.4.1/etils/ecolab/lazy_imports.py
+-rw-r--r--   0        0        0    11303 2023-07-31 13:39:13.982790 etils-1.4.1/etils/ecolab/lazy_utils.py
+-rw-r--r--   0        0        0     4436 2023-07-31 13:39:13.982790 etils-1.4.1/etils/ecolab/module_utils.py
+-rw-r--r--   0        0        0     2441 2023-07-31 13:39:13.982790 etils-1.4.1/etils/ecolab/patch_utils.py
+-rw-r--r--   0        0        0      756 2023-07-31 13:39:13.982790 etils-1.4.1/etils/ecolab/pyjs_com/__init__.py
+-rw-r--r--   0        0        0     3031 2023-07-31 13:39:13.982790 etils-1.4.1/etils/ecolab/pyjs_com/py_js_com.js
+-rw-r--r--   0        0        0     4460 2023-07-31 13:39:13.982790 etils-1.4.1/etils/ecolab/pyjs_com/py_js_com.py
+-rw-r--r--   0        0        0     1074 2023-07-31 13:39:13.982790 etils-1.4.1/etils/ecolab/static/highlight.css
+-rw-r--r--   0        0        0     1282 2023-07-31 13:39:13.982790 etils-1.4.1/etils/ecolab/test_utils.py
+-rw-r--r--   0        0        0      872 2023-07-31 13:39:13.982790 etils-1.4.1/etils/edc/__init__.py
+-rw-r--r--   0        0        0     1678 2023-07-31 13:39:13.982790 etils-1.4.1/etils/edc/cast_utils.py
+-rw-r--r--   0        0        0     2621 2023-07-31 13:39:13.982790 etils-1.4.1/etils/edc/context.py
+-rw-r--r--   0        0        0     8532 2023-07-31 13:39:13.982790 etils-1.4.1/etils/edc/dataclass_utils.py
+-rw-r--r--   0        0        0     5405 2023-07-31 13:39:13.982790 etils-1.4.1/etils/edc/field_utils.py
+-rw-r--r--   0        0        0     8161 2023-07-31 13:39:13.986790 etils-1.4.1/etils/edc/frozen_utils.py
+-rw-r--r--   0        0        0     5001 2023-07-31 13:39:13.986790 etils-1.4.1/etils/edc/helpers.py
+-rw-r--r--   0        0        0     1919 2023-07-31 13:39:13.986790 etils-1.4.1/etils/enp/__init__.py
+-rw-r--r--   0        0        0     3752 2023-07-31 13:39:13.986790 etils-1.4.1/etils/enp/array_spec.py
+-rw-r--r--   0        0        0      603 2023-07-31 13:39:13.986790 etils-1.4.1/etils/enp/array_types/__init__.py
+-rw-r--r--   0        0        0     7867 2023-07-31 13:39:13.986790 etils-1.4.1/etils/enp/array_types/dtypes.py
+-rw-r--r--   0        0        0     3725 2023-07-31 13:39:13.986790 etils-1.4.1/etils/enp/array_types/typing.py
+-rw-r--r--   0        0        0     9794 2023-07-31 13:39:13.986790 etils-1.4.1/etils/enp/checking.py
+-rw-r--r--   0        0        0     4233 2023-07-31 13:39:13.986790 etils-1.4.1/etils/enp/compat.py
+-rw-r--r--   0        0        0     2726 2023-07-31 13:39:13.986790 etils-1.4.1/etils/enp/geo_utils.py
+-rw-r--r--   0        0        0     4128 2023-07-31 13:39:13.986790 etils-1.4.1/etils/enp/interp_utils.py
+-rw-r--r--   0        0        0     1034 2023-07-31 13:39:13.986790 etils-1.4.1/etils/enp/linalg.py
+-rw-r--r--   0        0        0    10836 2023-07-31 13:39:13.986790 etils-1.4.1/etils/enp/numpy_utils.py
+-rw-r--r--   0        0        0     2804 2023-07-31 13:39:13.986790 etils-1.4.1/etils/enp/testing.py
+-rw-r--r--   0        0        0     2086 2023-07-31 13:39:13.986790 etils-1.4.1/etils/enp/type_parsing.py
+-rw-r--r--   0        0        0     2063 2023-07-31 13:39:13.986790 etils-1.4.1/etils/enp/typing.py
+-rw-r--r--   0        0        0      995 2023-07-31 13:39:13.986790 etils-1.4.1/etils/epath/__init__.py
+-rw-r--r--   0        0        0     6232 2023-07-31 13:39:13.986790 etils-1.4.1/etils/epath/abstract_path.py
+-rw-r--r--   0        0        0     9479 2023-07-31 13:39:13.986790 etils-1.4.1/etils/epath/backend.py
+-rw-r--r--   0        0        0     3159 2023-07-31 13:39:13.986790 etils-1.4.1/etils/epath/flags.py
+-rw-r--r--   0        0        0     9188 2023-07-31 13:39:13.986790 etils-1.4.1/etils/epath/gpath.py
+-rw-r--r--   0        0        0     3550 2023-07-31 13:39:13.986790 etils-1.4.1/etils/epath/register.py
+-rw-r--r--   0        0        0     4937 2023-07-31 13:39:13.986790 etils-1.4.1/etils/epath/resource_utils.py
+-rw-r--r--   0        0        0     1078 2023-07-31 13:39:13.986790 etils-1.4.1/etils/epath/stat_utils.py
+-rw-r--r--   0        0        0     4927 2023-07-31 13:39:13.986790 etils-1.4.1/etils/epath/testing.py
+-rw-r--r--   0        0        0      940 2023-07-31 13:39:13.986790 etils-1.4.1/etils/epath/typing.py
+-rw-r--r--   0        0        0     1559 2023-07-31 13:39:13.986790 etils-1.4.1/etils/epy/__init__.py
+-rw-r--r--   0        0        0     1622 2023-07-31 13:39:13.986790 etils-1.4.1/etils/epy/_internal.py
+-rw-r--r--   0        0        0     1629 2023-07-31 13:39:13.986790 etils-1.4.1/etils/epy/backports.py
+-rw-r--r--   0        0        0     2173 2023-07-31 13:39:13.986790 etils-1.4.1/etils/epy/contextlib.py
+-rw-r--r--   0        0        0     1097 2023-07-31 13:39:13.986790 etils-1.4.1/etils/epy/env_utils.py
+-rw-r--r--   0        0        0     3777 2023-07-31 13:39:13.986790 etils-1.4.1/etils/epy/itertools.py
+-rw-r--r--   0        0        0     3361 2023-07-31 13:39:13.986790 etils-1.4.1/etils/epy/lazy_imports_utils.py
+-rw-r--r--   0        0        0     4135 2023-07-31 13:39:13.986790 etils-1.4.1/etils/epy/py_utils.py
+-rw-r--r--   0        0        0     4859 2023-07-31 13:39:13.986790 etils-1.4.1/etils/epy/reraise_utils.py
+-rw-r--r--   0        0        0     2843 2023-07-31 13:39:13.986790 etils-1.4.1/etils/epy/testing.py
+-rw-r--r--   0        0        0     6205 2023-07-31 13:39:13.986790 etils-1.4.1/etils/epy/text_utils.py
+-rw-r--r--   0        0        0      642 2023-07-31 13:39:13.990790 etils-1.4.1/etils/etqdm/__init__.py
+-rw-r--r--   0        0        0     1454 2023-07-31 13:39:13.990790 etils-1.4.1/etils/etqdm/tqdm_utils.py
+-rw-r--r--   0        0        0     1195 2023-07-31 13:39:13.990790 etils-1.4.1/etils/etree/__init__.py
+-rw-r--r--   0        0        0     8009 2023-07-31 13:39:13.990790 etils-1.4.1/etils/etree/backend.py
+-rw-r--r--   0        0        0     4998 2023-07-31 13:39:13.990790 etils-1.4.1/etils/etree/tree_utils.py
+-rw-r--r--   0        0        0      906 2023-07-31 13:39:13.990790 etils-1.4.1/etils/etree/typing.py
+-rw-r--r--   0        0        0      965 2023-07-31 13:39:13.990790 etils-1.4.1/etils/lazy_imports/__init__.py
+-rw-r--r--   0        0        0     3099 2023-07-31 13:39:13.990790 etils-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     5869 1970-01-01 00:00:00.000000 etils-1.4.1/PKG-INFO
```

### Comparing `etils-1.4.0/LICENSE` & `etils-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/README.md` & `etils-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/__init__.py` & `etils-1.4.1/etils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,11 +12,11 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Etils API."""
 
 # A new PyPI release will be pushed everytime `__version__` is increased
 # When changing this, also update the CHANGELOG.md
-__version__ = '1.4.0'
+__version__ = '1.4.1'
 
 # Do NOT add anything to this file. This is left empty on purpose.
 # Users should import subprojects directly.
```

### Comparing `etils-1.4.0/etils/array_types/__init__.py` & `etils-1.4.1/etils/array_types/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/eapp/__init__.py` & `etils-1.4.1/etils/eapp/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/eapp/dataclass_flags.py` & `etils-1.4.1/etils/eapp/dataclass_flags.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/eapp/logging_utils.py` & `etils-1.4.1/etils/eapp/logging_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/ecolab/__init__.py` & `etils-1.4.1/etils/ecolab/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/ecolab/array_as_img.py` & `etils-1.4.1/etils/ecolab/array_as_img.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/ecolab/cell_autoreload.py` & `etils-1.4.1/etils/ecolab/cell_autoreload.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/ecolab/colab_utils.py` & `etils-1.4.1/etils/ecolab/colab_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/ecolab/highlight_util.py` & `etils-1.4.1/etils/ecolab/highlight_util.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/ecolab/inplace_reload.py` & `etils-1.4.1/etils/ecolab/inplace_reload.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/ecolab/inspects/__init__.py` & `etils-1.4.1/etils/ecolab/inspects/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/ecolab/inspects/attrs.py` & `etils-1.4.1/etils/ecolab/inspects/attrs.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/ecolab/inspects/auto_utils.py` & `etils-1.4.1/etils/ecolab/inspects/auto_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/ecolab/inspects/core.py` & `etils-1.4.1/etils/ecolab/inspects/core.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/ecolab/inspects/html_helper.py` & `etils-1.4.1/etils/ecolab/inspects/html_helper.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/ecolab/inspects/nodes.py` & `etils-1.4.1/etils/ecolab/inspects/nodes.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/ecolab/inspects/resource_utils.py` & `etils-1.4.1/etils/ecolab/inspects/resource_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/ecolab/inspects/static/auto_activate.js` & `etils-1.4.1/etils/ecolab/inspects/static/auto_activate.js`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/ecolab/inspects/static/main.js` & `etils-1.4.1/etils/ecolab/inspects/static/main.js`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/ecolab/inspects/static/theme.css` & `etils-1.4.1/etils/ecolab/inspects/static/theme.css`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/ecolab/ip_utils.py` & `etils-1.4.1/etils/ecolab/ip_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/ecolab/lazy_imports.py` & `etils-1.4.1/etils/ecolab/lazy_imports.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,21 +151,23 @@
   import dataclass_array as dca
   import einops
   import flask
   import flax
   from flax import linen as nn
   import functorch
   import gin
+  import grain.python as grain
   import graphviz
   import imageio
   # Even though `import ipywidgets as widgets` is the common alias, widgets
   # is likely too ambiguous.
   import ipywidgets
   import jax
   from jax import numpy as jnp
+  import jaxtyping
   import lark
   import matplotlib
   import matplotlib as mpl  # Standard alias
   from matplotlib import pyplot as plt
   import mediapy as media
   import ml_collections
   import networkx as nx
@@ -190,14 +192,15 @@
   # tqdm import also trigger additional imports.
   # TODO(epot): Currently pylance might not infer `tqdm.auto` match
   # `import tqdm.auto`
   # Could try to explicitly import inside a `if typing.TYPE_CHECKING:`
   tqdm.auto  # pylint: disable=pointless-statement
   tqdm.notebook  # pylint: disable=pointless-statement
   import tree
+  import typeguard
   import typing_extensions
   import plotly
   from plotly import express as px
   from plotly import graph_objects as go
   import pydantic
   import requests
   import sunds
```

### Comparing `etils-1.4.0/etils/ecolab/lazy_utils.py` & `etils-1.4.1/etils/ecolab/lazy_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/ecolab/module_utils.py` & `etils-1.4.1/etils/ecolab/module_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/ecolab/patch_utils.py` & `etils-1.4.1/etils/ecolab/patch_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/ecolab/pyjs_com/__init__.py` & `etils-1.4.1/etils/ecolab/pyjs_com/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/ecolab/pyjs_com/py_js_com.js` & `etils-1.4.1/etils/ecolab/pyjs_com/py_js_com.js`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/ecolab/pyjs_com/py_js_com.py` & `etils-1.4.1/etils/ecolab/pyjs_com/py_js_com.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/ecolab/static/highlight.css` & `etils-1.4.1/etils/ecolab/static/highlight.css`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/ecolab/test_utils.py` & `etils-1.4.1/etils/ecolab/test_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/edc/__init__.py` & `etils-1.4.1/etils/edc/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/edc/cast_utils.py` & `etils-1.4.1/etils/edc/cast_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/edc/context.py` & `etils-1.4.1/etils/edc/context.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/edc/dataclass_utils.py` & `etils-1.4.1/etils/edc/dataclass_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/edc/field_utils.py` & `etils-1.4.1/etils/edc/field_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/edc/frozen_utils.py` & `etils-1.4.1/etils/edc/frozen_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/edc/helpers.py` & `etils-1.4.1/etils/edc/helpers.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/enp/__init__.py` & `etils-1.4.1/etils/enp/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/enp/array_spec.py` & `etils-1.4.1/etils/enp/array_spec.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/enp/array_types/__init__.py` & `etils-1.4.1/etils/enp/array_types/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/enp/array_types/dtypes.py` & `etils-1.4.1/etils/enp/array_types/dtypes.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/enp/array_types/typing.py` & `etils-1.4.1/etils/enp/array_types/typing.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/enp/checking.py` & `etils-1.4.1/etils/enp/checking.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/enp/compat.py` & `etils-1.4.1/etils/enp/compat.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/enp/geo_utils.py` & `etils-1.4.1/etils/enp/geo_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/enp/interp_utils.py` & `etils-1.4.1/etils/enp/interp_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/enp/linalg.py` & `etils-1.4.1/etils/enp/linalg.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/enp/numpy_utils.py` & `etils-1.4.1/etils/enp/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/enp/testing.py` & `etils-1.4.1/etils/enp/testing.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/enp/type_parsing.py` & `etils-1.4.1/etils/enp/type_parsing.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/enp/typing.py` & `etils-1.4.1/etils/enp/typing.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/epath/__init__.py` & `etils-1.4.1/etils/epath/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/epath/abstract_path.py` & `etils-1.4.1/etils/epath/abstract_path.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,17 @@
 from __future__ import annotations
 
 import os
 import pathlib
 import typing
 from typing import Any, AnyStr, Iterator, Optional, Type, TypeVar
 
+from etils.epath import register
 from etils.epath import stat_utils
-from etils.epath.typing import PathLike
+from etils.epath.typing import PathLike  # pylint: disable=g-importing-member
 
 _T = TypeVar('_T')
 
 
 # Ideally, `Path` should be `abc.ABC`. However this trigger pytype errors
 # when calling `Path()` (can't instantiate abstract base class)
 # Also this allow path childs to only partially implement the Path API (e.g.
@@ -52,15 +53,14 @@
 
     Args:
       *args: Paths to create
 
     Returns:
       path: The registered path
     """
-    from etils.epath import register  # pylint: disable=g-import-not-at-top
 
     if cls == Path:
       if not args:
         return register.make_path('.')
       root, *parts = args
       return register.make_path(root).joinpath(*parts)
     else:
```

### Comparing `etils-1.4.0/etils/epath/backend.py` & `etils-1.4.1/etils/epath/backend.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/epath/flags.py` & `etils-1.4.1/etils/epath/flags.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/epath/gpath.py` & `etils-1.4.1/etils/epath/gpath.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,20 +23,21 @@
 import types
 import typing
 from typing import Any, ClassVar, Iterator, Optional, Type, TypeVar, Union
 
 from etils import epy
 from etils.epath import abstract_path
 from etils.epath import backend as backend_lib
+from etils.epath import register
 from etils.epath import stat_utils
-from etils.epath.typing import PathLike
+from etils.epath.typing import PathLike  # pylint: disable=g-multiple-import,g-importing-member
 
 _P = TypeVar('_P')
 
-URI_PREFIXES = ('gs://', 's3://')
+_URI_PREFIXES = ('gs://', 's3://')
 _URI_SCHEMES = frozenset(('gs', 's3'))
 
 _URI_MAP_ROOT = {
     'gs://': '/gs/',
     's3://': '/s3/',
 }
 
@@ -63,15 +64,15 @@
   # Use explicit `join()` rather than `super().joinpath()` to avoid infinite
   # recursion.
   # Do not use `os.path`, so `PosixGPath('gs://abc')` works on windows.
   _PATH: ClassVar[types.ModuleType]
 
   def __new__(cls: Type[_P], *parts: PathLike) -> _P:
     full_path = '/'.join(os.fspath(p) for p in parts)
-    if full_path.startswith(URI_PREFIXES):
+    if full_path.startswith(_URI_PREFIXES):
       prefix, _ = full_path.split('://', maxsplit=1)
       prefix = f'{prefix}://'
       new_prefix = _URI_MAP_ROOT[prefix]
       return super().__new__(cls, full_path.replace(prefix, new_prefix, 1))
     else:
       return super().__new__(cls, *parts)
 
@@ -275,17 +276,19 @@
   elif p1._backend in _GCS_BACKENDS:
     return p1._backend
   else:
     return p0._backend
   # pylint: enable=protected-access
 
 
+@register.register_path_cls(_URI_PREFIXES)
 class PosixGPath(_GPath):
   """Pathlib like api with gs://, s3:// support."""
 
   _PATH = posixpath
 
 
+@register.register_path_cls
 class WindowsGPath(pathlib.PureWindowsPath, _GPath):
   """Pathlib like api with gs://, s3:// support."""
 
   _PATH = ntpath
```

### Comparing `etils-1.4.0/etils/epath/register.py` & `etils-1.4.1/etils/epath/register.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,35 +14,31 @@
 
 """Register path."""
 
 from __future__ import annotations
 
 import os
 import typing
-from typing import Callable, Dict, Tuple, Type, TypeVar
+from typing import Callable, TypeVar
 
 from etils.epath import abstract_path
 from etils.epath import gpath
-from etils.epath.typing import PathLike  # pylint: disable=g-multiple-import
+from etils.epath.typing import PathLike  # pylint: disable=g-multiple-import,g-importing-member
 
 _T = TypeVar('_T')
 
-_PATHLIKE_CLS: Tuple[Type[abstract_path.Path], ...] = (
-    gpath.PosixGPath,
-    gpath.WindowsGPath,
-)
-_URI_PREFIXES_TO_CLS: Dict[str, Type[abstract_path.Path]] = {
-    # Even on Windows, `gs://`,... are PosixPath
-    uri_prefix: gpath.PosixGPath
-    for uri_prefix in gpath.URI_PREFIXES
-}
+# Classes and uri are registered in `gpath.py`
+_PATHLIKE_CLS: tuple[type[abstract_path.Path], ...] = ()
+_URI_PREFIXES_TO_CLS: dict[str, type[abstract_path.Path]] = {}
 
 
 @typing.overload
-def register_path_cls(path_cls_or_uri_prefix: str) -> Callable[[_T], _T]:
+def register_path_cls(
+    path_cls_or_uri_prefix: str | list[str] | tuple[str, ...]
+) -> Callable[[_T], _T]:
   ...
 
 
 @typing.overload
 def register_path_cls(path_cls_or_uri_prefix: _T) -> _T:
   ...
 
@@ -63,18 +59,22 @@
     path_cls_or_uri_prefix: If a uri prefix is given, then passing calling
       `tfds.core.as_path('prefix://path')` will call the decorated class.
 
   Returns:
     The decorator or decoratorated class
   """
   global _PATHLIKE_CLS
-  if isinstance(path_cls_or_uri_prefix, str):
+  if isinstance(path_cls_or_uri_prefix, (str, list, tuple)):
 
     def register_path_cls_decorator(cls: _T) -> _T:
-      _URI_PREFIXES_TO_CLS[path_cls_or_uri_prefix] = cls
+      if isinstance(path_cls_or_uri_prefix, str):
+        _URI_PREFIXES_TO_CLS[path_cls_or_uri_prefix] = cls
+      elif isinstance(path_cls_or_uri_prefix, (list, tuple)):
+        for uri_prefix in path_cls_or_uri_prefix:
+          _URI_PREFIXES_TO_CLS[uri_prefix] = cls
       return register_path_cls(cls)
 
     return register_path_cls_decorator
   else:
     _PATHLIKE_CLS = _PATHLIKE_CLS + (path_cls_or_uri_prefix,)
     return path_cls_or_uri_prefix
```

### Comparing `etils-1.4.0/etils/epath/resource_utils.py` & `etils-1.4.1/etils/epath/resource_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/epath/stat_utils.py` & `etils-1.4.1/etils/epath/stat_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/epath/testing.py` & `etils-1.4.1/etils/epath/testing.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/epath/typing.py` & `etils-1.4.1/etils/epath/typing.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/epy/__init__.py` & `etils-1.4.1/etils/epy/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/epy/_internal.py` & `etils-1.4.1/etils/epy/_internal.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/epy/backports.py` & `etils-1.4.1/etils/epy/backports.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/epy/contextlib.py` & `etils-1.4.1/etils/epy/contextlib.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/epy/env_utils.py` & `etils-1.4.1/etils/epy/env_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/epy/itertools.py` & `etils-1.4.1/etils/epy/itertools.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/epy/lazy_imports_utils.py` & `etils-1.4.1/etils/epy/lazy_imports_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/epy/py_utils.py` & `etils-1.4.1/etils/epy/py_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/epy/reraise_utils.py` & `etils-1.4.1/etils/epy/reraise_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/epy/testing.py` & `etils-1.4.1/etils/epy/testing.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/epy/text_utils.py` & `etils-1.4.1/etils/epy/text_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/etqdm/__init__.py` & `etils-1.4.1/etils/etqdm/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/etqdm/tqdm_utils.py` & `etils-1.4.1/etils/etqdm/tqdm_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/etree/__init__.py` & `etils-1.4.1/etils/etree/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/etree/backend.py` & `etils-1.4.1/etils/etree/backend.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/etree/tree_utils.py` & `etils-1.4.1/etils/etree/tree_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/etree/typing.py` & `etils-1.4.1/etils/etree/typing.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/etils/lazy_imports/__init__.py` & `etils-1.4.1/etils/lazy_imports/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/pyproject.toml` & `etils-1.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `etils-1.4.0/PKG-INFO` & `etils-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etils
-Version: 1.4.0
+Version: 1.4.1
 Summary: Collection of common python utils
 Keywords: utils,jax,tensorflow,tf,machine learning,deep learning
 Author-email: Conchylicultor <etils@google.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

