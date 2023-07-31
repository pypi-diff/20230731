# Comparing `tmp/foxes-0.4.1.tar.gz` & `tmp/foxes-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foxes-0.4.1.tar", last modified: Fri Jul  7 09:25:33 2023, max compression
+gzip compressed data, was "foxes-0.4.2.tar", last modified: Mon Jul 31 13:05:15 2023, max compression
```

## Comparing `foxes-0.4.1.tar` & `foxes-0.4.2.tar`

### file list

```diff
@@ -1,263 +1,264 @@
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.591802 foxes-0.4.1/
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1071 2023-06-02 08:05:39.000000 foxes-0.4.1/LICENSE
--rw-r--r--   0 jonas     (1000) jonas     (1000)    40774 2023-06-02 08:05:43.000000 foxes-0.4.1/Logo_FOXES.svg
--rw-r--r--   0 jonas     (1000) jonas     (1000)      215 2023-06-02 08:05:43.000000 foxes-0.4.1/MANIFEST.in
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7287 2023-07-07 09:25:33.591802 foxes-0.4.1/PKG-INFO
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6468 2023-07-07 09:20:16.000000 foxes-0.4.1/README.md
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.571802 foxes-0.4.1/foxes/
--rw-r--r--   0 jonas     (1000) jonas     (1000)        6 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/VERSION
--rw-r--r--   0 jonas     (1000) jonas     (1000)      717 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.571802 foxes-0.4.1/foxes/algorithms/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      188 2023-07-04 09:56:46.000000 foxes-0.4.1/foxes/algorithms/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.571802 foxes-0.4.1/foxes/algorithms/downwind/
--rw-r--r--   0 jonas     (1000) jonas     (1000)       53 2023-06-02 08:05:44.000000 foxes-0.4.1/foxes/algorithms/downwind/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    17768 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/algorithms/downwind/downwind.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.571802 foxes-0.4.1/foxes/algorithms/downwind/models/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      242 2023-06-02 08:05:44.000000 foxes-0.4.1/foxes/algorithms/downwind/models/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2292 2023-06-06 06:30:42.000000 foxes-0.4.1/foxes/algorithms/downwind/models/calc_order.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3382 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/algorithms/downwind/models/farm_wakes_calc.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4400 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/algorithms/downwind/models/point_wakes_calc.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1701 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/algorithms/downwind/models/set_amb_farm_results.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1500 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/algorithms/downwind/models/set_amb_point_results.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.571802 foxes-0.4.1/foxes/algorithms/iterative/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      137 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/algorithms/iterative/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4876 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/algorithms/iterative/iterative.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.571802 foxes-0.4.1/foxes/algorithms/iterative/models/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      125 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/algorithms/iterative/models/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6272 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/algorithms/iterative/models/convergence.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3355 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/algorithms/iterative/models/farm_wakes_calc.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2373 2023-07-07 09:22:06.000000 foxes-0.4.1/foxes/constants.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.571802 foxes-0.4.1/foxes/core/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      811 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/core/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    17540 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/core/algorithm.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5843 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/core/data.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     9387 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/core/data_calc_model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    12417 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/core/farm_controller.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7534 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/core/farm_data_model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      265 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/core/farm_model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    13023 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/core/model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5857 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/core/partial_wakes_model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7210 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/core/point_data_model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    12866 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/core/rotor_model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     8109 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/core/states.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3055 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/core/turbine.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1069 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/core/turbine_model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1410 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/core/turbine_type.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1633 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/core/vertical_profile.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6465 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/core/wake_frame.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3171 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/core/wake_model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2760 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/core/wake_superposition.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1709 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/core/wind_farm.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.571802 foxes-0.4.1/foxes/data/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      152 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/data/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.571802 foxes-0.4.1/foxes/data/farms/
--rw-r--r--   0 jonas     (1000) jonas     (1000)        0 2023-06-02 08:05:43.000000 foxes-0.4.1/foxes/data/farms/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1872 2023-06-02 08:05:43.000000 foxes-0.4.1/foxes/data/farms/test_farm_67.csv
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2949 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/data/parse.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.571802 foxes-0.4.1/foxes/data/power_ct_curves/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      410 2023-06-02 08:05:43.000000 foxes-0.4.1/foxes/data/power_ct_curves/DTU-10MW-D178d3-H119.csv
--rw-r--r--   0 jonas     (1000) jonas     (1000)      300 2023-06-02 08:05:43.000000 foxes-0.4.1/foxes/data/power_ct_curves/IEA-15MW-D240-H150.csv
--rw-r--r--   0 jonas     (1000) jonas     (1000)      851 2023-06-02 08:05:43.000000 foxes-0.4.1/foxes/data/power_ct_curves/IWT-7d5MW-D164-H100.csv
--rw-r--r--   0 jonas     (1000) jonas     (1000)      401 2023-06-02 08:05:43.000000 foxes-0.4.1/foxes/data/power_ct_curves/NREL-5MW-D126-H90.csv
--rw-r--r--   0 jonas     (1000) jonas     (1000)        0 2023-06-02 08:05:43.000000 foxes-0.4.1/foxes/data/power_ct_curves/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/data/states/
--rw-r--r--   0 jonas     (1000) jonas     (1000)   427815 2023-06-02 08:05:43.000000 foxes-0.4.1/foxes/data/states/WRF-Timeseries-4464.csv.gz
--rw-r--r--   0 jonas     (1000) jonas     (1000)        0 2023-06-02 08:05:43.000000 foxes-0.4.1/foxes/data/states/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)   126124 2023-06-02 08:05:43.000000 foxes-0.4.1/foxes/data/states/abl_states_6000.csv.gz
--rw-r--r--   0 jonas     (1000) jonas     (1000)      501 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/data/states/timeseries_100.csv.gz
--rw-r--r--   0 jonas     (1000) jonas     (1000)    29085 2023-06-02 08:05:43.000000 foxes-0.4.1/foxes/data/states/timeseries_3000.csv.gz
--rw-r--r--   0 jonas     (1000) jonas     (1000)    78694 2023-06-02 08:05:43.000000 foxes-0.4.1/foxes/data/states/timeseries_8000.csv.gz
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4943 2023-06-02 08:05:43.000000 foxes-0.4.1/foxes/data/states/wind_rose_bremen.csv
--rw-r--r--   0 jonas     (1000) jonas     (1000)    10990 2023-06-02 08:05:43.000000 foxes-0.4.1/foxes/data/states/wind_rotation.nc
--rw-r--r--   0 jonas     (1000) jonas     (1000)      539 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/data/static_data.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/input/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      125 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/input/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/input/farm_layout/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      250 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/input/farm_layout/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3185 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/input/farm_layout/from_csv.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      574 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/input/farm_layout/from_df.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1578 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/input/farm_layout/from_file.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1642 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/input/farm_layout/from_json.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1465 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/input/farm_layout/grid.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1196 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/input/farm_layout/row.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/input/states/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      302 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/input/states/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/input/states/create/
--rw-r--r--   0 jonas     (1000) jonas     (1000)       81 2023-06-02 08:05:43.000000 foxes-0.4.1/foxes/input/states/create/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3262 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/input/states/create/random_abl_states.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    16099 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/input/states/field_data_nc.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    12490 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/input/states/multi_height.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4455 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/input/states/scan_ws.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5842 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/input/states/single.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    10625 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/input/states/states_table.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/input/windio/
--rw-r--r--   0 jonas     (1000) jonas     (1000)       88 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/input/windio/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     8676 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/input/windio/windio.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/models/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      375 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/models/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/models/farm_controllers/
--rw-r--r--   0 jonas     (1000) jonas     (1000)       71 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/models/farm_controllers/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      249 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/farm_controllers/basic.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/models/farm_models/
--rw-r--r--   0 jonas     (1000) jonas     (1000)       65 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/models/farm_models/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3427 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/farm_models/turbine2farm.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    14000 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/model_book.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/models/partial_wakes/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      241 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/models/partial_wakes/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    11367 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/partial_wakes/axiwake.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    11820 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/partial_wakes/distsliced.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2518 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/partial_wakes/grid.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     8717 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/partial_wakes/mapped.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5656 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/partial_wakes/rotor_points.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    10173 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/partial_wakes/top_hat.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/models/point_models/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      130 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/models/point_models/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4540 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/point_models/set_uniform_data.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1399 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/point_models/tke2ti.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2027 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/models/point_models/wake_deltas.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/models/rotor_models/
--rw-r--r--   0 jonas     (1000) jonas     (1000)       82 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/models/rotor_models/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5607 2023-07-07 09:07:29.000000 foxes-0.4.1/foxes/models/rotor_models/centre.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4985 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/rotor_models/grid.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/models/turbine_models/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      457 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/models/turbine_models/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2650 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/turbine_models/calculator.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3136 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/turbine_models/kTI_model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5969 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/turbine_models/lookup_table.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5501 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/turbine_models/power_mask.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4464 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/turbine_models/rotor_centre_calc.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7688 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/turbine_models/sector_management.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3492 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/turbine_models/set_XYHD.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4543 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/turbine_models/set_farm_vars.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5239 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/turbine_models/table_factors.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2139 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/turbine_models/thrust2ct.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1780 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/turbine_models/yaw2yawm.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1751 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/turbine_models/yawm2yaw.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/models/turbine_types/
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1559 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/turbine_types/CpCt_file.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2277 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/turbine_types/CpCt_from_two.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7803 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/turbine_types/PCt_file.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     8954 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/turbine_types/PCt_from_two.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      248 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/models/turbine_types/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1312 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/turbine_types/null_type.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    11215 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/models/turbine_types/wsrho2PCt_from_two.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/models/vertical_profiles/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      314 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/models/vertical_profiles/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1117 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/vertical_profiles/abl_log_neutral_ws.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1196 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/vertical_profiles/abl_log_stable_ws.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1208 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/vertical_profiles/abl_log_unstable_ws.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2530 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/vertical_profiles/abl_log_ws.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1225 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/vertical_profiles/sheared_ws.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1191 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/vertical_profiles/uniform.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/models/wake_frames/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      197 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_frames/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4760 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_frames/farm_order.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3857 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_frames/rotor_wd.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    12397 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_frames/streamlines.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     9995 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_frames/timelines.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     8452 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_frames/yawed_wakes.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/models/wake_models/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      228 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/models/wake_models/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2990 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_models/axisymmetric.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7349 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_models/dist_sliced.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2951 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_models/gaussian.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/models/wake_models/ti/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      124 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/models/wake_models/ti/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     9069 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_models/ti/crespo_hernandez.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6718 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_models/ti/iec_ti.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5603 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_models/top_hat.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/models/wake_models/wind/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      212 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/models/wake_models/wind/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6051 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_models/wind/bastankhah.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5710 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_models/wind/jensen.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    17035 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_models/wind/porte_agel.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    13025 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_models/wind/turbopark.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/models/wake_superpositions/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      236 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/models/wake_superpositions/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7258 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_superpositions/linear.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     8021 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_superpositions/max.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4054 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_superpositions/product.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7814 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_superpositions/quadratic.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5068 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_superpositions/ti_superp.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/opt/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      171 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/opt/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/opt/constraints/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      158 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/opt/constraints/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6156 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/constraints/area_geometry.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7531 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/constraints/min_dist.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/opt/core/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      288 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/opt/core/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2009 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/core/farm_constraint.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2039 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/core/farm_objective.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    10671 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/core/farm_opt_problem.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7774 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/core/farm_vars_problem.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5676 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/core/pop_states.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/opt/objectives/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      152 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/opt/objectives/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     8983 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/objectives/farm_vars.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4149 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/objectives/max_n_turbines.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/opt/problems/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      102 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/problems/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/opt/problems/layout/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      228 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/opt/problems/layout/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5768 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/problems/layout/farm_layout.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/opt/problems/layout/geom_layouts/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      385 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/opt/problems/layout/geom_layouts/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    22624 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/problems/layout/geom_layouts/constraints.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     8164 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/problems/layout/geom_layouts/geom_layout.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7586 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/problems/layout/geom_layouts/geom_layout_gridded.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    10104 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/problems/layout/geom_layouts/geom_reggrid.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    14222 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/problems/layout/geom_layouts/geom_reggrids.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    17858 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/problems/layout/geom_layouts/objectives.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    11804 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/problems/layout/reggrids_layout.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    10629 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/problems/layout/regular_layout.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    19425 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/problems/opt_farm_vars.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/output/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      391 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/output/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    10639 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/output/farm_layout.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    15744 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/output/farm_results_eval.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    46575 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/output/flow_plots_2d.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2204 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/output/output.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2662 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/output/results_writer.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    10065 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/output/rose_plot.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2421 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/output/state_turbine_map.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5514 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/output/turbine_type_curves.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/utils/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      480 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/utils/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.591802 foxes-0.4.1/foxes/utils/abl/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      134 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/utils/abl/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1358 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/utils/abl/neutral.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      446 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/utils/abl/sheared.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1830 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/utils/abl/stable.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1611 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/utils/abl/unstable.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3321 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/utils/cubic_roots.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5302 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/utils/data_book.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      886 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/utils/dict.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.591802 foxes-0.4.1/foxes/utils/geom2d/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      251 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/utils/geom2d/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    19120 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/utils/geom2d/area_geometry.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4530 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/utils/geom2d/circle.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1626 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/utils/geom2d/example_intersection.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1750 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/utils/geom2d/example_union.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6167 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/utils/geom2d/half_plane.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5534 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/utils/geom2d/polygon.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7895 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/utils/geopandas_helpers.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4627 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/utils/pandas_helpers.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      369 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/utils/plotly_helpers.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.591802 foxes-0.4.1/foxes/utils/runners/
--rw-r--r--   0 jonas     (1000) jonas     (1000)       55 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/utils/runners/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6502 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/utils/runners/runners.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      380 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/utils/subclasses.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2810 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/utils/two_circles.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2825 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/utils/wind_dir.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4261 2023-07-07 09:22:17.000000 foxes-0.4.1/foxes/variables.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.571802 foxes-0.4.1/foxes.egg-info/
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7287 2023-07-07 09:25:33.000000 foxes-0.4.1/foxes.egg-info/PKG-INFO
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7763 2023-07-07 09:25:33.000000 foxes-0.4.1/foxes.egg-info/SOURCES.txt
--rw-r--r--   0 jonas     (1000) jonas     (1000)        1 2023-07-07 09:25:33.000000 foxes-0.4.1/foxes.egg-info/dependency_links.txt
--rw-r--r--   0 jonas     (1000) jonas     (1000)      200 2023-07-07 09:25:33.000000 foxes-0.4.1/foxes.egg-info/requires.txt
--rw-r--r--   0 jonas     (1000) jonas     (1000)        6 2023-07-07 09:25:33.000000 foxes-0.4.1/foxes.egg-info/top_level.txt
--rw-r--r--   0 jonas     (1000) jonas     (1000)        1 2023-07-07 09:25:33.000000 foxes-0.4.1/foxes.egg-info/zip-safe
--rw-r--r--   0 jonas     (1000) jonas     (1000)      185 2023-06-02 08:05:39.000000 foxes-0.4.1/pyproject.toml
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1136 2023-07-07 09:25:33.591802 foxes-0.4.1/setup.cfg
--rw-r--r--   0 jonas     (1000) jonas     (1000)       69 2023-06-02 08:05:43.000000 foxes-0.4.1/setup.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.427192 foxes-0.4.2/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1071 2022-11-29 14:27:28.000000 foxes-0.4.2/LICENSE
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    40774 2022-11-29 14:27:28.000000 foxes-0.4.2/Logo_FOXES.svg
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      215 2023-03-07 14:47:39.000000 foxes-0.4.2/MANIFEST.in
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     7287 2023-07-31 13:05:15.427192 foxes-0.4.2/PKG-INFO
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     6468 2023-07-31 08:01:59.000000 foxes-0.4.2/README.md
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.411192 foxes-0.4.2/foxes/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)        6 2023-07-31 13:04:17.000000 foxes-0.4.2/foxes/VERSION
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      717 2023-06-07 07:05:14.000000 foxes-0.4.2/foxes/__init__.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.411192 foxes-0.4.2/foxes/algorithms/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      188 2023-07-31 08:01:59.000000 foxes-0.4.2/foxes/algorithms/__init__.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.411192 foxes-0.4.2/foxes/algorithms/downwind/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)       53 2022-11-29 14:27:28.000000 foxes-0.4.2/foxes/algorithms/downwind/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    18196 2023-07-31 13:04:17.000000 foxes-0.4.2/foxes/algorithms/downwind/downwind.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.411192 foxes-0.4.2/foxes/algorithms/downwind/models/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      242 2022-11-29 14:27:28.000000 foxes-0.4.2/foxes/algorithms/downwind/models/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2328 2023-07-31 13:04:17.000000 foxes-0.4.2/foxes/algorithms/downwind/models/calc_order.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     3519 2023-07-31 13:04:17.000000 foxes-0.4.2/foxes/algorithms/downwind/models/farm_wakes_calc.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     6483 2023-07-31 13:04:17.000000 foxes-0.4.2/foxes/algorithms/downwind/models/point_wakes_calc.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1738 2023-07-31 13:04:17.000000 foxes-0.4.2/foxes/algorithms/downwind/models/set_amb_farm_results.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1610 2023-07-31 13:04:17.000000 foxes-0.4.2/foxes/algorithms/downwind/models/set_amb_point_results.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.411192 foxes-0.4.2/foxes/algorithms/iterative/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      137 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/algorithms/iterative/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5321 2023-07-31 13:04:17.000000 foxes-0.4.2/foxes/algorithms/iterative/iterative.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.411192 foxes-0.4.2/foxes/algorithms/iterative/models/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      125 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/algorithms/iterative/models/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     6445 2023-07-31 13:04:17.000000 foxes-0.4.2/foxes/algorithms/iterative/models/convergence.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     3392 2023-07-31 13:04:17.000000 foxes-0.4.2/foxes/algorithms/iterative/models/farm_wakes_calc.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2373 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/constants.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.415192 foxes-0.4.2/foxes/core/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      811 2023-06-07 07:05:14.000000 foxes-0.4.2/foxes/core/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    17540 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/core/algorithm.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5843 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/core/data.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     9387 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/core/data_calc_model.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    12417 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/core/farm_controller.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     7534 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/core/farm_data_model.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      265 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/core/farm_model.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    13023 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/core/model.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5857 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/core/partial_wakes_model.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     7210 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/core/point_data_model.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    12866 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/core/rotor_model.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     8109 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/core/states.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     3055 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/core/turbine.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1069 2023-06-26 13:27:01.000000 foxes-0.4.2/foxes/core/turbine_model.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1410 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/core/turbine_type.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1633 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/core/vertical_profile.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     6537 2023-07-31 13:04:17.000000 foxes-0.4.2/foxes/core/wake_frame.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     3171 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/core/wake_model.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2760 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/core/wake_superposition.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1709 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/core/wind_farm.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.415192 foxes-0.4.2/foxes/data/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      152 2023-06-07 07:05:14.000000 foxes-0.4.2/foxes/data/__init__.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.415192 foxes-0.4.2/foxes/data/farms/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)        0 2022-11-29 14:27:28.000000 foxes-0.4.2/foxes/data/farms/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1872 2022-11-29 14:27:28.000000 foxes-0.4.2/foxes/data/farms/test_farm_67.csv
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2949 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/data/parse.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.415192 foxes-0.4.2/foxes/data/power_ct_curves/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      410 2022-11-29 14:27:28.000000 foxes-0.4.2/foxes/data/power_ct_curves/DTU-10MW-D178d3-H119.csv
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      300 2022-11-29 14:27:28.000000 foxes-0.4.2/foxes/data/power_ct_curves/IEA-15MW-D240-H150.csv
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      851 2022-11-29 14:27:28.000000 foxes-0.4.2/foxes/data/power_ct_curves/IWT-7d5MW-D164-H100.csv
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      401 2022-11-29 14:27:28.000000 foxes-0.4.2/foxes/data/power_ct_curves/NREL-5MW-D126-H90.csv
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)        0 2022-11-29 14:27:28.000000 foxes-0.4.2/foxes/data/power_ct_curves/__init__.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.415192 foxes-0.4.2/foxes/data/states/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)   427815 2022-11-29 14:27:28.000000 foxes-0.4.2/foxes/data/states/WRF-Timeseries-4464.csv.gz
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)        0 2022-11-29 14:27:28.000000 foxes-0.4.2/foxes/data/states/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)   126124 2022-11-29 14:27:28.000000 foxes-0.4.2/foxes/data/states/abl_states_6000.csv.gz
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      501 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/data/states/timeseries_100.csv.gz
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    29085 2022-11-29 14:27:28.000000 foxes-0.4.2/foxes/data/states/timeseries_3000.csv.gz
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    78694 2022-11-29 14:27:28.000000 foxes-0.4.2/foxes/data/states/timeseries_8000.csv.gz
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     4943 2022-11-29 14:27:28.000000 foxes-0.4.2/foxes/data/states/wind_rose_bremen.csv
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    10990 2022-11-29 14:27:28.000000 foxes-0.4.2/foxes/data/states/wind_rotation.nc
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      539 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/data/static_data.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.415192 foxes-0.4.2/foxes/input/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      125 2023-06-07 07:05:14.000000 foxes-0.4.2/foxes/input/__init__.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.415192 foxes-0.4.2/foxes/input/farm_layout/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      250 2023-06-07 07:05:14.000000 foxes-0.4.2/foxes/input/farm_layout/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     3185 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/input/farm_layout/from_csv.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      574 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/input/farm_layout/from_df.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1578 2023-06-26 13:27:01.000000 foxes-0.4.2/foxes/input/farm_layout/from_file.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1642 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/input/farm_layout/from_json.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1465 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/input/farm_layout/grid.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1196 2023-06-26 13:27:01.000000 foxes-0.4.2/foxes/input/farm_layout/row.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.415192 foxes-0.4.2/foxes/input/states/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      302 2023-06-26 13:27:01.000000 foxes-0.4.2/foxes/input/states/__init__.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.419192 foxes-0.4.2/foxes/input/states/create/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)       81 2022-11-29 14:27:28.000000 foxes-0.4.2/foxes/input/states/create/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     3262 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/input/states/create/random_abl_states.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    16099 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/input/states/field_data_nc.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    12490 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/input/states/multi_height.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     4455 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/input/states/scan_ws.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5842 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/input/states/single.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    10783 2023-07-31 13:04:17.000000 foxes-0.4.2/foxes/input/states/states_table.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.419192 foxes-0.4.2/foxes/input/windio/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)       88 2023-06-07 07:05:14.000000 foxes-0.4.2/foxes/input/windio/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     8676 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/input/windio/windio.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.419192 foxes-0.4.2/foxes/models/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      375 2023-06-07 07:05:14.000000 foxes-0.4.2/foxes/models/__init__.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.419192 foxes-0.4.2/foxes/models/farm_controllers/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)       71 2023-06-07 07:05:14.000000 foxes-0.4.2/foxes/models/farm_controllers/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      249 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/farm_controllers/basic.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.419192 foxes-0.4.2/foxes/models/farm_models/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)       65 2023-06-07 07:05:14.000000 foxes-0.4.2/foxes/models/farm_models/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     3427 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/farm_models/turbine2farm.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    14000 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/model_book.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.419192 foxes-0.4.2/foxes/models/partial_wakes/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      241 2023-06-07 07:05:14.000000 foxes-0.4.2/foxes/models/partial_wakes/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    11367 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/partial_wakes/axiwake.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    11820 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/partial_wakes/distsliced.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2518 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/partial_wakes/grid.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     8717 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/partial_wakes/mapped.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5656 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/partial_wakes/rotor_points.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    10173 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/partial_wakes/top_hat.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.419192 foxes-0.4.2/foxes/models/point_models/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      130 2023-06-07 07:05:14.000000 foxes-0.4.2/foxes/models/point_models/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     4540 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/point_models/set_uniform_data.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1399 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/point_models/tke2ti.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2027 2023-06-26 13:27:01.000000 foxes-0.4.2/foxes/models/point_models/wake_deltas.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.419192 foxes-0.4.2/foxes/models/rotor_models/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)       82 2023-06-07 07:05:14.000000 foxes-0.4.2/foxes/models/rotor_models/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5607 2023-07-31 08:01:59.000000 foxes-0.4.2/foxes/models/rotor_models/centre.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     4985 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/rotor_models/grid.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.419192 foxes-0.4.2/foxes/models/turbine_models/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      457 2023-06-07 07:05:33.000000 foxes-0.4.2/foxes/models/turbine_models/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2650 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/turbine_models/calculator.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     3136 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/turbine_models/kTI_model.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5969 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/turbine_models/lookup_table.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5501 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/turbine_models/power_mask.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     4464 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/turbine_models/rotor_centre_calc.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     7688 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/turbine_models/sector_management.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     3492 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/turbine_models/set_XYHD.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     4543 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/turbine_models/set_farm_vars.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5239 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/turbine_models/table_factors.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2139 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/turbine_models/thrust2ct.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1780 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/turbine_models/yaw2yawm.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1751 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/turbine_models/yawm2yaw.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.419192 foxes-0.4.2/foxes/models/turbine_types/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1559 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/turbine_types/CpCt_file.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2277 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/turbine_types/CpCt_from_two.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     7803 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/turbine_types/PCt_file.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     8954 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/turbine_types/PCt_from_two.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      248 2023-06-26 13:27:01.000000 foxes-0.4.2/foxes/models/turbine_types/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1312 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/turbine_types/null_type.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    11215 2023-06-26 13:27:01.000000 foxes-0.4.2/foxes/models/turbine_types/wsrho2PCt_from_two.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.419192 foxes-0.4.2/foxes/models/vertical_profiles/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      314 2023-06-26 13:27:01.000000 foxes-0.4.2/foxes/models/vertical_profiles/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1117 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/vertical_profiles/abl_log_neutral_ws.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1196 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/vertical_profiles/abl_log_stable_ws.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1208 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/vertical_profiles/abl_log_unstable_ws.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2530 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/vertical_profiles/abl_log_ws.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1225 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/vertical_profiles/sheared_ws.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1191 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/vertical_profiles/uniform.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.423192 foxes-0.4.2/foxes/models/wake_frames/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      197 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/wake_frames/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     4760 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/wake_frames/farm_order.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     3857 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/wake_frames/rotor_wd.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    12397 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/wake_frames/streamlines.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     9995 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/wake_frames/timelines.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     8452 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/wake_frames/yawed_wakes.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.423192 foxes-0.4.2/foxes/models/wake_models/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      228 2023-06-07 07:05:14.000000 foxes-0.4.2/foxes/models/wake_models/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2990 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/wake_models/axisymmetric.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     7349 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/wake_models/dist_sliced.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2951 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/wake_models/gaussian.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.423192 foxes-0.4.2/foxes/models/wake_models/ti/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      124 2023-06-07 07:05:14.000000 foxes-0.4.2/foxes/models/wake_models/ti/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     9069 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/wake_models/ti/crespo_hernandez.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     6718 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/wake_models/ti/iec_ti.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5603 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/wake_models/top_hat.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.423192 foxes-0.4.2/foxes/models/wake_models/wind/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      212 2023-06-07 07:05:14.000000 foxes-0.4.2/foxes/models/wake_models/wind/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     6051 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/wake_models/wind/bastankhah.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5710 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/wake_models/wind/jensen.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    17035 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/wake_models/wind/porte_agel.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    13909 2023-07-31 13:04:17.000000 foxes-0.4.2/foxes/models/wake_models/wind/turbopark.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.423192 foxes-0.4.2/foxes/models/wake_superpositions/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      236 2023-06-07 07:05:14.000000 foxes-0.4.2/foxes/models/wake_superpositions/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     7258 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/wake_superpositions/linear.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     8021 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/wake_superpositions/max.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     4054 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/wake_superpositions/product.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     7814 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/wake_superpositions/quadratic.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5068 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/models/wake_superpositions/ti_superp.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.423192 foxes-0.4.2/foxes/opt/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      171 2023-06-07 07:05:14.000000 foxes-0.4.2/foxes/opt/__init__.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.423192 foxes-0.4.2/foxes/opt/constraints/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      158 2023-06-07 07:05:14.000000 foxes-0.4.2/foxes/opt/constraints/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     6156 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/opt/constraints/area_geometry.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     7531 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/opt/constraints/min_dist.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.423192 foxes-0.4.2/foxes/opt/core/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      288 2023-06-07 07:05:14.000000 foxes-0.4.2/foxes/opt/core/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2009 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/opt/core/farm_constraint.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2039 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/opt/core/farm_objective.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    10671 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/opt/core/farm_opt_problem.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     7774 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/opt/core/farm_vars_problem.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5676 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/opt/core/pop_states.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.423192 foxes-0.4.2/foxes/opt/objectives/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      152 2023-06-07 07:05:14.000000 foxes-0.4.2/foxes/opt/objectives/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     8983 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/opt/objectives/farm_vars.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     4149 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/opt/objectives/max_n_turbines.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.423192 foxes-0.4.2/foxes/opt/problems/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      102 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/opt/problems/__init__.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.423192 foxes-0.4.2/foxes/opt/problems/layout/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      228 2023-06-07 07:05:14.000000 foxes-0.4.2/foxes/opt/problems/layout/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5768 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/opt/problems/layout/farm_layout.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.423192 foxes-0.4.2/foxes/opt/problems/layout/geom_layouts/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      385 2023-06-07 07:05:14.000000 foxes-0.4.2/foxes/opt/problems/layout/geom_layouts/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    22624 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/opt/problems/layout/geom_layouts/constraints.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     8164 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/opt/problems/layout/geom_layouts/geom_layout.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     7586 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/opt/problems/layout/geom_layouts/geom_layout_gridded.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    10104 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/opt/problems/layout/geom_layouts/geom_reggrid.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    14222 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/opt/problems/layout/geom_layouts/geom_reggrids.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    17858 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/opt/problems/layout/geom_layouts/objectives.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    11804 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/opt/problems/layout/reggrids_layout.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    10629 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/opt/problems/layout/regular_layout.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    19425 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/opt/problems/opt_farm_vars.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.427192 foxes-0.4.2/foxes/output/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      423 2023-07-31 13:04:17.000000 foxes-0.4.2/foxes/output/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2665 2023-07-31 13:04:17.000000 foxes-0.4.2/foxes/output/animation.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    10841 2023-07-31 13:04:17.000000 foxes-0.4.2/foxes/output/farm_layout.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    17749 2023-07-31 13:04:17.000000 foxes-0.4.2/foxes/output/farm_results_eval.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    46401 2023-07-31 13:04:17.000000 foxes-0.4.2/foxes/output/flow_plots_2d.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2204 2023-06-26 13:27:01.000000 foxes-0.4.2/foxes/output/output.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2662 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/output/results_writer.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    10065 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/output/rose_plot.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2421 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/output/state_turbine_map.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5514 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/output/turbine_type_curves.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.427192 foxes-0.4.2/foxes/utils/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      480 2023-06-07 07:05:14.000000 foxes-0.4.2/foxes/utils/__init__.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.427192 foxes-0.4.2/foxes/utils/abl/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      134 2023-06-07 07:05:14.000000 foxes-0.4.2/foxes/utils/abl/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1358 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/utils/abl/neutral.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      446 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/utils/abl/sheared.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1830 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/utils/abl/stable.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1611 2023-06-26 13:27:01.000000 foxes-0.4.2/foxes/utils/abl/unstable.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     3321 2023-06-26 13:27:01.000000 foxes-0.4.2/foxes/utils/cubic_roots.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5302 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/utils/data_book.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      886 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/utils/dict.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.427192 foxes-0.4.2/foxes/utils/geom2d/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      251 2023-06-26 13:27:01.000000 foxes-0.4.2/foxes/utils/geom2d/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)    19120 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/utils/geom2d/area_geometry.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     4530 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/utils/geom2d/circle.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1626 2023-06-07 07:05:14.000000 foxes-0.4.2/foxes/utils/geom2d/example_intersection.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1750 2023-06-07 07:05:14.000000 foxes-0.4.2/foxes/utils/geom2d/example_union.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     6167 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/utils/geom2d/half_plane.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     5534 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/utils/geom2d/polygon.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     7895 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/utils/geopandas_helpers.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     4627 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/utils/pandas_helpers.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      369 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/utils/plotly_helpers.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.427192 foxes-0.4.2/foxes/utils/runners/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)       55 2023-06-26 13:27:01.000000 foxes-0.4.2/foxes/utils/runners/__init__.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     6502 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/utils/runners/runners.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      380 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/utils/subclasses.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2810 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/utils/two_circles.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     2825 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/utils/wind_dir.py
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     4261 2023-07-31 11:29:09.000000 foxes-0.4.2/foxes/variables.py
+drwxrwxr-x   0 jonas     (1001) jonas     (1001)        0 2023-07-31 13:05:15.411192 foxes-0.4.2/foxes.egg-info/
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     7287 2023-07-31 13:05:15.000000 foxes-0.4.2/foxes.egg-info/PKG-INFO
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     7789 2023-07-31 13:05:15.000000 foxes-0.4.2/foxes.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)        1 2023-07-31 13:05:15.000000 foxes-0.4.2/foxes.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      195 2023-07-31 13:05:15.000000 foxes-0.4.2/foxes.egg-info/requires.txt
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)        6 2023-07-31 13:05:15.000000 foxes-0.4.2/foxes.egg-info/top_level.txt
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)        1 2023-07-31 13:05:15.000000 foxes-0.4.2/foxes.egg-info/zip-safe
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)      185 2022-11-29 14:27:28.000000 foxes-0.4.2/pyproject.toml
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)     1130 2023-07-31 13:05:15.427192 foxes-0.4.2/setup.cfg
+-rw-rw-r--   0 jonas     (1001) jonas     (1001)       69 2022-11-29 14:27:28.000000 foxes-0.4.2/setup.py
```

### Comparing `foxes-0.4.1/LICENSE` & `foxes-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/Logo_FOXES.svg` & `foxes-0.4.2/Logo_FOXES.svg`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/PKG-INFO` & `foxes-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxes
-Version: 0.4.1
+Version: 0.4.2
 Summary: Farm Optimization and eXtended yield Evaluation Software
 Author: Fraunhofer IWES
 Author-email: jonas.schmidt@iwes.fraunhofer.de
 License: MIT
 Project-URL: Source Code, https://github.com/FraunhoferIWES/foxes
 Project-URL: Bug Tracker, https://github.com/FraunhoferIWES/foxes/issues
 Project-URL: Documentation, https://fraunhoferiwes.github.io/foxes.docs/index.html
```

### Comparing `foxes-0.4.1/README.md` & `foxes-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/__init__.py` & `foxes-0.4.2/foxes/__init__.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/algorithms/downwind/downwind.py` & `foxes-0.4.2/foxes/algorithms/downwind/downwind.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,78 +1,61 @@
 from foxes.core import Algorithm, FarmDataModelList
 from foxes.core import PointDataModel, PointDataModelList
 import foxes.models as fm
 import foxes.variables as FV
 import foxes.constants as FC
-from . import models as dm
+from . import models as mdls
 
 
 class Downwind(Algorithm):
     """
     The downwind algorithm.
 
     The turbines are evaluated once, in the order
     that is calculated by the provided `TurbineOrder`
     object.
 
-    Parameters
-    ----------
-    mbook : foxes.ModelBook
-        The model book
-    farm : foxes.WindFarm
-        The wind farm
-    states : foxes.core.States
-        The ambient states
-    wake_models : list of str
-        The wake models, applied to all turbines.
-        Will be looked up in the model book
-    rotor_model : str
-        The rotor model, for all turbines. Will be
-        looked up in the model book
-    wake_frame : str
-        The wake frame. Will be looked up in the
-        model book
-    partial_wakes_model : str
-        The partial wakes model. Will be
-        looked up in the model book
-    farm_controller : str
-        The farm controller. Will be
-        looked up in the model book
-    chunks : dict
-        The chunks choice for running in parallel with dask,
-        e.g. `{"state": 1000}` for chunks of 1000 states
-    dbook : foxes.DataBook, optional
-        The data book, or None for default
-    keep_models : set of str
-        Keep these models data in memory and do not finalize them
-    verbosity : int
-        The verbosity level, 0 means silent
-
     Attributes
     ----------
-    states : foxes.core.States
+    states: foxes.core.States
         The ambient states
-    wake_models : list of foxes.core.WakeModel
+    wake_models: list of foxes.core.WakeModel
         The wake models, applied to all turbines
-    rotor_model : foxes.core.RotorModel
+    rotor_model: foxes.core.RotorModel
         The rotor model, for all turbines
-    wake_frame : foxes.core.WakeFrame
+    wake_frame: foxes.core.WakeFrame
         The wake frame
-    partial_wakes_model : foxes.core.PartialWakesModel
+    partial_wakes_model: foxes.core.PartialWakesModel
         The partial wakes model
-    farm_controller : foxes.core.FarmController
+    farm_controller: foxes.core.FarmController
         The farm controller
-    n_states : int
+    n_states: int
         The number of states
 
+   :group: algorithms.downwind
+
     """
 
-    FarmWakesCalculation = dm.FarmWakesCalculation
-    PointWakesCalculation = dm.point_wakes_calc.PointWakesCalculation
-    SetAmbPointResults = dm.set_amb_point_results.SetAmbPointResults
+    @classmethod
+    def get_model(cls, name):
+        """
+        Get the algorithm specific model
+        
+        Parameters
+        ----------
+        name: str
+            The model name
+        
+        Returns
+        -------
+        model: foxes.core.model
+            The model
+        
+        """
+        return getattr(mdls, name)
 
     def __init__(
         self,
         mbook,
         farm,
         states,
         wake_models,
@@ -81,14 +64,51 @@
         partial_wakes_model="auto",
         farm_controller="basic_ctrl",
         chunks={FC.STATE: 1000},
         dbook=None,
         keep_models=set(),
         verbosity=1,
     ):
+        """
+        Constructor.
+
+        Parameters
+        ----------
+        mbook: foxes.ModelBook
+            The model book
+        farm: foxes.WindFarm
+            The wind farm
+        states: foxes.core.States
+            The ambient states
+        wake_models: list of str
+            The wake models, applied to all turbines.
+            Will be looked up in the model book
+        rotor_model: str
+            The rotor model, for all turbines. Will be
+            looked up in the model book
+        wake_frame: str
+            The wake frame. Will be looked up in the
+            model book
+        partial_wakes_model: str
+            The partial wakes model. Will be
+            looked up in the model book
+        farm_controller: str
+            The farm controller. Will be
+            looked up in the model book
+        chunks: dict
+            The chunks choice for running in parallel with dask,
+            e.g. `{"state": 1000}` for chunks of 1000 states
+        dbook: foxes.DataBook, optional
+            The data book, or None for default
+        keep_models: set of str
+            Keep these models data in memory and do not finalize them
+        verbosity: int
+            The verbosity level, 0 means silent
+
+        """
         super().__init__(mbook, farm, chunks, verbosity, dbook, keep_models)
 
         self.states = states
         self.n_states = None
         self.states_data = None
 
         self.rotor_model = self.mbook.rotor_models[rotor_model]
@@ -113,21 +133,21 @@
         Helper function for printing model names
         """
 
         deco = "-" * 50
         self.print(f"\n{deco}")
         self.print(f"  Running {self.name}: {func_name}")
         self.print(deco)
-        self.print(f"  n_states  : {self.n_states}")
+        self.print(f"  n_states : {self.n_states}")
         self.print(f"  n_turbines: {self.n_turbines}")
         if n_points is not None:
-            self.print(f"  n_points  : {n_points}")
+            self.print(f"  n_points : {n_points}")
         self.print(deco)
-        self.print(f"  states    : {self.states}")
-        self.print(f"  rotor     : {self.rotor_model}")
+        self.print(f"  states   : {self.states}")
+        self.print(f"  rotor    : {self.rotor_model}")
         self.print(f"  controller: {self.farm_controller}")
         self.print(f"  partialwks: {self.partial_wakes_model}")
         self.print(f"  wake frame: {self.wake_frame}")
         self.print(deco)
         self.print(f"  wakes:")
         for i, w in enumerate(self.wake_models):
             self.print(f"    {i}) {w}")
@@ -203,32 +223,32 @@
         mlist.models.append(self.rotor_model)
         calc_pars.append(calc_parameters.get(mlist.models[-1].name, {}))
         calc_pars[-1].update(
             {"store_rpoints": True, "store_rweights": True, "store_amb_res": True}
         )
 
         # 4) calculate turbine order:
-        mlist.models.append(dm.CalcOrder())
+        mlist.models.append(self.get_model("CalcOrder")())
         mlist.models[-1].name = "calc_order"
         calc_pars.append(calc_parameters.get(mlist.models[-1].name, {}))
 
         # 5) run post-rotor turbine models via farm controller:
         mlist.models.append(self.farm_controller)
         calc_pars.append(calc_parameters.get(mlist.models[-1].name, {}))
         calc_pars[-1]["pre_rotor"] = False
 
         # 6) copy results to ambient, requires self.farm_vars:
         self.farm_vars = mlist.output_farm_vars(self)
-        mlist.models.append(dm.SetAmbFarmResults())
+        mlist.models.append(self.get_model("SetAmbFarmResults")())
         mlist.models[-1].name = "set_amb_results"
         calc_pars.append(calc_parameters.get(mlist.models[-1].name, {}))
 
         # 7) calculate wake effects:
         if not ambient:
-            mlist.models.append(self.FarmWakesCalculation())
+            mlist.models.append(self.get_model("FarmWakesCalculation")())
             mlist.models[-1].name = "calc_wakes"
             calc_pars.append(calc_parameters.get(mlist.models[-1].name, {}))
 
         # initialize models:
         self.update_idata(mlist)
 
         # update variables:
@@ -259,30 +279,30 @@
         chunked_results=False,
     ):
         """
         Calculate farm data.
 
         Parameters
         ----------
-        calc_parameters : dict
+        calc_parameters: dict
             Parameters for model calculation.
             Key: model name str, value: parameter dict
-        persist : bool
+        persist: bool
             Switch for forcing dask to load all model data
             into memory
-        finalize : bool
+        finalize: bool
             Flag for finalization after calculation
-        ambient : bool
+        ambient: bool
             Flag for ambient instead of waked calculation
         chunked_results: bool
             Flag for chunked results
 
         Returns
         -------
-        farm_results : xarray.Dataset
+        farm_results: xarray.Dataset
             The farm results. The calculated variables have
             dimensions (state, turbine)
 
         """
         # initialize algorithm:
         if not self.initialized:
             self.initialize()
@@ -361,22 +381,24 @@
 
         # 1) calculate ambient extra eval point results:
         mlist.models.append(emodels)
         calc_pars.append({"parameters": emodels_cpars})
 
         # 2) transfer ambient results:
         mlist.models.append(
-            dm.SetAmbPointResults(point_vars=vars, vars_to_amb=vars_to_amb)
+            self.get_model("SetAmbPointResults")(
+                point_vars=vars, vars_to_amb=vars_to_amb)
         )
         mlist.models[-1].name = "set_amb_results"
         calc_pars.append(calc_parameters.get(mlist.models[-1].name, {}))
 
         # 3) calc wake effects:
         if not ambient:
-            mlist.models.append(dm.PointWakesCalculation(vars, emodels, emodels_cpars))
+            mlist.models.append(self.get_model("PointWakesCalculation")(
+                vars, emodels, emodels_cpars))
             mlist.models[-1].name = "calc_wakes"
             calc_pars.append(calc_parameters.get(mlist.models[-1].name, {}))
 
         # initialize models:
         self.update_idata(mlist)
 
         return mlist, calc_pars
@@ -396,46 +418,46 @@
         chunked_results=False,
     ):
         """
         Calculate data at a given set of points.
 
         Parameters
         ----------
-        farm_results : xarray.Dataset
+        farm_results: xarray.Dataset
             The farm results. The calculated variables have
             dimensions (state, turbine)
-        points : numpy.ndarray
+        points: numpy.ndarray
             The points of interest, shape: (n_states, n_points, 3)
-        vars : list of str, optional
+        vars: list of str, optional
             The variables that should be kept in the output,
             or `None` for all
-        vars_to_amb : list of str, optional
+        vars_to_amb: list of str, optional
             Variables for which ambient variables should
             be stored. None means all.
-        point_models : str or foxes.core.PointDataModel
+        point_models: str or foxes.core.PointDataModel
             Additional point models to be executed
-        calc_parameters : dict
+        calc_parameters: dict
             Parameters for model calculation.
             Key: model name str, value: parameter dict
-        persist_mdata : bool
+        persist_mdata: bool
             Switch for forcing dask to load all model data
             into memory
-        persist_fdata : bool
+        persist_fdata: bool
             Switch for forcing dask to load all farm data
             into memory
-        finalize : bool
+        finalize: bool
             Flag for finalization after calculation
-        ambient : bool
+        ambient: bool
             Flag for ambient instead of waked calculation
         chunked_results: bool
             Flag for chunked results
 
         Returns
         -------
-        point_results : xarray.Dataset
+        point_results: xarray.Dataset
             The point results. The calculated variables have
             dimensions (state, point)
 
         """
 
         if not self.initialized:
             self.initialize()
@@ -520,15 +542,15 @@
 
     def finalize(self, clear_mem=False):
         """
         Finalizes the algorithm.
 
         Parameters
         ----------
-        clear_mem : bool
+        clear_mem: bool
             Clear idata memory, including keep_models entries
 
         """
         if clear_mem:
             self.keep_models = set()
 
         mdls = [
```

### Comparing `foxes-0.4.1/foxes/algorithms/downwind/models/calc_order.py` & `foxes-0.4.2/foxes/algorithms/downwind/models/calc_order.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,36 +2,39 @@
 from foxes.core import FarmDataModel
 
 
 class CalcOrder(FarmDataModel):
     """
     This model calculates the turbine evaluation
     order, via wake frames.
+    
+    :group: algorithms.downwind.models
+
     """
 
     def initialize(self, algo, verbosity=0):
         """
         Initializes the model.
 
         This includes loading all required data from files. The model
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         idata = super().initialize(algo, verbosity)
         algo.update_idata(algo.wake_frame, idata=idata, verbosity=verbosity)
@@ -40,42 +43,42 @@
 
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         return [FV.ORDER]
 
     def calculate(self, algo, mdata, fdata):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
         return {FV.ORDER: algo.wake_frame.calc_order(algo, mdata, fdata)}
```

### Comparing `foxes-0.4.1/foxes/algorithms/downwind/models/farm_wakes_calc.py` & `foxes-0.4.2/foxes/algorithms/downwind/models/farm_wakes_calc.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,28 +4,37 @@
 import foxes.variables as FV
 from foxes.core import FarmDataModel
 
 
 class FarmWakesCalculation(FarmDataModel):
     """
     This model calculates wakes effects on farm data.
+
+    :group: algorithms.downwind.models
+
     """
 
+    def __init__(self):
+        """
+        Constructor.
+        """
+        super().__init__()
+        
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         ovars = deepcopy(algo.rotor_model.output_farm_vars(algo))
         ovars += algo.farm_controller.output_farm_vars(algo)
         return list(dict.fromkeys(ovars))
 
@@ -37,22 +46,22 @@
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         self.pwakes = algo.partial_wakes_model
         return super().initialize(algo, verbosity)
@@ -62,24 +71,24 @@
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
         torder = fdata[FV.ORDER]
         n_order = torder.shape[1]
         n_states = mdata.n_states
```

### Comparing `foxes-0.4.1/foxes/algorithms/downwind/models/point_wakes_calc.py` & `foxes-0.4.2/foxes/models/point_models/set_uniform_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,146 +1,154 @@
-import foxes.variables as FV
+import pandas as pd
+
+from foxes.core.point_data_model import PointDataModel
+from foxes.utils import PandasFileHelper
 import foxes.constants as FC
-from foxes.core import PointDataModel
+import foxes.variables as FV
 
 
-class PointWakesCalculation(PointDataModel):
+class SetUniformData(PointDataModel):
     """
-    This model calculates wake effects at points of interest.
-
-    Parameters
-    ----------
-    point_vars : list of str, optional
-        The variables of interest
-    emodels : foxes.core.PointDataModelList, optional
-        The extra evaluation models
-    emodels_cpars : list of dict, optional
-        The calculation parameters for extra models
+    Set uniform data (can be state dependent)
 
     Attributes
     ----------
-    point_vars : list of str
-        The variables of interest
-    emodels : foxes.core.PointDataModelList
-        The extra evaluation models
-    emodels_cpars : list of dict
-        The calculation parameters for extra models
+    data_source: str or pandas.DataFrame or dict
+        Either a file name, or a data frame, both assuming
+        state dependent data. Or a dict for state independent
+        uniform data (i.e., scalars)
+    ovars: list of str
+        The variables to be written
+    var2col: dict
+        Mapping from variable names to data column names
+
+    :group: models.point_models
 
     """
 
-    def __init__(self, point_vars=None, emodels=None, emodels_cpars=None):
-        super().__init__()
-        self._pvars = point_vars
-        self.emodels = emodels
-        self.emodels_cpars = emodels_cpars
+    def __init__(
+        self,
+        data_source,
+        output_vars,
+        var2col={},
+        pd_read_pars={},
+    ):
+        """
+        Constructor.
+
+        Parameters
+        ----------
+        data_source: str or pandas.DataFrame or dict
+            Either a file name, or a data frame, both assuming
+            state dependent data. Or a dict for state independent
+            uniform data (i.e., scalars)
+        output_vars: list of str
+            The variables to be written
+        var2col: dict
+            Mapping from variable names to data column names
+        pd_read_pars: dict
+            pandas file reading parameters
+
+        """
+        self.data_source = data_source
+        self.ovars = output_vars
+        self.var2col = var2col
+
+        self._rpars = pd_read_pars
 
     def initialize(self, algo, verbosity=0):
         """
         Initializes the model.
 
         This includes loading all required data from files. The model
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
-        self.pvars = (
-            algo.states.output_point_vars(algo) if self._pvars is None else self._pvars
-        )
+        self.VARS = self.var("VARS")
+        self.DATA = self.var("DATA")
+
+        if isinstance(self.data_source, pd.DataFrame):
+            data = self.data_source[
+                [self.var2col.get(v, v) for v in self.ovars]
+            ].to_numpy(FC.DTYPE)
+        elif isinstance(self.data_source, dict):
+            pass
+        else:
+            if verbosity:
+                print(f"States '{self.name}': Reading file {self.data_source}")
+            rpars = dict(index_col=0)
+            rpars.update(self._rpars)
+            data = PandasFileHelper().read_file(self.data_source, **rpars)
+            data = data[[self.var2col.get(v, v) for v in self.ovars]].to_numpy(FC.DTYPE)
 
         idata = super().initialize(algo, verbosity)
-        if self.emodels is not None:
-            algo.update_idata(self.emodels, idata=idata, verbosity=verbosity)
+        idata["coords"][self.VARS] = self.ovars
+        idata["data_vars"][self.DATA] = ((FC.STATE, self.VARS), data)
 
         return idata
 
     def output_point_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
-        return self.pvars
+        return self.ovars
 
     def calculate(self, algo, mdata, fdata, pdata):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        pdata : foxes.core.Data
+        pdata: foxes.core.Data
             The point data
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_points)
 
         """
-        torder = fdata[FV.ORDER].astype(FC.ITYPE)
-        n_order = torder.shape[1]
-
-        wdeltas = {}
-        wmodels = []
-        for w in algo.wake_models:
-            hdeltas = {}
-            w.init_wake_deltas(algo, mdata, fdata, pdata, hdeltas)
-            if len(set(self.pvars).intersection(hdeltas.keys())):
-                wdeltas.update(hdeltas)
-                wmodels.append(w)
-            del hdeltas
-
-        for oi in range(n_order):
-            o = torder[:, oi]
-            wcoos = algo.wake_frame.get_wake_coos(algo, mdata, fdata, pdata, o)
-
-            for w in wmodels:
-                w.contribute_to_wake_deltas(
-                    algo, mdata, fdata, pdata, o, wcoos, wdeltas
-                )
-
-        amb_res = {v: pdata[FV.var2amb[v]] for v in wdeltas}
-        for w in wmodels:
-            w.finalize_wake_deltas(algo, mdata, fdata, pdata, amb_res, wdeltas)
-
-        for v in self.pvars:
-            if v in wdeltas:
-                pdata[v] = amb_res[v] + wdeltas[v]
-
-        if self.emodels is not None:
-            self.emodels.calculate(algo, mdata, fdata, pdata, self.emodels_cpars)
+        for v in self.ovars:
+            if self.DATA in mdata:
+                pdata[v][:] = mdata[v][None, self.ovars.index(v)]
+            else:
+                pdata[v][:] = self.data_source[v]
 
-        return {v: pdata[v] for v in self.pvars}
+        return {v: pdata[v] for v in self.ovars}
```

### Comparing `foxes-0.4.1/foxes/algorithms/downwind/models/set_amb_farm_results.py` & `foxes-0.4.2/foxes/algorithms/downwind/models/set_amb_farm_results.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 
 class SetAmbFarmResults(FarmDataModel):
     """
     This model copies farm data results to ambient results.
 
     Attributes
     ----------
-    vars : list of str
+    vars: list of str
         The variables to be copied, or `None` for all
+    
+    :group: algorithms.downwind.models
 
     """
 
     def __init__(self):
         """
         Constructor.
         """
@@ -22,20 +24,20 @@
 
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         if self.vars is None:
             self.vars = set([v for v in algo.farm_vars if v in FV.var2amb])
         return [FV.var2amb[v] for v in self.vars]
 
@@ -44,24 +46,24 @@
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
         for v in self.vars:
             fdata[FV.var2amb[v]] = fdata[v].copy()
         return {v: fdata[v] for v in self.output_farm_vars(algo)}
```

### Comparing `foxes-0.4.1/foxes/algorithms/downwind/models/set_amb_point_results.py` & `foxes-0.4.2/foxes/algorithms/downwind/models/set_amb_point_results.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,31 +2,37 @@
 from foxes.core import PointDataModel
 
 
 class SetAmbPointResults(PointDataModel):
     """
     This model copies point results to ambient results.
 
-    Parameters
-    ----------
-    point_vars : list of str, optional
-        The point variables to be treated
-    vars_to_amb : list of str, optional
-        The variables to be copied to output
-
     Attributes
     ----------
-    pvars : list of str
+    pvars: list of str
         The point variables to be treated
-    vars : list of str
+    vars: list of str
         The variables to be copied to output
+    
+    :group: algorithms.downwind.models
 
     """
 
     def __init__(self, point_vars=None, vars_to_amb=None):
+        """
+        Constructor.
+
+        Parameters
+        ----------
+        point_vars: list of str, optional
+            The point variables to be treated
+        vars_to_amb: list of str, optional
+            The variables to be copied to output
+
+        """
         super().__init__()
         self._pvars = point_vars
         self._vars = vars_to_amb
 
     def initialize(self, algo, verbosity=0):
         self.pvars = (
             algo.states.output_point_vars(algo) if self._pvars is None else self._pvars
```

### Comparing `foxes-0.4.1/foxes/algorithms/iterative/iterative.py` & `foxes-0.4.2/foxes/algorithms/iterative/iterative.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,49 @@
 from foxes.algorithms.downwind.downwind import Downwind
 
 from foxes.core import FarmDataModelList
 import foxes.variables as FV
-from . import models as im
+from . import models as mdls
 
 
 class Iterative(Downwind):
     """
     Iterative calculation of farm data.
 
     Attributes
     ----------
     max_it: int
         The maximal number of iterations
     conv_crit: foxes.algorithms.iterative.ConvCrit
         The convergence criteria
 
+    :group: algorithms.iterative
+
     """
 
-    FarmWakesCalculation = im.FarmWakesCalculation
+    @classmethod
+    def get_model(cls, name):
+        """
+        Get the algorithm specific model
+        
+        Parameters
+        ----------
+        name: str
+            The model name
+        
+        Returns
+        -------
+        model: foxes.core.model
+            The model
+        
+        """
+        try:
+            return getattr(mdls, name)
+        except AttributeError:
+            return super().get_model(name)
 
     def __init__(self, *args, max_it=None, conv_crit=None, **kwargs):
         """
         Constructor.
 
         Parameters
         ----------
@@ -37,15 +58,15 @@
 
         """
 
         verbosity = int(kwargs.pop("verbosity", 1)) - 1
         super().__init__(*args, verbosity=verbosity, **kwargs)
 
         self.max_it = 2 * self.farm.n_turbines if max_it is None else max_it
-        self.conv_crit = im.DefaultConv() if conv_crit is None else conv_crit
+        self.conv_crit = self.get_model("DefaultConv")() if conv_crit is None else conv_crit
         self._it = None
         self._mlist = None
 
     @property
     def iterations(self):
         """
         The current iteration number
@@ -92,15 +113,15 @@
 
         # prepare:
         calc_pars = []
         mlist = FarmDataModelList(models=[])
         mlist.name = f"{self.name}_calc"
 
         # add model that calculates wake effects:
-        mlist.models.append(self.FarmWakesCalculation())
+        mlist.models.append(self.get_model("FarmWakesCalculation")())
         mlist.models[-1].name = "calc_wakes"
         calc_pars.append(calc_parameters.get(mlist.models[-1].name, {}))
 
         # initialize models:
         self.update_idata(mlist)
 
         # update variables:
@@ -132,22 +153,22 @@
 
     def calc_farm(self, finalize=True, **kwargs):
         """
         Calculate farm data.
 
         Parameters
         ----------
-        finalize : bool
+        finalize: bool
             Flag for finalization after calculation
         kwargs: dict, optional
             Arguments for calc_farm in the base class.
 
         Returns
         -------
-        farm_results : xarray.Dataset
+        farm_results: xarray.Dataset
             The farm results. The calculated variables have
             dimensions (state, turbine)
 
         """
         fres = None
         self._it = -1
         while self._it < self.max_it:
```

### Comparing `foxes-0.4.1/foxes/algorithms/iterative/models/convergence.py` & `foxes-0.4.2/foxes/algorithms/iterative/models/convergence.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,16 @@
     Abstract base class for convergence criteria
 
     Attributes
     ----------
     name: str, optional
         The convergence criteria name
 
+    :group: algorithms.iterative.models
+
     """
 
     def __init__(self, name=None):
         """
         Constructor.
 
         Parameters
@@ -72,14 +74,16 @@
     """
     A list of convergence criteria
 
     Attributes
     ----------
     crits: list of ConvCrit
         The criteria
+    
+    :group: algorithms.iterative.models
 
     """
 
     def __init__(self, crits=[], name=None):
         """
         Constructor.
 
@@ -159,14 +163,16 @@
     Attributes
     ----------
     limits: dict
         The convergence limits. Keys: variables str,
         values: float values
     wd_vars: list of str
         The wind direction type variables (unit deg)
+    
+    :group: algorithms.iterative.models
 
     """
 
     def __init__(self, limits, wd_vars=None, name=None):
         """
         Constructor.
 
@@ -252,14 +258,17 @@
         """
         return self._deltas
 
 
 class DefaultConv(ConvVarDelta):
     """
     Default convergence criteria.
+
+    :group: algorithms.iterative.models
+
     """
 
     def __init__(self):
         """
         Constructor.
         """
         super().__init__(
```

### Comparing `foxes-0.4.1/foxes/algorithms/iterative/models/farm_wakes_calc.py` & `foxes-0.4.2/foxes/algorithms/iterative/models/farm_wakes_calc.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,28 +5,31 @@
 import foxes.constants as FC
 from foxes.core import FarmDataModel
 
 
 class FarmWakesCalculation(FarmDataModel):
     """
     This model calculates wakes effects on farm data.
+
+    :group: algorithms.iterative.models
+    
     """
 
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
 
         Returns
         -------
-        output_vars : list of str
+        output_vars: list of str
             The output variable names
 
         """
         ovars = deepcopy(algo.rotor_model.output_farm_vars(algo))
         ovars += algo.farm_controller.output_farm_vars(algo)
         return list(dict.fromkeys(ovars))
 
@@ -38,22 +41,22 @@
         should return all array type data as part of the idata return
         dictionary (and not store it under self, for memory reasons). This
         data will then be chunked and provided as part of the mdata object
         during calculations.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity : int
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        idata : dict
+        idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         self.pwakes = algo.partial_wakes_model
         return super().initialize(algo, verbosity)
@@ -63,24 +66,24 @@
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
 
         torder = fdata[FV.ORDER]
         n_order = torder.shape[1]
```

### Comparing `foxes-0.4.1/foxes/constants.py` & `foxes-0.4.2/foxes/constants.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/core/__init__.py` & `foxes-0.4.2/foxes/core/__init__.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/core/algorithm.py` & `foxes-0.4.2/foxes/core/algorithm.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/core/data.py` & `foxes-0.4.2/foxes/core/data.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/core/data_calc_model.py` & `foxes-0.4.2/foxes/core/data_calc_model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/core/farm_controller.py` & `foxes-0.4.2/foxes/core/farm_controller.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/core/farm_data_model.py` & `foxes-0.4.2/foxes/core/farm_data_model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/core/model.py` & `foxes-0.4.2/foxes/core/model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/core/partial_wakes_model.py` & `foxes-0.4.2/foxes/core/partial_wakes_model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/core/point_data_model.py` & `foxes-0.4.2/foxes/core/point_data_model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/core/rotor_model.py` & `foxes-0.4.2/foxes/core/rotor_model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/core/states.py` & `foxes-0.4.2/foxes/core/states.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/core/turbine.py` & `foxes-0.4.2/foxes/core/turbine.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/core/turbine_model.py` & `foxes-0.4.2/foxes/core/turbine_model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/core/turbine_type.py` & `foxes-0.4.2/foxes/core/turbine_type.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/core/vertical_profile.py` & `foxes-0.4.2/foxes/core/vertical_profile.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/core/wake_frame.py` & `foxes-0.4.2/foxes/core/wake_frame.py`

 * *Files 6% similar despite different names*

```diff
@@ -110,14 +110,15 @@
         algo,
         mdata,
         fdata,
         states_source_turbine,
         variables,
         x,
         dx,
+        wake_models=None,
         **ipars,
     ):
         """
         Integrates variables along the centreline.
 
         Parameters
         ----------
@@ -133,14 +134,16 @@
         variables: list of str
             The variables to be integrated
         x: numpy.ndarray
             The wake frame x coordinates of the upper integral bounds,
             shape: (n_states, n_points)
         dx: float
             The step size of the integral
+        wake_models: list of foxes.core.WakeModels
+            The wake models to consider, default: from algo
         ipars: dict, optional
             Additional interpolation parameters
 
         Returns
         -------
         results: numpy.ndarray
             The integration results, shape: (n_states, n_points, n_vars)
@@ -162,41 +165,39 @@
         xpts = np.zeros((n_states, n_steps), dtype=FC.DTYPE)
         xpts[:] = xs[None, 1:]
         pts = self.get_centreline_points(
             algo, mdata, fdata, states_source_turbine, xpts
         )
 
         # run ambient calculation:
-        pdata = {FC.POINTS: pts}
-        pdims = {FC.POINTS: (FC.STATE, FC.POINT, FC.XYH)}
-        pdata.update(
-            {v: np.full((n_states, n_steps), np.nan, dtype=FC.DTYPE) for v in vrs}
+        pdata = Data.from_points(
+            pts,
+            data={v: np.full((n_states, n_steps), np.nan, dtype=FC.DTYPE) for v in vrs},
+            dims={v: (FC.STATE, FC.POINT) for v in vrs}
         )
-        pdims.update({v: (FC.STATE, FC.POINT) for v in vrs})
-        pdata = Data(pdata, pdims, loop_dims=[FC.STATE, FC.POINT])
         res = algo.states.calculate(algo, mdata, fdata, pdata)
         pdata.update(res)
         amb2var = algo.SetAmbPointResults()
         amb2var.initialize(algo, verbosity=0)
         res = amb2var.calculate(algo, mdata, fdata, pdata)
         pdata.update(res)
-        del pdims, res, amb2var
+        del res, amb2var
 
         # find out if all vars ambient:
         ambient = True
         for v in variables:
             if v not in FV.amb2var:
                 ambient = False
                 break
 
         # calc wakes:
         if not ambient:
-            wcalc = algo.PointWakesCalculation(vrs)
+            wcalc = algo.PointWakesCalculation(vrs, wake_models=wake_models)
             wcalc.initialize(algo, verbosity=0)
-            res = wcalc.calculate(algo, mdata, fdata, pdata)
+            res = wcalc.calculate(algo, mdata, fdata, pdata, states_source_turbine=states_source_turbine)
             pdata.update(res)
             del wcalc, res
 
         # collect integration results:
         iresults = np.zeros((n_states, n_ix, n_vars), dtype=FC.DTYPE)
         for vi, v in enumerate(variables):
             for i in range(n_steps):
```

### Comparing `foxes-0.4.1/foxes/core/wake_model.py` & `foxes-0.4.2/foxes/core/wake_model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/core/wake_superposition.py` & `foxes-0.4.2/foxes/core/wake_superposition.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/core/wind_farm.py` & `foxes-0.4.2/foxes/core/wind_farm.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/data/farms/test_farm_67.csv` & `foxes-0.4.2/foxes/data/farms/test_farm_67.csv`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/data/parse.py` & `foxes-0.4.2/foxes/data/parse.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/data/power_ct_curves/IWT-7d5MW-D164-H100.csv` & `foxes-0.4.2/foxes/data/power_ct_curves/IWT-7d5MW-D164-H100.csv`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/data/states/WRF-Timeseries-4464.csv.gz` & `foxes-0.4.2/foxes/data/states/WRF-Timeseries-4464.csv.gz`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/data/states/abl_states_6000.csv.gz` & `foxes-0.4.2/foxes/data/states/abl_states_6000.csv.gz`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/data/states/timeseries_3000.csv.gz` & `foxes-0.4.2/foxes/data/states/timeseries_3000.csv.gz`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/data/states/timeseries_8000.csv.gz` & `foxes-0.4.2/foxes/data/states/timeseries_8000.csv.gz`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/data/states/wind_rose_bremen.csv` & `foxes-0.4.2/foxes/data/states/wind_rose_bremen.csv`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/data/states/wind_rotation.nc` & `foxes-0.4.2/foxes/data/states/wind_rotation.nc`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/data/static_data.py` & `foxes-0.4.2/foxes/data/static_data.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/input/farm_layout/from_csv.py` & `foxes-0.4.2/foxes/input/farm_layout/from_csv.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/input/farm_layout/from_df.py` & `foxes-0.4.2/foxes/input/farm_layout/from_df.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/input/farm_layout/from_file.py` & `foxes-0.4.2/foxes/input/farm_layout/from_file.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/input/farm_layout/from_json.py` & `foxes-0.4.2/foxes/input/farm_layout/from_json.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/input/farm_layout/grid.py` & `foxes-0.4.2/foxes/input/farm_layout/grid.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/input/farm_layout/row.py` & `foxes-0.4.2/foxes/input/farm_layout/row.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/input/states/create/random_abl_states.py` & `foxes-0.4.2/foxes/input/states/create/random_abl_states.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/input/states/field_data_nc.py` & `foxes-0.4.2/foxes/input/states/field_data_nc.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/input/states/multi_height.py` & `foxes-0.4.2/foxes/input/states/multi_height.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/input/states/scan_ws.py` & `foxes-0.4.2/foxes/input/states/scan_ws.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/input/states/single.py` & `foxes-0.4.2/foxes/input/states/single.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/input/states/states_table.py` & `foxes-0.4.2/foxes/input/states/states_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,15 +312,19 @@
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_points)
 
         """
         z = pdata[FC.POINTS][:, :, 2]
 
         for i, v in enumerate(self._tvars):
-            pdata[v][:] = mdata[self.DATA][:, i, None]
+            if v in pdata:
+                pdata[v][:] = mdata[self.DATA][:, i, None]
+            else:
+                pdata[v] = mdata[self.DATA][:, i, None]
+                pdata.dims[v] = (FC.STATE, FC.POINT)
 
         for v, f in self.fixed_vars.items():
             pdata[v] = np.full((pdata.n_states, pdata.n_points), f, dtype=FC.DTYPE)
 
         for v, p in self._profiles.items():
             pres = p.calculate(pdata, z)
             pdata[v] = pres
```

### Comparing `foxes-0.4.1/foxes/input/windio/windio.py` & `foxes-0.4.2/foxes/input/windio/windio.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/farm_models/turbine2farm.py` & `foxes-0.4.2/foxes/models/farm_models/turbine2farm.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/model_book.py` & `foxes-0.4.2/foxes/models/model_book.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/partial_wakes/axiwake.py` & `foxes-0.4.2/foxes/models/partial_wakes/axiwake.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/partial_wakes/distsliced.py` & `foxes-0.4.2/foxes/models/partial_wakes/distsliced.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/partial_wakes/grid.py` & `foxes-0.4.2/foxes/models/partial_wakes/grid.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/partial_wakes/mapped.py` & `foxes-0.4.2/foxes/models/partial_wakes/mapped.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/partial_wakes/rotor_points.py` & `foxes-0.4.2/foxes/models/partial_wakes/rotor_points.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/partial_wakes/top_hat.py` & `foxes-0.4.2/foxes/models/partial_wakes/top_hat.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/point_models/set_uniform_data.py` & `foxes-0.4.2/foxes/models/turbine_models/table_factors.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,97 @@
+import numpy as np
 import pandas as pd
+from scipy.interpolate import interpn
 
-from foxes.core.point_data_model import PointDataModel
+from foxes.core import TurbineModel
 from foxes.utils import PandasFileHelper
 import foxes.constants as FC
-import foxes.variables as FV
 
 
-class SetUniformData(PointDataModel):
+class TableFactors(TurbineModel):
     """
-    Set uniform data (can be state dependent)
+    Multiplies variables by factors from a
+    two dimensional table.
+
+    The column names are expected to be numbers
+    that represent the col_var variable.
 
     Attributes
     ----------
-    data_source: str or pandas.DataFrame or dict
-        Either a file name, or a data frame, both assuming
-        state dependent data. Or a dict for state independent
-        uniform data (i.e., scalars)
+    data_source: str or pandas.DataFrame
+        Either path to a file or data
+    row_var: str
+        The row-wise variable
+    col_var: str
+        The column-wise variable
     ovars: list of str
-        The variables to be written
-    var2col: dict
-        Mapping from variable names to data column names
+        The variables onto which the factors
+        are multiplied
 
-    :group: models.point_models
+    :group: models.turbine_models
 
     """
 
     def __init__(
         self,
         data_source,
+        row_var,
+        col_var,
         output_vars,
-        var2col={},
-        pd_read_pars={},
+        pd_file_read_pars={},
+        **ipars,
     ):
         """
         Constructor.
 
         Parameters
         ----------
-        data_source: str or pandas.DataFrame or dict
-            Either a file name, or a data frame, both assuming
-            state dependent data. Or a dict for state independent
-            uniform data (i.e., scalars)
+        data_source: str or pandas.DataFrame
+            Either path to a file or data
+        row_var: str
+            The row-wise variable
+        col_var: str
+            The column-wise variable
         output_vars: list of str
-            The variables to be written
-        var2col: dict
-            Mapping from variable names to data column names
-        pd_read_pars: dict
-            pandas file reading parameters
+            The variables onto which the factors
+            are multiplied
+        pd_file_read_pars: dict
+            Parameters for pandas file reading
+        ipars: dict, optional
+            Parameters for scipy.interpolate.interpn
 
         """
+        super().__init__()
+
         self.data_source = data_source
+        self.row_var = row_var
+        self.col_var = col_var
         self.ovars = output_vars
-        self.var2col = var2col
+        self._rpars = pd_file_read_pars
+        self._ipars = ipars
+
+        self._cvals = None
+        self._data = None
+
+    def output_farm_vars(self, algo):
+        """
+        The variables which are being modified by the model.
+
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The calculation algorithm
 
-        self._rpars = pd_read_pars
+        Returns
+        -------
+        output_vars: list of str
+            The output variable names
+
+        """
+        return self.ovars
 
     def initialize(self, algo, verbosity=0):
         """
         Initializes the model.
 
         This includes loading all required data from files. The model
         should return all array type data as part of the idata return
@@ -76,79 +110,71 @@
         -------
         idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
-        self.VARS = self.var("VARS")
-        self.DATA = self.var("DATA")
-
         if isinstance(self.data_source, pd.DataFrame):
-            data = self.data_source[
-                [self.var2col.get(v, v) for v in self.ovars]
-            ].to_numpy(FC.DTYPE)
-        elif isinstance(self.data_source, dict):
-            pass
+            self._data = self.data_source
         else:
-            if verbosity:
-                print(f"States '{self.name}': Reading file {self.data_source}")
+            if verbosity > 0:
+                print(f"{self.name}: Reading file {self.data_source}")
             rpars = dict(index_col=0)
             rpars.update(self._rpars)
-            data = PandasFileHelper().read_file(self.data_source, **rpars)
-            data = data[[self.var2col.get(v, v) for v in self.ovars]].to_numpy(FC.DTYPE)
-
-        idata = super().initialize(algo, verbosity)
-        idata["coords"][self.VARS] = self.ovars
-        idata["data_vars"][self.DATA] = ((FC.STATE, self.VARS), data)
-
-        return idata
-
-    def output_point_vars(self, algo):
-        """
-        The variables which are being modified by the model.
-
-        Parameters
-        ----------
-        algo: foxes.core.Algorithm
-            The calculation algorithm
+            self._data = PandasFileHelper.read_file(self.data_source, **rpars)
 
-        Returns
-        -------
-        output_vars: list of str
-            The output variable names
+        self._rvals = self._data.index.to_numpy(FC.DTYPE)
+        self._cvals = self._data.columns.to_numpy(FC.DTYPE)
+        self._data = self._data.to_numpy(FC.DTYPE)
 
-        """
-        return self.ovars
+        return super().initialize(algo, verbosity)
 
-    def calculate(self, algo, mdata, fdata, pdata):
+    def calculate(self, algo, mdata, fdata, st_sel):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
-        pdata: foxes.core.Data
-            The point data
+        st_sel: numpy.ndarray of bool
+            The state-turbine selection,
+            shape: (n_states, n_turbines)
 
         Returns
         -------
         results: dict
             The resulting data, keys: output variable str.
-            Values: numpy.ndarray with shape (n_states, n_points)
+            Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
-        for v in self.ovars:
-            if self.DATA in mdata:
-                pdata[v][:] = mdata[v][None, self.ovars.index(v)]
-            else:
-                pdata[v][:] = self.data_source[v]
+        n_sel = np.sum(st_sel)
+        qts = np.zeros((n_sel, 2), dtype=FC.DTYPE)
+        qts[:, 0] = fdata[self.row_var][st_sel]
+        qts[:, 1] = fdata[self.col_var][st_sel]
+
+        try:
+            factors = interpn(
+                (self._rvals, self._cvals), self._data, qts, **self._ipars
+            )
+        except ValueError as e:
+            print(f"\nDATA       : ({self.row_var}, {self.col_var})")
+            print(
+                f"DATA BOUNDS: ({np.min(self._rvals)}, {np.min(self._cvals)}) -- ({np.max(self._rvals)}, {np.max(self._cvals)})"
+            )
+            print(
+                f"VALUE BOUNDS: ({np.min(qts[:, 0]):.4f}, {np.min(qts[:, 1]):.4f}) -- ({np.max(qts[:, 0]):.4f}, {np.max(qts[:, 1]):.4f})\n"
+            )
+            raise e
+
+        for v in self.output_farm_vars(algo):
+            fdata[v][st_sel] *= factors
 
-        return {v: pdata[v] for v in self.ovars}
+        return {v: fdata[v] for v in self.output_farm_vars(algo)}
```

### Comparing `foxes-0.4.1/foxes/models/point_models/tke2ti.py` & `foxes-0.4.2/foxes/models/point_models/tke2ti.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/point_models/wake_deltas.py` & `foxes-0.4.2/foxes/models/point_models/wake_deltas.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/rotor_models/centre.py` & `foxes-0.4.2/foxes/models/rotor_models/centre.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/rotor_models/grid.py` & `foxes-0.4.2/foxes/models/rotor_models/grid.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/turbine_models/calculator.py` & `foxes-0.4.2/foxes/models/turbine_models/calculator.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/turbine_models/kTI_model.py` & `foxes-0.4.2/foxes/models/turbine_models/kTI_model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/turbine_models/lookup_table.py` & `foxes-0.4.2/foxes/models/turbine_models/lookup_table.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/turbine_models/power_mask.py` & `foxes-0.4.2/foxes/models/turbine_models/power_mask.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/turbine_models/rotor_centre_calc.py` & `foxes-0.4.2/foxes/models/turbine_models/rotor_centre_calc.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/turbine_models/sector_management.py` & `foxes-0.4.2/foxes/models/turbine_models/sector_management.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/turbine_models/set_XYHD.py` & `foxes-0.4.2/foxes/models/turbine_models/set_XYHD.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/turbine_models/set_farm_vars.py` & `foxes-0.4.2/foxes/models/turbine_models/set_farm_vars.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/turbine_models/table_factors.py` & `foxes-0.4.2/foxes/models/wake_frames/farm_order.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,97 +1,44 @@
 import numpy as np
-import pandas as pd
-from scipy.interpolate import interpn
 
-from foxes.core import TurbineModel
-from foxes.utils import PandasFileHelper
 import foxes.constants as FC
+from .rotor_wd import RotorWD
+from foxes.core import WakeFrame
 
 
-class TableFactors(TurbineModel):
+class FarmOrder(WakeFrame):
     """
-    Multiplies variables by factors from a
-    two dimensional table.
+    Invokes turbine ordering as defined
+    by the wind farm.
 
-    The column names are expected to be numbers
-    that represent the col_var variable.
+    Warning: This is for testing purposes only, and in general
+    only gives correct calculation results when used
+    in an iterative algorithm.
 
     Attributes
     ----------
-    data_source: str or pandas.DataFrame
-        Either path to a file or data
-    row_var: str
-        The row-wise variable
-    col_var: str
-        The column-wise variable
-    ovars: list of str
-        The variables onto which the factors
-        are multiplied
+    base_frame: foxes.core.WakeFrame
+        The wake frame from which to start
 
-    :group: models.turbine_models
+    :group: models.wake_frames
 
     """
 
-    def __init__(
-        self,
-        data_source,
-        row_var,
-        col_var,
-        output_vars,
-        pd_file_read_pars={},
-        **ipars,
-    ):
+    def __init__(self, base_frame=RotorWD()):
         """
         Constructor.
 
         Parameters
         ----------
-        data_source: str or pandas.DataFrame
-            Either path to a file or data
-        row_var: str
-            The row-wise variable
-        col_var: str
-            The column-wise variable
-        output_vars: list of str
-            The variables onto which the factors
-            are multiplied
-        pd_file_read_pars: dict
-            Parameters for pandas file reading
-        ipars: dict, optional
-            Parameters for scipy.interpolate.interpn
+        base_frame: foxes.core.WakeFrame
+            The wake frame from which to start
 
         """
         super().__init__()
-
-        self.data_source = data_source
-        self.row_var = row_var
-        self.col_var = col_var
-        self.ovars = output_vars
-        self._rpars = pd_file_read_pars
-        self._ipars = ipars
-
-        self._cvals = None
-        self._data = None
-
-    def output_farm_vars(self, algo):
-        """
-        The variables which are being modified by the model.
-
-        Parameters
-        ----------
-        algo: foxes.core.Algorithm
-            The calculation algorithm
-
-        Returns
-        -------
-        output_vars: list of str
-            The output variable names
-
-        """
-        return self.ovars
+        self.base_frame = base_frame
 
     def initialize(self, algo, verbosity=0):
         """
         Initializes the model.
 
         This includes loading all required data from files. The model
         should return all array type data as part of the idata return
@@ -110,71 +57,112 @@
         -------
         idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
-        if isinstance(self.data_source, pd.DataFrame):
-            self._data = self.data_source
-        else:
-            if verbosity > 0:
-                print(f"{self.name}: Reading file {self.data_source}")
-            rpars = dict(index_col=0)
-            rpars.update(self._rpars)
-            self._data = PandasFileHelper.read_file(self.data_source, **rpars)
-
-        self._rvals = self._data.index.to_numpy(FC.DTYPE)
-        self._cvals = self._data.columns.to_numpy(FC.DTYPE)
-        self._data = self._data.to_numpy(FC.DTYPE)
+        idata = super().initialize(algo, verbosity)
+        algo.update_idata(self.base_frame, idata=idata, verbosity=verbosity)
 
-        return super().initialize(algo, verbosity)
+        return idata
 
-    def calculate(self, algo, mdata, fdata, st_sel):
+    def calc_order(self, algo, mdata, fdata):
         """ "
-        The main model calculation.
+        Calculates the order of turbine evaluation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
-        st_sel: numpy.ndarray of bool
-            The state-turbine selection,
-            shape: (n_states, n_turbines)
 
         Returns
         -------
-        results: dict
-            The resulting data, keys: output variable str.
-            Values: numpy.ndarray with shape (n_states, n_turbines)
-
-        """
-        n_sel = np.sum(st_sel)
-        qts = np.zeros((n_sel, 2), dtype=FC.DTYPE)
-        qts[:, 0] = fdata[self.row_var][st_sel]
-        qts[:, 1] = fdata[self.col_var][st_sel]
-
-        try:
-            factors = interpn(
-                (self._rvals, self._cvals), self._data, qts, **self._ipars
-            )
-        except ValueError as e:
-            print(f"\nDATA       : ({self.row_var}, {self.col_var})")
-            print(
-                f"DATA BOUNDS: ({np.min(self._rvals)}, {np.min(self._cvals)}) -- ({np.max(self._rvals)}, {np.max(self._cvals)})"
-            )
-            print(
-                f"VALUE BOUNDS: ({np.min(qts[:, 0]):.4f}, {np.min(qts[:, 1]):.4f}) -- ({np.max(qts[:, 0]):.4f}, {np.max(qts[:, 1]):.4f})\n"
-            )
-            raise e
+        order: numpy.ndarray
+            The turbine order, shape: (n_states, n_turbines)
+
+        """
+        order = np.zeros((fdata.n_states, fdata.n_turbines), dtype=FC.ITYPE)
+        order[:] = np.arange(fdata.n_turbines)[None, :]
+
+        return order
+
+    def get_wake_coos(self, algo, mdata, fdata, pdata, states_source_turbine):
+        """
+        Calculate wake coordinates.
+
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+        mdata: foxes.core.Data
+            The model data
+        fdata: foxes.core.Data
+            The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
+        states_source_turbine: numpy.ndarray
+            For each state, one turbine index for the
+            wake causing turbine. Shape: (n_states,)
+
+        Returns
+        -------
+        wake_coos: numpy.ndarray
+            The wake frame coordinates of the evaluation
+            points, shape: (n_states, n_points, 3)
+
+        """
+        return self.base_frame.get_wake_coos(
+            algo, mdata, fdata, pdata, states_source_turbine
+        )
 
-        for v in self.output_farm_vars(algo):
-            fdata[v][st_sel] *= factors
+    def get_centreline_points(self, algo, mdata, fdata, states_source_turbine, x):
+        """
+        Gets the points along the centreline for given
+        values of x.
 
-        return {v: fdata[v] for v in self.output_farm_vars(algo)}
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+        mdata: foxes.core.Data
+            The model data
+        fdata: foxes.core.Data
+            The farm data
+        states_source_turbine: numpy.ndarray
+            For each state, one turbine index for the
+            wake causing turbine. Shape: (n_states,)
+        x: numpy.ndarray
+            The wake frame x coordinates, shape: (n_states, n_points)
+
+        Returns
+        -------
+        points: numpy.ndarray
+            The centreline points, shape: (n_states, n_points, 3)
+
+        """
+        return self.base_frame.get_centreline_points(
+            algo, mdata, fdata, states_source_turbine, x
+        )
+
+    def finalize(self, algo, verbosity=0):
+        """
+        Finalizes the model.
+
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+        verbosity: int
+            The verbosity level, 0 = silent
+
+        """
+        if self.base_frame.initialized:
+            self.base_frame.finalize(algo, verbosity)
+        super().finalize(algo, verbosity)
```

### Comparing `foxes-0.4.1/foxes/models/turbine_models/thrust2ct.py` & `foxes-0.4.2/foxes/models/turbine_models/thrust2ct.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/turbine_models/yaw2yawm.py` & `foxes-0.4.2/foxes/models/turbine_models/yaw2yawm.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/turbine_models/yawm2yaw.py` & `foxes-0.4.2/foxes/models/turbine_models/yawm2yaw.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/turbine_types/CpCt_file.py` & `foxes-0.4.2/foxes/models/turbine_types/CpCt_file.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/turbine_types/CpCt_from_two.py` & `foxes-0.4.2/foxes/models/turbine_types/CpCt_from_two.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/turbine_types/PCt_file.py` & `foxes-0.4.2/foxes/models/turbine_types/PCt_file.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/turbine_types/PCt_from_two.py` & `foxes-0.4.2/foxes/models/turbine_types/PCt_from_two.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/turbine_types/null_type.py` & `foxes-0.4.2/foxes/models/turbine_types/null_type.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/turbine_types/wsrho2PCt_from_two.py` & `foxes-0.4.2/foxes/models/turbine_types/wsrho2PCt_from_two.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/vertical_profiles/abl_log_neutral_ws.py` & `foxes-0.4.2/foxes/models/vertical_profiles/abl_log_neutral_ws.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/vertical_profiles/abl_log_stable_ws.py` & `foxes-0.4.2/foxes/models/vertical_profiles/abl_log_stable_ws.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/vertical_profiles/abl_log_unstable_ws.py` & `foxes-0.4.2/foxes/models/vertical_profiles/abl_log_unstable_ws.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/vertical_profiles/abl_log_ws.py` & `foxes-0.4.2/foxes/models/vertical_profiles/abl_log_ws.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/vertical_profiles/sheared_ws.py` & `foxes-0.4.2/foxes/models/vertical_profiles/sheared_ws.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/vertical_profiles/uniform.py` & `foxes-0.4.2/foxes/models/vertical_profiles/uniform.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/wake_frames/rotor_wd.py` & `foxes-0.4.2/foxes/models/wake_frames/rotor_wd.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/wake_frames/streamlines.py` & `foxes-0.4.2/foxes/models/wake_frames/streamlines.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/wake_frames/timelines.py` & `foxes-0.4.2/foxes/models/wake_frames/timelines.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/wake_frames/yawed_wakes.py` & `foxes-0.4.2/foxes/models/wake_frames/yawed_wakes.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/wake_models/axisymmetric.py` & `foxes-0.4.2/foxes/models/wake_models/axisymmetric.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/wake_models/dist_sliced.py` & `foxes-0.4.2/foxes/models/wake_models/dist_sliced.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/wake_models/gaussian.py` & `foxes-0.4.2/foxes/models/wake_models/gaussian.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/wake_models/ti/crespo_hernandez.py` & `foxes-0.4.2/foxes/models/wake_models/ti/crespo_hernandez.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/wake_models/ti/iec_ti.py` & `foxes-0.4.2/foxes/models/wake_models/ti/iec_ti.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/wake_models/top_hat.py` & `foxes-0.4.2/foxes/models/wake_models/top_hat.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/wake_models/wind/bastankhah.py` & `foxes-0.4.2/foxes/models/wake_models/wind/bastankhah.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/wake_models/wind/jensen.py` & `foxes-0.4.2/foxes/models/wake_models/wind/jensen.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/wake_models/wind/porte_agel.py` & `foxes-0.4.2/foxes/models/wake_models/wind/porte_agel.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/wake_models/wind/turbopark.py` & `foxes-0.4.2/foxes/models/wake_models/wind/turbopark.py`

 * *Files 4% similar despite different names*

```diff
@@ -297,20 +297,21 @@
 
         self.dx = dx
         self.A = A
         self.ct_max = ct_max
         self.sbeta_factor = sbeta_factor
         self.ti_var = ti_var
         self.ipars = ipars
+        self._tiwakes = None
 
     def __repr__(self):
         s = super().__repr__()
         s += f"(ti={self.ti_var}, dx={self.dx}, A={self.A}, sp={self.superpositions[FV.WS]})"
         return s
-
+    
     def init_wake_deltas(self, algo, mdata, fdata, pdata, wake_deltas):
         """
         Initialize wake delta storage.
 
         They are added on the fly to the wake_deltas dict.
 
         Parameters
@@ -329,14 +330,25 @@
             wake delta applies, values: numpy.ndarray with
             shape (n_states, n_points, ...)
 
         """
         n_states = mdata.n_states
         wake_deltas[FV.WS] = np.zeros((n_states, pdata.n_points), dtype=FC.DTYPE)
 
+        # find TI wake models:
+        self._tiwakes = []
+        for w in algo.wake_models:
+            if w is not self:
+                wdel = {}
+                w.init_wake_deltas(algo, mdata, fdata, pdata, wdel)
+                if self.ti_var in wdel:
+                    self._tiwakes.append(w)
+        if len(self._tiwakes) == 0:
+            raise KeyError(f"Model '{self.name}': Missing wake model that computes wake delta for variable {self.ti_var}")
+
     def calc_amplitude_sigma_spsel(
         self,
         algo,
         mdata,
         fdata,
         pdata,
         states_source_turbine,
@@ -408,23 +420,24 @@
 
             # calculate sigma:
             sbeta = np.sqrt(0.5 * (1 + np.sqrt(1.0 - ct)) / np.sqrt(1.0 - ct))
             # sblim = 1 / (np.sqrt(8) * self.sbeta_factor)
             # sbeta[sbeta > sblim] = sblim
             epsilon = self.sbeta_factor * sbeta
 
-            # get TI by integratiion along centre line:
+            # get TI by integration along centre line:
             ti_ix = algo.wake_frame.calc_centreline_integral(
                 algo,
                 mdata,
                 fdata,
                 states_source_turbine,
                 [self.ti_var],
                 x,
                 dx=self.dx,
+                wake_models=self._tiwakes,
                 **self.ipars,
             )[:, :, 0]
 
             # calculate sigma (eqn 1, plus epsilon from eqn 4 for x = 0)
             sigma = D * epsilon + self.A * ti_ix[sp_sel]
 
             del (
@@ -447,7 +460,22 @@
         else:
             sp_sel = np.zeros_like(x, dtype=bool)
             n_sp = np.sum(sp_sel)
             ampld = np.zeros(n_sp, dtype=FC.DTYPE)
             sigma = np.zeros(n_sp, dtype=FC.DTYPE)
 
         return {FV.WS: (ampld, sigma)}, sp_sel
+
+    def finalize(self, algo, verbosity=0):
+        """
+        Finalizes the model.
+
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+        verbosity: int
+            The verbosity level, 0 = silent
+
+        """
+        self._tiwakes = None
+        super().finalize(algo, verbosity)
```

### Comparing `foxes-0.4.1/foxes/models/wake_superpositions/linear.py` & `foxes-0.4.2/foxes/models/wake_superpositions/linear.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/wake_superpositions/max.py` & `foxes-0.4.2/foxes/models/wake_superpositions/max.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/wake_superpositions/product.py` & `foxes-0.4.2/foxes/models/wake_superpositions/product.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/wake_superpositions/quadratic.py` & `foxes-0.4.2/foxes/models/wake_superpositions/quadratic.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/models/wake_superpositions/ti_superp.py` & `foxes-0.4.2/foxes/models/wake_superpositions/ti_superp.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/opt/constraints/area_geometry.py` & `foxes-0.4.2/foxes/opt/constraints/area_geometry.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/opt/constraints/min_dist.py` & `foxes-0.4.2/foxes/opt/constraints/min_dist.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/opt/core/farm_constraint.py` & `foxes-0.4.2/foxes/opt/core/farm_constraint.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/opt/core/farm_objective.py` & `foxes-0.4.2/foxes/opt/core/farm_objective.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/opt/core/farm_opt_problem.py` & `foxes-0.4.2/foxes/opt/core/farm_opt_problem.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/opt/core/farm_vars_problem.py` & `foxes-0.4.2/foxes/opt/core/farm_vars_problem.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/opt/core/pop_states.py` & `foxes-0.4.2/foxes/opt/core/pop_states.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/opt/objectives/farm_vars.py` & `foxes-0.4.2/foxes/opt/objectives/farm_vars.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/opt/objectives/max_n_turbines.py` & `foxes-0.4.2/foxes/opt/objectives/max_n_turbines.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/opt/problems/layout/farm_layout.py` & `foxes-0.4.2/foxes/opt/problems/layout/farm_layout.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/opt/problems/layout/geom_layouts/constraints.py` & `foxes-0.4.2/foxes/opt/problems/layout/geom_layouts/constraints.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/opt/problems/layout/geom_layouts/geom_layout.py` & `foxes-0.4.2/foxes/opt/problems/layout/geom_layouts/geom_layout.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/opt/problems/layout/geom_layouts/geom_layout_gridded.py` & `foxes-0.4.2/foxes/opt/problems/layout/geom_layouts/geom_layout_gridded.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/opt/problems/layout/geom_layouts/geom_reggrid.py` & `foxes-0.4.2/foxes/opt/problems/layout/geom_layouts/geom_reggrid.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/opt/problems/layout/geom_layouts/geom_reggrids.py` & `foxes-0.4.2/foxes/opt/problems/layout/geom_layouts/geom_reggrids.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/opt/problems/layout/geom_layouts/objectives.py` & `foxes-0.4.2/foxes/opt/problems/layout/geom_layouts/objectives.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/opt/problems/layout/reggrids_layout.py` & `foxes-0.4.2/foxes/opt/problems/layout/reggrids_layout.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/opt/problems/layout/regular_layout.py` & `foxes-0.4.2/foxes/opt/problems/layout/regular_layout.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/opt/problems/opt_farm_vars.py` & `foxes-0.4.2/foxes/opt/problems/opt_farm_vars.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/output/farm_layout.py` & `foxes-0.4.2/foxes/output/farm_layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,14 +123,16 @@
         annotate=1,
         title=None,
         fig=None,
         ax=None,
         normalize_D=False,
         ret_im=False,
         bargs={},
+        anno_delx=0,
+        anno_dely=0,
         **kwargs,
     ):
         """
         Creates farm layout figure.
 
         Parameters
         ----------
@@ -155,14 +157,18 @@
             The axis object, to which to add
         normalize_D: bool
             Normalize x, y wrt rotor diameter
         ret_im: bool
             Flag for returned image object
         bargs: dict
             Arguments for boundary plotting
+        anno_delx: float
+            The annotation delta x
+        anno_dely: float
+            The annotation delta y
         kwargs: dict, optional
             Parameters forwarded to `matplotlib.pyplot.scatter`
 
         Returns
         -------
         ax: matplotlib.pyplot.Axis
             The axis object
@@ -228,18 +234,18 @@
                         f"Unknown color_by '{color_by}'. Choose: mean_X, sum_X, min_X, max_X, where X is a farm_results variable"
                     )
 
             im = ax.scatter(x, y, **kw)
 
             if annotate == 1:
                 for i, txt in enumerate(n):
-                    ax.annotate(int(txt), (x[i], y[i]), size=fontsize)
+                    ax.annotate(int(txt), (x[i]+anno_delx, y[i]+anno_dely), size=fontsize)
             elif annotate == 2:
                 for i, t in enumerate(self.farm.turbines):
-                    ax.annotate(t.name, (x[i], y[i]), size=fontsize)
+                    ax.annotate(t.name, (x[i]+anno_delx, y[i]+anno_dely), size=fontsize)
 
         if self.farm.boundary is not None:
             hbargs = {"fill_mode": "inside_lightgray"}
             hbargs.update(bargs)
             self.farm.boundary.add_to_figure(ax, **hbargs)
 
         ti = (
```

### Comparing `foxes-0.4.1/foxes/output/farm_results_eval.py` & `foxes-0.4.2/foxes/output/farm_results_eval.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import numpy as np
 import pandas as pd
+from cycler import cycler
+import matplotlib.pyplot as plt
 
 from .output import Output
 import foxes.variables as FV
 import foxes.constants as FC
 
 
 class FarmResultsEval(Output):
@@ -548,7 +550,82 @@
         eff: float
             The farm efficiency
 
         """
         P = self.calc_mean_farm_power()
         P0 = self.calc_mean_farm_power(ambient=True) + 1e-14
         return P / P0
+
+    def gen_stdata(
+            self, 
+            turbines, 
+            variable, 
+            fig=None, 
+            ax=None, 
+            figsize=None,
+            legloc="lower right",
+            animated=True,
+            ret_im=True,
+        ):
+        """
+        Generates state-turbine data,
+        intended to be used in animations
+
+        Parameters
+        ----------
+        turbines: list of int
+            The turbines for which to scatter data
+        variable: str
+            The variable name
+        fig: plt.Figure, optional
+            The figure object
+        ax: plt.Axes, optional
+            The figure axes
+        figsize: tuple, optional
+            The figsize for plt.Figure
+        legloc: str
+            The legend location
+        animated: bool
+            Flag for animated output
+        ret_im: bool
+            Flag for image return,
+
+        Yields
+        ------
+        fig: matplotlib.Figure
+            The figure object
+        im: List of matplotlib.collections.PathCollection, optional
+            The scatter artists
+
+        """
+
+        if fig is None:
+            hfig = plt.figure(figsize=figsize)
+        else:
+            hfig = fig
+        if ax is None:
+            hax = hfig.add_subplot(111)
+        else:
+            hax = ax
+
+        hax.set_xlabel(f"State")
+        hax.set_ylabel(variable)
+        cc = cycler(color='bgrcmyk') 
+        
+        data = self.results[variable].to_numpy()
+        hasl = set()
+        for si in range(len(data)):
+
+            im = []
+            hax.set_prop_cycle(cc)
+            for ti in turbines:
+                lbl = None if ti in hasl else f"Turbine {ti}"
+                im += hax.plot(range(si), data[:si, ti], label=lbl,
+                                animated=animated)
+                hasl.add(ti)
+
+            hax.legend(loc=legloc)
+
+            if ret_im:
+                yield hfig, im
+            else:
+                yield hfig
```

### Comparing `foxes-0.4.1/foxes/output/flow_plots_2d.py` & `foxes-0.4.2/foxes/output/flow_plots_2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,15 @@
         if animated and title is None:
             if hasattr(s, "dtype") and np.issubdtype(s.dtype, np.datetime64):
                 t = np.datetime_as_string(s, unit="m").replace("T", " ")
             else:
                 t = s
             ttl = hax.text(
                 0.5,
-                1.02,
+                1.05,
                 f"State {t}",
                 backgroundcolor="w",
                 transform=hax.transAxes,
                 ha="center",
                 animated=True,
                 clip_on=False,
             )
@@ -266,40 +266,40 @@
             The title
         vlabel: str, optional
             The variable label
         fig: plt.Figure, optional
             The figure object
         ax: plt.Axes, optional
             The figure axes
-        add_bar: bool, optional
+        add_bar: bool
             Add a color bar
         cmap: str, optional
             The colormap
         weight_turbine: int, optional
             Index of the turbine from which to take the weight
         verbosity: int, optional
             The verbosity level
-        ret_state: bool, optional
+        ret_state: bool
             Flag for state index return
-        ret_im: bool, optional
+        ret_im: bool
             Flag for image return
         animated: bool
             Switch for usage for an animation
         kwargs: dict, optional
             Parameters forwarded to the algorithm's calc_points
             function.
 
         Yields
         ------
         fig: matplotlib.Figure
             The figure object
         si: int, optional
             The state index
         im: tuple, optional
-            The image objects, atplotlib.collections.QuadMesh
+            The image objects, matplotlib.collections.QuadMesh
             or matplotlib.QuadContourSet
 
         """
 
         # prepare:
         n_states = self.algo.n_states
 
@@ -478,40 +478,40 @@
             The title
         vlabel: str, optional
             The variable label
         fig: plt.Figure, optional
             The figure object
         ax: plt.Axes, optional
             The figure axes
-        add_bar: bool, optional
+        add_bar: bool
             Add a color bar
         cmap: str, optional
             The colormap
         weight_turbine: int, optional
             Index of the turbine from which to take the weight
         verbosity: int, optional
             The verbosity level
-        ret_state: bool, optional
+        ret_state: bool
             Flag for state index return
-        ret_im: bool, optional
+        ret_im: bool
             Flag for image return
         animated: bool
             Switch for usage for an animation
         kwargs: dict, optional
             Parameters forwarded to the algorithm's calc_points
             function.
 
         Yields
         ------
         fig: matplotlib.Figure
             The figure object
         si: int, optional
             The state index
         im: tuple, optional
-            The image objects, atplotlib.collections.QuadMesh
+            The image objects, matplotlib.collections.QuadMesh
             or matplotlib.QuadContourSet
 
         """
 
         # prepare:
         n_states = self.algo.n_states
         n_turbines = self.algo.n_turbines
@@ -706,40 +706,40 @@
             The title
         vlabel: str, optional
             The variable label
         fig: plt.Figure, optional
             The figure object
         ax: plt.Axes, optional
             The figure axes
-        add_bar: bool, optional
+        add_bar: bool
             Add a color bar
         cmap: str, optional
             The colormap
         weight_turbine: int, optional
             Index of the turbine from which to take the weight
         verbosity: int, optional
             The verbosity level
-        ret_state: bool, optional
+        ret_state: bool
             Flag for state index return
-        ret_im: bool, optional
+        ret_im: bool
             Flag for image return
         animated: bool
             Switch for usage for an animation
         kwargs: dict, optional
             Parameters forwarded to the algorithm's calc_points
             function.
 
         Yields
         ------
         fig: matplotlib.Figure
             The figure object
         si: int, optional
             The state index
         im: tuple, optional
-            The image objects, atplotlib.collections.QuadMesh
+            The image objects, matplotlib.collections.QuadMesh
             or matplotlib.QuadContourSet
 
         """
 
         # prepare:
         n_states = self.algo.n_states
         n_turbines = self.algo.n_turbines
@@ -930,42 +930,42 @@
             The title
         vlabel: str, optional
             The variable label
         fig: plt.Figure, optional
             The figure object
         ax: plt.Axes, optional
             The figure axes
-        add_bar: bool, optional
+        add_bar: bool
             Add a color bar
         cmap: str, optional
             The colormap
         quiver_n: int, optional
             Place a vector at each `n`th point
         quiver_pars: dict, optional
             Parameters for plt.quiver
         verbosity: int, optional
             The verbosity level
-        ret_state: bool, optional
+        ret_state: bool
             Flag for state index return
-        ret_im: bool, optional
+        ret_im: bool
             Flag for image return
         animated: bool
             Switch for usage for an animation
         kwargs: dict, optional
             Parameters forwarded to the algorithm's calc_points
             function.
 
         Yields
         ------
         fig: matplotlib.Figure
             The figure object
         si: int, optional
             The state index
         im: tuple, optional
-            The image objects, atplotlib.collections.QuadMesh
+            The image objects, matplotlib.collections.QuadMesh
             or matplotlib.QuadContourSet
 
         """
 
         # prepare:
         n_states = self.algo.n_states
 
@@ -1158,42 +1158,42 @@
             The title
         vlabel: str, optional
             The variable label
         fig: plt.Figure, optional
             The figure object
         ax: plt.Axes, optional
             The figure axes
-        add_bar: bool, optional
+        add_bar: bool
             Add a color bar
         cmap: str, optional
             The colormap
         quiver_n: int, optional
             Place a vector at ech `n`th point
         quiver_pars: dict, optional
             Parameters for plt.quiver
         verbosity: int, optional
             The verbosity level
-        ret_state: bool, optional
+        ret_state: bool
             Flag for state index return
-        ret_im: bool, optional
+        ret_im: bool
             Flag for image return
         animated: bool
             Switch for usage for an animation
         kwargs: dict, optional
             Parameters forwarded to the algorithm's calc_points
             function.
 
         Yields
         ------
         fig: matplotlib.Figure
             The figure object
         si: int, optional
             The state index
         im: tuple, optional
-            The image objects, atplotlib.collections.QuadMesh
+            The image objects, matplotlib.collections.QuadMesh
             or matplotlib.QuadContourSet
 
         """
 
         # prepare:
         n_states = self.algo.n_states
         n_turbines = self.algo.n_turbines
@@ -1403,42 +1403,42 @@
             The title
         vlabel: str, optional
             The variable label
         fig: plt.Figure, optional
             The figure object
         ax: plt.Axes, optional
             The figure axes
-        add_bar: bool, optional
+        add_bar: bool
             Add a color bar
         cmap: str, optional
             The colormap
         quiver_n: int, optional
             Place a vector at ech `n`th point
         quiver_pars: dict, optional
             Parameters for plt.quiver
         verbosity: int, optional
             The verbosity level
-        ret_state: bool, optional
+        ret_state: bool
             Flag for state index return
-        ret_im: bool, optional
+        ret_im: bool
             Flag for image return
         animated: bool
             Switch for usage for an animation
         kwargs: dict, optional
             Parameters forwarded to the algorithm's calc_points
             function.
 
         Yields
         ------
         fig: matplotlib.Figure
             The figure object
         si: int, optional
             The state index
         im: tuple, optional
-            The image objects, atplotlib.collections.QuadMesh
+            The image objects, matplotlib.collections.QuadMesh
             or matplotlib.QuadContourSet
 
         """
 
         # prepare:
         n_states = self.algo.n_states
         n_turbines = self.algo.n_turbines
```

### Comparing `foxes-0.4.1/foxes/output/output.py` & `foxes-0.4.2/foxes/output/output.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/output/results_writer.py` & `foxes-0.4.2/foxes/output/results_writer.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/output/rose_plot.py` & `foxes-0.4.2/foxes/output/rose_plot.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/output/state_turbine_map.py` & `foxes-0.4.2/foxes/output/state_turbine_map.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/output/turbine_type_curves.py` & `foxes-0.4.2/foxes/output/turbine_type_curves.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/utils/abl/neutral.py` & `foxes-0.4.2/foxes/utils/abl/neutral.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/utils/abl/stable.py` & `foxes-0.4.2/foxes/utils/abl/stable.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/utils/abl/unstable.py` & `foxes-0.4.2/foxes/utils/abl/unstable.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/utils/cubic_roots.py` & `foxes-0.4.2/foxes/utils/cubic_roots.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/utils/data_book.py` & `foxes-0.4.2/foxes/utils/data_book.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/utils/dict.py` & `foxes-0.4.2/foxes/utils/dict.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/utils/geom2d/area_geometry.py` & `foxes-0.4.2/foxes/utils/geom2d/area_geometry.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/utils/geom2d/circle.py` & `foxes-0.4.2/foxes/utils/geom2d/circle.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/utils/geom2d/example_intersection.py` & `foxes-0.4.2/foxes/utils/geom2d/example_intersection.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/utils/geom2d/example_union.py` & `foxes-0.4.2/foxes/utils/geom2d/example_union.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/utils/geom2d/half_plane.py` & `foxes-0.4.2/foxes/utils/geom2d/half_plane.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/utils/geom2d/polygon.py` & `foxes-0.4.2/foxes/utils/geom2d/polygon.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/utils/geopandas_helpers.py` & `foxes-0.4.2/foxes/utils/geopandas_helpers.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/utils/pandas_helpers.py` & `foxes-0.4.2/foxes/utils/pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/utils/runners/runners.py` & `foxes-0.4.2/foxes/utils/runners/runners.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/utils/two_circles.py` & `foxes-0.4.2/foxes/utils/two_circles.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/utils/wind_dir.py` & `foxes-0.4.2/foxes/utils/wind_dir.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes/variables.py` & `foxes-0.4.2/foxes/variables.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.1/foxes.egg-info/PKG-INFO` & `foxes-0.4.2/foxes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxes
-Version: 0.4.1
+Version: 0.4.2
 Summary: Farm Optimization and eXtended yield Evaluation Software
 Author: Fraunhofer IWES
 Author-email: jonas.schmidt@iwes.fraunhofer.de
 License: MIT
 Project-URL: Source Code, https://github.com/FraunhoferIWES/foxes
 Project-URL: Bug Tracker, https://github.com/FraunhoferIWES/foxes/issues
 Project-URL: Documentation, https://fraunhoferiwes.github.io/foxes.docs/index.html
```

### Comparing `foxes-0.4.1/foxes.egg-info/SOURCES.txt` & `foxes-0.4.2/foxes.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -180,14 +180,15 @@
 foxes/opt/problems/layout/geom_layouts/constraints.py
 foxes/opt/problems/layout/geom_layouts/geom_layout.py
 foxes/opt/problems/layout/geom_layouts/geom_layout_gridded.py
 foxes/opt/problems/layout/geom_layouts/geom_reggrid.py
 foxes/opt/problems/layout/geom_layouts/geom_reggrids.py
 foxes/opt/problems/layout/geom_layouts/objectives.py
 foxes/output/__init__.py
+foxes/output/animation.py
 foxes/output/farm_layout.py
 foxes/output/farm_results_eval.py
 foxes/output/flow_plots_2d.py
 foxes/output/output.py
 foxes/output/results_writer.py
 foxes/output/rose_plot.py
 foxes/output/state_turbine_map.py
```

### Comparing `foxes-0.4.1/setup.cfg` & `foxes-0.4.2/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 	dask[distributed]
 	scipy
 	netcdf4
 	plotly
 	kaleido
 	iwopy>=0.1.4
 	pymoo>=0.6
-	tqdm
 
 [options.extras_require]
 test = 
 	flake8
 	pytest
 doc = 
 	sphinx
```

