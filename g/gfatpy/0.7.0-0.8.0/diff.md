# Comparing `tmp/gfatpy-0.7.0.tar.gz` & `tmp/gfatpy-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gfatpy-0.7.0.tar", max compression
+gzip compressed data, was "gfatpy-0.8.0.tar", max compression
```

## Comparing `gfatpy-0.7.0.tar` & `gfatpy-0.8.0.tar`

### file list

```diff
@@ -1,113 +1,117 @@
--rw-r--r--   0        0        0     2288 2023-07-26 00:42:04.237764 gfatpy-0.7.0/gfatpy/__init__.py
--rw-r--r--   0        0        0     1077 2023-07-26 00:42:04.238767 gfatpy-0.7.0/gfatpy/aeronet/__init__.py
--rw-r--r--   0        0        0      710 2023-07-26 00:42:04.239769 gfatpy-0.7.0/gfatpy/aeronet/aeronet4lidar.py
--rw-r--r--   0        0        0     1053 2023-07-26 00:42:04.240767 gfatpy-0.7.0/gfatpy/aeronet/info.yml
--rw-r--r--   0        0        0    18417 2023-07-26 00:42:04.241770 gfatpy-0.7.0/gfatpy/aeronet/plot.py
--rw-r--r--   0        0        0     4040 2023-07-26 00:42:04.242282 gfatpy-0.7.0/gfatpy/aeronet/reader.py
--rw-r--r--   0        0        0     8855 2023-07-26 00:42:04.242282 gfatpy-0.7.0/gfatpy/aeronet/typing.py
--rw-r--r--   0        0        0    16725 2023-07-26 00:42:04.243852 gfatpy-0.7.0/gfatpy/aeronet/utils.py
--rw-r--r--   0        0        0    28725 2023-07-26 00:42:04.245810 gfatpy-0.7.0/gfatpy/assets/LOGO_GFAT_150pp.png
--rw-r--r--   0        0        0        0 2023-07-26 00:42:04.246811 gfatpy-0.7.0/gfatpy/atmo/__init__.py
--rw-r--r--   0        0        0    21888 2023-07-26 00:42:04.247809 gfatpy-0.7.0/gfatpy/atmo/atmo.py
--rw-r--r--   0        0        0     7262 2023-07-26 00:42:04.247809 gfatpy-0.7.0/gfatpy/atmo/ecmwf.py
--rw-r--r--   0        0        0    74896 2023-07-26 00:42:04.251827 gfatpy-0.7.0/gfatpy/atmo/solar.py
--rw-r--r--   0        0        0     4471 2023-07-26 00:42:04.253358 gfatpy-0.7.0/gfatpy/cli/lidar/main.py
--rw-r--r--   0        0        0     1183 2023-07-26 00:42:04.255406 gfatpy-0.7.0/gfatpy/cli/lidar/plot/main.py
--rw-r--r--   0        0        0      896 2023-07-26 00:42:04.256623 gfatpy-0.7.0/gfatpy/cli/main.py
--rw-r--r--   0        0        0      270 2023-07-26 00:42:04.257857 gfatpy-0.7.0/gfatpy/cloudnet/__init__.py
--rw-r--r--   0        0        0     8870 2023-07-26 00:42:04.258890 gfatpy-0.7.0/gfatpy/cloudnet/cloud_model.py
--rw-r--r--   0        0        0       49 2023-07-26 00:42:04.259913 gfatpy-0.7.0/gfatpy/cloudnet/info.yml
--rw-r--r--   0        0        0     4600 2023-07-26 00:42:04.259913 gfatpy-0.7.0/gfatpy/cloudnet/plot_deprecated.py
--rw-r--r--   0        0        0     5423 2023-07-26 00:42:04.260928 gfatpy-0.7.0/gfatpy/cloudnet/reader.py
--rw-r--r--   0        0        0    18077 2023-07-26 00:42:04.261931 gfatpy-0.7.0/gfatpy/cloudnet/utils.py
--rw-r--r--   0        0        0      237 2023-07-26 00:42:04.262874 gfatpy-0.7.0/gfatpy/config.py
--rw-r--r--   0        0        0      342 2023-07-26 00:42:04.262874 gfatpy-0.7.0/gfatpy/lidar/__init__.py
--rw-r--r--   0        0        0    14442 2023-07-26 00:42:04.320876 gfatpy-0.7.0/gfatpy/lidar/depolarization/calibration.py
--rw-r--r--   0        0        0     1463 2023-07-26 00:42:04.322070 gfatpy-0.7.0/gfatpy/lidar/depolarization/depolarization_calibration_alh.py
--rw-r--r--   0        0        0     9744 2023-07-26 00:42:04.322070 gfatpy-0.7.0/gfatpy/lidar/depolarization/depolarization_calibration_mhc.py
--rw-r--r--   0        0        0      913 2023-07-26 00:42:04.323346 gfatpy-0.7.0/gfatpy/lidar/depolarization/depolarization_calibration_vlt.py
--rw-r--r--   0        0        0      174 2023-07-26 00:42:04.265150 gfatpy-0.7.0/gfatpy/lidar/depolarization/GHK/.hg_archival.txt
--rw-r--r--   0        0        0      121 2023-07-26 00:42:04.266153 gfatpy-0.7.0/gfatpy/lidar/depolarization/GHK/.hgignore
--rw-r--r--   0        0        0      570 2023-07-26 00:42:04.266153 gfatpy-0.7.0/gfatpy/lidar/depolarization/GHK/.hgtags
--rw-r--r--   0        0        0  2508885 2023-07-26 00:42:04.294151 gfatpy-0.7.0/gfatpy/lidar/depolarization/GHK/About the effects of polarising optics_4b_1L_corr.pdf
--rw-r--r--   0        0        0     2541 2023-07-26 00:42:04.295148 gfatpy-0.7.0/gfatpy/lidar/depolarization/GHK/CHANGELOG.md
--rw-r--r--   0        0        0   179791 2023-07-26 00:42:04.298390 gfatpy-0.7.0/gfatpy/lidar/depolarization/GHK/GHK_0.9.8h_Py3.7.py
--rw-r--r--   0        0        0   793573 2023-07-26 00:42:04.309996 gfatpy-0.7.0/gfatpy/lidar/depolarization/GHK/Improvements_of_the_GHK_script_200529.pdf
--rw-r--r--   0        0        0    13468 2023-07-26 00:42:04.310994 gfatpy-0.7.0/gfatpy/lidar/depolarization/GHK/LICENSE.md
--rw-r--r--   0        0        0     1628 2023-07-26 00:42:04.311993 gfatpy-0.7.0/gfatpy/lidar/depolarization/GHK/README.md
--rw-r--r--   0        0        0      108 2023-07-26 00:42:04.311993 gfatpy-0.7.0/gfatpy/lidar/depolarization/GHK/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-26 00:42:04.313446 gfatpy-0.7.0/gfatpy/lidar/depolarization/GHK/system_settings/__init__.py
--rw-r--r--   0        0        0     7453 2023-07-26 00:42:04.314465 gfatpy-0.7.0/gfatpy/lidar/depolarization/GHK/system_settings/mulhacen_polarizer_template.py
--rw-r--r--   0        0        0     7455 2023-07-26 00:42:04.315468 gfatpy-0.7.0/gfatpy/lidar/depolarization/GHK/system_settings/mulhacen_rotator_casoG_template.py
--rw-r--r--   0        0        0     7390 2023-07-26 00:42:04.316468 gfatpy-0.7.0/gfatpy/lidar/depolarization/GHK/system_settings/mulhacen_run.py
--rw-r--r--   0        0        0    11034 2023-07-26 00:42:04.317466 gfatpy-0.7.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_0.9.8e4-PollyXT_Lacros.py
--rw-r--r--   0        0        0    10931 2023-07-26 00:42:04.317466 gfatpy-0.7.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_0.9.8h-PollyXT_Cyprus_532_210429_vf_4.py
--rw-r--r--   0        0        0    11059 2023-07-26 00:42:04.318466 gfatpy-0.7.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_mhc_pol_532x_20130101.py
--rw-r--r--   0        0        0    11059 2023-07-26 00:42:04.319464 gfatpy-0.7.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_mhc_rot_532x_20130101.py
--rw-r--r--   0        0        0    11059 2023-07-26 00:42:04.319464 gfatpy-0.7.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_mhc_rot_532x_20220614.py
--rw-r--r--   0        0        0     2533 2023-07-26 00:42:04.264135 gfatpy-0.7.0/gfatpy/lidar/depolarization/GHK.py
--rw-r--r--   0        0        0     1506 2023-07-26 00:42:04.323346 gfatpy-0.7.0/gfatpy/lidar/depolarization/io.py
--rw-r--r--   0        0        0     6044 2023-07-26 00:42:04.324365 gfatpy-0.7.0/gfatpy/lidar/depolarization/plot.py
--rw-r--r--   0        0        0    11856 2023-07-26 00:42:04.325369 gfatpy-0.7.0/gfatpy/lidar/depolarization/retrieval.py
--rw-r--r--   0        0        0     1429 2023-07-26 00:42:04.325369 gfatpy-0.7.0/gfatpy/lidar/depolarization/utils.py
--rw-r--r--   0        0        0     9911 2023-07-26 00:42:04.326369 gfatpy-0.7.0/gfatpy/lidar/file_manager.py
--rw-r--r--   0        0        0     5121 2023-07-26 00:42:04.327360 gfatpy-0.7.0/gfatpy/lidar/info.yml
--rw-r--r--   0        0        0     4072 2023-07-26 00:42:04.328436 gfatpy-0.7.0/gfatpy/lidar/nc_convert/configs/ALHAMBRA.toml
--rw-r--r--   0        0        0      920 2023-07-26 00:42:04.328436 gfatpy-0.7.0/gfatpy/lidar/nc_convert/configs/MULHACEN.toml
--rw-r--r--   0        0        0    12702 2023-07-26 00:42:04.329931 gfatpy-0.7.0/gfatpy/lidar/nc_convert/converter.py
--rw-r--r--   0        0        0      244 2023-07-26 00:42:04.329931 gfatpy-0.7.0/gfatpy/lidar/nc_convert/types.py
--rw-r--r--   0        0        0     2042 2023-07-26 00:42:04.331057 gfatpy-0.7.0/gfatpy/lidar/plot/info.yml
--rw-r--r--   0        0        0      168 2023-07-26 00:42:04.331057 gfatpy-0.7.0/gfatpy/lidar/plot/profile.py
--rw-r--r--   0        0        0     3442 2023-07-26 00:42:04.332078 gfatpy-0.7.0/gfatpy/lidar/plot/quicklook.py
--rw-r--r--   0        0        0     2299 2023-07-26 00:42:04.332141 gfatpy-0.7.0/gfatpy/lidar/preprocessing/__init__.py
--rw-r--r--   0        0        0     1931 2023-07-26 00:42:04.332141 gfatpy-0.7.0/gfatpy/lidar/preprocessing/gluing_de_la_rosa.py
--rw-r--r--   0        0        0     3364 2023-07-26 00:42:04.333455 gfatpy-0.7.0/gfatpy/lidar/preprocessing/gluing_de_la_rosa_slope.py
--rw-r--r--   0        0        0     2639 2023-07-26 00:42:04.334556 gfatpy-0.7.0/gfatpy/lidar/preprocessing/gluing_proportional.py
--rw-r--r--   0        0        0       26 2023-07-26 00:42:04.334556 gfatpy-0.7.0/gfatpy/lidar/preprocessing/lidar_dead_time.py
--rw-r--r--   0        0        0     2958 2023-07-26 00:42:04.335813 gfatpy-0.7.0/gfatpy/lidar/preprocessing/lidar_gluing_bravo_aranda.py
--rw-r--r--   0        0        0    21478 2023-07-26 00:42:04.337477 gfatpy-0.7.0/gfatpy/lidar/preprocessing/lidar_gluing_damico.py
--rw-r--r--   0        0        0     3626 2023-07-26 00:42:04.338493 gfatpy-0.7.0/gfatpy/lidar/preprocessing/lidar_linear_response_region.py
--rw-r--r--   0        0        0    17135 2023-07-26 00:42:04.339493 gfatpy-0.7.0/gfatpy/lidar/preprocessing/lidar_preprocessing.py
--rw-r--r--   0        0        0    14976 2023-07-26 00:42:04.340493 gfatpy-0.7.0/gfatpy/lidar/preprocessing/lidar_preprocessing_tools.py
--rw-r--r--   0        0        0    38037 2023-07-26 00:42:04.340493 gfatpy-0.7.0/gfatpy/lidar/preprocessing/study_dead_time.py
--rw-r--r--   0        0        0     1064 2023-07-26 00:42:04.342018 gfatpy-0.7.0/gfatpy/lidar/quality_assurance/common.py
--rw-r--r--   0        0        0        0 2023-07-26 00:42:04.342018 gfatpy-0.7.0/gfatpy/lidar/quality_assurance/dark_measurement.py
--rw-r--r--   0        0        0     5097 2023-07-26 00:42:04.343034 gfatpy-0.7.0/gfatpy/lidar/quality_assurance/io.py
--rw-r--r--   0        0        0     8242 2023-07-26 00:42:04.344031 gfatpy-0.7.0/gfatpy/lidar/quality_assurance/overlap.py
--rw-r--r--   0        0        0    10544 2023-07-26 00:42:04.344543 gfatpy-0.7.0/gfatpy/lidar/quality_assurance/plot.py
--rw-r--r--   0        0        0    10162 2023-07-26 00:42:04.345555 gfatpy-0.7.0/gfatpy/lidar/quality_assurance/rayleigh_fit.py
--rw-r--r--   0        0        0     8044 2023-07-26 00:42:04.346555 gfatpy-0.7.0/gfatpy/lidar/quality_assurance/telecover.py
--rw-r--r--   0        0        0    10850 2023-07-26 00:42:04.346555 gfatpy-0.7.0/gfatpy/lidar/reader.py
--rw-r--r--   0        0        0        0 2023-07-26 00:42:04.347559 gfatpy-0.7.0/gfatpy/lidar/retrieval/__init__.py
--rw-r--r--   0        0        0     3563 2023-07-26 00:42:04.348558 gfatpy-0.7.0/gfatpy/lidar/retrieval/helper.py
--rw-r--r--   0        0        0     6175 2023-07-26 00:42:04.348558 gfatpy-0.7.0/gfatpy/lidar/retrieval/klett.py
--rw-r--r--   0        0        0     5145 2023-07-26 00:42:04.349558 gfatpy-0.7.0/gfatpy/lidar/retrieval/lidar_layer_detection.py
--rw-r--r--   0        0        0        0 2023-07-26 00:42:04.349558 gfatpy-0.7.0/gfatpy/lidar/retrieval/number_concentration.py
--rw-r--r--   0        0        0     7009 2023-07-26 00:42:04.350559 gfatpy-0.7.0/gfatpy/lidar/retrieval/raman.py
--rw-r--r--   0        0        0     8196 2023-07-26 00:42:04.352083 gfatpy-0.7.0/gfatpy/lidar/retrieval/synthetic/generator.py
--rw-r--r--   0        0        0     2151 2023-07-26 00:42:04.352083 gfatpy-0.7.0/gfatpy/lidar/types.py
--rw-r--r--   0        0        0     6247 2023-07-26 00:42:04.353341 gfatpy-0.7.0/gfatpy/lidar/utils.py
--rw-r--r--   0        0        0      244 2023-07-26 00:42:04.354361 gfatpy-0.7.0/gfatpy/radar/__init__.py
--rw-r--r--   0        0        0      101 2023-07-26 00:42:04.355363 gfatpy-0.7.0/gfatpy/radar/info.yml
--rw-r--r--   0        0        0        0 2023-07-26 00:42:04.355363 gfatpy-0.7.0/gfatpy/radar/plot/info.yml
--rw-r--r--   0        0        0     2225 2023-07-26 00:42:04.356356 gfatpy-0.7.0/gfatpy/radar/reader.py
--rw-r--r--   0        0        0    61357 2023-07-26 00:42:04.357461 gfatpy-0.7.0/gfatpy/radar/scattering_databases/0.C_24.1GHz.csv
--rw-r--r--   0        0        0    61200 2023-07-26 00:42:04.358680 gfatpy-0.7.0/gfatpy/radar/scattering_databases/0.C_35.5GHz.csv
--rw-r--r--   0        0        0    60964 2023-07-26 00:42:04.359198 gfatpy-0.7.0/gfatpy/radar/scattering_databases/0.C_94.0GHz.csv
--rw-r--r--   0        0        0    61372 2023-07-26 00:42:04.360408 gfatpy-0.7.0/gfatpy/radar/scattering_databases/10C_24.1GHz.csv
--rw-r--r--   0        0        0    61213 2023-07-26 00:42:04.361921 gfatpy-0.7.0/gfatpy/radar/scattering_databases/10C_35.5GHz.csv
--rw-r--r--   0        0        0    60965 2023-07-26 00:42:04.362939 gfatpy-0.7.0/gfatpy/radar/scattering_databases/10C_94.0GHz.csv
--rw-r--r--   0        0        0    60528 2023-07-26 00:42:04.363937 gfatpy-0.7.0/gfatpy/radar/scattering_databases/20C_24.1GHz.csv
--rw-r--r--   0        0        0    61215 2023-07-26 00:42:04.365127 gfatpy-0.7.0/gfatpy/radar/scattering_databases/20C_35.5GHz.csv
--rw-r--r--   0        0        0    60984 2023-07-26 00:42:04.366482 gfatpy-0.7.0/gfatpy/radar/scattering_databases/20C_94.0GHz.csv
--rw-r--r--   0        0        0     1305 2023-07-26 00:42:04.367524 gfatpy-0.7.0/gfatpy/radar/types.py
--rw-r--r--   0        0        0     5853 2023-07-26 00:42:04.368542 gfatpy-0.7.0/gfatpy/radar/utils.py
--rw-r--r--   0        0        0       34 2023-07-26 00:42:04.369846 gfatpy-0.7.0/gfatpy/utils/__init__.py
--rw-r--r--   0        0        0     9655 2023-07-26 00:42:04.372402 gfatpy-0.7.0/gfatpy/utils/calibration.py
--rw-r--r--   0        0        0     3468 2023-07-26 00:42:04.373419 gfatpy-0.7.0/gfatpy/utils/io.py
--rw-r--r--   0        0        0     2870 2023-07-26 00:42:04.373419 gfatpy-0.7.0/gfatpy/utils/optimized.py
--rw-r--r--   0        0        0     6664 2023-07-26 00:42:04.374433 gfatpy-0.7.0/gfatpy/utils/plot.py
--rw-r--r--   0        0        0    13283 2023-07-26 00:42:04.375432 gfatpy-0.7.0/gfatpy/utils/utils.py
--rw-r--r--   0        0        0     1470 2023-07-26 00:42:04.236766 gfatpy-0.7.0/LICENSE
--rw-r--r--   0        0        0     1535 2023-07-26 02:55:08.098691 gfatpy-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     1466 1970-01-01 00:00:00.000000 gfatpy-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1470 2023-01-19 15:14:33.615682 gfatpy-0.8.0/LICENSE
+-rw-r--r--   0        0        0     2288 2023-07-25 03:08:40.486165 gfatpy-0.8.0/gfatpy/__init__.py
+-rw-r--r--   0        0        0     1077 2023-01-19 15:14:33.615682 gfatpy-0.8.0/gfatpy/aeronet/__init__.py
+-rw-r--r--   0        0        0      710 2023-01-19 15:14:33.615682 gfatpy-0.8.0/gfatpy/aeronet/aeronet4lidar.py
+-rw-r--r--   0        0        0     1053 2023-01-19 15:14:33.615682 gfatpy-0.8.0/gfatpy/aeronet/info.yml
+-rw-r--r--   0        0        0    18417 2023-07-25 03:08:40.486165 gfatpy-0.8.0/gfatpy/aeronet/plot.py
+-rw-r--r--   0        0        0     4040 2023-07-25 03:08:40.486165 gfatpy-0.8.0/gfatpy/aeronet/reader.py
+-rw-r--r--   0        0        0     8855 2023-07-25 03:08:40.486165 gfatpy-0.8.0/gfatpy/aeronet/typing.py
+-rw-r--r--   0        0        0    16725 2023-07-25 03:08:40.486165 gfatpy-0.8.0/gfatpy/aeronet/utils.py
+-rw-r--r--   0        0        0    28725 2023-01-19 15:14:33.615682 gfatpy-0.8.0/gfatpy/assets/LOGO_GFAT_150pp.png
+-rw-r--r--   0        0        0        0 2023-01-19 15:14:33.615682 gfatpy-0.8.0/gfatpy/atmo/__init__.py
+-rw-r--r--   0        0        0    21888 2023-07-25 03:08:40.486165 gfatpy-0.8.0/gfatpy/atmo/atmo.py
+-rw-r--r--   0        0        0     7262 2023-07-25 03:08:40.486165 gfatpy-0.8.0/gfatpy/atmo/ecmwf.py
+-rw-r--r--   0        0        0    74896 2023-01-19 15:14:33.615682 gfatpy-0.8.0/gfatpy/atmo/solar.py
+-rw-r--r--   0        0        0     4471 2023-07-25 03:08:40.486165 gfatpy-0.8.0/gfatpy/cli/lidar/main.py
+-rw-r--r--   0        0        0     1183 2023-01-19 15:14:33.615682 gfatpy-0.8.0/gfatpy/cli/lidar/plot/main.py
+-rw-r--r--   0        0        0      896 2023-01-19 15:14:33.615682 gfatpy-0.8.0/gfatpy/cli/main.py
+-rw-r--r--   0        0        0      270 2023-01-19 15:14:33.615682 gfatpy-0.8.0/gfatpy/cloudnet/__init__.py
+-rw-r--r--   0        0        0     8870 2023-07-25 03:08:40.486165 gfatpy-0.8.0/gfatpy/cloudnet/cloud_model.py
+-rw-r--r--   0        0        0       49 2023-01-19 15:14:33.615682 gfatpy-0.8.0/gfatpy/cloudnet/info.yml
+-rw-r--r--   0        0        0     4600 2023-01-19 15:14:33.615682 gfatpy-0.8.0/gfatpy/cloudnet/plot_deprecated.py
+-rw-r--r--   0        0        0     5423 2023-01-19 15:14:33.615682 gfatpy-0.8.0/gfatpy/cloudnet/reader.py
+-rw-r--r--   0        0        0    18077 2023-07-25 03:08:40.486165 gfatpy-0.8.0/gfatpy/cloudnet/utils.py
+-rw-r--r--   0        0        0      237 2023-07-25 03:08:40.486165 gfatpy-0.8.0/gfatpy/config.py
+-rw-r--r--   0        0        0      342 2023-07-25 03:08:40.486165 gfatpy-0.8.0/gfatpy/lidar/__init__.py
+-rw-r--r--   0        0        0      174 2023-01-19 15:14:33.615682 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/.hg_archival.txt
+-rw-r--r--   0        0        0      121 2023-01-19 15:14:33.615682 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/.hgignore
+-rw-r--r--   0        0        0      570 2023-01-19 15:14:33.615682 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/.hgtags
+-rw-r--r--   0        0        0  2508885 2023-01-19 15:14:33.625682 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/About the effects of polarising optics_4b_1L_corr.pdf
+-rw-r--r--   0        0        0     2541 2023-01-19 15:14:33.625682 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/CHANGELOG.md
+-rw-r--r--   0        0        0   179791 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/GHK_0.9.8h_Py3.7.py
+-rw-r--r--   0        0        0   793573 2023-01-19 15:14:33.625682 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/Improvements_of_the_GHK_script_200529.pdf
+-rw-r--r--   0        0        0    13468 2023-01-19 15:14:33.625682 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/LICENSE.md
+-rw-r--r--   0        0        0     1628 2023-01-19 15:14:33.625682 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/README.md
+-rw-r--r--   0        0        0      108 2023-01-19 15:14:33.625682 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/requirements.txt
+-rw-r--r--   0        0        0        0 2023-01-19 15:14:33.625682 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/system_settings/__init__.py
+-rw-r--r--   0        0        0     7453 2023-04-18 20:55:26.084565 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/system_settings/mulhacen_polarizer_template.py
+-rw-r--r--   0        0        0     7455 2023-04-18 20:55:26.084565 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/system_settings/mulhacen_rotator_casoG_template.py
+-rw-r--r--   0        0        0     7390 2023-04-18 20:55:26.084565 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/system_settings/mulhacen_run.py
+-rw-r--r--   0        0        0    11034 2023-04-18 20:55:26.084565 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_0.9.8e4-PollyXT_Lacros.py
+-rw-r--r--   0        0        0    10931 2023-04-18 20:55:26.084565 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_0.9.8h-PollyXT_Cyprus_532_210429_vf_4.py
+-rw-r--r--   0        0        0    11059 2023-01-19 15:14:33.625682 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_mhc_pol_532x_20130101.py
+-rw-r--r--   0        0        0    11059 2023-01-19 15:14:33.625682 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_mhc_rot_532x_20130101.py
+-rw-r--r--   0        0        0    11059 2023-01-19 15:14:33.625682 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_mhc_rot_532x_20220614.py
+-rw-r--r--   0        0        0     2533 2023-07-25 03:08:40.486165 gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK.py
+-rw-r--r--   0        0        0    14442 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/depolarization/calibration.py
+-rw-r--r--   0        0        0     1463 2023-04-01 21:13:27.762405 gfatpy-0.8.0/gfatpy/lidar/depolarization/depolarization_calibration_alh.py
+-rw-r--r--   0        0        0     9744 2023-04-01 21:13:27.762405 gfatpy-0.8.0/gfatpy/lidar/depolarization/depolarization_calibration_mhc.py
+-rw-r--r--   0        0        0      913 2023-04-01 21:13:27.762405 gfatpy-0.8.0/gfatpy/lidar/depolarization/depolarization_calibration_vlt.py
+-rw-r--r--   0        0        0     1506 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/depolarization/io.py
+-rw-r--r--   0        0        0     6044 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/depolarization/plot.py
+-rw-r--r--   0        0        0    11856 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/depolarization/retrieval.py
+-rw-r--r--   0        0        0     1429 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/depolarization/utils.py
+-rw-r--r--   0        0        0     9911 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/file_manager.py
+-rw-r--r--   0        0        0     5121 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/info.yml
+-rw-r--r--   0        0        0     4072 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/nc_convert/configs/ALHAMBRA.toml
+-rw-r--r--   0        0        0      920 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/nc_convert/configs/MULHACEN.toml
+-rw-r--r--   0        0        0    12676 2023-07-31 14:23:15.575739 gfatpy-0.8.0/gfatpy/lidar/nc_convert/converter.py
+-rw-r--r--   0        0        0      244 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/nc_convert/types.py
+-rw-r--r--   0        0        0     2042 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/plot/info.yml
+-rw-r--r--   0        0        0      168 2023-01-19 15:14:33.625682 gfatpy-0.8.0/gfatpy/lidar/plot/profile.py
+-rw-r--r--   0        0        0     3442 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/plot/quicklook.py
+-rw-r--r--   0        0        0     2299 2023-01-19 15:14:33.625682 gfatpy-0.8.0/gfatpy/lidar/preprocessing/__init__.py
+-rw-r--r--   0        0        0     1931 2023-01-19 15:14:33.625682 gfatpy-0.8.0/gfatpy/lidar/preprocessing/gluing_de_la_rosa.py
+-rw-r--r--   0        0        0     3364 2023-01-19 15:14:33.625682 gfatpy-0.8.0/gfatpy/lidar/preprocessing/gluing_de_la_rosa_slope.py
+-rw-r--r--   0        0        0     2639 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/preprocessing/gluing_proportional.py
+-rw-r--r--   0        0        0       26 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/preprocessing/lidar_dead_time.py
+-rw-r--r--   0        0        0     2958 2023-01-19 15:14:33.625682 gfatpy-0.8.0/gfatpy/lidar/preprocessing/lidar_gluing_bravo_aranda.py
+-rw-r--r--   0        0        0    21478 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/preprocessing/lidar_gluing_damico.py
+-rw-r--r--   0        0        0     3626 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/preprocessing/lidar_linear_response_region.py
+-rw-r--r--   0        0        0    17135 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/preprocessing/lidar_preprocessing.py
+-rw-r--r--   0        0        0    14976 2023-01-19 15:14:33.625682 gfatpy-0.8.0/gfatpy/lidar/preprocessing/lidar_preprocessing_tools.py
+-rw-r--r--   0        0        0    38037 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/preprocessing/study_dead_time.py
+-rw-r--r--   0        0        0     1064 2023-01-19 15:14:33.625682 gfatpy-0.8.0/gfatpy/lidar/quality_assurance/common.py
+-rw-r--r--   0        0        0        0 2023-01-19 15:14:33.625682 gfatpy-0.8.0/gfatpy/lidar/quality_assurance/dark_measurement.py
+-rw-r--r--   0        0        0     5097 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/quality_assurance/io.py
+-rw-r--r--   0        0        0     8242 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/quality_assurance/overlap.py
+-rw-r--r--   0        0        0    10544 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/quality_assurance/plot.py
+-rw-r--r--   0        0        0    10162 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/quality_assurance/rayleigh_fit.py
+-rw-r--r--   0        0        0     8044 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/quality_assurance/telecover.py
+-rw-r--r--   0        0        0    10850 2023-01-19 15:14:33.635682 gfatpy-0.8.0/gfatpy/lidar/reader.py
+-rw-r--r--   0        0        0        0 2023-01-19 15:14:33.635682 gfatpy-0.8.0/gfatpy/lidar/retrieval/__init__.py
+-rw-r--r--   0        0        0     3563 2023-01-19 15:14:33.635682 gfatpy-0.8.0/gfatpy/lidar/retrieval/helper.py
+-rw-r--r--   0        0        0     6175 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/retrieval/klett.py
+-rw-r--r--   0        0        0     5145 2023-01-19 15:14:33.635682 gfatpy-0.8.0/gfatpy/lidar/retrieval/lidar_layer_detection.py
+-rw-r--r--   0        0        0        0 2023-01-19 15:14:33.635682 gfatpy-0.8.0/gfatpy/lidar/retrieval/number_concentration.py
+-rw-r--r--   0        0        0     7009 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/retrieval/raman.py
+-rw-r--r--   0        0        0     8196 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/retrieval/synthetic/generator.py
+-rw-r--r--   0        0        0      563 2023-07-31 14:12:26.725658 gfatpy-0.8.0/gfatpy/lidar/scc/systems/alhambra/alhambra.py
+-rw-r--r--   0        0        0      634 2023-07-31 14:12:26.725658 gfatpy-0.8.0/gfatpy/lidar/scc/systems/alhambra/alhambra_729.py
+-rw-r--r--   0        0        0    10769 2023-07-31 14:12:26.725658 gfatpy-0.8.0/gfatpy/lidar/scc/systems/alhambra/alhambra_all.py
+-rw-r--r--   0        0        0     2151 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/types.py
+-rw-r--r--   0        0        0     6247 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/lidar/utils.py
+-rw-r--r--   0        0        0      244 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/radar/__init__.py
+-rw-r--r--   0        0        0      101 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/radar/info.yml
+-rw-r--r--   0        0        0        0 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/radar/plot/info.yml
+-rw-r--r--   0        0        0     2225 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/radar/reader.py
+-rw-r--r--   0        0        0    61357 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/radar/scattering_databases/0.C_24.1GHz.csv
+-rw-r--r--   0        0        0    61200 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/radar/scattering_databases/0.C_35.5GHz.csv
+-rw-r--r--   0        0        0    60964 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/radar/scattering_databases/0.C_94.0GHz.csv
+-rw-r--r--   0        0        0    61372 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/radar/scattering_databases/10C_24.1GHz.csv
+-rw-r--r--   0        0        0    61213 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/radar/scattering_databases/10C_35.5GHz.csv
+-rw-r--r--   0        0        0    60965 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/radar/scattering_databases/10C_94.0GHz.csv
+-rw-r--r--   0        0        0    60528 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/radar/scattering_databases/20C_24.1GHz.csv
+-rw-r--r--   0        0        0    61215 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/radar/scattering_databases/20C_35.5GHz.csv
+-rw-r--r--   0        0        0    60984 2023-07-25 03:08:40.496165 gfatpy-0.8.0/gfatpy/radar/scattering_databases/20C_94.0GHz.csv
+-rw-r--r--   0        0        0     1305 2023-07-25 03:08:40.506165 gfatpy-0.8.0/gfatpy/radar/types.py
+-rw-r--r--   0        0        0     5853 2023-07-25 03:08:40.506165 gfatpy-0.8.0/gfatpy/radar/utils.py
+-rw-r--r--   0        0        0       34 2023-01-19 15:14:33.635682 gfatpy-0.8.0/gfatpy/utils/__init__.py
+-rw-r--r--   0        0        0     9655 2023-07-25 03:08:40.506165 gfatpy-0.8.0/gfatpy/utils/calibration.py
+-rw-r--r--   0        0        0     3510 2023-07-31 14:23:02.085738 gfatpy-0.8.0/gfatpy/utils/io.py
+-rw-r--r--   0        0        0     2870 2023-07-25 03:08:40.506165 gfatpy-0.8.0/gfatpy/utils/optimized.py
+-rw-r--r--   0        0        0     6664 2023-01-19 15:14:33.635682 gfatpy-0.8.0/gfatpy/utils/plot.py
+-rw-r--r--   0        0        0    13283 2023-07-25 03:08:40.506165 gfatpy-0.8.0/gfatpy/utils/utils.py
+-rw-r--r--   0        0        0     1510 2023-07-31 14:23:26.055740 gfatpy-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1892 1970-01-01 00:00:00.000000 gfatpy-0.8.0/setup.py
+-rw-r--r--   0        0        0     1517 1970-01-01 00:00:00.000000 gfatpy-0.8.0/PKG-INFO
```

### Comparing `gfatpy-0.7.0/gfatpy/__init__.py` & `gfatpy-0.8.0/gfatpy/__init__.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/aeronet/__init__.py` & `gfatpy-0.8.0/gfatpy/aeronet/__init__.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/aeronet/aeronet4lidar.py` & `gfatpy-0.8.0/gfatpy/aeronet/aeronet4lidar.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/aeronet/info.yml` & `gfatpy-0.8.0/gfatpy/aeronet/info.yml`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/aeronet/plot.py` & `gfatpy-0.8.0/gfatpy/aeronet/plot.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/aeronet/reader.py` & `gfatpy-0.8.0/gfatpy/aeronet/reader.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/aeronet/typing.py` & `gfatpy-0.8.0/gfatpy/aeronet/typing.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/aeronet/utils.py` & `gfatpy-0.8.0/gfatpy/aeronet/utils.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/assets/LOGO_GFAT_150pp.png` & `gfatpy-0.8.0/gfatpy/assets/LOGO_GFAT_150pp.png`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/atmo/atmo.py` & `gfatpy-0.8.0/gfatpy/atmo/atmo.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/atmo/ecmwf.py` & `gfatpy-0.8.0/gfatpy/atmo/ecmwf.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/atmo/solar.py` & `gfatpy-0.8.0/gfatpy/atmo/solar.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/cli/lidar/main.py` & `gfatpy-0.8.0/gfatpy/cli/lidar/main.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/cli/lidar/plot/main.py` & `gfatpy-0.8.0/gfatpy/cli/lidar/plot/main.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/cli/main.py` & `gfatpy-0.8.0/gfatpy/cli/main.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/cloudnet/cloud_model.py` & `gfatpy-0.8.0/gfatpy/cloudnet/cloud_model.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/cloudnet/plot_deprecated.py` & `gfatpy-0.8.0/gfatpy/cloudnet/plot_deprecated.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/cloudnet/reader.py` & `gfatpy-0.8.0/gfatpy/cloudnet/reader.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/cloudnet/utils.py` & `gfatpy-0.8.0/gfatpy/cloudnet/utils.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/depolarization/calibration.py` & `gfatpy-0.8.0/gfatpy/lidar/depolarization/calibration.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/depolarization/depolarization_calibration_alh.py` & `gfatpy-0.8.0/gfatpy/lidar/depolarization/depolarization_calibration_alh.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/depolarization/depolarization_calibration_mhc.py` & `gfatpy-0.8.0/gfatpy/lidar/depolarization/depolarization_calibration_mhc.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/depolarization/depolarization_calibration_vlt.py` & `gfatpy-0.8.0/gfatpy/lidar/depolarization/depolarization_calibration_vlt.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/depolarization/GHK/.hgtags` & `gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/.hgtags`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/depolarization/GHK/About the effects of polarising optics_4b_1L_corr.pdf` & `gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/About the effects of polarising optics_4b_1L_corr.pdf`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/depolarization/GHK/CHANGELOG.md` & `gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/depolarization/GHK/GHK_0.9.8h_Py3.7.py` & `gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/GHK_0.9.8h_Py3.7.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/depolarization/GHK/Improvements_of_the_GHK_script_200529.pdf` & `gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/Improvements_of_the_GHK_script_200529.pdf`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/depolarization/GHK/LICENSE.md` & `gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/depolarization/GHK/README.md` & `gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/README.md`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/depolarization/GHK/system_settings/mulhacen_polarizer_template.py` & `gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/system_settings/mulhacen_polarizer_template.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/depolarization/GHK/system_settings/mulhacen_rotator_casoG_template.py` & `gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/system_settings/mulhacen_rotator_casoG_template.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/depolarization/GHK/system_settings/mulhacen_run.py` & `gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/system_settings/mulhacen_run.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_0.9.8e4-PollyXT_Lacros.py` & `gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_0.9.8e4-PollyXT_Lacros.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_0.9.8h-PollyXT_Cyprus_532_210429_vf_4.py` & `gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_0.9.8h-PollyXT_Cyprus_532_210429_vf_4.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_mhc_pol_532x_20130101.py` & `gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_mhc_pol_532x_20130101.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_mhc_rot_532x_20130101.py` & `gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_mhc_rot_532x_20130101.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_mhc_rot_532x_20220614.py` & `gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_mhc_rot_532x_20220614.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/depolarization/GHK.py` & `gfatpy-0.8.0/gfatpy/lidar/depolarization/GHK.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/depolarization/io.py` & `gfatpy-0.8.0/gfatpy/lidar/depolarization/io.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/depolarization/plot.py` & `gfatpy-0.8.0/gfatpy/lidar/depolarization/plot.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/depolarization/retrieval.py` & `gfatpy-0.8.0/gfatpy/lidar/depolarization/retrieval.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/depolarization/utils.py` & `gfatpy-0.8.0/gfatpy/lidar/depolarization/utils.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/file_manager.py` & `gfatpy-0.8.0/gfatpy/lidar/file_manager.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/info.yml` & `gfatpy-0.8.0/gfatpy/lidar/info.yml`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/nc_convert/configs/ALHAMBRA.toml` & `gfatpy-0.8.0/gfatpy/lidar/nc_convert/configs/ALHAMBRA.toml`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/nc_convert/configs/MULHACEN.toml` & `gfatpy-0.8.0/gfatpy/lidar/nc_convert/configs/MULHACEN.toml`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/nc_convert/converter.py` & `gfatpy-0.8.0/gfatpy/lidar/nc_convert/converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import re
 import shutil
 import sys
-from pdb import set_trace
 from pathlib import Path
 from datetime import datetime, timedelta
 from typing import Iterator
 
 from linc import write_nc_legacy
 from linc.config import get_config, Config
 from loguru import logger
```

### Comparing `gfatpy-0.7.0/gfatpy/lidar/plot/info.yml` & `gfatpy-0.8.0/gfatpy/lidar/plot/info.yml`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/plot/quicklook.py` & `gfatpy-0.8.0/gfatpy/lidar/plot/quicklook.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/preprocessing/__init__.py` & `gfatpy-0.8.0/gfatpy/lidar/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/preprocessing/gluing_de_la_rosa.py` & `gfatpy-0.8.0/gfatpy/lidar/preprocessing/gluing_de_la_rosa.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/preprocessing/gluing_de_la_rosa_slope.py` & `gfatpy-0.8.0/gfatpy/lidar/preprocessing/gluing_de_la_rosa_slope.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/preprocessing/gluing_proportional.py` & `gfatpy-0.8.0/gfatpy/lidar/preprocessing/gluing_proportional.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/preprocessing/lidar_gluing_bravo_aranda.py` & `gfatpy-0.8.0/gfatpy/lidar/preprocessing/lidar_gluing_bravo_aranda.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/preprocessing/lidar_gluing_damico.py` & `gfatpy-0.8.0/gfatpy/lidar/preprocessing/lidar_gluing_damico.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/preprocessing/lidar_linear_response_region.py` & `gfatpy-0.8.0/gfatpy/lidar/preprocessing/lidar_linear_response_region.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/preprocessing/lidar_preprocessing.py` & `gfatpy-0.8.0/gfatpy/lidar/preprocessing/lidar_preprocessing.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/preprocessing/lidar_preprocessing_tools.py` & `gfatpy-0.8.0/gfatpy/lidar/preprocessing/lidar_preprocessing_tools.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/preprocessing/study_dead_time.py` & `gfatpy-0.8.0/gfatpy/lidar/preprocessing/study_dead_time.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/quality_assurance/common.py` & `gfatpy-0.8.0/gfatpy/lidar/quality_assurance/common.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/quality_assurance/io.py` & `gfatpy-0.8.0/gfatpy/lidar/quality_assurance/io.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/quality_assurance/overlap.py` & `gfatpy-0.8.0/gfatpy/lidar/quality_assurance/overlap.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/quality_assurance/plot.py` & `gfatpy-0.8.0/gfatpy/lidar/quality_assurance/plot.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/quality_assurance/rayleigh_fit.py` & `gfatpy-0.8.0/gfatpy/lidar/quality_assurance/rayleigh_fit.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/quality_assurance/telecover.py` & `gfatpy-0.8.0/gfatpy/lidar/quality_assurance/telecover.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/reader.py` & `gfatpy-0.8.0/gfatpy/lidar/reader.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/retrieval/helper.py` & `gfatpy-0.8.0/gfatpy/lidar/retrieval/helper.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/retrieval/klett.py` & `gfatpy-0.8.0/gfatpy/lidar/retrieval/klett.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/retrieval/lidar_layer_detection.py` & `gfatpy-0.8.0/gfatpy/lidar/retrieval/lidar_layer_detection.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/retrieval/raman.py` & `gfatpy-0.8.0/gfatpy/lidar/retrieval/raman.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/retrieval/synthetic/generator.py` & `gfatpy-0.8.0/gfatpy/lidar/retrieval/synthetic/generator.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/types.py` & `gfatpy-0.8.0/gfatpy/lidar/types.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/lidar/utils.py` & `gfatpy-0.8.0/gfatpy/lidar/utils.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/radar/reader.py` & `gfatpy-0.8.0/gfatpy/radar/reader.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/radar/scattering_databases/0.C_24.1GHz.csv` & `gfatpy-0.8.0/gfatpy/radar/scattering_databases/0.C_24.1GHz.csv`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/radar/scattering_databases/0.C_35.5GHz.csv` & `gfatpy-0.8.0/gfatpy/radar/scattering_databases/0.C_35.5GHz.csv`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/radar/scattering_databases/0.C_94.0GHz.csv` & `gfatpy-0.8.0/gfatpy/radar/scattering_databases/0.C_94.0GHz.csv`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/radar/scattering_databases/10C_24.1GHz.csv` & `gfatpy-0.8.0/gfatpy/radar/scattering_databases/10C_24.1GHz.csv`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/radar/scattering_databases/10C_35.5GHz.csv` & `gfatpy-0.8.0/gfatpy/radar/scattering_databases/10C_35.5GHz.csv`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/radar/scattering_databases/10C_94.0GHz.csv` & `gfatpy-0.8.0/gfatpy/radar/scattering_databases/10C_94.0GHz.csv`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/radar/scattering_databases/20C_24.1GHz.csv` & `gfatpy-0.8.0/gfatpy/radar/scattering_databases/20C_24.1GHz.csv`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/radar/scattering_databases/20C_35.5GHz.csv` & `gfatpy-0.8.0/gfatpy/radar/scattering_databases/20C_35.5GHz.csv`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/radar/scattering_databases/20C_94.0GHz.csv` & `gfatpy-0.8.0/gfatpy/radar/scattering_databases/20C_94.0GHz.csv`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/radar/types.py` & `gfatpy-0.8.0/gfatpy/radar/types.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/radar/utils.py` & `gfatpy-0.8.0/gfatpy/radar/utils.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/utils/calibration.py` & `gfatpy-0.8.0/gfatpy/utils/calibration.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/utils/io.py` & `gfatpy-0.8.0/gfatpy/utils/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,48 +2,48 @@
 import zipfile
 import tempfile
 import numpy as np
 from typing import Any, Tuple
 from pathlib import Path
 from datetime import datetime
 
-from pdfminer.pdfinterp import PDFResourceManager, PDFPageInterpreter
-from pdfminer.converter import TextConverter
-from pdfminer.layout import LAParams
-from pdfminer.pdfpage import PDFPage
+# from pdfminer.pdfinterp import PDFResourceManager, PDFPageInterpreter
+# from pdfminer.converter import TextConverter
+# from pdfminer.layout import LAParams
+# from pdfminer.pdfpage import PDFPage
 from io import StringIO
 import yaml
 
 
 def read_yaml(path: Path | str) -> Any:
     """
     Reads a yaml file and returns the data as a dictionary.
     """
     with open(path, "r") as stream:
         return yaml.safe_load(stream)
 
 
-def convert_pdf_to_txt(path, pages=None):
-    if not pages:
-        pagenums = set()
-    else:
-        pagenums = set(pages)
-    output = StringIO()
-    manager = PDFResourceManager()
-    converter = TextConverter(manager, output, laparams=LAParams())
-    interpreter = PDFPageInterpreter(manager, converter)
-
-    infile = open(path, "rb")
-    for page in PDFPage.get_pages(infile, pagenums):
-        interpreter.process_page(page)
-    infile.close()
-    converter.close()
-    text = output.getvalue()
-    output.close()
-    return text
+# def convert_pdf_to_txt(path, pages=None):
+#     if not pages:
+#         pagenums = set()
+#     else:
+#         pagenums = set(pages)
+#     output = StringIO()
+#     manager = PDFResourceManager()
+#     converter = TextConverter(manager, output, laparams=LAParams())
+#     interpreter = PDFPageInterpreter(manager, converter)
+
+#     infile = open(path, "rb")
+#     for page in PDFPage.get_pages(infile, pagenums):
+#         interpreter.process_page(page)
+#     infile.close()
+#     converter.close()
+#     text = output.getvalue()
+#     output.close()
+#     return text
 
 
 from pathlib import Path
 import numpy as np
 from datetime import datetime
```

### Comparing `gfatpy-0.7.0/gfatpy/utils/optimized.py` & `gfatpy-0.8.0/gfatpy/utils/optimized.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/utils/plot.py` & `gfatpy-0.8.0/gfatpy/utils/plot.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/gfatpy/utils/utils.py` & `gfatpy-0.8.0/gfatpy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/LICENSE` & `gfatpy-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gfatpy-0.7.0/pyproject.toml` & `gfatpy-0.8.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gfatpy"
-version = "0.7.0"
+version = "0.8.0"
 description = "A python package for GFAT utilities"
 # Can be extended to multiple authors
 authors = [
     "Juan Diego De la Rosa <jdidelarc@gmail.com>"
 ]
 classifiers = [
     "Intended Audience :: Science/Research",
@@ -33,15 +33,14 @@
 notebook = {version = "^6.4.12", optional = true}
 ipywidgets = {version = "^8.0.2", optional = true}
 typing-extensions = "^4.3.0"
 seaborn = "^0.12.0"
 numba = "^0.56.2"
 scikit-image = "^0.19.3"
 linc = "^1.7.0"
-# pdfminer = "^20191125"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.6.0"
 pytest = "^7.1.2"
 notebook = "^6.4.12"
 pre-commit = "^2.20.0"
 ipywidgets = "^8.0.2"
```

### Comparing `gfatpy-0.7.0/PKG-INFO` & `gfatpy-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: gfatpy
-Version: 0.7.0
+Version: 0.8.0
 Summary: A python package for GFAT utilities
 Author: Juan Diego De la Rosa
 Author-email: jdidelarc@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Provides-Extra: docs
 Provides-Extra: jupyter
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: dask (>=2022.7.1,<2023.0.0)
 Requires-Dist: ipywidgets (>=8.0.2,<9.0.0)
 Requires-Dist: linc (>=1.7.0,<2.0.0)
```

