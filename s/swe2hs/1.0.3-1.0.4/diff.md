# Comparing `tmp/swe2hs-1.0.3.tar.gz` & `tmp/swe2hs-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swe2hs-1.0.3.tar", last modified: Wed Oct 19 21:53:53 2022, max compression
+gzip compressed data, was "swe2hs-1.0.4.tar", last modified: Mon Jul 31 18:08:59 2023, max compression
```

## Comparing `swe2hs-1.0.3.tar` & `swe2hs-1.0.4.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-19 21:53:53.213761 swe2hs-1.0.3/
--rw-rw-rw-   0 root         (0) root         (0)      589 2022-05-12 13:37:12.000000 swe2hs-1.0.3/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)      550 2022-05-12 13:37:12.000000 swe2hs-1.0.3/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      855 2022-10-19 11:03:55.000000 swe2hs-1.0.3/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      490 2022-05-12 13:37:12.000000 swe2hs-1.0.3/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)       87 2022-05-12 13:37:12.000000 swe2hs-1.0.3/AUTHORS.rst
--rw-rw-rw-   0 root         (0) root         (0)     1911 2022-10-19 21:11:07.000000 swe2hs-1.0.3/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     9832 2022-10-19 21:11:07.000000 swe2hs-1.0.3/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)    32473 2022-05-12 13:37:12.000000 swe2hs-1.0.3/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     6517 2022-10-19 21:53:53.213761 swe2hs-1.0.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5421 2022-10-19 21:11:07.000000 swe2hs-1.0.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-19 21:53:53.197761 swe2hs-1.0.3/docs/
--rw-rw-rw-   0 root         (0) root         (0)     1154 2022-05-12 13:37:12.000000 swe2hs-1.0.3/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-19 21:53:53.201761 swe2hs-1.0.3/docs/_autosummary/
--rw-rw-rw-   0 root         (0) root         (0)      147 2022-10-17 14:45:17.000000 swe2hs-1.0.3/docs/_autosummary/swe2hs.one_dimensional.convert_1d.rst
--rw-rw-rw-   0 root         (0) root         (0)      190 2022-10-17 14:45:17.000000 swe2hs-1.0.3/docs/_autosummary/swe2hs.stepwise.process_timestep_from_nc_files.rst
--rw-rw-rw-   0 root         (0) root         (0)      147 2022-10-17 14:45:17.000000 swe2hs-1.0.3/docs/_autosummary/swe2hs.two_dimensional.convert_2d.rst
--rw-rw-rw-   0 root         (0) root         (0)      148 2022-09-13 19:45:52.000000 swe2hs-1.0.3/docs/_autosummary/swe2hs.utils.continuous_timedeltas.rst
--rw-rw-rw-   0 root         (0) root         (0)      208 2022-09-13 19:45:52.000000 swe2hs-1.0.3/docs/_autosummary/swe2hs.utils.continuous_timedeltas_in_nonzero_chunks.rst
--rw-rw-rw-   0 root         (0) root         (0)      132 2022-09-13 19:45:52.000000 swe2hs-1.0.3/docs/_autosummary/swe2hs.utils.fill_small_gaps.rst
--rw-rw-rw-   0 root         (0) root         (0)      155 2022-09-13 19:45:52.000000 swe2hs-1.0.3/docs/_autosummary/swe2hs.utils.get_nonzero_chunk_idxs.rst
--rw-rw-rw-   0 root         (0) root         (0)      143 2022-09-13 19:45:52.000000 swe2hs-1.0.3/docs/_autosummary/swe2hs.utils.get_small_gap_idxs.rst
--rw-rw-rw-   0 root         (0) root         (0)      158 2022-09-13 19:45:52.000000 swe2hs-1.0.3/docs/_autosummary/swe2hs.utils.get_zeropadded_gap_idxs.rst
--rw-rw-rw-   0 root         (0) root         (0)      160 2022-10-17 14:45:17.000000 swe2hs-1.0.3/docs/_autosummary/swe2hs.visualization.groupby_hydroyear.rst
--rw-rw-rw-   0 root         (0) root         (0)      139 2022-10-17 14:45:17.000000 swe2hs-1.0.3/docs/_autosummary/swe2hs.visualization.layer_plot.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-19 21:53:53.205761 swe2hs-1.0.3/docs/_static/
--rw-rw-rw-   0 root         (0) root         (0)       18 2022-05-12 13:37:12.000000 swe2hs-1.0.3/docs/_static/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     4869 2022-10-17 14:45:17.000000 swe2hs-1.0.3/docs/_static/SLF_Logo_cmyk.svg
--rw-rw-rw-   0 root         (0) root         (0)   458081 2022-09-13 19:45:52.000000 swe2hs-1.0.3/docs/_static/colored_layers_kuhtai_2002.png
--rw-rw-rw-   0 root         (0) root         (0)     3011 2022-10-17 14:45:17.000000 swe2hs-1.0.3/docs/_static/pypi-blue-cube.svg
--rw-rw-rw-   0 root         (0) root         (0)     3095 2022-09-13 19:45:52.000000 swe2hs-1.0.3/docs/_static/swe2hs_logo.svg
--rw-rw-rw-   0 root         (0) root         (0)     1213 2022-10-17 14:45:17.000000 swe2hs-1.0.3/docs/api.rst
--rw-rw-rw-   0 root         (0) root         (0)       29 2022-10-17 14:45:17.000000 swe2hs-1.0.3/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)    10326 2022-10-19 21:11:07.000000 swe2hs-1.0.3/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-05-12 13:37:12.000000 swe2hs-1.0.3/docs/contributing.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-19 21:53:53.205761 swe2hs-1.0.3/docs/examples/
--rw-rw-rw-   0 root         (0) root         (0)     4229 2022-10-19 21:11:07.000000 swe2hs-1.0.3/docs/examples/transfer_one_dimensional_series.md
--rw-rw-rw-   0 root         (0) root         (0)     7249 2022-10-19 21:11:07.000000 swe2hs-1.0.3/docs/examples/transfer_two_dimensional_dataarray.md
--rw-rw-rw-   0 root         (0) root         (0)      372 2022-10-19 21:11:07.000000 swe2hs-1.0.3/docs/examples.rst
--rw-rw-rw-   0 root         (0) root         (0)      238 2022-10-17 14:45:17.000000 swe2hs-1.0.3/docs/getting_started.rst
--rw-rw-rw-   0 root         (0) root         (0)     1163 2022-10-17 14:45:17.000000 swe2hs-1.0.3/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      286 2022-09-13 19:45:52.000000 swe2hs-1.0.3/docs/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      355 2022-05-12 13:37:12.000000 swe2hs-1.0.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1781 2022-10-19 21:53:53.213761 swe2hs-1.0.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      703 2022-05-12 13:37:12.000000 swe2hs-1.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-19 21:53:53.189761 swe2hs-1.0.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-19 21:53:53.205761 swe2hs-1.0.3/src/swe2hs/
--rw-rw-rw-   0 root         (0) root         (0)      706 2022-10-17 14:45:17.000000 swe2hs-1.0.3/src/swe2hs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14533 2022-10-19 11:03:55.000000 swe2hs-1.0.3/src/swe2hs/_core.py
--rw-rw-rw-   0 root         (0) root         (0)      173 2022-10-19 11:03:55.000000 swe2hs-1.0.3/src/swe2hs/_default_model_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    11272 2022-10-19 11:03:55.000000 swe2hs-1.0.3/src/swe2hs/one_dimensional.py
--rw-rw-rw-   0 root         (0) root         (0)    16262 2022-10-19 11:03:55.000000 swe2hs-1.0.3/src/swe2hs/stepwise.py
--rw-rw-rw-   0 root         (0) root         (0)    10713 2022-10-19 11:03:55.000000 swe2hs-1.0.3/src/swe2hs/two_dimensional.py
--rw-rw-rw-   0 root         (0) root         (0)    10241 2022-10-17 14:45:17.000000 swe2hs-1.0.3/src/swe2hs/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5418 2022-10-17 14:45:17.000000 swe2hs-1.0.3/src/swe2hs/visualization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-19 21:53:53.209761 swe2hs-1.0.3/src/swe2hs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6517 2022-10-19 21:53:53.000000 swe2hs-1.0.3/src/swe2hs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1818 2022-10-19 21:53:53.000000 swe2hs-1.0.3/src/swe2hs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-19 21:53:53.000000 swe2hs-1.0.3/src/swe2hs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-19 21:53:52.000000 swe2hs-1.0.3/src/swe2hs.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      178 2022-10-19 21:53:53.000000 swe2hs-1.0.3/src/swe2hs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-10-19 21:53:53.000000 swe2hs-1.0.3/src/swe2hs.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-19 21:53:53.213761 swe2hs-1.0.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)     4884 2022-10-19 11:03:55.000000 swe2hs-1.0.3/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     5369 2022-10-19 11:03:55.000000 swe2hs-1.0.3/tests/test_core.py
--rw-rw-rw-   0 root         (0) root         (0)     1669 2022-10-17 14:45:17.000000 swe2hs-1.0.3/tests/test_one_dimensional.py
--rw-rw-rw-   0 root         (0) root         (0)     8531 2022-10-19 11:03:55.000000 swe2hs-1.0.3/tests/test_stepwise.py
--rw-rw-rw-   0 root         (0) root         (0)     7182 2022-10-19 11:03:55.000000 swe2hs-1.0.3/tests/test_two_dimensional.py
--rw-rw-rw-   0 root         (0) root         (0)    12658 2022-10-17 14:45:17.000000 swe2hs-1.0.3/tests/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      907 2022-10-17 14:45:17.000000 swe2hs-1.0.3/tests/test_visualization.py
--rw-rw-rw-   0 root         (0) root         (0)     2031 2022-10-19 11:03:55.000000 swe2hs-1.0.3/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:08:59.009192 swe2hs-1.0.4/
+-rw-rw-rw-   0 root         (0) root         (0)      589 2023-07-31 17:14:12.000000 swe2hs-1.0.4/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)      550 2023-07-31 17:14:12.000000 swe2hs-1.0.4/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-07-31 17:14:12.000000 swe2hs-1.0.4/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      490 2023-07-31 17:14:12.000000 swe2hs-1.0.4/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-07-31 17:14:12.000000 swe2hs-1.0.4/AUTHORS.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2270 2023-07-31 17:14:12.000000 swe2hs-1.0.4/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     9832 2023-07-31 17:14:12.000000 swe2hs-1.0.4/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)    32473 2023-07-31 17:14:12.000000 swe2hs-1.0.4/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     6730 2023-07-31 18:08:59.009192 swe2hs-1.0.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5634 2023-07-31 17:14:12.000000 swe2hs-1.0.4/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:08:58.981192 swe2hs-1.0.4/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-07-31 17:14:12.000000 swe2hs-1.0.4/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:08:58.993192 swe2hs-1.0.4/docs/_autosummary/
+-rw-rw-rw-   0 root         (0) root         (0)      147 2023-07-31 17:14:12.000000 swe2hs-1.0.4/docs/_autosummary/swe2hs.one_dimensional.convert_1d.rst
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-07-31 17:14:12.000000 swe2hs-1.0.4/docs/_autosummary/swe2hs.stepwise.process_timestep_from_nc_files.rst
+-rw-rw-rw-   0 root         (0) root         (0)      147 2023-07-31 17:14:12.000000 swe2hs-1.0.4/docs/_autosummary/swe2hs.two_dimensional.convert_2d.rst
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-07-31 17:14:12.000000 swe2hs-1.0.4/docs/_autosummary/swe2hs.utils.continuous_timedeltas.rst
+-rw-rw-rw-   0 root         (0) root         (0)      208 2023-07-31 17:14:12.000000 swe2hs-1.0.4/docs/_autosummary/swe2hs.utils.continuous_timedeltas_in_nonzero_chunks.rst
+-rw-rw-rw-   0 root         (0) root         (0)      132 2023-07-31 17:14:12.000000 swe2hs-1.0.4/docs/_autosummary/swe2hs.utils.fill_small_gaps.rst
+-rw-rw-rw-   0 root         (0) root         (0)      155 2023-07-31 17:14:12.000000 swe2hs-1.0.4/docs/_autosummary/swe2hs.utils.get_nonzero_chunk_idxs.rst
+-rw-rw-rw-   0 root         (0) root         (0)      143 2023-07-31 17:14:12.000000 swe2hs-1.0.4/docs/_autosummary/swe2hs.utils.get_small_gap_idxs.rst
+-rw-rw-rw-   0 root         (0) root         (0)      158 2023-07-31 17:14:12.000000 swe2hs-1.0.4/docs/_autosummary/swe2hs.utils.get_zeropadded_gap_idxs.rst
+-rw-rw-rw-   0 root         (0) root         (0)      160 2023-07-31 17:14:12.000000 swe2hs-1.0.4/docs/_autosummary/swe2hs.visualization.groupby_hydroyear.rst
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-07-31 17:14:12.000000 swe2hs-1.0.4/docs/_autosummary/swe2hs.visualization.layer_plot.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:08:58.997192 swe2hs-1.0.4/docs/_static/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-07-31 17:14:12.000000 swe2hs-1.0.4/docs/_static/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     4869 2023-07-31 17:14:12.000000 swe2hs-1.0.4/docs/_static/SLF_Logo_cmyk.svg
+-rw-rw-rw-   0 root         (0) root         (0)   458081 2023-07-31 17:14:12.000000 swe2hs-1.0.4/docs/_static/colored_layers_kuhtai_2002.png
+-rw-rw-rw-   0 root         (0) root         (0)     3011 2023-07-31 17:14:12.000000 swe2hs-1.0.4/docs/_static/pypi-blue-cube.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3095 2023-07-31 17:14:12.000000 swe2hs-1.0.4/docs/_static/swe2hs_logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1213 2023-07-31 17:14:12.000000 swe2hs-1.0.4/docs/api.rst
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-07-31 17:14:12.000000 swe2hs-1.0.4/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)    10326 2023-07-31 17:14:12.000000 swe2hs-1.0.4/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-31 17:14:12.000000 swe2hs-1.0.4/docs/contributing.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:08:59.001192 swe2hs-1.0.4/docs/examples/
+-rw-rw-rw-   0 root         (0) root         (0)     4229 2023-07-31 17:14:12.000000 swe2hs-1.0.4/docs/examples/transfer_one_dimensional_series.md
+-rw-rw-rw-   0 root         (0) root         (0)     7249 2023-07-31 17:14:12.000000 swe2hs-1.0.4/docs/examples/transfer_two_dimensional_dataarray.md
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-07-31 17:14:12.000000 swe2hs-1.0.4/docs/examples.rst
+-rw-rw-rw-   0 root         (0) root         (0)      238 2023-07-31 17:14:12.000000 swe2hs-1.0.4/docs/getting_started.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1163 2023-07-31 17:14:12.000000 swe2hs-1.0.4/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-07-31 17:14:12.000000 swe2hs-1.0.4/docs/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      355 2023-07-31 17:14:12.000000 swe2hs-1.0.4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1781 2023-07-31 18:08:59.009192 swe2hs-1.0.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      703 2023-07-31 17:14:12.000000 swe2hs-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:08:58.969191 swe2hs-1.0.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:08:59.001192 swe2hs-1.0.4/src/swe2hs/
+-rw-rw-rw-   0 root         (0) root         (0)      706 2023-07-31 17:14:12.000000 swe2hs-1.0.4/src/swe2hs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14533 2023-07-31 17:14:12.000000 swe2hs-1.0.4/src/swe2hs/_core.py
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-07-31 17:14:12.000000 swe2hs-1.0.4/src/swe2hs/_default_model_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    11272 2023-07-31 17:14:12.000000 swe2hs-1.0.4/src/swe2hs/one_dimensional.py
+-rw-rw-rw-   0 root         (0) root         (0)    16262 2023-07-31 17:14:12.000000 swe2hs-1.0.4/src/swe2hs/stepwise.py
+-rw-rw-rw-   0 root         (0) root         (0)    10713 2023-07-31 17:14:12.000000 swe2hs-1.0.4/src/swe2hs/two_dimensional.py
+-rw-rw-rw-   0 root         (0) root         (0)    10241 2023-07-31 17:14:12.000000 swe2hs-1.0.4/src/swe2hs/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5580 2023-07-31 17:14:12.000000 swe2hs-1.0.4/src/swe2hs/visualization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:08:59.001192 swe2hs-1.0.4/src/swe2hs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6730 2023-07-31 18:08:58.000000 swe2hs-1.0.4/src/swe2hs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-07-31 18:08:58.000000 swe2hs-1.0.4/src/swe2hs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 18:08:58.000000 swe2hs-1.0.4/src/swe2hs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 18:08:58.000000 swe2hs-1.0.4/src/swe2hs.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      178 2023-07-31 18:08:58.000000 swe2hs-1.0.4/src/swe2hs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-31 18:08:58.000000 swe2hs-1.0.4/src/swe2hs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 18:08:59.005192 swe2hs-1.0.4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     4884 2023-07-31 17:14:12.000000 swe2hs-1.0.4/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     5369 2023-07-31 17:14:12.000000 swe2hs-1.0.4/tests/test_core.py
+-rw-rw-rw-   0 root         (0) root         (0)     1669 2023-07-31 17:14:12.000000 swe2hs-1.0.4/tests/test_one_dimensional.py
+-rw-rw-rw-   0 root         (0) root         (0)     8531 2023-07-31 17:14:12.000000 swe2hs-1.0.4/tests/test_stepwise.py
+-rw-rw-rw-   0 root         (0) root         (0)     7182 2023-07-31 17:14:12.000000 swe2hs-1.0.4/tests/test_two_dimensional.py
+-rw-rw-rw-   0 root         (0) root         (0)    12658 2023-07-31 17:14:12.000000 swe2hs-1.0.4/tests/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      907 2023-07-31 17:14:12.000000 swe2hs-1.0.4/tests/test_visualization.py
+-rw-rw-rw-   0 root         (0) root         (0)     2031 2023-07-31 17:14:12.000000 swe2hs-1.0.4/tox.ini
```

### Comparing `swe2hs-1.0.3/.coveragerc` & `swe2hs-1.0.4/.coveragerc`

 * *Files identical despite different names*

### Comparing `swe2hs-1.0.3/.gitignore` & `swe2hs-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `swe2hs-1.0.3/.gitlab-ci.yml` & `swe2hs-1.0.4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `swe2hs-1.0.3/CHANGELOG.rst` & `swe2hs-1.0.4/CHANGELOG.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 =========
 Changelog
 =========
 
+Version 1.0.4 (2023-07-31)
+==============================
+
+Improvements to the :func:`~swe2hs.visualization.layer_plot` function 
+[`!10 <https://gitlabext.wsl.ch/aschauer/swe2hs/-/merge_requests/10>`_]:
+
+- optional colorbar plotting
+- faster color plotting
+- no layer borders are drawn for empty layers
+
+Added reference to model description paper in readme.
+
 Version 1.0.3 (2022-10-19)
 ==========================
 
 Minor patch which fixes typos and broken links in the documentation.
 
 Version 1.0.2 (2022-10-19)
 ==========================
```

### Comparing `swe2hs-1.0.3/CONTRIBUTING.rst` & `swe2hs-1.0.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `swe2hs-1.0.3/LICENSE.txt` & `swe2hs-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `swe2hs-1.0.3/PKG-INFO` & `swe2hs-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swe2hs
-Version: 1.0.3
+Version: 1.0.4
 Summary: Conceptual snow density model for transferring snow water equivalent to snow depth.
 Home-page: https://code.wsl.ch/aschauer/swe2hs
 Author: Johannes Aschauer
 Author-email: johannes.aschauer@slf.ch
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://aschauer.gitlab-pages.wsl.ch/swe2hs/
 Project-URL: Changelog, https://aschauer.gitlab-pages.wsl.ch/swe2hs/changelog.html
@@ -49,29 +49,36 @@
 equivalent (SWE) of the snow cover to snow depth (HS). Some people informally 
 call it JOPACK, which is an acronym for Just density Of the snowPACK.
 
 The density model calculates snow depth at a daily resolution and is 
 driven by the daily snow water equivalent of the snow cover only. The 
 model creates a new layer with a fixed new snow density :math:`\rho_{new}` for
 every increase in SWE such that, over time, a snowpack of individual layers 
-builds up. The density of a layer increases exponentially with time towards 
-a time-varying maximum density. The maximum density is starting with an initial 
-value at creation time of the layer and is subsequently increasing towards 
+builds up. The density of a layer increases with an exponential decay function towards 
+a time-varying maximum density. The maximum density starts with an initial 
+value at creation time of the layer and subsequently increases towards 
 a higher value based on the overburden a layer has experienced and the 
 occurrence of SWE losses in the snow pack. When SWE decreases, the model 
-removes SWE from the top of the snowpack. The layer number :math:`n` can thus
+removes layers from the top of the snowpack. The layer number :math:`n` can thus
 undergo changes over time based on the number of SWE increases and losses in 
 the snowpack. The model neglects constructive metamorphism, refreezing, and 
-is not able to capture rain-on-snow (ROS) events which might lead to an 
-increase in SWE but no increase in HS. 
+is not able to capture rain-on-snow events which might lead to an 
+increase in SWE but no increase in snow depth.
+
+Citation
+========
+
+For more information on the model and how it was calibrated, please refer to the 
+model description paper:
+
+Aschauer, J.; Michel, A.; Jonas, T.; Marty, C., 2023: An empirical model to 
+calculate snow depth from daily snow water equivalent: SWE2HS 1.0. 
+Geoscientific Model Development, 16, 14: 4063-4081. doi: 
+`10.5194/gmd-16-4063-2023 <https://doi.org/10.5194/gmd-16-4063-2023>`_ 
 
-.. TODO: add the following paragraph once the paper is published:
-.. For further information on the model and how it was calibrated please refer to the 
-.. model description paper:
-.. CITATION HERE.
 .. end_intro
 
 |
 
 .. image:: https://code.wsl.ch/aschauer/swe2hs/-/raw/master/docs/_static/colored_layers_kuhtai_2002.png
    :alt: Schematic snowpack evolution
 
@@ -170,12 +177,14 @@
 .. _new issue: https://code.wsl.ch/aschauer/swe2hs/-/issues/new
 .. _existing issues: https://code.wsl.ch/aschauer/swe2hs/-/issues
 
 .. end_help
 
 .. start_bib
 
+|
+
 .. [#Krajci2017] Krajci, P., Kirnbauer, R., Parajka, J., Schöber, J., & Blöschl, G. (2017). The Kühtai 
    data set: 25 years of lysimetric, snow pillow, and meteorological measurements, 
    *Water Resources Research*, 53, 5158-5165, https://doi.org/10.1002/2017WR020445.
 .. end_bib
```

### Comparing `swe2hs-1.0.3/README.rst` & `swe2hs-1.0.4/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -24,29 +24,36 @@
 equivalent (SWE) of the snow cover to snow depth (HS). Some people informally 
 call it JOPACK, which is an acronym for Just density Of the snowPACK.
 
 The density model calculates snow depth at a daily resolution and is 
 driven by the daily snow water equivalent of the snow cover only. The 
 model creates a new layer with a fixed new snow density :math:`\rho_{new}` for
 every increase in SWE such that, over time, a snowpack of individual layers 
-builds up. The density of a layer increases exponentially with time towards 
-a time-varying maximum density. The maximum density is starting with an initial 
-value at creation time of the layer and is subsequently increasing towards 
+builds up. The density of a layer increases with an exponential decay function towards 
+a time-varying maximum density. The maximum density starts with an initial 
+value at creation time of the layer and subsequently increases towards 
 a higher value based on the overburden a layer has experienced and the 
 occurrence of SWE losses in the snow pack. When SWE decreases, the model 
-removes SWE from the top of the snowpack. The layer number :math:`n` can thus
+removes layers from the top of the snowpack. The layer number :math:`n` can thus
 undergo changes over time based on the number of SWE increases and losses in 
 the snowpack. The model neglects constructive metamorphism, refreezing, and 
-is not able to capture rain-on-snow (ROS) events which might lead to an 
-increase in SWE but no increase in HS. 
+is not able to capture rain-on-snow events which might lead to an 
+increase in SWE but no increase in snow depth.
+
+Citation
+========
+
+For more information on the model and how it was calibrated, please refer to the 
+model description paper:
+
+Aschauer, J.; Michel, A.; Jonas, T.; Marty, C., 2023: An empirical model to 
+calculate snow depth from daily snow water equivalent: SWE2HS 1.0. 
+Geoscientific Model Development, 16, 14: 4063-4081. doi: 
+`10.5194/gmd-16-4063-2023 <https://doi.org/10.5194/gmd-16-4063-2023>`_ 
 
-.. TODO: add the following paragraph once the paper is published:
-.. For further information on the model and how it was calibrated please refer to the 
-.. model description paper:
-.. CITATION HERE.
 .. end_intro
 
 |
 
 .. image:: https://code.wsl.ch/aschauer/swe2hs/-/raw/master/docs/_static/colored_layers_kuhtai_2002.png
    :alt: Schematic snowpack evolution
 
@@ -145,12 +152,14 @@
 .. _new issue: https://code.wsl.ch/aschauer/swe2hs/-/issues/new
 .. _existing issues: https://code.wsl.ch/aschauer/swe2hs/-/issues
 
 .. end_help
 
 .. start_bib
 
+|
+
 .. [#Krajci2017] Krajci, P., Kirnbauer, R., Parajka, J., Schöber, J., & Blöschl, G. (2017). The Kühtai 
    data set: 25 years of lysimetric, snow pillow, and meteorological measurements, 
    *Water Resources Research*, 53, 5158-5165, https://doi.org/10.1002/2017WR020445.
 .. end_bib
```

### Comparing `swe2hs-1.0.3/docs/Makefile` & `swe2hs-1.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `swe2hs-1.0.3/docs/_static/SLF_Logo_cmyk.svg` & `swe2hs-1.0.4/docs/_static/SLF_Logo_cmyk.svg`

 * *Files identical despite different names*

### Comparing `swe2hs-1.0.3/docs/_static/colored_layers_kuhtai_2002.png` & `swe2hs-1.0.4/docs/_static/colored_layers_kuhtai_2002.png`

 * *Files identical despite different names*

### Comparing `swe2hs-1.0.3/docs/_static/pypi-blue-cube.svg` & `swe2hs-1.0.4/docs/_static/pypi-blue-cube.svg`

 * *Files identical despite different names*

### Comparing `swe2hs-1.0.3/docs/_static/swe2hs_logo.svg` & `swe2hs-1.0.4/docs/_static/swe2hs_logo.svg`

 * *Files identical despite different names*

### Comparing `swe2hs-1.0.3/docs/api.rst` & `swe2hs-1.0.4/docs/api.rst`

 * *Files identical despite different names*

### Comparing `swe2hs-1.0.3/docs/conf.py` & `swe2hs-1.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `swe2hs-1.0.3/docs/examples/transfer_one_dimensional_series.md` & `swe2hs-1.0.4/docs/examples/transfer_one_dimensional_series.md`

 * *Files identical despite different names*

### Comparing `swe2hs-1.0.3/docs/examples/transfer_two_dimensional_dataarray.md` & `swe2hs-1.0.4/docs/examples/transfer_two_dimensional_dataarray.md`

 * *Files identical despite different names*

### Comparing `swe2hs-1.0.3/docs/index.rst` & `swe2hs-1.0.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `swe2hs-1.0.3/setup.cfg` & `swe2hs-1.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `swe2hs-1.0.3/setup.py` & `swe2hs-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `swe2hs-1.0.3/src/swe2hs/__init__.py` & `swe2hs-1.0.4/src/swe2hs/__init__.py`

 * *Files identical despite different names*

### Comparing `swe2hs-1.0.3/src/swe2hs/_core.py` & `swe2hs-1.0.4/src/swe2hs/_core.py`

 * *Files identical despite different names*

### Comparing `swe2hs-1.0.3/src/swe2hs/one_dimensional.py` & `swe2hs-1.0.4/src/swe2hs/one_dimensional.py`

 * *Files identical despite different names*

### Comparing `swe2hs-1.0.3/src/swe2hs/stepwise.py` & `swe2hs-1.0.4/src/swe2hs/stepwise.py`

 * *Files identical despite different names*

### Comparing `swe2hs-1.0.3/src/swe2hs/two_dimensional.py` & `swe2hs-1.0.4/src/swe2hs/two_dimensional.py`

 * *Files identical despite different names*

### Comparing `swe2hs-1.0.3/src/swe2hs/utils.py` & `swe2hs-1.0.4/src/swe2hs/utils.py`

 * *Files identical despite different names*

### Comparing `swe2hs-1.0.3/src/swe2hs/visualization.py` & `swe2hs-1.0.4/src/swe2hs/visualization.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     color_variable='layer_densities',
     vmin=50.,
     vmax=550.,
     cmap='cool',
     cbar_label='Density [kg/m$^{3}$]',
     top_line_kwargs=None,
     layer_line_kwargs=None,
+    colorbar=True,
     cax_kwargs=None,
 ):
 
     """
     Plot the layers in the modeled snowpack with optional coloring relating to
     one of the state variables 'layer_heights', 'layer_densities', or 
     'layer_max_densities'.
@@ -73,72 +74,85 @@
         Label of the colorbar. The default is 'Density [kg/m$^{3}$]'.
     top_line_kwargs : dict or None, optional
         Keyword arguments for the line at top of the snowpack. The default is
         None which sets reasonable defaults.
     layer_line_kwargs : dict or None, optional
         Keyword arguments for the lines between the snow layers. The default is
         None which sets reasonable defaults.
+    colorbar : bool
+        Whether to plot a colorbar or not.
     cax_kwargs : dict or None, optional
         Keyword arguments passed to :func:`matplotlib.colorbar.make_axes`. The default
         is None.
     Returns
     -------
     None.
 
     Notes
     -----
-    If `color_variable` is not None, the performance will be very poor and 
-    plotting takes a lot of time.
+    If `color_variable` is not None, plotting is slower than without any coloring
+    of the layers.
 
     Examples
     --------
     Examples are given in :ref:`the respective section <layer_plot_example>`
     of the 1d example notebook. 
     """
     d_large = ds.copy()
 
     if color_variable is not None:
         # drop=True leads to reduced array for faster plotting:
         d_small = d_large.where(d_large['layer_heights'] != 0, drop=True)
         d_small['layer_tops'] = d_small['layer_heights'].cumsum(dim='layers', skipna=True)
         color_norm = mpl.colors.Normalize(vmin=vmin, vmax=vmax, clip=True)
         color_mapper = mpl.cm.ScalarMappable(norm=color_norm, cmap=cmap)
-        for l in d_small['layers'].to_index():
-            for t in d_small['time'].to_index():
-                if not np.isnan(d_small['layer_heights'].sel(layers=l, time=t)):
-                    polygon = mpl.patches.Rectangle(
-                        # xy defines lower left corner of Rectange:
-                        xy=(mpl.dates.date2num(t)-0.5, # center over the day
-                            float(d_small['layer_tops'].sel(layers=l, time=t)-d_small['layer_heights'].sel(layers=l, time=t)) # get bottom of layer
-                            ),
-                        width=1, # one day has width of 1
-                        height=float(d_small['layer_heights'].sel(layers=l, time=t)),
-                        edgecolor=None,
-                        facecolor=color_mapper.to_rgba(
-                            float(d_small[color_variable].sel(layers=l, time=t))
-                            )
-                        )
-                    ax.add_patch(polygon)
+
+        for t in d_small['time'].to_index():
+            tops = d_small['layer_tops'].sel(time=t).to_numpy()
+            colors = d_small[color_variable].sel(time=t).to_numpy()
+            # removing nans from tops and colors
+            tops = tops[~np.isnan(colors)]
+            colors = colors[~np.isnan(colors)]
+            # add zero to beginning of tops 
+            # for flat shading in pcolormesh, Z needs to be smaller than x and y
+            y = np.concatenate((np.array([0]), tops))
+            Z = colors.reshape(len(colors), 1)
+            x = [mpl.dates.date2num(t)-0.5, mpl.dates.date2num(t)+0.5]
+            ax.pcolormesh(
+                x,
+                y,
+                Z,
+                shading='flat',
+                cmap=cmap,
+                norm=color_norm)
 
     # we now need the complete time index for layertops to go to zero. Otherwise
     # there would be nans and and the layertops would be connected from arbitrary
     # locations
     d_large['layer_tops'] = d_large['layer_heights'].cumsum(dim='layers', skipna=True)
+    # remove layers with nan in color variable in order to avoid the same layer 
+    # border to be drawn several times
+    tops = (d_large['layer_tops']
+        .where(
+            ~np.isnan(d_large['layer_densities']).all(dim='time'),
+            drop=True
+        )
+    )
     # draw layerborders
     l_kwargs = {'lw': 0.5, 'c': 'k'}
     if layer_line_kwargs is not None:
         l_kwargs.update(layer_line_kwargs)
-    ax.plot(d_large['time'].to_index(), d_large['layer_tops'].to_numpy().T, **l_kwargs)
+    ax.plot(d_large['time'].to_index(), tops.to_numpy().T, **l_kwargs)
     # draw line at top of the snowcover
     t_kwargs = {'lw': 2, 'c': 'k', 'label': 'HS modeled'}
     if top_line_kwargs is not None:
         t_kwargs.update(top_line_kwargs)
     ax.plot(d_large['time'].to_index(), d_large['hs'].to_pandas(), **t_kwargs)
 
-    if color_variable is not None:
+    if color_variable is not None and colorbar:
         c_kwargs = {'pad': 0.01}
         if cax_kwargs is not None:
             c_kwargs.update(cax_kwargs)
         cax, _ = mpl.colorbar.make_axes(ax, **c_kwargs)
         cbar = plt.colorbar(color_mapper, cax, ax)
         cbar.set_label(cbar_label)
     return None
```

### Comparing `swe2hs-1.0.3/src/swe2hs.egg-info/PKG-INFO` & `swe2hs-1.0.4/src/swe2hs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swe2hs
-Version: 1.0.3
+Version: 1.0.4
 Summary: Conceptual snow density model for transferring snow water equivalent to snow depth.
 Home-page: https://code.wsl.ch/aschauer/swe2hs
 Author: Johannes Aschauer
 Author-email: johannes.aschauer@slf.ch
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://aschauer.gitlab-pages.wsl.ch/swe2hs/
 Project-URL: Changelog, https://aschauer.gitlab-pages.wsl.ch/swe2hs/changelog.html
@@ -49,29 +49,36 @@
 equivalent (SWE) of the snow cover to snow depth (HS). Some people informally 
 call it JOPACK, which is an acronym for Just density Of the snowPACK.
 
 The density model calculates snow depth at a daily resolution and is 
 driven by the daily snow water equivalent of the snow cover only. The 
 model creates a new layer with a fixed new snow density :math:`\rho_{new}` for
 every increase in SWE such that, over time, a snowpack of individual layers 
-builds up. The density of a layer increases exponentially with time towards 
-a time-varying maximum density. The maximum density is starting with an initial 
-value at creation time of the layer and is subsequently increasing towards 
+builds up. The density of a layer increases with an exponential decay function towards 
+a time-varying maximum density. The maximum density starts with an initial 
+value at creation time of the layer and subsequently increases towards 
 a higher value based on the overburden a layer has experienced and the 
 occurrence of SWE losses in the snow pack. When SWE decreases, the model 
-removes SWE from the top of the snowpack. The layer number :math:`n` can thus
+removes layers from the top of the snowpack. The layer number :math:`n` can thus
 undergo changes over time based on the number of SWE increases and losses in 
 the snowpack. The model neglects constructive metamorphism, refreezing, and 
-is not able to capture rain-on-snow (ROS) events which might lead to an 
-increase in SWE but no increase in HS. 
+is not able to capture rain-on-snow events which might lead to an 
+increase in SWE but no increase in snow depth.
+
+Citation
+========
+
+For more information on the model and how it was calibrated, please refer to the 
+model description paper:
+
+Aschauer, J.; Michel, A.; Jonas, T.; Marty, C., 2023: An empirical model to 
+calculate snow depth from daily snow water equivalent: SWE2HS 1.0. 
+Geoscientific Model Development, 16, 14: 4063-4081. doi: 
+`10.5194/gmd-16-4063-2023 <https://doi.org/10.5194/gmd-16-4063-2023>`_ 
 
-.. TODO: add the following paragraph once the paper is published:
-.. For further information on the model and how it was calibrated please refer to the 
-.. model description paper:
-.. CITATION HERE.
 .. end_intro
 
 |
 
 .. image:: https://code.wsl.ch/aschauer/swe2hs/-/raw/master/docs/_static/colored_layers_kuhtai_2002.png
    :alt: Schematic snowpack evolution
 
@@ -170,12 +177,14 @@
 .. _new issue: https://code.wsl.ch/aschauer/swe2hs/-/issues/new
 .. _existing issues: https://code.wsl.ch/aschauer/swe2hs/-/issues
 
 .. end_help
 
 .. start_bib
 
+|
+
 .. [#Krajci2017] Krajci, P., Kirnbauer, R., Parajka, J., Schöber, J., & Blöschl, G. (2017). The Kühtai 
    data set: 25 years of lysimetric, snow pillow, and meteorological measurements, 
    *Water Resources Research*, 53, 5158-5165, https://doi.org/10.1002/2017WR020445.
 .. end_bib
```

### Comparing `swe2hs-1.0.3/src/swe2hs.egg-info/SOURCES.txt` & `swe2hs-1.0.4/src/swe2hs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swe2hs-1.0.3/tests/conftest.py` & `swe2hs-1.0.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swe2hs-1.0.3/tests/test_core.py` & `swe2hs-1.0.4/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `swe2hs-1.0.3/tests/test_one_dimensional.py` & `swe2hs-1.0.4/tests/test_one_dimensional.py`

 * *Files identical despite different names*

### Comparing `swe2hs-1.0.3/tests/test_stepwise.py` & `swe2hs-1.0.4/tests/test_stepwise.py`

 * *Files identical despite different names*

### Comparing `swe2hs-1.0.3/tests/test_two_dimensional.py` & `swe2hs-1.0.4/tests/test_two_dimensional.py`

 * *Files identical despite different names*

### Comparing `swe2hs-1.0.3/tests/test_utils.py` & `swe2hs-1.0.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `swe2hs-1.0.3/tests/test_visualization.py` & `swe2hs-1.0.4/tests/test_visualization.py`

 * *Files identical despite different names*

### Comparing `swe2hs-1.0.3/tox.ini` & `swe2hs-1.0.4/tox.ini`

 * *Files identical despite different names*

