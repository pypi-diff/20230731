# Comparing `tmp/power-grid-model-1.5.0rc9232816587778.tar.gz` & `tmp/power-grid-model-1.5.0rc9232904017091.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "power-grid-model-1.5.0rc9232816587778.tar", last modified: Thu Jul 27 14:27:55 2023, max compression
+gzip compressed data, was "power-grid-model-1.5.0rc9232904017091.tar", last modified: Thu Jul 27 18:24:38 2023, max compression
```

## Comparing `power-grid-model-1.5.0rc9232816587778.tar` & `power-grid-model-1.5.0rc9232904017091.tar`

### file list

```diff
@@ -1,593 +1,593 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.655530 power-grid-model-1.5.0rc9232816587778/
--rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-27 14:27:55.655530 power-grid-model-1.5.0rc9232816587778/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 14:27:08.000000 power-grid-model-1.5.0rc9232816587778/PYPI_VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.595528 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.595528 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.587528 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.595528 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.595528 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.595528 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/
--rw-r--r--   0 runner    (1001) docker     (123)    30276 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/input.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    17268 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/output.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/update.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12219 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.599528 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20689 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10636 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    15156 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.599528 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/input.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    23037 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/output.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/state.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/update.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    61980 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.599528 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    41768 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7132 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    25179 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16203 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20649 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    30907 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.599528 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.599528 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.599528 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/basics.h
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/buffer.h
--rw-r--r--   0 runner    (1001) docker     (123)    55882 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/dataset_definitions.h
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/handle.h
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/meta_data.h
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/model.h
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/options.h
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.603528 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/src/buffer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    93852 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/src/dataset_definitions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/src/handle.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/src/handle.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/src/meta_data.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/src/model.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/src/options.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/src/options.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 14:27:55.655530 power-grid-model-1.5.0rc9232816587778/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.587528 power-grid-model-1.5.0rc9232816587778/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.603528 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.603528 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/core/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/core/data_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/core/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/core/index_integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/core/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/core/power_grid_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/core/power_grid_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    22015 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/core/power_grid_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    21661 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.607529 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/validation/assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/validation/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    35027 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/validation/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/validation/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    29999 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model/validation/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.603528 power-grid-model-1.5.0rc9232816587778/src/power_grid_model.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-27 14:27:55.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    35498 2023-07-27 14:27:55.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:27:55.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-27 14:27:55.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 14:27:55.000000 power-grid-model-1.5.0rc9232816587778/src/power_grid_model.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.591528 power-grid-model-1.5.0rc9232816587778/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.591528 power-grid-model-1.5.0rc9232816587778/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.591528 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.607529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/1os2msr/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/1os2msr/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/1os2msr/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/1os2msr/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/1os2msr/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/1os2msr/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/1os2msr/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.607529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test/
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.607529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.607529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.611528 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.611528 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-incomplete-input/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.611528 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.615529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.615529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-newton/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-newton/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-newton/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-newton/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-newton/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-newton/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-newton/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-newton/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-newton/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.615529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-i-n-optional/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-i-n-optional/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-i-n-optional/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-i-n-optional/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-i-n-optional/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.615529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/gaia-example/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/gaia-example/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/gaia-example/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/gaia-example/gaia_grid.gnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/gaia-example/gaia_grid.gnf.license
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/gaia-example/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/gaia-example/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/gaia-example/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/gaia-example/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.615529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/multi-source-with-angle/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/multi-source-with-angle/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/multi-source-with-angle/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/multi-source-with-angle/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/multi-source-with-angle/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/multi-source-with-angle/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/multi-source-with-angle/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.591528 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.591528 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.591528 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.619529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.619529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.619529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/line/
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/line/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/line/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/line/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/line/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/line/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.619529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/node/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/node/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.619529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/shunt/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.623529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/source/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/source/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/source/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/source/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/source/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/source/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.623529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.623529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.623529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.591528 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.627529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/basic-node/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/basic-node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.627529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/line/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/line/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/line/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/line/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/line/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/line/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.627529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/node/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/node/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.627529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/shunt/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/shunt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.627529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/source/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/source/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/source/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/source/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/source/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/source/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.631529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.631529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.631529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.631529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.591528 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.591528 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.635529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.635529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.591528 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.635529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.635529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.639529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/r-state-estimation/
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/r-state-estimation/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/r-state-estimation/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/r-state-estimation/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/r-state-estimation/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/r-state-estimation/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/r-state-estimation/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.639529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/three-winding-transformer/
--rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/three-winding-transformer/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/three-winding-transformer/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/three-winding-transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/three-winding-transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/three-winding-transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/three-winding-transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/three-winding-transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/three-winding-transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/three-winding-transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/three-winding-transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.639529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-example/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-example/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-example/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-example/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-example/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-example/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-example/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-example/vision_grid.vnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-example/vision_grid.vnf.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.639529 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-validation-network/
--rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-validation-network/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-validation-network/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    30756 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-validation-network/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-validation-network/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-validation-network/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-validation-network/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-validation-network/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-validation-network/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    35119 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.591528 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.643529 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/single_phase_to_ground/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/single_phase_to_ground/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/single_phase_to_ground/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/single_phase_to_ground/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/single_phase_to_ground/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)   243263 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/single_phase_to_ground/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/single_phase_to_ground/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/single_phase_to_ground/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/single_phase_to_ground/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.643529 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/three_phase/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/three_phase/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/three_phase/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/three_phase/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/three_phase/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    58928 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/three_phase/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/three_phase/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/three_phase/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/three_phase/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.643529 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)   236282 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.647529 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase_to_ground/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase_to_ground/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase_to_ground/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase_to_ground/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase_to_ground/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)   242819 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase_to_ground/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase_to_ground/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase_to_ground/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase_to_ground/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.591528 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.647529 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/1os2msr/
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/1os2msr/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/1os2msr/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/1os2msr/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/1os2msr/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/1os2msr/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/1os2msr/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.647529 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/1os2msr-no-angle/
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/1os2msr-no-angle/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/1os2msr-no-angle/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/1os2msr-no-angle/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/1os2msr-no-angle/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/1os2msr-no-angle/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/1os2msr-no-angle/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.647529 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    19468 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/distribution-case/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/distribution-case/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.647529 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/dummy-test-sym/
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/dummy-test-sym/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/dummy-test-sym/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/dummy-test-sym/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/dummy-test-sym/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/dummy-test-sym/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/dummy-test-sym/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.651530 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/node-injection-sensor-and-zero-injection/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.651530 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/residual-test/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/residual-test/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/residual-test/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/residual-test/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/residual-test/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/residual-test/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/residual-test/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.651530 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/single-line-load/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/single-line-load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/single-line-load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/single-line-load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/single-line-load/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/single-line-load/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/single-line-load/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.651530 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/three_winding_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/three_winding_transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/three_winding_transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/three_winding_transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/three_winding_transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/three_winding_transformer/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/three_winding_transformer/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.651530 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    29158 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/transmission-case/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/transmission-case/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/transmission-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/transmission-case/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/transmission-case/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.651530 power-grid-model-1.5.0rc9232816587778/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/unit/test_0Z_model_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/unit/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/unit/test_meta_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/unit/test_power_grid_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    20807 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/unit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:27:55.655530 power-grid-model-1.5.0rc9232816587778/tests/unit/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/unit/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/unit/validation/test_assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/unit/validation/test_batch_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/unit/validation/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    29354 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/unit/validation/test_input_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19701 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/unit/validation/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/unit/validation/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24851 2023-07-27 14:27:05.000000 power-grid-model-1.5.0rc9232816587778/tests/unit/validation/test_validation_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.865939 power-grid-model-1.5.0rc9232904017091/
+-rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-27 18:24:38.865939 power-grid-model-1.5.0rc9232904017091/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 18:24:03.000000 power-grid-model-1.5.0rc9232904017091/PYPI_VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.805936 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.805936 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.797935 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.805936 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.805936 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.805936 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)    30276 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/input.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17268 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/output.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/update.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12219 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.809936 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/component/
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20689 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10636 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15156 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.809936 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/input.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23037 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/output.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/state.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/update.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    61980 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.809936 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    41768 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7132 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25179 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16203 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20649 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30907 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.809936 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.809936 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.809936 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/basics.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/buffer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    55882 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/dataset_definitions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/handle.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/meta_data.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/model.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.813936 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/src/buffer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    93852 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/src/dataset_definitions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/src/handle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/src/handle.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/src/meta_data.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/src/model.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/src/options.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/src/options.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 18:24:38.865939 power-grid-model-1.5.0rc9232904017091/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.797935 power-grid-model-1.5.0rc9232904017091/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.813936 power-grid-model-1.5.0rc9232904017091/src/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/src/power_grid_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.813936 power-grid-model-1.5.0rc9232904017091/src/power_grid_model/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/src/power_grid_model/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/src/power_grid_model/core/data_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/src/power_grid_model/core/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/src/power_grid_model/core/index_integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/src/power_grid_model/core/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/src/power_grid_model/core/power_grid_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/src/power_grid_model/core/power_grid_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22015 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/src/power_grid_model/core/power_grid_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/src/power_grid_model/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/src/power_grid_model/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/src/power_grid_model/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21661 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/src/power_grid_model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.813936 power-grid-model-1.5.0rc9232904017091/src/power_grid_model/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/src/power_grid_model/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/src/power_grid_model/validation/assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/src/power_grid_model/validation/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35027 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/src/power_grid_model/validation/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/src/power_grid_model/validation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30357 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/src/power_grid_model/validation/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.813936 power-grid-model-1.5.0rc9232904017091/src/power_grid_model.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-27 18:24:38.000000 power-grid-model-1.5.0rc9232904017091/src/power_grid_model.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35498 2023-07-27 18:24:38.000000 power-grid-model-1.5.0rc9232904017091/src/power_grid_model.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 18:24:38.000000 power-grid-model-1.5.0rc9232904017091/src/power_grid_model.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-27 18:24:38.000000 power-grid-model-1.5.0rc9232904017091/src/power_grid_model.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 18:24:38.000000 power-grid-model-1.5.0rc9232904017091/src/power_grid_model.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.801936 power-grid-model-1.5.0rc9232904017091/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.801936 power-grid-model-1.5.0rc9232904017091/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.801936 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.813936 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/1os2msr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/1os2msr/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/1os2msr/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/1os2msr/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/1os2msr/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/1os2msr/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/1os2msr/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.817937 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.817937 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.817937 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-dependent-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.817937 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.821937 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-incomplete-input/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.821937 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-independent-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.821937 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.821937 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-newton/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-newton/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-newton/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-newton/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-newton/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-newton/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-newton/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-newton/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-newton/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.825937 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-i-n-optional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-i-n-optional/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-i-n-optional/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-i-n-optional/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-i-n-optional/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.825937 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/gaia-example/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/gaia-example/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/gaia-example/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/gaia-example/gaia_grid.gnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/gaia-example/gaia_grid.gnf.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/gaia-example/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/gaia-example/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/gaia-example/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/gaia-example/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.825937 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/multi-source-with-angle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/multi-source-with-angle/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/multi-source-with-angle/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/multi-source-with-angle/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/multi-source-with-angle/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/multi-source-with-angle/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/multi-source-with-angle/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.801936 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.801936 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.801936 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.825937 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.825937 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/asym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.829937 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/line/
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/line/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/line/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/line/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/line/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/line/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.829937 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/node/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.829937 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/shunt/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.829937 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/source/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/source/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/source/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/source/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/source/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.833937 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.833937 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/sym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.833937 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.801936 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.833937 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/basic-node/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/basic-node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.837937 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/line/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/line/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/line/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/line/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/line/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/line/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.837937 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/node/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.837937 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/shunt/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/shunt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.837937 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/source/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/source/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/source/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/source/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/source/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.841938 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/sym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.841938 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/sym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.841938 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.841938 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.801936 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.801936 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/asymmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.845938 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.845938 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.801936 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/symmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.845938 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.845938 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.849938 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/r-state-estimation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/r-state-estimation/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/r-state-estimation/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/r-state-estimation/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/r-state-estimation/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/r-state-estimation/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/r-state-estimation/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.849938 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/three-winding-transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/three-winding-transformer/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/three-winding-transformer/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/three-winding-transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/three-winding-transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/three-winding-transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/three-winding-transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/three-winding-transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/three-winding-transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/three-winding-transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/three-winding-transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.849938 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/vision-example/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/vision-example/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/vision-example/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/vision-example/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/vision-example/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/vision-example/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/vision-example/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/vision-example/vision_grid.vnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/vision-example/vision_grid.vnf.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.849938 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/vision-validation-network/
+-rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/vision-validation-network/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/vision-validation-network/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    30756 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/vision-validation-network/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/vision-validation-network/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/vision-validation-network/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/vision-validation-network/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/vision-validation-network/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/vision-validation-network/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    35119 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.801936 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.853938 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/single_phase_to_ground/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/single_phase_to_ground/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/single_phase_to_ground/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/single_phase_to_ground/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/single_phase_to_ground/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)   243263 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/single_phase_to_ground/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/single_phase_to_ground/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/single_phase_to_ground/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/single_phase_to_ground/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.853938 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/three_phase/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/three_phase/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/three_phase/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/three_phase/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/three_phase/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    58928 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/three_phase/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/three_phase/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/three_phase/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/three_phase/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.853938 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/two_phase/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/two_phase/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/two_phase/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/two_phase/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/two_phase/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)   236282 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/two_phase/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/two_phase/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/two_phase/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/two_phase/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.857938 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/two_phase_to_ground/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/two_phase_to_ground/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/two_phase_to_ground/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/two_phase_to_ground/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/two_phase_to_ground/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)   242819 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/two_phase_to_ground/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/two_phase_to_ground/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/two_phase_to_ground/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/two_phase_to_ground/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.801936 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.857938 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/1os2msr/
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/1os2msr/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/1os2msr/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/1os2msr/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/1os2msr/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/1os2msr/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/1os2msr/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.857938 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/1os2msr-no-angle/
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/1os2msr-no-angle/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/1os2msr-no-angle/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/1os2msr-no-angle/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/1os2msr-no-angle/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/1os2msr-no-angle/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/1os2msr-no-angle/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.857938 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    19468 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/distribution-case/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/distribution-case/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.857938 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/dummy-test-sym/
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/dummy-test-sym/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/dummy-test-sym/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/dummy-test-sym/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/dummy-test-sym/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/dummy-test-sym/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/dummy-test-sym/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.861939 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/node-injection-sensor-and-zero-injection/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.861939 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/residual-test/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/residual-test/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/residual-test/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/residual-test/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/residual-test/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/residual-test/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/residual-test/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.861939 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/single-line-load/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/single-line-load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/single-line-load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/single-line-load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/single-line-load/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/single-line-load/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/single-line-load/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.861939 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/three_winding_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/three_winding_transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/three_winding_transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/three_winding_transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/three_winding_transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/three_winding_transformer/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/three_winding_transformer/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.861939 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    29158 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/transmission-case/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/transmission-case/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/transmission-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/transmission-case/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/transmission-case/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.865939 power-grid-model-1.5.0rc9232904017091/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/unit/test_0Z_model_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/unit/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/unit/test_meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/unit/test_power_grid_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20807 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/unit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:24:38.865939 power-grid-model-1.5.0rc9232904017091/tests/unit/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/unit/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/unit/validation/test_assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/unit/validation/test_batch_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/unit/validation/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29354 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/unit/validation/test_input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19701 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/unit/validation/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/unit/validation/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25462 2023-07-27 18:24:00.000000 power-grid-model-1.5.0rc9232904017091/tests/unit/validation/test_validation_functions.py
```

### Comparing `power-grid-model-1.5.0rc9232816587778/LICENSE` & `power-grid-model-1.5.0rc9232904017091/LICENSE`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/PKG-INFO` & `power-grid-model-1.5.0rc9232904017091/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: power-grid-model
-Version: 1.5.0rc9232816587778
+Version: 1.5.0rc9232904017091
 Summary: Python/C++ library for distribution power system analysis
 Author-email: Alliander Dynamic Grid Calculation <dynamic.grid.calculation@alliander.com>
 License: MPL-2.0
 Project-URL: Home-page, https://lfenergy.org/projects/power-grid-model/
 Project-URL: GitHub, https://github.com/PowerGridModel/power-grid-model
 Project-URL: Documentation, https://power-grid-model.readthedocs.io/en/stable/
 Project-URL: Mailing-list, https://lists.lfenergy.org/g/powergridmodel
```

### Comparing `power-grid-model-1.5.0rc9232816587778/README.md` & `power-grid-model-1.5.0rc9232904017091/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/CMakeLists.txt` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/input.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/input.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/output.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/output.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/update.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/update.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/input.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/input.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/output.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/output.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/state.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/state.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/update.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/update.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/CMakeLists.txt` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/basics.h` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/basics.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/buffer.h` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/buffer.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/dataset_definitions.h` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/dataset_definitions.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/handle.h` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/handle.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/meta_data.h` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/meta_data.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/model.h` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/model.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/options.h` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/options.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/src/buffer.cpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/src/buffer.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/src/dataset_definitions.cpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/src/dataset_definitions.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/src/handle.cpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/src/handle.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/src/handle.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/src/handle.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/src/meta_data.cpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/src/meta_data.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/src/model.cpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/src/model.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/src/options.cpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/src/options.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/power_grid_model_c/power_grid_model_c/src/options.hpp` & `power-grid-model-1.5.0rc9232904017091/power_grid_model_c/power_grid_model_c/src/options.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/pyproject.toml` & `power-grid-model-1.5.0rc9232904017091/pyproject.toml`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/setup.py` & `power-grid-model-1.5.0rc9232904017091/setup.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/src/power_grid_model/__init__.py` & `power-grid-model-1.5.0rc9232904017091/src/power_grid_model/__init__.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/src/power_grid_model/core/data_handling.py` & `power-grid-model-1.5.0rc9232904017091/src/power_grid_model/core/data_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/src/power_grid_model/core/error_handling.py` & `power-grid-model-1.5.0rc9232904017091/src/power_grid_model/core/error_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/src/power_grid_model/core/options.py` & `power-grid-model-1.5.0rc9232904017091/src/power_grid_model/core/options.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/src/power_grid_model/core/power_grid_core.py` & `power-grid-model-1.5.0rc9232904017091/src/power_grid_model/core/power_grid_core.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/src/power_grid_model/core/power_grid_meta.py` & `power-grid-model-1.5.0rc9232904017091/src/power_grid_model/core/power_grid_meta.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/src/power_grid_model/core/power_grid_model.py` & `power-grid-model-1.5.0rc9232904017091/src/power_grid_model/core/power_grid_model.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/src/power_grid_model/data_types.py` & `power-grid-model-1.5.0rc9232904017091/src/power_grid_model/data_types.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/src/power_grid_model/enum.py` & `power-grid-model-1.5.0rc9232904017091/src/power_grid_model/enum.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/src/power_grid_model/utils.py` & `power-grid-model-1.5.0rc9232904017091/src/power_grid_model/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/src/power_grid_model/validation/__init__.py` & `power-grid-model-1.5.0rc9232904017091/src/power_grid_model/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/src/power_grid_model/validation/assertions.py` & `power-grid-model-1.5.0rc9232904017091/src/power_grid_model/validation/assertions.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/src/power_grid_model/validation/errors.py` & `power-grid-model-1.5.0rc9232904017091/src/power_grid_model/validation/errors.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/src/power_grid_model/validation/rules.py` & `power-grid-model-1.5.0rc9232904017091/src/power_grid_model/validation/rules.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/src/power_grid_model/validation/utils.py` & `power-grid-model-1.5.0rc9232904017091/src/power_grid_model/validation/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/src/power_grid_model/validation/validation.py` & `power-grid-model-1.5.0rc9232904017091/src/power_grid_model/validation/validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     # A deep copy is made of the input data, since default values will be added in the validation process
     input_data_copy = copy.deepcopy(input_data)
     assert_valid_data_structure(input_data_copy, "input")
 
     errors: List[ValidationError] = []
     errors += validate_required_values(input_data_copy, calculation_type, symmetric)
     errors += validate_unique_ids_across_components(input_data_copy)
-    errors += validate_values(input_data_copy)
+    errors += validate_values(input_data_copy, calculation_type)
     return errors if errors else None
 
 
 def validate_batch_data(
     input_data: SingleDataset,
     update_data: BatchDataset,
     calculation_type: Optional[CalculationType] = None,
@@ -135,15 +135,15 @@
         assert_valid_data_structure(batch_update_data, "update")
         id_errors: List[ValidationError] = list(validate_ids_exist(batch_update_data, input_data))
 
         batch_errors = input_errors + id_errors
         if not id_errors:
             merged_data = update_input_data(input_data, batch_update_data)
             batch_errors += validate_required_values(merged_data, calculation_type, symmetric)
-            batch_errors += validate_values(merged_data)
+            batch_errors += validate_values(merged_data, calculation_type)
 
         if batch_errors:
             errors[batch] = batch_errors
 
     return errors if errors else None
 
 
@@ -329,26 +329,30 @@
     if not symmetric or asym_sc:
         required["line"] += ["r0", "x0", "c0", "tan0"]
         required["shunt"] += ["g0", "b0"]
 
     return list(chain(*(none_missing(data, component, required.get(component, [])) for component in data)))
 
 
-def validate_values(data: SingleDataset) -> List[ValidationError]:  # pylint: disable=too-many-branches
+def validate_values(  # pylint: disable=too-many-branches
+    data: SingleDataset, calculation_type: Optional[CalculationType] = None
+) -> List[ValidationError]:
     """
     For each component supplied in the data, call the appropriate validation function
 
     Args:
         data: A power-grid-model input dataset
+        calculation_type: Supply a calculation method, to allow missing values for unused fields
 
     Returns:
         An empty list if all required data is valid, or a list of ValidationErrors.
 
     """
     errors: List[ValidationError] = list(all_finite(data))
+
     if "node" in data:
         errors += validate_node(data)
     if "line" in data:
         errors += validate_line(data)
     if "link" in data:
         errors += validate_branch(data, "link")
     if "transformer" in data:
@@ -363,24 +367,28 @@
         errors += validate_generic_load_gen(data, "sym_gen")
     if "asym_load" in data:
         errors += validate_generic_load_gen(data, "asym_load")
     if "asym_gen" in data:
         errors += validate_generic_load_gen(data, "asym_gen")
     if "shunt" in data:
         errors += validate_shunt(data)
-    if "sym_voltage_sensor" in data:
-        errors += validate_generic_voltage_sensor(data, "sym_voltage_sensor")
-    if "asym_voltage_sensor" in data:
-        errors += validate_generic_voltage_sensor(data, "asym_voltage_sensor")
-    if "sym_power_sensor" in data:
-        errors += validate_generic_power_sensor(data, "sym_power_sensor")
-    if "asym_power_sensor" in data:
-        errors += validate_generic_power_sensor(data, "asym_power_sensor")
-    if "fault" in data:
+
+    if calculation_type in (None, CalculationType.state_estimation):
+        if "sym_voltage_sensor" in data:
+            errors += validate_generic_voltage_sensor(data, "sym_voltage_sensor")
+        if "asym_voltage_sensor" in data:
+            errors += validate_generic_voltage_sensor(data, "asym_voltage_sensor")
+        if "sym_power_sensor" in data:
+            errors += validate_generic_power_sensor(data, "sym_power_sensor")
+        if "asym_power_sensor" in data:
+            errors += validate_generic_power_sensor(data, "asym_power_sensor")
+
+    if calculation_type in (None, CalculationType.short_circuit) and "fault" in data:
         errors += validate_fault(data)
+
     return errors
 
 
 # pylint: disable=missing-function-docstring
 
 
 def validate_base(data: SingleDataset, component: str) -> List[ValidationError]:
```

### Comparing `power-grid-model-1.5.0rc9232816587778/src/power_grid_model.egg-info/PKG-INFO` & `power-grid-model-1.5.0rc9232904017091/src/power_grid_model.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: power-grid-model
-Version: 1.5.0rc9232816587778
+Version: 1.5.0rc9232904017091
 Summary: Python/C++ library for distribution power system analysis
 Author-email: Alliander Dynamic Grid Calculation <dynamic.grid.calculation@alliander.com>
 License: MPL-2.0
 Project-URL: Home-page, https://lfenergy.org/projects/power-grid-model/
 Project-URL: GitHub, https://github.com/PowerGridModel/power-grid-model
 Project-URL: Documentation, https://power-grid-model.readthedocs.io/en/stable/
 Project-URL: Mailing-list, https://lists.lfenergy.org/g/powergridmodel
```

### Comparing `power-grid-model-1.5.0rc9232816587778/src/power_grid_model.egg-info/SOURCES.txt` & `power-grid-model-1.5.0rc9232904017091/src/power_grid_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/1os2msr/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/1os2msr/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/1os2msr/sym_output.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/1os2msr/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test/sym_output.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-batch-newton/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-batch-newton/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-i-n-optional/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-i-n-optional/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/gaia-example/asym_output.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/gaia-example/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/gaia-example/gaia_grid.gnf` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/gaia-example/gaia_grid.gnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/gaia-example/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/gaia-example/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/multi-source-with-angle/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/multi-source-with-angle/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/line/README.md` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/line/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/line/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/line/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/node/README.md` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/node/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/node/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/node/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/source/README.md` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/source/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/source/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/source/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/line/README.md` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/line/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/line/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/line/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/node/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/node/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/source/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/source/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/r-state-estimation/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/r-state-estimation/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/r-state-estimation/sym_output.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/r-state-estimation/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/three-winding-transformer/asym_output_batch.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/three-winding-transformer/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/three-winding-transformer/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/three-winding-transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/three-winding-transformer/sym_output_batch.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/three-winding-transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/three-winding-transformer/update_batch.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/three-winding-transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-example/asym_output.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/vision-example/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-example/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/vision-example/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-example/vision_grid.vnf` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/vision-example/vision_grid.vnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-validation-network/asym_output.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/vision-validation-network/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-validation-network/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/vision-validation-network/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-validation-network/sym_output.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/vision-validation-network/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf` & `power-grid-model-1.5.0rc9232904017091/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/single_phase_to_ground/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/single_phase_to_ground/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/single_phase_to_ground/sc_output_batch.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/single_phase_to_ground/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/single_phase_to_ground/update_batch.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/single_phase_to_ground/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/three_phase/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/three_phase/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/three_phase/sc_output_batch.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/three_phase/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/three_phase/update_batch.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/three_phase/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/two_phase/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase/sc_output_batch.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/two_phase/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase/update_batch.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/two_phase/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase_to_ground/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/two_phase_to_ground/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase_to_ground/sc_output_batch.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/two_phase_to_ground/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/short_circuit/two_phase_to_ground/update_batch.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/short_circuit/two_phase_to_ground/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/1os2msr/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/1os2msr/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/1os2msr/sym_output.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/1os2msr/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/1os2msr-no-angle/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/1os2msr-no-angle/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/1os2msr-no-angle/sym_output.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/1os2msr-no-angle/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/distribution-case/README.md` & `power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/distribution-case/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/distribution-case/sym_output_batch.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/distribution-case/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/distribution-case/update_batch.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/dummy-test-sym/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/dummy-test-sym/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/dummy-test-sym/sym_output.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/dummy-test-sym/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/single-line-load/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/single-line-load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/single-line-load/sym_output.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/single-line-load/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/three_winding_transformer/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/three_winding_transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/three_winding_transformer/sym_output.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/three_winding_transformer/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/transmission-case/README.md` & `power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/transmission-case/asym_output.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/transmission-case/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/transmission-case/input.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/data/state_estimation/transmission-case/sym_output.json` & `power-grid-model-1.5.0rc9232904017091/tests/data/state_estimation/transmission-case/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/unit/test_0Z_model_validation.py` & `power-grid-model-1.5.0rc9232904017091/tests/unit/test_0Z_model_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/unit/test_error_handling.py` & `power-grid-model-1.5.0rc9232904017091/tests/unit/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/unit/test_meta_data.py` & `power-grid-model-1.5.0rc9232904017091/tests/unit/test_meta_data.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/unit/test_power_grid_model.py` & `power-grid-model-1.5.0rc9232904017091/tests/unit/test_power_grid_model.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/unit/test_utils.py` & `power-grid-model-1.5.0rc9232904017091/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/unit/utils.py` & `power-grid-model-1.5.0rc9232904017091/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/unit/validation/test_assertions.py` & `power-grid-model-1.5.0rc9232904017091/tests/unit/validation/test_assertions.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/unit/validation/test_batch_validation.py` & `power-grid-model-1.5.0rc9232904017091/tests/unit/validation/test_batch_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/unit/validation/test_errors.py` & `power-grid-model-1.5.0rc9232904017091/tests/unit/validation/test_errors.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/unit/validation/test_input_validation.py` & `power-grid-model-1.5.0rc9232904017091/tests/unit/validation/test_input_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/unit/validation/test_rules.py` & `power-grid-model-1.5.0rc9232904017091/tests/unit/validation/test_rules.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/unit/validation/test_utils.py` & `power-grid-model-1.5.0rc9232904017091/tests/unit/validation/test_utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9232816587778/tests/unit/validation/test_validation_functions.py` & `power-grid-model-1.5.0rc9232904017091/tests/unit/validation/test_validation_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -389,14 +389,29 @@
     # Validate nodes and lines combined
     both_errors = validate_values({"node": node, "line": line})
 
     # The errors should add up (in this simple case)
     assert both_errors == node_errors + line_errors
 
 
+def test_validate_values__calculation_types():
+    # Create invalid sensor
+    sym_voltage_sensor = initialize_array("input", "sym_voltage_sensor", 3)
+    all_errors = validate_values({"sym_voltage_sensor": sym_voltage_sensor})
+    power_flow_errors = validate_values(
+        {"sym_voltage_sensor": sym_voltage_sensor}, calculation_type=CalculationType.power_flow
+    )
+    state_estimation_errors = validate_values(
+        {"sym_voltage_sensor": sym_voltage_sensor}, calculation_type=CalculationType.state_estimation
+    )
+
+    assert not power_flow_errors
+    assert all_errors == state_estimation_errors
+
+
 @pytest.mark.parametrize("measured_terminal_type", MeasuredTerminalType)
 @patch("power_grid_model.validation.validation.validate_base", new=MagicMock())
 @patch("power_grid_model.validation.validation.all_greater_than_zero", new=MagicMock())
 @patch("power_grid_model.validation.validation.all_valid_enum_values", new=MagicMock())
 @patch("power_grid_model.validation.validation.all_valid_ids")
 def test_validate_generic_power_sensor__all_terminal_types(
     all_valid_ids: MagicMock, measured_terminal_type: MeasuredTerminalType
```

