# Comparing `tmp/circuitpython-uplot-1.0.1.tar.gz` & `tmp/circuitpython-uplot-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-uplot-1.0.1.tar", last modified: Sat Jul 29 19:03:18 2023, max compression
+gzip compressed data, was "circuitpython-uplot-1.1.1.tar", last modified: Mon Jul 31 21:50:23 2023, max compression
```

## Comparing `circuitpython-uplot-1.0.1.tar` & `circuitpython-uplot-1.1.1.tar`

### file list

```diff
@@ -1,122 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:03:18.111083 circuitpython-uplot-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:03:18.087084 circuitpython-uplot-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:03:18.087084 circuitpython-uplot-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-07-29 19:03:18.111083 circuitpython-uplot-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:03:18.091084 circuitpython-uplot-1.0.1/circuitpython_uplot/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/circuitpython_uplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11810 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/circuitpython_uplot/bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/circuitpython_uplot/cartesian.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/circuitpython_uplot/fillbetween.py
--rw-r--r--   0 runner    (1001) docker     (123)    22247 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/circuitpython_uplot/icons.py
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/circuitpython_uplot/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/circuitpython_uplot/map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/circuitpython_uplot/pie.py
--rw-r--r--   0 runner    (1001) docker     (123)    14594 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/circuitpython_uplot/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/circuitpython_uplot/polar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/circuitpython_uplot/scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/circuitpython_uplot/shade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/circuitpython_uplot/svg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:03:18.091084 circuitpython-uplot-1.0.1/circuitpython_uplot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-07-29 19:03:18.000000 circuitpython-uplot-1.0.1/circuitpython_uplot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-07-29 19:03:18.000000 circuitpython-uplot-1.0.1/circuitpython_uplot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 19:03:18.000000 circuitpython-uplot-1.0.1/circuitpython_uplot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-29 19:03:18.000000 circuitpython-uplot-1.0.1/circuitpython_uplot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 19:03:18.000000 circuitpython-uplot-1.0.1/circuitpython_uplot.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:03:18.103083 circuitpython-uplot-1.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:03:18.103083 circuitpython-uplot-1.0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10445 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/bar_example.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    13469 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/bar_palette.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    16680 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/bar_scale.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    24099 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/cartesian_trig_functions.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12802 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/fillbetween_example.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)   107604 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/lissajous.jpg
--rw-r--r--   0 runner    (1001) docker     (123)  3215396 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/logging.png
--rw-r--r--   0 runner    (1001) docker     (123)    19404 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/logging_fill.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    14791 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/logging_table.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    34215 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/map.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/plot_simple_test.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   110829 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/polar_advanced.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    37528 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/polar_example.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    59396 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/polar_plots.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    14534 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/quick_start.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/readme.png
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/readme2.png
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    67674 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/scatter.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    20454 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/uplot_3DBars.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   221907 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/uplot_cartesian.gif
--rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/uplot_cartesian_advance.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    22878 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/uplot_ex10.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    13589 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/uplot_ex12.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/uplot_ex16.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    22907 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/uplot_ex3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    10823 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/uplot_ex4.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    12133 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/uplot_ex5.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/uplot_ex6.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    10973 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/uplot_pie.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    65562 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/uplot_shade.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    23581 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/docs/uplot_svg.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:03:18.111083 circuitpython-uplot-1.0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/examples/cartesian_trig_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 19:03:18.111083 circuitpython-uplot-1.0.1/examples/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    86848 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/examples/fonts/LeagueSpartan-Bold-16.bdf
--rw-r--r--   0 runner    (1001) docker     (123)    68124 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/examples/fonts/LibreBodoniv2002-Bold-10.bdf
--rw-r--r--   0 runner    (1001) docker     (123)    85245 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/examples/fonts/LibreBodoniv2002-Regular-17.bdf
--rwxr-xr-x   0 runner    (1001) docker     (123)   408924 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/examples/fonts/forkawesome-36.pcf
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/examples/fonts/forkawesome-36.pcf.license
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/examples/lissajous_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/examples/plot_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/examples/polar_advanced.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/examples/uplot_bar_3Dbars.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/examples/uplot_bar_color_changing.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/examples/uplot_bar_colorpalette.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/examples/uplot_bar_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/examples/uplot_bar_scale_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/examples/uplot_bar_updating_values.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/examples/uplot_cartesian_advanced.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/examples/uplot_cartesian_loggin_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/examples/uplot_cartesian_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/examples/uplot_display_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/examples/uplot_fillbetween.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/examples/uplot_integration_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/examples/uplot_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/examples/uplot_logging_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/examples/uplot_logging_changing_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/examples/uplot_logging_fill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/examples/uplot_logging_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/examples/uplot_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/examples/uplot_pie_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/examples/uplot_plot_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/examples/uplot_polar_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/examples/uplot_polar_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/examples/uplot_readme_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/examples/uplot_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/examples/uplot_shade_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/examples/uplot_sparkline.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/examples/uplot_stackplot.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/examples/uplot_svg_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/examples/uplot_tickparameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/examples/uplot_uboxplot.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-29 19:03:08.000000 circuitpython-uplot-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-29 19:02:58.000000 circuitpython-uplot-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 19:03:18.111083 circuitpython-uplot-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:50:23.678046 circuitpython-uplot-1.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:50:23.654046 circuitpython-uplot-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:50:23.658046 circuitpython-uplot-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-07-31 21:50:23.678046 circuitpython-uplot-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:50:23.658046 circuitpython-uplot-1.1.1/circuitpython_uplot/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/circuitpython_uplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11810 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/circuitpython_uplot/bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/circuitpython_uplot/cartesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/circuitpython_uplot/fillbetween.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22247 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/circuitpython_uplot/icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/circuitpython_uplot/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/circuitpython_uplot/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/circuitpython_uplot/pie.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15659 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/circuitpython_uplot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/circuitpython_uplot/polar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/circuitpython_uplot/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/circuitpython_uplot/shade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/circuitpython_uplot/svg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:50:23.658046 circuitpython-uplot-1.1.1/circuitpython_uplot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-07-31 21:50:23.000000 circuitpython-uplot-1.1.1/circuitpython_uplot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-31 21:50:23.000000 circuitpython-uplot-1.1.1/circuitpython_uplot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 21:50:23.000000 circuitpython-uplot-1.1.1/circuitpython_uplot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-31 21:50:23.000000 circuitpython-uplot-1.1.1/circuitpython_uplot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-31 21:50:23.000000 circuitpython-uplot-1.1.1/circuitpython_uplot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:50:23.670046 circuitpython-uplot-1.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    20454 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/3DBars.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:50:23.670046 circuitpython-uplot-1.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10445 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/bar_example.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    13469 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/bar_palette.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    16680 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/bar_scale.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/cartesian_advance.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   221907 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/cartesian_logging_data.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    86420 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/cartesian_scatter_polyfit.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    24099 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/cartesian_trig_functions.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/display_shapes.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12802 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/fillbetween_example.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12133 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/integration_example.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    24305 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/line_style.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   107604 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/lissajous.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)  3215396 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/logging.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19404 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/logging_fill.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    22764 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/logging_limits.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    14791 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/logging_table.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    34215 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/map.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    10973 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/pie.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    10823 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/plot_example.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/plot_simple_test.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   110829 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/polar_advanced.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    37528 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/polar_example.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    59396 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/polar_plots.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    15254 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/quick_start.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/readme.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/readme2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    67674 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/scatter.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   127777 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/scatter_circle_radius.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   109739 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/scatter_pointers.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   102046 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/scatter_using_different_datasets.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    65562 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/shade.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    13589 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/stackplot_example.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    23581 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/svg.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    22907 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/tickparameters.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/docs/uboxplot_example.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:50:23.674046 circuitpython-uplot-1.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/bar_3Dbars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/bar_color_changing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/bar_colorpalette.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/bar_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/bar_scale_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/bar_updating_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/cartersian_and_scatter_polyfit_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/cartesian_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/cartesian_logging_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/cartesian_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/cartesian_trig_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/display_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/fillbetween.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:50:23.674046 circuitpython-uplot-1.1.1/examples/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    86848 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/examples/fonts/LeagueSpartan-Bold-16.bdf
+-rw-r--r--   0 runner    (1001) docker     (123)    68124 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/examples/fonts/LibreBodoniv2002-Bold-10.bdf
+-rw-r--r--   0 runner    (1001) docker     (123)    85245 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/examples/fonts/LibreBodoniv2002-Regular-17.bdf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   408924 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/examples/fonts/forkawesome-36.pcf
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/examples/fonts/forkawesome-36.pcf.license
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/integration_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/lissajous_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/logging_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/logging_changing_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/logging_fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/logging_limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/logging_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/pie_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/plot_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/plot_line_styles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/plot_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/polar_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/polar_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/polar_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/readme_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/scatter_circle_radius.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/scatter_pointers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/scatter_using_different_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/shade_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/sparkline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/stackplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/svg_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/tickparameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/examples/uboxplot_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-31 21:50:16.000000 circuitpython-uplot-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-31 21:50:08.000000 circuitpython-uplot-1.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 21:50:23.678046 circuitpython-uplot-1.1.1/setup.cfg
```

### Comparing `circuitpython-uplot-1.0.1/.github/workflows/release_gh.yml` & `circuitpython-uplot-1.1.1/.github/workflows/release_gh.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/.pre-commit-config.yaml` & `circuitpython-uplot-1.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/.pylintrc` & `circuitpython-uplot-1.1.1/.pylintrc`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 valid-classmethod-first-arg=cls
 valid-metaclass-classmethod-first-arg=mcs
 
 [DESIGN]
 max-args=15
 max-attributes=30
 max-bool-expr=5
-max-branches=20
+max-branches=25
 max-locals=25
 max-parents=7
 max-public-methods=20
 max-returns=6
 max-statements=60
 min-public-methods=0
```

### Comparing `circuitpython-uplot-1.0.1/LICENSE` & `circuitpython-uplot-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/PKG-INFO` & `circuitpython-uplot-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-uplot
-Version: 1.0.1
+Version: 1.1.1
 Summary: framework to display different plots in displayio. similar to widget
 Author-email: JDM <uplot@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_uplot
 Keywords: circuitpython,uplot,bar,stackplot,fillbetween,piechart,scatter,line,displayio,graphics,library,ulab,svg,widget,graph,graphing,chart,charts,plotting,plot,plotter
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -42,15 +42,15 @@
 For detailed view of the library please refer to the `Quick start guide <https://circuitpython-uplot.readthedocs.io/>`_
 
 .. image:: https://github.com/jposada202020/CircuitPython_uplot/blob/main/docs/readme.png
 
 .. image:: https://github.com/jposada202020/CircuitPython_uplot/blob/main/docs/readme2.png
 
 
-Below a picture oa a real live application. for more information visit the project `page <https://github.com/casainho/temperature_humidity_sensor_eink_display>`_. Thanks to @Casainho
+Below a picture of a real live application. for more information visit the project `page <https://github.com/casainho/temperature_humidity_sensor_eink_display>`_. Thanks to @Casainho
 
 .. image:: https://github.com/jposada202020/CircuitPython_uplot/blob/main/docs/logging.png
 
 
 Dependencies
 =============
 This library depends on:
```

### Comparing `circuitpython-uplot-1.0.1/README.rst` & `circuitpython-uplot-1.1.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 For detailed view of the library please refer to the `Quick start guide <https://circuitpython-uplot.readthedocs.io/>`_
 
 .. image:: https://github.com/jposada202020/CircuitPython_uplot/blob/main/docs/readme.png
 
 .. image:: https://github.com/jposada202020/CircuitPython_uplot/blob/main/docs/readme2.png
 
 
-Below a picture oa a real live application. for more information visit the project `page <https://github.com/casainho/temperature_humidity_sensor_eink_display>`_. Thanks to @Casainho
+Below a picture of a real live application. for more information visit the project `page <https://github.com/casainho/temperature_humidity_sensor_eink_display>`_. Thanks to @Casainho
 
 .. image:: https://github.com/jposada202020/CircuitPython_uplot/blob/main/docs/logging.png
 
 
 Dependencies
 =============
 This library depends on:
```

### Comparing `circuitpython-uplot-1.0.1/circuitpython_uplot/bar.py` & `circuitpython-uplot-1.1.1/circuitpython_uplot/bar.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 except ImportError:
     pass
 from math import sin, cos, ceil
 from displayio import Palette
 from bitmaptools import draw_line
 from vectorio import Rectangle, Polygon
 
-__version__ = "1.0.1"
+__version__ = "1.1.1"
 __repo__ = "https://github.com/adafruit/CircuitPython_uplot.git"
 
 # pylint: disable=protected-access
 # pylint: disable=no-self-use
 
 
 class Bar:
```

### Comparing `circuitpython-uplot-1.0.1/circuitpython_uplot/cartesian.py` & `circuitpython-uplot-1.1.1/circuitpython_uplot/polar.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,146 +1,156 @@
 # SPDX-FileCopyrightText: Copyright (c) 2023 Jose D. Montoya
 #
 # SPDX-License-Identifier: MIT
 
 """
 
-`cartesian`
+`polar`
 ================================================================================
 
-CircuitPython cartesian graph
+CircuitPython Polar graph
 
 * Author(s): Jose D. Montoya
 
 
 """
 try:
     from typing import Optional, Union
     from circuitpython_uplot.plot import Plot
 except ImportError:
     pass
-from bitmaptools import draw_line, fill_region
+from bitmaptools import draw_line, draw_circle
 from ulab import numpy as np
-from vectorio import Polygon
 
-__version__ = "1.0.1"
+__version__ = "0.11.0"
 __repo__ = "https://github.com/adafruit/CircuitPython_uplot.git"
 
 
-class Cartesian:
+# pylint: disable=dangerous-default-value
+class Polar:
     """
-    Class to draw cartesian plane
+    Class to draw polar plots
     """
 
     def __init__(
         self,
         plot: Plot,
-        x: Union[list, np.linspace, np.ndarray],
-        y: Union[list, np.linspace, np.ndarray],
+        radius: Union[list, np.linspace, np.ndarray],
+        theta: Union[list, np.linspace, np.ndarray],
         rangex: Optional[list] = None,
         rangey: Optional[list] = None,
         line_color: Optional[int] = None,
-        fill: bool = False,
+        polar_plot_line_color: int = 0x647182,
         nudge: bool = True,
-        logging: bool = False,
+        radius_ticks: list = [1.0, 2.0],
     ) -> None:
         """
 
         :param Plot plot: Plot object for the scatter to be drawn
-        :param list|ulab.numpy.linspace|ulab.numpy.ndarray x: x points coordinates
-        :param list|ulab.numpy.linspace|ulab.numpy.ndarray y: y points coordinates
+        :param list|ulab.numpy.linspace|ulab.numpy.ndarray radius: radius points
+        :param list|ulab.numpy.linspace|ulab.numpy.ndarray theta: theta points
         :param list|None rangex: x range limits. Defaults to None
         :param list|None rangey: y range limits. Defaults to None
         :param int|None line_color: line color. Defaults to None
         :param bool fill: Show the filling. Defaults to `False`
         :param bool nudge: moves the graph a little for better displaying. Defaults to `True`
-        :param bool logging: used to change the logic of the cartesian to work as a logger
 
         """
-        self.points = []
+
+        angles_list = [45, 90, 135, 180, 225, 270, 315, 360]
+        angles = np.ndarray(angles_list, dtype=np.int16)
+
+        self.angle_radians = np.radians(angles)
+        self._color_index = plot._index_colorused + 1
 
         if line_color is not None:
             plot._plot_palette[plot._index_colorused] = line_color
 
+        plot._plot_palette[self._color_index] = polar_plot_line_color
+
         if nudge:
             nudge_factor = 1
         else:
             nudge_factor = 0
 
         if rangex is None:
-            xmin = np.min(x) - nudge_factor * (abs(np.max(x) - np.min(x)) / 10)
-            xmax = np.max(x) + nudge_factor * (abs(np.max(x) - np.min(x)) / 10)
+            xmin = np.min(radius) - nudge_factor * (
+                abs(np.max(radius) - np.min(radius)) / 10
+            )
+            xmax = np.max(radius) + nudge_factor * (
+                abs(np.max(radius) - np.min(radius)) / 10
+            )
         else:
             xmin = min(rangex)
             xmax = max(rangex)
 
         if rangey is None:
-            ymin = np.min(y) - nudge_factor * (abs(np.max(y) - np.min(y)) / 10)
-            ymax = np.max(y) + nudge_factor * (abs(np.max(y) - np.min(y)) / 10)
+            ymin = np.min(theta) - nudge_factor * (
+                abs(np.max(theta) - np.min(theta)) / 10
+            )
+            ymax = np.max(theta) + nudge_factor * (
+                abs(np.max(theta) - np.min(theta)) / 10
+            )
         else:
             ymin = min(rangey)
             ymax = max(rangey)
 
-        x = np.array(x)
-        y = np.array(y)
-
         xnorm = np.array(
-            plot.transform(xmin, xmax, plot._newxmin, plot._newxmax, x),
+            plot.transform(
+                xmin,
+                xmax,
+                plot._newxmin,
+                plot._newxmax,
+                np.cos(np.array(radius)) * np.array(theta),
+            ),
             dtype=np.int16,
         )
         ynorm = np.array(
-            plot.transform(ymin, ymax, plot._newymin, plot._newymax, y),
+            plot.transform(
+                ymin,
+                ymax,
+                plot._newymin,
+                plot._newymax,
+                np.sin(np.array(radius)) * np.array(theta),
+            ),
             dtype=np.int16,
         )
 
-        if fill:
-            self.points.append((xnorm[0], plot._newymin))
-            for index, item in enumerate(xnorm):
-                self.points.append((item, ynorm[index]))
-            self.points.append((xnorm[-1], plot._newymin))
-            self.points.append((xnorm[0], plot._newymin))
-            plot.append(
-                Polygon(
-                    pixel_shader=plot._plot_palette,
-                    points=self.points,
-                    x=0,
-                    y=0,
-                    color_index=plot._index_colorused,
-                )
+        rnorm = np.array(
+            plot.transform(
+                0, xmax, plot._newxmin, plot._newxmax, np.array(radius_ticks)
+            ),
+            dtype=np.int16,
+        )
+
+        self.originx = int(plot.transform(xmin, xmax, plot._newxmin, plot._newxmax, 0))
+        self.originy = int(plot.transform(ymin, ymax, plot._newymin, plot._newymax, 0))
+
+        for index, _ in enumerate(xnorm):
+            if index + 1 >= len(xnorm):
+                break
+            if theta[index] >= ymax:
+                continue
+            draw_line(
+                plot._plotbitmap,
+                xnorm[index],
+                ynorm[index],
+                xnorm[index + 1],
+                ynorm[index + 1],
+                plot._index_colorused,
+            )
+        for radius_norm in rnorm:
+            draw_circle(
+                plot._plotbitmap,
+                self.originx,
+                self.originy,
+                radius_norm // 2,
+                self._color_index,
             )
-        else:
-            if logging:
-                fill_region(
-                    plot._plotbitmap,
-                    plot._newxmin + plot._tickheightx + 1,
-                    plot._newymax + 1,
-                    plot._newxmax - 1,
-                    plot._newymin - plot._tickheighty,
-                    0,
-                )
-
-            for index, _ in enumerate(xnorm):
-                if index + 1 >= len(xnorm):
-                    break
-                if y[index] >= ymax:
-                    continue
-                draw_line(
-                    plot._plotbitmap,
-                    xnorm[index],
-                    ynorm[index],
-                    xnorm[index + 1],
-                    ynorm[index + 1],
-                    plot._index_colorused,
-                )
-        if plot._showticks:
-            if plot._cartesianfirst:
-                if logging:
-                    x = np.linspace(xmin, xmax, 100)
-                    y = np.linspace(ymin, ymax, 100)
-                plot._draw_ticks(x, y)
-                plot._cartesianfirst = False
-                plot._showticks = False
 
-        if logging:
-            plot._index_colorused = plot._index_colorused
-        else:
-            plot._index_colorused = plot._index_colorused + 1
+        for element in self.angle_radians:
+            x = self.originx + int(np.cos(element) * rnorm[-1] // 2)
+            y = self.originy + int(np.sin(element) * rnorm[-1] // 2)
+
+            draw_line(
+                plot._plotbitmap, self.originx, self.originy, x, y, self._color_index
+            )
```

### Comparing `circuitpython-uplot-1.0.1/circuitpython_uplot/fillbetween.py` & `circuitpython-uplot-1.1.1/circuitpython_uplot/fillbetween.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     from circuitpython_uplot.plot import Plot
 except ImportError:
     pass
 from ulab import numpy as np
 from vectorio import Polygon
 
 
-__version__ = "1.0.1"
+__version__ = "1.1.1"
 __repo__ = "https://github.com/adafruit/CircuitPython_uplot.git"
 
 
 class Fillbetween:
     """
     Class to draw a fillbetween graph
     """
```

### Comparing `circuitpython-uplot-1.0.1/circuitpython_uplot/icons.py` & `circuitpython-uplot-1.1.1/circuitpython_uplot/icons.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/circuitpython_uplot/logging.py` & `circuitpython-uplot-1.1.1/circuitpython_uplot/logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 CircuitPython logging data graph
 
 * Author(s): Jose D. Montoya
 
 
 """
 try:
-    from typing import Union
+    from typing import Union, Optional
     from circuitpython_uplot.plot import Plot
 except ImportError:
     pass
 from bitmaptools import draw_line, fill_region
 from ulab import numpy as np
 
-__version__ = "1.0.1"
+__version__ = "1.1.1"
 __repo__ = "https://github.com/adafruit/CircuitPython_uplot.git"
 
 
 class Logging:
     """
     Class to log data
     """
@@ -38,14 +38,16 @@
         rangex: list,
         rangey: list,
         line_color: int = 0xFFFFFF,
         ticksx: Union[np.array, list] = np.array([0, 10, 30, 50, 70, 90]),
         ticksy: Union[np.array, list] = np.array([0, 10, 30, 50, 70, 90]),
         tick_pos: bool = False,
         fill: bool = False,
+        limits: Optional[list] = None,
+        limits_color: int = 0xFF0000,
     ) -> None:
         """
 
         :param Plot plot: Plot object for the log to be drawn
         :param list|ulab.numpy.linspace|ulab.numpy.ndarray x: x points coordinates
         :param list|ulab.numpy.linspace|ulab.numpy.ndarray y: y points coordinates
         :param list|None rangex: x range limits. Defaults to None
@@ -66,19 +68,30 @@
             self._tickposy = plot._tickheighty
         else:
             self._tickposx = 0
             self._tickposy = 0
 
         plot._plot_palette[plot._index_colorused] = line_color
 
+        self._line_index = plot._index_colorused
+
         self.xmin = rangex[0]
         self.xmax = rangex[1]
         self.ymin = rangey[0]
         self.ymax = rangey[1]
 
+        if limits is not None:
+            self._limits = np.array(
+                plot.transform(
+                    self.ymin, self.ymax, plot._newymin, plot._newymax, np.array(limits)
+                ),
+                dtype=np.int16,
+            )
+            plot._plot_palette[9] = limits_color
+
         self.draw_points(plot, x, y, fill)
 
         if plot._showticks:
             if plot._loggingfirst:
                 self._draw_ticks(plot)
                 plot._loggingfirst = False
                 plot._showticks = False
@@ -182,19 +195,37 @@
                     break
                 draw_line(
                     plot._plotbitmap,
                     xnorm[index],
                     ynorm[index],
                     xnorm[index + 1],
                     ynorm[index + 1],
-                    plot._index_colorused,
+                    self._line_index,
                 )
             if fill:
                 for index, _ in enumerate(xnorm):
                     draw_line(
                         plot._plotbitmap,
                         xnorm[index],
                         ynorm[index],
                         xnorm[index],
                         plot._newymin,
-                        plot._index_colorused,
+                        self._line_index,
                     )
+
+    def _draw_limit_lines(self, plot: Plot) -> None:
+        draw_line(
+            plot._plotbitmap,
+            plot._newxmin,
+            self._limits[0],
+            plot._newxmax,
+            self._limits[0],
+            9,
+        )
+        draw_line(
+            plot._plotbitmap,
+            plot._newxmin,
+            self._limits[1],
+            plot._newxmax,
+            self._limits[1],
+            9,
+        )
```

### Comparing `circuitpython-uplot-1.0.1/circuitpython_uplot/map.py` & `circuitpython-uplot-1.1.1/circuitpython_uplot/map.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 except ImportError:
     pass
 
 from ulab import numpy as np
 import displayio
 from vectorio import Rectangle
 
-__version__ = "1.0.1"
+__version__ = "1.1.1"
 __repo__ = "https://github.com/adafruit/CircuitPython_uplot.git"
 
 
 class Map:
     """
     Main class to display different graphics
     """
```

### Comparing `circuitpython-uplot-1.0.1/circuitpython_uplot/pie.py` & `circuitpython-uplot-1.1.1/circuitpython_uplot/pie.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 except ImportError:
     pass
 
 
 import math
 from vectorio import Polygon
 
-__version__ = "1.0.1"
+__version__ = "1.1.1"
 __repo__ = "https://github.com/adafruit/CircuitPython_uplot.git"
 
 
 class Pie:
     """
     Class to draw pie
     """
```

### Comparing `circuitpython-uplot-1.0.1/circuitpython_uplot/plot.py` & `circuitpython-uplot-1.1.1/circuitpython_uplot/plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 import displayio
 import terminalio
 from bitmaptools import draw_line
 from vectorio import Circle
 from ulab import numpy as np
 
 
-__version__ = "1.0.1"
+__version__ = "1.1.1"
 __repo__ = "https://github.com/jposada202020/CircuitPython_uplot.git"
 
 
 class Plot(displayio.Group):
     """
     Canvas Class to add different elements to the screen.
     The origin point set by ``x`` and ``y`` properties
@@ -105,14 +105,15 @@
         self._newxmax = width - padding - 1
 
         self._newymin = height - padding - 1
         self._newymax = padding
 
         self._cartesianfirst = True
         self._loggingfirst = True
+        self._scatterfirst = True
 
         self._showtext = False
 
         self._tickheightx = tickx_height
         self._tickheighty = ticky_height
         self._tickcolor = 0xFFFFFF
         self._showticks = False
@@ -123,15 +124,15 @@
 
         self._barcolor = 0x69FF8F
 
         self._piecolor = 0x8B77FF
 
         self._index_colorused = 4
 
-        self._plotbitmap = displayio.Bitmap(width, height, 20)
+        self._plotbitmap = displayio.Bitmap(width, height, 10)
 
         if show_box:
             self._drawbox()
 
         self._plot_palette = displayio.Palette(20)
         self._plot_palette[0] = background_color
         self._plot_palette[1] = box_color
@@ -319,28 +320,34 @@
                 self._newymin,
                 tick,
                 self._newymin - self._tickheightx,
                 2,
             )
             if self._showtext:
                 self.show_text(
-                    "{:.2f}".format(ticksxnorm[i]), tick, self._newymin, (0.5, 0.0)
+                    "{:.{}f}".format(ticksxnorm[i], self._decimal_points),
+                    tick,
+                    self._newymin,
+                    (0.5, 0.0),
                 )
         for i, tick in enumerate(ticksyrenorm):
             draw_line(
                 self._plotbitmap,
                 self._newxmin,
                 tick,
                 self._newxmin + self._tickheighty,
                 tick,
                 2,
             )
             if self._showtext:
                 self.show_text(
-                    "{:.2f}".format(ticksynorm[i]), self._newxmin, tick, (1.0, 0.5)
+                    "{:.{}f}".format(ticksynorm[i], self._decimal_points),
+                    self._newxmin,
+                    tick,
+                    (1.0, 0.5),
                 )
         for tick in subticksxrenorm:
             draw_line(
                 self._plotbitmap,
                 tick,
                 self._newymin,
                 tick,
@@ -365,34 +372,42 @@
         self,
         show_ticks=True,
         tickx_height: int = 8,
         ticky_height: int = 8,
         tickcolor: int = 0xFFFFFF,
         tickgrid: bool = False,
         showtext: bool = False,
+        decimal_points: int = 0,
     ) -> None:
         """
         Function to set ticks parameters
 
+        :param bool show_ticks: Show ticks. Defaults to `True`
         :param int tickx_height: X axes tick height in pixels. Defaults to 8
         :param int ticky_height: Y axes tick height in pixels. Defaults to 8
         :param int tickcolor: tick color in hex. Defaults to white. ``0xFFFFFF``
         :param bool tickgrid: defines if the grid is to be shown. Defaults to `False`
         :param bool showtext: Show Axes text. Defaults to `False`
+        :param int decimal_points: Number of decimal points to show. Defaults to :const:`0`
 
         :return: None
 
         """
+        if showtext and self.padding < 20:
+            raise ValueError(
+                "Please select a padding that allows to show the tick text"
+            )
 
         self._showticks = show_ticks
         self._tickheightx = tickx_height
         self._tickheighty = ticky_height
         self._plot_palette[2] = tickcolor
         self._tickgrid = tickgrid
         self._showtext = showtext
+        self._decimal_points = decimal_points
         if self._showtext:
             from adafruit_display_text import bitmap_label
 
             self.bitmap_label = bitmap_label
 
     def _draw_gridx(self, ticks_data: list[int]) -> None:
         """
@@ -445,27 +460,43 @@
         :return: None
 
         """
 
         self._drawbox()
 
     def show_text(
-        self, text: str, x: int, y: int, anchorpoint: Tuple = (0.5, 0.0)
+        self,
+        text: str,
+        x: int,
+        y: int,
+        anchorpoint: Tuple = (0.5, 0.0),
+        text_color: int = 0xFFFFFF,
+        free_text: bool = False,
     ) -> None:
         """
 
         Show desired text in the screen
         :param str text: text to be displayed
         :param int x: x coordinate
         :param int y: y coordinate
         :param Tuple anchorpoint: Display_text anchor point. Defaults to (0.5, 0.0)
+        :param int color: text color. Defaults to :const:`0xFFFFFF`
+        :param bool free_text: Select to show free text
         :return: None
         """
-        if self._showtext:
-            text_toplot = self.bitmap_label.Label(terminalio.FONT, text=text, x=x, y=y)
+        try:
+            self.bitmap_label
+        except AttributeError:
+            from adafruit_display_text import bitmap_label
+
+            self.bitmap_label = bitmap_label
+        if self._showtext or free_text:
+            text_toplot = self.bitmap_label.Label(
+                terminalio.FONT, text=text, x=x, y=y, color=text_color
+            )
             text_toplot.anchor_point = anchorpoint
             text_toplot.anchored_position = (x, y)
             self.append(text_toplot)
 
 
 # pylint: disable=missing-class-docstring, too-few-public-methods, invalid-name
 class color:
```

### Comparing `circuitpython-uplot-1.0.1/circuitpython_uplot/shade.py` & `circuitpython-uplot-1.1.1/circuitpython_uplot/shade.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 # SPDX-License-Identifier: MIT
 
 """
 
 `shade`
 ================================================================================
 
-CircuitPython shade utility for uPlot.
+CircuitPython shade utility for Plotting.
 
 * Author(s): Jose D. Montoya
 
 
 """
 try:
     from typing import Optional, Union
     from circuitpython_uplot.plot import Plot
 except ImportError:
     pass
 from ulab import numpy as np
 from bitmaptools import fill_region
 
 
-__version__ = "1.0.1"
+__version__ = "1.1.1"
 __repo__ = "https://github.com/adafruit/CircuitPython_uplot.git"
 
 
 class shade:
     """
     Class to draw shade between two lines
     """
```

### Comparing `circuitpython-uplot-1.0.1/circuitpython_uplot/svg.py` & `circuitpython-uplot-1.1.1/circuitpython_uplot/svg.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 try:
     from circuitpython_uplot.plot import Plot
 except ImportError:
     pass
 from bitmaptools import draw_line
 
 
-__version__ = "1.0.1"
+__version__ = "1.1.1"
 __repo__ = "https://github.com/adafruit/CircuitPython_uplot.git"
 
 
 # pylint: disable=too-many-arguments, invalid-name, no-self-use, too-few-public-methods
 # pylint: disable=too-many-locals, too-many-branches, protected-access, unnecessary-list-index-lookup
 class SVG:
     """
```

### Comparing `circuitpython-uplot-1.0.1/circuitpython_uplot.egg-info/PKG-INFO` & `circuitpython-uplot-1.1.1/circuitpython_uplot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-uplot
-Version: 1.0.1
+Version: 1.1.1
 Summary: framework to display different plots in displayio. similar to widget
 Author-email: JDM <uplot@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_uplot
 Keywords: circuitpython,uplot,bar,stackplot,fillbetween,piechart,scatter,line,displayio,graphics,library,ulab,svg,widget,graph,graphing,chart,charts,plotting,plot,plotter
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -42,15 +42,15 @@
 For detailed view of the library please refer to the `Quick start guide <https://circuitpython-uplot.readthedocs.io/>`_
 
 .. image:: https://github.com/jposada202020/CircuitPython_uplot/blob/main/docs/readme.png
 
 .. image:: https://github.com/jposada202020/CircuitPython_uplot/blob/main/docs/readme2.png
 
 
-Below a picture oa a real live application. for more information visit the project `page <https://github.com/casainho/temperature_humidity_sensor_eink_display>`_. Thanks to @Casainho
+Below a picture of a real live application. for more information visit the project `page <https://github.com/casainho/temperature_humidity_sensor_eink_display>`_. Thanks to @Casainho
 
 .. image:: https://github.com/jposada202020/CircuitPython_uplot/blob/main/docs/logging.png
 
 
 Dependencies
 =============
 This library depends on:
```

### Comparing `circuitpython-uplot-1.0.1/circuitpython_uplot.egg-info/SOURCES.txt` & `circuitpython-uplot-1.1.1/circuitpython_uplot.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -24,88 +24,99 @@
 circuitpython_uplot/shade.py
 circuitpython_uplot/svg.py
 circuitpython_uplot.egg-info/PKG-INFO
 circuitpython_uplot.egg-info/SOURCES.txt
 circuitpython_uplot.egg-info/dependency_links.txt
 circuitpython_uplot.egg-info/requires.txt
 circuitpython_uplot.egg-info/top_level.txt
+docs/3DBars.jpg
 docs/api.rst
 docs/bar_example.jpg
 docs/bar_palette.jpg
 docs/bar_scale.jpg
+docs/cartesian_advance.jpg
+docs/cartesian_logging_data.gif
+docs/cartesian_scatter_polyfit.jpg
 docs/cartesian_trig_functions.jpg
 docs/conf.py
+docs/display_shapes.jpg
 docs/examples.rst
 docs/fillbetween_example.jpg
 docs/index.rst
+docs/integration_example.jpg
+docs/line_style.jpg
 docs/lissajous.jpg
 docs/logging.png
 docs/logging_fill.jpg
+docs/logging_limits.jpg
 docs/logging_table.jpg
 docs/map.jpg
+docs/pie.jpg
+docs/plot_example.jpg
 docs/plot_simple_test.jpg
 docs/polar_advanced.jpg
 docs/polar_example.jpg
 docs/polar_plots.jpg
 docs/quick_start.rst
 docs/readme.png
 docs/readme2.png
 docs/requirements.txt
 docs/scatter.jpg
-docs/uplot_3DBars.jpg
-docs/uplot_cartesian.gif
-docs/uplot_cartesian_advance.jpg
-docs/uplot_ex10.jpg
-docs/uplot_ex12.jpg
-docs/uplot_ex16.jpg
-docs/uplot_ex3.jpg
-docs/uplot_ex4.jpg
-docs/uplot_ex5.jpg
-docs/uplot_ex6.jpg
-docs/uplot_pie.jpg
-docs/uplot_shade.jpg
-docs/uplot_svg.jpg
+docs/scatter_circle_radius.jpg
+docs/scatter_pointers.jpg
+docs/scatter_using_different_datasets.jpg
+docs/shade.jpg
+docs/stackplot_example.jpg
+docs/svg.jpg
+docs/tickparameters.jpg
+docs/uboxplot_example.jpg
 docs/_static/Logo.png
 docs/_static/Logo.png.license
 docs/_static/extra_css.css
 docs/_static/extra_css.css.license
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
+examples/bar_3Dbars.py
+examples/bar_color_changing.py
+examples/bar_colorpalette.py
+examples/bar_example.py
+examples/bar_scale_example.py
+examples/bar_updating_values.py
+examples/cartersian_and_scatter_polyfit_example.py
+examples/cartesian_advanced.py
+examples/cartesian_logging_data.py
+examples/cartesian_table.py
 examples/cartesian_trig_functions.py
+examples/display_shapes.py
+examples/fillbetween.py
+examples/integration_example.py
 examples/lissajous_curves.py
+examples/logging.py
+examples/logging_animation.py
+examples/logging_changing_values.py
+examples/logging_fill.py
+examples/logging_limits.py
+examples/logging_table.py
+examples/map.py
+examples/pie_example.py
+examples/plot_example.py
+examples/plot_line_styles.py
 examples/plot_simpletest.py
 examples/polar_advanced.py
-examples/uplot_bar_3Dbars.py
-examples/uplot_bar_color_changing.py
-examples/uplot_bar_colorpalette.py
-examples/uplot_bar_example.py
-examples/uplot_bar_scale_example.py
-examples/uplot_bar_updating_values.py
-examples/uplot_cartesian_advanced.py
-examples/uplot_cartesian_loggin_data.py
-examples/uplot_cartesian_table.py
-examples/uplot_display_shapes.py
-examples/uplot_fillbetween.py
-examples/uplot_integration_example.py
-examples/uplot_logging.py
-examples/uplot_logging_animation.py
-examples/uplot_logging_changing_values.py
-examples/uplot_logging_fill.py
-examples/uplot_logging_table.py
-examples/uplot_map.py
-examples/uplot_pie_example.py
-examples/uplot_plot_example.py
-examples/uplot_polar_example.py
-examples/uplot_polar_plots.py
-examples/uplot_readme_example.py
-examples/uplot_scatter.py
-examples/uplot_shade_example.py
-examples/uplot_sparkline.py
-examples/uplot_stackplot.py
-examples/uplot_svg_example.py
-examples/uplot_tickparameters.py
-examples/uplot_uboxplot.py
+examples/polar_example.py
+examples/polar_plots.py
+examples/readme_example.py
+examples/scatter.py
+examples/scatter_circle_radius.py
+examples/scatter_pointers.py
+examples/scatter_using_different_datasets.py
+examples/shade_example.py
+examples/sparkline.py
+examples/stackplot.py
+examples/svg_example.py
+examples/tickparameters.py
+examples/uboxplot_example.py
 examples/fonts/LeagueSpartan-Bold-16.bdf
 examples/fonts/LibreBodoniv2002-Bold-10.bdf
 examples/fonts/LibreBodoniv2002-Regular-17.bdf
 examples/fonts/forkawesome-36.pcf
 examples/fonts/forkawesome-36.pcf.license
```

### Comparing `circuitpython-uplot-1.0.1/docs/_static/Logo.png` & `circuitpython-uplot-1.1.1/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/docs/_static/favicon.ico` & `circuitpython-uplot-1.1.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/docs/api.rst` & `circuitpython-uplot-1.1.1/docs/api.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Uplot Library
-==============
+Microplot Library
+======================
 
 .. automodule:: circuitpython_uplot.plot
     :members:
 
 .. automodule:: circuitpython_uplot.scatter
     :members:
```

### Comparing `circuitpython-uplot-1.0.1/docs/bar_example.jpg` & `circuitpython-uplot-1.1.1/docs/bar_example.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/docs/bar_palette.jpg` & `circuitpython-uplot-1.1.1/docs/bar_palette.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/docs/bar_scale.jpg` & `circuitpython-uplot-1.1.1/docs/bar_scale.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/docs/cartesian_trig_functions.jpg` & `circuitpython-uplot-1.1.1/docs/cartesian_trig_functions.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/docs/conf.py` & `circuitpython-uplot-1.1.1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 # Show the docstring from both the class and its __init__() method.
 autoclass_content = "both"
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 source_suffix = ".rst"
 master_doc = "index"
 # General information about the project.
-project = "CircuitPython uplot Library"
+project = "CircuitPython microplot Library"
 creation_year = "2023"
 current_year = str(datetime.datetime.now().year)
 year_duration = (
     current_year
     if current_year == creation_year
     else creation_year + " - " + current_year
 )
```

### Comparing `circuitpython-uplot-1.0.1/docs/examples.rst` & `circuitpython-uplot-1.1.1/docs/examples.rst`

 * *Files 18% similar despite different names*

```diff
@@ -10,149 +10,201 @@
 .. image:: ../docs/plot_simple_test.jpg
 
 Plot Example
 -------------
 
 Plot some data for x and y
 
-.. literalinclude:: ../examples/uplot_plot_example.py
-    :caption: examples/uplot_plot_example.py
+.. literalinclude:: ../examples/plot_example.py
+    :caption: examples/plot_example.py
     :lines: 5-
 
-.. image:: ../docs/uplot_ex4.jpg
+.. image:: ../docs/plot_example.jpg
 
 Tick Parameters Settings Example
 ----------------------------------
 
 Setting up the ticks parameters
 
-.. literalinclude:: ../examples/uplot_tickparameters.py
-    :caption: examples/uplot_tickparameters.py
+.. literalinclude:: ../examples/tickparameters.py
+    :caption: examples/tickparameters.py
     :lines: 5-
 
-.. image:: ../docs/uplot_ex3.jpg
+.. image:: ../docs/tickparameters.jpg
+
+Plot Line Style Example
+---------------------------
+
+Plot some data for x and y with different line styles
+
+.. literalinclude:: ../examples/plot_line_styles.py
+    :caption: examples/plot_line_styles.py
+    :lines: 5-
+.. image:: ../docs/line_style.jpg
 
 Integration Example
 -------------------
 
 Example showing different graphics elements integration
 
-.. literalinclude:: ../examples/uplot_integration_example.py
-    :caption: examples/uplot_integration_example.py
+.. literalinclude:: ../examples/integration_example.py
+    :caption: examples/integration_example.py
     :lines: 5-
-.. image:: ../docs/uplot_ex5.jpg
+.. image:: ../docs/integration_example.jpg
 
 Scatter Example
 -------------------
 
 Scatter plot Example
 
-.. literalinclude:: ../examples/uplot_scatter.py
-    :caption: examples/uplot_scatter.py
+.. literalinclude:: ../examples/scatter.py
+    :caption: examples/scatter.py
     :lines: 5-
 .. image:: ../docs/scatter.jpg
 
+Scatter Circle Pointers with diferent Radius
+---------------------------------------------
+
+Example showing how to use different radius in the circle pointers
+
+.. literalinclude:: ../examples/scatter_circle_radius.py
+    :caption: examples/scatter_circle_radius.py
+    :lines: 5-
+.. image:: ../docs/scatter_circle_radius.jpg
+
+Scatter Pointers Example
+----------------------------
+
+Example showing how to use different pointers
+
+.. literalinclude:: ../examples/scatter.py
+    :caption: examples/scatter.py
+    :lines: 5-
+.. image:: ../docs/scatter_pointers.jpg
+
+Scatter using different datasets
+----------------------------------
+
+Example showing how to use different datasets
+
+.. literalinclude:: ../examples/scatter.py
+    :caption: examples/scatter.py
+    :lines: 5-
+.. image:: ../docs/scatter_using_different_datasets.jpg
+
+
+Cartesian and Scatter Example
+------------------------------
+
+Example showing how to use cartesian and scatter in the same plot
+
+.. literalinclude:: ../examples/cartersian_and_scatter_polyfit_example.py
+    :caption: examples/cartersian_and_scatter_polyfit_example.py
+    :lines: 5-
+.. image:: ../docs/cartesian_scatter_polyfit.jpg
+
+
 Display_shapes Example
 -----------------------
 
 Display Shapes integration example
 
-.. literalinclude:: ../examples/uplot_display_shapes.py
-    :caption: examples/uplot_display_shapes.py
+.. literalinclude:: ../examples/display_shapes.py
+    :caption: examples/display_shapes.py
     :lines: 5-
-.. image:: ../docs/uplot_ex6.jpg
+.. image:: ../docs/display_shapes.jpg
 
 Bar Example
 ----------------
 
 Bar example
 
-.. literalinclude:: ../examples/uplot_bar_example.py
-    :caption: examples/uplot_bar_example.py
+.. literalinclude:: ../examples/bar_example.py
+    :caption: examples/bar_example.py
     :lines: 5-
 .. image:: ../docs/bar_example.jpg
 
 Bar Scale Example
 ---------------------
 
 Bar plot example showing how to use the scale
 
-.. literalinclude:: ../examples/uplot_bar_scale_example.py
-    :caption: examples/uplot_bar_scale_example.py
+.. literalinclude:: ../examples/bar_scale_example.py
+    :caption: examples/bar_scale_example.py
     :lines: 5-
 .. image:: ../docs/bar_scale.jpg
 
 
 Bar Color Palette Example
 ----------------------------
 
 Bar plot example showing how to pass a user color Palette
 
-.. literalinclude:: ../examples/uplot_bar_colorpalette.py
-    :caption: examples/uplot_bar_colorpalette.py
+.. literalinclude:: ../examples/bar_colorpalette.py
+    :caption: examples/bar_colorpalette.py
     :lines: 5-
 .. image:: ../docs/bar_palette.jpg
 
 
 Bar plot updating values Example
 ---------------------------------
 
 Bar Plot example showing how to update values for a filled bars bar plot
 
-.. literalinclude:: ../examples/uplot_bar_updating_values.py
-    :caption: examples/uplot_bar_updating_values.py
+.. literalinclude:: ../examples/bar_updating_values.py
+    :caption: examples/bar_updating_values.py
     :lines: 5-
 
 Bar plot updating bar colors Example
 -------------------------------------
 
 Bar Plot example showing how to update colors for a filled bars bar plot
 
-.. literalinclude:: ../examples/uplot_bar_color_changing.py
-    :caption: examples/uplot_bar_color_changing.py
+.. literalinclude:: ../examples/bar_color_changing.py
+    :caption: examples/bar_color_changing.py
     :lines: 5-
 
 
 Bar 3D Example
 ----------------
 
 Bar 3D example
 
-.. literalinclude:: ../examples/uplot_bar_3Dbars.py
-    :caption: examples/uplot_bar_3Dbars.py
+.. literalinclude:: ../examples/bar_3Dbars.py
+    :caption: examples/bar_3Dbars.py
     :lines: 5-
-.. image:: ../docs/uplot_3DBars.jpg
+.. image:: ../docs/3DBars.jpg
 
 Pie Example
 ----------------
 
 Pie example
 
-.. literalinclude:: ../examples/uplot_pie_example.py
-    :caption: examples/uplot_pie_example.py
+.. literalinclude:: ../examples/pie_example.py
+    :caption: examples/pie_example.py
     :lines: 5-
-.. image:: ../docs/uplot_pie.jpg
+.. image:: ../docs/pie.jpg
 
 Cartesian Advanced Example
 ---------------------------
 
 Showing the ability to display to graphs in the same plot with different colors
 
-.. literalinclude:: ../examples/uplot_cartesian_advanced.py
-    :caption: examples/uplot_cartesian_advanced.py
+.. literalinclude:: ../examples/cartesian_advanced.py
+    :caption: examples/cartesian_advanced.py
     :lines: 5-
-.. image:: ../docs/uplot_cartesian_advance.jpg
+.. image:: ../docs/cartesian_advance.jpg
 
 Cartesian Table Example
 ---------------------------
 
 Example showing how to add a data table to the plot
 
-.. literalinclude:: ../examples/uplot_cartesian_table.py
-    :caption: examples/uplot_cartesian_table.py
+.. literalinclude:: ../examples/cartesian_table.py
+    :caption: examples/cartesian_table.py
     :lines: 5-
 
 Lissajous Curves Example
 ---------------------------
 
 Example showing how to draw lissajous curves
 
@@ -162,16 +214,16 @@
 .. image:: ../docs/lissajous.jpg
 
 Cartesian Polar Plots Example
 --------------------------------
 
 Example showing how to draw polar plots using Cartesian
 
-.. literalinclude:: ../examples/uplot_polar_plots.py
-    :caption: examples/uplot_polar_plots.py
+.. literalinclude:: ../examples/polar_plots.py
+    :caption: examples/polar_plots.py
     :lines: 5-
 .. image:: ../docs/polar_plots.jpg
 
 Cartesian Trigonometric Plots Example
 --------------------------------------
 
 Example showing how to draw Trigonometrics plots using Cartesian
@@ -182,154 +234,164 @@
 .. image:: ../docs/cartesian_trig_functions.jpg
 
 Stackplot Example
 ---------------------------
 
 Stackplot simple example
 
-.. literalinclude:: ../examples/uplot_stackplot.py
-    :caption: examples/uplot_stackplot.py
+.. literalinclude:: ../examples/stackplot.py
+    :caption: examples/stackplot.py
     :lines: 8-
-.. image:: ../docs/uplot_ex12.jpg
+.. image:: ../docs/stackplot_example.jpg
 
 Advanced Example
 ---------------------------
 
 plot different ulements in a single display
 
-.. literalinclude:: ../examples/uplot_readme_example.py
-    :caption: examples/uplot_readme_example.py
+.. literalinclude:: ../examples/readme_example.py
+    :caption: examples/readme_example.py
     :lines: 5-
 .. image:: ../docs/readme.png
 
 Fillbetween Example
 ---------------------------
 
 Example of fillbetween plot
 
-.. literalinclude:: ../examples/uplot_fillbetween.py
-    :caption: examples/uplot_fillbetween.py
+.. literalinclude:: ../examples/fillbetween.py
+    :caption: examples/fillbetween.py
     :lines: 5-
 .. image:: ../docs/fillbetween_example.jpg
 
 Uboxplot Example
 ---------------------------
 
-example of uboxplot integration with uplot
+example of uboxplot integration in a plot
 
-.. literalinclude:: ../examples/uplot_uboxplot.py
-    :caption: examples/uplot_uboxplot.py
+.. literalinclude:: ../examples/uboxplot_example.py
+    :caption: examples/uboxplot_example.py
     :lines: 8-
-.. image:: ../docs/uplot_ex16.jpg
+.. image:: ../docs/uboxplot_example.jpg
 
 Map Example
 ---------------------------
 
 map simple example
 
-.. literalinclude:: ../examples/uplot_map.py
-    :caption: examples/uplot_map.py
+.. literalinclude:: ../examples/map.py
+    :caption: examples/map.py
     :lines: 5-
 .. image:: ../docs/map.jpg
 
 Sparkline Animation Example
 ---------------------------
 
 Sparkline animation example
 
-.. literalinclude:: ../examples/uplot_sparkline.py
-    :caption: examples/uplot_sparkline.py
+.. literalinclude:: ../examples/sparkline.py
+    :caption: examples/sparkline.py
     :lines: 5-
 
 Cartesian Animation Example
 ---------------------------
 
 Cartesian animation example
 
-.. literalinclude:: ../examples/uplot_cartesian_loggin_data.py
-    :caption: examples/uplot_cartesian_loggin_data.py
+.. literalinclude:: ../examples/cartesian_logging_data.py
+    :caption: examples/cartesian_logging_data.py
     :lines: 5-
-.. image:: ../docs/uplot_cartesian.gif
+.. image:: ../docs/cartesian_logging_data.gif
 
 Logging Example
 ---------------------------
 
 Logging example
 
-.. literalinclude:: ../examples/uplot_logging.py
-    :caption: examples/uplot_logging.py
+.. literalinclude:: ../examples/logging.py
+    :caption: examples/logging.py
     :lines: 5-
 
 Logging Fill Example
 ---------------------------
 
 Logging fill example
 
-.. literalinclude:: ../examples/uplot_logging_fill.py
-    :caption: examples/uplot_logging_fill.py
+.. literalinclude:: ../examples/logging_fill.py
+    :caption: examples/logging_fill.py
     :lines: 5-
 .. image:: ../docs/logging_fill.jpg
 
 
 Logging Changing Values Example
 ---------------------------------------
 
 This example shows how to redraw new_values in the same plot
 
-.. literalinclude:: ../examples/uplot_logging_changing_values.py
-    :caption: examples/uplot_logging_changing_values.py
+.. literalinclude:: ../examples/logging_changing_values.py
+    :caption: examples/logging_changing_values.py
     :lines: 5-
 
 Logging with Table Example
 ---------------------------------------
 
 This example shows how to add a data table to the plot
 
-.. literalinclude:: ../examples/uplot_logging_table.py
-    :caption: examples/uplot_logging_table.py
+.. literalinclude:: ../examples/logging_table.py
+    :caption: examples/logging_table.py
     :lines: 10-
 .. image:: ../docs/logging_table.jpg
 
 
 Logging Animation Example
 ---------------------------------------
 
 This example shows how to animate a plot
 
-.. literalinclude:: ../examples/uplot_logging_animation.py
-    :caption: examples/uplot_logging_animation.py
+.. literalinclude:: ../examples/logging_animation.py
+    :caption: examples/logging_animation.py
+    :lines: 5-
+
+Logging Animation Example
+---------------------------------------
+
+This example shows how to add limits to our plot
+
+.. literalinclude:: ../examples/logging_limits.py
+    :caption: examples/logging_limits.py
     :lines: 5-
+.. image:: ../docs/logging_limits.jpg
 
 SVG Images examples
 ---------------------------
 
 SVG Images example
 
-.. literalinclude:: ../examples/uplot_svg_example.py
-    :caption: examples/uplot_svg_example.py
+.. literalinclude:: ../examples/svg_example.py
+    :caption: examples/svg_example.py
     :lines: 5-
-.. image:: ../docs/uplot_svg.jpg
+.. image:: ../docs/svg.jpg
 
 Shade examples
 ---------------------------
 
 Shade example
 
-.. literalinclude:: ../examples/uplot_shade_example.py
-    :caption: examples/uplot_shade_example.py
+.. literalinclude:: ../examples/shade_example.py
+    :caption: examples/shade_example.py
     :lines: 5-
-.. image:: ../docs/uplot_shade.jpg
+.. image:: ../docs/shade.jpg
 
 Polar example
 ---------------------------
 
 Show how to use the Polar Plot
 
-.. literalinclude:: ../examples/uplot_polar_example.py
-    :caption: examples/uplot_polar_example.py
+.. literalinclude:: ../examples/polar_example.py
+    :caption: examples/polar_example.py
     :lines: 5-
 .. image:: ../docs/polar_example.jpg
 
 Polar Advanced Example
 ---------------------------
 
 Polar Advanced example
```

### Comparing `circuitpython-uplot-1.0.1/docs/fillbetween_example.jpg` & `circuitpython-uplot-1.1.1/docs/fillbetween_example.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/docs/index.rst` & `circuitpython-uplot-1.1.1/docs/index.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 :orphan:
 
-.. title:: uplot documentation
+.. title:: microplot documentation
 
 .. module:: uplot
 
-###################
-uplot documentation
-###################
+#########################
+Microplot documentation
+#########################
 
 Framework to display different plots in displayio. Similar to widget
 Take a look in the `examples <https://circuitpython-uplot.readthedocs.io/en/latest/examples.html>`_ section in RTD to see the gallery
 
-uplot is to be used with CircuitPython as some of the behind the curtains methods are
+microplot is to be used with CircuitPython as some of the behind the curtains methods are
 in the CircuitPython core and could differ from MicroPython or Python
 
 
 Quick Start
 ==============
 
 .. include:: ../docs/quick_start.rst
```

### Comparing `circuitpython-uplot-1.0.1/docs/lissajous.jpg` & `circuitpython-uplot-1.1.1/docs/lissajous.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/docs/logging.png` & `circuitpython-uplot-1.1.1/docs/logging.png`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/docs/logging_fill.jpg` & `circuitpython-uplot-1.1.1/docs/logging_fill.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/docs/logging_table.jpg` & `circuitpython-uplot-1.1.1/docs/logging_table.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/docs/map.jpg` & `circuitpython-uplot-1.1.1/docs/map.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/docs/plot_simple_test.jpg` & `circuitpython-uplot-1.1.1/docs/plot_simple_test.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/docs/polar_advanced.jpg` & `circuitpython-uplot-1.1.1/docs/polar_advanced.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/docs/polar_example.jpg` & `circuitpython-uplot-1.1.1/docs/polar_example.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/docs/polar_plots.jpg` & `circuitpython-uplot-1.1.1/docs/polar_plots.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/docs/quick_start.rst` & `circuitpython-uplot-1.1.1/docs/quick_start.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-A small tour for uplot.
+A small tour for microplot.
 
 
 Plot Usage
 =============
 We start importing some fundamental libraries for plot to operate
 
+
 .. code-block:: python
 
     import board
     import displayio
     from circuitpython_uplot.plot import Plot
 
 For reference, screen in CircuitPython are defined from left to right and up to bottom. This means
@@ -61,14 +62,17 @@
 * Elements in the library
     * Cartesian Plane
     * Fillbetween graph
     * Stackplot
     * Bar graph
     * Pie Chart
     * Colormap
+    * Polar graph
+    * SVG Rudimentary support
+    * Logging graph
 * Display_shapes library objects
 * Histograms from the uhistogram library
 * Boxplots from the uboxplot library
 * Individual Vectorio Objects
 
 In a more advanced method it is possible to add directly to the plot area using the plot bitmap object
 
@@ -110,33 +114,51 @@
 
     plot = Plot(0, 0, display.width, display.height)
     plot.axs_params(axstype="cartesian")
 
 Tick spacing and numbers are selected by default. However it's possible to customize
 the following parameters:
 
-.. py:function:: Plot.tick_params(tickx_height, ticky_height, tickcolor, tickgrid)
+.. py:function:: Plot.tick_params(showtick, tickx_height, ticky_height, tickcolor, tickgrid, showtext, decimal_points)
 
+   :param bool showtick: displays the tick. Defaults to `True`
    :param int tickx_height: tickx_height in pixels
    :param int ticky_height: ticky_height in pixels
    :param int tickcolor: tickcolor in Hex format
    :param bool tickgrid: displays the tickgrid. Defaults to `False`
+   :param bool showtext: displays the tick text. Defaults to `False`
+   :param int decimal_points: number of decimal points to show. Defaults to :const:`0`
+
 
 .. code-block:: python
 
     plot.tick_params(tickx_height=12, tickcolor=0xFF0008)
 
 
 Gridlines are normally ``OFF``. If you want visible gridlines then use:
 
 .. code-block:: python
 
     plot.tick_params(tickgrid=True)
 
 
+If you want to show the axes text. You can use:
+
+.. code-block:: python
+
+    plot.tick_params(showtext=True)
+
+If you want to show some decimal places in the text. use:
+
+.. code-block:: python
+
+    plot.tick_params(decimal_points=2)
+
+
+
 Colors
 ===============
 You can choose some colors directly from the library. This can be done by importing the color class:
 
 .. code-block:: python
 
     from circuitpython_uplot.plot import color
@@ -260,26 +282,26 @@
     a = np.linspace(1, 100)
     b = [choice(a) for _ in a]
     Scatter(plot, a, b)
 
 
 There are some parameters that you can customize:
     * rangex and rangey: you can specify the ranges of your graph. This allows you to move your graph according to your needs. This parameters only accept lists
-    * radius: circles radius/radii
-    * circle_color: you can specify the color in HEX
+    * radius: circles radius/radii. If a different value is given for each point, the radius should be a list of values. If selected pointer is not a circle, this parameter will be ignored
+    * pointer_color: you can specify the color in HEX
     * nudge: this parameter allows you to move the graph slighty. This is useful when the data start/end in the limits of your range
 
 
 .. code-block:: python
 
     a = np.linspace(1, 200, 150)
     z = [4, 5, 6, 7, 8]
     radi = [choice(z) for _ in a]
     b = [choice(a) for _ in a]
-    Scatter(plot, a, b, rangex=[0,210], rangey=[0, 210], radius=radi, circle_color=0xF456F3)
+    Scatter(plot, a, b, rangex=[0,210], rangey=[0, 210], radius=radi, pointer_color=0xF456F3)
 
 ===============
 Bar Plot
 ===============
 
 Allows you to graph bar plots. You just need to give the values of the bar in a python list.
 You can choose to create shell or filled bars.
```

### Comparing `circuitpython-uplot-1.0.1/docs/readme.png` & `circuitpython-uplot-1.1.1/docs/readme.png`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/docs/readme2.png` & `circuitpython-uplot-1.1.1/docs/readme2.png`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/docs/scatter.jpg` & `circuitpython-uplot-1.1.1/docs/scatter.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/docs/uplot_3DBars.jpg` & `circuitpython-uplot-1.1.1/docs/3DBars.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/docs/uplot_cartesian.gif` & `circuitpython-uplot-1.1.1/docs/cartesian_logging_data.gif`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/docs/uplot_cartesian_advance.jpg` & `circuitpython-uplot-1.1.1/docs/cartesian_advance.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/docs/uplot_ex12.jpg` & `circuitpython-uplot-1.1.1/docs/stackplot_example.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/docs/uplot_ex16.jpg` & `circuitpython-uplot-1.1.1/docs/uboxplot_example.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/docs/uplot_ex3.jpg` & `circuitpython-uplot-1.1.1/docs/tickparameters.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/docs/uplot_ex4.jpg` & `circuitpython-uplot-1.1.1/docs/plot_example.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/docs/uplot_ex5.jpg` & `circuitpython-uplot-1.1.1/docs/integration_example.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/docs/uplot_ex6.jpg` & `circuitpython-uplot-1.1.1/docs/display_shapes.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/docs/uplot_pie.jpg` & `circuitpython-uplot-1.1.1/docs/pie.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/docs/uplot_shade.jpg` & `circuitpython-uplot-1.1.1/docs/shade.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/docs/uplot_svg.jpg` & `circuitpython-uplot-1.1.1/docs/svg.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/examples/cartesian_trig_functions.py` & `circuitpython-uplot-1.1.1/examples/cartesian_trig_functions.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/examples/fonts/LeagueSpartan-Bold-16.bdf` & `circuitpython-uplot-1.1.1/examples/fonts/LeagueSpartan-Bold-16.bdf`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/examples/fonts/LibreBodoniv2002-Bold-10.bdf` & `circuitpython-uplot-1.1.1/examples/fonts/LibreBodoniv2002-Bold-10.bdf`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/examples/fonts/LibreBodoniv2002-Regular-17.bdf` & `circuitpython-uplot-1.1.1/examples/fonts/LibreBodoniv2002-Regular-17.bdf`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/examples/fonts/forkawesome-36.pcf` & `circuitpython-uplot-1.1.1/examples/fonts/forkawesome-36.pcf`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/examples/lissajous_curves.py` & `circuitpython-uplot-1.1.1/examples/lissajous_curves.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/examples/polar_advanced.py` & `circuitpython-uplot-1.1.1/examples/polar_advanced.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/examples/uplot_bar_3Dbars.py` & `circuitpython-uplot-1.1.1/examples/bar_3Dbars.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/examples/uplot_bar_color_changing.py` & `circuitpython-uplot-1.1.1/examples/bar_color_changing.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/examples/uplot_bar_colorpalette.py` & `circuitpython-uplot-1.1.1/examples/bar_colorpalette.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/examples/uplot_bar_example.py` & `circuitpython-uplot-1.1.1/examples/bar_example.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/examples/uplot_bar_scale_example.py` & `circuitpython-uplot-1.1.1/examples/bar_scale_example.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/examples/uplot_bar_updating_values.py` & `circuitpython-uplot-1.1.1/examples/bar_updating_values.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/examples/uplot_cartesian_advanced.py` & `circuitpython-uplot-1.1.1/examples/cartesian_advanced.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/examples/uplot_cartesian_loggin_data.py` & `circuitpython-uplot-1.1.1/examples/cartesian_logging_data.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/examples/uplot_cartesian_table.py` & `circuitpython-uplot-1.1.1/examples/cartesian_table.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/examples/uplot_display_shapes.py` & `circuitpython-uplot-1.1.1/examples/display_shapes.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/examples/uplot_fillbetween.py` & `circuitpython-uplot-1.1.1/examples/fillbetween.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/examples/uplot_integration_example.py` & `circuitpython-uplot-1.1.1/examples/integration_example.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/examples/uplot_logging.py` & `circuitpython-uplot-1.1.1/examples/logging.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/examples/uplot_logging_animation.py` & `circuitpython-uplot-1.1.1/examples/logging_animation.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/examples/uplot_logging_changing_values.py` & `circuitpython-uplot-1.1.1/examples/logging_changing_values.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/examples/uplot_logging_fill.py` & `circuitpython-uplot-1.1.1/examples/logging_fill.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/examples/uplot_logging_table.py` & `circuitpython-uplot-1.1.1/examples/logging_table.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/examples/uplot_map.py` & `circuitpython-uplot-1.1.1/examples/map.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/examples/uplot_plot_example.py` & `circuitpython-uplot-1.1.1/examples/plot_example.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/examples/uplot_polar_example.py` & `circuitpython-uplot-1.1.1/examples/polar_example.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/examples/uplot_polar_plots.py` & `circuitpython-uplot-1.1.1/examples/polar_plots.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/examples/uplot_readme_example.py` & `circuitpython-uplot-1.1.1/examples/readme_example.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/examples/uplot_scatter.py` & `circuitpython-uplot-1.1.1/examples/scatter.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/examples/uplot_shade_example.py` & `circuitpython-uplot-1.1.1/examples/shade_example.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/examples/uplot_sparkline.py` & `circuitpython-uplot-1.1.1/examples/sparkline.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/examples/uplot_stackplot.py` & `circuitpython-uplot-1.1.1/examples/stackplot.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/examples/uplot_svg_example.py` & `circuitpython-uplot-1.1.1/examples/svg_example.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/examples/uplot_tickparameters.py` & `circuitpython-uplot-1.1.1/examples/tickparameters.py`

 * *Files identical despite different names*

### Comparing `circuitpython-uplot-1.0.1/examples/uplot_uboxplot.py` & `circuitpython-uplot-1.1.1/examples/uboxplot_example.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 """
 Simple test to display boxplot using plot
 """
 
 import board
-from uboxplot import Boxplot
+from examples.uboxplot_example import Boxplot
 from circuitpython_uplot.plot import Plot
 
 
 display = board.DISPLAY
 
 plot = Plot(0, 0, display.width, display.height)
```

### Comparing `circuitpython-uplot-1.0.1/pyproject.toml` & `circuitpython-uplot-1.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-uplot"
 description = "framework to display different plots in displayio. similar to widget"
-version = "1.0.1"
+version = "1.1.1"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "uplot@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/CircuitPython_uplot"}
 keywords = [
     "circuitpython",
```

