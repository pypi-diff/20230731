# Comparing `tmp/pandapipes-0.8.4.zip` & `tmp/pandapipes-0.8.5.zip`

## zipinfo {}

```diff
@@ -1,472 +1,474 @@
-Zip file size: 1440198 bytes, number of entries: 470
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/.github/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/
--rw-r--r--  2.0 unx    16441 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/PKG-INFO
--rw-r--r--  2.0 unx    12217 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/CHANGELOG.rst
--rw-r--r--  2.0 unx      618 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/AUTHORS
--rw-r--r--  2.0 unx     2352 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/setup.py
--rw-r--r--  2.0 unx      109 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/setup.cfg
--rw-r--r--  2.0 unx     3036 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/README.rst
--rw-r--r--  2.0 unx      159 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/MANIFEST.in
--rw-r--r--  2.0 unx     1676 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/LICENSE
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/.github/workflows/
--rw-r--r--  2.0 unx     3329 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/.github/workflows/release.yml
--rw-r--r--  2.0 unx     4728 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/.github/workflows/run_tests_develop.yml
--rw-r--r--  2.0 unx     3431 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/.github/workflows/run_tests_master.yml
--rw-r--r--  2.0 unx    16441 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes.egg-info/PKG-INFO
--rw-r--r--  2.0 unx    23636 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       11 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes.egg-info/top_level.txt
--rw-r--r--  2.0 unx      277 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes.egg-info/requires.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes.egg-info/dependency_links.txt
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/timeseries/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/std_types/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/pf/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/io/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/converter/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/control/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/component_models/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/topology/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/multinet/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/plotting/
--rw-r--r--  2.0 unx    15101 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/pipeflow.py
--rw-r--r--  2.0 unx    87241 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/create.py
--rw-r--r--  2.0 unx      745 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/__init__.py
--rw-r--r--  2.0 unx     1011 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/constants.py
--rw-r--r--  2.0 unx    28258 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/toolbox.py
--rw-r--r--  2.0 unx      928 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/idx_node.py
--rw-r--r--  2.0 unx     3231 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/pandapipes_net.py
--rw-r--r--  2.0 unx     1894 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/idx_branch.py
--rw-r--r--  2.0 unx     5243 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/timeseries/run_time_series.py
--rw-r--r--  2.0 unx      406 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/timeseries/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/std_types/library/
--rw-r--r--  2.0 unx     8846 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/std_types/std_types.py
--rw-r--r--  2.0 unx      360 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/std_types/__init__.py
--rw-r--r--  2.0 unx    10171 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/std_types/std_type_class.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/std_types/library/Pump/
--rw-r--r--  2.0 unx     8971 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/std_types/library/Pipe.csv
--rw-r--r--  2.0 unx       51 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/std_types/library/Pump/P3.csv
--rw-r--r--  2.0 unx       58 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/std_types/library/Pump/P2.csv
--rw-r--r--  2.0 unx       45 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/std_types/library/Pump/P1.csv
--rw-r--r--  2.0 unx     8985 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/pf/build_system_matrix.py
--rw-r--r--  2.0 unx    29751 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/pf/pipeflow_setup.py
--rw-r--r--  2.0 unx     8666 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/pf/derivative_toolbox_numba.py
--rw-r--r--  2.0 unx     8103 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/pf/derivative_calculation.py
--rw-r--r--  2.0 unx    12526 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/pf/result_extraction.py
--rw-r--r--  2.0 unx      403 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/pf/__init__.py
--rw-r--r--  2.0 unx     5374 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/pf/internals_toolbox.py
--rw-r--r--  2.0 unx     6682 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/pf/derivative_toolbox.py
--rw-r--r--  2.0 unx     6384 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/io/file_io.py
--rw-r--r--  2.0 unx      312 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/io/__init__.py
--rw-r--r--  2.0 unx     3069 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/io/convert_format.py
--rw-r--r--  2.0 unx     4881 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/io/io_utils.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/stanet_comparison/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/openmodelica_comparison/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/io/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/converter/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/networks/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/multinet/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/properties/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/plotting/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/
--rw-r--r--  2.0 unx    14678 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/test_toolbox.py
--rw-r--r--  2.0 unx     4258 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/run_tests.py
--rw-r--r--  2.0 unx      541 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/__init__.py
--rw-r--r--  2.0 unx      744 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/test_imports.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/
--rw-r--r--  2.0 unx     1271 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/test_update_matrix.py
--rw-r--r--  2.0 unx     3987 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/test_pipeflow_modes.py
--rw-r--r--  2.0 unx     2493 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/test_options.py
--rw-r--r--  2.0 unx    24386 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/test_inservice.py
--rw-r--r--  2.0 unx      346 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/__init__.py
--rw-r--r--  2.0 unx     1416 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/test_non_convergence.py
--rw-r--r--  2.0 unx     7253 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/test_time_series.py
--rw-r--r--  2.0 unx    15454 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/test_pipeflow_analytic_comparison.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_results/
--rw-r--r--  2.0 unx      332 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/Temperature_masche_1load_an.csv
--rw-r--r--  2.0 unx      152 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_valve.csv
--rw-r--r--  2.0 unx     1178 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_source_profiles.csv
--rw-r--r--  2.0 unx      266 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/Temperature_masche_1load_direction_an.csv
--rw-r--r--  2.0 unx       71 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_pump.csv
--rw-r--r--  2.0 unx      325 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/Temperature_2zu_2ab_an.csv
--rw-r--r--  2.0 unx       56 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/pressure_control_test_analytical.csv
--rw-r--r--  2.0 unx       11 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/ext_grid_p.csv
--rw-r--r--  2.0 unx       22 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/hydraulics.csv
--rw-r--r--  2.0 unx      196 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/Temperature_tee_2ab_1zu_an.csv
--rw-r--r--  2.0 unx      127 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_circ_pump_mass.csv
--rw-r--r--  2.0 unx      182 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/Temperature_tee_2zu_1ab_an.csv
--rw-r--r--  2.0 unx       93 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/heat_exchanger_test.csv
--rw-r--r--  2.0 unx       57 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_pressure_control.csv
--rw-r--r--  2.0 unx      300 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/Temperature_one_pipe_an.csv
--rw-r--r--  2.0 unx     1893 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/gas_sections_an.csv
--rw-r--r--  2.0 unx      133 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_circ_pump_pressure.csv
--rw-r--r--  2.0 unx     3427 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_sink_profiles.csv
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_sink/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_ext_grid/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_junction/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_source/
--rw-r--r--  2.0 unx     5944 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/lambda.csv
--rw-r--r--  2.0 unx     5737 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/reynolds.csv
--rw-r--r--  2.0 unx     5381 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/v_mean_m_per_s.csv
--rw-r--r--  2.0 unx     3431 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_sink/mdot_kg_per_s.csv
--rw-r--r--  2.0 unx     1171 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_ext_grid/mdot_kg_per_s.csv
--rw-r--r--  2.0 unx     4901 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_junction/p_bar.csv
--rw-r--r--  2.0 unx     1181 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_source/mdot_kg_per_s.csv
--rw-r--r--  2.0 unx     6912 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/stanet_comparison/pipeflow_stanet_comparison.py
--rw-r--r--  2.0 unx    11177 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/stanet_comparison/test_gas_stanet.py
--rw-r--r--  2.0 unx      264 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/stanet_comparison/__init__.py
--rw-r--r--  2.0 unx    11373 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/stanet_comparison/test_water_stanet.py
--rw-r--r--  2.0 unx     4103 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/openmodelica_comparison/test_heat_transfer_openmodelica.py
--rw-r--r--  2.0 unx    12229 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/openmodelica_comparison/test_water_openmodelica.py
--rw-r--r--  2.0 unx    11348 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/openmodelica_comparison/pipeflow_openmodelica_comparison.py
--rw-r--r--  2.0 unx      264 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/openmodelica_comparison/__init__.py
--rw-r--r--  2.0 unx     6422 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/io/test_file_io.py
--rw-r--r--  2.0 unx      264 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/io/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/converter/converter_test_files/
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/converter/__init__.py
--rw-r--r--  2.0 unx     3518 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/converter/test_stanet_converter.py
--rw-r--r--  2.0 unx   592867 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_2valvepipe.csv
--rw-r--r--  2.0 unx   899403 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/converter/converter_test_files/Exampelonia_mini.csv
--rw-r--r--  2.0 unx   618341 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_valve_2sliders_closed.csv
--rw-r--r--  2.0 unx   618340 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_valve_2sliders_open.csv
--rw-r--r--  2.0 unx      264 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/networks/__init__.py
--rw-r--r--  2.0 unx      983 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/networks/test_networks.py
--rw-r--r--  2.0 unx      238 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/multinet/__init__.py
--rw-r--r--  2.0 unx    16572 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/multinet/test_control_multinet.py
--rw-r--r--  2.0 unx     6176 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/multinet/test_time_series_multinet.py
--rw-r--r--  2.0 unx      264 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/properties/__init__.py
--rw-r--r--  2.0 unx    19769 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/properties/test_properties_toolbox.py
--rw-r--r--  2.0 unx     2564 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/properties/test_fluid_specials.py
--rw-r--r--  2.0 unx     9471 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/plotting/test_collections.py
--rw-r--r--  2.0 unx     1987 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/plotting/test_pipeflow_results.py
--rw-r--r--  2.0 unx      264 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/plotting/__init__.py
--rw-r--r--  2.0 unx     7984 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/plotting/test_simple_collections.py
--rw-r--r--  2.0 unx     1467 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/plotting/test_generic_coordinates.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/test_components/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/release_cycle/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/old_versions/
--rw-r--r--  2.0 unx      688 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/test_aux_function.py
--rw-r--r--  2.0 unx    12568 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/test_std_types.py
--rw-r--r--  2.0 unx    36831 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/test_create.py
--rw-r--r--  2.0 unx      264 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/__init__.py
--rw-r--r--  2.0 unx     3814 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/test_special_networks.py
--rw-r--r--  2.0 unx     4584 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/test_network_tables.py
--rw-r--r--  2.0 unx      721 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/test_time_series.py
--rw-r--r--  2.0 unx     2507 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/test_convert_format.py
--rw-r--r--  2.0 unx     2565 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/test_components/test_circ_pump_pressure.py
--rw-r--r--  2.0 unx     2469 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/test_components/test_circ_pump_mass.py
--rw-r--r--  2.0 unx     3152 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/test_components/test_valve.py
--rw-r--r--  2.0 unx     8218 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/test_components/test_pump.py
--rw-r--r--  2.0 unx     3188 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/test_components/test_compressor.py
--rw-r--r--  2.0 unx     1548 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/test_components/test_heat_exchanger.py
--rw-r--r--  2.0 unx     3615 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/test_components/test_flow_control.py
--rw-r--r--  2.0 unx     3898 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/test_components/test_pipe_results.py
--rw-r--r--  2.0 unx      264 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/test_components/__init__.py
--rw-r--r--  2.0 unx    18462 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/test_components/test_ext_grid.py
--rw-r--r--  2.0 unx     1099 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/test_components/test_mass_storage.py
--rw-r--r--  2.0 unx     2966 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/test_components/test_pressure_control.py
--rw-r--r--  2.0 unx      123 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/release_cycle/release_control_test_sink_profiles.csv
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/release_cycle/release_control_test_source_profiles.csv
--rw-r--r--  2.0 unx    31791 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.8.1_gas.json
--rw-r--r--  2.0 unx    23578 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.2.0.json
--rw-r--r--  2.0 unx    31791 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.8.4_gas.json
--rw-r--r--  2.0 unx    37279 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.8.2_water.json
--rw-r--r--  2.0 unx    37279 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.8.3_water.json
--rw-r--r--  2.0 unx    23570 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.1.2.json
--rw-r--r--  2.0 unx    31791 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.8.3_gas.json
--rw-r--r--  2.0 unx    31791 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.8.0_gas.json
--rw-r--r--  2.0 unx    37279 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.8.4_water.json
--rw-r--r--  2.0 unx    23456 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.1.1.json
--rw-r--r--  2.0 unx    37279 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.8.1_water.json
--rw-r--r--  2.0 unx    23456 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.1.0.json
--rw-r--r--  2.0 unx    23777 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.5.0.json
--rw-r--r--  2.0 unx    31791 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.8.2_gas.json
--rw-r--r--  2.0 unx    34898 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.7.0.json
--rw-r--r--  2.0 unx    37548 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.8.0_water.json
--rw-r--r--  2.0 unx    23709 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.4.0.json
--rw-r--r--  2.0 unx    24263 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.6.0.json
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/converter/stanet/
--rw-r--r--  2.0 unx      344 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/converter/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/converter/stanet/valve_pipe_component/
--rw-r--r--  2.0 unx     6108 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/converter/stanet/data_cleaning.py
--rw-r--r--  2.0 unx    21992 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/converter/stanet/preparing_steps.py
--rw-r--r--  2.0 unx     9988 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/converter/stanet/stanet2pandapipes.py
--rw-r--r--  2.0 unx      366 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/converter/stanet/__init__.py
--rw-r--r--  2.0 unx    56282 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/converter/stanet/table_creation.py
--rw-r--r--  2.0 unx     4068 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/converter/stanet/valve_pipe_component/valve_pipe_component.py
--rw-r--r--  2.0 unx     5066 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/converter/stanet/valve_pipe_component/valve_pipe_plotting.py
--rw-r--r--  2.0 unx      369 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/converter/stanet/valve_pipe_component/__init__.py
--rw-r--r--  2.0 unx     9385 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/converter/stanet/valve_pipe_component/create_valve_pipe.py
--rw-r--r--  2.0 unx     1690 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/control/run_control.py
--rw-r--r--  2.0 unx      320 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/control/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/
--rw-r--r--  2.0 unx    19224 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/simple_water_networks.py
--rw-r--r--  2.0 unx     3330 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/simple_heat_transfer_networks.py
--rw-r--r--  2.0 unx    10258 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/simple_gas_networks.py
--rw-r--r--  2.0 unx     2180 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/nw_aux.py
--rw-r--r--  2.0 unx      439 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/
--rw-r--r--  2.0 unx   909128 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/gas_net_schutterwald_1bar.json
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/combined_networks/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/t_cross/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/two_pressure_junctions/
--rw-r--r--  2.0 unx    57835 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/two_pumps.json
--rw-r--r--  2.0 unx    55322 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/two_pipes.json
--rw-r--r--  2.0 unx    56504 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/strand_net.json
--rw-r--r--  2.0 unx    56329 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/cross_3ext.json
--rw-r--r--  2.0 unx    64589 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/combined_networks/versatility.json
--rw-r--r--  2.0 unx    56599 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/combined_networks/mixed_net.json
--rw-r--r--  2.0 unx    55168 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_2.json
--rw-r--r--  2.0 unx    55223 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_3.json
--rw-r--r--  2.0 unx    55168 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_1.json
--rw-r--r--  2.0 unx    55598 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/t_cross/t_cross.json
--rw-r--r--  2.0 unx    56141 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/t_cross/valves.json
--rw-r--r--  2.0 unx    56034 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/delta.json
--rw-r--r--  2.0 unx    56878 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/pumps.json
--rw-r--r--  2.0 unx    56506 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/two_valves.json
--rw-r--r--  2.0 unx    55689 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/heights.json
--rw-r--r--  2.0 unx    55367 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/two_pressure_junctions/two_pipes.json
--rw-r--r--  2.0 unx    56131 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/delta.json
--rw-r--r--  2.0 unx    56240 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/t_cross.json
--rw-r--r--  2.0 unx    56166 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/delta_2sinks.json
--rw-r--r--  2.0 unx    56454 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/one_source.json
--rw-r--r--  2.0 unx    55467 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/one_pipe.json
--rw-r--r--  2.0 unx    55867 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/two_pipes.json
--rw-r--r--  2.0 unx    57799 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/section_variation.json
--rw-r--r--  2.0 unx    56990 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/heights.json
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/combined_networks/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/t_cross/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/two_pressure_junctions/
--rw-r--r--  2.0 unx    57684 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net_stanet_variation2.json
--rw-r--r--  2.0 unx    57834 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/two_pumps.json
--rw-r--r--  2.0 unx    55322 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/two_pipes.json
--rw-r--r--  2.0 unx    56504 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net.json
--rw-r--r--  2.0 unx    56328 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/cross_3ext.json
--rw-r--r--  2.0 unx    57679 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net_stanet_variation1.json
--rw-r--r--  2.0 unx    64589 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/combined_networks/versatility.json
--rw-r--r--  2.0 unx    56599 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/combined_networks/mixed_net.json
--rw-r--r--  2.0 unx    55168 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_2.json
--rw-r--r--  2.0 unx    55223 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_3.json
--rw-r--r--  2.0 unx    55168 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_1.json
--rw-r--r--  2.0 unx    55599 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/t_cross/t_cross.json
--rw-r--r--  2.0 unx    56138 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/t_cross/valves.json
--rw-r--r--  2.0 unx    56033 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/delta.json
--rw-r--r--  2.0 unx    57295 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/one_valve_stanet.json
--rw-r--r--  2.0 unx    56878 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/pumps.json
--rw-r--r--  2.0 unx    56508 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/two_valves.json
--rw-r--r--  2.0 unx    55688 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/heights.json
--rw-r--r--  2.0 unx    55365 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/two_pressure_junctions/two_pipes.json
--rw-r--r--  2.0 unx    54582 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/two_pressure_junctions/one_pipe_stanet.json
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/t_cross/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/two_pressure_junctions/
--rw-r--r--  2.0 unx    55950 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/two_pipes_PC.json
--rw-r--r--  2.0 unx    57824 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/strand_net_N.json
--rw-r--r--  2.0 unx    55950 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/two_pipes_N.json
--rw-r--r--  2.0 unx    57259 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/cross_PC.json
--rw-r--r--  2.0 unx    56917 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/pump_N.json
--rw-r--r--  2.0 unx    57823 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/strand_net_PC.json
--rw-r--r--  2.0 unx    61200 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/versatility_N.json
--rw-r--r--  2.0 unx    59829 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/district_N.json
--rw-r--r--  2.0 unx    61178 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/versatility_PC.json
--rw-r--r--  2.0 unx    59850 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/district_PC.json
--rw-r--r--  2.0 unx    55711 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_3_PC.json
--rw-r--r--  2.0 unx    55711 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_3_N.json
--rw-r--r--  2.0 unx    55710 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_1_PC.json
--rw-r--r--  2.0 unx    55729 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_2_PC.json
--rw-r--r--  2.0 unx    55729 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_2_N.json
--rw-r--r--  2.0 unx    55710 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_1_N.json
--rw-r--r--  2.0 unx    56252 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/t_cross/t_cross_N.json
--rw-r--r--  2.0 unx    56252 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/t_cross/t_cross_PC.json
--rw-r--r--  2.0 unx    56759 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/delta_N.json
--rw-r--r--  2.0 unx    58149 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/two_valves_PC.json
--rw-r--r--  2.0 unx    58148 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/two_valves_N.json
--rw-r--r--  2.0 unx    57075 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/pumps_N.json
--rw-r--r--  2.0 unx    56017 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/two_pressure_junctions/two_pipes_PC.json
--rw-r--r--  2.0 unx    56017 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/two_pressure_junctions/two_pipes_N.json
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/two_pressure_junctions/
--rw-r--r--  2.0 unx    56037 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/two_pipes_PC.json
--rw-r--r--  2.0 unx    56039 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/two_pipes_N.json
--rw-r--r--  2.0 unx    56989 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/pump_N.json
--rw-r--r--  2.0 unx    57070 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/parallel_PC.json
--rw-r--r--  2.0 unx    57068 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/parallel_N.json
--rw-r--r--  2.0 unx    61403 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/versatility_PC.json
--rw-r--r--  2.0 unx    55786 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_1_PC.json
--rw-r--r--  2.0 unx    55789 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_2_PC.json
--rw-r--r--  2.0 unx    55789 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_2_N.json
--rw-r--r--  2.0 unx    55786 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_1_N.json
--rw-r--r--  2.0 unx    56917 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross2_N.json
--rw-r--r--  2.0 unx    56327 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross1_PC.json
--rw-r--r--  2.0 unx    56917 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross2_PC.json
--rw-r--r--  2.0 unx    56349 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross1_N.json
--rw-r--r--  2.0 unx    56823 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/square_N.json
--rw-r--r--  2.0 unx    56826 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/square_PC.json
--rw-r--r--  2.0 unx    58261 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/two_valves_PC.json
--rw-r--r--  2.0 unx    58259 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/two_valves_N.json
--rw-r--r--  2.0 unx    56859 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/delta_PC.json
--rw-r--r--  2.0 unx    57188 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/pumps_N.json
--rw-r--r--  2.0 unx    56947 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/two_pressure_junctions/H_net_N.json
--rw-r--r--  2.0 unx    56961 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/two_pressure_junctions/H_net_PC.json
--rw-r--r--  2.0 unx    68396 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb4--0-no_sw.json
--rw-r--r--  2.0 unx    93171 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/1-LV-urban6--0-sw.json
--rw-r--r--  2.0 unx    60010 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural1--0-no_sw.json
--rw-r--r--  2.0 unx    83798 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural2--0-no_sw.json
--rw-r--r--  2.0 unx    64695 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural1--0-sw.json
--rw-r--r--  2.0 unx   114320 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural2--0-sw.json
--rw-r--r--  2.0 unx    93714 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural3--0-no_sw.json
--rw-r--r--  2.0 unx   122940 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb5--0-sw.json
--rw-r--r--  2.0 unx   135170 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural3--0-sw.json
--rw-r--r--  2.0 unx    87743 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb5--0-no_sw.json
--rw-r--r--  2.0 unx    74935 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/1-LV-urban6--0-no_sw.json
--rw-r--r--  2.0 unx    82067 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb4--0-sw.json
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/component_models/abstract_models/
--rw-r--r--  2.0 unx     4385 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/component_models/ext_grid_component.py
--rw-r--r--  2.0 unx     5428 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/component_models/flow_control_component.py
--rw-r--r--  2.0 unx     2416 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/component_models/compressor_component.py
--rw-r--r--  2.0 unx    16471 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/component_models/pipe_component.py
--rw-r--r--  2.0 unx     1665 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/component_models/mass_storage_component.py
--rw-r--r--  2.0 unx      740 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/component_models/source_component.py
--rw-r--r--  2.0 unx     5596 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/component_models/junction_component.py
--rw-r--r--  2.0 unx     2477 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/component_models/circulation_pump_mass_component.py
--rw-r--r--  2.0 unx     2110 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/component_models/circulation_pump_pressure_component.py
--rw-r--r--  2.0 unx     1156 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/component_models/__init__.py
--rw-r--r--  2.0 unx     6379 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/component_models/pressure_control_component.py
--rw-r--r--  2.0 unx     4857 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/component_models/heat_exchanger_component.py
--rw-r--r--  2.0 unx      735 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/component_models/sink_component.py
--rw-r--r--  2.0 unx     6978 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/component_models/component_toolbox.py
--rw-r--r--  2.0 unx     4518 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/component_models/valve_component.py
--rw-r--r--  2.0 unx     8689 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/component_models/pump_component.py
--rw-r--r--  2.0 unx     3707 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/component_models/abstract_models/branch_wo_internals_models.py
--rw-r--r--  2.0 unx     5808 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/component_models/abstract_models/branch_models.py
--rw-r--r--  2.0 unx     1976 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/component_models/abstract_models/branch_wzerolength_models.py
--rw-r--r--  2.0 unx     3722 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/component_models/abstract_models/const_flow_models.py
--rw-r--r--  2.0 unx     5300 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/component_models/abstract_models/base_component.py
--rw-r--r--  2.0 unx      575 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/component_models/abstract_models/__init__.py
--rw-r--r--  2.0 unx     5328 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/component_models/abstract_models/circulation_pump.py
--rw-r--r--  2.0 unx     1435 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/component_models/abstract_models/node_element_models.py
--rw-r--r--  2.0 unx     1949 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/component_models/abstract_models/node_models.py
--rw-r--r--  2.0 unx     8489 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/component_models/abstract_models/branch_w_internals_models.py
--rw-r--r--  2.0 unx     3255 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/topology/graph_searches.py
--rw-r--r--  2.0 unx      450 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/topology/__init__.py
--rw-r--r--  2.0 unx     9234 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/topology/create_graph.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/multinet/timeseries/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/multinet/control/
--rw-r--r--  2.0 unx     3295 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/multinet/multinet.py
--rw-r--r--  2.0 unx     2913 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/multinet/create_multinet.py
--rw-r--r--  2.0 unx      567 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/multinet/__init__.py
--rw-r--r--  2.0 unx      318 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/multinet/timeseries/__init__.py
--rw-r--r--  2.0 unx     6314 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/multinet/timeseries/run_time_series_multinet.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/multinet/control/controller/
--rw-r--r--  2.0 unx    13431 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/multinet/control/run_control_multinet.py
--rw-r--r--  2.0 unx      311 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/multinet/control/__init__.py
--rw-r--r--  2.0 unx    30354 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/multinet/control/controller/multinet_control.py
--rw-r--r--  2.0 unx      297 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/multinet/control/controller/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/carbondioxide/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/lgas/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/hydrogen/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/hgas/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/methane/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/ethane/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/water/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/air/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/nitrogen/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/oxygen/
--rw-r--r--  2.0 unx     5775 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/properties_toolbox.py
--rw-r--r--  2.0 unx      308 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/__init__.py
--rw-r--r--  2.0 unx    26389 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/fluids.py
--rw-r--r--  2.0 unx      103 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/carbondioxide/heat_capacity.txt
--rw-r--r--  2.0 unx        5 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/carbondioxide/molar_mass.txt
--rw-r--r--  2.0 unx      103 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/carbondioxide/viscosity.txt
--rw-r--r--  2.0 unx       79 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/carbondioxide/density.txt
--rw-r--r--  2.0 unx      241 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/lgas/heat_capacity.txt
--rw-r--r--  2.0 unx       21 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/lgas/molar_mass.txt
--rw-r--r--  2.0 unx       54 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/lgas/compressibility.txt
--rw-r--r--  2.0 unx      271 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/lgas/viscosity.txt
--rw-r--r--  2.0 unx       65 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/lgas/higher_heating_value.txt
--rw-r--r--  2.0 unx       64 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/lgas/lower_heating_value.txt
--rw-r--r--  2.0 unx      244 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/lgas/density.txt
--rw-r--r--  2.0 unx       47 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/lgas/der_compressibility.txt
--rw-r--r--  2.0 unx     1392 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/hydrogen/heat_capacity.txt
--rw-r--r--  2.0 unx       21 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/hydrogen/molar_mass.txt
--rw-r--r--  2.0 unx      384 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/hydrogen/compressibility.txt
--rw-r--r--  2.0 unx     1723 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/hydrogen/viscosity.txt
--rw-r--r--  2.0 unx       84 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/hydrogen/higher_heating_value.txt
--rw-r--r--  2.0 unx       83 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/hydrogen/lower_heating_value.txt
--rw-r--r--  2.0 unx     1552 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/hydrogen/density.txt
--rw-r--r--  2.0 unx      496 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/hydrogen/der_compressibility.txt
--rw-r--r--  2.0 unx      238 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/hgas/heat_capacity.txt
--rw-r--r--  2.0 unx       19 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/hgas/molar_mass.txt
--rw-r--r--  2.0 unx       54 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/hgas/compressibility.txt
--rw-r--r--  2.0 unx      267 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/hgas/viscosity.txt
--rw-r--r--  2.0 unx       65 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/hgas/higher_heating_value.txt
--rw-r--r--  2.0 unx       64 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/hgas/lower_heating_value.txt
--rw-r--r--  2.0 unx      243 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/hgas/density.txt
--rw-r--r--  2.0 unx       47 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/hgas/der_compressibility.txt
--rw-r--r--  2.0 unx      180 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/methane/heat_capacity.txt
--rw-r--r--  2.0 unx       15 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/methane/molar_mass.txt
--rw-r--r--  2.0 unx       54 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/methane/compressibility.txt
--rw-r--r--  2.0 unx      174 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/methane/viscosity.txt
--rw-r--r--  2.0 unx       65 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/methane/higher_heating_value.txt
--rw-r--r--  2.0 unx       64 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/methane/lower_heating_value.txt
--rw-r--r--  2.0 unx      175 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/methane/density.txt
--rw-r--r--  2.0 unx       47 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/methane/der_compressibility.txt
--rw-r--r--  2.0 unx      119 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/ethane/heat_capacity.txt
--rw-r--r--  2.0 unx        5 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/ethane/molar_mass.txt
--rw-r--r--  2.0 unx      116 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/ethane/viscosity.txt
--rw-r--r--  2.0 unx      105 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/ethane/density.txt
--rw-r--r--  2.0 unx      111 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/water/heat_capacity.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/water/molar_mass.txt
--rw-r--r--  2.0 unx        3 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/water/compressibility.txt
--rw-r--r--  2.0 unx      261 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/water/viscosity.txt
--rw-r--r--  2.0 unx      216 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/water/density.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/water/der_compressibility.txt
--rw-r--r--  2.0 unx      301 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/air/heat_capacity.txt
--rw-r--r--  2.0 unx        5 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/air/molar_mass.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/air/compressibility.txt
--rw-r--r--  2.0 unx      326 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/air/viscosity.txt
--rw-r--r--  2.0 unx      266 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/air/density.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/air/der_compressibility.txt
--rw-r--r--  2.0 unx     1456 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/nitrogen/heat_capacity.txt
--rw-r--r--  2.0 unx       35 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/nitrogen/molar_mass.txt
--rw-r--r--  2.0 unx     1629 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/nitrogen/viscosity.txt
--rw-r--r--  2.0 unx     1495 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/nitrogen/density.txt
--rw-r--r--  2.0 unx     1454 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/oxygen/heat_capacity.txt
--rw-r--r--  2.0 unx       38 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/oxygen/molar_mass.txt
--rw-r--r--  2.0 unx     1630 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/oxygen/viscosity.txt
--rw-r--r--  2.0 unx     1552 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/properties/oxygen/density.txt
--rw-r--r--  2.0 unx    19547 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/plotting/simple_plot.py
--rw-r--r--  2.0 unx     4888 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/plotting/generic_geodata.py
--rw-r--r--  2.0 unx     2753 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/plotting/geo.py
--rw-r--r--  2.0 unx     1391 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/plotting/pipeflow_results.py
--rw-r--r--  2.0 unx     1026 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/plotting/__init__.py
--rw-r--r--  2.0 unx    10253 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/plotting/patch_makers.py
--rw-r--r--  2.0 unx     2503 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/plotting/plotting_toolbox.py
--rw-r--r--  2.0 unx    31552 b- defN 23-Feb-02 15:59 pandapipes-0.8.4/pandapipes/plotting/collections.py
-470 files, 11559185 bytes uncompressed, 1332886 bytes compressed:  88.5%
+Zip file size: 1450360 bytes, number of entries: 472
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/.github/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes.egg-info/
+-rw-r--r--  2.0 unx      109 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/setup.cfg
+-rw-r--r--  2.0 unx     3036 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/README.rst
+-rw-r--r--  2.0 unx    16876 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/PKG-INFO
+-rw-r--r--  2.0 unx      159 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/MANIFEST.in
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/LICENSE
+-rw-r--r--  2.0 unx      618 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/AUTHORS
+-rw-r--r--  2.0 unx     2338 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/setup.py
+-rw-r--r--  2.0 unx    12702 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/CHANGELOG.rst
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/.github/workflows/
+-rw-r--r--  2.0 unx     4700 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/.github/workflows/run_tests_develop.yml
+-rw-r--r--  2.0 unx     3315 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/.github/workflows/release.yml
+-rw-r--r--  2.0 unx     3404 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/.github/workflows/run_tests_master.yml
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/control/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/timeseries/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/multinet/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/converter/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/io/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/pf/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/topology/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/plotting/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/std_types/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/
+-rw-r--r--  2.0 unx    87241 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/create.py
+-rw-r--r--  2.0 unx    28258 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/toolbox.py
+-rw-r--r--  2.0 unx    15103 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/pipeflow.py
+-rw-r--r--  2.0 unx      928 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/idx_node.py
+-rw-r--r--  2.0 unx     3231 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/pandapipes_net.py
+-rw-r--r--  2.0 unx      745 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/__init__.py
+-rw-r--r--  2.0 unx     1894 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/idx_branch.py
+-rw-r--r--  2.0 unx     1011 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/constants.py
+-rw-r--r--  2.0 unx     1690 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/control/run_control.py
+-rw-r--r--  2.0 unx      320 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/control/__init__.py
+-rw-r--r--  2.0 unx      406 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/timeseries/__init__.py
+-rw-r--r--  2.0 unx     5243 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/timeseries/run_time_series.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/abstract_models/
+-rw-r--r--  2.0 unx     2477 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/circulation_pump_mass_component.py
+-rw-r--r--  2.0 unx     6379 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/pressure_control_component.py
+-rw-r--r--  2.0 unx     4518 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/valve_component.py
+-rw-r--r--  2.0 unx     4857 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/heat_exchanger_component.py
+-rw-r--r--  2.0 unx      740 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/source_component.py
+-rw-r--r--  2.0 unx     8723 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/pump_component.py
+-rw-r--r--  2.0 unx     4385 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/ext_grid_component.py
+-rw-r--r--  2.0 unx     5596 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/junction_component.py
+-rw-r--r--  2.0 unx     6978 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/component_toolbox.py
+-rw-r--r--  2.0 unx    16471 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/pipe_component.py
+-rw-r--r--  2.0 unx     1665 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/mass_storage_component.py
+-rw-r--r--  2.0 unx     5428 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/flow_control_component.py
+-rw-r--r--  2.0 unx     2110 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/circulation_pump_pressure_component.py
+-rw-r--r--  2.0 unx     1156 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/__init__.py
+-rw-r--r--  2.0 unx      735 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/sink_component.py
+-rw-r--r--  2.0 unx     2416 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/compressor_component.py
+-rw-r--r--  2.0 unx     5300 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/abstract_models/base_component.py
+-rw-r--r--  2.0 unx     5808 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/abstract_models/branch_models.py
+-rw-r--r--  2.0 unx     1976 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/abstract_models/branch_wzerolength_models.py
+-rw-r--r--  2.0 unx     1949 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/abstract_models/node_models.py
+-rw-r--r--  2.0 unx     3707 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/abstract_models/branch_wo_internals_models.py
+-rw-r--r--  2.0 unx     8489 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/abstract_models/branch_w_internals_models.py
+-rw-r--r--  2.0 unx     5328 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/abstract_models/circulation_pump.py
+-rw-r--r--  2.0 unx     3722 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/abstract_models/const_flow_models.py
+-rw-r--r--  2.0 unx      575 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/abstract_models/__init__.py
+-rw-r--r--  2.0 unx     1435 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/abstract_models/node_element_models.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/multinet/control/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/multinet/timeseries/
+-rw-r--r--  2.0 unx     3295 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/multinet/multinet.py
+-rw-r--r--  2.0 unx      567 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/multinet/__init__.py
+-rw-r--r--  2.0 unx     2913 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/multinet/create_multinet.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/multinet/control/controller/
+-rw-r--r--  2.0 unx      311 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/multinet/control/__init__.py
+-rw-r--r--  2.0 unx    13431 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/multinet/control/run_control_multinet.py
+-rw-r--r--  2.0 unx    30354 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/multinet/control/controller/multinet_control.py
+-rw-r--r--  2.0 unx      297 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/multinet/control/controller/__init__.py
+-rw-r--r--  2.0 unx     6314 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/multinet/timeseries/run_time_series_multinet.py
+-rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/multinet/timeseries/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/converter/stanet/
+-rw-r--r--  2.0 unx      344 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/converter/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/converter/stanet/valve_pipe_component/
+-rw-r--r--  2.0 unx     6108 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/converter/stanet/data_cleaning.py
+-rw-r--r--  2.0 unx     9988 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/converter/stanet/stanet2pandapipes.py
+-rw-r--r--  2.0 unx      366 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/converter/stanet/__init__.py
+-rw-r--r--  2.0 unx    21992 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/converter/stanet/preparing_steps.py
+-rw-r--r--  2.0 unx    56282 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/converter/stanet/table_creation.py
+-rw-r--r--  2.0 unx     4068 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/converter/stanet/valve_pipe_component/valve_pipe_component.py
+-rw-r--r--  2.0 unx     5066 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/converter/stanet/valve_pipe_component/valve_pipe_plotting.py
+-rw-r--r--  2.0 unx     9385 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/converter/stanet/valve_pipe_component/create_valve_pipe.py
+-rw-r--r--  2.0 unx      369 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/converter/stanet/valve_pipe_component/__init__.py
+-rw-r--r--  2.0 unx     6384 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/io/file_io.py
+-rw-r--r--  2.0 unx     3069 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/io/convert_format.py
+-rw-r--r--  2.0 unx     4881 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/io/io_utils.py
+-rw-r--r--  2.0 unx      312 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/io/__init__.py
+-rw-r--r--  2.0 unx     6682 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/pf/derivative_toolbox.py
+-rw-r--r--  2.0 unx    12526 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/pf/result_extraction.py
+-rw-r--r--  2.0 unx     8666 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/pf/derivative_toolbox_numba.py
+-rw-r--r--  2.0 unx    29751 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/pf/pipeflow_setup.py
+-rw-r--r--  2.0 unx      403 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/pf/__init__.py
+-rw-r--r--  2.0 unx     5374 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/pf/internals_toolbox.py
+-rw-r--r--  2.0 unx     8103 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/pf/derivative_calculation.py
+-rw-r--r--  2.0 unx     8985 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/pf/build_system_matrix.py
+-rw-r--r--  2.0 unx     3255 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/topology/graph_searches.py
+-rw-r--r--  2.0 unx      450 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/topology/__init__.py
+-rw-r--r--  2.0 unx     9234 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/topology/create_graph.py
+-rw-r--r--  2.0 unx     1391 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/plotting/pipeflow_results.py
+-rw-r--r--  2.0 unx     2753 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/plotting/geo.py
+-rw-r--r--  2.0 unx     4867 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/plotting/generic_geodata.py
+-rw-r--r--  2.0 unx    19547 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/plotting/simple_plot.py
+-rw-r--r--  2.0 unx    10253 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/plotting/patch_makers.py
+-rw-r--r--  2.0 unx    31552 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/plotting/collections.py
+-rw-r--r--  2.0 unx     1026 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/plotting/__init__.py
+-rw-r--r--  2.0 unx     2503 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/plotting/plotting_toolbox.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/methane/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/carbondioxide/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/lgas/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/ethane/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/air/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/water/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/nitrogen/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/hgas/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/oxygen/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/hydrogen/
+-rw-r--r--  2.0 unx     5775 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/properties_toolbox.py
+-rw-r--r--  2.0 unx      308 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/__init__.py
+-rw-r--r--  2.0 unx    26389 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/fluids.py
+-rw-r--r--  2.0 unx       65 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/methane/higher_heating_value.txt
+-rw-r--r--  2.0 unx       54 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/methane/compressibility.txt
+-rw-r--r--  2.0 unx       15 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/methane/molar_mass.txt
+-rw-r--r--  2.0 unx      175 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/methane/density.txt
+-rw-r--r--  2.0 unx      180 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/methane/heat_capacity.txt
+-rw-r--r--  2.0 unx       47 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/methane/der_compressibility.txt
+-rw-r--r--  2.0 unx      174 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/methane/viscosity.txt
+-rw-r--r--  2.0 unx       64 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/methane/lower_heating_value.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/carbondioxide/molar_mass.txt
+-rw-r--r--  2.0 unx       79 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/carbondioxide/density.txt
+-rw-r--r--  2.0 unx      103 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/carbondioxide/heat_capacity.txt
+-rw-r--r--  2.0 unx      103 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/carbondioxide/viscosity.txt
+-rw-r--r--  2.0 unx       65 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/lgas/higher_heating_value.txt
+-rw-r--r--  2.0 unx       54 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/lgas/compressibility.txt
+-rw-r--r--  2.0 unx       21 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/lgas/molar_mass.txt
+-rw-r--r--  2.0 unx      244 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/lgas/density.txt
+-rw-r--r--  2.0 unx      241 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/lgas/heat_capacity.txt
+-rw-r--r--  2.0 unx       47 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/lgas/der_compressibility.txt
+-rw-r--r--  2.0 unx      271 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/lgas/viscosity.txt
+-rw-r--r--  2.0 unx       64 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/lgas/lower_heating_value.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/ethane/molar_mass.txt
+-rw-r--r--  2.0 unx      105 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/ethane/density.txt
+-rw-r--r--  2.0 unx      119 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/ethane/heat_capacity.txt
+-rw-r--r--  2.0 unx      116 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/ethane/viscosity.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/air/compressibility.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/air/molar_mass.txt
+-rw-r--r--  2.0 unx      266 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/air/density.txt
+-rw-r--r--  2.0 unx      301 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/air/heat_capacity.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/air/der_compressibility.txt
+-rw-r--r--  2.0 unx      326 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/air/viscosity.txt
+-rw-r--r--  2.0 unx        3 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/water/compressibility.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/water/molar_mass.txt
+-rw-r--r--  2.0 unx      216 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/water/density.txt
+-rw-r--r--  2.0 unx      111 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/water/heat_capacity.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/water/der_compressibility.txt
+-rw-r--r--  2.0 unx      261 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/water/viscosity.txt
+-rw-r--r--  2.0 unx       35 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/nitrogen/molar_mass.txt
+-rw-r--r--  2.0 unx     1495 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/nitrogen/density.txt
+-rw-r--r--  2.0 unx     1456 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/nitrogen/heat_capacity.txt
+-rw-r--r--  2.0 unx     1629 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/nitrogen/viscosity.txt
+-rw-r--r--  2.0 unx       65 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/hgas/higher_heating_value.txt
+-rw-r--r--  2.0 unx       54 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/hgas/compressibility.txt
+-rw-r--r--  2.0 unx       19 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/hgas/molar_mass.txt
+-rw-r--r--  2.0 unx      243 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/hgas/density.txt
+-rw-r--r--  2.0 unx      238 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/hgas/heat_capacity.txt
+-rw-r--r--  2.0 unx       47 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/hgas/der_compressibility.txt
+-rw-r--r--  2.0 unx      267 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/hgas/viscosity.txt
+-rw-r--r--  2.0 unx       64 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/hgas/lower_heating_value.txt
+-rw-r--r--  2.0 unx       38 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/oxygen/molar_mass.txt
+-rw-r--r--  2.0 unx     1552 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/oxygen/density.txt
+-rw-r--r--  2.0 unx     1454 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/oxygen/heat_capacity.txt
+-rw-r--r--  2.0 unx     1630 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/oxygen/viscosity.txt
+-rw-r--r--  2.0 unx       84 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/hydrogen/higher_heating_value.txt
+-rw-r--r--  2.0 unx      384 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/hydrogen/compressibility.txt
+-rw-r--r--  2.0 unx       21 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/hydrogen/molar_mass.txt
+-rw-r--r--  2.0 unx     1552 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/hydrogen/density.txt
+-rw-r--r--  2.0 unx     1392 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/hydrogen/heat_capacity.txt
+-rw-r--r--  2.0 unx      496 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/hydrogen/der_compressibility.txt
+-rw-r--r--  2.0 unx     1723 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/hydrogen/viscosity.txt
+-rw-r--r--  2.0 unx       83 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/hydrogen/lower_heating_value.txt
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/std_types/library/
+-rw-r--r--  2.0 unx     8846 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/std_types/std_types.py
+-rw-r--r--  2.0 unx    10196 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/std_types/std_type_class.py
+-rw-r--r--  2.0 unx      360 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/std_types/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/std_types/library/Pump/
+-rw-r--r--  2.0 unx     8971 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/std_types/library/Pipe.csv
+-rw-r--r--  2.0 unx       51 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/std_types/library/Pump/P3.csv
+-rw-r--r--  2.0 unx       45 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/std_types/library/Pump/P1.csv
+-rw-r--r--  2.0 unx       58 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/std_types/library/Pump/P2.csv
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/multinet/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/converter/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/io/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/openmodelica_comparison/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/plotting/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/properties/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/stanet_comparison/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/networks/
+-rw-r--r--  2.0 unx      744 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/test_imports.py
+-rw-r--r--  2.0 unx     4258 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/run_tests.py
+-rw-r--r--  2.0 unx    14678 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/test_toolbox.py
+-rw-r--r--  2.0 unx      541 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/
+-rw-r--r--  2.0 unx     3987 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_pipeflow_modes.py
+-rw-r--r--  2.0 unx    24386 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_inservice.py
+-rw-r--r--  2.0 unx    15454 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_pipeflow_analytic_comparison.py
+-rw-r--r--  2.0 unx     2493 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_options.py
+-rw-r--r--  2.0 unx     1416 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_non_convergence.py
+-rw-r--r--  2.0 unx      346 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/__init__.py
+-rw-r--r--  2.0 unx     1271 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_update_matrix.py
+-rw-r--r--  2.0 unx     7253 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_time_series.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/
+-rw-r--r--  2.0 unx      325 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/Temperature_2zu_2ab_an.csv
+-rw-r--r--  2.0 unx       22 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/hydraulics.csv
+-rw-r--r--  2.0 unx      152 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_valve.csv
+-rw-r--r--  2.0 unx      196 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/Temperature_tee_2ab_1zu_an.csv
+-rw-r--r--  2.0 unx       71 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_pump.csv
+-rw-r--r--  2.0 unx      332 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/Temperature_masche_1load_an.csv
+-rw-r--r--  2.0 unx     3427 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_sink_profiles.csv
+-rw-r--r--  2.0 unx      300 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/Temperature_one_pipe_an.csv
+-rw-r--r--  2.0 unx     1178 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_source_profiles.csv
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/ext_grid_p.csv
+-rw-r--r--  2.0 unx       57 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_pressure_control.csv
+-rw-r--r--  2.0 unx      266 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/Temperature_masche_1load_direction_an.csv
+-rw-r--r--  2.0 unx      182 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/Temperature_tee_2zu_1ab_an.csv
+-rw-r--r--  2.0 unx     1893 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/gas_sections_an.csv
+-rw-r--r--  2.0 unx      133 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_circ_pump_pressure.csv
+-rw-r--r--  2.0 unx      127 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_circ_pump_mass.csv
+-rw-r--r--  2.0 unx       93 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/heat_exchanger_test.csv
+-rw-r--r--  2.0 unx       56 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/pressure_control_test_analytical.csv
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_sink/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_source/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_ext_grid/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_junction/
+-rw-r--r--  2.0 unx     3431 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_sink/mdot_kg_per_s.csv
+-rw-r--r--  2.0 unx     1181 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_source/mdot_kg_per_s.csv
+-rw-r--r--  2.0 unx     1171 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_ext_grid/mdot_kg_per_s.csv
+-rw-r--r--  2.0 unx     5381 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/v_mean_m_per_s.csv
+-rw-r--r--  2.0 unx     5944 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/lambda.csv
+-rw-r--r--  2.0 unx     5737 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/reynolds.csv
+-rw-r--r--  2.0 unx     4901 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_junction/p_bar.csv
+-rw-r--r--  2.0 unx     6176 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/multinet/test_time_series_multinet.py
+-rw-r--r--  2.0 unx    16572 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/multinet/test_control_multinet.py
+-rw-r--r--  2.0 unx      238 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/multinet/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/converter/converter_test_files/
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/converter/__init__.py
+-rw-r--r--  2.0 unx     3518 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/converter/test_stanet_converter.py
+-rw-r--r--  2.0 unx   592867 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_2valvepipe.csv
+-rw-r--r--  2.0 unx   899403 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/converter/converter_test_files/Exampelonia_mini.csv
+-rw-r--r--  2.0 unx   618341 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_valve_2sliders_closed.csv
+-rw-r--r--  2.0 unx   618340 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_valve_2sliders_open.csv
+-rw-r--r--  2.0 unx      264 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/io/__init__.py
+-rw-r--r--  2.0 unx     6422 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/io/test_file_io.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_components/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/release_cycle/
+-rw-r--r--  2.0 unx      688 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_aux_function.py
+-rw-r--r--  2.0 unx     3814 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_special_networks.py
+-rw-r--r--  2.0 unx    36831 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_create.py
+-rw-r--r--  2.0 unx    12568 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_std_types.py
+-rw-r--r--  2.0 unx     2507 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_convert_format.py
+-rw-r--r--  2.0 unx      264 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/__init__.py
+-rw-r--r--  2.0 unx     4584 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_network_tables.py
+-rw-r--r--  2.0 unx      721 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_time_series.py
+-rw-r--r--  2.0 unx    18462 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_components/test_ext_grid.py
+-rw-r--r--  2.0 unx     1548 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_components/test_heat_exchanger.py
+-rw-r--r--  2.0 unx     3152 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_components/test_valve.py
+-rw-r--r--  2.0 unx     3615 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_components/test_flow_control.py
+-rw-r--r--  2.0 unx    10376 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_components/test_pump.py
+-rw-r--r--  2.0 unx     2966 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_components/test_pressure_control.py
+-rw-r--r--  2.0 unx     3188 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_components/test_compressor.py
+-rw-r--r--  2.0 unx     3898 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_components/test_pipe_results.py
+-rw-r--r--  2.0 unx      264 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_components/__init__.py
+-rw-r--r--  2.0 unx     1099 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_components/test_mass_storage.py
+-rw-r--r--  2.0 unx     2469 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_components/test_circ_pump_mass.py
+-rw-r--r--  2.0 unx     2565 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_components/test_circ_pump_pressure.py
+-rw-r--r--  2.0 unx    23456 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.1.1.json
+-rw-r--r--  2.0 unx    37279 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.5_water.json
+-rw-r--r--  2.0 unx    23709 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.4.0.json
+-rw-r--r--  2.0 unx    37279 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.3_water.json
+-rw-r--r--  2.0 unx    34898 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.7.0.json
+-rw-r--r--  2.0 unx    37279 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.2_water.json
+-rw-r--r--  2.0 unx    31791 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.4_gas.json
+-rw-r--r--  2.0 unx    31791 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.3_gas.json
+-rw-r--r--  2.0 unx    24263 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.6.0.json
+-rw-r--r--  2.0 unx    31791 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.5_gas.json
+-rw-r--r--  2.0 unx    31791 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.1_gas.json
+-rw-r--r--  2.0 unx    31791 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.0_gas.json
+-rw-r--r--  2.0 unx    37279 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.1_water.json
+-rw-r--r--  2.0 unx    37279 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.4_water.json
+-rw-r--r--  2.0 unx    23570 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.1.2.json
+-rw-r--r--  2.0 unx    23456 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.1.0.json
+-rw-r--r--  2.0 unx    31791 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.2_gas.json
+-rw-r--r--  2.0 unx    23777 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.5.0.json
+-rw-r--r--  2.0 unx    23578 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.2.0.json
+-rw-r--r--  2.0 unx    37548 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.0_water.json
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/release_cycle/release_control_test_source_profiles.csv
+-rw-r--r--  2.0 unx      123 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/release_cycle/release_control_test_sink_profiles.csv
+-rw-r--r--  2.0 unx    12229 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/openmodelica_comparison/test_water_openmodelica.py
+-rw-r--r--  2.0 unx    11348 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/openmodelica_comparison/pipeflow_openmodelica_comparison.py
+-rw-r--r--  2.0 unx     4103 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/openmodelica_comparison/test_heat_transfer_openmodelica.py
+-rw-r--r--  2.0 unx      264 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/openmodelica_comparison/__init__.py
+-rw-r--r--  2.0 unx     7984 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/plotting/test_simple_collections.py
+-rw-r--r--  2.0 unx     1460 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/plotting/test_generic_coordinates.py
+-rw-r--r--  2.0 unx     1987 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/plotting/test_pipeflow_results.py
+-rw-r--r--  2.0 unx      264 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/plotting/__init__.py
+-rw-r--r--  2.0 unx     9471 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/plotting/test_collections.py
+-rw-r--r--  2.0 unx     2564 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/properties/test_fluid_specials.py
+-rw-r--r--  2.0 unx    19769 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/properties/test_properties_toolbox.py
+-rw-r--r--  2.0 unx      264 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/properties/__init__.py
+-rw-r--r--  2.0 unx    11373 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/stanet_comparison/test_water_stanet.py
+-rw-r--r--  2.0 unx    11177 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/stanet_comparison/test_gas_stanet.py
+-rw-r--r--  2.0 unx     6912 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/stanet_comparison/pipeflow_stanet_comparison.py
+-rw-r--r--  2.0 unx      264 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/stanet_comparison/__init__.py
+-rw-r--r--  2.0 unx      983 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/networks/test_networks.py
+-rw-r--r--  2.0 unx      264 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/networks/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/
+-rw-r--r--  2.0 unx     2180 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/nw_aux.py
+-rw-r--r--  2.0 unx    19224 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/simple_water_networks.py
+-rw-r--r--  2.0 unx     3330 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/simple_heat_transfer_networks.py
+-rw-r--r--  2.0 unx      439 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/__init__.py
+-rw-r--r--  2.0 unx    10258 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/simple_gas_networks.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/
+-rw-r--r--  2.0 unx   909128 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/gas_net_schutterwald_1bar.json
+-rw-r--r--  2.0 unx    82067 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb4--0-sw.json
+-rw-r--r--  2.0 unx    60010 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural1--0-no_sw.json
+-rw-r--r--  2.0 unx   122940 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb5--0-sw.json
+-rw-r--r--  2.0 unx    87743 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb5--0-no_sw.json
+-rw-r--r--  2.0 unx   114320 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural2--0-sw.json
+-rw-r--r--  2.0 unx    74935 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-urban6--0-no_sw.json
+-rw-r--r--  2.0 unx    93171 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-urban6--0-sw.json
+-rw-r--r--  2.0 unx   135170 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural3--0-sw.json
+-rw-r--r--  2.0 unx    83798 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural2--0-no_sw.json
+-rw-r--r--  2.0 unx    64695 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural1--0-sw.json
+-rw-r--r--  2.0 unx    68396 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb4--0-no_sw.json
+-rw-r--r--  2.0 unx    93714 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural3--0-no_sw.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/two_pressure_junctions/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/
+-rw-r--r--  2.0 unx    56039 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/two_pipes_N.json
+-rw-r--r--  2.0 unx    56037 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/two_pipes_PC.json
+-rw-r--r--  2.0 unx    56989 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/pump_N.json
+-rw-r--r--  2.0 unx    57068 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/parallel_N.json
+-rw-r--r--  2.0 unx    57070 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/parallel_PC.json
+-rw-r--r--  2.0 unx    61403 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/versatility_PC.json
+-rw-r--r--  2.0 unx    56349 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross1_N.json
+-rw-r--r--  2.0 unx    56917 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross2_PC.json
+-rw-r--r--  2.0 unx    56917 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross2_N.json
+-rw-r--r--  2.0 unx    56327 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross1_PC.json
+-rw-r--r--  2.0 unx    58261 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/two_valves_PC.json
+-rw-r--r--  2.0 unx    56823 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/square_N.json
+-rw-r--r--  2.0 unx    58259 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/two_valves_N.json
+-rw-r--r--  2.0 unx    56859 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/delta_PC.json
+-rw-r--r--  2.0 unx    57188 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/pumps_N.json
+-rw-r--r--  2.0 unx    56826 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/square_PC.json
+-rw-r--r--  2.0 unx    56961 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/two_pressure_junctions/H_net_PC.json
+-rw-r--r--  2.0 unx    56947 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/two_pressure_junctions/H_net_N.json
+-rw-r--r--  2.0 unx    55786 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_1_N.json
+-rw-r--r--  2.0 unx    55789 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_2_N.json
+-rw-r--r--  2.0 unx    55786 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_1_PC.json
+-rw-r--r--  2.0 unx    55789 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_2_PC.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/t_cross/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/two_pressure_junctions/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/
+-rw-r--r--  2.0 unx    55950 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/two_pipes_N.json
+-rw-r--r--  2.0 unx    55950 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/two_pipes_PC.json
+-rw-r--r--  2.0 unx    56917 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/pump_N.json
+-rw-r--r--  2.0 unx    57824 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/strand_net_N.json
+-rw-r--r--  2.0 unx    57259 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/cross_PC.json
+-rw-r--r--  2.0 unx    57823 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/strand_net_PC.json
+-rw-r--r--  2.0 unx    61200 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/versatility_N.json
+-rw-r--r--  2.0 unx    59850 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/district_PC.json
+-rw-r--r--  2.0 unx    61178 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/versatility_PC.json
+-rw-r--r--  2.0 unx    59829 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/district_N.json
+-rw-r--r--  2.0 unx    56252 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/t_cross/t_cross_N.json
+-rw-r--r--  2.0 unx    56252 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/t_cross/t_cross_PC.json
+-rw-r--r--  2.0 unx    58149 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/two_valves_PC.json
+-rw-r--r--  2.0 unx    58148 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/two_valves_N.json
+-rw-r--r--  2.0 unx    56759 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/delta_N.json
+-rw-r--r--  2.0 unx    57075 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/pumps_N.json
+-rw-r--r--  2.0 unx    56017 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/two_pressure_junctions/two_pipes_N.json
+-rw-r--r--  2.0 unx    56017 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/two_pressure_junctions/two_pipes_PC.json
+-rw-r--r--  2.0 unx    55710 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_1_N.json
+-rw-r--r--  2.0 unx    55729 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_2_N.json
+-rw-r--r--  2.0 unx    55711 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_3_N.json
+-rw-r--r--  2.0 unx    55710 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_1_PC.json
+-rw-r--r--  2.0 unx    55711 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_3_PC.json
+-rw-r--r--  2.0 unx    55729 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_2_PC.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/
+-rw-r--r--  2.0 unx    56240 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/t_cross.json
+-rw-r--r--  2.0 unx    56990 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/heights.json
+-rw-r--r--  2.0 unx    55467 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/one_pipe.json
+-rw-r--r--  2.0 unx    56454 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/one_source.json
+-rw-r--r--  2.0 unx    56166 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/delta_2sinks.json
+-rw-r--r--  2.0 unx    56131 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/delta.json
+-rw-r--r--  2.0 unx    55867 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/two_pipes.json
+-rw-r--r--  2.0 unx    57799 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/section_variation.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/combined_networks/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/t_cross/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/two_pressure_junctions/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/
+-rw-r--r--  2.0 unx    57835 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/two_pumps.json
+-rw-r--r--  2.0 unx    56504 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/strand_net.json
+-rw-r--r--  2.0 unx    56329 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/cross_3ext.json
+-rw-r--r--  2.0 unx    55322 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/two_pipes.json
+-rw-r--r--  2.0 unx    64589 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/combined_networks/versatility.json
+-rw-r--r--  2.0 unx    56599 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/combined_networks/mixed_net.json
+-rw-r--r--  2.0 unx    55598 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/t_cross/t_cross.json
+-rw-r--r--  2.0 unx    56141 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/t_cross/valves.json
+-rw-r--r--  2.0 unx    55689 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/heights.json
+-rw-r--r--  2.0 unx    56878 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/pumps.json
+-rw-r--r--  2.0 unx    56034 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/delta.json
+-rw-r--r--  2.0 unx    56506 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/two_valves.json
+-rw-r--r--  2.0 unx    55367 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/two_pressure_junctions/two_pipes.json
+-rw-r--r--  2.0 unx    55223 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_3.json
+-rw-r--r--  2.0 unx    55168 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_1.json
+-rw-r--r--  2.0 unx    55168 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_2.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/combined_networks/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/t_cross/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/two_pressure_junctions/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/
+-rw-r--r--  2.0 unx    57679 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net_stanet_variation1.json
+-rw-r--r--  2.0 unx    57834 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/two_pumps.json
+-rw-r--r--  2.0 unx    56504 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net.json
+-rw-r--r--  2.0 unx    56328 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/cross_3ext.json
+-rw-r--r--  2.0 unx    57684 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net_stanet_variation2.json
+-rw-r--r--  2.0 unx    55322 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/two_pipes.json
+-rw-r--r--  2.0 unx    64589 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/combined_networks/versatility.json
+-rw-r--r--  2.0 unx    56599 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/combined_networks/mixed_net.json
+-rw-r--r--  2.0 unx    55599 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/t_cross/t_cross.json
+-rw-r--r--  2.0 unx    56138 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/t_cross/valves.json
+-rw-r--r--  2.0 unx    55688 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/heights.json
+-rw-r--r--  2.0 unx    57295 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/one_valve_stanet.json
+-rw-r--r--  2.0 unx    56878 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/pumps.json
+-rw-r--r--  2.0 unx    56033 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/delta.json
+-rw-r--r--  2.0 unx    56508 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/two_valves.json
+-rw-r--r--  2.0 unx    54582 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/two_pressure_junctions/one_pipe_stanet.json
+-rw-r--r--  2.0 unx    55365 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/two_pressure_junctions/two_pipes.json
+-rw-r--r--  2.0 unx    55223 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_3.json
+-rw-r--r--  2.0 unx    55168 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_1.json
+-rw-r--r--  2.0 unx    55168 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_2.json
+-rw-r--r--  2.0 unx    16876 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes.egg-info/top_level.txt
+-rw-r--r--  2.0 unx    23750 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx      263 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes.egg-info/requires.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes.egg-info/dependency_links.txt
+472 files, 11631818 bytes uncompressed, 1342604 bytes compressed:  88.5%
```

## zipnote {}

```diff
@@ -1,1411 +1,1417 @@
-Filename: pandapipes-0.8.4/
+Filename: pandapipes-0.8.5/
 Comment: 
 
-Filename: pandapipes-0.8.4/.github/
+Filename: pandapipes-0.8.5/.github/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes.egg-info/
+Filename: pandapipes-0.8.5/pandapipes/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/
+Filename: pandapipes-0.8.5/pandapipes.egg-info/
 Comment: 
 
-Filename: pandapipes-0.8.4/PKG-INFO
+Filename: pandapipes-0.8.5/setup.cfg
 Comment: 
 
-Filename: pandapipes-0.8.4/CHANGELOG.rst
+Filename: pandapipes-0.8.5/README.rst
 Comment: 
 
-Filename: pandapipes-0.8.4/AUTHORS
+Filename: pandapipes-0.8.5/PKG-INFO
 Comment: 
 
-Filename: pandapipes-0.8.4/setup.py
+Filename: pandapipes-0.8.5/MANIFEST.in
 Comment: 
 
-Filename: pandapipes-0.8.4/setup.cfg
+Filename: pandapipes-0.8.5/LICENSE
 Comment: 
 
-Filename: pandapipes-0.8.4/README.rst
+Filename: pandapipes-0.8.5/AUTHORS
 Comment: 
 
-Filename: pandapipes-0.8.4/MANIFEST.in
+Filename: pandapipes-0.8.5/setup.py
 Comment: 
 
-Filename: pandapipes-0.8.4/LICENSE
+Filename: pandapipes-0.8.5/CHANGELOG.rst
 Comment: 
 
-Filename: pandapipes-0.8.4/.github/workflows/
+Filename: pandapipes-0.8.5/.github/workflows/
 Comment: 
 
-Filename: pandapipes-0.8.4/.github/workflows/release.yml
+Filename: pandapipes-0.8.5/.github/workflows/run_tests_develop.yml
 Comment: 
 
-Filename: pandapipes-0.8.4/.github/workflows/run_tests_develop.yml
+Filename: pandapipes-0.8.5/.github/workflows/release.yml
 Comment: 
 
-Filename: pandapipes-0.8.4/.github/workflows/run_tests_master.yml
+Filename: pandapipes-0.8.5/.github/workflows/run_tests_master.yml
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes.egg-info/PKG-INFO
+Filename: pandapipes-0.8.5/pandapipes/control/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes.egg-info/SOURCES.txt
+Filename: pandapipes-0.8.5/pandapipes/timeseries/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes.egg-info/top_level.txt
+Filename: pandapipes-0.8.5/pandapipes/component_models/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes.egg-info/requires.txt
+Filename: pandapipes-0.8.5/pandapipes/multinet/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes.egg-info/dependency_links.txt
+Filename: pandapipes-0.8.5/pandapipes/converter/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/timeseries/
+Filename: pandapipes-0.8.5/pandapipes/io/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/std_types/
+Filename: pandapipes-0.8.5/pandapipes/pf/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/pf/
+Filename: pandapipes-0.8.5/pandapipes/topology/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/io/
+Filename: pandapipes-0.8.5/pandapipes/plotting/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/
+Filename: pandapipes-0.8.5/pandapipes/properties/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/converter/
+Filename: pandapipes-0.8.5/pandapipes/std_types/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/control/
+Filename: pandapipes-0.8.5/pandapipes/test/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/
+Filename: pandapipes-0.8.5/pandapipes/networks/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/component_models/
+Filename: pandapipes-0.8.5/pandapipes/create.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/topology/
+Filename: pandapipes-0.8.5/pandapipes/toolbox.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/multinet/
+Filename: pandapipes-0.8.5/pandapipes/pipeflow.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/
+Filename: pandapipes-0.8.5/pandapipes/idx_node.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/plotting/
+Filename: pandapipes-0.8.5/pandapipes/pandapipes_net.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/pipeflow.py
+Filename: pandapipes-0.8.5/pandapipes/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/create.py
+Filename: pandapipes-0.8.5/pandapipes/idx_branch.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/__init__.py
+Filename: pandapipes-0.8.5/pandapipes/constants.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/constants.py
+Filename: pandapipes-0.8.5/pandapipes/control/run_control.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/toolbox.py
+Filename: pandapipes-0.8.5/pandapipes/control/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/idx_node.py
+Filename: pandapipes-0.8.5/pandapipes/timeseries/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/pandapipes_net.py
+Filename: pandapipes-0.8.5/pandapipes/timeseries/run_time_series.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/idx_branch.py
+Filename: pandapipes-0.8.5/pandapipes/component_models/abstract_models/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/timeseries/run_time_series.py
+Filename: pandapipes-0.8.5/pandapipes/component_models/circulation_pump_mass_component.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/timeseries/__init__.py
+Filename: pandapipes-0.8.5/pandapipes/component_models/pressure_control_component.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/std_types/library/
+Filename: pandapipes-0.8.5/pandapipes/component_models/valve_component.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/std_types/std_types.py
+Filename: pandapipes-0.8.5/pandapipes/component_models/heat_exchanger_component.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/std_types/__init__.py
+Filename: pandapipes-0.8.5/pandapipes/component_models/source_component.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/std_types/std_type_class.py
+Filename: pandapipes-0.8.5/pandapipes/component_models/pump_component.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/std_types/library/Pump/
+Filename: pandapipes-0.8.5/pandapipes/component_models/ext_grid_component.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/std_types/library/Pipe.csv
+Filename: pandapipes-0.8.5/pandapipes/component_models/junction_component.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/std_types/library/Pump/P3.csv
+Filename: pandapipes-0.8.5/pandapipes/component_models/component_toolbox.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/std_types/library/Pump/P2.csv
+Filename: pandapipes-0.8.5/pandapipes/component_models/pipe_component.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/std_types/library/Pump/P1.csv
+Filename: pandapipes-0.8.5/pandapipes/component_models/mass_storage_component.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/pf/build_system_matrix.py
+Filename: pandapipes-0.8.5/pandapipes/component_models/flow_control_component.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/pf/pipeflow_setup.py
+Filename: pandapipes-0.8.5/pandapipes/component_models/circulation_pump_pressure_component.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/pf/derivative_toolbox_numba.py
+Filename: pandapipes-0.8.5/pandapipes/component_models/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/pf/derivative_calculation.py
+Filename: pandapipes-0.8.5/pandapipes/component_models/sink_component.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/pf/result_extraction.py
+Filename: pandapipes-0.8.5/pandapipes/component_models/compressor_component.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/pf/__init__.py
+Filename: pandapipes-0.8.5/pandapipes/component_models/abstract_models/base_component.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/pf/internals_toolbox.py
+Filename: pandapipes-0.8.5/pandapipes/component_models/abstract_models/branch_models.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/pf/derivative_toolbox.py
+Filename: pandapipes-0.8.5/pandapipes/component_models/abstract_models/branch_wzerolength_models.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/io/file_io.py
+Filename: pandapipes-0.8.5/pandapipes/component_models/abstract_models/node_models.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/io/__init__.py
+Filename: pandapipes-0.8.5/pandapipes/component_models/abstract_models/branch_wo_internals_models.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/io/convert_format.py
+Filename: pandapipes-0.8.5/pandapipes/component_models/abstract_models/branch_w_internals_models.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/io/io_utils.py
+Filename: pandapipes-0.8.5/pandapipes/component_models/abstract_models/circulation_pump.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/
+Filename: pandapipes-0.8.5/pandapipes/component_models/abstract_models/const_flow_models.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/stanet_comparison/
+Filename: pandapipes-0.8.5/pandapipes/component_models/abstract_models/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/openmodelica_comparison/
+Filename: pandapipes-0.8.5/pandapipes/component_models/abstract_models/node_element_models.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/io/
+Filename: pandapipes-0.8.5/pandapipes/multinet/control/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/converter/
+Filename: pandapipes-0.8.5/pandapipes/multinet/timeseries/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/networks/
+Filename: pandapipes-0.8.5/pandapipes/multinet/multinet.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/multinet/
+Filename: pandapipes-0.8.5/pandapipes/multinet/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/properties/
+Filename: pandapipes-0.8.5/pandapipes/multinet/create_multinet.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/plotting/
+Filename: pandapipes-0.8.5/pandapipes/multinet/control/controller/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/
+Filename: pandapipes-0.8.5/pandapipes/multinet/control/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/test_toolbox.py
+Filename: pandapipes-0.8.5/pandapipes/multinet/control/run_control_multinet.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/run_tests.py
+Filename: pandapipes-0.8.5/pandapipes/multinet/control/controller/multinet_control.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/__init__.py
+Filename: pandapipes-0.8.5/pandapipes/multinet/control/controller/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/test_imports.py
+Filename: pandapipes-0.8.5/pandapipes/multinet/timeseries/run_time_series_multinet.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/
+Filename: pandapipes-0.8.5/pandapipes/multinet/timeseries/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/test_update_matrix.py
+Filename: pandapipes-0.8.5/pandapipes/converter/stanet/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/test_pipeflow_modes.py
+Filename: pandapipes-0.8.5/pandapipes/converter/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/test_options.py
+Filename: pandapipes-0.8.5/pandapipes/converter/stanet/valve_pipe_component/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/test_inservice.py
+Filename: pandapipes-0.8.5/pandapipes/converter/stanet/data_cleaning.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/__init__.py
+Filename: pandapipes-0.8.5/pandapipes/converter/stanet/stanet2pandapipes.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/test_non_convergence.py
+Filename: pandapipes-0.8.5/pandapipes/converter/stanet/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/test_time_series.py
+Filename: pandapipes-0.8.5/pandapipes/converter/stanet/preparing_steps.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/test_pipeflow_analytic_comparison.py
+Filename: pandapipes-0.8.5/pandapipes/converter/stanet/table_creation.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_results/
+Filename: pandapipes-0.8.5/pandapipes/converter/stanet/valve_pipe_component/valve_pipe_component.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/Temperature_masche_1load_an.csv
+Filename: pandapipes-0.8.5/pandapipes/converter/stanet/valve_pipe_component/valve_pipe_plotting.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_valve.csv
+Filename: pandapipes-0.8.5/pandapipes/converter/stanet/valve_pipe_component/create_valve_pipe.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_source_profiles.csv
+Filename: pandapipes-0.8.5/pandapipes/converter/stanet/valve_pipe_component/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/Temperature_masche_1load_direction_an.csv
+Filename: pandapipes-0.8.5/pandapipes/io/file_io.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_pump.csv
+Filename: pandapipes-0.8.5/pandapipes/io/convert_format.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/Temperature_2zu_2ab_an.csv
+Filename: pandapipes-0.8.5/pandapipes/io/io_utils.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/pressure_control_test_analytical.csv
+Filename: pandapipes-0.8.5/pandapipes/io/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/ext_grid_p.csv
+Filename: pandapipes-0.8.5/pandapipes/pf/derivative_toolbox.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/hydraulics.csv
+Filename: pandapipes-0.8.5/pandapipes/pf/result_extraction.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/Temperature_tee_2ab_1zu_an.csv
+Filename: pandapipes-0.8.5/pandapipes/pf/derivative_toolbox_numba.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_circ_pump_mass.csv
+Filename: pandapipes-0.8.5/pandapipes/pf/pipeflow_setup.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/Temperature_tee_2zu_1ab_an.csv
+Filename: pandapipes-0.8.5/pandapipes/pf/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/heat_exchanger_test.csv
+Filename: pandapipes-0.8.5/pandapipes/pf/internals_toolbox.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_pressure_control.csv
+Filename: pandapipes-0.8.5/pandapipes/pf/derivative_calculation.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/Temperature_one_pipe_an.csv
+Filename: pandapipes-0.8.5/pandapipes/pf/build_system_matrix.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/gas_sections_an.csv
+Filename: pandapipes-0.8.5/pandapipes/topology/graph_searches.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_circ_pump_pressure.csv
+Filename: pandapipes-0.8.5/pandapipes/topology/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_sink_profiles.csv
+Filename: pandapipes-0.8.5/pandapipes/topology/create_graph.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/
+Filename: pandapipes-0.8.5/pandapipes/plotting/pipeflow_results.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_sink/
+Filename: pandapipes-0.8.5/pandapipes/plotting/geo.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_ext_grid/
+Filename: pandapipes-0.8.5/pandapipes/plotting/generic_geodata.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_junction/
+Filename: pandapipes-0.8.5/pandapipes/plotting/simple_plot.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_source/
+Filename: pandapipes-0.8.5/pandapipes/plotting/patch_makers.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/lambda.csv
+Filename: pandapipes-0.8.5/pandapipes/plotting/collections.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/reynolds.csv
+Filename: pandapipes-0.8.5/pandapipes/plotting/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/v_mean_m_per_s.csv
+Filename: pandapipes-0.8.5/pandapipes/plotting/plotting_toolbox.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_sink/mdot_kg_per_s.csv
+Filename: pandapipes-0.8.5/pandapipes/properties/methane/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_ext_grid/mdot_kg_per_s.csv
+Filename: pandapipes-0.8.5/pandapipes/properties/carbondioxide/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_junction/p_bar.csv
+Filename: pandapipes-0.8.5/pandapipes/properties/lgas/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_source/mdot_kg_per_s.csv
+Filename: pandapipes-0.8.5/pandapipes/properties/ethane/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/stanet_comparison/pipeflow_stanet_comparison.py
+Filename: pandapipes-0.8.5/pandapipes/properties/air/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/stanet_comparison/test_gas_stanet.py
+Filename: pandapipes-0.8.5/pandapipes/properties/water/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/stanet_comparison/__init__.py
+Filename: pandapipes-0.8.5/pandapipes/properties/nitrogen/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/stanet_comparison/test_water_stanet.py
+Filename: pandapipes-0.8.5/pandapipes/properties/hgas/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/openmodelica_comparison/test_heat_transfer_openmodelica.py
+Filename: pandapipes-0.8.5/pandapipes/properties/oxygen/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/openmodelica_comparison/test_water_openmodelica.py
+Filename: pandapipes-0.8.5/pandapipes/properties/hydrogen/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/openmodelica_comparison/pipeflow_openmodelica_comparison.py
+Filename: pandapipes-0.8.5/pandapipes/properties/properties_toolbox.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/openmodelica_comparison/__init__.py
+Filename: pandapipes-0.8.5/pandapipes/properties/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/io/test_file_io.py
+Filename: pandapipes-0.8.5/pandapipes/properties/fluids.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/io/__init__.py
+Filename: pandapipes-0.8.5/pandapipes/properties/methane/higher_heating_value.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/converter/converter_test_files/
+Filename: pandapipes-0.8.5/pandapipes/properties/methane/compressibility.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/converter/__init__.py
+Filename: pandapipes-0.8.5/pandapipes/properties/methane/molar_mass.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/converter/test_stanet_converter.py
+Filename: pandapipes-0.8.5/pandapipes/properties/methane/density.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_2valvepipe.csv
+Filename: pandapipes-0.8.5/pandapipes/properties/methane/heat_capacity.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/converter/converter_test_files/Exampelonia_mini.csv
+Filename: pandapipes-0.8.5/pandapipes/properties/methane/der_compressibility.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_valve_2sliders_closed.csv
+Filename: pandapipes-0.8.5/pandapipes/properties/methane/viscosity.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_valve_2sliders_open.csv
+Filename: pandapipes-0.8.5/pandapipes/properties/methane/lower_heating_value.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/networks/__init__.py
+Filename: pandapipes-0.8.5/pandapipes/properties/carbondioxide/molar_mass.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/networks/test_networks.py
+Filename: pandapipes-0.8.5/pandapipes/properties/carbondioxide/density.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/multinet/__init__.py
+Filename: pandapipes-0.8.5/pandapipes/properties/carbondioxide/heat_capacity.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/multinet/test_control_multinet.py
+Filename: pandapipes-0.8.5/pandapipes/properties/carbondioxide/viscosity.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/multinet/test_time_series_multinet.py
+Filename: pandapipes-0.8.5/pandapipes/properties/lgas/higher_heating_value.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/properties/__init__.py
+Filename: pandapipes-0.8.5/pandapipes/properties/lgas/compressibility.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/properties/test_properties_toolbox.py
+Filename: pandapipes-0.8.5/pandapipes/properties/lgas/molar_mass.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/properties/test_fluid_specials.py
+Filename: pandapipes-0.8.5/pandapipes/properties/lgas/density.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/plotting/test_collections.py
+Filename: pandapipes-0.8.5/pandapipes/properties/lgas/heat_capacity.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/plotting/test_pipeflow_results.py
+Filename: pandapipes-0.8.5/pandapipes/properties/lgas/der_compressibility.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/plotting/__init__.py
+Filename: pandapipes-0.8.5/pandapipes/properties/lgas/viscosity.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/plotting/test_simple_collections.py
+Filename: pandapipes-0.8.5/pandapipes/properties/lgas/lower_heating_value.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/plotting/test_generic_coordinates.py
+Filename: pandapipes-0.8.5/pandapipes/properties/ethane/molar_mass.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/test_components/
+Filename: pandapipes-0.8.5/pandapipes/properties/ethane/density.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/release_cycle/
+Filename: pandapipes-0.8.5/pandapipes/properties/ethane/heat_capacity.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/old_versions/
+Filename: pandapipes-0.8.5/pandapipes/properties/ethane/viscosity.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/test_aux_function.py
+Filename: pandapipes-0.8.5/pandapipes/properties/air/compressibility.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/test_std_types.py
+Filename: pandapipes-0.8.5/pandapipes/properties/air/molar_mass.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/test_create.py
+Filename: pandapipes-0.8.5/pandapipes/properties/air/density.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/__init__.py
+Filename: pandapipes-0.8.5/pandapipes/properties/air/heat_capacity.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/test_special_networks.py
+Filename: pandapipes-0.8.5/pandapipes/properties/air/der_compressibility.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/test_network_tables.py
+Filename: pandapipes-0.8.5/pandapipes/properties/air/viscosity.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/test_time_series.py
+Filename: pandapipes-0.8.5/pandapipes/properties/water/compressibility.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/test_convert_format.py
+Filename: pandapipes-0.8.5/pandapipes/properties/water/molar_mass.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/test_components/test_circ_pump_pressure.py
+Filename: pandapipes-0.8.5/pandapipes/properties/water/density.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/test_components/test_circ_pump_mass.py
+Filename: pandapipes-0.8.5/pandapipes/properties/water/heat_capacity.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/test_components/test_valve.py
+Filename: pandapipes-0.8.5/pandapipes/properties/water/der_compressibility.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/test_components/test_pump.py
+Filename: pandapipes-0.8.5/pandapipes/properties/water/viscosity.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/test_components/test_compressor.py
+Filename: pandapipes-0.8.5/pandapipes/properties/nitrogen/molar_mass.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/test_components/test_heat_exchanger.py
+Filename: pandapipes-0.8.5/pandapipes/properties/nitrogen/density.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/test_components/test_flow_control.py
+Filename: pandapipes-0.8.5/pandapipes/properties/nitrogen/heat_capacity.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/test_components/test_pipe_results.py
+Filename: pandapipes-0.8.5/pandapipes/properties/nitrogen/viscosity.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/test_components/__init__.py
+Filename: pandapipes-0.8.5/pandapipes/properties/hgas/higher_heating_value.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/test_components/test_ext_grid.py
+Filename: pandapipes-0.8.5/pandapipes/properties/hgas/compressibility.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/test_components/test_mass_storage.py
+Filename: pandapipes-0.8.5/pandapipes/properties/hgas/molar_mass.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/test_components/test_pressure_control.py
+Filename: pandapipes-0.8.5/pandapipes/properties/hgas/density.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/release_cycle/release_control_test_sink_profiles.csv
+Filename: pandapipes-0.8.5/pandapipes/properties/hgas/heat_capacity.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/release_cycle/release_control_test_source_profiles.csv
+Filename: pandapipes-0.8.5/pandapipes/properties/hgas/der_compressibility.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.8.1_gas.json
+Filename: pandapipes-0.8.5/pandapipes/properties/hgas/viscosity.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.2.0.json
+Filename: pandapipes-0.8.5/pandapipes/properties/hgas/lower_heating_value.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.8.4_gas.json
+Filename: pandapipes-0.8.5/pandapipes/properties/oxygen/molar_mass.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.8.2_water.json
+Filename: pandapipes-0.8.5/pandapipes/properties/oxygen/density.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.8.3_water.json
+Filename: pandapipes-0.8.5/pandapipes/properties/oxygen/heat_capacity.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.1.2.json
+Filename: pandapipes-0.8.5/pandapipes/properties/oxygen/viscosity.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.8.3_gas.json
+Filename: pandapipes-0.8.5/pandapipes/properties/hydrogen/higher_heating_value.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.8.0_gas.json
+Filename: pandapipes-0.8.5/pandapipes/properties/hydrogen/compressibility.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.8.4_water.json
+Filename: pandapipes-0.8.5/pandapipes/properties/hydrogen/molar_mass.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.1.1.json
+Filename: pandapipes-0.8.5/pandapipes/properties/hydrogen/density.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.8.1_water.json
+Filename: pandapipes-0.8.5/pandapipes/properties/hydrogen/heat_capacity.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.1.0.json
+Filename: pandapipes-0.8.5/pandapipes/properties/hydrogen/der_compressibility.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.5.0.json
+Filename: pandapipes-0.8.5/pandapipes/properties/hydrogen/viscosity.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.8.2_gas.json
+Filename: pandapipes-0.8.5/pandapipes/properties/hydrogen/lower_heating_value.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.7.0.json
+Filename: pandapipes-0.8.5/pandapipes/std_types/library/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.8.0_water.json
+Filename: pandapipes-0.8.5/pandapipes/std_types/std_types.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.4.0.json
+Filename: pandapipes-0.8.5/pandapipes/std_types/std_type_class.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.6.0.json
+Filename: pandapipes-0.8.5/pandapipes/std_types/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/converter/stanet/
+Filename: pandapipes-0.8.5/pandapipes/std_types/library/Pump/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/converter/__init__.py
+Filename: pandapipes-0.8.5/pandapipes/std_types/library/Pipe.csv
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/converter/stanet/valve_pipe_component/
+Filename: pandapipes-0.8.5/pandapipes/std_types/library/Pump/P3.csv
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/converter/stanet/data_cleaning.py
+Filename: pandapipes-0.8.5/pandapipes/std_types/library/Pump/P1.csv
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/converter/stanet/preparing_steps.py
+Filename: pandapipes-0.8.5/pandapipes/std_types/library/Pump/P2.csv
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/converter/stanet/stanet2pandapipes.py
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/converter/stanet/__init__.py
+Filename: pandapipes-0.8.5/pandapipes/test/multinet/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/converter/stanet/table_creation.py
+Filename: pandapipes-0.8.5/pandapipes/test/converter/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/converter/stanet/valve_pipe_component/valve_pipe_component.py
+Filename: pandapipes-0.8.5/pandapipes/test/io/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/converter/stanet/valve_pipe_component/valve_pipe_plotting.py
+Filename: pandapipes-0.8.5/pandapipes/test/api/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/converter/stanet/valve_pipe_component/__init__.py
+Filename: pandapipes-0.8.5/pandapipes/test/openmodelica_comparison/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/converter/stanet/valve_pipe_component/create_valve_pipe.py
+Filename: pandapipes-0.8.5/pandapipes/test/plotting/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/control/run_control.py
+Filename: pandapipes-0.8.5/pandapipes/test/properties/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/control/__init__.py
+Filename: pandapipes-0.8.5/pandapipes/test/stanet_comparison/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/
+Filename: pandapipes-0.8.5/pandapipes/test/networks/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/simple_water_networks.py
+Filename: pandapipes-0.8.5/pandapipes/test/test_imports.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/simple_heat_transfer_networks.py
+Filename: pandapipes-0.8.5/pandapipes/test/run_tests.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/simple_gas_networks.py
+Filename: pandapipes-0.8.5/pandapipes/test/test_toolbox.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/nw_aux.py
+Filename: pandapipes-0.8.5/pandapipes/test/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/__init__.py
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_pipeflow_modes.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_inservice.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_pipeflow_analytic_comparison.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/gas_net_schutterwald_1bar.json
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_options.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_non_convergence.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_update_matrix.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_time_series.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/combined_networks/
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/Temperature_2zu_2ab_an.csv
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/t_cross/
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/hydraulics.csv
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_valve.csv
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/two_pressure_junctions/
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/Temperature_tee_2ab_1zu_an.csv
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/two_pumps.json
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_pump.csv
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/two_pipes.json
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/Temperature_masche_1load_an.csv
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/strand_net.json
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_sink_profiles.csv
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/cross_3ext.json
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/Temperature_one_pipe_an.csv
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/combined_networks/versatility.json
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_source_profiles.csv
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/combined_networks/mixed_net.json
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/ext_grid_p.csv
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_2.json
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_pressure_control.csv
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_3.json
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/Temperature_masche_1load_direction_an.csv
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_1.json
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/Temperature_tee_2zu_1ab_an.csv
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/t_cross/t_cross.json
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/gas_sections_an.csv
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/t_cross/valves.json
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_circ_pump_pressure.csv
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/delta.json
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_circ_pump_mass.csv
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/pumps.json
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/heat_exchanger_test.csv
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/two_valves.json
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/pressure_control_test_analytical.csv
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/heights.json
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_sink/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/two_pressure_junctions/two_pipes.json
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_source/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/delta.json
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_ext_grid/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/t_cross.json
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/delta_2sinks.json
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_junction/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/one_source.json
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_sink/mdot_kg_per_s.csv
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/one_pipe.json
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_source/mdot_kg_per_s.csv
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/two_pipes.json
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_ext_grid/mdot_kg_per_s.csv
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/section_variation.json
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/v_mean_m_per_s.csv
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/heights.json
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/lambda.csv
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/reynolds.csv
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/combined_networks/
+Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_junction/p_bar.csv
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/
+Filename: pandapipes-0.8.5/pandapipes/test/multinet/test_time_series_multinet.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/t_cross/
+Filename: pandapipes-0.8.5/pandapipes/test/multinet/test_control_multinet.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/
+Filename: pandapipes-0.8.5/pandapipes/test/multinet/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/two_pressure_junctions/
+Filename: pandapipes-0.8.5/pandapipes/test/converter/converter_test_files/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net_stanet_variation2.json
+Filename: pandapipes-0.8.5/pandapipes/test/converter/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/two_pumps.json
+Filename: pandapipes-0.8.5/pandapipes/test/converter/test_stanet_converter.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/two_pipes.json
+Filename: pandapipes-0.8.5/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_2valvepipe.csv
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net.json
+Filename: pandapipes-0.8.5/pandapipes/test/converter/converter_test_files/Exampelonia_mini.csv
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/cross_3ext.json
+Filename: pandapipes-0.8.5/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_valve_2sliders_closed.csv
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net_stanet_variation1.json
+Filename: pandapipes-0.8.5/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_valve_2sliders_open.csv
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/combined_networks/versatility.json
+Filename: pandapipes-0.8.5/pandapipes/test/io/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/combined_networks/mixed_net.json
+Filename: pandapipes-0.8.5/pandapipes/test/io/test_file_io.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_2.json
+Filename: pandapipes-0.8.5/pandapipes/test/api/test_components/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_3.json
+Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_1.json
+Filename: pandapipes-0.8.5/pandapipes/test/api/release_cycle/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/t_cross/t_cross.json
+Filename: pandapipes-0.8.5/pandapipes/test/api/test_aux_function.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/t_cross/valves.json
+Filename: pandapipes-0.8.5/pandapipes/test/api/test_special_networks.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/delta.json
+Filename: pandapipes-0.8.5/pandapipes/test/api/test_create.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/one_valve_stanet.json
+Filename: pandapipes-0.8.5/pandapipes/test/api/test_std_types.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/pumps.json
+Filename: pandapipes-0.8.5/pandapipes/test/api/test_convert_format.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/two_valves.json
+Filename: pandapipes-0.8.5/pandapipes/test/api/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/heights.json
+Filename: pandapipes-0.8.5/pandapipes/test/api/test_network_tables.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/two_pressure_junctions/two_pipes.json
+Filename: pandapipes-0.8.5/pandapipes/test/api/test_time_series.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/two_pressure_junctions/one_pipe_stanet.json
+Filename: pandapipes-0.8.5/pandapipes/test/api/test_components/test_ext_grid.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/
+Filename: pandapipes-0.8.5/pandapipes/test/api/test_components/test_heat_exchanger.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/
+Filename: pandapipes-0.8.5/pandapipes/test/api/test_components/test_valve.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/
+Filename: pandapipes-0.8.5/pandapipes/test/api/test_components/test_flow_control.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/
+Filename: pandapipes-0.8.5/pandapipes/test/api/test_components/test_pump.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/
+Filename: pandapipes-0.8.5/pandapipes/test/api/test_components/test_pressure_control.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/t_cross/
+Filename: pandapipes-0.8.5/pandapipes/test/api/test_components/test_compressor.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/
+Filename: pandapipes-0.8.5/pandapipes/test/api/test_components/test_pipe_results.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/two_pressure_junctions/
+Filename: pandapipes-0.8.5/pandapipes/test/api/test_components/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/two_pipes_PC.json
+Filename: pandapipes-0.8.5/pandapipes/test/api/test_components/test_mass_storage.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/strand_net_N.json
+Filename: pandapipes-0.8.5/pandapipes/test/api/test_components/test_circ_pump_mass.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/two_pipes_N.json
+Filename: pandapipes-0.8.5/pandapipes/test/api/test_components/test_circ_pump_pressure.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/cross_PC.json
+Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.1.1.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/pump_N.json
+Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.5_water.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/strand_net_PC.json
+Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.4.0.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/versatility_N.json
+Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.3_water.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/district_N.json
+Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.7.0.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/versatility_PC.json
+Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.2_water.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/district_PC.json
+Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.4_gas.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_3_PC.json
+Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.3_gas.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_3_N.json
+Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.6.0.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_1_PC.json
+Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.5_gas.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_2_PC.json
+Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.1_gas.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_2_N.json
+Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.0_gas.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_1_N.json
+Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.1_water.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/t_cross/t_cross_N.json
+Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.4_water.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/t_cross/t_cross_PC.json
+Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.1.2.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/delta_N.json
+Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.1.0.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/two_valves_PC.json
+Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.2_gas.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/two_valves_N.json
+Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.5.0.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/pumps_N.json
+Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.2.0.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/two_pressure_junctions/two_pipes_PC.json
+Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.0_water.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/two_pressure_junctions/two_pipes_N.json
+Filename: pandapipes-0.8.5/pandapipes/test/api/release_cycle/release_control_test_source_profiles.csv
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/
+Filename: pandapipes-0.8.5/pandapipes/test/api/release_cycle/release_control_test_sink_profiles.csv
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/
+Filename: pandapipes-0.8.5/pandapipes/test/openmodelica_comparison/test_water_openmodelica.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/
+Filename: pandapipes-0.8.5/pandapipes/test/openmodelica_comparison/pipeflow_openmodelica_comparison.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/
+Filename: pandapipes-0.8.5/pandapipes/test/openmodelica_comparison/test_heat_transfer_openmodelica.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/
+Filename: pandapipes-0.8.5/pandapipes/test/openmodelica_comparison/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/two_pressure_junctions/
+Filename: pandapipes-0.8.5/pandapipes/test/plotting/test_simple_collections.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/two_pipes_PC.json
+Filename: pandapipes-0.8.5/pandapipes/test/plotting/test_generic_coordinates.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/two_pipes_N.json
+Filename: pandapipes-0.8.5/pandapipes/test/plotting/test_pipeflow_results.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/pump_N.json
+Filename: pandapipes-0.8.5/pandapipes/test/plotting/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/parallel_PC.json
+Filename: pandapipes-0.8.5/pandapipes/test/plotting/test_collections.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/parallel_N.json
+Filename: pandapipes-0.8.5/pandapipes/test/properties/test_fluid_specials.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/versatility_PC.json
+Filename: pandapipes-0.8.5/pandapipes/test/properties/test_properties_toolbox.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_1_PC.json
+Filename: pandapipes-0.8.5/pandapipes/test/properties/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_2_PC.json
+Filename: pandapipes-0.8.5/pandapipes/test/stanet_comparison/test_water_stanet.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_2_N.json
+Filename: pandapipes-0.8.5/pandapipes/test/stanet_comparison/test_gas_stanet.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_1_N.json
+Filename: pandapipes-0.8.5/pandapipes/test/stanet_comparison/pipeflow_stanet_comparison.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross2_N.json
+Filename: pandapipes-0.8.5/pandapipes/test/stanet_comparison/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross1_PC.json
+Filename: pandapipes-0.8.5/pandapipes/test/networks/test_networks.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross2_PC.json
+Filename: pandapipes-0.8.5/pandapipes/test/networks/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross1_N.json
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/square_N.json
+Filename: pandapipes-0.8.5/pandapipes/networks/nw_aux.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/square_PC.json
+Filename: pandapipes-0.8.5/pandapipes/networks/simple_water_networks.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/two_valves_PC.json
+Filename: pandapipes-0.8.5/pandapipes/networks/simple_heat_transfer_networks.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/two_valves_N.json
+Filename: pandapipes-0.8.5/pandapipes/networks/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/delta_PC.json
+Filename: pandapipes-0.8.5/pandapipes/networks/simple_gas_networks.py
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/pumps_N.json
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/two_pressure_junctions/H_net_N.json
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/two_pressure_junctions/H_net_PC.json
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb4--0-no_sw.json
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/gas_net_schutterwald_1bar.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/1-LV-urban6--0-sw.json
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb4--0-sw.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural1--0-no_sw.json
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural1--0-no_sw.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural2--0-no_sw.json
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb5--0-sw.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural1--0-sw.json
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb5--0-no_sw.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural2--0-sw.json
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural2--0-sw.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural3--0-no_sw.json
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-urban6--0-no_sw.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb5--0-sw.json
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-urban6--0-sw.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural3--0-sw.json
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural3--0-sw.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb5--0-no_sw.json
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural2--0-no_sw.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/1-LV-urban6--0-no_sw.json
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural1--0-sw.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb4--0-sw.json
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb4--0-no_sw.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/component_models/abstract_models/
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural3--0-no_sw.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/component_models/ext_grid_component.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/component_models/flow_control_component.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/component_models/compressor_component.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/component_models/pipe_component.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/component_models/mass_storage_component.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/component_models/source_component.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/component_models/junction_component.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/two_pressure_junctions/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/component_models/circulation_pump_mass_component.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/component_models/circulation_pump_pressure_component.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/two_pipes_N.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/component_models/__init__.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/two_pipes_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/component_models/pressure_control_component.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/pump_N.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/component_models/heat_exchanger_component.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/parallel_N.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/component_models/sink_component.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/parallel_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/component_models/component_toolbox.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/versatility_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/component_models/valve_component.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross1_N.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/component_models/pump_component.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross2_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/component_models/abstract_models/branch_wo_internals_models.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross2_N.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/component_models/abstract_models/branch_models.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross1_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/component_models/abstract_models/branch_wzerolength_models.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/two_valves_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/component_models/abstract_models/const_flow_models.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/square_N.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/component_models/abstract_models/base_component.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/two_valves_N.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/component_models/abstract_models/__init__.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/delta_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/component_models/abstract_models/circulation_pump.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/pumps_N.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/component_models/abstract_models/node_element_models.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/square_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/component_models/abstract_models/node_models.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/two_pressure_junctions/H_net_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/component_models/abstract_models/branch_w_internals_models.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/two_pressure_junctions/H_net_N.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/topology/graph_searches.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_1_N.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/topology/__init__.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_2_N.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/topology/create_graph.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_1_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/multinet/timeseries/
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_2_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/multinet/control/
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/multinet/multinet.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/multinet/create_multinet.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/t_cross/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/multinet/__init__.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/multinet/timeseries/__init__.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/two_pressure_junctions/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/multinet/timeseries/run_time_series_multinet.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/multinet/control/controller/
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/two_pipes_N.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/multinet/control/run_control_multinet.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/two_pipes_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/multinet/control/__init__.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/pump_N.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/multinet/control/controller/multinet_control.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/strand_net_N.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/multinet/control/controller/__init__.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/cross_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/carbondioxide/
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/strand_net_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/lgas/
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/versatility_N.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/hydrogen/
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/district_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/hgas/
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/versatility_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/methane/
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/district_N.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/ethane/
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/t_cross/t_cross_N.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/water/
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/t_cross/t_cross_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/air/
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/two_valves_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/nitrogen/
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/two_valves_N.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/oxygen/
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/delta_N.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/properties_toolbox.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/pumps_N.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/__init__.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/two_pressure_junctions/two_pipes_N.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/fluids.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/two_pressure_junctions/two_pipes_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/carbondioxide/heat_capacity.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_1_N.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/carbondioxide/molar_mass.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_2_N.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/carbondioxide/viscosity.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_3_N.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/carbondioxide/density.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_1_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/lgas/heat_capacity.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_3_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/lgas/molar_mass.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_2_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/lgas/compressibility.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/lgas/viscosity.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/lgas/higher_heating_value.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/lgas/lower_heating_value.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/t_cross.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/lgas/density.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/heights.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/lgas/der_compressibility.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/one_pipe.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/hydrogen/heat_capacity.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/one_source.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/hydrogen/molar_mass.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/delta_2sinks.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/hydrogen/compressibility.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/delta.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/hydrogen/viscosity.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/two_pipes.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/hydrogen/higher_heating_value.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/section_variation.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/hydrogen/lower_heating_value.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/hydrogen/density.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/combined_networks/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/hydrogen/der_compressibility.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/t_cross/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/hgas/heat_capacity.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/hgas/molar_mass.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/two_pressure_junctions/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/hgas/compressibility.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/hgas/viscosity.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/two_pumps.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/hgas/higher_heating_value.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/strand_net.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/hgas/lower_heating_value.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/cross_3ext.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/hgas/density.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/two_pipes.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/hgas/der_compressibility.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/combined_networks/versatility.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/methane/heat_capacity.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/combined_networks/mixed_net.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/methane/molar_mass.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/t_cross/t_cross.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/methane/compressibility.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/t_cross/valves.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/methane/viscosity.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/heights.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/methane/higher_heating_value.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/pumps.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/methane/lower_heating_value.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/delta.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/methane/density.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/two_valves.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/methane/der_compressibility.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/two_pressure_junctions/two_pipes.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/ethane/heat_capacity.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_3.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/ethane/molar_mass.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_1.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/ethane/viscosity.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_2.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/ethane/density.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/water/heat_capacity.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/combined_networks/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/water/molar_mass.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/t_cross/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/water/compressibility.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/water/viscosity.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/two_pressure_junctions/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/water/density.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/water/der_compressibility.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net_stanet_variation1.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/air/heat_capacity.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/two_pumps.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/air/molar_mass.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/air/compressibility.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/cross_3ext.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/air/viscosity.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net_stanet_variation2.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/air/density.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/two_pipes.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/air/der_compressibility.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/combined_networks/versatility.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/nitrogen/heat_capacity.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/combined_networks/mixed_net.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/nitrogen/molar_mass.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/t_cross/t_cross.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/nitrogen/viscosity.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/t_cross/valves.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/nitrogen/density.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/heights.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/oxygen/heat_capacity.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/one_valve_stanet.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/oxygen/molar_mass.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/pumps.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/oxygen/viscosity.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/delta.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/properties/oxygen/density.txt
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/two_valves.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/plotting/simple_plot.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/two_pressure_junctions/one_pipe_stanet.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/plotting/generic_geodata.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/two_pressure_junctions/two_pipes.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/plotting/geo.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_3.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/plotting/pipeflow_results.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_1.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/plotting/__init__.py
+Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_2.json
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/plotting/patch_makers.py
+Filename: pandapipes-0.8.5/pandapipes.egg-info/PKG-INFO
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/plotting/plotting_toolbox.py
+Filename: pandapipes-0.8.5/pandapipes.egg-info/top_level.txt
 Comment: 
 
-Filename: pandapipes-0.8.4/pandapipes/plotting/collections.py
+Filename: pandapipes-0.8.5/pandapipes.egg-info/SOURCES.txt
+Comment: 
+
+Filename: pandapipes-0.8.5/pandapipes.egg-info/requires.txt
+Comment: 
+
+Filename: pandapipes-0.8.5/pandapipes.egg-info/dependency_links.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `pandapipes-0.8.4/PKG-INFO` & `pandapipes-0.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandapipes
-Version: 0.8.4
+Version: 0.8.5
 Summary: A pipeflow calculation tool that complements pandapower in the simulation of multi energy grids
 Home-page: http://www.pandapipes.org
 Author: Simon Ruben Drauz-Mauel, Daniel Lohmeier, Jolando Marius Kisse
 Author-email: simon.ruben.drauz-mauel@iee.fraunhofer.de, daniel.lohmeier@retoflow.de, jolando.kisse@uni-kassel.de
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -12,18 +12,17 @@
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: plotting
 Provides-Extra: test
 Provides-Extra: all
 License-File: LICENSE
 
@@ -110,14 +109,22 @@
 We welcome contributions to pandapipes of any kind - if you want to contribute, please check out
 the `pandapipes contribution guidelines <https://github.com/e2nIEE/pandapipes/blob/develop/CONTRIBUTING.rst>`_.
 
 
 Change Log
 =============
 
+[0.8.5] - 2023-06-19
+-------------------------------
+- [FIXED] consider ambient pressure in calculation of compression power for pumps/compressors
+- [FIXED] np.bool error in pipeflow calculation due to deprecation of np.bool
+- [FIXED] use igraph package instead of python-igraph (has been renamed)
+- [ADDED] gas specific calculation of heat capacity ration kappa = cp/cv (for pumps/compressors)
+- [REMOVED] Python 3.7 removed from test pipeline due to inconsistencies with pandapower
+
 [0.8.4] - 2023-02-02
 -------------------------------
 - [FIXED] added flow control to nxgraph
 - [FIXED] in case of multiple pumps, there was a bug when calculating pressure
 - [FIXED] if all pumps are out of service, the pipeflow did not converge
 - [FIXED] remove unnecessary checkout in release.yml and tutorial tests
```

## Comparing `pandapipes-0.8.4/CHANGELOG.rst` & `pandapipes-0.8.5/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Change Log
 =============
 
+[0.8.5] - 2023-06-19
+-------------------------------
+- [FIXED] consider ambient pressure in calculation of compression power for pumps/compressors
+- [FIXED] np.bool error in pipeflow calculation due to deprecation of np.bool
+- [FIXED] use igraph package instead of python-igraph (has been renamed)
+- [ADDED] gas specific calculation of heat capacity ration kappa = cp/cv (for pumps/compressors)
+- [REMOVED] Python 3.7 removed from test pipeline due to inconsistencies with pandapower
+
 [0.8.4] - 2023-02-02
 -------------------------------
 - [FIXED] added flow control to nxgraph
 - [FIXED] in case of multiple pumps, there was a bug when calculating pressure
 - [FIXED] if all pumps are out of service, the pipeflow did not converge
 - [FIXED] remove unnecessary checkout in release.yml and tutorial tests
```

## Comparing `pandapipes-0.8.4/AUTHORS` & `pandapipes-0.8.5/AUTHORS`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/setup.py` & `pandapipes-0.8.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,34 +22,34 @@
     'Natural Language :: English',
     'Operating System :: OS Independent',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3']
 
 with open('.github/workflows/run_tests_master.yml', 'rb') as f:
     lines = f.read().decode('utf-8')
-    versions = set(re.findall('3.[7-9]', lines)) | set(re.findall('3.1[0-9]', lines))
+    versions = set(re.findall('3.[8-9]', lines)) | set(re.findall('3.1[0-9]', lines))
     for version in versions:
         classifiers.append('Programming Language :: Python :: %s' % version)
 
 long_description = '\n\n'.join((install, changelog))
 
 setup(
     name='pandapipes',
-    version='0.8.4',
+    version='0.8.5',
     author='Simon Ruben Drauz-Mauel, Daniel Lohmeier, Jolando Marius Kisse',
     author_email='simon.ruben.drauz-mauel@iee.fraunhofer.de, daniel.lohmeier@retoflow.de, '
                  'jolando.kisse@uni-kassel.de',
     description='A pipeflow calculation tool that complements pandapower in the simulation of multi energy grids',
     long_description=long_description,
 	long_description_content_type='text/x-rst',
     url='http://www.pandapipes.org',
     license='BSD',
     install_requires=["pandapower>=2.11.1", "matplotlib", "shapely"],
     extras_require={"docs": ["numpydoc", "sphinx", "sphinx_rtd_theme", "sphinxcontrib.bibtex"],
-                    "plotting": ["plotly", "python-igraph"],
+                    "plotting": ["plotly", "igraph"],
                     "test": ["pytest", "pytest-xdist", "nbmake"],
                     "all": ["numpydoc", "sphinx", "sphinx_rtd_theme", "sphinxcontrib.bibtex",
-                            "plotly", "python-igraph", "pytest", "pytest-xdist", "nbmake"]},
+                            "plotly", "igraph", "pytest", "pytest-xdist", "nbmake"]},
     packages=find_packages(),
     include_package_data=True,
     classifiers=classifiers
 )
```

## Comparing `pandapipes-0.8.4/README.rst` & `pandapipes-0.8.5/README.rst`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/LICENSE` & `pandapipes-0.8.5/LICENSE`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/.github/workflows/release.yml` & `pandapipes-0.8.5/.github/workflows/release.yml`

 * *Files 5% similar despite different names*

```diff
@@ -71,25 +71,25 @@
 
   build:
 
     runs-on: ${{ matrix.os }}
     needs: upload
     strategy:
       matrix:
-        python-version: ['3.7', '3.8', '3.9', '3.10']
+        python-version: ['3.8', '3.9', '3.10']
         os:  [ ubuntu-latest, windows-latest ]
     steps:
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          python -m pip install pytest python-igraph pytest-split numba
+          python -m pip install pytest igraph pytest-split numba
       - name: Install pandapipes from TestPyPI
         if: ${{ inputs.upload_server == 'testpypi'}}
         run: |
           pip install --no-cache-dir -i https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple pandapipes
       - name: Install pandapipes from PyPI
         if: ${{ inputs.upload_server == 'pypi'}}
         run: |
```

## Comparing `pandapipes-0.8.4/.github/workflows/run_tests_develop.yml` & `pandapipes-0.8.5/.github/workflows/run_tests_develop.yml`

 * *Files 1% similar despite different names*

```diff
@@ -14,25 +14,25 @@
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ['3.7', '3.8', '3.9', '3.10']
+        python-version: ['3.8', '3.9', '3.10']
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          python -m pip install pytest python-igraph pytest-split numba
+          python -m pip install pytest igraph pytest-split numba
           if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
           python -m pip install git+https://github.com/e2nIEE/pandapower@develop#egg=pandapower
           pip install .
       - name: List all installed packages
         run: |
           pip list
       - name: Test with pytest
@@ -82,25 +82,25 @@
           # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
           flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
 
   tutorial_tests:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ['3.7', '3.8', '3.9', '3.10']
+        python-version: ['3.8', '3.9', '3.10']
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          python -m pip install pytest nbmake pytest-xdist pytest-split python-igraph numba 
+          python -m pip install pytest nbmake pytest-xdist pytest-split igraph numba 
           if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
           python -m pip install git+https://github.com/e2nIEE/pandapower@develop#egg=pandapower
           pip install .
       - name: List all installed packages
         run: |
           pip list
       - name: Test with pytest
```

## Comparing `pandapipes-0.8.4/.github/workflows/run_tests_master.yml` & `pandapipes-0.8.5/.github/workflows/run_tests_master.yml`

 * *Files 2% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ['3.7', '3.8', '3.9', '3.10']
+        python-version: ['3.8', '3.9', '3.10']
 
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          python -m pip install pytest python-igraph pytest-split numba
+          python -m pip install pytest igraph pytest-split numba
           if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
-          python -m pip install git+https://github.com/e2nIEE/pandapower@master#egg=pandapower
+          python -m pip install git+https://github.com/e2nIEE/pandapower@master#egg=pandapower;
           pip install .
       - name: List all installed packages
         run: |
           pip list
       - name: Test with pytest
         if: ${{ matrix.python-version != '3.9' }}
         run: |
@@ -50,25 +50,25 @@
         with:
           verbose: true
 
   tutorial_tests:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ['3.7', '3.8', '3.9', '3.10']
+        python-version: ['3.8', '3.9', '3.10']
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          python -m pip install pytest nbmake pytest-xdist pytest-split python-igraph numba 
+          python -m pip install pytest nbmake pytest-xdist pytest-split igraph numba 
           if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
           python -m pip install git+https://github.com/e2nIEE/pandapower@master#egg=pandapower
           pip install .
       - name: List all installed packages
         run: |
           pip list
       - name: Test with pytest
```

## Comparing `pandapipes-0.8.4/pandapipes.egg-info/PKG-INFO` & `pandapipes-0.8.5/pandapipes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandapipes
-Version: 0.8.4
+Version: 0.8.5
 Summary: A pipeflow calculation tool that complements pandapower in the simulation of multi energy grids
 Home-page: http://www.pandapipes.org
 Author: Simon Ruben Drauz-Mauel, Daniel Lohmeier, Jolando Marius Kisse
 Author-email: simon.ruben.drauz-mauel@iee.fraunhofer.de, daniel.lohmeier@retoflow.de, jolando.kisse@uni-kassel.de
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -12,18 +12,17 @@
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: plotting
 Provides-Extra: test
 Provides-Extra: all
 License-File: LICENSE
 
@@ -110,14 +109,22 @@
 We welcome contributions to pandapipes of any kind - if you want to contribute, please check out
 the `pandapipes contribution guidelines <https://github.com/e2nIEE/pandapipes/blob/develop/CONTRIBUTING.rst>`_.
 
 
 Change Log
 =============
 
+[0.8.5] - 2023-06-19
+-------------------------------
+- [FIXED] consider ambient pressure in calculation of compression power for pumps/compressors
+- [FIXED] np.bool error in pipeflow calculation due to deprecation of np.bool
+- [FIXED] use igraph package instead of python-igraph (has been renamed)
+- [ADDED] gas specific calculation of heat capacity ration kappa = cp/cv (for pumps/compressors)
+- [REMOVED] Python 3.7 removed from test pipeline due to inconsistencies with pandapower
+
 [0.8.4] - 2023-02-02
 -------------------------------
 - [FIXED] added flow control to nxgraph
 - [FIXED] in case of multiple pumps, there was a bug when calculating pressure
 - [FIXED] if all pumps are out of service, the pipeflow did not converge
 - [FIXED] remove unnecessary checkout in release.yml and tutorial tests
```

## Comparing `pandapipes-0.8.4/pandapipes.egg-info/SOURCES.txt` & `pandapipes-0.8.5/pandapipes.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -292,14 +292,16 @@
 pandapipes/test/api/old_versions/example_0.8.1_water.json
 pandapipes/test/api/old_versions/example_0.8.2_gas.json
 pandapipes/test/api/old_versions/example_0.8.2_water.json
 pandapipes/test/api/old_versions/example_0.8.3_gas.json
 pandapipes/test/api/old_versions/example_0.8.3_water.json
 pandapipes/test/api/old_versions/example_0.8.4_gas.json
 pandapipes/test/api/old_versions/example_0.8.4_water.json
+pandapipes/test/api/old_versions/example_0.8.5_gas.json
+pandapipes/test/api/old_versions/example_0.8.5_water.json
 pandapipes/test/api/release_cycle/release_control_test_sink_profiles.csv
 pandapipes/test/api/release_cycle/release_control_test_source_profiles.csv
 pandapipes/test/api/test_components/__init__.py
 pandapipes/test/api/test_components/test_circ_pump_mass.py
 pandapipes/test/api/test_components/test_circ_pump_pressure.py
 pandapipes/test/api/test_components/test_compressor.py
 pandapipes/test/api/test_components/test_ext_grid.py
```

## Comparing `pandapipes-0.8.4/pandapipes/pipeflow.py` & `pandapipes-0.8.5/pandapipes/pipeflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,16 +79,16 @@
     calculate_hydraulics = calculation_mode in ["hydraulics", "all"]
     calculate_heat = calculation_mode in ["heat", "all"]
 
     if get_net_option(net, "check_connectivity"):
         nodes_connected, branches_connected = check_connectivity(
             net, branch_pit, node_pit, check_heat=calculate_heat)
     else:
-        nodes_connected = node_pit[:, ACTIVE_ND].astype(np.bool)
-        branches_connected = branch_pit[:, ACTIVE_BR].astype(np.bool)
+        nodes_connected = node_pit[:, ACTIVE_ND].astype(np.bool_)
+        branches_connected = branch_pit[:, ACTIVE_BR].astype(np.bool_)
 
     reduce_pit(net, node_pit, branch_pit, nodes_connected, branches_connected)
 
     if calculation_mode == "heat" and not net.user_pf_options["hyd_flag"]:
         raise UserWarning("Converged flag not set. Make sure that hydraulic calculation results "
                           "are available.")
     elif calculation_mode == "heat" and net.user_pf_options["hyd_flag"]:
```

## Comparing `pandapipes-0.8.4/pandapipes/create.py` & `pandapipes-0.8.5/pandapipes/create.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/__init__.py` & `pandapipes-0.8.5/pandapipes/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
-__version__ = '0.8.4'
+__version__ = '0.8.5'
 __format_version__ = '0.8.0'
 
 import pandas as pd
 import os
 
 pd.options.mode.chained_assignment = None  # default='warn'
 pp_dir = os.path.dirname(os.path.realpath(__file__))
```

## Comparing `pandapipes-0.8.4/pandapipes/constants.py` & `pandapipes-0.8.5/pandapipes/constants.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/toolbox.py` & `pandapipes-0.8.5/pandapipes/toolbox.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/idx_node.py` & `pandapipes-0.8.5/pandapipes/idx_node.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/pandapipes_net.py` & `pandapipes-0.8.5/pandapipes/pandapipes_net.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/idx_branch.py` & `pandapipes-0.8.5/pandapipes/idx_branch.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/timeseries/run_time_series.py` & `pandapipes-0.8.5/pandapipes/timeseries/run_time_series.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/std_types/std_types.py` & `pandapipes-0.8.5/pandapipes/std_types/std_types.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/std_types/std_type_class.py` & `pandapipes-0.8.5/pandapipes/std_types/std_type_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,16 +213,17 @@
         reg_st = cls(name, reg_par)
         cls.init_std_type(reg_st, x_values, y_values, degree)
         return reg_st
 
     @classmethod
     def from_list(cls, name, x_values, y_values, degree):
         reg_par, x_values, y_values, degree = cls._from_list(x_values, y_values, degree)
-        reg_st = cls(name, reg_par)
-        cls.init_std_type(reg_st, x_values, y_values, degree)
+        pump_st = cls(name, reg_par)
+        cls.init_std_type(pump_st, x_values, y_values, degree)
+        return pump_st
 
     @classmethod
     def load_data(cls, path):
         """
         load_data.
 
         :param path:
```

## Comparing `pandapipes-0.8.4/pandapipes/std_types/library/Pipe.csv` & `pandapipes-0.8.5/pandapipes/std_types/library/Pipe.csv`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/pf/build_system_matrix.py` & `pandapipes-0.8.5/pandapipes/pf/build_system_matrix.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/pf/pipeflow_setup.py` & `pandapipes-0.8.5/pandapipes/pf/pipeflow_setup.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/pf/derivative_toolbox_numba.py` & `pandapipes-0.8.5/pandapipes/pf/derivative_toolbox_numba.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/pf/derivative_calculation.py` & `pandapipes-0.8.5/pandapipes/pf/derivative_calculation.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/pf/result_extraction.py` & `pandapipes-0.8.5/pandapipes/pf/result_extraction.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/pf/internals_toolbox.py` & `pandapipes-0.8.5/pandapipes/pf/internals_toolbox.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/pf/derivative_toolbox.py` & `pandapipes-0.8.5/pandapipes/pf/derivative_toolbox.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/io/file_io.py` & `pandapipes-0.8.5/pandapipes/io/file_io.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/io/convert_format.py` & `pandapipes-0.8.5/pandapipes/io/convert_format.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/io/io_utils.py` & `pandapipes-0.8.5/pandapipes/io/io_utils.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/test_toolbox.py` & `pandapipes-0.8.5/pandapipes/test/test_toolbox.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/run_tests.py` & `pandapipes-0.8.5/pandapipes/test/run_tests.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/__init__.py` & `pandapipes-0.8.5/pandapipes/test/__init__.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/test_imports.py` & `pandapipes-0.8.5/pandapipes/test/test_imports.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/pipeflow_internals/test_update_matrix.py` & `pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_update_matrix.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/pipeflow_internals/test_pipeflow_modes.py` & `pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_pipeflow_modes.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/pipeflow_internals/test_options.py` & `pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_options.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/pipeflow_internals/test_inservice.py` & `pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_inservice.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/pipeflow_internals/test_non_convergence.py` & `pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_non_convergence.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/pipeflow_internals/test_time_series.py` & `pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_time_series.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/pipeflow_internals/test_pipeflow_analytic_comparison.py` & `pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_pipeflow_analytic_comparison.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_source_profiles.csv` & `pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_source_profiles.csv`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/gas_sections_an.csv` & `pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/gas_sections_an.csv`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_sink_profiles.csv` & `pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_sink_profiles.csv`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/lambda.csv` & `pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/lambda.csv`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/reynolds.csv` & `pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/reynolds.csv`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/v_mean_m_per_s.csv` & `pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/v_mean_m_per_s.csv`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_sink/mdot_kg_per_s.csv` & `pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_sink/mdot_kg_per_s.csv`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_ext_grid/mdot_kg_per_s.csv` & `pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_ext_grid/mdot_kg_per_s.csv`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_junction/p_bar.csv` & `pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_junction/p_bar.csv`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_source/mdot_kg_per_s.csv` & `pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_source/mdot_kg_per_s.csv`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/stanet_comparison/pipeflow_stanet_comparison.py` & `pandapipes-0.8.5/pandapipes/test/stanet_comparison/pipeflow_stanet_comparison.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/stanet_comparison/test_gas_stanet.py` & `pandapipes-0.8.5/pandapipes/test/stanet_comparison/test_gas_stanet.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/stanet_comparison/test_water_stanet.py` & `pandapipes-0.8.5/pandapipes/test/stanet_comparison/test_water_stanet.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/openmodelica_comparison/test_heat_transfer_openmodelica.py` & `pandapipes-0.8.5/pandapipes/test/openmodelica_comparison/test_heat_transfer_openmodelica.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/openmodelica_comparison/test_water_openmodelica.py` & `pandapipes-0.8.5/pandapipes/test/openmodelica_comparison/test_water_openmodelica.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/openmodelica_comparison/pipeflow_openmodelica_comparison.py` & `pandapipes-0.8.5/pandapipes/test/openmodelica_comparison/pipeflow_openmodelica_comparison.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/io/test_file_io.py` & `pandapipes-0.8.5/pandapipes/test/io/test_file_io.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/converter/test_stanet_converter.py` & `pandapipes-0.8.5/pandapipes/test/converter/test_stanet_converter.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_2valvepipe.csv` & `pandapipes-0.8.5/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_2valvepipe.csv`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/converter/converter_test_files/Exampelonia_mini.csv` & `pandapipes-0.8.5/pandapipes/test/converter/converter_test_files/Exampelonia_mini.csv`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_valve_2sliders_closed.csv` & `pandapipes-0.8.5/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_valve_2sliders_closed.csv`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_valve_2sliders_open.csv` & `pandapipes-0.8.5/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_valve_2sliders_open.csv`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/networks/test_networks.py` & `pandapipes-0.8.5/pandapipes/test/networks/test_networks.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/multinet/test_control_multinet.py` & `pandapipes-0.8.5/pandapipes/test/multinet/test_control_multinet.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/multinet/test_time_series_multinet.py` & `pandapipes-0.8.5/pandapipes/test/multinet/test_time_series_multinet.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/properties/test_properties_toolbox.py` & `pandapipes-0.8.5/pandapipes/test/properties/test_properties_toolbox.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/properties/test_fluid_specials.py` & `pandapipes-0.8.5/pandapipes/test/properties/test_fluid_specials.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/plotting/test_collections.py` & `pandapipes-0.8.5/pandapipes/test/plotting/test_collections.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/plotting/test_pipeflow_results.py` & `pandapipes-0.8.5/pandapipes/test/plotting/test_pipeflow_results.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/plotting/test_simple_collections.py` & `pandapipes-0.8.5/pandapipes/test/plotting/test_simple_collections.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/plotting/test_generic_coordinates.py` & `pandapipes-0.8.5/pandapipes/test/plotting/test_generic_coordinates.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     import igraph
 
     IGRAPH_INSTALLED = True
 except ImportError:
     IGRAPH_INSTALLED = False
 
 
-@pytest.mark.skipif(IGRAPH_INSTALLED is False, reason="Requires python-igraph.")
+@pytest.mark.skipif(IGRAPH_INSTALLED is False, reason="Requires igraph.")
 def test_create_generic_coordinates_igraph(base_net_is_with_pumps):
     net = copy.deepcopy(base_net_is_with_pumps)
     net.junction_geodata.drop(net.junction_geodata.index, inplace=True)
     create_generic_coordinates(net, library="igraph")
     assert len(net.junction_geodata) == len(net.junction)
```

## Comparing `pandapipes-0.8.4/pandapipes/test/api/test_aux_function.py` & `pandapipes-0.8.5/pandapipes/test/api/test_aux_function.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/api/test_std_types.py` & `pandapipes-0.8.5/pandapipes/test/api/test_std_types.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/api/test_create.py` & `pandapipes-0.8.5/pandapipes/test/api/test_create.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/api/test_special_networks.py` & `pandapipes-0.8.5/pandapipes/test/api/test_special_networks.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/api/test_network_tables.py` & `pandapipes-0.8.5/pandapipes/test/api/test_network_tables.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/api/test_time_series.py` & `pandapipes-0.8.5/pandapipes/test/api/test_time_series.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/api/test_convert_format.py` & `pandapipes-0.8.5/pandapipes/test/api/test_convert_format.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/api/test_components/test_circ_pump_pressure.py` & `pandapipes-0.8.5/pandapipes/test/api/test_components/test_circ_pump_pressure.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/api/test_components/test_circ_pump_mass.py` & `pandapipes-0.8.5/pandapipes/test/api/test_components/test_circ_pump_mass.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/api/test_components/test_valve.py` & `pandapipes-0.8.5/pandapipes/test/api/test_components/test_valve.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/api/test_components/test_pump.py` & `pandapipes-0.8.5/pandapipes/test/api/test_components/test_pump.py`

 * *Files 10% similar despite different names*

```diff
@@ -187,9 +187,52 @@
                         mode="hydraulics", transient=False, nonlinear_method="automatic",
                         tol_p=1e-4, tol_v=1e-4, use_numba=use_numba)
 
     assert net.res_pump.deltap_bar.isin([0]).all()
     assert np.isclose(net.res_junction.loc[1, "p_bar"], net.res_junction.loc[2, "p_bar"])
 
 
+@pytest.mark.parametrize("use_numba", [True, False])
+def test_compression_power(use_numba):
+    # based on example by "oporras"
+    from pandapipes.component_models import R_UNIVERSAL
+    from pandapipes.idx_node import PAMB
+
+    height_asl_m = 2842
+    net = pandapipes.create_empty_network(fluid="methane")
+
+    j0 = pandapipes.create_junction(net, pn_bar=1.05, tfluid_k=293.15, height_m=height_asl_m)
+    j1 = pandapipes.create_junction(net, pn_bar=1.05, tfluid_k=293.15, height_m=height_asl_m)
+    j2 = pandapipes.create_junction(net, pn_bar=1.05, tfluid_k=293.15, height_m=height_asl_m+10)
+    j3 = pandapipes.create_junction(net, pn_bar=1.05, tfluid_k=293.15, height_m=height_asl_m+10)
+
+    _ = pandapipes.create_pipe_from_parameters(net, from_junction=j0, to_junction=j1, length_km=0.1,
+                                            diameter_m=0.05)
+    _ = pandapipes.create_pipe_from_parameters(net, from_junction=j2, to_junction=j3, length_km=0.5,
+                                            diameter_m=0.05)
+
+    _ = pandapipes.create_pump(net, from_junction=j1, to_junction=j2, std_type="P2", name="Pump1")
+
+    _ = pandapipes.create_ext_grid(net, junction=j0, p_bar=4, t_k=293.15)
+    _ = pandapipes.create_sink(net, junction=j3, mdot_kg_per_s=0.05)
+
+    pandapipes.pipeflow(net, use_numba=use_numba)
+
+    # Local ambiental (atmospheric) pressure
+    p_amb_bar_j1 = net["_pit"]['node'][1][PAMB]
+    p_amb_bar_j2 = net["_pit"]['node'][2][PAMB]
+
+    # Isentropic power for the compression
+    R_spec = R_UNIVERSAL * 1e3 / pandapipes.get_fluid(net).get_molar_mass()
+    cp = pandapipes.get_fluid(net).get_heat_capacity(293.15)
+    cv = cp - R_spec
+    k = cp/cv
+    pressure_ratio = ((net.res_pump.p_to_bar[0] + p_amb_bar_j2) /
+                      (net.res_pump.p_from_bar[0] + p_amb_bar_j1))
+    compr = pandapipes.get_fluid(net).get_compressibility(net.res_pump.p_from_bar[0] + + p_amb_bar_j1)
+    pow_pump_MW = (net.res_pump.mdot_from_kg_per_s[0] * (k / (k - 1)) * R_spec *
+                   compr * net.res_pump.t_from_k[0] * (pressure_ratio ** ((k - 1) / k) - 1) / 1e6)
+    assert np.isclose(pow_pump_MW[0], net.res_pump.compr_power_mw[0])
+
+
 if __name__ == '__main__':
     n = pytest.main(["test_pump.py"])
```

## Comparing `pandapipes-0.8.4/pandapipes/test/api/test_components/test_compressor.py` & `pandapipes-0.8.5/pandapipes/test/api/test_components/test_compressor.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/api/test_components/test_heat_exchanger.py` & `pandapipes-0.8.5/pandapipes/test/api/test_components/test_heat_exchanger.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/api/test_components/test_flow_control.py` & `pandapipes-0.8.5/pandapipes/test/api/test_components/test_flow_control.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/api/test_components/test_pipe_results.py` & `pandapipes-0.8.5/pandapipes/test/api/test_components/test_pipe_results.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/api/test_components/test_ext_grid.py` & `pandapipes-0.8.5/pandapipes/test/api/test_components/test_ext_grid.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/api/test_components/test_mass_storage.py` & `pandapipes-0.8.5/pandapipes/test/api/test_components/test_mass_storage.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/api/test_components/test_pressure_control.py` & `pandapipes-0.8.5/pandapipes/test/api/test_components/test_pressure_control.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.8.1_gas.json` & `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.1_gas.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.2.0.json` & `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.2.0.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.8.4_gas.json` & `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.4_gas.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.8.2_water.json` & `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.2_water.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.8.3_water.json` & `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.3_water.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.1.2.json` & `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.1.2.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.8.3_gas.json` & `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.3_gas.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.8.0_gas.json` & `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.0_gas.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.8.4_water.json` & `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.4_water.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.1.1.json` & `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.1.1.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.8.1_water.json` & `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.1_water.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.1.0.json` & `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.1.0.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.5.0.json` & `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.5.0.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.8.2_gas.json` & `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.2_gas.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.7.0.json` & `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.7.0.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.8.0_water.json` & `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.0_water.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.4.0.json` & `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.4.0.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/test/api/old_versions/example_0.6.0.json` & `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.6.0.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/converter/stanet/data_cleaning.py` & `pandapipes-0.8.5/pandapipes/converter/stanet/data_cleaning.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/converter/stanet/preparing_steps.py` & `pandapipes-0.8.5/pandapipes/converter/stanet/preparing_steps.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/converter/stanet/stanet2pandapipes.py` & `pandapipes-0.8.5/pandapipes/converter/stanet/stanet2pandapipes.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/converter/stanet/table_creation.py` & `pandapipes-0.8.5/pandapipes/converter/stanet/table_creation.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/converter/stanet/valve_pipe_component/valve_pipe_component.py` & `pandapipes-0.8.5/pandapipes/converter/stanet/valve_pipe_component/valve_pipe_component.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/converter/stanet/valve_pipe_component/valve_pipe_plotting.py` & `pandapipes-0.8.5/pandapipes/converter/stanet/valve_pipe_component/valve_pipe_plotting.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/converter/stanet/valve_pipe_component/create_valve_pipe.py` & `pandapipes-0.8.5/pandapipes/converter/stanet/valve_pipe_component/create_valve_pipe.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/control/run_control.py` & `pandapipes-0.8.5/pandapipes/control/run_control.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/simple_water_networks.py` & `pandapipes-0.8.5/pandapipes/networks/simple_water_networks.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/simple_heat_transfer_networks.py` & `pandapipes-0.8.5/pandapipes/networks/simple_heat_transfer_networks.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/simple_gas_networks.py` & `pandapipes-0.8.5/pandapipes/networks/simple_gas_networks.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/nw_aux.py` & `pandapipes-0.8.5/pandapipes/networks/nw_aux.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/gas_net_schutterwald_1bar.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/gas_net_schutterwald_1bar.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/two_pumps.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/two_pumps.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/two_pipes.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/two_pipes.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/strand_net.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/strand_net.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/cross_3ext.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/cross_3ext.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/combined_networks/versatility.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/combined_networks/versatility.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/combined_networks/mixed_net.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/combined_networks/mixed_net.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_2.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_2.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_3.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_3.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_1.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_1.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/t_cross/t_cross.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/t_cross/t_cross.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/t_cross/valves.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/t_cross/valves.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/delta.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/delta.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/pumps.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/pumps.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/two_valves.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/two_valves.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/heights.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/heights.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/two_pressure_junctions/two_pipes.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/two_pressure_junctions/two_pipes.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/delta.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/delta.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/t_cross.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/t_cross.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/delta_2sinks.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/delta_2sinks.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/one_source.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/one_source.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/one_pipe.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/one_pipe.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/two_pipes.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/two_pipes.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/section_variation.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/section_variation.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/heights.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/heights.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net_stanet_variation2.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net_stanet_variation2.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/two_pumps.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/two_pumps.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/two_pipes.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/two_pipes.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/cross_3ext.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/cross_3ext.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net_stanet_variation1.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net_stanet_variation1.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/combined_networks/versatility.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/combined_networks/versatility.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/combined_networks/mixed_net.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/combined_networks/mixed_net.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_2.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_2.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_3.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_3.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_1.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_1.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/t_cross/t_cross.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/t_cross/t_cross.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/t_cross/valves.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/t_cross/valves.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/delta.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/delta.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/one_valve_stanet.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/one_valve_stanet.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/pumps.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/pumps.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/two_valves.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/two_valves.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/heights.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/heights.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/two_pressure_junctions/two_pipes.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/two_pressure_junctions/two_pipes.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/two_pressure_junctions/one_pipe_stanet.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/two_pressure_junctions/one_pipe_stanet.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/two_pipes_PC.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/two_pipes_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/strand_net_N.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/strand_net_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/two_pipes_N.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/two_pipes_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/cross_PC.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/cross_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/pump_N.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/pump_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/strand_net_PC.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/strand_net_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/versatility_N.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/versatility_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/district_N.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/district_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/versatility_PC.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/versatility_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/district_PC.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/district_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_3_PC.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_3_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_3_N.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_3_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_1_PC.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_1_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_2_PC.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_2_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_2_N.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_2_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_1_N.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_1_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/t_cross/t_cross_N.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/t_cross/t_cross_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/t_cross/t_cross_PC.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/t_cross/t_cross_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/delta_N.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/delta_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/two_valves_PC.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/two_valves_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/two_valves_N.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/two_valves_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/pumps_N.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/pumps_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/two_pressure_junctions/two_pipes_PC.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/two_pressure_junctions/two_pipes_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/water_cases/two_pressure_junctions/two_pipes_N.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/two_pressure_junctions/two_pipes_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/two_pipes_PC.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/two_pipes_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/two_pipes_N.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/two_pipes_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/pump_N.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/pump_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/parallel_PC.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/parallel_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/parallel_N.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/parallel_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/versatility_PC.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/versatility_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_1_PC.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_1_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_2_PC.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_2_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_2_N.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_2_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_1_N.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_1_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross2_N.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross2_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross1_PC.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross1_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross2_PC.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross2_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross1_N.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross1_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/square_N.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/square_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/square_PC.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/square_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/two_valves_PC.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/two_valves_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/two_valves_N.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/two_valves_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/delta_PC.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/delta_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/pumps_N.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/pumps_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/two_pressure_junctions/H_net_N.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/two_pressure_junctions/H_net_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/stanet_test_networks/gas_cases/two_pressure_junctions/H_net_PC.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/two_pressure_junctions/H_net_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb4--0-no_sw.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb4--0-no_sw.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/1-LV-urban6--0-sw.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-urban6--0-sw.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural1--0-no_sw.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural1--0-no_sw.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural2--0-no_sw.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural2--0-no_sw.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural1--0-sw.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural1--0-sw.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural2--0-sw.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural2--0-sw.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural3--0-no_sw.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural3--0-no_sw.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb5--0-sw.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb5--0-sw.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural3--0-sw.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural3--0-sw.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb5--0-no_sw.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb5--0-no_sw.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/1-LV-urban6--0-no_sw.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-urban6--0-no_sw.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb4--0-sw.json` & `pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb4--0-sw.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/component_models/ext_grid_component.py` & `pandapipes-0.8.5/pandapipes/component_models/ext_grid_component.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/component_models/flow_control_component.py` & `pandapipes-0.8.5/pandapipes/component_models/flow_control_component.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/component_models/compressor_component.py` & `pandapipes-0.8.5/pandapipes/component_models/compressor_component.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/component_models/pipe_component.py` & `pandapipes-0.8.5/pandapipes/component_models/pipe_component.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/component_models/mass_storage_component.py` & `pandapipes-0.8.5/pandapipes/component_models/mass_storage_component.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/component_models/source_component.py` & `pandapipes-0.8.5/pandapipes/component_models/source_component.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/component_models/junction_component.py` & `pandapipes-0.8.5/pandapipes/component_models/junction_component.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/component_models/circulation_pump_mass_component.py` & `pandapipes-0.8.5/pandapipes/component_models/circulation_pump_mass_component.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/component_models/circulation_pump_pressure_component.py` & `pandapipes-0.8.5/pandapipes/component_models/circulation_pump_pressure_component.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/component_models/__init__.py` & `pandapipes-0.8.5/pandapipes/component_models/__init__.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/component_models/pressure_control_component.py` & `pandapipes-0.8.5/pandapipes/component_models/pressure_control_component.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/component_models/heat_exchanger_component.py` & `pandapipes-0.8.5/pandapipes/component_models/heat_exchanger_component.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/component_models/sink_component.py` & `pandapipes-0.8.5/pandapipes/component_models/sink_component.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/component_models/component_toolbox.py` & `pandapipes-0.8.5/pandapipes/component_models/component_toolbox.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/component_models/valve_component.py` & `pandapipes-0.8.5/pandapipes/component_models/valve_component.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/component_models/pump_component.py` & `pandapipes-0.8.5/pandapipes/component_models/pump_component.py`

 * *Files 3% similar despite different names*

```diff
@@ -144,33 +144,35 @@
             required_results.extend([("v_mean_m_per_s", "v_mps")])
 
         extract_branch_results_without_internals(net, branch_results, required_results,
                                                  cls.table_name(), branches_connected)
 
         if calc_compr_pow:
             f, t = get_lookup(net, "branch", "from_to")[cls.table_name()]
+            from_nodes = branch_results["from_nodes"][f:t]
+
             res_table = net["res_" + cls.table_name()]
             if net.fluid.is_gas:
-                p_from = branch_results["p_from"][f:t]
-                p_to = branch_results["p_to"][f:t]
-                from_nodes = branch_results["from_nodes"][f:t]
+                p_from = branch_results["p_abs_from"][f:t]
+                p_to = branch_results["p_abs_to"][f:t]
                 t0 = net["_pit"]["node"][from_nodes, TINIT_NODE]
                 mf_sum_int = branch_results["mf_from"][f:t]
                 # calculate ideal compression power
                 compr = get_fluid(net).get_property("compressibility", p_from)
                 try:
                     molar_mass = net.fluid.get_molar_mass()  # [g/mol]
                 except UserWarning:
                     logger.error('Molar mass is missing in your fluid. Before you are able to '
                                  'retrieve the compression power make sure that the molar mass is'
                                  ' defined')
                 else:
                     r_spec = 1e3 * R_UNIVERSAL / molar_mass  # [J/(kg * K)]
-                    # 'kappa' heat capacity ratio:
-                    k = 1.4  # TODO: implement proper calculation of kappa
+                    cp = net.fluid.get_heat_capacity(t0)
+                    cv = cp - r_spec
+                    k = cp/cv  # 'kappa' heat capacity ratio
                     w_real_isentr = (k / (k - 1)) * r_spec * compr * t0 * \
                                     (np.divide(p_to, p_from) ** ((k - 1) / k) - 1)
                     res_table['compr_power_mw'].values[:] = \
                         w_real_isentr * np.abs(mf_sum_int) / 10 ** 6
             else:
                 vf_sum_int = branch_results["vf"][f:t]
                 pl = branch_results["pl"][f:t]
```

## Comparing `pandapipes-0.8.4/pandapipes/component_models/abstract_models/branch_wo_internals_models.py` & `pandapipes-0.8.5/pandapipes/component_models/abstract_models/branch_wo_internals_models.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/component_models/abstract_models/branch_models.py` & `pandapipes-0.8.5/pandapipes/component_models/abstract_models/branch_models.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/component_models/abstract_models/branch_wzerolength_models.py` & `pandapipes-0.8.5/pandapipes/component_models/abstract_models/branch_wzerolength_models.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/component_models/abstract_models/const_flow_models.py` & `pandapipes-0.8.5/pandapipes/component_models/abstract_models/const_flow_models.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/component_models/abstract_models/base_component.py` & `pandapipes-0.8.5/pandapipes/component_models/abstract_models/base_component.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/component_models/abstract_models/__init__.py` & `pandapipes-0.8.5/pandapipes/component_models/abstract_models/__init__.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/component_models/abstract_models/circulation_pump.py` & `pandapipes-0.8.5/pandapipes/component_models/abstract_models/circulation_pump.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/component_models/abstract_models/node_element_models.py` & `pandapipes-0.8.5/pandapipes/component_models/abstract_models/node_element_models.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/component_models/abstract_models/node_models.py` & `pandapipes-0.8.5/pandapipes/component_models/abstract_models/node_models.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/component_models/abstract_models/branch_w_internals_models.py` & `pandapipes-0.8.5/pandapipes/component_models/abstract_models/branch_w_internals_models.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/topology/graph_searches.py` & `pandapipes-0.8.5/pandapipes/topology/graph_searches.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/topology/create_graph.py` & `pandapipes-0.8.5/pandapipes/topology/create_graph.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/multinet/multinet.py` & `pandapipes-0.8.5/pandapipes/multinet/multinet.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/multinet/create_multinet.py` & `pandapipes-0.8.5/pandapipes/multinet/create_multinet.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/multinet/__init__.py` & `pandapipes-0.8.5/pandapipes/multinet/__init__.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/multinet/timeseries/run_time_series_multinet.py` & `pandapipes-0.8.5/pandapipes/multinet/timeseries/run_time_series_multinet.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/multinet/control/run_control_multinet.py` & `pandapipes-0.8.5/pandapipes/multinet/control/run_control_multinet.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/multinet/control/controller/multinet_control.py` & `pandapipes-0.8.5/pandapipes/multinet/control/controller/multinet_control.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/properties/properties_toolbox.py` & `pandapipes-0.8.5/pandapipes/properties/properties_toolbox.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/properties/fluids.py` & `pandapipes-0.8.5/pandapipes/properties/fluids.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/properties/hydrogen/heat_capacity.txt` & `pandapipes-0.8.5/pandapipes/properties/hydrogen/heat_capacity.txt`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/properties/hydrogen/viscosity.txt` & `pandapipes-0.8.5/pandapipes/properties/hydrogen/viscosity.txt`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/properties/hydrogen/density.txt` & `pandapipes-0.8.5/pandapipes/properties/hydrogen/density.txt`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/properties/nitrogen/heat_capacity.txt` & `pandapipes-0.8.5/pandapipes/properties/nitrogen/heat_capacity.txt`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/properties/nitrogen/viscosity.txt` & `pandapipes-0.8.5/pandapipes/properties/nitrogen/viscosity.txt`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/properties/nitrogen/density.txt` & `pandapipes-0.8.5/pandapipes/properties/nitrogen/density.txt`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/properties/oxygen/heat_capacity.txt` & `pandapipes-0.8.5/pandapipes/properties/oxygen/heat_capacity.txt`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/properties/oxygen/viscosity.txt` & `pandapipes-0.8.5/pandapipes/properties/oxygen/viscosity.txt`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/properties/oxygen/density.txt` & `pandapipes-0.8.5/pandapipes/properties/oxygen/density.txt`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/plotting/simple_plot.py` & `pandapipes-0.8.5/pandapipes/plotting/simple_plot.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/plotting/generic_geodata.py` & `pandapipes-0.8.5/pandapipes/plotting/generic_geodata.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,17 +35,17 @@
     :Example:
         graph, meshed, roots = build_igraph_from_pp(net)
     """
 
     try:
         import igraph as ig
     except (DeprecationWarning, ImportError):
-        raise ImportError("Please install python-igraph with "
-                          "`pip install python-igraph` or "
-                          "`conda install python-igraph` "
+        raise ImportError("Please install igraph with "
+                          "`pip install igraph` or "
+                          "`conda install igraph` "
                           "or from https://www.lfd.uci.edu/~gohlke/pythonlibs")
     g = ig.Graph(directed=True)
     junction_index = net.junction.index if junctions is None else np.array(junctions)
     nr_junctions = len(junction_index)
     g.add_vertices(nr_junctions)
     g.vs["label"] = list(junction_index)
     pp_junction_mapping = dict(list(zip(junction_index, list(range(nr_junctions)))))
```

## Comparing `pandapipes-0.8.4/pandapipes/plotting/geo.py` & `pandapipes-0.8.5/pandapipes/plotting/geo.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/plotting/pipeflow_results.py` & `pandapipes-0.8.5/pandapipes/plotting/pipeflow_results.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/plotting/__init__.py` & `pandapipes-0.8.5/pandapipes/plotting/__init__.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/plotting/patch_makers.py` & `pandapipes-0.8.5/pandapipes/plotting/patch_makers.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/plotting/plotting_toolbox.py` & `pandapipes-0.8.5/pandapipes/plotting/plotting_toolbox.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.4/pandapipes/plotting/collections.py` & `pandapipes-0.8.5/pandapipes/plotting/collections.py`

 * *Files identical despite different names*

